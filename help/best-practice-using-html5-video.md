---
title: Bewährte Verfahren für die Verwendung des HTML5-Video-Viewers
description: Erfahren Sie mehr über die Best Practices für die Verwendung des HTML5-Video-Viewers.
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
feature: Dynamic Media Classic, Viewer, Video
role: Business Practitioner
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
translation-type: tm+mt
source-git-commit: 31ac96e6fd11c47284d58540f5ec0135f0e6223b
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 13%

---

# Bewährte Verfahren für die Verwendung des HTML5-Video-Viewers{#best-practice-using-the-html-video-viewer}

Die HTML5-Video-Viewer-Vorgaben von Dynamic Media Classic sind robuste Video-Player. Auf der Entwurfsseite des Players können Sie die gesamte Funktionalität des Videoplayers mit standardmäßigen Webentwicklungstools erstellen. Sie können beispielsweise die Schaltflächen, die Steuerelemente und den benutzerdefinierten Standbildhintergrund mithilfe von HTML5 und CSS gestalten, um Ihren Kunden ein benutzerdefiniertes Erscheinungsbild zu bieten.

Bei der Wiedergabe erkennt der Viewers automatisch die Videofähigkeit des Browsers. Anschließend wird das Video mit HLS (HTTP Live Streaming), auch als adaptives Video-Streaming bezeichnet, bereitgestellt. Oder, wenn diese Versand-Methode nicht vorhanden ist, wird stattdessen progressives HTML5 verwendet.

Durch Kombination der folgenden Fähigkeiten zu einem einzelnen Spieler:

* Wiedergabe-Komponenten, die mit HTML5 und CSS entwickelt wurden
* Eingebettete Wiedergabe
* Verwendung von adaptivem und progressivem Streaming je nach Browserfähigkeiten

Sie erweitern die Reichweite Ihrer Rich-Media-Inhalte auf Desktop- und Mobilbenutzer. Sie können außerdem eine optimierte Videoerfahrung sicherstellen.

Siehe auch [Informationen zu HTML5-Viewern](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) im Adobe Viewer-Referenzhandbuch.

## Wiedergabe von Videos auf Desktop-Computern und Mobilgeräten mit dem Dynamic Media Classic Video Viewer {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Beim adaptiven Video-Streaming für Desktop- und Mobilgeräte basieren die für das Umschalten zwischen den Bitraten verwendeten Videos auf allen MP4-Videos im adaptiven Video-Set.

Die Videowiedergabe erfolgt entweder über HLS oder progressives Video. HLS (HTTP Live Streaming) ist ein Apple-Standard für adaptives Video-Streaming, mit dem die Wiedergabe automatisch an die Netzwerkbandbreitenkapazität angepasst wird. Sie ermöglicht dem Kunden auch, zu jedem Punkt im Video zu suchen, ohne dass der Rest des Videos heruntergeladen werden muss. Siehe auch [HTTP Live Streaming](https://developer.apple.com/streaming/). Progressives Video wird bereitgestellt, indem das Video lokal auf den Desktop-Bildschirm oder das Mobilgerät eines Benutzers heruntergeladen und gespeichert wird.

In der folgenden Tabelle sind das Gerät, der Browser und die Wiedergabe von Videos auf Desktopcomputern und Mobilgeräten mit dem Dynamic Media Classic Video Viewer beschrieben.

| Gerät | Browser | Videowiedergabemodus |
|--- |--- |--- |
| Desktop | Internet Explorer 9 und 10 | Progressiver Download. |
| Desktop | Internet Explorer 11+ | HLS-Videostreaming. |
| Desktop | Firefox 23-44 | Progressiver Download. |
| Desktop | Firefox 45 oder neuer | HLS-Videostreaming. |
| Desktop | Chrome | HLS-Videostreaming. |
| Desktop | Safari (Mac) | HLS-Videostreaming. |
| Mobil | Chrome (Android™ 6 oder früher) | Progressiver Download. |
| Mobil | Chrome (Android™ 7 oder höher) | HLS-Videostreaming. |
| Mobil | Android™ (Standardbrowser) | Progressiver Download. |
| Mobil | Safari (iOS) | HLS-Videostreaming. |
| Mobil | Chrome (iOS) | HLS-Videostreaming. |
| Mobil | BlackBerry® | HLS-Videostreaming. |
