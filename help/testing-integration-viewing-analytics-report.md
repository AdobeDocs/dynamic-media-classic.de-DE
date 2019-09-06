---
title: Testen der Adobe Analytics-Integration durch Anzeigen eines Adobe Analytics-Berichts
seo-title: Testen der Adobe Analytics-Integration durch Anzeigen eines Adobe Analytics-Berichts
description: 'null'
seo-description: Erfahren Sie, wie Sie die Integration testen, indem Sie einen Adobe Analytics-Bericht ansehen.
uuid: 937375 e 0-6 dea -4 baa-a 2 b 0-4 f 3 e 461 c 9 ee 2
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: 1 ddc 89 ff-d 2 e 9-42 eb-a 442-aa 6 b 9871 c 991
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Testen der Adobe Analytics-Integration durch Anzeigen eines Adobe Analytics-Berichts{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Nachdem Sie die erforderlichen Variablen in Adobe Analytics erstellt, diese mit dynamischen Media Classic-Ereignissen verknüpft und die erforderlichen Implementierungsschritte durchgeführt haben, sollten Sie das Setup testen. Sie können in Adobe Analytics selbst testen und prüfen, ob die Daten erfasst werden. Wenn das Setup hier funktioniert, sind keine weiteren Schritte nötig. Wenn Sie die oben genannten Schritte ausgeführt und Ihre Ereignisdaten für dynamische Medien mit mindestens einer benutzerspezifischen Traffic-Variablen verknüpft haben, testen Sie die Daten in Adobe Analytics mit diesem Arbeitsablauf.

**So testen Sie die Integration durch Anzeigen eines Adobe Analytics-Berichts**

1. Starten Sie einen dynamischen Media Classic-Viewer aus Ihrem Konto, insbesondere einen, der die zu erfassende Metrik überträgt, und interagieren Sie mit dieser, um Ereignisdaten zu erstellen.

   Wenn Sie z. B. die beliebtesten alternativen Ansichten in einem Bildset ermitteln möchten, zeigen Sie eine Vorschau des Bildsets an und klicken Sie auf die verschiedenen Miniaturbilder.

1. Inside Adobe Analytics, go to Custom Traffic &gt; Custom Traffic 1-10 &gt; [Name of prop], selecting your traffic prop name from the menu choices.

   Wenn Sie z. B. die Eigenschaft „LoadAsset“ in unserem Beispielkonto aufrufen möchten, wählen Sie entsprechend „Benutzerspez. Traffic“ &gt; „Benutzerspezifischer Traffic 1-10“ &gt; „LoadAsset“. Wenn Sie über mehr als zehn benutzerdefinierte Eigenschaften verfügen, werden unter Umständen weitere Menüoptionen angezeigt.

1. Zeigen Sie das von Adobe Analytics erstellte Diagramm an. Beachten Sie, dass es normalerweise nur die Daten für eine Metrik enthält. Wenn Sie darüber hinaus wissen möchten, mit welchem Asset diese Daten verknüpft sind (z. B. welches Video nur auf 50% angesehen wird oder welches Bild in einem Satz am beliebtesten ist), sollten Sie die Asset-Daten dieses Ereignisses ebenfalls erfassen.

>[!NOTE]
>
>Alle dynamischen Media-Viewer-Daten werden in benutzerspezifischen Traffic-Berichten oder in benutzerdefinierten Konversionsberichten von Adobe Analytics angezeigt.

Weitere Informationen finden Sie unter [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en).
