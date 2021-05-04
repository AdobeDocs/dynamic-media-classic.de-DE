---
title: Testen der Adobe Analytics-Integration durch Anzeigen eines Adobe Analytics-Berichts
description: Erfahren Sie, wie Sie die Integration testen können, indem Sie einen Adobe Analytics-Bericht anzeigen.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
translation-type: tm+mt
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 15%

---

# Testen der Adobe Analytics-Integration durch Anzeigen eines Adobe Analytics-Berichts{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Nachdem Sie die erforderlichen Variablen in Adobe Analytics erstellt, sie mit Dynamic Media Classic-Ereignissen verknüpft und die erforderlichen Implementierungsschritte ausgeführt haben, können Sie die Einrichtung testen. Sie können in Adobe Analytics selbst testen und prüfen, ob die Daten erfasst werden. Wenn das Setup hier funktioniert, sind keine weiteren Schritte nötig. Wenn Sie die obigen Schritte ausgeführt und Ihre Dynamic Media Classic-Ereignis-Daten mit einer oder mehreren benutzerspezifischen Traffic-Variablen verknüpft haben, führen Sie diesen Arbeitsablauf aus, um Ihre Daten in Adobe Analytics zu testen.

**So testen Sie die Integration durch Anzeigen eines Adobe Analytics-Berichts:**

1. Beginn eines Dynamic Media Classic-Viewers über Ihr Konto, insbesondere mit einer Metrik, die Sie erhalten möchten, und Interaktion mit diesem, um Ereignis-Daten zu erstellen.

   Wenn Sie beispielsweise beliebte alternative Ansichten in einem Bildsatz messen möchten, führen Sie die Vorschau eines Bildsatzes durch und klicken Sie auf die verschiedenen Miniaturbilder.

1. Gehen Sie innerhalb von Adobe Analytics zu **[!UICONTROL Benutzerspezifischer Traffic]** > **[!UICONTROL Benutzerspezifischer Traffic 1-10]** > [Name der Eigenschaft] und wählen Sie Ihren Traffic-Eigenschaftsnamen aus den Menüoptionen.

   Um beispielsweise auf die Eigenschaft **[!UICONTROL LoadAsset]** im Beispielkonto zuzugreifen, wäre die richtige Menüoption **[!UICONTROL Benutzerspezifischer Traffic]** > **[!UICONTROL Benutzerspezifischer Traffic 1-10]** > **[!UICONTROL LoadAsset]**. Wenn Sie über mehr als zehn benutzerdefinierte Eigenschaften verfügen, werden auch andere Menüoptionen angezeigt.

1. Zeigen Sie das von Adobe Analytics erstellte Diagramm an. Dieses Diagramm ist normalerweise nur die Daten einer einzelnen Metrik. Wenn Sie auch wissen möchten, mit welchem Asset diese Daten verknüpft sind, rufen Sie die Asset-Daten dieses Ereignisses ab. Beispielsweise ist es oft hilfreich zu wissen, welches Video nur zu 50 % angesehen wird oder welches Bild in einem Set beliebt ist.

>[!NOTE]
>
>Alle Dynamic Media Classic Viewer-Daten werden in benutzerspezifischen Traffic-Berichten oder benutzerspezifischen Konvertierungsberichten von Adobe Analytics angezeigt und in Berichten aufgeführt.

Weitere Informationen finden Sie unter [Analytics-Tutorials](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html).