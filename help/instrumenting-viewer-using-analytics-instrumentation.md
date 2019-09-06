---
title: Instrumentieren eines Viewers mit dem Adobe Analytics-Instrumentierungskit
seo-title: Instrumentieren eines Viewers mit dem Adobe Analytics-Instrumentierungskit
description: 'null'
seo-description: Erfahren Sie, wie Sie einen Viewer mit dem Adobe Analytics-Instrumentierungskit instrumentieren.
uuid: cf 9 a 4002-966 d -4641-9 cd 0-2 ee 8 b 5454 f 60
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: a 2824244-1755-42 de-a 167-42 af 117 cf 038
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Instrumentieren eines Viewers mit dem Adobe Analytics-Instrumentierungskit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Sie können das Adobe Analytics-Instrumentierungskit verwenden, um einen HTML 5-Viewer in Adobe Analytics zu integrieren.

Wenn Sie eine der vordefinierten HTML 5-Viewer-Vorgaben für dynamische Medien verwenden, beachten Sie, dass sie bereits den gesamten Implementierungscode enthalten, der zum Senden von Daten an Adobe Analytics benötigt wird. —Es ist keine weitere Instrumentierung erforderlich.

## Richten Sie die Adobe Analytics-Nachverfolgung im Scene7 Publishing System ein.{#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Fügen Sie für alle HTML 5-Viewer dem HTML-Container das folgende javascript hinzu, normalerweise im &lt; head &gt;-Element:

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<SPS Company ID>&preset=companypreset-1"></script>
```

`Company` wird auf den SPS-Unternehmensnamen gesetzt. `&preset` ist optional, es sei denn, der Unternehmensvorgabenname ist nicht `companypreset`. In such cases, it could be `companypreset-1, companypreset-2`, and so on. Die höhere Zahl bedeutet eine neure Instanz der Vorgabe. To determine the correct company preset value name, click **Copy URL** , and then look at the `preset=`parameter to find the company preset name.

Anschließend fügen Sie eine Funktion hinzu, die das Viewer-Ereignis an den Adobe Analytics-Rückverfolgungscode sendet.

Add the `s7ComponentEvent()` function to the container HTML (or JSP, or ASPX or other):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Beachten Sie beim Funktionsnamen die Groß-/Kleinschreibung. The only parameter passed to `s7componentEvent`that is required is the last one: `eventData`. `s7track()` in "s_ code. jsp" definiert ist. `s7track` verarbeitet alle Verfolgung pro Ereignis. (Wenn Sie an Adobe Analytics übermittelte Daten weiter anpassen müssen, sollten Sie dies an dieser Stelle tun.)

## Aktivieren von HREF- und ITEM-Ereignissen {#enabling-href-and-item-events}

Sie können HREF-Ereignisse (Rollover) und ITEM-Ereignisse (Mausklicks/Berührungen) in den Viewern aktivieren, indem Sie die Imagemap bearbeiten. Definieren Sie die Identifikatoren für HREF und ITEM in der mit dem Viewer-Inhalt verknüpften Imagemap. Add a `&rolloverKey=` parameter to the HREF value within the Image Map.
