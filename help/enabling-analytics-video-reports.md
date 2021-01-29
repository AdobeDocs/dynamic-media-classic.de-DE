---
title: Aktivieren von Adobe Analytics-Videoberichten
description: Erfahren Sie, wie Sie Adobe Analytics-Videoberichte aktivieren.
uuid: 078594b2-7d53-4714-8128-ff3b5c3a5e36
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 18644a53-92da-40ab-b961-318d8332c54d
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 23%

---


# Aktivieren von Adobe Analytics-Videoberichten{#enabling-adobe-analytics-video-reports}

Bei Verwendung von Adobe Analytics Heartbeat-basiertem Video-Berichte müssen Sie die vier Video-Viewer-Ereignis (Wiedergabe, Pause, Stopp, Milestone) nicht mehr aktivieren, wenn Sie Adobe Analytics in Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit vordefinierten Dynamic Media Classic HTML5 Video- und MixedMedia-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten.

* Die Integration von Adobe Analytics-Videoberichten mit Dynamic Media Classic unterstützt Lösungsvariablen, jedoch keine benutzerspezifischen Variablen.

   Weitere Informationen zu Lösungsvariablen und benutzerspezifischen Berichten finden Sie unter [Analytics-Video konfigurieren](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html).

* Standardisierte (Out-of-the-box) Segmente mit Schritten von einer Minute werden unterstützt. Andererseits wird die Berichterstellung für benutzerdefinierte Segmente, wie benutzerdefinierte Meilensteine basierend auf Zeitschritten, % Meilenstein oder Offset-Meilensteine nicht unterstützt.

Weitere Informationen zu Video Heartbeat-Anforderungen und -Einstellungen finden Sie unter [Videomessung in Adobe Analytics mit Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Wenn Ihre lizenzierte Adobe Analytics-Lösung Video Heartbeat nicht enthält, müssen Sie die in diesem Kapitel beschriebenen Schritte fortsetzen, um Dynamic Media Classic-Viewer-Ereignissen und -Variablen Adobe Analytics-Variablen zuzuweisen.

