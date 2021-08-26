---
title: Instrumentieren eines Viewers mit dem Adobe Analytics Instrumentation Kit
description: Erfahren Sie, wie Sie einen Viewer mit dem Adobe Analytics Instrumentation Kit in Dynamic Media Classic instrumentieren.
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
source-git-commit: bb387446f294cf1e90d26ae1df4422879ad29db7
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 20%

---

# Instrumentieren eines Viewers mit dem Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Sie können das Adobe Analytics Instrumentation Kit verwenden, um einen HTML5-Viewer in Adobe Analytics zu integrieren.

Wenn Sie eine der vordefinierten HTML5-Viewer-Vorgaben von Dynamic Media Classic verwenden, enthalten diese bereits den gesamten Implementierungscode zum Senden von Daten an Adobe Analytics. Sie benötigen keine weitere Instrumentierung.

## Einrichten des Adobe Analytics-Trackings über Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Fügen Sie für alle HTML5-Viewer das folgende JavaScript zum HTML-Container hinzu, normalerweise im &lt;head> -Element:

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Dabei ist `Dynamic Media Classic Company ID` auf den Unternehmensnamen von Dynamic Media Classic festgelegt. Und `&preset` ist optional, es sei denn, der Unternehmensvorgabenname ist nicht `companypreset`. In solchen Fällen könnte es `companypreset-1, companypreset-2` sein usw. Die höhere Zahl bedeutet eine neure Instanz der Vorgabe. Um den richtigen Namen für den Unternehmensvorgabenwert zu ermitteln, wählen Sie **[!UICONTROL URL kopieren]** und dann den Parameter `preset=`aus, um den Unternehmensvorgabennamen zu finden.

Fügen Sie nun eine Funktion hinzu, die das Viewer-Ereignis an den Adobe Analytics-Trackingcode sendet.

Fügen Sie die Funktion `s7ComponentEvent()` zum Container-HTML (oder JSP, ASPX oder anderen) hinzu:

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Beim Funktionsnamen wird zwischen Groß- und Kleinschreibung unterschieden. Der einzige Parameter, der an `s7componentEvent`übergeben wird und erforderlich ist, ist der letzte: `eventData`. Wobei `s7track()` in s_code.jsp definiert ist, die oben aufgeführt sind. Und `s7track` verarbeitet das gesamte Tracking pro Ereignis. (Wenn Sie an Adobe Analytics übermittelte Daten weiter anpassen müssen, sollten Sie dies an dieser Stelle tun.)

## Aktivieren von HREF- und ITEM-Ereignissen {#enabling-href-and-item-events}

Sie können HREF-Ereignisse (Rollover) und ITEM-Ereignisse (Mausklicks/Berührungen) in den Viewern aktivieren, indem Sie die Imagemap bearbeiten. Definieren Sie die Identifikatoren für HREF und ITEM in der mit dem Viewer-Inhalt verknüpften Imagemap. Fügen Sie dem HREF-Wert in der Imagemap den Parameter `&rolloverKey=` hinzu.
