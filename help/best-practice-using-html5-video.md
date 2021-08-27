---
title: Best Practice für die Verwendung des HTML5-Video-Viewers
description: Erfahren Sie mehr über Best Practices für die Verwendung des HTML5-Video-Viewers.
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 13%

---

# Best Practices für die Verwendung des HTML5-Video-Viewers{#best-practice-using-the-html-video-viewer}

Die Adobe Dynamic Media Classic HTML5-Video-Viewer-Vorgaben sind robuste Video-Player. Auf der Entwurfsseite des Players können Sie die gesamte Funktionalität des Videoplayers mithilfe standardmäßiger Webentwicklungstools erstellen. Sie können beispielsweise die Schaltflächen, die Steuerelemente und den benutzerdefinierten Standbildhintergrund mithilfe von HTML5 und CSS gestalten, um Ihren Kunden ein benutzerdefiniertes Erscheinungsbild zu bieten.

Bei der Wiedergabe erkennt der Viewers automatisch die Videofähigkeit des Browsers. Anschließend wird das Video mithilfe von HLS (HTTP Live Streaming), auch als adaptives Video-Streaming bezeichnet, bereitgestellt. Oder wenn diese Bereitstellungsmethode nicht vorhanden ist, wird stattdessen die progressive HTML5-Version verwendet.

Indem Sie die folgenden Fähigkeiten in einem einzelnen Player kombinieren:

* Wiedergabekomponenten, die mit HTML5 und CSS erstellt wurden
* Eingebettete Wiedergabe
* Verwendung von adaptivem und progressivem Streaming basierend auf der Browserfunktion

Sie erweitern die Reichweite Ihrer Rich-Media-Inhalte auf Desktop- und Mobilbenutzer. Sie stellen auch ein optimiertes Videoerlebnis sicher.

Siehe auch [Über HTML5-Viewer](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) im Adobe Viewer-Referenzhandbuch.

## Wiedergabe von Videos auf Desktop-Computern und Mobilgeräten mit der Adobe Dynamic Media Classic Video Viewer {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Beim adaptiven Video-Streaming auf Desktop- und Mobilgeräten basieren die für den Bitratenwechsel verwendeten Videos auf allen MP4-Videos im adaptiven Videoset.

Die Videowiedergabe erfolgt entweder über HLS oder progressive Videos. HLS (HTTP Live Streaming) ist ein Apple-Standard für adaptives Video-Streaming, der die Wiedergabe automatisch an die Netzwerkbandbreitenkapazität anpasst. Außerdem kann der Kunde einen beliebigen Punkt im Video &quot;suchen&quot;, ohne auf den Download des restlichen Videos warten zu müssen. Siehe auch [HTTP Live Streaming](https://developer.apple.com/streaming/). Progressives Video wird bereitgestellt, indem das Video lokal auf den Desktop-Bildschirm oder das Mobilgerät eines Benutzers heruntergeladen und gespeichert wird.

In der folgenden Tabelle werden das Gerät, der Browser und die Wiedergabemethode von Videos auf Desktop-Computern und Mobilgeräten mit der Adobe Dynamic Media Classic Video Viewer beschrieben.

| Gerät | Browser | Videowiedergabemodus |
|--- |--- |--- |
| Desktop | Internet Explorer 9 und 10 | Progressiver Download. |
| Desktop | Internet Explorer 11+ | HLS-Video-Streaming. |
| Desktop | Firefox 23-44 | Progressiver Download. |
| Desktop | Firefox 45 oder neuer | HLS-Video-Streaming. |
| Desktop | Chrome | HLS-Video-Streaming. |
| Desktop | Safari (Mac) | HLS-Video-Streaming. |
| Mobil | Chrome (Android™ 6 oder früher) | Progressiver Download. |
| Mobil | Chrome (Android™ 7 oder höher) | HLS-Video-Streaming. |
| Mobil | Android™ (Standardbrowser) | Progressiver Download. |
| Mobil | Safari (iOS) | HLS-Video-Streaming. |
| Mobil | Chrome (iOS) | HLS-Video-Streaming. |
| Mobil | BlackBerry® | HLS-Video-Streaming. |
