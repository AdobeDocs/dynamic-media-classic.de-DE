---
title: Adobe Analytics-Videoberichte aktivieren
description: Erfahren Sie, wie Sie Adobe Analytics-Videoberichte in Adobe Dynamic Media Classic aktivieren.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 12%

---

# Adobe Analytics-Videoberichte aktivieren{#enabling-adobe-analytics-video-reports}

Bei der Verwendung von Heartbeat-basierten Videoberichten in Adobe Analytics müssen Sie die vier Video-Viewer-Ereignisse (Wiedergabe, Pause, Stopp, Milestone) nicht mehr aktivieren, wenn Sie Adobe Analytics in Adobe Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit nativen Adobe Dynamic Media Classic HTML5 Video- und Mixed Media-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten.

* Eine Einführung in Streaming-Medien und &quot;Heartbeat-Messung&quot;finden Sie unter [Informationen zu Adobe Analytics für Streaming-Medien](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* Die Integration von Adobe Analytics-Videoberichten mit Adobe Dynamic Media Classic unterstützt Lösungsvariablen, jedoch keine benutzerdefinierten Variablen.

   Weitere Informationen zu Lösungsvariablen und benutzerdefinierten Variablen finden Sie unter [Audio- und Videoparameter](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) .

* Vordefinierte Segmente mit einminütigen Schritten werden unterstützt. Andererseits wird die Berichterstellung für benutzerdefinierte Segmente, wie benutzerdefinierte Meilensteine basierend auf Zeitschritten, % Meilenstein oder Offset-Meilensteine nicht unterstützt.

   Weitere Informationen zu Streaming-Medienanforderungen und zur Einrichtung finden Sie unter [Steaming-Medien in Adobe Analytics messen](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Informationen zu benutzerdefinierten Variablen und Lösungsvariablen finden Sie unter [Aktivierung von Medienberichten](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Wenn Ihre lizenzierte Adobe Analytics-Lösung Video Heartbeat nicht enthält, müssen Sie die in diesem Kapitel beschriebenen Schritte fortsetzen, um Adobe Analytics-Variablen Adobe Dynamic Media Classic-Viewer-Ereignissen und -Variablen zuzuweisen.
