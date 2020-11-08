---
title: Hochladen von Dateien
seo-title: Hochladen von Dateien
description: 'null'
seo-description: Erfahren Sie, wie Sie Dateien hochladen.
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '3855'
ht-degree: 43%

---


# Hochladen von Dateien{#uploading-files}

Bevor Sie Asset-Dateien in Dynamic Media Classic hochladen, vergewissern Sie sich, dass die Asset-Dateien korrekt benannt sind und dass die Ordnerstruktur wie gewünscht eingerichtet und organisiert ist. Sie können Dateien von einer mit Dynamic Media Classic bereitgestellten FTP-Site oder direkt von Ihrem Computer oder Netzwerk hochladen. Optionen für Dynamic Media Classic-Angebote zum Optimieren von Dateien beim Hochladen. Wenn Sie die Adobe Dynamic Media Classic-Desktopanwendung installiert haben, können Sie Dateien und Ordner direkt von Ihrem Desktop aus hochladen. (Siehe [Allgemeine Programmeinstellungen](application-setup.md#general_settings).)

## Vorbereiten von Assets und Ordnern zum Hochladen {#preparing-your-assets-and-folders-for-uploading}

Vergewissern Sie sich vor dem Hochladen von Assets in Dynamic Media Classic, dass sie im richtigen Format und in der richtigen Größe vorliegen. Außerdem müssen Sie die Regeln für die Benennung von Assets in Dynamic Media Classic beachten. Indem Sie eine Ordnerorganisation und -struktur konfigurieren, erleichtern Sie sich das Auffinden von Dateien und die Arbeit mit den Dateien.

### Unterstützte Asset-Dateiformate {#supported-asset-file-formats}

In dieser Tabelle werden die von Dynamic Media Classic unterstützten Asset-Dateiformate Liste. For information on supported Camera Raw files, see [www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en).

| Asset-Dateiformate | Beschreibung |
|--- |--- |
| Audio | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Cascading Stylesheet | CSS |
| Farbprofile | ICC, ICM |
| Schriftarten | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Bilder | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (nur Windows), TIF, TIFF |
| InDesign | INDD, INDT |
| MS Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG und Camera Raw |
| PostScript | EPS, PS |
| Dynamic Media Classic Image Authoring | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Video | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

Die Upload-Unterstützung von ZIP- und TAR-Archiven umfasst ein Kontrollkästchen, mit dem Sie angeben können, ob die Dateien entpackt werden sollen.

### Nicht unterstützte Bildformate in dynamischen Medien {#unsupported-image-formats-dynamic-media}

In der folgenden Liste werden die Untertypen der Rasterbilddateiformate beschrieben, die in dynamischen Medien *nicht* unterstützt werden.

Siehe auch [Erkennung nicht unterstützter Dateiformate für dynamische Medien](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* PNG-Dateien mit einer IDAT-Größe größer als 100 MB.
* PSB-Dateien.
* PSD-Dateien mit einem anderen Farbraum als CMYK, RGB, Graustufen oder Bitmap werden nicht unterstützt. DuoTone-, Lab- und indizierte Farbräume werden nicht unterstützt.
* PSD-Dateien mit einer Bittiefe größer als 16.
* TIFF-Dateien mit Gleitkommadaten.
* TIFF-Dateien mit Lab-Farbraum.

### Asset-Typen {#asset-types}

Um optimale Ergebnisse mit der Dynamic Media Classic-Plattform zu erzielen, sollten Sie die empfohlenen Dateiformate und -größen verwenden. In der folgenden Tabelle sind die empfohlenen Formate und Dateigrößen für häufig verwendete Assets aufgeführt.

| Asset-Typ | Beschreibung/Empfehlungen |
|--- |--- |
| Audio | Zu den Eingabeformaten von Audio-Assets gehören AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3. Sie können Audio-Daten in die folgenden Formate transcodieren: MP3, AAC und HE-AAC. |
| Bilder (für Bildgrößenänderungen, Zoom, Bildsätze, Rotationssets) | Bilder müssen an der längsten Seite mindestens 2000 Pixel haben. Die normalen Bildgrößen liegen zwischen 1500 und 2500 Pixel an der längsten Seite. Verlustfreie Bildformate, z. B. TIFF und PNG, sind zu empfehlen. Bei Verwendung eines JPEG-Bildes sollten Sie die höchste Qualitätseinstellung wählen. Animierte GIF-Dateien werden wie andere statische Inhalte behandelt. |
| E-Kataloge | Verwenden Sie hoch auflösende PDF-Dateien, die mit Adobe® Acrobat® oder einer Creative Suite-Anwendung erstellt und als „druckbereit“ gespeichert wurden. PDF-Dateien beinhalten alle erforderlichen Schriftarten, Bilder, Masken und Grafikelemente, auf die verwiesen wird, entweder als Einzelseiten, doppelseitige Druckbögen oder in einem mehrseitigen Format. Sortieren Sie die Seiten, indem Sie die Dateien in alphanumerischer Reihenfolge benennen. Platzieren Sie alle PDF-Dateien für einen E-Katalog in einem einzigen Ordner, um das Hochladen zu vereinfachen. Beim Hochladen können Sie Schnittoptionen auswählen, um die Zuschneidebereiche, einschließlich Schnittmarken, Passermarken oder Farbkontrollstreifen, aus den PDF-Dateien zu entfernen. Da die meisten druckbereiten PDF-Dateien im CMYK-Farbraum gespeichert werden, ist es wichtig, das für die PDF-Dateien verwendete ICC-Farbprofil für CMYK zu ermitteln und abzurufen. |
| Vorlagen | Bild- oder Layoutentwürfe mit Ebenen können Text, Bilder und Ebenen enthalten. Bildebenen, Textzeichenfolgen und Ebenenattribute wie Farbe und Größe können parametrisiert werden, sodass variable Daten angepasst werden können. Die Anforderungen für in Vorlagen verwendete Bilder sind dieselben wie für andere Bilder. Bereiten Sie Grafiken in Photoshop oder einem anderen Bildbearbeitungsprogramm vor. Speichern Sie jede Grafik einzeln als reduzierte, transparente Datei im TIFF- oder PNG-Format. Stellen Sie sicher, dass die Bildauflösung für den beabsichtigten Verwendungszweck geeignet ist. Bilder, die für Druckzwecke verwendet werden sollen, sollten eine Auflösung von 300 ppi besitzen. |
| Videos | Dynamic Media Classic unterstützt Videodateien im OGV- und MP4-Format. Sie können Dateien beim Hochladen in das Format MP4 transkodieren.Siehe [Unterstützte Asset-Dateiformate](#supported-static-file-formats). |
| Schriftarten | Hochgeladene TrueType-, Type1- (nur Windows), OpenType-Schriftarten und PhotoFonts |
| Bilder | Bilder und Bilddateien mit mehreren Ebenen. |
| Bildsätze und Mustersets | Sammlungen zusammengehöriger Bilder, die in einem Viewer angezeigt werden können. |
| ICC-Profile | Farbprofil, mit dem ein hochgeladenes Bild aus dem Ursprungsfarbraum in einen anderen Farbraum konvertiert werden kann. |
| Vignetten | Mit dem Image Authoring-Programm erstellte Bilder sowie zugehörige Dateien. |
| Inhaltsdateien | Adobe InDesign-, Illustrator- oder Photoshop-Inhaltsdateien. |
| FXG-Dateien | Auflösungsunabhängige Grafikformatdateien, mit deren Hilfe Sie anpassbare Vorlagen für die Ausgabe auf Druckern, im Web, als E-Mail, auf einem Desktop und auf anderen Geräten erstellen können. |
| SVG-Dateien | Skalierbare Vektorgrafikdateien, die vom Image-Serving-Server gerendert werden können. |
| XML-Dateien | Dateien, die Vorverarbeitungsregeln zum Verändern der Pfad- und Abfrageabschnitte von Anforderungen festlegen. |
| Cascading Stylesheet-Dateien | Laden Sie CSS-Skins zur Anpassung von HTML5-Viewern hoch. |
| JavaScript-Dateien | JavaScript-Dateien werden für die Viewer-Instrumentation verwendet, um Kontoinformationen festzuhalten. Adobe Security empfiehlt dies ausschließlich für Client-Konten, die für die Zustellung eine separate Domain haben (um das Site-übergreifende Scripting zu verhindern). |

>[!NOTE]
>
>Wenn Sie Bilddateien und PDFs in Dynamic Media Classic hochladen, konvertiert das System diese Quelldateien in P-TIFF-Dateien (Pyramid TIFF). Bei diesen P-TIFFs handelt es sich um Dateien, die später auf den Image-Servern für dynamische Medien veröffentlicht werden. Dynamic Media Classic verwendet das Pyramid Tiff-Dateiformat, da es verschiedene Zoomverhältnisse enthält, die eine schnelle Zoomfunktion bei der Anzeige mit einem Dynamic Media Classic-Zoom-Viewer ermöglichen.

### Unterstützte statische Dateiformate {#supported-static-file-formats}

Dynamic Media Classic unterstützt mehrere statische Dateiformate. Statischer Inhalt ist jedes Asset, das unverändert veröffentlicht wird, z. B. CSS, PDF, SVG, XML usw.

Die folgenden Dateitypen können veröffentlicht werden:

* Animiertes GIF
* Audiodateien
* CSS
* JavaScript (wenn das Unternehmen mit einer eigenen Domäne konfiguriert wurde)
* Mastervideo
* PDF (wenn PDF-Dateien speziell zur Veröffentlichung nach dem Upload markiert wurden, dies verhindert die Bereitstellung aller PDF-Dateien für den vorhandene eCatalog-/PDF-Arbeitsablauf)
* PrX-Video
* SVG
* XML
* ZIP

Dynamic Media Classic bietet keine Option zum Generieren einer Vorschauen-URL statischer Inhalte.

### Dateinamenanforderungen {#filename-requirements}

Da beim Hochladen die Erweiterungen aus den Dateinamen entfernt werden, sind Dateien mit demselben Stammnamen nicht zulässig. Im System Dynamic Media Classic wird der Asset-Dateiname ohne Dateinamenerweiterung zur Asset-ID. Deshalb muss jedes Asset einen eindeutigen Namen haben.

Stellen Sie deshalb sicher, dass allen Benutzern in Ihrem Unternehmen die folgenden Dateinamensregeln vertraut sind:

* Asset-IDs mit exakt demselben Namen sind im System nicht zulässig.
* Bei Asset-ID-Namen wird die Groß-/Kleinschreibung berücksichtigt.
* Asset-IDs sollten keine Leerzeichen enthalten (z. B. nicht „Schwarze Jacke.tif“ oder „Blaue Jacke.jpg“). ASCII-Kodierungen von Dynamic Media Classic in Elementnamen kodieren Leerzeichen, wenn zum Erstellen von URL-Zeichenfolgen Elementnamen verwendet werden. Diese ASCII-Codierung beeinträchtigt jedoch die Lesbarkeit der URLs.
* Sprachspezifische Zeichen sind in Dateinamen zulässig. Allerdings dürfen Dateinamen die folgenden Zeichen nicht enthalten:

   \ ; / ? : @ &amp; = + $ , * &quot; &lt; > | &#39; { } %

   Wenn ein Dateiname eines oder mehrere der oben aufgeführten Zeichen enthält, werden die Zeichen beim Hochladen aus dem Dateinamen entfernt.

In den meisten Fällen kann als Asset-Dateiname die Elementnummer, Produkt-SKU oder ein anderer Name des dargestellten Elements verwendet werden, wie im Folgenden:

| Element | Dateiname | Asset-ID |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Ordnerorganisation und -struktur {#folder-organization-and-structure}

Organisieren und strukturieren Sie Ordner und Unterordner für Ihre Inhalte in Dynamic Media Classic, bevor Sie Ihre Inhalte in das System hochladen. Eine solche Vorausplanung hat die folgenden zwei wichtigen Vorteile:

* Wenn Sie Ihre Inhalte per FTP auf Dynamic Media Classic hochladen, können Sie das System anweisen, Ihre Ordnerstruktur während des Hochladevorgangs zu replizieren. Auf diese Weise werden Ihre Inhalte in denselben Ordnern und Unterordnern in Dynamic Media Classic wie auf Ihrem Computer oder im Netzwerk organisiert. (Um Ihre Ordnerstruktur in Dynamic Media Classic zu replizieren, wählen Sie beim Hochladen von Assets per FTP die Option &quot;Unterordner einschließen&quot;.)
* Es ist sehr viel schwieriger, Ordner nach dem Hochladen der Dateien innerhalb des Systems neu zu organisieren, als vorab eine sorgfältig vorbereitete Ordnerstruktur zu erstellen.

Die Vorgehensweise und die Struktur zum Benennen von Ordnern, die Sie zum Speichern Ihrer Inhalte in Dynamisch Media Classic auswählen, hängt von den Anforderungen Ihres Unternehmens ab. Es folgen einige Beispiele für Ordnerstrukturen:

**SKU-basierte** Ordner werden nach SKUs oder Elementnummern benannt. Beispielsweise werden separate Ordner für alle mit 0, 20, 30 usw. beginnenden Nummerserien erstellt. 

**Markenbasiert** Für Hersteller mit mehreren Markenlinien und Einzelhändler, die andere Marken aus anderen Firmen vertreiben, trennen Sie die Dateien in Produktordner, die nach verschiedenen Marken benannt sind.

**Projektbasierte** Ordner werden nach Rollout-/Ablagedatum oder Projektname organisiert. Kunden, die hauptsächlich E-Kataloge erstellen, bevorzugen diese Vorgehensweise.

**Spiegeln der Ordnerhierarchie** auf der Website Diese Ordnerstruktur spiegelt die Ordnerstruktur der Website wider, wobei die Ordner beispielsweise für Produktordner benannt sind.

## Informationen zum Hochladen von Dateien {#uploading-your-files}

Sie können einzelne Dateien vom Desktop oder Ordner über FTP hochladen. If you want to upload more than 100 MB of files or upload entire folders and subfolders, select the **VIA FTP** tab.

Dynamic Media Classic sendet Ihnen eine E-Mail-Nachricht, um zu bestätigen, wann der Upload-Auftrag beginnt und endet, und Sie über Probleme zu informieren.

Während eines oder unmittelbar nach einem großen Upload-Auftrag(s) wird u. U. für einige neue Elemente die Meldung „Bild wurde noch nicht optimiert“ angezeigt. Diese Meldung wird angezeigt, weil die Dateien noch nicht vollständig verarbeitet sind und zu Dynamic Media Classic hinzugefügt werden. Sie können die betroffenen Dateien später optimieren. (Siehe [Optimieren von Dateien](application-setup.md#optimize_files).)

### Hochladen von Dateien auf der Registerkarte &quot;VON DESKTOP&quot; {#upload-files-using-sps-desktop-application}

Mit der Desktop-Anwendung Dynamic Media Classic können Sie Dateien und Ordner durch Ziehen hochladen.

1. In the Dynamic Media Classic Desktop application, on the Global Navigation bar, click **Upload**.
1. On the Upload page, click the **FROM DESKTOP** tab.
1. Klicken Sie auf der linken Seite der Seite &quot;Hochladen&quot;im Bereich &quot;Hochzuladende Dateien **auswählen** &quot;auf **Durchsuchen** , um die hochzuladenden Dateien oder Ordner auszuwählen, und klicken Sie dann auf **Öffnen**.
1. Navigieren Sie auf der rechten Seite der Seite &quot;Hochladen&quot;im Bereich &quot;Ordnerziel **auswählen** &quot;zu einem Zielordner, in dem die hochgeladenen Dateien oder Ordner hinzugefügt werden sollen.
1. (Optional) Geben Sie unten auf der Seite &quot;Hochladen&quot;im Feld &quot; **Auftragsname** &quot;den neuen Namen des Upload-Auftrags ein. Oder Sie können einfach den standardmäßigen, systemgenerierten Namen verwenden, den Dynamic Media Classic bereitstellt. Dieser Auftrag wird ebenso wie andere Upload- und Veröffentlichungsaufträge auf der Seite „Aufträge“ erfasst – hier können Sie den Status von Aufträgen prüfen.
Siehe [Überprüfen von Auftragsdateien](checking-job-files.md#checking_job_files).
1. (Optional) Wählen Sie unten auf der Seite &quot;Hochladen&quot;die Option Nach dem Hochladen **veröffentlichen** , wenn Sie die hochgeladenen Assets automatisch veröffentlichen möchten.
Wenn Sie Dateien veröffentlichen, werden die Dateien an Live-Server gesendet. Die URLs für diese Dateien können dann auf externen Websites und in externen Anwendungen verwendet werden. Beachten Sie, dass dieselbe Option auch im Dialogfeld &quot;Auftragsoptionen&quot;verfügbar ist.
1. (Optional) Wählen Sie im unteren Bereich der Seite &quot;Hochladen&quot;die Option &quot;In einem beliebigen Ordner **überschreiben&quot;aus, und zwar unabhängig von der Erweiterung** , wenn Sie möchten, dass die hochgeladenen Dateien die vorhandenen Dateien mit denselben Namen ersetzen. Beachten Sie, dass dieselbe Option auch im Dialogfeld &quot;Auftragsoptionen&quot;verfügbar ist.
The name of this option could be different, depending on the settings in **Application Setup > General Settings > Upload to Application > Overwrite Images**.
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   Siehe [Optionen für das Hochladen](uploading-files.md#upload_options).

1. Klicken Sie im Dialogfeld „Upload-Auftragsoptionen“ auf **Speichern**.
1. Klicken Sie in der rechten unteren Ecke der Seite &quot;Hochladen&quot;auf **&quot;Hochladen**senden&quot;.
Klicken Sie auf der globalen Navigationsleiste auf **Aufträge**, um den Fortschritt beim Hochladen anzuzeigen. Sie können die Arbeit in Dynamic Media Classic fortsetzen und jederzeit zur Seite &quot;Aufträge&quot;zurückkehren, um einen in Verarbeitung befindlichen Auftrag zu überprüfen. Wenn Sie einen in Verarbeitung befindlichen Upload-Auftrag stornieren möchten, klicken Sie auf die Schaltfläche **Abbrechen** neben der Angabe „Dauer“.

### Hochladen von Dateien auf der Registerkarte &quot;VIA FTP&quot; {#upload-files-using-via-ftp}

1. Melden Sie sich bei der FTP-Site Dynamic Media Classic an, die für Ihre Region spezifisch ist. Melden Sie sich mit dem von Ihrem Administrator erhaltenen FTP-Benutzernamen und -Kennwort an.
1. Klicken Sie in Dynamic Media Classic in der Symbolleiste für globale Navigation auf **Hochladen**.
1. On the Upload page, click the **VIA FTP** tab.
1. Wählen Sie auf der linken Seite der Seite &quot;Hochladen&quot;im Bereich &quot;FTP-Ordner zum Hochladen **** auswählen&quot;einen FTP-Ordner aus, aus dem die Dateien hochgeladen werden sollen.
1. Wählen Sie auf der rechten Seite der Seite &quot;Hochladen&quot;im Bereich &quot;Dynamic Media-Ordnerziel **auswählen** &quot;einen Zielordner in &quot;Dynamic Media Classic&quot;.
1. (Optional) Geben Sie unten auf der Seite &quot;Hochladen&quot;im Feld &quot; **Auftragsname** &quot;den neuen Namen des Upload-Auftrags ein. Oder Sie können einfach den standardmäßigen, systemgenerierten Namen verwenden, den Dynamic Media Classic bereitstellt. Dieser Auftrag wird ebenso wie andere Upload- und Veröffentlichungsaufträge auf der Seite „Aufträge“ erfasst – hier können Sie den Status von Aufträgen prüfen.
Siehe [Überprüfen von Auftragsdateien](checking-job-files.md#checking_job_files).
1. (Optional) Wählen Sie unten auf der Seite &quot;Hochladen&quot;die Option Nach dem Hochladen **veröffentlichen** , wenn Sie die hochgeladenen Assets automatisch veröffentlichen möchten.
Wenn Sie Dateien veröffentlichen, werden die Dateien an Live-Server gesendet. Die URLs für diese Dateien können dann auf externen Websites und in externen Anwendungen verwendet werden. Beachten Sie, dass dieselbe Option auch im Dialogfeld &quot;Auftragsoptionen&quot;verfügbar ist.
1. (Optional) Wählen Sie im unteren Bereich der Seite &quot;Hochladen&quot;die Option &quot;In einem beliebigen Ordner **überschreiben&quot;aus, und zwar unabhängig von der Erweiterung** , wenn Sie möchten, dass die hochgeladenen Dateien die vorhandenen Dateien mit denselben Namen ersetzen. Beachten Sie, dass dieselbe Option auch im Dialogfeld &quot;Auftragsoptionen&quot;verfügbar ist.
The name of this option could be different, depending on the settings in **Application Setup > General Settings > Upload to Application > Overwrite Images**.
1. (Optional) nur verfügbar, wenn Sie auf die Registerkarte **VIA FTP** geklickt haben) Wählen Sie unten auf der Seite &quot;Hochladen&quot;die Option &quot;ZIP- oder Tear-Dateien beim Hochladen **entpacken&quot;aus, wenn Sie alle Dateien automatisch aus Ihrer hochgeladenen ZIP- oder TAR-Datei extrahieren möchten** . Beachten Sie, dass dieselbe Option auch im Dialogfeld &quot;Auftragsoptionen&quot;verfügbar ist.
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   Siehe [Optionen für das Hochladen](uploading-files.md#upload_options).

1. Klicken Sie im Dialogfeld „Upload-Auftragsoptionen“ auf **Speichern**.
1. Klicken Sie in der rechten unteren Ecke der Seite &quot;Hochladen&quot;auf **&quot;Hochladen** senden&quot;.

   Klicken Sie auf der globalen Navigationsleiste auf **Aufträge**, um den Fortschritt beim Hochladen anzuzeigen. Die Seite „Aufträge“ wird eingeblendet. Sie sehen darin den Fortschritt des Hochladevorgangs. Sie können die Arbeit in Dynamic Media Classic fortsetzen und jederzeit zur Seite &quot;Aufträge&quot;zurückkehren, um einen in Verarbeitung befindlichen Auftrag zu überprüfen.

Wenn Sie einen in Verarbeitung befindlichen Upload-Auftrag stornieren möchten, klicken Sie auf die Schaltfläche **Abbrechen** neben der Angabe „Dauer“.

## Dialogfeld &quot;Upload-Auftragsoptionen&quot; {#upload-options}

Beim Hochladen von Dateien stehen Ihnen im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die folgenden Optionen zur Verfügung:

* **AUFTRAG** — Klicken Sie auf **AUFTRAG** , um Optionen auszuwählen, die sich auf den gesamten Upload-Auftrag auswirken.

   Beachten Sie, dass Sie auch *Standardoptionen* zum Hochladen von Aufträgen auswählen können, indem Sie das Dialogfeld &quot; **Standard-Upload-Optionen** &quot;in den allgemeinen Einstellungen verwenden. Klicken Sie auf **Einstellungen > Anwendungseinstellungen > Allgemeine Einstellungen > Standard-Upload-Optionen** und legen Sie dann die gewünschten Standardoptionen fest.

   * **Wann** — Die Option &quot; **Wann** &quot;ist nur verfügbar, wenn Sie die Registerkarte &quot; **VIA FTP** &quot;ausgewählt haben.
      * **Einmalig** — Geben Sie einen Upload-Auftrag an, der einmal ausgeführt wird. Zu den Optionen gehören:
         * **Jetzt** — Führt den Upload-Auftrag unmittelbar aus, nachdem Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;auf **Speichern** geklickt haben, und klicken Sie dann auf der Seite &quot;Hochladen&quot;auf Hochladen **Hochladen** .
         * **Für später** einplanen — Wählen Sie Jahr, Monat, Tag und Uhrzeit (in Schritten von 15 Minuten) aus, für die der Upload-Auftrag ausgeführt werden soll.
      * **Wiederkehrend** — Geben Sie einen Upload-Auftrag an, der täglich, wöchentlich oder monatlich ausgeführt wird. Oder passen Sie den Upload-Auftrag nach Ihren eigenen Spezifikationen an.
         * **Täglich** — Legen Sie die Zeit fest, die der Auftrag täglich ausgeführt werden soll. Wenn der Auftrag nur von Montag bis Freitag ausgeführt werden soll, wählen Sie &quot;Nur **Wochentage**&quot;aus.
         * **Wöchentlich** — Wählen Sie einen bestimmten Wochentag und eine bestimmte Uhrzeit aus, zu der der Auftrag ausgeführt werden soll.
         * **Monatlich** — Wählen Sie einen bestimmten Wochentag (einschließlich der Beginn-Zeit) aus, an dem der Auftrag ausgeführt werden soll.
         * **Benutzerspezifisch** — Passen Sie das Zeitintervall für Upload- oder Veröffentlichungsaufträge an Ihre eigenen Spezifikationen an. Siehe [Festlegen eines individuellen Zeitintervalls für Upload-Aufträge bzw. Veröffentlichungsaufträge](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).
   * **Nach dem Hochladen** veröffentlichen — Verfügbar, wenn Sie entweder die Registerkarte &quot; **VON DESKTOP** &quot;oder &quot; **VIA FTP** &quot;ausgewählt haben. Wählen Sie diese Option, um die hochgeladenen Elemente automatisch zu veröffentlichen. Wenn Sie Dateien veröffentlichen, werden die Dateien an Live-Server gesendet. Die URLs für diese Dateien können dann auf externen Websites und in externen Anwendungen verwendet werden. Diese Option steht auch auf der Seite „Hochladen“ zur Verfügung.

   * **In jedem Ordner, demselben Asset-Namen, unabhängig von der Erweiterung** , überschreiben — Verfügbar, wenn Sie entweder die Registerkarte &quot; **VON DESKTOP** &quot;oder &quot; **VIA FTP** &quot;ausgewählt haben. Aktivieren Sie diese Option, wenn die hochgeladenen Dateien vorhandene gleichnamige Dateien ersetzen sollen. Diese Option steht auch auf der Seite „Hochladen“ zur Verfügung. The name of this option could be different, depending on the settings in **Application Setup > General Settings > Upload to Application > Overwrite Images**.

   * **Entpacken von ZIP- oder ZAR-Dateien beim Hochladen** — Verfügbar, wenn Sie entweder die Registerkarte &quot; **VON DESKTOP** &quot;oder &quot; **VIA FTP** &quot;ausgewählt haben.
Wählen Sie diese Option, wenn Sie alle Dateien automatisch aus Ihrer hochgeladenen ZIP- oder TAR-Datei extrahieren möchten. Beachten Sie, dass dieselbe Option auch im Dialogfeld &quot;Auftragsoptionen&quot;verfügbar ist.

   * **Unterordner einschließen** — Nur verfügbar, wenn Sie die Registerkarte &quot; **VIA FTP** &quot;ausgewählt haben.
Aktivieren Sie diese Option, wenn Sie auch die Unterordner im hochzuladenden Ordner hochladen möchten. Die Namen des hochgeladenen Ordners und der darin enthaltenen Unterordner werden automatisch in Dynamic Media Classic eingegeben.

   * **Metadatendateien** verarbeiten — Nur verfügbar, wenn Sie die Registerkarte &quot; **VIA FTP** &quot;ausgewählt haben. Wenn diese Option aktiviert ist, können Sie eine tabulatorgetrennte Datei oder XML-Datei hochladen, um gleichzeitig mehreren Assets Metadaten hinzuzufügen.
Siehe [Importieren von Metadaten (über FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **CROP-OPTIONS** — Um weiße Flächen automatisch von einem Bild abzuschneiden, öffnen Sie das Menü &quot;Beschneiden&quot;, wählen Sie &quot;Manuell&quot;und geben Sie in die Felder &quot;Oben&quot;, &quot;Rechts&quot;, &quot;Unten&quot;und &quot;Links&quot;die gewünschten Pixelwerte ein, um sie von den Kanten abzuschneiden. Sie können auch „Beschneiden“ > „Beschneiden“ und eine der folgenden Optionen wählen:

   * **Entfernen basierend auf** — Wählen Sie aus, ob das Bild basierend auf Farbe oder Transparenz beschnitten werden soll:

      * **Farbe** — Wählen Sie die Option &quot;Farbe&quot;. Wählen Sie anschließend im Menü „Ecke“ die Bildecke mit der Farbe aus, die der Farbe der weißen Flächen, die Sie entfernen möchten, am besten entspricht.

         Beschneiden basierend auf Farbe: Wenn Sie den Wert 0 einstellen, werden Pixel nur abgeschnitten, wenn sie exakt der Farbe entsprechen, die Sie in der Bildecke ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.

      * **Transparenz** —  Wählen Sie die Option &quot;Transparenz&quot;.

         Beschneiden basierend auf Transparenz: Wenn Sie den Wert 0 einstellen, werden Pixel nur abgeschnitten, wenn sie vollkommen transparent sind. Werte, die näher an 1 liegen, lassen eine größere Transparenz zu.

      * **Toleranz** — Ziehen Sie den Regler, um eine Toleranz zwischen 0 und 1 festzulegen.

* **PROFIL-OPTIONS** — Wählen Sie eine Farbkonvertierung, wenn Sie optimierte Dateien erstellen, die für den dynamischen Versand von Dynamic Media Classic verwendet werden:

   * **Beibehaltung der Standardfarbe** — Behält die Quellbildfarben bei, wenn die Bilder Farbrauminformationen enthalten; Es gibt keine Farbkonvertierung. Heutzutage ist in fast allen Bildern das entsprechende Farbprofil eingebettet. Wenn jedoch ein CMYK-Quellbild kein eingebettetes Farbprofil enthält, werden die Farben in den sRGB-Farbraum (standardmäßiges Rot Grün Blau) umgewandelt. sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Websites.

   * **Original-Farbraum** beibehalten — Behält die Originalfarben ohne Farbkonvertierung zum Zeitpunkt der Erfassung in Dynamic Media Classic bei. Bei Bildern ohne eingebettetes Farbprofil finden alle erforderlichen Konvertierungen zum Bearbeiten von Anforderungen für das Bild in den Standardfarbprofilen statt, die in den Veröffentlichungseinstellungen konfiguriert sind. Diese Farbprofile stimmen möglicherweise nicht mit der Farbe in Dateien überein, die mit dieser Option erstellt wurde. Deshalb empfehlen wir, die Option „Beibehaltung der Standardfarbe“ zu verwenden.

   * **Benutzerdefiniert von > bis** — Öffnet Menüs, in denen Sie einen Farbraum für &quot;Konvertieren von&quot;und &quot;Konvertieren in&quot;auswählen können. Diese erweiterte Option überschreibt alle Farbinformationen, die in die Quelldatei eingebettet sind. Wählen Sie diese Option nur, wenn alle übermittelten Profile falsche oder fehlende Farbdaten enthalten.

* **OPTIONS** ZUR BILDBEARBEITUNG — Sie können die Schnittmasken &lt;> in Bildern beibehalten und ein Profil auswählen.
Siehe [Bildbearbeitungsoptionen beim Hochladen](image-editing-options-upload.md#image-editing-options-at-upload).

* **POSTSCRIPT-OPTIONS** — Sie können PostScript® rastern, Dateien beschneiden, transparente Hintergründe beibehalten, eine Auflösung wählen und einen Farbraum wählen.
Siehe [Arbeiten mit PostScript- und Illustrator-Dateien](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **PHOTOSHOP OPTIONS** — Sie können Vorlagen aus Adobe® Photoshop®-Dateien erstellen, Ebenen verwalten, angeben, wie Ebenen benannt werden, Text extrahieren und angeben, wie Bilder in Vorlagen verankert werden.
Siehe [Optionen für das Hochladen von PSD-Dateien](psd-files.md#psd_upload_options).

* **PDF-OPTIONS** — Sie können die Dateien rastern, Suchbegriffe und Links extrahieren, automatisch einen E-Katalog erstellen, die Auflösung festlegen und einen Farbraum auswählen.
Siehe [Optionen für das Hochladen von PDF-Dateien](pdfs.md#pdf_upload_options).

* **ILLUSTRATOR OPTIONS** — Sie können Adobe Illustrator®-Dateien rastern, transparente Hintergründe beibehalten, eine Auflösung wählen und einen Farbraum wählen.
Siehe [Arbeiten mit PostScript- und Illustrator-Dateien](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **EVIDEO-OPTIONS** — Sie können eine Videodatei durch Auswahl einer Video-Vorgabe transkodieren.
Siehe [Arbeiten mit Videokodierungsvorgaben](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **ZUSÄTZLICHE METADATEN** — Geben Sie Suchbegriffe ein, die die hochzuladenden Dateien beschreiben. Trennen Sie Schlüsselwörter mit Kommata. Schlüsselwörter vereinfachen die Suche nach Assets. Siehe [Durchführen einer erweiterten Suche](searching-assets.md#conducting_an_advanced_search).

* **STAPELVORGABEN** — Wenn Sie aus den hochgeladenen Dateien ein Bildsatz, ein Multiachsen-Rotationsset oder ein Musterset erstellen möchten, klicken Sie auf die Spalte &quot;Aktiv&quot;für die gewünschte Vorgabe. Sie können mehrere Vorgaben auswählen. Die Vorgaben werden auf der Seite „Anwendungseinstellungen“ > „Stapelsatzvorgaben“ erstellt. Siehe [Stapelsatzvorgaben](application-setup.md#batch_set_presets).

* **ERWEITERT** — Siehe [Folgen Sie einem Upload-Auftrag](uploading-files.md#follow-an-upload-with-another-job).

## Starten eines weiteren Auftrags im Anschluss an einen Upload-Auftrag {#follow-an-upload-with-another-job}

Wenn Sie Elemente per FTP hochladen, können Sie einen Folgeauftrag unmittelbar nach Abschluss des Uploads beginnen lassen. (Wenn für diesen Zeitpunkt die Ausführung anderer Aufträge geplant ist, wird der hier terminierte Auftrag in der Warteschlange hinter diesen Aufträgen eingereiht.)

Für den neuen Auftrag wird eine Benachrichtigung an die von Ihnen festgelegte Adresse geschickt, sodass Code am vorgesehenen Ort ausgelöst werden kann. Der nachfolgende Veröffentlichungsauftrag erhält den Namen des Upload-Auftrags mit dem Präfix *Pub_*(für Publikation).

**So folgen Sie dem Hochladen mit einem anderen Auftrag**

1. Click **Upload**, then click the **VIA FTP** tab.
1. In the lower-right corner of the Upload page, click **Job Options**.
1. Erweitern Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;den Abschnitt **ADVANCED** .
1. Wählen Sie in der Dropdown-Liste &quot; **Nach Upload weiteren Auftrag** ausführen&quot;eine der folgenden Optionen:

   * Keine
   * HTTP-Anfrage
   * Veröffentlichung zum Image-Server
   * Mit Image Rendering veröffentlichen
   * Videoveröffentlichung

1. Geben Sie die HTTP-Adresse an.
1. Geben Sie an, ob Sie nur ausgeführt werden möchten, wenn Dateien hochgeladen wurden.
1. Geben Sie an, ob die Anfrage jedes Mal nach Abschluss eines Auftrags oder nur nach der Veröffentlichung von Dateien ausgeführt werden soll.

   >[!NOTE]
   >
   >Bei geplanten regelmäßigen Aufträgen werden unter Umständen keine Dateien veröffentlicht.

>[!MORELIKETHIS]
>
>* [Arbeiten mit Asset-Ordnern](asset-folders.md#working_with_asset_folders)
>* [Umgang mit wiederkehrenden Upload-Aufträgen und Veröffentlichungsaufträgen](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Verwenden eines Upload-Auftrags oder Veröffentlichungsauftrags als Auslöser](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

