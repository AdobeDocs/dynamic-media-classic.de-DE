---
title: Instrumentieren eines Viewers mit dem Adobe Analytics Instrumentation Kit
description: Erfahren Sie, wie Sie einen Viewer mit dem Adobe Analytics Instrumentation Kit in Adobe Dynamic Media Classic instrumentieren.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
topic: Integrations, Development
level: Experienced
source-git-commit: 163eb32112ec6fbefd1dacf48212353ff3053d54
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 15%

---

# Instrumentieren eines Viewers mit dem Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Mit dem Adobe Analytics Instrumentation Kit können Sie einen HTML5-Viewer in Adobe Analytics integrieren.

Wenn Sie eine der vordefinierten Adobe Dynamic Media Classic HTML5-Viewer-Vorgaben verwenden, enthalten diese bereits den gesamten Implementierungscode zum Senden von Daten an Adobe Analytics. Sie müssen keine weitere Instrumentierung hinzufügen.

## Einrichten von Adobe Analytics-Tracking über Adobe Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Fügen Sie für alle HTML5-Viewer das folgende JavaScript zum HTML-Container hinzu, normalerweise im &lt;head> element:

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Wo `Adobe Dynamic Media Classic Company ID` auf den Adobe Dynamic Media Classic-Unternehmensnamen festgelegt ist. und `&preset` ist optional. Wenn der Vorgabenname des Unternehmens nicht `companypreset`festgelegt ist, ist dies nicht optional. In solchen Fällen kann es `companypreset-1, companypreset-2`usw. Die höhere Zahl bedeutet eine neure Instanz der Vorgabe. Um den richtigen Namen für die Unternehmensvorgabe zu bestimmen, wählen Sie **[!UICONTROL URL kopieren]**, und sehen Sie sich dann die `preset=`-Parameter, um den Unternehmensvorgabennamen zu finden.

Fügen Sie nun eine Funktion hinzu, die das Viewer-Ereignis an den Adobe Analytics-Trackingcode sendet.

Fügen Sie die `s7ComponentEvent()` -Funktion auf die Container-HTML (oder JSP, ASPX oder andere):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Beim Funktionsnamen wird zwischen Groß- und Kleinschreibung unterschieden. Der einzige Parameter, der an `s7componentEvent`erforderlich ist der letzte: `eventData`. Wo `s7track()` ist in s_code.jsp definiert, die oben enthalten ist. und `s7track` verarbeitet das gesamte Tracking pro Ereignis. (In diesem Bereich können Sie die an Adobe Analytics übermittelten Daten weiter anpassen.)

## HREF- und ITEM-Ereignisse aktivieren {#enabling-href-and-item-events}

Sie können HREF-Ereignisse (Rollover) und ITEM-Ereignisse (Mausklicks/Berührungen) in den Viewern aktivieren, indem Sie die Imagemap bearbeiten. Definieren Sie die Identifikatoren für HREF und ITEM in der mit dem Viewer-Inhalt verknüpften Imagemap. Hinzufügen einer `&rolloverKey=` zum HREF-Wert in der Imagemap.
