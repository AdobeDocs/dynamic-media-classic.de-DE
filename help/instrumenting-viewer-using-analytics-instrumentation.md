---
title: Instrumentieren eines Viewers mit dem Adobe Analytics-Instrumentierungskit
seo-title: Instrumentieren eines Viewers mit dem Adobe Analytics-Instrumentierungskit
description: 'null'
seo-description: Erfahren Sie, wie Sie einen Viewer mit dem Adobe Analytics Instrumentation Kit instrumentieren.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 41%

---


# Instrumentieren eines Viewers mit dem Adobe Analytics-Instrumentierungskit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Sie können das Adobe Analytics Instrumentation Kit verwenden, um einen HTML5-Viewer in Adobe Analytics zu integrieren.

Wenn Sie eine der vordefinierten HTML5-Viewer-Vorgaben von Dynamic Media Classic verwenden, beachten Sie, dass diese bereits den Implementierungscode enthalten, der zum Senden von Daten an Adobe Analytics erforderlich ist. Eine weitere Instrumentierung ist nicht erforderlich.

## Einrichten der Adobe Analytics-Verfolgung von Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Fügen Sie für alle HTML5-Viewer dem HTML-Container das folgende JavaScript hinzu, normalerweise im Element &lt;head>:

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

`Company` auf den Namen der Dynamic Media Classic-Firma festgelegt ist. `&preset` ist optional, es sei denn, der Unternehmensvorgabenname ist nicht `companypreset`. In such cases, it could be `companypreset-1, companypreset-2`, and so on. Die höhere Zahl bedeutet eine neure Instanz der Vorgabe. To determine the correct company preset value name, click **Copy URL** , and then look at the `preset=`parameter to find the company preset name.

Anschließend fügen Sie eine Funktion hinzu, die das Viewer-Ereignis an den Adobe Analytics-Rückverfolgungscode sendet.

Add the `s7ComponentEvent()` function to the container HTML (or JSP, or ASPX or other):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Beachten Sie beim Funktionsnamen die Groß-/Kleinschreibung. The only parameter passed to `s7componentEvent`that is required is the last one: `eventData`. `s7track()` ist in s_code.jsp definiert, die oben aufgeführt sind. `s7track` verarbeitet die gesamte Verfolgung pro Ereignis. (Wenn Sie an Adobe Analytics übermittelte Daten weiter anpassen müssen, sollten Sie dies an dieser Stelle tun.)

## Aktivieren von HREF- und ITEM-Ereignissen {#enabling-href-and-item-events}

Sie können HREF-Ereignisse (Rollover) und ITEM-Ereignisse (Mausklicks/Berührungen) in den Viewern aktivieren, indem Sie die Imagemap bearbeiten. Definieren Sie die Identifikatoren für HREF und ITEM in der mit dem Viewer-Inhalt verknüpften Imagemap. Add a `&rolloverKey=` parameter to the HREF value within the Image Map.
