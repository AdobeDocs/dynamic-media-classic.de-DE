---
title: Aktivieren von Adobe Analytics-Videoberichten
description: Erfahren Sie, wie Sie Adobe Analytics-Videoberichte in Adobe Dynamic Media Classic aktivieren.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
autotag-review: '2026-05-13T19:47:00.853Z'
TQID: 'https://experienceleague.adobe.com/bXlrGU0zMEyfa-E-x-29-biChC17GJTEViBP8GoouTU'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 270
ht-degree: 0%

---

# Aktivieren von Adobe Analytics-Videoberichten{#enabling-adobe-analytics-video-reports}

Bei der Verwendung von Adobe Analytics Heartbeat-basierten Videoberichten müssen Sie die vier Video-Viewer-Ereignisse (Wiedergabe, Pause, Stopp, Meilenstein) nicht mehr aktivieren, wenn Sie Adobe Analytics in Adobe Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit nativen Adobe Dynamic Media Classic HTML5-Video- und gemischten Medien-Viewern. Der Video-Player generiert Tracking-Daten zur Anzeige in Adobe Analytics-Videoberichten.

* Eine Einführung in Streaming-Medien und die Heartbeat-Messung finden Sie unter [Über Adobe Analytics für Streaming-Medien](https://experienceleague.adobe.com/de/docs/media-analytics/using/media-overview).

* Die Integration von Adobe Analytics-Videoberichten mit Adobe Dynamic Media Classic unterstützt Lösungsvariablen, jedoch keine benutzerdefinierten Variablen.

  Weitere Informationen [&#x200B; Lösungsvariablen und benutzerdefinierten Variablen finden Sie &#x200B;](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters) „Audio- und Videoparameter“.

* Vorkonfigurierte Segmente von Intervallen von einer Minute werden unterstützt. Benutzerdefinierte Segmentberichte, wie kundendefinierte Meilensteine, die auf Zeitinkrementen, %-Meilensteinen oder Offset-Meilensteinen basieren, werden jedoch nicht unterstützt.

  Weitere Informationen zu den Anforderungen und zur Einrichtung von Streaming-Medien finden Sie unter [&#x200B; von Streaming-Medien in Adobe Analytics](https://experienceleague.adobe.com/de/docs/media-analytics/using/media-overview).

* Informationen zu benutzerdefinierten und Lösungsvariablen finden Sie unter [Aktivierung von Medienberichten](https://experienceleague.adobe.com/de/docs/media-analytics/using/media-reports/media-reports-enable#media-reports).

>[!NOTE]
>
>Wenn Ihre lizenzierte Adobe Analytics-Lösung Video Heartbeat nicht enthält, fahren Sie mit den in diesem Kapitel beschriebenen Schritten fort, um Adobe Dynamic Media Classic-Viewer-Ereignissen und -Variablen Adobe Analytics-Variablen zuzuweisen.
