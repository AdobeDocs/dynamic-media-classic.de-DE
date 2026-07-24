---
title: Best Practices für die Verwendung des HTML5-Video-Viewers
description: Erfahren Sie mehr über die Best Practices für die Verwendung des HTML5-Video-Viewers.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:39:23.475Z'
TQID: 'https://experienceleague.adobe.com/wGnoHGEOQLVV-rnoKBOE8wzphK3VaM-vr9YB1Y-gT8c'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 5fdabd28c4d0defdf9f145b581c89640cc1f6118
workflow-type: tm+mt
source-wordcount: 482
ht-degree: 2%

---

# Best Practices für die Verwendung des HTML5 Video Viewers{#best-practice-using-the-html-video-viewer}

Die Adobe Dynamic Media Classic HTML5-Video-Viewer-Vorgaben sind leistungsstarke Video-Player. Für das Player-Design können Sie die gesamte Funktionalität des Video-Players mit standardmäßigen Web-Entwicklungs-Tools erstellen. Um das Erscheinungsbild anzupassen, können Sie Schaltflächen, Steuerelemente und ein benutzerdefiniertes Standbild mit HTML5 und CSS entwerfen.

Bei der Viewer-Wiedergabe werden die Videofunktionen des Browsers automatisch erkannt. Anschließend werden die Videos mit HLS (HTTP Live Streaming), auch als adaptives Video-Streaming bezeichnet, bereitgestellt. Wenn diese Bereitstellungsmethode nicht vorhanden ist, wird stattdessen HTML5 Progressive verwendet.

Durch die Kombination der folgenden Funktionen zu einem einzelnen Player:

* Wiedergabekomponenten, die mit HTML5 und CSS entwickelt wurden.
* Eingebettete Wiedergabe
* Verwendung von adaptivem und progressivem Streaming basierend auf den Browser-Funktionen.

Sie erhöhen die Verfügbarkeit Ihrer Rich-Media-Inhalte für Desktop- und Mobile-Benutzer. Außerdem sorgen Sie für ein optimiertes Videoerlebnis.

Siehe auch [Über HTML5-Viewer](https://experienceleague.adobe.com/de/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only) im Adobe Viewers-Referenzhandbuch.

Siehe auch [Viewer-Vorgaben](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) Schulungsvideo.

## Wiedergabe von Videos auf Desktop-Computern und Mobilgeräten mit dem Adobe Dynamic Media Classic Video Viewer {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Beim adaptiven Video-Streaming auf Desktop und Mobilgeräten basieren die für den Bit-Ratenwechsel verwendeten Videos auf allen MP4-Videos im adaptiven Videoset.

Die Videowiedergabe erfolgt entweder mit HLS oder mit progressivem Video. HLS (HTTP Live Streaming) ist ein Apple-Standard für adaptives Video-Streaming, der die Wiedergabe automatisch an die Netzwerkbandbreitenkapazität anpasst. Außerdem können Benutzer zu jedem Punkt im Video navigieren, ohne auf den Download des restlichen Videos warten zu müssen. Siehe auch [HTTP Live Streaming](https://developer.apple.com/streaming/). Das System stellt progressive Videos bereit, indem es sie lokal auf den Desktop-Bildschirm oder das Mobilgerät eines Benutzers herunterlädt und speichert.

In der folgenden Tabelle werden das Gerät, der Browser und die Wiedergabemethode für Videos auf Desktop-Computern und Mobilgeräten mit dem Adobe Dynamic Media Classic Video Viewer beschrieben.

| Gerät | Browser | Videowiedergabemodus |
|--- |--- |--- |
| Desktop | Internet Explorer 9 und 10 | Progressiver Download |
| Desktop | Internet Explorer 11+ | HLS-Video-Streaming. |
| Desktop | Firefox 23-44 | Progressiver Download |
| Desktop | Firefox 45 oder höher | HLS-Video-Streaming. |
| Desktop | Chrome | HLS-Video-Streaming. |
| Desktop | Safari (Mac) | HLS-Video-Streaming. |
| Mobil | Chrome (Android™ 6 oder früher) | Progressiver Download |
| Mobil | Chrome (Android™ 7 oder höher) | HLS-Video-Streaming. |
| Mobil | Android™ (Standardbrowser) | Progressiver Download |
| Mobil | Safari (iOS) | HLS-Video-Streaming. |
| Mobil | Chrome (iOS) | HLS-Video-Streaming. |
| Mobil | BlackBerry® | HLS-Video-Streaming. |
