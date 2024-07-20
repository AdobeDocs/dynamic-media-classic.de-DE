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
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 15%

---

# Instrumentieren eines Viewers mit dem Adobe Analytics Instrumentation Kit{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Mit dem Adobe Analytics Instrumentation Kit können Sie einen HTML5-Viewer in Adobe Analytics integrieren.

Wenn Sie eine der vordefinierten Adobe Dynamic Media Classic HTML5 Viewer-Vorgaben verwenden, enthalten diese bereits den gesamten Implementierungscode zum Senden von Daten an Adobe Analytics. Sie müssen keine weitere Instrumentierung hinzufügen.

## Einrichten von Adobe Analytics-Tracking über Adobe Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

Fügen Sie für alle HTML5-Viewer den HTML-Container die folgende JavaScript hinzu, normalerweise im Element &lt;head> :

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

Wobei `Adobe Dynamic Media Classic Company ID` auf den Adobe Dynamic Media Classic-Unternehmensnamen festgelegt ist. Und `&preset` ist optional. Wenn der Name der Unternehmensvorgabe nicht `companypreset` ist, ist er nicht optional. In solchen Fällen könnte es `companypreset-1, companypreset-2` sein usw. Die höhere Zahl bedeutet eine neure Instanz der Vorgabe. Um den richtigen Namen für den Unternehmensvorgabenwert zu ermitteln, wählen Sie **[!UICONTROL URL kopieren]** und suchen Sie dann den Parameter `preset=` , um den Unternehmensvorgabennamen zu finden.

Fügen Sie nun eine Funktion hinzu, die das Viewer-Ereignis an den Adobe Analytics-Trackingcode sendet.

Fügen Sie die Funktion `s7ComponentEvent()` zum Container-HTML (oder JSP, ASPX oder anderen) hinzu:

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

Beim Funktionsnamen wird zwischen Groß- und Kleinschreibung unterschieden. Der einzige Parameter, der an `s7componentEvent`übergeben wird und erforderlich ist, ist der letzte: `eventData`. Wobei `s7track()` in s_code.jsp definiert ist, die oben enthalten sind. Und `s7track` verarbeitet das gesamte Tracking pro Ereignis. (In diesem Bereich können Sie die an Adobe Analytics übermittelten Daten weiter anpassen.)

## HREF- und ITEM-Ereignisse aktivieren {#enabling-href-and-item-events}

Sie können HREF-Ereignisse (Rollover) und ITEM-Ereignisse (Mausklicks/Berührungen) in den Viewern aktivieren, indem Sie die Imagemap bearbeiten. Definieren Sie die Identifikatoren für HREF und ITEM in der mit dem Viewer-Inhalt verknüpften Imagemap. Fügen Sie dem HREF-Wert in der Imagemap den Parameter `&rolloverKey=` hinzu.
