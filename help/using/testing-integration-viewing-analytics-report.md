---
title: Testen der Integration durch Anzeigen eines Adobe Analytics-Berichts
description: Erfahren Sie, wie Sie die Integration in Adobe Dynamic Media Classic testen können, indem Sie sich einen Adobe Analytics-Bericht ansehen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
topic: Integrations, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 5%

---

# Testen der Integration durch Anzeigen eines Adobe Analytics-Berichts{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Nachdem Sie die erforderlichen Variablen in Adobe Analytics erstellt, mit Adobe Dynamic Media Classic-Ereignissen verknüpft und die erforderlichen Implementierungsschritte abgeschlossen haben, können Sie die Einrichtung testen. Sie können testen und überprüfen, ob die Daten in Adobe Analytics selbst erfasst werden. Wenn das Setup hier funktioniert, sind keine weiteren Schritte nötig. Wenn Sie die oben genannten Schritte ausgeführt und Ihre Adobe Dynamic Media Classic-Ereignisdaten mit einer oder mehreren Custom Traffic-Variablen verknüpft haben, befolgen Sie diesen Workflow, um Ihre Daten in Adobe Analytics zu testen.

**So testen Sie die Integration durch Anzeigen eines Adobe Analytics-Berichts:**

1. Starten Sie einen Adobe Dynamic Media Classic-Viewer über Ihr Konto, insbesondere einen, der die Metrik sendet, die Sie erhalten möchten, und interagieren Sie mit ihm, um Ereignisdaten zu erstellen.

   Wenn Sie beispielsweise beliebte alternative Ansichten in einem Bildset messen möchten, zeigen Sie eine Vorschau eines Bildsets an und klicken Sie auf die verschiedenen Miniaturen.

1. Navigieren Sie in Adobe Analytics zu **[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > [Name der Prop] und wählen Sie Ihren Traffic-Prop-Namen aus den Menüoptionen aus.

   Um beispielsweise auf die Prop **[!UICONTROL LoadAsset]** im Beispielkonto zuzugreifen, lautet die richtige Menüauswahl **[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > **[!UICONTROL LoadAsset]**. Wenn Sie mehr als zehn benutzerdefinierte Eigenschaften haben, sehen Sie auch andere Menüoptionen.

1. Zeigen Sie das von Adobe Analytics erstellte Diagramm an. Dieses Diagramm enthält normalerweise nur die Daten für eine einzelne Metrik. Wenn Sie auch wissen möchten, mit welchem Asset diese Daten verknüpft sind, rufen Sie die Asset-Daten dieses Ereignisses ab. Beispielsweise ist es oft nützlich zu wissen, welches Video nur zu 50 % angesehen wird oder welches Bild in einem Set beliebt ist.

>[!NOTE]
>
>Alle Adobe Dynamic Media Classic-Viewer-Daten werden in Custom Traffic-Berichten oder Custom Conversion-Berichten von Adobe Analytics angezeigt und gemeldet.

Weitere Informationen finden Sie unter [Analytics-Tutorials](https://experienceleague.adobe.com/de/docs/analytics-learn/tutorials/overview).