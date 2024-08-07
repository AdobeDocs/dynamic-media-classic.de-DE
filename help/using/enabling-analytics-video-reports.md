---
title: Adobe Analytics-Videoberichte aktivieren
description: Erfahren Sie, wie Sie Adobe Analytics-Videoberichte in Adobe Dynamic Media Classic aktivieren.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Adobe Analytics-Videoberichte aktivieren{#enabling-adobe-analytics-video-reports}

Bei der Verwendung von Heartbeat-basierten Videoberichten in Adobe Analytics müssen Sie die vier Video-Viewer-Ereignisse (Wiedergabe, Pause, Stopp, Milestone) nicht mehr aktivieren, wenn Sie Adobe Analytics in Adobe Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit nativen Adobe Dynamic Media Classic HTML5-Video- und gemischten Medien-Viewern. Der Videoplayer generiert Tracking-Daten für die Anzeige in Adobe Analytics-Videoberichten.

* Eine Einführung in Streaming-Medien und &quot;Heartbeat-Messung&quot;finden Sie unter [Über Adobe Analytics für Streaming-Medien](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* Die Integration von Adobe Analytics-Videoberichten mit Adobe Dynamic Media Classic unterstützt Lösungsvariablen, jedoch keine benutzerdefinierten Variablen.

  Weitere Informationen zu Lösungsvariablen und benutzerdefinierten Variablen finden Sie unter [Audio- und Videoparameter](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters) .

* Vordefinierte Segmente mit einminütigen Schritten werden unterstützt. Benutzerdefinierte Segmentberichte wie kundendefinierte Meilensteine basierend auf Zeitinkrementen, %-Meilensteinen oder Offset-Meilensteinen werden jedoch nicht unterstützt.

  Weitere Informationen zu Streaming-Medienanforderungen und zur Einrichtung finden Sie unter [Messen von Streaming-Medien in Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* Informationen zu benutzerspezifischen Variablen und Lösungsvariablen finden Sie unter [Aktivierung von Medienberichten](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-reports/media-reports-enable#media-reports).

>[!NOTE]
>
>Wenn Ihre lizenzierte Adobe Analytics-Lösung Video Heartbeat nicht enthält, führen Sie die in diesem Kapitel beschriebenen Schritte aus, um Adobe Dynamic Media Classic-Viewer-Ereignissen und -Variablen Adobe Analytics-Variablen zuzuweisen.
