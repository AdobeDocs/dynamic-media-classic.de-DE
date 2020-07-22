---
title: Aktivieren von Adobe Analytics-Videoberichten
seo-title: Aktivieren von Adobe Analytics-Videoberichten
description: 'null'
seo-description: Erfahren Sie, wie Sie Adobe Analytics-Videoberichte aktivieren.
uuid: 078594b2-7d53-4714-8128-ff3b5c3a5e36
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 18644a53-92da-40ab-b961-318d8332c54d
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 26%

---


# Aktivieren von Adobe Analytics-Videoberichten{#enabling-adobe-analytics-video-reports}

Mit Adobe Analytics Heartbeat-basiertem Video-Berichte müssen Sie die vier Video-Viewer-Ereignis (Wiedergabe, Pause, Stopp, Meilenstein) nicht mehr aktivieren, wenn Sie Adobe Analytics in Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit standardmäßigen Dynamic Media Classic HTML5 Video- und MixedMedia-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten.

* Die Integration von Adobe Analytics-Videoberichten mit Dynamic Media Classic unterstützt Lösungsvariablen, jedoch keine benutzerspezifischen Variablen.

   See [Configure Analytics Video Reporting](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) for more information about solution variables and custom variables.

* Standardisierte (Out-of-the-box) Segmente mit Schritten von einer Minute werden unterstützt. Andererseits wird die Berichterstellung für benutzerdefinierte Segmente, wie benutzerdefinierte Meilensteine basierend auf Zeitschritten, % Meilenstein oder Offset-Meilensteine nicht unterstützt.

For more information about Video Heartbeat requirements and setup, see [Measuring Video in Adobe Analytics using Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Wenn Ihre lizenzierte Adobe Analytics-Lösung Video Heartbeat nicht enthält, müssen Sie die in diesem Kapitel beschriebenen Schritte fortsetzen, um Adobe Analytics-Variablen Dynamic Media Classic-Viewer-Ereignissen und -Variablen zuzuweisen.

