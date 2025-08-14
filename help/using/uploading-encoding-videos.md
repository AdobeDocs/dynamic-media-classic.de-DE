---
title: Videos hochladen und kodieren
description: Erfahren Sie, wie Sie Videos in Adobe Dynamic Media Classic hochladen und kodieren.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 93ad91d7-f3dd-484b-b62c-633fcb864bbf
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '3981'
ht-degree: 40%

---

# Videos hochladen und kodieren{#uploading-and-encoding-videos}

Um einzelne Videos oder adaptive Videosets für die Bereitstellung im Web oder auf Mobilgeräten zu erstellen, laden Sie zunächst Ihre primären Videodateien in Adobe Dynamic Media Classic hoch. Adobe Dynamic Media Classic kodiert Videos im MP4-Format und veröffentlicht Videos in den folgenden Dateiformaten:

* **MP4**: Adobe Dynamic Media Classic empfiehlt MP4 als bevorzugtes Videodateiformat. Verwenden Sie MP4-Dateien für Folgendes:

   * HTTP Dynamic Streaming an Desktops.
   * HTTP Live Streaming (Streaming-Protokoll von Apple).
   * Progressive Videobereitstellung auf Android™-, BlackBerry®- und Windows®-Mobilgeräten

  Adobe Dynamic Media Classic bietet zwei Workflows zum Hochladen von Videodateien:

* **Vorkodierte Videos**: Sie laden MP4-Dateien direkt in Adobe Dynamic Media Classic hoch. Bei diesem Arbeitsablauf werden Dateien zum Zeitpunkt des Hochladens nicht kodiert. Die Dateien werden vorkodiert und so für die Ausgabe auf dem Desktop und mobilen Geräten vorbereitet.

* **Primäre Quellvideos**: Laden Sie Primärquellen-Videodateien hoch und kodieren Sie diese Dateien beim Hochladen in MP4-Dateien. Kodierte Videos sind im Durchsuchen-Panel mit „Video“ gekennzeichnet. Adobe Dynamic Media Classic unterstützt die Kodierung von Videodateien in vielen Formaten.

   * Stellen Sie sicher, dass die zu kodierenden Primär-Videodateien unterstützt werden.

     Siehe [Unterstützte Videodateitypen für die Kodierung](uploading-encoding-videos.md#supported-video-file-types-for-encoding).

   * Wählen Sie eine Videokodierungsvorgabe aus.

     Siehe [Video-Vorgaben zum Kodieren von Videodateien](application-setup.md#video-presets-for-encoding-video-files).

     Siehe [Bewährte Vorgehensweisen für die Videokodierung](uploading-encoding-videos.md#best-practices-for-video-encoding).

Adobe Dynamic Media Classic generiert auch Videominiaturen. Erfahren Sie mehr über Videominiaturen, das Abrufen ihrer URLs und das Bearbeiten von Standbildern.

Siehe [Arbeiten mit Videominiaturen](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**Hochladen und Kodieren von Videos:**

Führen Sie einen der folgenden Schritte aus.

*Wenn Ihre Videos bereits kodiert sind*

1. Wählen Sie in der Symbolleiste für globale Navigation **[!UICONTROL Hochladen]** aus.
1. Wählen Sie auf der Seite Hochladen die Registerkarte **[!UICONTROL Von Desktop]** aus.
1. Wählen Sie auf der Seite Hochladen im Bedienfeld **[!UICONTROL Dateien zum Hochladen auswählen]** die Option **[!UICONTROL Durchsuchen]**, navigieren Sie zu einer MP4-Videodatei und klicken Sie dann auf **[!UICONTROL Öffnen]**.
1. Wählen Sie im Bedienfeld **[!UICONTROL Ordnerziel]** einen Ordner für die hochgeladene Datei aus.
1. Stellen Sie auf der Seite Hochladen sicher, dass **[!UICONTROL Nach Hochladen veröffentlichen]** aktiviert ist.
1. Wählen Sie **[!UICONTROL Upload starten]** aus.

*Wenn Sie Ihre Videos mit Adobe Dynamic Media Classic kodieren möchten*

1. Wählen Sie in der Symbolleiste für globale Navigation **[!UICONTROL Hochladen]** aus.
1. Wählen Sie auf der Seite Hochladen die Registerkarte **[!UICONTROL Von Desktop]** aus.
1. Wählen Sie im Bedienfeld **[!UICONTROL Dateien zum Hochladen auswählen]** die Option **[!UICONTROL Durchsuchen]**, navigieren Sie zu einer Primärvideodatei und klicken Sie dann auf **[!UICONTROL Öffnen]**.
1. Wählen Sie im Bedienfeld **[!UICONTROL Ordnerziel]** einen Ordner für die hochgeladene Datei aus.
1. Klicken Sie unten rechts auf der Seite auf **[!UICONTROL Auftragsoptionen]**,
1. Erweitern Sie im Dialogfeld Upload-Auftragsoptionen **[!UICONTROL EVideo-Optionen]** und führen Sie dann einen der folgenden Schritte aus:

   * Es empfiehlt sich, „Adaptive **[!UICONTROL &quot;]** wählen. Siehe [Adaptive Video (Standard)](application-setup.md#adaptive-video-default).
   * Optional. Wenn Sie individuelle Kodierungseinstellungen verwenden möchten, erweitern Sie **[!UICONTROL Einzelne Kodierungsvorgaben]** und wählen Sie dann die gewünschten Kodierungsoptionen für Desktop, Mobilgerät und Tablet aus.
Siehe [ Vorgaben für die Videokodierung für Desktop-PCs](application-setup.md#desktop-video-encoding-presets), [Vorgaben für die Videokodierung für Mobilgeräte](application-setup.md#mobile-video-encoding-presets), [Vorgaben für die Videokodierung für Tablets](application-setup.md#tablet-video-encoding-presets).
1. Wählen Sie im Dialogfeld Upload-Auftragsoptionen die Option **[!UICONTROL Speichern]**.
1. Stellen Sie auf der Seite Hochladen sicher, dass **[!UICONTROL Nach Hochladen veröffentlichen]** aktiviert ist.
1. Wählen Sie auf der Seite „Hochladen“ in der rechten unteren Ecke **[!UICONTROL Upload starten]**.

*Wenn Sie eine zuvor hochgeladene Videodatei erneut kodieren möchten*

1. Navigieren Sie in Adobe Dynamic Media Classic im Durchsuchen-Panel zum Video und wählen Sie es aus.
1. Navigieren Sie **[!UICONTROL Datei]** > **[!UICONTROL Erneut verarbeiten]**.
1. Erweitern Sie im Dialogfeld Assets erneut verarbeiten **[!UICONTROL EVideo-Optionen]** und führen Sie dann einen der folgenden Schritte aus:
   * Es empfiehlt sich, die folgende Methode zu verwenden. Wählen Sie **Adaptives Video** aus.
Siehe [Adaptive Video (Standard)](application-setup.md#adaptive-video-default).
   * Optional. Wenn Sie individuelle Kodierungseinstellungen verwenden möchten, erweitern Sie **[!UICONTROL Einzelne Kodierungsvorgaben]** und wählen Sie dann die gewünschten Kodierungsoptionen für Desktop, Mobilgerät und Tablet aus.
Siehe [ Vorgaben für die Videokodierung für Desktop-PCs](application-setup.md#desktop-video-encoding-presets), [Vorgaben für die Videokodierung für Mobilgeräte](application-setup.md#mobile-video-encoding-presets), [Vorgaben für die Videokodierung für Tablets](application-setup.md#tablet-video-encoding-presets).
1. Wählen Sie im Dialogfeld Assets erneut verarbeiten die Option **[!UICONTROL Senden]** aus.

Wenn Sie eine adaptive Videokodierungsvorgabe oder mehrere Einzelkodierungsvorgaben verwenden, ist das Ergebnis ein adaptives Videoset, das automatisch mit mehreren Videokodierungen erstellt wird. Sie können auch manuell ein adaptives Videoset erstellen, indem Sie die einzelnen Videos auswählen.

Wenn Sie ein adaptives Videoset entweder automatisch oder manuell erstellen, werden nur MP4- und M4V-Dateien erzeugt.

## Unterstützte Videodateitypen für die Kodierung {#supported-video-file-types-for-encoding}

In der folgenden Tabelle sind die Videodateitypen (mit zulässigen Video-Codecs) aufgelistet, die Sie beim Hochladen in das Format MP4 oder OGV kodieren lassen können. Die Tabelle enthält Dateiformate und Codecs:

* **Videodateiformate**: Ähnlich wie eine ZIP-Datei bestimmt ein Videodateiformat, wie Dateien in der Videodatei enthalten sind. Eine Videodatei besteht in der Regel aus mehreren Spuren – einer Videospur (ohne Audio) und einer oder mehreren Audiospuren (ohne Video) –, die miteinander verknüpft und synchronisiert sind. Das Videodateiformat legt fest, wie diese unterschiedlichen Datenspuren in der Videodatei organisiert sind.

* **Video-Codecs**: Ein Video-Codec beschreibt den Algorithmus, mit dem ein Video kodiert wird. Ein Video-Player dekodiert das Video entsprechend dem Codec und zeigt dann eine Reihe von Bildern, auch Frames oder Bildfelder genannt, auf dem Bildschirm an. Codecs reduzieren die Datenmenge, die in Videodateien gespeichert werden muss, um das Video wiedergeben zu können. Anstelle von Informationen zu jedem einzelnen Frame werden nur Informationen über die Unterschiede zwischen einem Frame und dem nächsten gespeichert. Da sich die meisten Videos von einem Frame zum nächsten nur wenig ändern, ermöglichen Codecs hohe Komprimierungsraten, was zu kleineren Dateigrößen führt.

  | Videodateiformat | Video-Codecs |
  | --- | --- |
  | 3GP | H.263, H.264 |
  | AVI | DivX, DV |
  | M2P | MPEG-2 PS |
  | M2T | MPEG-2 TS |
  | M2TS | MPEG-2 TS |
  | M2V | MPEG-2 ES |
  | M4V | H.264 |
  | MOV | DV, DVCPro 50, H.261, H.263, H.264, Sorenson Video 1 |
  | MP4 | `H.264/MPEG-4` AVC |
  | MPEG | MPEG-2 SS |
  | MPG | MPEG-2 SS |
  | MTS | MPEG-2 |
  | ProRes | APCN, APCS, APCO, APCH, AP4H |
  | TS | DVCPro 50 |
  | VOB | MPEG-2 |
  | WMV/ASF | VC-1, Windows® Media Video 7, Windows® Media Video 8 |

  >[!NOTE]
  >
  >Auf der Seite „Aufträge“ werden Sie darauf hingewiesen, wenn eine Datei beim Hochladen und Kodieren zurückgewiesen wurde, da sie einen nicht unterstützten Codec oder Dateicontainer enthält. Weitere Informationen finden Sie unter [Überprüfen von Auftragsdateien](checking-job-files.md).

## Optimale Vorgehensweisen für die Videokodierung {#best-practices-for-video-encoding}

Im Folgenden finden Sie Best Practice-Tipps für die Kodierung von Quellvideodateien in Adobe Dynamic Media Classic.

<!-- THE FOLLOWINGS LINKS APPEAR TO BE DEAD AND THE CONTENT COMPLETELY LOST. THE GO URL DOESN'T EVEN WORK ANYMORE.
For advice about video encoding, see the following:

* Article: [Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution][www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en). THIS MATERIAL WAS FOUND ON A THIRD PARTY WEBSITE HERE: https://streaminglearningcenter.com/articles/streaming-101-the-basics-codecs-bandwidth-data-rate-and-resolution.html MATERIAL IS GOOD BUT DO NOT LINK TO IT
* Video: [Video Encoding Basics][www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en). -->

### Quell-Videodateien {#source-video-files}

Beim Kodieren einer Videodatei sollten Sie eine Quell-Videodatei mit der höchstmöglichen Qualität verwenden. Vermeiden Sie es, Dateien zu nutzen, die bereits zuvor kodiert wurden, da diese schon komprimiert sind. Eine weitere Kodierung würde zu einem Video von minderwertiger Qualität führen.

Die folgende Tabelle beschreibt die empfohlenen Werte für Größe, Seitenverhältnis und Mindest-Bitrate bei der Kodierung von Quellvideodateien:

| Größe | Seitenverhältnis | Minimale Bitrate |
| --- | --- | --- |
| 1024 X 768 | 4 :3 | 4500 Kbit/s sind für die meisten Videos ausreichend. |
| 1280 X 720 | 16 :9 | 3000: 6000 kBit/s, je nach Bewegungsdauer im Video. |
| 1920 X 1080 | 16 :9 | 6000: 8000 kBit/s, je nach Bewegungsdauer im Video. |

### Abrufen der Metadaten einer Datei {#obtaining-a-file-s-metadata}

Sie können die Metadaten einer Datei abrufen, indem Sie diese in Adobe Dynamic Media Classic mit einem Videobearbeitungs-Tool anzeigen oder ein Programm verwenden, das zum Abrufen von Metadaten entwickelt wurde. Im Folgenden wird die Verwendung von MediaInfo, eines Drittanbieterprogramms, zum Abrufen der Metadaten einer Videodatei beschrieben:

1. Wechseln Sie zu dieser Web-Seite: [https://mediaarea.net/en/MediaInfo](https://mediaarea.net/en/MediaInfo).
1. Wählen Sie das Installationsprogramm für die GUI-Version aus und laden Sie es herunter. Befolgen Sie anschließend die Installationsanweisungen.
1. Klicken Sie nach der Installation mit der rechten Maustaste auf die Videodatei (nur Windows®) und wählen Sie MediaInfo aus, oder öffnen Sie MediaInfo und ziehen Sie die Videodatei in die Anwendung. Es werden alle mit der Videodatei verknüpften Metadaten angezeigt, einschließlich Breite, Höhe und FPS.

### Seitenverhältnis {#aspect-ratio}

Wenn Sie eine Videokodierungsvorgabe für die primäre Videodatei auswählen oder erstellen, stellen Sie sicher, dass die Vorgabe dasselbe Seitenverhältnis wie die primäre Videodatei hat. Das *Seitenverhältnis* ist das Verhältnis von Breite und Höhe des Videos.

Um das Seitenverhältnis einer Videodatei zu bestimmen, rufen Sie die Metadaten der Datei ab und notieren Sie die Breite und Höhe der Datei (siehe [Abrufen der Metadaten einer Datei](uploading-encoding-videos.md#obtaining_a_file_s_metadata)). Berechnen Sie das Seitenverhältnis anhand der folgenden Formel:

Breite/Höhe = Seitenverhältnis

In der folgenden Tabelle sind die Formelergebnisse und die zugehörigen gebräuchlichen Seitenverhältnisse angegeben:

| Formelergebnis | Seitenverhältnis |
| --- | --- |
| 1,33 | 4 :3 |
| 0,75 | 3 :4 |
| 1,78 | 16 :9 |
| 0,56 | 9 :16 |

Beispielsweise hat ein Video mit einer Breite × Höhe von 1.440 und einem Seitenverhältnis von 1.440 zu 1.080 bzw. 1,33. In diesem Fall wählen Sie eine Videokodierungsvorgabe mit einem Seitenverhältnis von 4:3 aus, um die Videodatei zu kodieren.

### Datenrate {#data-rate}

Die *Datenrate* (auch als *Bitrate* bezeichnet) ist die Menge an Daten, die für eine Videowiedergabe von einer einzigen Sekunde Dauer kodiert wird. Die Datenrate wird in Kilobit pro Sekunde (Kbit/s) gemessen.

>[!NOTE]
>
>Da alle Codecs eine verlustreiche Komprimierung verwenden, ist die Datenrate der wichtigste Faktor für die Videoqualität. Bei einer verlustreichen Komprimierung gilt, dass die Qualität umso stärker beeinträchtigt wird, je mehr Sie eine Videodatei komprimieren. Aus diesem Grund ist die Qualität der komprimierten Datei umso niedriger, je niedriger die Datenrate ist (vorausgesetzt, dass alle anderen Merkmale wie Auflösung, Bildfrequenz und Codec gleich sind).

Achten Sie bei der Auswahl einer Videokodierungsvorgabe darauf, die Verbindungsgeschwindigkeit des Zielendbenutzers zu berücksichtigen. Wählen Sie eine Vorgabe mit einer Datenrate, die 80 Prozent dieser Geschwindigkeit beträgt. Wenn die Verbindungsgeschwindigkeit des Ziel-Endbenutzers beispielsweise 1000 kBit/s beträgt, hat die optimale Vorgabe eine Videodatenrate von 800 kBit/s.

In dieser Tabelle sind die Datenraten typischer Verbindungsgeschwindigkeiten aufgeführt.

| Geschwindigkeit (Kbit/s) | Verbindungstyp |
| --- | --- |
| 256 | Einwählverbindung. |
| 800 | Typische Mobilverbindung. Für diese Verbindung sollten Sie für eine wahre 3G-Erfahrung eine Datenrate zwischen 400 und maximal 800 Kbit/s veranschlagen. |
| 2000 | Typische Breitband-Desktop-Verbindung. Für diese Verbindung sollten Sie eine Datenrate zwischen 800 und 2000 Kbit/s veranschlagen, wobei die meisten Datenraten zwischen 1200 und 1500 Kbit/s liegen. |
| 5000 | Typische Hochgeschwindigkeits-Breitbandverbindung. Eine Kodierung in diesem oberen Bereich wird nicht empfohlen, da eine Videoübertragung in dieser Geschwindigkeit für die meisten Kunden nicht verfügbar ist. |

### Auflösung {#resolution}

*Auflösung* beschreibt die Höhe und Breite einer Videodatei in Pixel. Die meisten Quellvideos werden mit hoher Auflösung gespeichert (z. B. 1920 × 1080). Zu Streaming-Zwecken werden Quellvideos in eine niedrigere Auflösung komprimiert (640 × 480 oder weniger).

Auflösung und Datenrate sind zwei eng miteinander verknüpfte Faktoren, die die Videoqualität bestimmen. Um stets die gleiche Videoqualität aufrechtzuerhalten, muss bei einer Erhöhung der Pixelanzahl in einer Videodatei (d. h. bei einer höheren Auflösung) auch eine entsprechend höhere Datenrate verwendet werden. Betrachten Sie beispielsweise die Anzahl der Pixel pro Frame in einer Videodatei mit einer Auflösung von 320 × 240 und einer Videodatei mit einer Auflösung von 640 × 480:

| Auflösung | Pixel pro Bild |
| --- | --- |
| 320 × 240 | 76.800 |
| 640 × 480 | 307.200 |

Die Datei mit 640 × 480 hat viermal so viele Pixel pro Frame. Um dieselbe Datenrate für diese beiden Auflösungen zu erreichen, wenden Sie eine vierfache Komprimierung auf die Datei mit 640 × 480 an, was die Videoqualität beeinträchtigen kann. Daher führt eine Videodatenrate von 250 kBit/s zu einer hohen Anzeigequalität bei einer Auflösung von 320 × 240, aber nicht bei einer Auflösung von 640 × 480.

>[!NOTE]
>
>Im Allgemeinen gilt: Je höher die verwendete Datenrate, desto besser sieht das Video aus, und je höher die verwendete Auflösung, desto höher ist die benötigte Datenrate, um die Anzeigequalität aufrechtzuerhalten (im Vergleich zu niedrigeren Auflösungen).

Da Auflösung und Datenrate eng miteinander verbunden sind, haben Sie beim Kodieren von Video zwei Optionen:

* Wählen Sie eine Datenrate und kodieren Sie dann mit der höchsten Auflösung, die am besten mit der gewählten Datenrate aussieht.
* Wählen Sie eine Auflösung und kodieren Sie dann mit der Datenrate, die zum Erzielen von hochwertigem Video mit der gewählten Auflösung erforderlich ist.

Wenn Sie eine Videokodierungsvorgabe für die primäre Videodatei auswählen (oder erstellen), verwenden Sie diese Tabelle, um die richtige Auflösung auszuwählen:

| Auflösung | Höhe (Pixel) | Bildschirmgröße |
| --- | --- | --- |
| 240p | 240 | Winziger Bildschirm |
| 300p | 300 | Kleine Bildschirme, wie sie bei Mobilgeräten typisch sind |
| 360p | 360 | Kleiner Bildschirm |
| 480p | 480 | Mittelgroßer Bildschirm |
| 720p | 720 | Großer Bildschirm |
| 1080p | 1080 | Großer HD-Bildschirm |

### FPS (Frames pro Sekunde) {#fps-frames-per-second}

In den USA und Japan werden die meisten Videos mit 29,97 Frames pro Sekunde (FPS) aufgenommen, in Europa mit 25 FPS. Der Film wird mit 24 FPS gedreht.

Wählen Sie eine Videokodierungsvorgabe aus, die der FPS-Rate der primären Videodatei entspricht. Wenn Ihr Primärvideo beispielsweise 25 FPS aufweist, wählen Sie eine Kodierungsvorgabe mit 25 FPS. Standardmäßig wird bei allen benutzerdefinierten Codierungen der FPS der primären Videodatei verwendet. Daher ist es nicht erforderlich, beim Erstellen einer Videokodierungsvorgabe die FPS-Einstellung anzugeben.

### Maße für die Videokodierung {#video-encoding-dimensions}

Um optimale Ergebnisse zu erzielen, wählen Sie Kodierungsmaße, bei denen die Größe des Quellvideos ein ganzes Vielfaches aller Ihrer kodierten Videos aufweist.

Um dies zu berechnen, dividieren Sie die ursprüngliche Breite durch die kodierte Breite; dies ergibt das Breitenverhältnis. Dividieren Sie anschließend die ursprüngliche Höhe durch die kodierte Höhe; dies ergibt das Höhenverhältnis.

Wenn das resultierende Verhältnis eine Ganzzahl ist, bedeutet dies, dass das Video optimal skaliert ist. Wenn das resultierende Verhältnis keine Ganzzahl ist, beeinträchtigt dies die Videoqualität, weil verbleibende Pixelartefakte auf dem Bildschirm sichtbar sind. Dies wird insbesondere dann deutlich, wenn das Video Text enthält.

Nehmen wir als Beispiel an, dass Ihr Quellvideo 1920 × 1080 ist. In der folgenden Tabelle werden die optimalen Kodierungseinstellungen für drei kodierte Videos aufgeführt.

| Videotyp | Breite × Höhe | Breitenverhältnis | Höhenverhältnis |
| --- | --- | --- | --- |
| Quelle | 1 920 × 1 080 | 1 | 1 |
| Kodiert | 960 × 540 | 2 | 2 |
| Kodiert | 640 × 360 | 3 | 3 |
| Kodiert | 480 × 270 | 4 | 4 |

### Kodiertes Videodateiformat {#encoded-video-file-format}

Adobe Dynamic Media Classic empfiehlt die Verwendung von MP4 H.264-Videokodierungsvorgaben. Da MP4-Dateien den H.264-Videocodec verwenden, wird hochwertiges Videomaterial in einer komprimierten Datei geliefert.

## Arbeiten mit Videokodierungsvorgaben {#working-with-video-encoding-presets}

Primäre Videodateien, die mit Videoproduktionsgeräten und Videobearbeitungssoftware erstellt wurden, sind oft zu groß und nicht im richtigen Format für die Bereitstellung an Online-Ziele. Um digitales Videomaterial in geeignete Formate für verschiedene Ausgabemedien zu konvertieren, können Sie die Videodateien *transkodieren* (ein Vorgang, der auch als *Kodieren* bezeichnet wird). Während des Kodierungsprozesses wird das Video auf eine kleinere, effiziente Dateigröße komprimiert. Dies erfolgt für eine optimale Bereitstellung im Internet und auf Mobilgeräten.

Siehe [Hochladen und Kodieren von Videos](uploading-encoding-videos.md#uploading-and-encoding-videos).

Adobe Dynamic Media Classic bietet eine Bibliothek mit vordefinierten Videokodierungsvorgaben, die die gängigsten Kodierungseinstellungen widerspiegeln, die heute verwendet werden. Diese Kodierungsvorgaben wurden für die Wiedergabe auf den jeweiligen Zieldisplays optimiert. Außerdem können Administratoren eigene Videokodierungsvorgaben erstellen, um die Größe und Wiedergabe von Videos für Endbenutzer anzupassen. Alle Videokodierungsvorgaben, unabhängig davon, ob sie vorkonfiguriert in Adobe Dynamic Media Classic oder benutzerdefiniert sind, geben Videos im MP4-Dateiformat aus.

Über den Anzeigebereich „Video-Vorgaben“ können Administratoren Videokodierungen einrichten und verwalten. Sie haben folgende Möglichkeiten:

* Aktivieren und Deaktivieren von Videokodierungsvorgaben.
* Erstellen einer Videokodierungsvorgabe.
* Bearbeiten von Videokodierungsvorgaben.
* Löschen von Videovorgaben.

Jedes Video, das Sie in Adobe Dynamic Media Classic hochladen oder in Adobe Dynamic Media Classic kodieren, wird als „Video“ behandelt. Diese Asset-Bezeichnung bedeutet, dass Sie das Video für die Wiedergabe auf Desktops, mobilen Geräten oder beiden bereitstellen können. Sie können beispielsweise eine Vorschau dieser Videotypen in Adobe Dynamic Media Classic anzeigen. Sie können auch URLs (mithilfe der Funktion „URL kopieren“) sowie Einbettungscode (mithilfe der Funktion „Code einbetten“) für die Verwendung mit Video-Playern, auf Websites usw. generieren.

Siehe [Vorschau von Videos in einem Video-Viewer](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

Siehe [Verknüpfen einer Video-URL mit einer mobilen Site oder einer Website](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

Siehe [Einbetten des Video-Viewers auf einer Web-Seite](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

Für Video-Assets, die Sie in Adobe Dynamic Media Classic hochladen und kodieren, werden Videos im folgenden Dateiformat bereitgestellt:

**MP4 H.264** Verwenden Sie MP4-Dateien für Folgendes:

* HTTP Dynamic Streaming an Desktops.
* HLS (HTTP Live Streaming, Streaming-Protokoll von Apple).
* Progressive Videobereitstellung auf Android™, BlackBerry® und Windows® Mobilgeräten.

Alle anderen Videoformate und Codecs werden als &quot;Primäre Videos“ behandelt. Diese Asset-Bezeichnung bedeutet, dass das Video eine Quellvideodatei ist und nicht für die Wiedergabe auf Desktops oder mobilen Geräten verwendet werden kann. Sie können diese Videotypen beispielsweise nicht in Adobe Dynamic Media Classic in der Vorschau anzeigen. Sie können keine Copy-URLs oder Embed-Code für die Verwendung in Video-Playern, auf Websites usw. generieren.

### Filtern der Liste von Videokodierungsvorgaben {#filtering-the-list-of-video-encoding-presets}

Die Seite „Videovorgaben“ und die Seite „Adaptive Videovorgaben“ bestehen aus einer Tabelle, in der der aktive Status, der Name der Vorgabe, das vorgesehene Wiedergabegerät, die Videogröße und die Datenrate jeder Videovorgabe aufgelistet sind.

Sie können diese Liste anpassen, indem Sie den Filter „Beide“, „Aktiv“ oder „Inaktiv“ auswählen, um entweder alle Videovorgaben anzuzeigen oder die Liste auf aktive bzw. inaktive Vorgaben zu beschränken.

Sie können auch basierend auf einem Wiedergabegerät filtern, um die Liste auf Videovorgaben zu beschränken, die für alle Geräte, Desktops, Mobilgeräte oder Tablets entwickelt wurden.

**So filtern Sie die Liste der Videokodierungsvorgaben:**

1. Wechseln Sie in Adobe Dynamic Media Classic in der globalen Navigationsleiste zu **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Videovorgaben]** > **[!UICONTROL Adaptive Videovorgaben]** oder **[!UICONTROL Einfache Kodierungsvorgaben]**.

   Die Seiten für adaptive Videovorgaben und einzelne Kodierungsvorgaben enthalten eine Tabelle, in der der aktive Status, der Vorgabenname, das vorgesehene Wiedergabegerät, die Videoabmessungen und die Datenrate jeder Videovorgabe aufgeführt sind.

1. Verwenden Sie auf der Seite „Einzelne Kodierungsvorgaben“ mit der Bezeichnung „Video-Vorgaben“ die beiden Dropdownlisten auf der Symbolleiste „Videovorgaben“, um die Tabelle basierend auf dem aktiven Status und dem Wiedergabegerät anzupassen.

   * Wählen Sie in der ersten, schmaleren Dropdownliste die Option **[!UICONTROL Beide]**, um alle Videovorgaben anzuzeigen, oder wählen Sie entweder **[!UICONTROL Aktiv]** oder **[!UICONTROL Inaktiv]**, um die Liste auf die Vorgaben zu beschränken, die entweder aktiv oder inaktiv sind.
   * Wählen in der zweiten, breiteren Dropdownliste eine Wiedergabegerät aus, um die Liste auf Videovorgaben zu beschränken, die für die Wiedergabe von Videos auf Desktops entwickelt wurden. Alternativ wählen Sie Videovorgaben aus, die für die Wiedergabe von Videos auf mobilen Geräten oder Tablets entwickelt wurden.

### Aktivieren oder Deaktivieren von Videokodierungsvorgaben {#activating-or-deactivating-video-encoding-presets}

Aktivierte Videovorgaben werden im Dialogfeld „Upload-Auftragseinstellungen“ angezeigt. Das Dialogfeld wird angezeigt, wenn ein Benutzer beim Hochladen Videodateien hochlädt. Sie können in einer Liste oder aktivierten Kodierungsvorgaben wählen.

1. Navigieren Sie in Adobe Dynamic Media Classic in der globalen Navigationsleiste zu **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Videovorgaben]**.
1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Adaptive Videovorgaben]** aus.
   * Wählen Sie **[!UICONTROL Einzelne Kodierungsvorgaben]** aus.

1. Führen Sie einen der folgenden Schritte aus:

   * Um eine Videovorgabe zu aktivieren, aktivieren Sie auf der Seite „Vorgaben“ unter der Spalte „Aktiv“ das Kontrollkästchen neben einem Vorgabenamen.
   * Um eine Videovorgabe zu deaktivieren, deaktivieren Sie das Kontrollkästchen neben der Videovorgabe, die Sie inaktiv machen möchten.

     >[!NOTE]
     >
     >Inaktive Videovorgaben werden im Dialogfeld „Upload-Auftragseinstellungen“ nicht angezeigt.

1. Klicken Sie unten rechts auf der Seite auf **[!UICONTROL Schließen]**.

### Hinzufügen oder Bearbeiten einer Videokodierungsvorgabe {#adding-or-editing-a-video-encoding-preset}

Sie können eigene benutzerdefinierte Videovorgaben mit einer Kodierung erstellen und sie zur Tabelle „Videovorgaben“ hinzufügen. Sie können auch alle vordefinierten Videovorgaben für die Einzelkodierung ändern, die im Lieferumfang von Adobe Dynamic Media Classic enthalten sind, sofern Sie die bearbeitete Vorgabe unter einem neuen Namen speichern.

Adobe Dynamic Media Classic hat Höchstwerte für die Zieldatenrate, Auflösungshöhe und Auflösungsbreite festgelegt, um ein ordnungsgemäßes Wiedergabeerlebnis zu gewährleisten. Beim Überschreiten dieser Grenzwerte werden Warnmeldungen angezeigt, die wie folgt lauten:

* Für die Computerwiedergabe gelten folgende Grenzwerte: (Breite/16) &#42; (Höhe/16) &lt; 8192.
* Für die Wiedergabe auf Mobilgeräten gelten folgende Beschränkungen: (Breite/16) &#42; (Höhe/16) &lt; 660; Ziel-Datenrate &lt; 4000.
* Für die Tablet-Wiedergabe gelten folgende Grenzwerte: (Breite/16) &#42; (Höhe/16) &lt; 3600.

**So fügen Sie eine Videokodierungsvorgabe hinzu oder bearbeiten sie:**

1. Navigieren Sie in Adobe Dynamic Media Classic in der globalen Navigationsleiste zu **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Videovorgaben]**.
1. Wählen Sie **[!UICONTROL Einzelne Kodierungsvorgaben]** aus.
1. Auf der Seite „Video-Vorgaben“ führen Sie einen der folgenden Schritte aus:

   * Klicken Sie in der Symbolleiste „Videovorgaben **[!UICONTROL auf „Hinzufügen]**, um eine Videovorgabe hinzuzufügen.
   * Wählen Sie eine Video-Vorgabe aus. Klicken Sie in der Symbolleiste auf **[!UICONTROL Bearbeiten]**.

     Sie können vordefinierte Adobe Dynamic Media Classic-Vorgaben nicht bearbeiten. Sie können eine Vorgabe nur aus einer vorhandenen Vorgabe erstellen, indem Sie **[!UICONTROL Speichern unter]** auswählen.

1. Legen Sie auf der Seite „Video-Vorgabe hinzufügen“ oder „Video-Vorgabe bearbeiten“ die Optionen für die Video-Vorgaben wie folgt fest.

   Die empfohlenen Einstellungen finden Sie unter [Bewährte Vorgehensweise für die Videokodierung](uploading-encoding-videos.md#best-practices-for-video-encoding).

   | Option „Video-Vorgabe“ | Beschreibung |
   | --- | --- |
   | Vorgabenname | Geben Sie einen beschreibenden Namen für die Video-Vorgabe ein. Der hier eingegebene Name wird im Dialogfeld „Upload-Auftragsoptionen“ angezeigt, in dem Benutzer Optionen zum Transkodieren auswählen. |
   | Beschreibung | Beschreiben Sie die Video-Vorgabe. Was Sie eingeben, wird als QuickInfo angezeigt. Wenn Benutzer Transkodierungsoptionen auswählen, wird die QuickInfo angezeigt, wenn sie den Mauszeiger über den Namen der Vorgabe im Dialogfeld Upload-Auftragsoptionen bewegen. |
   | Wiedergabegerät | Wählen Sie das Gerät aus, auf dem das Video wiedergegeben werden soll. Die Optionen sind Computer (Desktops), Mobil (iPhone, iPad, Android™) oder Tablet (nur iPad). Diese Einstellung bestimmt automatisch den entsprechenden Video- und Audio-Codec, der bei der Kodierung verwendet wird. |
   | Zieldatenrate | Geben Sie die durchschnittliche Verbindungsgeschwindigkeit des Endbenutzers in Kilobit pro Sekunde ein. Sie können die Datenrate eingeben oder zur Eingabe den Regler ziehen. Für die Verbindungsgeschwindigkeit werden typische Geschwindigkeiten für Breitband-, DSL-, mobile und DFÜ-Verbindungen aufgelistet. Diese Einstellung legt automatisch die kombinierte Video- und Audiodatenrate fest. Anders ausgedrückt, die Datenmenge, die kodiert wird, um eine einzige Sekunde für die Videowiedergabe zu generieren. Je höher die Datenrate, desto besser ist die Qualität des resultierenden Videos. Ist die Datenrate jedoch zu hoch, kommt es zu erheblich größeren Dateien und dadurch zu einer Beeinträchtigung der Wiedergabe bei geringeren Bandbreiten. Es empfiehlt sich, einen Kompromiss zwischen hohen und niedrigen Datenraten einzugehen. Versuchen Sie, ein qualitativ hochwertiges Wiedergabeerlebnis zu schaffen, ohne sich über Benutzer mit engen Bandbreiten zu ärgern. |
   | Seitenverhältnis | Das Seitenverhältnis ist das Verhältnis zwischen Breite und Höhe des Videos. Die ersten beiden Seitenverhältnisse in der Liste werden häufig verwendet, um Video horizontal anzuzeigen:<ul><li> 4:3: Wird für fast alle Standard Definition TV-Broadcast-Inhalte verwendet.</li><li>16:9: Wird für fast alle Widescreen-Inhalte und Filme auf High-Definition-Fernsehen (HDTV) verwendet.</li><li>Automatische Skalierung: (Standard) Eine Vorgabe für die einzelne Kodierung, die mit jedem Seitenverhältnis verwendet werden kann, um Videos für die Bereitstellung auf Mobilgeräten, Tablets und Desktops zu erstellen. Hochgeladene Quellvideos, die mit dieser Vorgabe kodiert wurden, weisen eine feste Höhe auf. Die Breite wird jedoch automatisch skaliert, um das Seitenverhältnis des Videos beizubehalten (Verhältnis Breite zu Höhe).</li><li>Benutzerdefiniert: Wird verwendet, wenn Sie eine nicht standardmäßige Videogröße definieren möchten.</li><li>Das Seitenverhältnis, das Sie auswählen, bestimmt die Breite und Höhe für die Auflösungsgröße. Die Breite und Höhe werden automatisch auf das richtige Seitenverhältnis skaliert.</li></ul> |
   | Auflösung | Die Auflösungsgröße, ausgedrückt als Anzahl der Pixel durch die Anzahl der Pixel hoch, bestimmt die Größe. Geben Sie eine Breite und einen Höhenwert in Pixel ein oder ziehen Sie den Regler, um diese Werte einzugeben. Für die Auflösung werden typische Werte aufgelistet. Der Wert für die Breite und die Höhe werden automatisch an das ausgewählte Seitenverhältnis angepasst. Wenn Sie beispielsweise 4:3 als Seitenverhältnis auswählen und 400 für die Breite eingeben, wird automatisch 300 für die Höhe eingegeben. Wenn Sie für die Einstellung „Seitenverhältnis“ die Option „Automatisch skalieren“ ausgewählt haben, wird der Wert für „Breite“ für die Auflösungsgröße automatisch auf „Automatisch“ festgelegt. Wählen Sie **[!UICONTROL Vorschau]** aus, um ein Browser-Fenster zu öffnen und Ihre Auflösungsoptionen dort anzuzeigen. |
   | Kodierungsdateisuffix | Geben Sie ein Suffix ein. Dieses Suffix wird dem Namen der Videodatei nach erfolgter Kodierung angehängt. Der Name darf Bindestriche und Unterstriche enthalten, jedoch keine Leerzeichen oder Sonderzeichen. |
   | Andere Einstellungen | Adobe Dynamic Media Classic bestimmt alle anderen Kodierungseinstellungen automatisch gemäß den Richtlinien für die Best-Practice-Kodierung. |

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Speichern]**, wenn Sie eine Videovorgabe hinzugefügt oder bearbeitet haben.
   * Wählen Sie **[!UICONTROL Speichern unter]**, wenn Sie eine Videovorgabe hinzugefügt haben, indem Sie mit einer vorhandenen Vorgabe beginnen.

### Löschen einer Videokodierungsvorgabe {#delete-a-video-encoding-preset}

Administratoren können benutzerdefinierte Video-Vorgaben löschen. Videovorgaben, die mit Adobe Dynamic Media Classic geliefert werden, können nicht gelöscht werden.

1. Navigieren Sie in Adobe Dynamic Media Classic in der globalen Navigationsleiste zu **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Videovorgaben]**.
1. Wählen Sie **[!UICONTROL Einzelne Kodierungsvorgaben]** aus.
1. Wählen Sie auf der Seite „Video-Vorgaben“ die Vorgabe aus, die Sie nicht mehr benötigen und entfernen möchten.
1. Klicken Sie in der Symbolleiste „Videovorgaben“ auf **[!UICONTROL Löschen]**.
1. Klicken Sie im Dialogfeld Vorgabe löschen auf **[!UICONTROL Löschen]**.

>[!MORELIKETHIS]
>
>* [Schnellstart: Video in Adobe Dynamic Media Classic](quick-start-video.md#quick-start-video)
>* [Videos hochladen und kodieren](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [Arbeiten mit Video-Viewer-Vorgaben](previewing-videos-video-viewer.md#working-with-video-viewer-presets)
>* [Videovorgaben](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) Schulungsvideo
