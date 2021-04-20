---
title: Aktivieren von Adobe Analytics-Videoberichten
description: Erfahren Sie, wie Sie Adobe Analytics-Videoberichte aktivieren.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: 3def4a02eda8dc36f2811b3d4f0e870fff1994e4
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 16%

---


# Aktivieren von Adobe Analytics-Videoberichten{#enabling-adobe-analytics-video-reports}

Bei Verwendung des Adobe Analytics Heartbeat-basierten Video-Berichte müssen Sie die vier Video-Viewer-Ereignis (Wiedergabe, Pause, Stopp, Milestone) nicht mehr aktivieren, wenn Sie Adobe Analytics in Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit vordefinierten Dynamic Media Classic HTML5 Video- und MixedMedia-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten.

* Eine Einführung in Streaming-Medien und &quot;Heartbeat-Messung&quot;finden Sie unter [Info zu Adobe Analytics für Streaming Media](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* Die Integration von Adobe Analytics-Videoberichten mit Dynamic Media Classic unterstützt Lösungsvariablen, jedoch keine benutzerspezifischen Variablen.

   Weitere Informationen zu Lösungsvariablen und benutzerspezifischen Variablen finden Sie unter [Audio- und Video-Parameter](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata).

* Standardmäßige Segmente mit Inkrementierungen von einer Minute werden unterstützt. Andererseits wird die Berichterstellung für benutzerdefinierte Segmente, wie benutzerdefinierte Meilensteine basierend auf Zeitschritten, % Meilenstein oder Offset-Meilensteine nicht unterstützt.

   Weitere Informationen zu Streaming-Medienanforderungen und -Einstellungen finden Sie unter [Messen von Streaming-Medien in Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Weitere Informationen zu benutzerspezifischen Variablen und Lösungsvariablen finden Sie unter [Aktivierung von Medienberichten](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Wenn Ihre lizenzierte Adobe Analytics-Lösung Video Heartbeat nicht enthält, müssen Sie die in diesem Kapitel beschriebenen Schritte fortsetzen, um Dynamic Media Classic-Viewer-Ereignissen und -Variablen Adobe Analytics-Variablen zuzuweisen.

