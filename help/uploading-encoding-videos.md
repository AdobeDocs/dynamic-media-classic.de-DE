---
title: Hochladen und Kodieren von Video
seo-title: Hochladen und Kodieren von Video
description: Erfahren Sie, wie Sie Videos hochladen und kodieren.
seo-description: Erfahren Sie, wie Sie Videos hochladen und kodieren.
uuid: 9a7d6513-b10c-40b0-aebb-18a795c2b8d1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: a0941823-850c-4373-9e37-f32032de3805
feature: Dynamic Media Classic, Viewer, Video
role: Business Practitioner
exl-id: 93ad91d7-f3dd-484b-b62c-633fcb864bbf
translation-type: tm+mt
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '3882'
ht-degree: 69%

---

# Hochladen und Kodieren von Video{#uploading-and-encoding-videos}

Um einzelne Video- oder adaptive Videosets für den Versand auf das Web oder Mobilgeräte zu erstellen, laden Sie zunächst Ihre Übergeordnet-Videodateien nach Dynamic Media Classic hoch. Dynamic Media Classic kodiert Videos in das MP4-Format und veröffentlicht Videos in den folgenden Dateiformaten:

* **MP4**  - Dynamic Media Classic empfiehlt MP4 als bevorzugtes Videodateiformat. Verwenden Sie MP4-Dateien für Folgendes:

   * HTTP Dynamic Streaming an Desktops.
   * HTTP Live Streaming (Apple Streaming-Protokoll).
   * Progressiver Video-Versand zu Android™-, BlackBerry®- und Windows®-Mobilgeräten

   Dynamic Media Classic-Angebote mit zwei Workflows zum Hochladen von Videodateien:

* **Vorkodierte Videos** : Sie laden MP4-Dateien direkt in Dynamic Media Classic hoch. Bei diesem Arbeitsablauf werden Dateien zum Zeitpunkt des Hochladens nicht kodiert. Die Dateien werden vorkodiert und so für die Ausgabe auf dem Desktop und mobilen Geräten vorbereitet.

* **Übergeordnet-Quellvideos**  - Laden Sie Übergeordnet-Quellvideodateien hoch und kodieren Sie sie beim Hochladen in MP4-Dateien. Kodierte Videos haben im Bedienfeld „Durchsuchen“ die Bezeichnung „Video“. Dynamic Media Classic unterstützt die Kodierung von Videodateien in vielen Formaten.

   * Stellen Sie sicher, dass die Übergeordnet zu kodierenden Quellvideodateien unterstützt werden.

      Siehe [Unterstützte Videodateitypen für die Kodierung](uploading-encoding-videos.md#supported-video-file-types-for-encoding).

   * Wählen Sie eine Videokodierungsvorgabe aus.

      Siehe [Video-Vorgaben zum Kodieren von Videodateien](application-setup.md#video-presets-for-encoding-video-files).

      Siehe [Bewährte Vorgehensweisen für die Videokodierung](uploading-encoding-videos.md#best-practices-for-video-encoding).

Dynamic Media Classic generiert auch Videominiaturen. Erfahren Sie mehr über Videominiaturen, das Abrufen ihrer URLs und das Bearbeiten von Standbildern.

Siehe [Arbeiten mit Videominiaturen](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**So laden Sie Videos hoch und kodieren sie:**

Führen Sie einen der folgenden Schritte aus.

*Ihre Videos wurden bereits kodiert*

1. Klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Hochladen]**.
1. Klicken Sie auf der Seite &quot;Hochladen&quot;auf die Registerkarte **[!UICONTROL Vom Desktop]**.
1. Klicken Sie auf der Seite &quot;Hochladen&quot;im Bedienfeld **[!UICONTROL Hochzuladende Dateien auswählen]** auf **[!UICONTROL Durchsuchen]**, navigieren Sie zu einer MP4-Videodatei und klicken Sie dann auf **[!UICONTROL Öffnen]**.
1. Wählen Sie im Bedienfeld **[!UICONTROL Ordnerziel auswählen]** einen Ordner für die hochgeladene Datei aus.
1. Stellen Sie auf der Seite &quot;Hochladen&quot;sicher, dass **[!UICONTROL Nach dem Hochladen veröffentlichen]** markiert ist.
1. Klicken Sie auf **[!UICONTROL Upload starten]**.

*Wenn Sie Ihre Videos mit Dynamic Media Classic kodieren möchten*

1. Klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Hochladen]**.
1. Klicken Sie auf der Seite &quot;Hochladen&quot;auf die Registerkarte **[!UICONTROL Vom Desktop]**.
1. Klicken Sie im Bedienfeld **[!UICONTROL Hochzuladende Dateien auswählen]** auf **[!UICONTROL Durchsuchen]**, navigieren Sie zu einer Übergeordnet Quellvideodatei und klicken Sie dann auf **[!UICONTROL Öffnen]**.
1. Wählen Sie im Bedienfeld **[!UICONTROL Ordnerziel auswählen]** einen Ordner für die hochgeladene Datei aus.
1. Klicken Sie in der unteren rechten Ecke der Seite auf **[!UICONTROL Auftragsoptionen]**,
1. Erweitern Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL eVideo-Optionen]** und führen Sie dann einen der folgenden Schritte aus:

   * Es empfiehlt sich, **[!UICONTROL Adaptive Videokodierung]** auszuwählen. Siehe [Adaptive Video (Standard)](application-setup.md#adaptive-video-default).
   * Optional. Wenn Sie einzelne Kodierungseinstellungen verwenden möchten, erweitern Sie **[!UICONTROL Einzelne Kodierungsvorgaben]** und wählen Sie dann die gewünschten Kodierungsoptionen für Desktop, Mobil und Tablet aus.
Siehe [ Vorgaben für die Videokodierung für Desktop-PCs](application-setup.md#desktop-video-encoding-presets), [Vorgaben für die Videokodierung für Mobilgeräte](application-setup.md#mobile-video-encoding-presets), [Vorgaben für die Videokodierung für Tablets](application-setup.md#tablet-video-encoding-presets).
1. Klicken Sie im Dialogfeld „Upload-Auftragsoptionen“ auf **[!UICONTROL Speichern]**.
1. Stellen Sie auf der Seite &quot;Hochladen&quot;sicher, dass **[!UICONTROL Nach dem Hochladen veröffentlichen]** markiert ist.
1. Klicken Sie unten rechts auf der Seite „Hochladen“ auf **[!UICONTROL Upload starten]**.

*Wenn Sie eine bereits hochgeladene Videodatei neu kodieren möchten*

1. Navigieren Sie in Dynamic Media Classic im Durchsuchenbedienfeld zum Video und wählen Sie es aus.
1. Klicken Sie auf **[!UICONTROL Datei]** > **[!UICONTROL Neu verarbeiten]**.
1. Erweitern Sie im Dialogfeld &quot;Assets neu verarbeiten&quot;die Option **[!UICONTROL eVideo-Optionen]** und führen Sie dann einen der folgenden Schritte aus:
   * Wie empfehlen, die folgende Methode zu verwenden. Wählen Sie **Adaptive Video**.
Siehe [Adaptive Video (Standard)](application-setup.md#adaptive-video-default).
   * Optional. Wenn Sie einzelne Kodierungseinstellungen verwenden möchten, erweitern Sie ****[!UICONTROL Einzelne Kodierungsvorgaben]**** und wählen Sie dann die gewünschten Kodierungsoptionen für Desktop, Mobil und Tablet aus.
Siehe [ Vorgaben für die Videokodierung für Desktop-PCs](application-setup.md#desktop-video-encoding-presets), [Vorgaben für die Videokodierung für Mobilgeräte](application-setup.md#mobile-video-encoding-presets), [Vorgaben für die Videokodierung für Tablets](application-setup.md#tablet-video-encoding-presets).
1. Klicken Sie im Dialogfeld „Assets neu verarbeiten“ auf **[!UICONTROL Absenden]**.

Wenn Sie eine Kodierungsvorgabe für adaptives Video oder mehrere einzelne Kodierungsvorgaben verwenden, ist das Ergebnis ein adaptives Videoset, das automatisch mit mehreren Videokodierungen erzeugt wurde. Sie können auch manuell ein adaptives Videoset erstellen, indem Sie die einzelnen Videos auswählen.

Wenn Sie ein adaptives Videoset entweder automatisch oder manuell erstellen, werden nur MP4- und M4V-Dateien erzeugt.

## Unterstützte Videodateitypen für die Kodierung {#supported-video-file-types-for-encoding}

In der folgenden Tabelle sind die Videodateitypen (mit zulässigen Video-Codecs) aufgelistet, die Sie beim Hochladen in das Format MP4 oder OGV kodieren lassen können. Die Tabelle enthält Dateiformate und Codecs:

* **Videodateiformate**  - Ähnlich wie bei einer ZIP-Datei bestimmt das Videodateiformat, wie Dateien in der Videodatei enthalten sind. Eine Videodatei besteht in der Regel aus mehreren Spuren – einer Videospur (ohne Audio) und einer oder mehreren Audiospuren (ohne Video) –, die miteinander verknüpft und synchronisiert sind. Das Videodateiformat legt fest, wie diese unterschiedlichen Datenspuren in der Videodatei organisiert sind.

* **Video-Codecs**  - Ein Video-Codec beschreibt den Algorithmus, mit dem ein Video kodiert wird. Ein Video-Player dekodiert das Video entsprechend dem Codec und zeigt dann eine Reihe von Bildern, auch Frames oder Bildfelder genannt, auf dem Bildschirm an. Codecs reduzieren die Datenmenge, die in Videodateien gespeichert werden muss, um das Video wiedergeben zu können. Statt Daten zu jedem einzelnen Bildfeld zu speichern, werden nur die Unterschiede zwischen zwei Bildfeldern gespeichert. Da die meisten Videos kaum von einem Frame zum nächsten wechseln, lassen Codecs hohe Komprimierungsraten zu, was zu kleineren Dateigrößen führt.

   | Videodateiformat | Video-Codecs |
   |:--- |:--- |
   | 3GP | H.263, H.264 |
   | AVI | DivX, DV |
   | M2P | MPEG-2 PS |
   | M2T | MPEG-2 TS |
   | M2TS | MPEG-2 TS |
   | M2V | MPEG-2 ES |
   | M4V | H.264 |
   | MOV | DV, DVCPro 50, H.261, H.263, H.264, Sorenson Video 1 |
   | MP4 | H.264/MPEG-4 AVC |
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

## Optimale Vorgehensweisen für die Videokodierung  {#best-practices-for-video-encoding}

Im Folgenden finden Sie Tipps zu bewährten Verfahren zum Kodieren von Quellvideodateien in Dynamic Media Classic.

<!-- THE FOLLOWINGS LINKS APPEAR TO BE DEAD AND THE CONTENT COMPLETELY LOST. THE GO URL DOESN'T EVEN WORK ANYMORE.
For advice about video encoding, see the following:

* Article: [Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution][www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en). THIS MATERIAL WAS FOUND ON A THIRD PARTY WEBSITE HERE: https://streaminglearningcenter.com/articles/streaming-101-the-basics-codecs-bandwidth-data-rate-and-resolution.html MATERIAL IS GOOD BUT DO NOT LINK TO IT
* Video: [Video Encoding Basics][www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en). -->

### Quell-Videodateien {#source-video-files}

Beim Kodieren einer Videodatei sollten Sie eine Quell-Videodatei mit der höchstmöglichen Qualität verwenden. Vermeiden Sie es, Dateien zu nutzen, die bereits zuvor kodiert wurden, da diese schon komprimiert sind. Eine weitere Kodierung würde zu einem Video von minderwertiger Qualität führen.

In der folgenden Tabelle werden die empfohlene Größe, das Seitenverhältnis und die minimale Bitrate beschrieben, die Ihre Quellvideodateien beim Kodieren aufweisen müssen:

| Größe | Seitenverhältnis | Minimale Bitrate |
|--- |--- |--- |
| 1024 X 768 | 4:3 | 4500 Kbit/s sind für die meisten Videos ausreichend. |
| 1280 X 720 | 16:9 | 3000–6000 Kbit/s, je nach Ausmaß der Bewegungen im Video. |
| 1920 X 1080 | 16:9 | 6000–8000 Kbit/s, je nach Ausmaß der Bewegungen im Video. |

### Abrufen der Metadaten der Datei  {#obtaining-a-file-s-metadata}

Sie können die Metadaten einer Datei abrufen, indem Sie die Metadaten in Dynamic Media Classic anzeigen, ein Video-Bearbeitungswerkzeug verwenden oder eine Anwendung zum Abrufen von Metadaten verwenden. Im Folgenden finden Sie Anweisungen zur Verwendung von MediaInfo, einer Drittanbieter-Anwendung zum Abrufen der Metadaten einer Videodatei.

1. Gehen Sie zu dieser Webseite: [https://mediainfo.sourceforge.net/en/Download](https://mediainfo.sourceforge.net/en/Download).
1. Wählen Sie das Installationsprogramm für die GUI-Version aus und laden Sie es herunter. Befolgen Sie anschließend die Installationsanweisungen.
1. Klicken Sie nach der Installation entweder mit der rechten Maustaste auf die Videodatei (nur Windows®) und wählen Sie MediaInfo oder öffnen Sie MediaInfo und ziehen Sie die Videodatei in die Anwendung. Es werden alle mit der Videodatei verknüpften Metadaten angezeigt, einschließlich Breite, Höhe und FPS.

### Seitenverhältnis  {#aspect-ratio}

Beim Auswählen bzw. beim Erstellen einer Videokodierungsvorgabe für Ihre Mastervideodatei müssen Sie sicherstellen, dass die Vorgabe das gleiche Seitenverhältnis wie die Mastervideodatei aufweist. Das *Seitenverhältnis* ist das Verhältnis von Breite und Höhe des Videos.

Um das Seitenverhältnis einer Videodatei zu ermitteln, rufen Sie die Metadaten der Datei ab und notieren Sie die Breite und Höhe der Datei (siehe [Abrufen der Metadaten einer Datei](uploading-encoding-videos.md#obtaining_a_file_s_metadata)). Berechnen Sie das Seitenverhältnis anhand der folgenden Formel:

Breite/Höhe = Seitenverhältnis

In der folgenden Tabelle sind die Formelergebnisse und die zugehörigen gebräuchlichen Seitenverhältnisse angegeben:

| Formelergebnis | Seitenverhältnis |
|--- |--- |
| 1,33 | 4:3 |
| 0,75 | 3:4 |
| 1,78 | 16:9 |
| 0,56 | 9:16 |

Beispiel: Ein Video mit einer Breite von 1440 x 1080 hat ein Seitenverhältnis von 1440/1080 oder 1,33. In diesem Fall wählen Sie eine Videokodierungsvorgabe mit einem Seitenverhältnis von 4:3, um die Videodatei zu kodieren.

### Datenrate {#data-rate}

Die *Datenrate* (auch als *Bitrate* bezeichnet) ist die Menge an Daten, die kodiert werden, um eine Videowiedergabe mit einer Dauer von einer Sekunde zu erzeugen. Die Datenrate wird in Kilobit pro Sekunde (Kbit/s) gemessen.

>[!NOTE]
>
>Da alle Codecs eine verlustreiche Komprimierung verwenden, ist die Datenrate der wichtigste Faktor für die Videoqualität. Bei einer verlustreichen Komprimierung gilt, dass die Qualität umso stärker beeinträchtigt wird, je mehr Sie eine Videodatei komprimieren. Aus diesem Grund ist die Qualität der komprimierten Datei umso niedriger, je niedriger die Datenrate ist (vorausgesetzt, dass alle anderen Merkmale wie Auflösung, Bildfrequenz und Codec gleich sind).

Berücksichtigen Sie bei der Auswahl einer Videokodierungsvorgabe die Verbindungsgeschwindigkeit des Endbenutzers in der Zielgruppe. Wählen Sie eine Vorgabe mit einer Datenrate von 80 % dieser Geschwindigkeit. Wenn die Verbindungsgeschwindigkeit des Endbenutzers beispielsweise 1000 Kbit/s beträgt, dann ist die beste Vorgabe eine mit einer Videodatenrate von 800 Kbit/s.

In dieser Tabelle sind die Datenraten typischer Verbindungsgeschwindigkeiten aufgeführt.

| Geschwindigkeit (Kbit/s) | Verbindungstyp |
|--- |--- |
| 256 | Einwählverbindung. |
| 800 | Typische Mobilverbindung. Für diese Verbindung sollten Sie für eine wahre 3G-Erfahrung eine Datenrate zwischen 400 und maximal 800 Kbit/s veranschlagen. |
| 2000 | Typische Breitband-Desktop-Verbindung. Hierzu wird eine Datenrate im Bereich von 800-2000 Kbit/s Zielgruppe, wobei die meisten Zielgruppen im Durchschnitt 1200-1500 Kbit/s betragen. |
| 5000 | Typische Hochgeschwindigkeits-Breitbandverbindung. Eine Kodierung in diesem oberen Bereich wird nicht empfohlen, da eine Videoübertragung in dieser Geschwindigkeit für die meisten Kunden nicht verfügbar ist. |

### Auflösung  {#resolution}

Als *Auflösung* wird die Höhe und Breite einer Videodatei in Pixel bezeichnet. Die meisten Quell-Videodateien werden mit einer hohen Auflösung (z. B. 1920 x 1080) gespeichert. Für Streaming-Zwecke wird die Quell-Videodatei auf eine kleinere Auflösung komprimiert (640 x 480 oder kleiner).

Auflösung und Datenrate sind zwei eng miteinander verknüpfte Faktoren, die die Videoqualität bestimmen. Um stets die gleiche Videoqualität aufrechtzuerhalten, muss bei einer Erhöhung der Pixelanzahl in einer Videodatei (d. h. bei einer höheren Auflösung) auch eine entsprechend höhere Datenrate verwendet werden. Nehmen Sie beispielsweise die Anzahl der Pixel pro Bild in einer Videodatei mit einer Auflösung von 320 x 240 und einer anderen mit einer Auflösung von 640 x 480:

| Auflösung | Pixel pro Bild |
|--- |--- |
| 320 x 240 | 76.800 |
| 640 x 480 | 307.200 |

Die Datei mit der Auflösung 640 x 480 hat viermal mehr Pixel pro Bild. Um für diese beiden Beispielauflösungen die gleiche Datenrate zu erzielen, wenden Sie auf die Datei mit einer Auflösung von 640 x 480 die vierfache Komprimierung an, was jedoch die Qualität des Videos beeinträchtigt. Daher ergibt eine Video-Datenrate von 250 Kbit/s eine hochwertige Anzeige bei einer Auflösung von 320 x 240, jedoch nicht bei einer Auflösung von 640 x 480.

>[!NOTE]
>
>Im Allgemeinen gilt: Je höher die verwendete Datenrate, desto besser wird Ihr Video angezeigt und je höher die Auflösung, desto höher muss die Anzeigequalität sein (im Vergleich zu niedrigeren Auflösungen).

Da Auflösung und Datenrate eng miteinander verbunden sind, haben Sie beim Kodieren von Video zwei Optionen:

* Wählen Sie eine Datenrate und kodieren Sie dann mit der höchsten Auflösung, die bei der von Ihnen gewählten Datenrate am besten angezeigt wird.
* Wählen Sie eine Auflösung und kodieren Sie dann mit der Datenrate, die zum Erzielen von hochwertigem Video mit der gewählten Auflösung erforderlich ist.

Bei der Auswahl (bzw. beim Erstellen) einer Videokodierungsvorgabe für Ihre Master-Videodatei, ermitteln Sie anhand der folgenden Tabelle die korrekte Auflösung:

| Auflösung | Höhe (Pixel) | Bildschirmgröße |
|--- |--- |--- |
| 240p | 240 | Winziger Bildschirm |
| 300p | 300 | Kleiner Bildschirm wie bei Mobilgeräten |
| 360p | 360 | Kleiner Bildschirm |
| 480p | 480 | Mittelgroßer Bildschirm |
| 720p | 720 | Großer Bildschirm |
| 1080p | 1080 | Großer HD-Bildschirm |

### Fps (Einzelbilder pro Sekunde)  {#fps-frames-per-second}

In den USA und Japan werden die meisten Videos mit 29,97 Bildern pro Sekunde (fps) aufgenommen und in Europa mit 25 fps. Film wird mit 24 fps aufgenommen.

Wählen Sie eine Videokodierungsvorgabe, die der fps-Rate Ihrer Master-Videodatei entspricht. Wenn Ihr Mastervideo beispielsweise mit 25 fps aufgenommen wurde, wählen Sie eine Kodierungsvorgabe mit 25 fps. Standardmäßig verwenden alle benutzerdefinierten Kodierungen die fps-Rate der Master-Videodatei. Aus diesem Grund müssen Sie die fps-Rate beim Erstellen einer Videokodierungsvorgabe nicht eigens angeben.

### Maße für die Videokodierung  {#video-encoding-dimensions}

Um optimale Ergebnisse zu erzielen, wählen Sie Kodierungsmaße, bei denen die Größe des Quellvideos ein ganzes Vielfaches aller Ihrer kodierten Videos aufweist.

Um dies zu berechnen, dividieren Sie die ursprüngliche Breite durch die kodierte Breite; dies ergibt das Breitenverhältnis. Dividieren Sie anschließend die ursprüngliche Höhe durch die kodierte Höhe; dies ergibt das Höhenverhältnis.

Wenn das resultierende Verhältnis eine Ganzzahl ist, bedeutet dies, dass das Video optimal skaliert ist. Wenn das resultierende Verhältnis keine Ganzzahl ist, beeinträchtigt dies die Videoqualität, weil verbleibende Pixelartefakte auf dem Bildschirm sichtbar sind. Dies wird insbesondere dann deutlich, wenn das Video Text enthält.

Ein Beispiel: Angenommen das Quellvideo hat die Maße 1920 x 1080. In der folgenden Tabelle werden die optimalen Kodierungseinstellungen für drei kodierte Videos aufgeführt.

| Videotyp | Breite x Höhe | Breitenverhältnis | Höhenverhältnis |
|--- |--- |--- |--- |
| Quelle | 1920 x 1080 | 1 | 1 |
| Kodiert | 960 x 540 | 2 | 2 |
| Kodiert | 640 x 360 | 3 | 3 |
| Kodiert | 480 x 270 | 4 | 4 |

### Kodiertes Videodateiformat  {#encoded-video-file-format}

Adobe Dynamic Media Classic empfiehlt die Verwendung von MP4 H.264-Videokodierungsvorgaben. Da MP4-Dateien den H.264-Videocodec verwenden, wird hochwertiges Videomaterial in einer komprimierten Datei geliefert.

## Arbeiten mit Videokodierungsvorgaben  {#working-with-video-encoding-presets}

Mastervideodateien, die mit professioneller Produktionsausrüstung und Videoschnittsoftware erstellt wurden, sind häufig zu groß und liegen in einem für Online-Medien ungeeigneten Format vor. Um digitales Videomaterial in geeignete Formate für verschiedene Ausgabemedien zu konvertieren, können Sie die Videodateien *transkodieren* (ein Vorgang, der auch als *Kodieren* bezeichnet wird). Durch das Kodieren wird das Video komprimiert und in Größe und Format für die Ausgabe auf Websites und mobilen Geräten optimiert.

Siehe [Hochladen und Kodieren von Video](uploading-encoding-videos.md#uploading-and-encoding-videos).

Dynamic Media Classic bietet eine Bibliothek vordefinierter Videokodierungsvorgaben, die die am häufigsten verwendeten Kodierungseinstellungen widerspiegeln. Diese Kodierungsvorgaben wurden für die Wiedergabe auf den jeweiligen Zieldisplays optimiert. Außerdem können Administratoren eigene Videokodierungsvorgaben erstellen, um die Größe und Wiedergabe von Videos für Endbenutzer anzupassen. Alle Videokodierungsvorgaben, ob standardmäßig von Dynamic Media Classic oder benutzerdefiniert, geben Videos im MP4-Dateiformat aus.

Über den Anzeigebereich „Video-Vorgaben“ können Administratoren Videokodierungen einrichten und verwalten. Sie haben folgende Möglichkeiten:

* Aktivieren und Deaktivieren von Videokodierungsvorgaben.
* Erstellen einer Videokodierungsvorgabe.
* Bearbeiten von Videokodierungsvorgaben.
* Löschen von Videokodierungsvorgaben.

Jedes Video, das Sie in Dynamic Media Classic hochladen oder das Sie in Dynamic Media Classic kodieren, wird als &quot;Video&quot;behandelt. Diese Asset-Bezeichnung bedeutet, dass Sie das Video für die Wiedergabe auf Desktops, mobilen Geräten oder beiden bereitstellen können. Sie können diese Videotypen beispielsweise in Dynamic Media Classic Vorschau haben. Sie können auch URLs (mithilfe der Funktion „URL kopieren“) sowie Einbettungscode (mithilfe der Funktion „Code einbetten“) für die Verwendung mit Video-Playern, auf Websites usw. generieren.

Siehe [Anzeigen einer Vorschau von Videos in einem Video-Viewer](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

Siehe [Verknüpfen einer Video-URL mit einer mobilen Site oder Website](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

Siehe [Einbetten des Video-Viewers auf einer Webseite](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

Für Video-Assets, die Sie in Dynamic Media Classic hochladen und kodieren, wird das Video im folgenden Dateiformat bereitgestellt:

**MP4 H.264** Verwenden Sie MP4-Dateien für Folgendes:

* HTTP Dynamic Streaming an Desktops.
* HLS (HTTP Live Streaming, Apple-Streaming-Protokoll).
* Progressiver Versand auf Android™-, BlackBerry®- und Windows®-Mobilgeräte.

Alle anderen Videoformate und Codecs werden als &quot;Übergeordnet Video&quot;behandelt. Diese Asset-Bezeichnung bedeutet, dass das Video eine Quellvideodatei ist und nicht für die Wiedergabe auf Desktops oder mobilen Geräten verwendet werden kann. Sie können diese Videotypen beispielsweise nicht in Dynamic Media Classic Vorschau haben. Sie können auch keine Verknüpfungen des Typs „URL kopieren“ sowie Einbettungscode für die Verwendung in Video-Playern, auf Websites usw. generieren.

### Filtern der Liste von Videokodierungsvorgaben  {#filtering-the-list-of-video-encoding-presets}

Die Seite &quot;Video-Vorgaben&quot;und die Seite &quot;Adaptive Video-Vorgaben&quot;bestehen aus einer Tabelle, in der der aktive Status, der Vorgabenname, das vorgesehene Wiedergabegerät, die Videogröße und die Datenrate jeder Videovorgabe Liste werden.

Sie können diese Liste anpassen, indem Sie den Filter „Beide“, „Aktiv“ oder „Inaktiv“ auswählen, um entweder alle Videovorgaben anzuzeigen oder die Liste auf aktive bzw. inaktive Vorgaben zu beschränken.

Sie können auch basierend auf einem Wiedergabegerät filtern, um die Liste auf Videovorgaben zu beschränken, die für alle Geräte, Desktops, Mobilgeräte oder Tablets entwickelt wurden.

**So filtern Sie die Liste der Videokodierungsvorgaben:**

1. Klicken Sie in Dynamic Media Classic in der Symbolleiste für globale Navigation auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Video-Vorgaben]** > **[!UICONTROL Adaptive Video-Vorgaben]** oder **[!UICONTROL Einzelne Kodierungsvorgaben]**.

   Die Seiten für adaptive Video-Vorgaben und Einzelne Kodierungsvorgaben enthalten eine Tabelle, in der der Aktiv-Status, der Name der Vorgabe, das vorgesehene Wiedergabegerät, die Videoabmessungen und die Datenrate jeder Videovorgabe Liste werden.

1. Verwenden Sie auf der Seite „Einzelne Kodierungsvorgaben“ mit der Bezeichnung „Video-Vorgaben“ die beiden Dropdownlisten auf der Symbolleiste „Videovorgaben“, um die Tabelle basierend auf dem aktiven Status und dem Wiedergabegerät anzupassen.

   * Wählen Sie in der ersten, schmaleren Dropdownliste die Option **[!UICONTROL Beide]**, um alle Videovorgaben anzuzeigen, oder wählen Sie entweder **[!UICONTROL Aktiv]** oder **[!UICONTROL Inaktiv]**, um die Liste auf die Vorgaben zu beschränken, die entweder aktiv oder inaktiv sind.
   * Wählen in der zweiten, breiteren Dropdownliste eine Wiedergabegerät aus, um die Liste auf Videovorgaben zu beschränken, die für die Wiedergabe von Videos auf Desktops entwickelt wurden. Alternativ wählen Sie Videovorgaben aus, die für die Wiedergabe von Videos auf mobilen Geräten oder Tablets entwickelt wurden.

### Aktivieren oder Deaktivieren von Videokodierungsvorgaben  {#activating-or-deactivating-video-encoding-presets}

Aktivierte Videovorgaben werden im Dialogfeld „Upload-Auftragseinstellungen“ angezeigt. Das Dialogfeld wird angezeigt, wenn ein Benutzer während des Uploads Videodateien hochlädt. Sie können in einer Liste oder aktivierten Kodierungsvorgaben wählen.

1. Klicken Sie in Dynamic Media Classic in der Symbolleiste für globale Navigation auf **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Video-Vorgaben]**.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **[!UICONTROL Adaptive Videovorgaben]**.
   * Klicken Sie auf **[!UICONTROL Einzelne Kodierungsvorgaben]**.

1. Führen Sie einen der folgenden Schritte aus:

   * Zum Aktivieren einer Videovorgabe aktivieren Sie auf der Seite der Vorgaben unter der Spalte „Aktiv“ das Kontrollkästchen neben einem Vorgabenamen.
   * Zum Deaktivieren einer Videovorgabe deaktivieren Sie das Kontrollkästchen dem Videovorgabenamen, den Sie deaktivieren möchten.

      >[!NOTE]
      >
      >Inaktive Videovorgaben werden im Dialogfeld „Upload-Auftragseinstellungen“ nicht angezeigt.

1. Klicken Sie in der rechten unteren Ecke der Seite auf **[!UICONTROL Schließen]**.

### Hinzufügen oder Bearbeiten einer Videokodierungsvorgabe  {#adding-or-editing-a-video-encoding-preset}

Sie können Ihre eigenen, benutzerdefinierten einzelnen Kodierungsvorlagen erstellen und sie zur Tabelle der Videovorgaben hinzufügen. Sie können auch vordefinierte Video-Vorgaben für die einzelne Kodierung ändern, die im Lieferumfang von Dynamic Media Classic enthalten sind, vorausgesetzt, Sie speichern die bearbeitete Vorgabe unter einem neuen Namen.

Dynamic Media Classic hat Höchstgrenzen für die Datenrate, die Höhe der Auflösung und die Breite der Zielgruppe festgelegt, um eine ordnungsgemäße Wiedergabe zu gewährleisten. Es werden Warnmeldungen angezeigt, wenn Sie diese Beschränkungen überschreiten:

* Für die Wiedergabe auf dem Computer gilt für die Obergrenzen: (Breite/16) * (Höhe/16) &lt; 8192.
* Für die Wiedergabe auf mobilen Geräten gilt für die Obergrenzen: (Breite/16) * (Höhe/16) &lt; 660; Zieldatenrate &lt; 4000.
* Für die Wiedergabe auf Tablet-Geräten gilt für die Obergrenzen: (Breite/16) * (Höhe/16) &lt; 3600.

**So fügen Sie eine Videokodierungsvorgabe hinzu oder bearbeiten sie:**

1. Klicken Sie in Dynamic Media Classic in der Symbolleiste für globale Navigation auf **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Video-Vorgaben]**.
1. Klicken Sie auf **[!UICONTROL Einzelne Kodierungsvorgaben]**.
1. Auf der Seite „Video-Vorgaben“ führen Sie einen der folgenden Schritte aus:

   * Klicken Sie in der Symbolleiste &quot;Video-Vorgaben&quot;auf **[!UICONTROL Hinzufügen]**, um eine Video-Vorgabe hinzuzufügen.
   * Wählen Sie eine Video-Vorgabe aus. Klicken Sie auf der Symbolleiste auf **[!UICONTROL Bearbeiten]**.

      Vordefinierte Vorgaben von Dynamic Media Classic können nicht bearbeitet werden. Sie können eine Vorgabe nur aus einer vorhandenen erstellen, indem Sie **[!UICONTROL Speichern unter]** wählen.

1. Legen Sie auf der Seite „Video-Vorgabe hinzufügen“ oder „Video-Vorgabe bearbeiten“ die Optionen für die Video-Vorgaben wie folgt fest.

   Die empfohlenen Einstellungen finden Sie unter [Bewährte Vorgehensweise für die Videokodierung](uploading-encoding-videos.md#best-practices-for-video-encoding).

   | Option „Video-Vorgabe“ | Beschreibung |
   |--- |--- |
   | Vorgabenname | Geben Sie einen beschreibenden Namen für die Video-Vorgabe ein. Der hier eingegebene Name wird im Dialogfeld „Upload-Auftragsoptionen“ angezeigt, in dem Benutzer Optionen zum Transkodieren auswählen. |
   | Beschreibung | Beschreiben Sie die Video-Vorgabe. Der hier eingegebene Text wird als QuickInfo angezeigt, wenn Sie den Mauszeiger über den Namen der Vorgabe im Dialogfeld &quot;Upload-Auftragsoptionen&quot;bewegen, in dem Benutzer Optionen zum Transkodieren auswählen. |
   | Wiedergabegerät | Wählen Sie das Gerät aus, auf dem das Video wiedergegeben werden soll. Die Optionen sind Computer (Desktop-PCs), Mobil (iPhone, iPad, Android™). oder Tablet (nur iPad). Über diese Einstellung wird automatisch der geeignete Video- und Audio-Codec für die Kodierung festgelegt. |
   | Zieldatenrate | Geben Sie die durchschnittliche Verbindungsgeschwindigkeit des Endbenutzers in Kilobit pro Sekunde ein. Sie können die Datenrate eingeben oder zur Eingabe den Regler ziehen. Für die Verbindungsgeschwindigkeit werden typische Geschwindigkeiten für Breitband-, DSL-, mobile und DFÜ-Verbindungen aufgelistet. Diese Einstellung legt automatisch die kombinierte Video- und Audiodatenrate fest. Anders ausgedrückt, die Datenmenge, die kodiert wird, um eine einzige Sekunde für die Videowiedergabe zu generieren. Je höher die Datenrate, desto besser ist die Qualität des resultierenden Videos. Ist die Datenrate jedoch zu hoch, kommt es zu erheblich größeren Dateien und dadurch zu einer Beeinträchtigung der Wiedergabe bei geringeren Bandbreiten. Es empfiehlt sich, einen Kompromiss zwischen hohen und niedrigen Datenraten einzugehen. Die Videos sollten in möglichst hoher Qualität wiedergegeben werden, ohne jedoch Benutzer mit langsameren Verbindungen zu benachteiligen. |
   | Seitenverhältnis | Das Seitenverhältnis ist das Verhältnis von Breite und Höhe des Videos. Die ersten beiden Seitenverhältnisse in der Liste werden häufig verwendet, um Video horizontal anzuzeigen:<ul><li> 4:3: Wird für nahezu alle TV-Übertragungen in Standardauflösung verwendet.</li><li>16:9: Wird für nahezu alle HDTV-Übertragungen in Widescreen sowie für Spielfilme verwendet.</li><li>Autom. Skalierung (Standard): Eine einzelne Kodierungsvorgabe, die mit jedem Seitenverhältnis verwendet werden kann, um Videos zur Wiedergabe auf Mobilgeräten, Tablets und Desktops zu erstellen. Hochgeladene Quellvideos, die mit dieser Vorgabe kodiert wurden, weisen eine feste Höhe auf. Die Breite wird jedoch automatisch skaliert, um das Seitenverhältnis des Videos (Verhältnis von Breite zu Höhe) beizubehalten.</li><li>Benutzerdefiniert: Verwenden Sie diese Einstellung, wenn Sie ein eigenes Videoformat festlegen möchten.</li><li>Das ausgewählte Seitenverhältnis legt die Einstellungen für Breite und Höhe für die Auflösungsgröße fest. Der Breiten- bzw. Höhenwert wird automatisch an das jeweilige Seitenverhältnis angepasst.</li></ul> |
   | Auflösung | Die Auflösung, ausgedrückt durch die Anzahl der Pixel breit durch die Anzahl der Pixel hoch, bestimmt die Größe. Geben Sie einen Wert für die Breite und Höhe in Pixeln ein oder ziehen Sie zur Eingabe den Regler. Für die Auflösung werden typische Werte aufgelistet. Die Werte für Breite und Höhe werden jeweils automatisch an das ausgewählte Seitenverhältnis angepasst. Wenn Sie zum Beispiel als Seitenverhältnis „4:3“ festlegen und als Breite „400“ eingeben, wird für die Höhe automatisch „300“ eingegeben. Wenn Sie für das Seitenverhältnis die Einstellung Autom. Skalierung festgelegt haben, wird für die Breite der Auflösungsgröße automatisch der Wert Auto festgelegt. Klicken Sie auf &quot;Vorschau&quot;, um ein Browserfenster zu öffnen und die ausgewählten Auflösungseinstellungen anzuzeigen. |
   | Kodierungsdateisuffix | Geben Sie ein Suffix ein. Dieses Suffix wird dem Namen der Videodatei nach erfolgter Kodierung angehängt. Der Name darf Bindestriche und Unterstriche enthalten, jedoch keine Leerzeichen oder Sonderzeichen. |
   | Andere Einstellungen | Dynamic Media Classic legt alle anderen Kodierungseinstellungen gemäß den Richtlinien für die optimale Kodierung automatisch fest. |

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie eine Video-Vorgabe hinzugefügt oder bearbeitet haben.
   * Klicken Sie auf **[!UICONTROL Speichern unter]**, wenn Sie eine Video-Vorgabe auf Grundlage einer bereits vorhandenen Vorgabe erstellt haben.

### Löschen einer Videokodierungsvorgabe  {#deleting-a-video-encoding-preset}

Administratoren können benutzerdefinierte Video-Vorgaben löschen. Mit Dynamic Media Classic gelieferte Video-Vorgaben können nicht gelöscht werden.

1. Klicken Sie in Dynamic Media Classic in der Symbolleiste für globale Navigation auf **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Video-Vorgaben]**.
1. Klicken Sie auf **[!UICONTROL Einzelne Kodierungsvorgaben]**.
1. Wählen Sie auf der Seite „Video-Vorgaben“ die Vorgabe aus, die Sie nicht mehr benötigen und entfernen möchten.
1. Klicken Sie auf der Symbolleiste „Video-Vorgabe“ auf **[!UICONTROL Löschen]**.
1. Klicken Sie im Dialogfeld „Voreinstellung löschen“ auf **[!UICONTROL Löschen]**.

>[!MORELIKETHIS]
>
>* [Kurzanleitung: Video](quick-start-video.md#quick-start-video)
>* [Hochladen und Kodieren von Video](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [Arbeiten mit Video-Viewer-Vorgaben](previewing-videos-video-viewer.md#working-with-video-viewer-presets)

