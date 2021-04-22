---
title: Instrumentieren eines Viewers mit dem Adobe Analytics-Instrumentierungskit
description: Erfahren Sie, wie Sie einen Viewer mit dem Adobe Analytics Instrumentation Kit instrumentieren.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
translation-type: tm+mt
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 28%

---

# Instrumentieren eines Viewers mit dem Adobe Analytics-Instrumentierungskit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Sie können das Adobe Analytics Instrumentation Kit verwenden, um einen HTML5-Viewer in Adobe Analytics zu integrieren.

Wenn Sie eine der vordefinierten Dynamic Media Classic HTML5-Viewer-Vorgaben verwenden, enthalten diese bereits den gesamten Implementierungscode zum Senden von Daten an Adobe Analytics; Sie benötigen keine weitere Instrumentierung.

## Einrichten der Adobe Analytics-Verfolgung von Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Fügen Sie für alle HTML5-Viewer dem HTML-Container den folgenden JavaScript™-Code hinzu, üblicherweise im Element &lt;head>:

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Dabei ist `Dynamic Media Classic Company ID` auf den Namen der Dynamic Media Classic-Firma eingestellt. Und `&preset` ist optional, es sei denn, der Vorgabenname der Firma ist nicht `companypreset`. In solchen Fällen könnte es `companypreset-1, companypreset-2` sein usw. Die höhere Zahl bedeutet eine neure Instanz der Vorgabe. Um den richtigen Vorgabenamen für die Firma zu ermitteln, klicken Sie auf **[!UICONTROL URL kopieren]** und suchen Sie dann den `preset=`Parameter, um den Vorgabennamen für die Firma zu finden.

Fügen Sie nun eine Funktion hinzu, die das Viewer-Ereignis an den Adobe Analytics-Trackingcode sendet.

hinzufügen Sie die Funktion `s7ComponentEvent()` auf den Container HTML (oder JSP oder ASPX oder andere):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Beim Funktionsnamen wird die Groß-/Kleinschreibung beachtet. Der einzige Parameter, der an `s7componentEvent`weitergeleitet wird und erforderlich ist, ist der letzte: `eventData`. Dabei ist `s7track()` in s_code.jsp definiert, die oben aufgeführt sind. Und `s7track` verarbeitet alle Verfolgungen pro Ereignis. (Wenn Sie an Adobe Analytics übermittelte Daten weiter anpassen müssen, sollten Sie dies an dieser Stelle tun.)

## Aktivieren von HREF- und ITEM-Ereignissen  {#enabling-href-and-item-events}

Sie können HREF-Ereignisse (Rollover) und ITEM-Ereignisse (Mausklicks/Berührungen) in den Viewern aktivieren, indem Sie die Imagemap bearbeiten. Definieren Sie die Identifikatoren für HREF und ITEM in der mit dem Viewer-Inhalt verknüpften Imagemap. hinzufügen Sie den HREF-Wert in der Imagemap mit dem Parameter `&rolloverKey=`.
