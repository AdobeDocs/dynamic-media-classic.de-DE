---
title: Testen der Adobe Analytics-Integration durch Anzeigen eines Adobe Analytics-Berichts
seo-title: Testen der Adobe Analytics-Integration durch Anzeigen eines Adobe Analytics-Berichts
description: 'null'
seo-description: Erfahren Sie, wie Sie die Integration testen können, indem Sie einen Adobe Analytics-Bericht anzeigen.
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 42%

---


# Testen der Adobe Analytics-Integration durch Anzeigen eines Adobe Analytics-Berichts{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Nachdem Sie die erforderlichen Variablen in Adobe Analytics erstellt, sie mit Dynamic Media Classic-Ereignissen verknüpft und die erforderlichen Implementierungsschritte abgeschlossen haben, sollten Sie die Einrichtung testen. Sie können in Adobe Analytics selbst testen und prüfen, ob die Daten erfasst werden. Wenn das Setup hier funktioniert, sind keine weiteren Schritte nötig. Wenn Sie die obigen Schritte ausgeführt und Ihre Dynamic Media Classic-Ereignis-Daten mit einer oder mehreren benutzerspezifischen Traffic-Variablen verknüpft haben, führen Sie diesen Arbeitsablauf aus, um Ihre Daten in Adobe Analytics zu testen.

**So testen Sie die Integration durch Anzeigen eines Adobe Analytics-Berichts**

1. Starten Sie einen Dynamic Media Classic-Viewer von Ihrem Konto aus, insbesondere einen, der die zu erfassende Metrik überträgt, und interagieren Sie damit, um einige Ereignis-Daten zu erstellen.

   Wenn Sie z. B. die beliebtesten alternativen Ansichten in einem Bildset ermitteln möchten, zeigen Sie eine Vorschau des Bildsets an und klicken Sie auf die verschiedenen Miniaturbilder.

1. Gehen Sie innerhalb von Adobe Analytics zu Custom Traffic > Custom Traffic 1-10 > [Name der Eigenschaft] und wählen Sie Ihren Traffic-Eigenschaftsnamen aus den Menüoptionen.

   Wenn Sie z. B. die Eigenschaft „LoadAsset“ in unserem Beispielkonto aufrufen möchten, wählen Sie entsprechend „Benutzerspez. Traffic“ > „Benutzerspezifischer Traffic 1-10“ > „LoadAsset“. Wenn Sie über mehr als zehn benutzerdefinierte Eigenschaften verfügen, werden unter Umständen weitere Menüoptionen angezeigt.

1. Zeigen Sie das von Adobe Analytics erstellte Diagramm an. Beachten Sie, dass es normalerweise nur die Daten für eine Metrik enthält. Wenn Sie auch wissen möchten, mit welchem Asset diese Daten verknüpft sind (z. B. welches Video nur zu 50 % angesehen wird oder welches Bild in einem Set am beliebtesten ist), erfassen Sie unbedingt auch die Asset-Daten dieses Ereignisses.

>[!NOTE]
>
>Alle Dynamic Media Classic Viewer-Daten werden in benutzerspezifischen Traffic-Berichten oder benutzerspezifischen Konvertierungsberichten von Adobe Analytics angezeigt und in Berichten aufgeführt.

Weitere Informationen finden Sie unter [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en).
