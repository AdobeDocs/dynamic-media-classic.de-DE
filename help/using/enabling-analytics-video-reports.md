---
title: Aktivieren von Adobe Analytics-Videoberichten
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

# Aktivieren von Adobe Analytics-Videoberichten{#enabling-adobe-analytics-video-reports}

Bei der Verwendung von Adobe Analytics Heartbeat-basierten Videoberichten müssen Sie die vier Video-Viewer-Ereignisse (Wiedergabe, Pause, Stopp, Meilenstein) nicht mehr aktivieren, wenn Sie Adobe Analytics in Adobe Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit nativen Adobe Dynamic Media Classic HTML5-Video- und gemischten Medien-Viewern. Der Video-Player generiert Tracking-Daten zur Anzeige in Adobe Analytics-Videoberichten.

* Eine Einführung in Streaming-Medien und Heartbeat-Messungen finden Sie unter [Über Adobe Analytics für Streaming-Medien](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* Die Integration von Adobe Analytics-Videoberichten mit Adobe Dynamic Media Classic unterstützt Lösungsvariablen, jedoch keine benutzerdefinierten Variablen.

  Weitere Informationen [ Lösungsvariablen und benutzerdefinierten Variablen finden Sie ](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters) „Audio- und Videoparameter“.

* Vorkonfigurierte Segmente von Intervallen von einer Minute werden unterstützt. Benutzerdefinierte Segmentberichte, wie kundendefinierte Meilensteine, die auf Zeitinkrementen, %-Meilensteinen oder Offset-Meilensteinen basieren, werden jedoch nicht unterstützt.

  Weitere Informationen zu den Anforderungen und zur Einrichtung von Streaming-Medien finden Sie unter [ von Streaming-Medien in Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* Informationen zu benutzerdefinierten und Lösungsvariablen finden Sie unter [Aktivierung von Medienberichten](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-reports/media-reports-enable#media-reports).

>[!NOTE]
>
>Wenn Ihre lizenzierte Adobe Analytics-Lösung Video Heartbeat nicht enthält, fahren Sie mit den in diesem Kapitel beschriebenen Schritten fort, um Adobe Dynamic Media Classic-Viewer-Ereignissen und -Variablen Adobe Analytics-Variablen zuzuweisen.
