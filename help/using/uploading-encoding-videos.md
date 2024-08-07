---
title: Hochladen und Kodieren von Videos
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
source-wordcount: '3989'
ht-degree: 40%

---

# Hochladen und Kodieren von Videos{#uploading-and-encoding-videos}

Um einzelne Video- oder Adaptive Video-Sets für die Bereitstellung im Web oder auf Mobilgeräten zu erstellen, laden Sie zunächst Ihre primären Videodateien in Adobe Dynamic Media Classic hoch. Adobe Dynamic Media Classic kodiert Videos in das MP4-Format und veröffentlicht Videos in den folgenden Dateiformaten:

* **MP4**: Adobe Dynamic Media Classic empfiehlt MP4 als bevorzugtes Videodateiformat. Verwenden Sie MP4-Dateien für Folgendes:

   * HTTP Dynamic Streaming an Desktops.
   * HTTP Live Streaming (Streaming-Protokoll von Apple).
   * Progressive Videowiedergabe auf Mobilgeräten von Android™, BlackBerry® und Windows®

  Adobe Dynamic Media Classic bietet zwei Workflows zum Hochladen von Videodateien:

* **Vorkodierte Videos**: Sie laden MP4-Dateien direkt in Adobe Dynamic Media Classic hoch. Bei diesem Arbeitsablauf werden Dateien zum Zeitpunkt des Hochladens nicht kodiert. Die Dateien werden vorkodiert und so für die Ausgabe auf dem Desktop und mobilen Geräten vorbereitet.

* **Primäre Quellvideos**: Laden Sie die Primär-Quellvideodateien hoch und kodieren Sie sie beim Hochladen in MP4-Dateien. Kodierte Videos werden im Bedienfeld &quot;Durchsuchen&quot;mit &quot;Video&quot;beschriftet. Adobe Dynamic Media Classic unterstützt die Kodierung von Videodateien in vielen Formaten.

   * Stellen Sie sicher, dass die Primärquellen-Videodateien, die Sie kodieren möchten, unterstützt werden.

     Siehe [Unterstützte Videodateitypen für die Kodierung](uploading-encoding-videos.md#supported-video-file-types-for-encoding).

   * Wählen Sie eine Videokodierungsvorgabe aus.

     Siehe [Video-Vorgaben zum Kodieren von Videodateien](application-setup.md#video-presets-for-encoding-video-files).

     Siehe [Bewährte Vorgehensweisen für die Videokodierung](uploading-encoding-videos.md#best-practices-for-video-encoding).

Adobe Dynamic Media Classic generiert auch Videominiaturen. Erfahren Sie mehr über Videominiaturen, das Abrufen ihrer URLs und das Bearbeiten von Standbildern.

Siehe [Arbeiten mit Videominiaturen](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**So laden Sie Videos hoch und kodieren sie:**

Führen Sie einen der folgenden Schritte aus.

*Wenn Ihre Videos bereits kodiert sind*

1. Wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Upload]** aus.
1. Wählen Sie auf der Seite Hochladen die Registerkarte **[!UICONTROL From Desktop]** aus.
1. Wählen Sie auf der Seite &quot;Hochladen&quot;im Bedienfeld **[!UICONTROL Dateien zum Hochladen auswählen]** die Option **[!UICONTROL Durchsuchen]**, navigieren Sie zu einer MP4-Videodatei und wählen Sie dann **[!UICONTROL Öffnen]** aus.
1. Wählen Sie im ausgewählten Bereich **[!UICONTROL Ordnerziel]** einen Ordner für die hochgeladene Datei aus.
1. Stellen Sie auf der Seite &quot;Hochladen&quot;sicher, dass **[!UICONTROL Publish nach dem Hochladen]** aktiviert ist.
1. Wählen Sie **[!UICONTROL Upload starten]** aus.

*Wenn Sie Ihre Videos mit Adobe Dynamic Media Classic kodieren möchten*

1. Wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Upload]** aus.
1. Wählen Sie auf der Seite Hochladen die Registerkarte **[!UICONTROL From Desktop]** aus.
1. Wählen Sie im Bedienfeld **[!UICONTROL Hochzuladende Dateien auswählen]** die Option **[!UICONTROL Durchsuchen]**, navigieren Sie zu einer Primär-Quellvideodatei und wählen Sie dann **[!UICONTROL Öffnen]** aus.
1. Wählen Sie im ausgewählten Bereich **[!UICONTROL Ordnerziel]** einen Ordner für die hochgeladene Datei aus.
1. Wählen Sie in der rechten unteren Ecke der Seite **[!UICONTROL Auftragsoptionen]**,
1. Erweitern Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;den Eintrag **[!UICONTROL eVideo-Optionen]** und führen Sie dann einen der folgenden Schritte aus:

   * Die Best Practice ist, **[!UICONTROL Adaptive Videokodierung]** auszuwählen. Siehe [Adaptive Video (Standard)](application-setup.md#adaptive-video-default).
   * Optional. Wenn Sie einzelne Kodierungseinstellungen verwenden möchten, erweitern Sie **[!UICONTROL Einzelne Kodierungsvorgaben]** und wählen Sie dann die gewünschten Kodierungsoptionen für Desktop, Mobilgerät und Tablet aus.
Siehe [ Vorgaben für die Videokodierung für Desktop-PCs](application-setup.md#desktop-video-encoding-presets), [Vorgaben für die Videokodierung für Mobilgeräte](application-setup.md#mobile-video-encoding-presets), [Vorgaben für die Videokodierung für Tablets](application-setup.md#tablet-video-encoding-presets).
1. Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL Speichern]**.
1. Stellen Sie auf der Seite &quot;Hochladen&quot;sicher, dass **[!UICONTROL Publish nach dem Hochladen]** aktiviert ist.
1. Wählen Sie auf der Seite &quot;Hochladen&quot;in der rechten unteren Ecke **[!UICONTROL Upload starten]** aus.

*Wenn Sie eine zuvor hochgeladene Videodatei neu kodieren möchten,*

1. Navigieren Sie in Adobe Dynamic Media Classic im Bedienfeld Durchsuchen zum Video und wählen Sie es aus.
1. Wechseln Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Neuverarbeitung]**.
1. Erweitern Sie im Dialogfeld &quot;Assets erneut verarbeiten&quot;den Eintrag **[!UICONTROL eVideo-Optionen]** und führen Sie dann einen der folgenden Schritte aus:
   * Es empfiehlt sich, die folgende Methode zu verwenden. Wählen Sie **Adaptives Video** aus.
Siehe [Adaptive Video (Standard)](application-setup.md#adaptive-video-default).
   * Optional. Wenn Sie einzelne Kodierungseinstellungen verwenden möchten, erweitern Sie **[!UICONTROL Einzelne Kodierungsvorgaben]** und wählen Sie dann die gewünschten Kodierungsoptionen für Desktop, Mobilgerät und Tablet aus.
Siehe [ Vorgaben für die Videokodierung für Desktop-PCs](application-setup.md#desktop-video-encoding-presets), [Vorgaben für die Videokodierung für Mobilgeräte](application-setup.md#mobile-video-encoding-presets), [Vorgaben für die Videokodierung für Tablets](application-setup.md#tablet-video-encoding-presets).
1. Wählen Sie im Dialogfeld &quot;Assets erneut verarbeiten&quot;die Option **[!UICONTROL Senden]**.

Wenn Sie eine Kodierungsvorgabe für adaptive Videos oder mehrere Vorgaben für die einmalige Kodierung verwenden, ist das Ergebnis ein adaptives Videoset, das automatisch mit mehreren Videokodierungen erstellt wird. Sie können auch manuell ein adaptives Videoset erstellen, indem Sie die einzelnen Videos auswählen.

Wenn Sie ein adaptives Videoset entweder automatisch oder manuell erstellen, werden nur MP4- und M4V-Dateien erzeugt.

## Unterstützte Videodateitypen für die Kodierung {#supported-video-file-types-for-encoding}

In der folgenden Tabelle sind die Videodateitypen (mit zulässigen Video-Codecs) aufgelistet, die Sie beim Hochladen in das Format MP4 oder OGV kodieren lassen können. Die Tabelle enthält Dateiformate und Codecs:

* **Videodateiformate**: Ähnlich wie bei ZIP-Dateien bestimmt das Videodateiformat, wie Dateien in der Videodatei enthalten sind. Eine Videodatei besteht in der Regel aus mehreren Spuren – einer Videospur (ohne Audio) und einer oder mehreren Audiospuren (ohne Video) –, die miteinander verknüpft und synchronisiert sind. Das Videodateiformat legt fest, wie diese unterschiedlichen Datenspuren in der Videodatei organisiert sind.

* **Video-Codecs**: Ein Video-Codec beschreibt den Algorithmus, mit dem ein Video kodiert wird. Ein Video-Player dekodiert das Video entsprechend dem Codec und zeigt dann eine Reihe von Bildern, auch Frames oder Bildfelder genannt, auf dem Bildschirm an. Codecs reduzieren die Datenmenge, die in Videodateien gespeichert werden muss, um das Video wiedergeben zu können. Statt Informationen zu jedem einzelnen Frame werden nur Informationen zu den Unterschieden zwischen einem Frame und dem nächsten gespeichert. Da sich die meisten Videos von einem Frame zum nächsten kaum ändern, ermöglichen Codecs hohe Komprimierungsraten, was zu kleineren Dateigrößen führt.

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

Im Folgenden finden Sie Best Practices für die Kodierung von Quellvideodateien in Adobe Dynamic Media Classic.

<!-- THE FOLLOWINGS LINKS APPEAR TO BE DEAD AND THE CONTENT COMPLETELY LOST. THE GO URL DOESN'T EVEN WORK ANYMORE.
For advice about video encoding, see the following:

* Article: [Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution][www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en). THIS MATERIAL WAS FOUND ON A THIRD PARTY WEBSITE HERE: https://streaminglearningcenter.com/articles/streaming-101-the-basics-codecs-bandwidth-data-rate-and-resolution.html MATERIAL IS GOOD BUT DO NOT LINK TO IT
* Video: [Video Encoding Basics][www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en). -->

### Quell-Videodateien {#source-video-files}

Beim Kodieren einer Videodatei sollten Sie eine Quell-Videodatei mit der höchstmöglichen Qualität verwenden. Vermeiden Sie es, Dateien zu nutzen, die bereits zuvor kodiert wurden, da diese schon komprimiert sind. Eine weitere Kodierung würde zu einem Video von minderwertiger Qualität führen.

In der folgenden Tabelle werden die empfohlene Größe, das Seitenverhältnis und die minimale Bitrate beschrieben, die Ihre Quellvideodateien bei der Kodierung aufweisen müssen:

| Größe | Seitenverhältnis | Minimale Bitrate |
| --- | --- | --- |
| 1024 X 768 | 4:3 | 4500 Kbit/s sind für die meisten Videos ausreichend. |
| 1280 X 720 | 16:9 | 3000: 6000 kBit/s, je nach Bewegungsdauer im Video. |
| 1920 X 1080 | 16:9 | 6000: 8000 kBit/s, je nach Bewegungsdauer im Video. |

### Abrufen der Metadaten einer Datei {#obtaining-a-file-s-metadata}

Sie können die Metadaten einer Datei abrufen, indem Sie die Metadaten in Adobe Dynamic Media Classic anzeigen, ein Video-Bearbeitungswerkzeug verwenden oder eine Anwendung zum Abrufen von Metadaten verwenden. Im Folgenden finden Sie Anweisungen zur Verwendung von MediaInfo, einer Drittanbieteranwendung, um die Metadaten einer Videodatei abzurufen:

1. Rufen Sie diese Webseite auf: [https://mediaarea.net/en/MediaInfo](https://mediaarea.net/en/MediaInfo).
1. Wählen Sie das Installationsprogramm für die GUI-Version aus und laden Sie es herunter. Befolgen Sie anschließend die Installationsanweisungen.
1. Klicken Sie nach der Installation mit der rechten Maustaste auf die Videodatei (nur Windows®) und wählen Sie MediaInfo aus oder öffnen Sie MediaInfo und ziehen Sie die Videodatei in die Anwendung. Es werden alle mit der Videodatei verknüpften Metadaten angezeigt, einschließlich Breite, Höhe und FPS.

### Seitenverhältnis {#aspect-ratio}

Wenn Sie eine Videokodierungsvorgabe für Ihre primäre Videodatei auswählen oder erstellen, achten Sie darauf, dass die Vorgabe dasselbe Seitenverhältnis wie die primäre Videodatei aufweist. Das *Seitenverhältnis* ist das Verhältnis von Breite und Höhe des Videos.

Um das Seitenverhältnis einer Videodatei zu ermitteln, rufen Sie die Metadaten der Datei ab und notieren Sie die Breite und Höhe der Datei (siehe [Metadaten einer Datei abrufen](uploading-encoding-videos.md#obtaining_a_file_s_metadata)). Berechnen Sie das Seitenverhältnis anhand der folgenden Formel:

Breite/Höhe = Seitenverhältnis

In der folgenden Tabelle sind die Formelergebnisse und die zugehörigen gebräuchlichen Seitenverhältnisse angegeben:

| Formelergebnis | Seitenverhältnis |
| --- | --- |
| 1,33 | 4:3 |
| 0,75 | 3:4 |
| 1,78 | 16:9 |
| 0,56 | 9:16 |

Beispiel: Ein Video mit einer Breite von 1440 × 1080 hat ein Seitenverhältnis von 1440/1080 oder 1,33. In diesem Fall wählen Sie eine Videokodierungsvorgabe mit einem Seitenverhältnis von 4:3 aus, um die Videodatei zu kodieren.

### Datenrate {#data-rate}

Die *Datenrate* (auch als *Bitrate* bezeichnet) ist die Datenmenge, die kodiert wird, um eine Sekunde Videowiedergabe zu bilden. Die Datenrate wird in Kilobit pro Sekunde (Kbit/s) gemessen.

>[!NOTE]
>
>Da alle Codecs eine verlustreiche Komprimierung verwenden, ist die Datenrate der wichtigste Faktor für die Videoqualität. Bei einer verlustreichen Komprimierung gilt, dass die Qualität umso stärker beeinträchtigt wird, je mehr Sie eine Videodatei komprimieren. Aus diesem Grund ist die Qualität der komprimierten Datei umso niedriger, je niedriger die Datenrate ist (vorausgesetzt, dass alle anderen Merkmale wie Auflösung, Bildfrequenz und Codec gleich sind).

Berücksichtigen Sie bei der Auswahl einer Videokodierungsvorgabe die Verbindungsgeschwindigkeit des Zielendbenutzers. Wählen Sie eine Vorgabe mit einer Datenrate, die 80 Prozent dieser Geschwindigkeit beträgt. Wenn die Verbindungsgeschwindigkeit des Zielendbenutzers beispielsweise 1000 kBit/s beträgt, ist die beste Vorgabe eine mit einer Videodatenrate von 800 kBit/s.

In dieser Tabelle sind die Datenraten typischer Verbindungsgeschwindigkeiten aufgeführt.

| Geschwindigkeit (Kbit/s) | Verbindungstyp |
| --- | --- |
| 256 | Einwählverbindung. |
| 800 | Typische Mobilverbindung. Für diese Verbindung sollten Sie für eine wahre 3G-Erfahrung eine Datenrate zwischen 400 und maximal 800 Kbit/s veranschlagen. |
| 2000 | Typische Breitband-Desktop-Verbindung. Für diese Verbindung sollten Sie eine Datenrate zwischen 800 und 2000 Kbit/s veranschlagen, wobei die meisten Datenraten zwischen 1200 und 1500 Kbit/s liegen. |
| 5000 | Typische Hochgeschwindigkeits-Breitbandverbindung. Eine Kodierung in diesem oberen Bereich wird nicht empfohlen, da eine Videoübertragung in dieser Geschwindigkeit für die meisten Kunden nicht verfügbar ist. |

### Auflösung {#resolution}

*Auflösung* beschreibt die Höhe und Breite einer Videodatei in Pixel. Die meisten Quellvideos werden mit hoher Auflösung gespeichert (z. B. 1920 × 1080). Zu Streaming-Zwecken werden Quellvideos in eine kleinere Auflösung komprimiert (640 × 480 oder kleiner).

Auflösung und Datenrate sind zwei eng miteinander verknüpfte Faktoren, die die Videoqualität bestimmen. Um stets die gleiche Videoqualität aufrechtzuerhalten, muss bei einer Erhöhung der Pixelanzahl in einer Videodatei (d. h. bei einer höheren Auflösung) auch eine entsprechend höhere Datenrate verwendet werden. Betrachten Sie beispielsweise die Anzahl der Pixel pro Frame in einer Videodatei mit der Auflösung 320 × 240 und der Auflösung 640 × 480:

| Auflösung | Pixel pro Bild |
| --- | --- |
| 320 × 240 | 76.800 |
| 640 × 480 | 307.200 |

Die Datei 640 × 480 hat viermal mehr Pixel pro Frame. Um dieselbe Datenrate für diese beiden Beispielauflösungen zu erzielen, wenden Sie die vierfache Komprimierung auf die Datei 640 × 480 an, wodurch die Qualität des Videos reduziert werden kann. Daher erzeugt eine Videodatenrate von 250 kBit/s eine hochwertige Wiedergabe mit einer Auflösung von 320 × 240, jedoch nicht mit einer Auflösung von 640 × 480.

>[!NOTE]
>
>Im Allgemeinen gilt: Je höher die verwendete Datenrate, desto besser wird Ihr Video angezeigt und desto höher die verwendete Auflösung. Je höher die Datenrate ist, desto höher muss die Anzeigequalität sein (im Vergleich zu niedrigeren Auflösungen).

Da Auflösung und Datenrate eng miteinander verbunden sind, haben Sie beim Kodieren von Video zwei Optionen:

* Wählen Sie eine Datenrate aus und kodieren Sie dann mit der höchsten Auflösung, die bei der von Ihnen gewählten Datenrate am besten angezeigt wird.
* Wählen Sie eine Auflösung und kodieren Sie dann mit der Datenrate, die zum Erzielen von hochwertigem Video mit der gewählten Auflösung erforderlich ist.

Wenn Sie eine Videokodierungsvorgabe für Ihre primäre Videodatei auswählen (oder erstellen), verwenden Sie diese Tabelle, um die richtige Auflösung auszuwählen:

| Auflösung | Höhe (Pixel) | Bildschirmgröße |
| --- | --- | --- |
| 240p | 240 | Winziger Bildschirm |
| 300p | 300 | Kleine Bildschirme, typisch für Mobilgeräte |
| 360p | 360 | Kleiner Bildschirm |
| 480p | 480 | Mittelgroßer Bildschirm |
| 720p | 720 | Großer Bildschirm |
| 1080p | 1080 | Großer HD-Bildschirm |

### FPS (Frames pro Sekunde) {#fps-frames-per-second}

In den USA und Japan wird das meiste Video mit 29,97 Frames pro Sekunde (FPS) aufgenommen, in Europa mit 25 FPS. Der Film wird mit 24 FPS aufgenommen.

Wählen Sie eine Videokodierungsvorgabe aus, die der FPS-Rate der primären Videodatei entspricht. Wenn Ihr Primärvideo beispielsweise 25 FPS aufweist, wählen Sie eine Kodierungsvorgabe mit 25 FPS. Standardmäßig verwenden alle benutzerdefinierten Kodierungen den FPS-Wert der Primär-Videodatei. Aus diesem Grund ist es nicht erforderlich, die FPS-Einstellung beim Erstellen einer Videokodierungsvorgabe anzugeben.

### Maße für die Videokodierung {#video-encoding-dimensions}

Um optimale Ergebnisse zu erzielen, wählen Sie Kodierungsmaße, bei denen die Größe des Quellvideos ein ganzes Vielfaches aller Ihrer kodierten Videos aufweist.

Um dies zu berechnen, dividieren Sie die ursprüngliche Breite durch die kodierte Breite; dies ergibt das Breitenverhältnis. Dividieren Sie anschließend die ursprüngliche Höhe durch die kodierte Höhe; dies ergibt das Höhenverhältnis.

Wenn das resultierende Verhältnis eine Ganzzahl ist, bedeutet dies, dass das Video optimal skaliert ist. Wenn das resultierende Verhältnis keine Ganzzahl ist, beeinträchtigt dies die Videoqualität, weil verbleibende Pixelartefakte auf dem Bildschirm sichtbar sind. Dies wird insbesondere dann deutlich, wenn das Video Text enthält.

Angenommen, Ihr Quellvideo hat das Format 1920 × 1080. In der folgenden Tabelle werden die optimalen Kodierungseinstellungen für drei kodierte Videos aufgeführt.

| Videotyp | Breite × Höhe | Breitenverhältnis | Höhenverhältnis |
| --- | --- | --- | --- |
| Quelle | 1920 × 1080 | 1 | 1 |
| Kodiert | 960 × 540 | 2 | 2 |
| Kodiert | 640 × 360 | 3 | 3 |
| Kodiert | 480 × 270 | 4 | 4 |

### Kodiertes Videodateiformat {#encoded-video-file-format}

Adobe Dynamic Media Classic empfiehlt die Verwendung von MP4 H.264-Videokodierungsvorgaben. Da MP4-Dateien den H.264-Videocodec verwenden, wird hochwertiges Videomaterial in einer komprimierten Datei geliefert.

## Arbeiten mit Videokodierungsvorgaben {#working-with-video-encoding-presets}

Primäre Videodateien, die mit Videoproduktionsgeräten und Videobearbeitungssoftware erstellt wurden, sind häufig zu groß und nicht im richtigen Format für die Bereitstellung an Online-Zielorte. Um digitales Videomaterial in geeignete Formate für verschiedene Ausgabemedien zu konvertieren, können Sie die Videodateien *transkodieren* (ein Vorgang, der auch als *Kodieren* bezeichnet wird). Während des Kodierungsprozesses wird das Video in eine kleinere, effiziente Dateigröße komprimiert. Dies geschieht für eine optimale Bereitstellung im Internet und auf Mobilgeräten.

Siehe [Hochladen und Kodieren von Videos](uploading-encoding-videos.md#uploading-and-encoding-videos).

Adobe Dynamic Media Classic bietet eine Bibliothek vordefinierter Videokodierungsvorgaben, die die am häufigsten verwendeten Kodierungseinstellungen widerspiegeln. Diese Kodierungsvorgaben wurden für die Wiedergabe auf den jeweiligen Zieldisplays optimiert. Außerdem können Administratoren eigene Videokodierungsvorgaben erstellen, um die Größe und Wiedergabe von Videos für Endbenutzer anzupassen. Alle Videokodierungsvorgaben, unabhängig davon, ob sie vorkonfiguriert von Adobe Dynamic Media Classic oder benutzerdefiniert sind, geben Videos im MP4-Dateiformat aus.

Über den Anzeigebereich „Video-Vorgaben“ können Administratoren Videokodierungen einrichten und verwalten. Sie haben folgende Möglichkeiten:

* Aktivieren und Deaktivieren von Videokodierungsvorgaben.
* Erstellen einer Videokodierungsvorgabe.
* Bearbeiten von Videokodierungsvorgaben.
* Videovorgaben löschen

Jedes Video, das Sie in Adobe Dynamic Media Classic hochladen oder in Adobe Dynamic Media Classic kodieren, wird als &quot;Video&quot;behandelt. Diese Asset-Bezeichnung bedeutet, dass Sie das Video für die Wiedergabe auf Desktops, mobilen Geräten oder beiden bereitstellen können. Beispielsweise können Sie eine Vorschau dieser Videotypen in Adobe Dynamic Media Classic anzeigen. Sie können auch URLs (mithilfe der Funktion „URL kopieren“) sowie Einbettungscode (mithilfe der Funktion „Code einbetten“) für die Verwendung mit Video-Playern, auf Websites usw. generieren.

Siehe [Anzeigen einer Videovorschau in einem Video-Viewer](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

Siehe [Verknüpfen einer Video-URL mit einer mobilen Site oder Website](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

Siehe [Einbetten des Video-Viewers auf einer Web-Seite](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

Für Video-Assets, die Sie in Adobe Dynamic Media Classic hochladen und kodieren, wird das Video im folgenden Dateiformat bereitgestellt:

**MP4 H.264** Verwenden Sie MP4-Dateien für Folgendes:

* HTTP Dynamic Streaming an Desktops.
* HLS (HTTP Live Streaming, Streaming-Protokoll von Apple).
* Progressive Videowiedergabe auf mobilen Android™-, BlackBerry®- und Windows®-Geräten.

Jedes andere Videoformat und jeder andere Codec werden als &quot;Primäres Video&quot;behandelt. Diese Asset-Bezeichnung bedeutet, dass das Video eine Quellvideodatei ist und nicht für die Wiedergabe auf Desktops oder mobilen Geräten verwendet werden kann. Beispielsweise können Sie diese Videotypen nicht in Adobe Dynamic Media Classic in der Vorschau anzeigen. Sie können keine Kopier-URLs oder Einbettungscodes generieren, die in Videoplayern, auf Websites usw. verwendet werden können.

### Filtern der Liste der Videokodierungsvorgaben {#filtering-the-list-of-video-encoding-presets}

Die Seite &quot;Videovorgaben&quot;und die Seite &quot;Adaptive Videovorgaben&quot;bestehen aus einer Tabelle, in der der aktive Status, der Vorgabenname, das vorgesehene Wiedergabegerät, die Videogröße und die Datenrate jeder Videovorgabe aufgelistet sind.

Sie können diese Liste anpassen, indem Sie den Filter „Beide“, „Aktiv“ oder „Inaktiv“ auswählen, um entweder alle Videovorgaben anzuzeigen oder die Liste auf aktive bzw. inaktive Vorgaben zu beschränken.

Sie können auch basierend auf einem Wiedergabegerät filtern, um die Liste auf Videovorgaben zu beschränken, die für alle Geräte, Desktops, Mobilgeräte oder Tablets entwickelt wurden.

**So filtern Sie die Liste der Videokodierungsvorgaben:**

1. Navigieren Sie in Adobe Dynamic Media Classic auf der globalen Navigationsleiste zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Videovorgaben]** > **[!UICONTROL Adaptive Videovorgaben]** oder **[!UICONTROL Einzelne Kodierungsvorgaben]**.

   Die Seiten für adaptive Videovorgaben und einzelne Kodierungsvorgaben enthalten eine Tabelle, in der der aktive Status, der Name der Vorgabe, das vorgesehene Wiedergabegerät, die Videodimensionen und die Datenrate jeder Videovorgabe aufgelistet werden.

1. Verwenden Sie auf der Seite „Einzelne Kodierungsvorgaben“ mit der Bezeichnung „Video-Vorgaben“ die beiden Dropdownlisten auf der Symbolleiste „Videovorgaben“, um die Tabelle basierend auf dem aktiven Status und dem Wiedergabegerät anzupassen.

   * Wählen Sie in der ersten, schmaleren Dropdownliste die Option **[!UICONTROL Beide]**, um alle Videovorgaben anzuzeigen, oder wählen Sie entweder **[!UICONTROL Aktiv]** oder **[!UICONTROL Inaktiv]**, um die Liste auf die Vorgaben zu beschränken, die entweder aktiv oder inaktiv sind.
   * Wählen in der zweiten, breiteren Dropdownliste eine Wiedergabegerät aus, um die Liste auf Videovorgaben zu beschränken, die für die Wiedergabe von Videos auf Desktops entwickelt wurden. Alternativ wählen Sie Videovorgaben aus, die für die Wiedergabe von Videos auf mobilen Geräten oder Tablets entwickelt wurden.

### Aktivieren oder Deaktivieren von Videokodierungsvorgaben {#activating-or-deactivating-video-encoding-presets}

Aktivierte Videovorgaben werden im Dialogfeld „Upload-Auftragseinstellungen“ angezeigt. Das Dialogfeld wird angezeigt, wenn ein Benutzer während des Upload-Prozesses Videodateien hochlädt. Sie können in einer Liste oder aktivierten Kodierungsvorgaben wählen.

1. Navigieren Sie in Adobe Dynamic Media Classic auf der globalen Navigationsleiste zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Videovorgaben]**.
1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Adaptive Videovorgaben]** aus.
   * Wählen Sie **[!UICONTROL Einzelne Kodierungsvorgaben]** aus.

1. Führen Sie einen der folgenden Schritte aus:

   * Um eine Videovorgabe zu aktivieren, wählen Sie auf der Seite &quot;Vorgaben&quot;unter der Spalte &quot;Aktiv&quot;das Feld neben dem Vorgabennamen aus.
   * Um eine Videovorgabe zu deaktivieren, deaktivieren Sie das Kontrollkästchen neben der Videovorgabe, die Sie inaktiv machen möchten.

     >[!NOTE]
     >
     >Inaktive Videovorgaben werden im Dialogfeld „Upload-Auftragseinstellungen“ nicht angezeigt.

1. Wählen Sie rechts unten auf der Seite **[!UICONTROL Schließen]** aus.

### Hinzufügen oder Bearbeiten einer Videokodierungsvorgabe {#adding-or-editing-a-video-encoding-preset}

Sie können Ihre eigenen benutzerdefinierten, einkodierten Videovorgaben erstellen und sie der Tabelle &quot;Videovorgaben&quot;hinzufügen. Sie können auch alle vordefinierten Videovorgaben mit Einzelkodierung ändern, die in Adobe Dynamic Media Classic enthalten sind, vorausgesetzt, Sie speichern die bearbeitete Vorgabe unter einem neuen Namen.

Adobe Dynamic Media Classic hat Höchstgrenzen für die Zieldatenrate, die Auflösungshöhe und die Auflösungsbreite festgelegt, um eine ordnungsgemäße Wiedergabe sicherzustellen. Warnmeldungen werden angezeigt, wenn Sie diese Beschränkungen überschreiten, die folgende sind:

* Für die Computerwiedergabe sind die Beschränkungen: (Breite/16) &#42; (Höhe/16) &lt; 8192.
* Für die Wiedergabe auf Mobilgeräten gelten folgende Beschränkungen: (Breite/16) &#42; (Höhe/16) &lt; 660; Zieldatenrate &lt; 4000.
* Für die Wiedergabe auf Tablets gelten folgende Beschränkungen: (Breite/16) &#42; (Höhe/16) &lt; 3600.

**So fügen Sie eine Videokodierungsvorgabe hinzu oder bearbeiten sie:**

1. Navigieren Sie in Adobe Dynamic Media Classic auf der globalen Navigationsleiste zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Videovorgaben]**.
1. Wählen Sie **[!UICONTROL Einzelne Kodierungsvorgaben]** aus.
1. Auf der Seite „Video-Vorgaben“ führen Sie einen der folgenden Schritte aus:

   * Wählen Sie in der Symbolleiste &quot;Videovorgaben&quot;die Option **[!UICONTROL Hinzufügen]** aus, damit Sie eine Videovorgabe hinzufügen können.
   * Wählen Sie eine Video-Vorgabe aus. Wählen Sie in der Symbolleiste **[!UICONTROL Bearbeiten]** aus.

     Vordefinierte Adobe Dynamic Media Classic-Vorgaben können nicht bearbeitet werden. Sie können eine Vorgabe nur aus einer vorhandenen Vorgabe erstellen, indem Sie &quot;**[!UICONTROL Speichern unter]**&quot; auswählen.

1. Legen Sie auf der Seite „Video-Vorgabe hinzufügen“ oder „Video-Vorgabe bearbeiten“ die Optionen für die Video-Vorgaben wie folgt fest.

   Die empfohlenen Einstellungen finden Sie unter [Bewährte Vorgehensweise für die Videokodierung](uploading-encoding-videos.md#best-practices-for-video-encoding).

   | Option „Video-Vorgabe“ | Beschreibung |
   | --- | --- |
   | Vorgabenname | Geben Sie einen beschreibenden Namen für die Video-Vorgabe ein. Der hier eingegebene Name wird im Dialogfeld „Upload-Auftragsoptionen“ angezeigt, in dem Benutzer Optionen zum Transkodieren auswählen. |
   | Beschreibung | Beschreiben Sie die Video-Vorgabe. Was Sie eingeben, wird als QuickInfo angezeigt. Wenn Benutzer Transkodierungsoptionen auswählen, wird die QuickInfo angezeigt, wenn sie den Mauszeiger im Dialogfeld &quot;Upload-Auftragsoptionen&quot;über den Namen der Vorgabe bewegen. |
   | Wiedergabegerät | Wählen Sie das Gerät aus, auf dem das Video wiedergegeben werden soll. Die Optionen sind Computer (Desktops), Mobil (iPhone, iPad, Android™) oder Tablet (nur iPad). Diese Einstellung bestimmt automatisch den entsprechenden Video- und Audio-Codec, der während der Kodierung verwendet wird. |
   | Zieldatenrate | Geben Sie die durchschnittliche Verbindungsgeschwindigkeit des Endbenutzers in Kilobit pro Sekunde ein. Sie können die Datenrate eingeben oder zur Eingabe den Regler ziehen. Für die Verbindungsgeschwindigkeit werden typische Geschwindigkeiten für Breitband-, DSL-, mobile und DFÜ-Verbindungen aufgelistet. Diese Einstellung legt automatisch die kombinierte Video- und Audiodatenrate fest. Anders ausgedrückt, die Datenmenge, die kodiert wird, um eine einzige Sekunde für die Videowiedergabe zu generieren. Je höher die Datenrate, desto besser ist die Qualität des resultierenden Videos. Ist die Datenrate jedoch zu hoch, kommt es zu erheblich größeren Dateien und dadurch zu einer Beeinträchtigung der Wiedergabe bei geringeren Bandbreiten. Es empfiehlt sich, einen Kompromiss zwischen hohen und niedrigen Datenraten einzugehen. Versuchen Sie, eine angemessene Wiedergabe zu erzielen, ohne Benutzer mit schmalen Bandbreiten zu verfremden. |
   | Seitenverhältnis | Das Seitenverhältnis ist das Verhältnis zwischen Breite und Höhe des Videos. Die ersten beiden Seitenverhältnisse in der Liste werden häufig verwendet, um Video horizontal anzuzeigen:<ul><li> 4:3: Wird für fast alle standardmäßigen TV-Broadcast-Inhalte mit Definition verwendet.</li><li>16:9: Wird für fast alle Breitbildinhalte und Filme im High-Definition-Fernsehen (HDTV) verwendet.</li><li>Automatische Skalierung: (Standard) Eine einzelne Kodierungsvorgabe, die mit jedem Seitenverhältnis verwendet werden kann, um Videos für die Bereitstellung auf Mobilgeräten, Tablets und Desktops zu erstellen. Hochgeladene Quellvideos, die mit dieser Vorgabe kodiert wurden, weisen eine feste Höhe auf. Die Breite wird jedoch automatisch skaliert, um das Seitenverhältnis des Videos beizubehalten (Verhältnis von Breite zu Höhe).</li><li>Benutzerspezifisch: Wird verwendet, wenn Sie eine nicht standardmäßige Videogröße definieren möchten.</li><li>Das ausgewählte Seitenverhältnis bestimmt die Breite und Höhe für die Auflösungsgröße. Die Breite und der Höhenwert werden automatisch auf das richtige Seitenverhältnis skaliert.</li></ul> |
   | Auflösung | Die Größe der Auflösung, ausgedrückt durch die Anzahl der Pixel breit durch die Anzahl der Pixel hoch, bestimmt die Größe. Geben Sie eine Breite und eine Höhe in Pixel ein oder ziehen Sie den Schieberegler, um diese Werte einzugeben. Für die Auflösung werden typische Werte aufgelistet. Der Breitenwert und der Höhenwert entsprechen automatisch dem von Ihnen ausgewählten Seitenverhältnis. Wenn Sie beispielsweise als Seitenverhältnis &quot;4:3&quot;und als Breite &quot;400&quot;eingeben, wird für die Höhe automatisch &quot;300&quot;eingegeben. Wenn Sie für die Einstellung &quot;Seitenverhältnis&quot;die Option &quot;Automatische Skalierung&quot;ausgewählt haben, wird der Breitenwert für die Auflösungsgröße automatisch auf &quot;Auto&quot;gesetzt. Wählen Sie **[!UICONTROL Vorschau]** aus, damit Sie ein Browser-Fenster öffnen und dort Ihre Lösungsoptionen anzeigen können. |
   | Kodierungsdateisuffix | Geben Sie ein Suffix ein. Dieses Suffix wird dem Namen der Videodatei nach erfolgter Kodierung angehängt. Der Name darf Bindestriche und Unterstriche enthalten, jedoch keine Leerzeichen oder Sonderzeichen. |
   | Andere Einstellungen | Adobe Dynamic Media Classic ermittelt alle anderen Kodierungseinstellungen automatisch gemäß den Best Practice-Kodierungsrichtlinien. |

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Speichern]** aus, wenn Sie eine Videovorgabe hinzugefügt oder bearbeitet haben.
   * Wählen Sie &quot;**[!UICONTROL Speichern unter]**&quot;, wenn Sie eine Videovorgabe hinzugefügt haben, indem Sie mit einer vorhandenen Vorgabe beginnen.

### Löschen einer Videokodierungsvorgabe {#delete-a-video-encoding-preset}

Administratoren können benutzerdefinierte Video-Vorgaben löschen. Videovorgaben aus Adobe Dynamic Media Classic können nicht gelöscht werden.

1. Navigieren Sie in Adobe Dynamic Media Classic auf der globalen Navigationsleiste zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Videovorgaben]**.
1. Wählen Sie **[!UICONTROL Einzelne Kodierungsvorgaben]** aus.
1. Wählen Sie auf der Seite „Video-Vorgaben“ die Vorgabe aus, die Sie nicht mehr benötigen und entfernen möchten.
1. Wählen Sie in der Symbolleiste &quot;Videovorgaben&quot;die Option **[!UICONTROL Löschen]** aus.
1. Wählen Sie im Dialogfeld &quot;Vorgabe löschen&quot;die Option **[!UICONTROL Löschen]**.

>[!MORELIKETHIS]
>
>* [Schnellstart: Video in Adobe Dynamic Media Classic](quick-start-video.md#quick-start-video)
>* [Videos hochladen und kodieren](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [Arbeiten mit Video-Viewer-Vorgaben](previewing-videos-video-viewer.md#working-with-video-viewer-presets)
>* Schulungsvideo für [Videovorgaben](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS)
