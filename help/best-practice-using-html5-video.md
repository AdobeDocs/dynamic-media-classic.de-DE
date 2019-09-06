---
title: '"Optimale Vorgehensweise: Verwenden des HTML5-Video-Viewers"'
seo-title: '"Optimale Vorgehensweise: Verwenden des HTML5-Video-Viewers"'
description: 'null'
seo-description: Erfahren Sie mehr über Best Practices für die Verwendung des HTML 5-Video-Viewers.
uuid: 3 c 8924 dc -7 bea -4 c 25-b 77 b -005 f 57 b 71 b 64
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/video
discoiquuid: 4 b 11 cab 7-88 cf -42 dd -8554-2 eea 530753 bb
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Optimale Vorgehensweise: Verwenden des HTML5-Video-Viewers{#best-practice-using-the-html-video-viewer}

Die Dynamic Media Classic HTML 5 Video Viewer-Vorgaben sind robuste Video-Player. Im Design des Players können Sie alle Funktionen des Videoplayers mit standardmäßigen Webentwicklungstools erstellen. Sie können beispielsweise die Schaltflächen, die Steuerelemente und den benutzerdefinierten Standbildhintergrund mithilfe von HTML5 und CSS gestalten, um Ihren Kunden ein benutzerdefiniertes Erscheinungsbild zu bieten.

Bei der Wiedergabe erkennt der Viewers automatisch die Videofähigkeit des Browsers. Anschließend wird das Video über HLS (adaptives Video-Streaming) bereitgestellt. Wenn diese Bereitstellungsmethode nicht vorhanden ist, wird stattdessen HTML 5 Progressive verwendet.

Durch Kombination der Gestaltungsmöglichkeit der Wiedergabekomponenten mit HTML5 und CSS, der eingebetteten Wiedergabe und der Verwendung von adaptivem und progressivem Streaming je nach Browserfähigkeiten in einem einzigen Player, erweitern Sie die Reichweite ihrer Rich Media-Inhalte auf Desktop- und Mobilgerätebenutzer und stellen eine optimierte Videoerfahrung sicher.

Siehe auch [Info zu HTML 5-Viewern](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/c_html5_viewers_about.html) im Referenzhandbuch zu Adobe Viewers.

## Wiedergabe von Videos auf Desktopcomputern und mobilen Geräten mithilfe des dynamischen Media-Viewers für die Video-Viewer {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

Für adaptives und mobiles Video-Streaming für Mobilgeräte basieren die für das Umschalten zwischen den Bitraten verwendeten Videos auf allen MP 4-Videos im adaptiven Videoset.

Die Videowiedergabe erfolgt entweder über HLS oder progressiv. HLS (HTTP Live Streaming) ist ein Apple-Standard für adaptive Videostreaming, der die Wiedergabe automatisch an die Netzwerkbandbreitenkapazität anpasst. Außerdem wird der Kunde zu einem beliebigen Punkt im Video "Suche" , ohne dass darauf gewartet werden muss, dass der Rest des Videos heruntergeladen wird (siehe auch [HTTP Live Streaming](#UnresolvedLink-https://developer.apple.com/streaming/)). Progressives Video wird bereitgestellt, indem das Video lokal auf den Desktop-Bildschirm oder das Mobilgerät eines Benutzers heruntergeladen und gespeichert wird.

Die folgende Tabelle beschreibt das Gerät, den Browser und die Wiedergabemethode von Videos auf Desktopcomputern und mobilen Geräten mithilfe des Dynamic Media Classic Video Viewers.

| Gerät | Browser | Videowiedergabemodus |
|--- |--- |--- |
| Deskop | Internet Explorer 9 und 10 | Progressives Herunterladen. |
| Desktop | Internet Explorer 11 + | HLS-Videostreaming. |
| Desktop | Firefox 23-44 | Progressives Herunterladen. |
| Desktop | Firefox 45 oder neuer | HLS-Videostreaming. |
| Desktop | Chrome | HLS-Videostreaming. |
| Desktop | Safari (Mac) | HLS-Videostreaming. |
| Mobil | Chrome (Android 6 oder früher) | Progressives Herunterladen. |
| Mobil | Chrome (Android 7 oder höher) | HLS-Videostreaming. |
| Mobil | Android (Standardbrowser) | Progressives Herunterladen. |
| Mobil | Safari (ios) | HLS-Videostreaming. |
| Mobil | Chrome (ios) | HLS-Videostreaming. |
| Mobil | Blackberry | HLS-Videostreaming. |
