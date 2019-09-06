---
title: Aktivieren von Adobe Analytics-Videoberichten
seo-title: Aktivieren von Adobe Analytics-Videoberichten
description: 'null'
seo-description: Erfahren Sie, wie Sie Adobe Analytics-Videoberichte aktivieren.
uuid: 078594 b 2-7 d 53-4714-8128-ff 3 b 5 c 3 a 5 e 36
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: 18644 a 53-92 da -40 ab-b 961-318 d 8332 c 54 d
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Aktivieren von Adobe Analytics-Videoberichten{#enabling-adobe-analytics-video-reports}

Bei Verwendung von Adobe Analytics Heartbeat-basierenden Videoberichten müssen Sie die vier Video-Viewer-Ereignisse (Play, Pause, Stopp, Milestone) nicht mehr aktivieren, wenn Sie Adobe Analytics in Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit vordefinierten dynamischen Media Classic HTML 5 Video- und mixedmedia-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten.

* Die Integration von Adobe Analytics-Videoberichten mit Dynamic Media Classic unterstützt Lösungsvariablen, jedoch keine benutzerspezifischen Variablen.

   See [Configure Analytics Video Reporting](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) for more information about solution variables and custom variables.

* Standardisierte (Out-of-the-box) Segmente mit Schritten von einer Minute werden unterstützt. Andererseits wird die Berichterstellung für benutzerdefinierte Segmente, wie benutzerdefinierte Meilensteine basierend auf Zeitschritten, % Meilenstein oder Offset-Meilensteine nicht unterstützt.

For more information about Video Heartbeat requirements and setup, see [Measuring Video in Adobe Analytics using Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Wenn Ihre lizenzierte Lösung von Adobe Analytics keine Video Heartbeat enthält, müssen Sie weiterhin die Schritte in diesem Kapitel verwenden, um Adobe Analytics-Variablen zu dynamischen Media Classic-Viewer-Ereignissen und -variablen zuzuweisen.

