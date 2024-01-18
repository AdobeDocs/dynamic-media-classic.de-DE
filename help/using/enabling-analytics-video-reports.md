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
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 5%

---

# Adobe Analytics-Videoberichte aktivieren{#enabling-adobe-analytics-video-reports}

Bei der Verwendung von Heartbeat-basierten Videoberichten in Adobe Analytics müssen Sie die vier Video-Viewer-Ereignisse (Wiedergabe, Pause, Stopp, Milestone) nicht mehr aktivieren, wenn Sie Adobe Analytics in Adobe Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit nativen Adobe Dynamic Media Classic HTML5-Video- und gemischten Medien-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten.

* Eine Einführung in Streaming-Medien und &quot;Heartbeat-Messung&quot;finden Sie unter [Über Adobe Analytics für Streaming-Medien](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Die Integration von Adobe Analytics-Videoberichten mit Adobe Dynamic Media Classic unterstützt Lösungsvariablen, jedoch keine benutzerdefinierten Variablen.

  Siehe [Audio- und Videoparameter](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/variables/audio-video-parameters.html) für weitere Informationen zu Lösungsvariablen und benutzerdefinierten Variablen.

* Vordefinierte Segmente mit einminütigen Schritten werden unterstützt. Benutzerdefinierte Segmentberichte wie kundendefinierte Meilensteine basierend auf Zeitinkrementen, %-Meilensteinen oder Offset-Meilensteinen werden jedoch nicht unterstützt.

  Weitere Informationen zu Streaming-Medien-Anforderungen und -Einstellungen finden Sie unter [Messen von Streaming-Medien in Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Informationen zu benutzerdefinierten Variablen und Lösungsvariablen finden Sie unter [Aktivierung von Medienberichten](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Wenn Ihre lizenzierte Adobe Analytics-Lösung Video Heartbeat nicht enthält, müssen Sie die in diesem Kapitel beschriebenen Schritte fortsetzen, um Adobe Dynamic Media Classic-Viewer-Ereignissen und -Variablen Adobe Analytics-Variablen zuzuweisen.
