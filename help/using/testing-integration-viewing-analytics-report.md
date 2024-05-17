---
title: Integration durch Anzeigen eines Adobe Analytics-Berichts testen
description: Erfahren Sie, wie Sie die Integration in Adobe Dynamic Media Classic testen können, indem Sie einen Adobe Analytics-Bericht anzeigen.
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

# Integration durch Anzeigen eines Adobe Analytics-Berichts testen{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Nachdem Sie die erforderlichen Variablen in Adobe Analytics erstellt, mit Adobe Dynamic Media Classic-Ereignissen verknüpft und die erforderlichen Implementierungsschritte ausgeführt haben, können Sie die Einrichtung testen. Sie können testen und überprüfen, ob die Daten in Adobe Analytics selbst erfasst werden. Wenn das Setup hier funktioniert, sind keine weiteren Schritte nötig. Wenn Sie die oben genannten Schritte ausgeführt und Ihre Adobe Dynamic Media Classic-Ereignisdaten mit einer oder mehreren benutzerspezifischen Traffic-Variablen verknüpft haben, führen Sie diesen Workflow aus, um Ihre Daten in Adobe Analytics zu testen.

**So testen Sie die Integration durch Anzeigen eines Adobe Analytics-Berichts:**

1. Starten Sie einen Adobe Dynamic Media Classic-Viewer von Ihrem Konto aus, insbesondere einen, der die gewünschte Metrik sendet, und interagieren Sie mit ihm, um einige Ereignisdaten zu erstellen.

   Wenn Sie beispielsweise beliebte alternative Ansichten in einem Bildset messen möchten, zeigen Sie eine Vorschau eines Bildsets an und klicken Sie auf die verschiedenen Miniaturansichten.

1. Gehen Sie innerhalb von Adobe Analytics zu **[!UICONTROL Benutzerspezifischer Traffic]** > **[!UICONTROL Benutzerspezifischer Traffic 1-10]** > [Name der Prop], indem Sie Ihren Traffic-Eigenschaftsnamen aus den Menüoptionen auswählen.

   Um beispielsweise auf die **[!UICONTROL LoadAsset]** prop im Beispielkonto, ist die richtige Menüoption **[!UICONTROL Benutzerspezifischer Traffic]** > **[!UICONTROL Benutzerspezifischer Traffic 1-10]** > **[!UICONTROL LoadAsset]**. Wenn Sie über mehr als zehn benutzerdefinierte Eigenschaften verfügen, werden Ihnen auch andere Menüoptionen angezeigt.

1. Zeigen Sie das von Adobe Analytics erstellte Diagramm an. Dieses Diagramm stellt normalerweise nur die Daten einer einzelnen Metrik dar. Wenn Sie auch wissen möchten, mit welchem Asset diese Daten verknüpft sind, rufen Sie die Asset-Daten dieses Ereignisses ab. Beispielsweise ist es oft hilfreich zu wissen, welches Video nur zu 50 % angesehen wird oder welches Bild in einem Set beliebt ist.

>[!NOTE]
>
>Alle Adobe Dynamic Media Classic-Viewer-Daten werden in benutzerspezifischen Traffic-Berichten oder benutzerspezifischen Konversionsberichten von Adobe Analytics angezeigt und gemeldet.

Weitere Informationen finden Sie unter [Analytics-Tutorials](https://experienceleague.adobe.com/en/docs/analytics-learn/tutorials/overview).