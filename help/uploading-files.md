---
title: Hochladen von Dateien
seo-title: Hochladen von Dateien
description: 'null'
seo-description: Hier erfahren Sie, wie Sie Dateien hochladen.
uuid: b 3025 f 84-4 f 28-4276-bc 9 c-f 0 c 0 c 2 a 26 e 12
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: b 2 bc 3 bf 9-e 313-481 a -8670-c 3 bedde 21 b 1 a
translation-type: tm+mt
source-git-commit: 684950586bf9b1df897ac46b52d84a21f4cb4120

---


# Hochladen von Dateien{#uploading-files}

Bevor Sie Asset-Dateien in das Scene7 Publishing System hochladen, sollten Sie sich vergewissern, dass die Asset-Dateien korrekt benannt sind und dass die Ordnerstruktur Ihren Vorstellungen entspricht. Sie können Dateien von einer vom Classic Media Classic bereitgestellten FTP-Site oder direkt von Ihrem Computer oder Netzwerk aus hochladen. Dynamic Media Classic bietet Optionen zum Optimieren von Dateien beim Hochladen. Wenn Sie die Adobe Scene7 Publishing System-Desktop-Anwendung installieren, können Sie Dateien und Ordner vom Desktop in einen Zielordner ziehen und so in diesen Ordner hochladen. (Siehe [Allgemeine Programmeinstellungen](application-setup.md#general_settings).)

## Vorbereiten von Assets und Ordnern zum Hochladen {#preparing-your-assets-and-folders-for-uploading}

Vergewissern Sie sich vor dem Hochladen von Assets in das Scene7 Publishing System, dass diese das richtige Format und die richtige Größe haben. Außerdem müssen Sie die Regeln für dynamische Medien für die Benennung von Assets beachten. Indem Sie eine Ordnerorganisation und -struktur konfigurieren, erleichtern Sie sich das Auffinden von Dateien und die Arbeit mit den Dateien.

### Unterstützte Asset-Dateiformate {#supported-asset-file-formats}

In der folgenden Tabelle sind die vom Scene7 Publishing System unterstützten Asset-Dateiformate aufgeführt. For information on supported Camera Raw files, see [www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en).

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

### Asset-Typen {#asset-types}

Um optimale Ergebnisse mit der Plattform für dynamische Medien zu erzielen, sollten Sie die empfohlenen Dateiformate und -größen verwenden. In der folgenden Tabelle sind die empfohlenen Formate und Dateigrößen für häufig verwendete Assets aufgeführt.

| Asset-Typ | Beschreibung/Empfehlungen |
|--- |--- |
| Audio | Zu den Eingabeformaten von Audio-Assets gehören AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3. Sie können Audio-Daten in die folgenden Formate transcodieren: MP3, AAC und HE-AAC. |
| Bilder (für Bildgrößenänderungen, Zoom, Bildsätze, Rotationssets) | Bilder müssen an der längsten Seite mindestens 2000 Pixel haben. Die normalen Bildgrößen liegen zwischen 1500 und 2500 Pixel an der längsten Seite. Verlustfreie Bildformate, z. B. TIFF und PNG, sind zu empfehlen. Bei Verwendung eines JPEG-Bildes sollten Sie die höchste Qualitätseinstellung wählen. Animierte GIF-Dateien werden wie andere statische Inhalte behandelt. |
| E-Kataloge | Verwenden Sie hoch auflösende PDF-Dateien, die mit Adobe® Acrobat® oder einer Creative Suite-Anwendung erstellt und als „druckbereit“ gespeichert wurden. PDF-Dateien beinhalten alle erforderlichen Schriftarten, Bilder, Masken und Grafikelemente, auf die verwiesen wird, entweder als Einzelseiten, doppelseitige Druckbögen oder in einem mehrseitigen Format. Sortieren Sie die Seiten, indem Sie die Dateien in alphanumerischer Reihenfolge benennen. Platzieren Sie alle PDF-Dateien für einen E-Katalog in einem einzigen Ordner, um das Hochladen zu vereinfachen. Beim Hochladen können Sie Schnittoptionen auswählen, um die Zuschneidebereiche, einschließlich Schnittmarken, Passermarken oder Farbkontrollstreifen, aus den PDF-Dateien zu entfernen. Da die meisten druckbereiten PDF-Dateien im CMYK-Farbraum gespeichert werden, ist es wichtig, das für die PDF-Dateien verwendete ICC-Farbprofil für CMYK zu ermitteln und abzurufen. |
| Vorlagen | Bild- oder Layoutentwürfe mit Ebenen können Text, Bilder und Ebenen enthalten. Bildebenen, Textzeichenfolgen und Ebenenattribute wie Farbe und Größe können parametrisiert werden, sodass variable Daten angepasst werden können. Die Anforderungen für in Vorlagen verwendete Bilder sind dieselben wie für andere Bilder. Bereiten Sie Grafiken in Photoshop oder einem anderen Bildbearbeitungsprogramm vor. Speichern Sie jede Grafik einzeln als reduzierte, transparente Datei im TIFF- oder PNG-Format. Stellen Sie sicher, dass die Bildauflösung für den beabsichtigten Verwendungszweck geeignet ist. Bilder, die für Druckzwecke verwendet werden sollen, sollten eine Auflösung von 300 ppi besitzen. |
| Videos | Dynamic Media Classic unterstützt Videodateien, die im Format OGV und MP 4 gespeichert wurden. Sie können Dateien beim Hochladen in das Format MP 4 transkodieren. Siehe [Unterstützte Asset-Dateiformate](#supported-static-file-formats). |
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
>Beim Hochladen von Bilddateien und PDF-Dateien in SPS konvertiert das System diese Quelldateien in P-TIFF-Dateien (Pyramid TIFF). Diese P-TIFF-Dateien werden später auf dynamischen Medienservern veröffentlicht. Dynamic Media Classic verwendet das Pyramid Tiff-Dateiformat, da es verschiedene Zoomverhältnisse enthält, die beim Anzeigen mit einem dynamischen Media-Zoom-Viewer einen schnellen Zoom ermöglichen.

### Unterstützte statische Dateiformate {#supported-static-file-formats}

Dynamic Media Classic unterstützt mehrere statische Dateiformate. Statischer Inhalt ist ein beliebiges Asset, das veröffentlicht wird, z. B. CSS, PDF, SVG, XML usw.

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

Dynamic Media Classic bietet keine Option zum Generieren einer Vorschau-URL von statischem Inhalt.

### Dateinamenanforderungen {#filename-requirements}

Da beim Hochladen die Erweiterungen aus den Dateinamen entfernt werden, sind Dateien mit demselben Stammnamen nicht zulässig. Im System "Dynamic Media Classic" wird der Asset-Dateiname ohne die Dateinamenerweiterung zur Asset-ID für das Asset. Deshalb muss jedes Asset einen eindeutigen Namen haben.

Stellen Sie deshalb sicher, dass allen Benutzern in Ihrem Unternehmen die folgenden Dateinamensregeln vertraut sind:

* Asset-IDs mit exakt demselben Namen sind im System nicht zulässig.
* Bei Asset-ID-Namen wird die Groß-/Kleinschreibung berücksichtigt.
* Asset-IDs sollten keine Leerzeichen enthalten (z. B. nicht „Schwarze Jacke.tif“ oder „Blaue Jacke.jpg“). Dynamic Media Classic ASCII-kodiert Leerzeichen in Asset-Namen, wenn sie Asset-Namen zum Erstellen von URL-Zeichenfolgen verwenden. Diese ASCII-Codierung beeinträchtigt jedoch die Lesbarkeit der URLs.
* Sprachspezifische Zeichen sind in Dateinamen zulässig. Allerdings dürfen Dateinamen die folgenden Zeichen nicht enthalten:

   \ ; / ? : @ &amp; = + $ , * " &lt; &gt; | ' { } %

   Wenn ein Dateiname eines oder mehrere der oben aufgeführten Zeichen enthält, werden die Zeichen beim Hochladen aus dem Dateinamen entfernt.

In den meisten Fällen kann als Asset-Dateiname die Elementnummer, Produkt-SKU oder ein anderer Name des dargestellten Elements verwendet werden, wie im Folgenden:

| Element | Dateiname | Asset-ID |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Ordnerorganisation und -struktur {#folder-organization-and-structure}

Erstellen Sie im Scene7 Publishing System eine Ordner- und Unterordnerorganisationsstruktur, bevor Sie die eigentlichen Inhalte in das System hochladen. Eine solche Vorausplanung hat die folgenden zwei wichtigen Vorteile:

* Wenn Sie die Inhalte per FTP in SPS hochladen, können Sie das System anweisen, Ihre Ordnerstruktur beim Hochladen zu replizieren. Auf diese Weise werden die Inhalte in SPS in denselben Ordnern und Unterordnern organisiert wie auf Ihrem Computer oder in Ihrem Netzwerk. (Um die Ordnerstruktur in SPS zu replizieren, wählen Sie beim Hochladen von Assets per FTP die Option „Unterordner einschließen“.)
* Es ist sehr viel schwieriger, Ordner nach dem Hochladen der Dateien innerhalb des Systems neu zu organisieren, als vorab eine sorgfältig vorbereitete Ordnerstruktur zu erstellen.

Welche Vorgehensweise Sie bei der Benennung von Ordnern und der Ordnerstruktur im Scene7 Publishing System verfolgen, hängt vom Bedarf Ihres Unternehmens ab. Es folgen einige Beispiele für Ordnerstrukturen:

**SKU-basierte** Ordner werden gemäß skus oder Elementnummern benannt. Beispielsweise werden separate Ordner für alle mit 0, 20, 30 usw. beginnenden Nummerserien erstellt. 

**Markenbasiertes** Unternehmen für Hersteller mehrerer Marken und Einzelhändler, die andere Marken anderer Unternehmen verkaufen, trennen Sie Dateien in Produktordner, die nach verschiedenen Marken benannt sind.

**Projektbasierte** Ordner werden nach dem Start-/Ablegen-Datum oder dem Projektnamen organisiert. Kunden, die hauptsächlich E-Kataloge erstellen, bevorzugen diese Vorgehensweise.

**Spiegeln der Website-Ordnerhierarchie** Diese Ordnerstruktur spiegelt die Ordnerstruktur der Website zusammen mit den Ordnern für Produktkategorien wider.

## Grundlagen zum Hochladen von Dateien {#uploading-your-files}

Sie können einzelne Dateien vom Desktop oder Ordner über FTP hochladen. If you want to upload more than 100 MB of files or upload entire folders and subfolders, select the **VIA FTP** tab.

Wenn Sie die Scene 7 Publishing System-Desktopanwendung installiert haben, können Sie Dateien und Ordner direkt vom Desktop in den Zielordner ziehen.

Sie erhalten vom Scene7 Publishing System eine E-Mail zur Bestätigung des Beginns und Endes Ihres Upload-Auftrags; Sie werden außerdem benachrichtigt, wenn Probleme auftreten.

Während eines oder unmittelbar nach einem großen Upload-Auftrag(s) wird u. U. für einige neue Elemente die Meldung „Bild wurde noch nicht optimiert“ angezeigt. Diese Meldung wird angezeigt, da die Dateien noch nicht vollständig verarbeitet und dem SPS hinzugefügt wurden. Sie können die betroffenen Dateien später optimieren. (Siehe [Optimieren von Dateien](application-setup.md#optimize_files).)

### Hochladen von Dateien über die Registerkarte VON DESKTOP {#upload-files-using-sps-desktop-application}

Mit der Scene7 Publishing System-Desktop-Anwendung können Sie Dateien und Ordner in einen Zielordner ziehen und so in diesen Ordner hochladen.

1. Klicken Sie in der Desktop-Anwendung von Scene7 Publishing System auf der globalen Navigationsleiste auf **Hochladen**.
1. On the Upload page, click the **FROM DESKTOP** tab.
1. Klicken Sie auf der linken Seite der Seite Hochladen im Bereich **"Hochzuladende Dateien** auswählen" auf **Durchsuchen** , um die Dateien oder Ordner auszuwählen, die Sie hochladen möchten, und klicken Sie dann auf **Öffnen**.
1. Navigieren Sie auf der rechten Seite der Seite **"Hochladen" im** Bereich" Ordner auswählen" zu einem Zielordner, in den die hochgeladenen Dateien oder Ordner eingefügt werden sollen.
1. (Optional) Geben Sie unten auf der Seite "Hochladen" im Feld **" Auftragsname** " den neuen Namen des Upload-Auftrags an. Sie können auch einfach den standardmäßigen, systemgenerierten Namen verwenden, den SPS bereitstellt. Dieser Auftrag wird ebenso wie andere Upload- und Veröffentlichungsaufträge auf der Seite „Aufträge“ erfasst – hier können Sie den Status von Aufträgen prüfen.
Siehe [Überprüfen von Auftragsdateien](checking-job-files.md#checking_job_files).
1. (Optional) Wählen Sie unten auf der Seite "Hochladen" die Option Nach dem Hochladen **veröffentlichen,** wenn Sie die hochgeladenen Assets automatisch veröffentlichen möchten.
Wenn Sie Dateien veröffentlichen, werden die Dateien an Live-Server gesendet. Die URLs für diese Dateien können dann auf externen Websites und in externen Anwendungen verwendet werden. Beachten Sie, dass dieselbe Option auch im Dialogfeld "Auftragsoptionen" verfügbar ist.
1. (Optional) Wählen Sie unten auf der Seite "Hochladen" die Option **In einem beliebigen Ordner überschreiben, unabhängig von der Erweiterung,** wenn die hochgeladenen Dateien vorhandene Dateien mit denselben Namen ersetzen sollen. Beachten Sie, dass dieselbe Option auch im Dialogfeld "Auftragsoptionen" verfügbar ist.
The name of this option could be different, depending on the settings in **Application Setup &gt; General Settings &gt; Upload to Application &gt; Overwrite Images**.
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   Siehe [Optionen für das Hochladen](uploading-files.md#upload_options).

1. Klicken Sie im Dialogfeld „Upload-Auftragsoptionen“ auf **Speichern**.
1. Klicken Sie in der rechten unteren Ecke der Seite "Hochladen" auf" Hochladen **senden**«.
Klicken Sie auf der globalen Navigationsleiste auf **Aufträge**, um den Fortschritt beim Hochladen anzuzeigen. Sie können Ihre Arbeit im Scene7 Publishing System fortsetzen und bei Bedarf jederzeit wieder zur Seite „Aufträge“ wechseln, um einen in Verarbeitung befindlichen Auftrag zu überprüfen. Wenn Sie einen in Verarbeitung befindlichen Upload-Auftrag stornieren möchten, klicken Sie auf die Schaltfläche **Abbrechen** neben der Angabe „Dauer“.

### Hochladen von Dateien über die Registerkarte "ÜBER FTP « {#upload-files-using-via-ftp}

1. Melden Sie sich bei der Google Media Classic-FTP-Site an, die speziell für Ihre Region gilt. Melden Sie sich mit dem von Ihrem Administrator erhaltenen FTP-Benutzernamen und -Kennwort an.
1. Klicken Sie in Dynamic Media Classic in der Symbolleiste für globale Navigation auf **Hochladen**.
1. On the Upload page, click the **VIA FTP** tab.
1. Wählen Sie auf der linken Seite der Seite "Hochladen" im **Bereich" FTP-Ordner für Upload** auswählen" einen FTP-Ordner aus, aus dem Dateien hochgeladen werden sollen.
1. Wählen Sie rechts auf der Seite "Hochladen **«im Bereich" Zielordner** wählen" einen Zielordner im Scene 7 Publishing System aus.
1. (Optional) Geben Sie unten auf der Seite "Hochladen" im Feld **" Auftragsname** " den neuen Namen des Upload-Auftrags an. Sie können auch einfach den standardmäßigen, systemgenerierten Namen verwenden, den SPS bereitstellt. Dieser Auftrag wird ebenso wie andere Upload- und Veröffentlichungsaufträge auf der Seite „Aufträge“ erfasst – hier können Sie den Status von Aufträgen prüfen.
Siehe [Überprüfen von Auftragsdateien](checking-job-files.md#checking_job_files).
1. (Optional) Wählen Sie unten auf der Seite "Hochladen" die Option **Nach dem Hochladen** veröffentlichen, wenn Sie die hochgeladenen Assets automatisch veröffentlichen möchten.
Wenn Sie Dateien veröffentlichen, werden die Dateien an Live-Server gesendet. Die URLs für diese Dateien können dann auf externen Websites und in externen Anwendungen verwendet werden. Beachten Sie, dass dieselbe Option auch im Dialogfeld "Auftragsoptionen" verfügbar ist.
1. (Optional) Wählen Sie unten auf der Seite "Hochladen" die Option **In einem beliebigen Ordner überschreiben, unabhängig von der Erweiterung,** wenn die hochgeladenen Dateien vorhandene Dateien mit denselben Namen ersetzen sollen. Beachten Sie, dass dieselbe Option auch im Dialogfeld "Auftragsoptionen" verfügbar ist.
The name of this option could be different, depending on the settings in **Application Setup &gt; General Settings &gt; Upload to Application &gt; Overwrite Images**.
1. (Optional; nur verfügbar, wenn Sie auf die Registerkarte **Über FTP** klicken) Wählen Sie unten auf der Seite Hochladen die Option **Entpackt Zip- oder Tar-Dateien beim Hochladen** aus, wenn Sie alle Dateien aus Ihrer hochgeladenen ZIP- oder TAR-Datei automatisch extrahieren möchten. Beachten Sie, dass dieselbe Option auch im Dialogfeld "Auftragsoptionen" verfügbar ist.
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   Siehe [Optionen für das Hochladen](uploading-files.md#upload_options).

1. Klicken Sie im Dialogfeld „Upload-Auftragsoptionen“ auf **Speichern**.
1. Klicken Sie in der rechten unteren Ecke der Seite "Hochladen" auf" Hochladen **senden**«.

   Klicken Sie auf der globalen Navigationsleiste auf **Aufträge**, um den Fortschritt beim Hochladen anzuzeigen. Die Seite „Aufträge“ wird eingeblendet. Sie sehen darin den Fortschritt des Hochladevorgangs. Sie können Ihre Arbeit im Scene7 Publishing System fortsetzen und bei Bedarf jederzeit wieder zur Seite „Aufträge“ wechseln, um einen in Verarbeitung befindlichen Auftrag zu überprüfen.

Wenn Sie einen in Verarbeitung befindlichen Upload-Auftrag stornieren möchten, klicken Sie auf die Schaltfläche **Abbrechen** neben der Angabe „Dauer“.

## Upload-Auftragsoptionen, Dialogfeld {#upload-options}

Beim Hochladen von Dateien können Sie aus den folgenden Optionen im Dialogfeld "Upload-Auftragsoptionen" auswählen:

* **JOB** — Klicken **Sie auf JOB,** um die Optionen auszuwählen, die sich auf den gesamten Upload-Auftrag auswirken.

   Sie können *auch Standardoptionen* für das Hochladen von Aufträgen festlegen, indem Sie unter "Allgemeine Einstellungen" das Dialogfeld" **Standardupload-Optionen** " verwenden. Klicken **Sie auf Einstellungen &gt; Anwendungseinstellungen &gt; Allgemeine Einstellungen &gt; Standardmäßige Upload-Optionen** und legen Sie dann die gewünschten Standardoptionen fest.

   * **Wann** — Die **Option "Wann"** ist nur verfügbar, wenn Sie die Registerkarte **" ÜBER FTP** " ausgewählt haben.
      * **Einmalig** — Geben Sie einen Upload-Auftrag an, der einmal ausgeführt wird. Zu den Optionen zählen:
         * **** Jetzt— Führt den Upload-Auftrag unmittelbar nach dem Klicken **auf Speichern** im Dialogfeld Upload-Auftragsoptionen aus und klicken **dann auf der Seite Hochladen auf Hochladen** starten.
         * **Für später** planen— Wählen Sie das Jahr, den Monat, den Tag und die Uhrzeit (in Schritten von 15 Minuten) aus, die der Upload-Auftrag ausführen soll.
      * **Wiederholt** — Geben Sie einen Upload-Auftrag an, der täglich, wöchentlich oder monatlich ausgeführt wird. Oder passen Sie den Upload-Auftrag auf Ihre eigenen Spezifikationen an.
         * **Täglich** — Legen Sie den Zeitpunkt fest, an dem der Auftrag jeden Tag ausgeführt werden soll. Wenn der Auftrag nur Montag bis Freitag ausgeführt werden soll, wählen Sie **"Nur Wochentage"** aus.
         * **Wöchentlich** — Wählen Sie einen bestimmten Wochentag aus, an dem der Auftrag ausgeführt werden soll.
         * **Monatlich** — Wählen Sie einen bestimmten Tag des Monats oder Tages der Woche aus, einschließlich der Startzeit, die der Auftrag ausführen soll.
         * **Benutzerdefiniert** — Passen Sie ein Zeitintervall für Upload-Aufträge oder Veröffentlichungsaufträge an Ihre eigenen Spezifikationen an. Siehe [Festlegen eines individuellen Zeitintervalls für Upload-Aufträge bzw. Veröffentlichungsaufträge](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).
   * **Nach dem Hochladen** veröffentlichen— Verfügbar, wenn Sie die Registerkarte **"FROM DESKTOP** «oder die Registerkarte **" ÜBER FTP** " ausgewählt haben. Wählen Sie diese Option, um die hochgeladenen Elemente automatisch zu veröffentlichen. Wenn Sie Dateien veröffentlichen, werden die Dateien an Live-Server gesendet. Die URLs für diese Dateien können dann auf externen Websites und in externen Anwendungen verwendet werden. Diese Option steht auch auf der Seite „Hochladen“ zur Verfügung.

   * **In beliebigem Ordner und demselben Namen unabhängig von der Erweiterung** überschreiben— Verfügbar, wenn Sie die Registerkarte **"FROM DESKTOP** «oder die Registerkarte **" ÜBER FTP** " ausgewählt haben. Aktivieren Sie diese Option, wenn die hochgeladenen Dateien vorhandene gleichnamige Dateien ersetzen sollen. Diese Option steht auch auf der Seite „Hochladen“ zur Verfügung. The name of this option could be different, depending on the settings in **Application Setup &gt; General Settings &gt; Upload to Application &gt; Overwrite Images**.

   * **Dekomprimieren von Zip- oder Tar-Dateien beim Hochladen** — Verfügbar, wenn Sie die Registerkarte **"FROM DESKTOP** «oder die Registerkarte **" ÜBER FTP** " ausgewählt haben.
Wählen Sie diese Option, wenn Sie alle Dateien aus Ihrer hochgeladenen ZIP- oder TAR-Datei automatisch extrahieren möchten. Beachten Sie, dass dieselbe Option auch im Dialogfeld "Auftragsoptionen" verfügbar ist.

   * **Unterordner** einschließen— Nur verfügbar, wenn Sie die Registerkarte **Über FTP** ausgewählt haben.
Aktivieren Sie diese Option, wenn Sie auch die Unterordner im hochzuladenden Ordner hochladen möchten. Der Name des hochgeladenen Ordners und die Namen der darin enthaltenen Unterordner werden automatisch in das SPS eingetragen.

   * **Metadatendateien verarbeiten** — Nur verfügbar, wenn Sie die Registerkarte **Über FTP** ausgewählt haben. Wenn diese Option aktiviert ist, können Sie eine tabulatorgetrennte Datei oder XML-Datei hochladen, um gleichzeitig mehreren Assets Metadaten hinzuzufügen.
Siehe [Importieren von Metadaten (über FTP)](viewing-adding-exporting-metadata.md#import-metadata).


* **BESCHNEIDUNGSOPTIONEN** : Um weiße Randpixel automatisch von einem Bild zu entfernen, öffnen Sie das Menü "Beschneiden" , wählen Sie" Manuell" und geben Sie in den Feldern "Oben" ," Rechts" , "Unten" und" Links" Pixelmaße ein, um den Abstand von den Seiten zu entfernen. Sie können auch „Beschneiden“ &gt; „Beschneiden“ und eine der folgenden Optionen wählen:

   * **Beschneiden basierend** auf— Wählen Sie aus, ob basierend auf Farbe oder Transparenz abgeschnitten werden soll:

      * **Farbe** — Wählen Sie die Option "Farbe" . Wählen Sie anschließend im Menü „Ecke“ die Bildecke mit der Farbe aus, die der Farbe der weißen Flächen, die Sie entfernen möchten, am besten entspricht.

         Beschneiden basierend auf Farbe: Wenn Sie den Wert 0 einstellen, werden Pixel nur abgeschnitten, wenn sie exakt der Farbe entsprechen, die Sie in der Ecke des Bilds ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.

      * **Transparenz** — Wählen Sie die Option "Transparenz" .

         Beschneiden basierend auf Transparenz: Wenn Sie den Wert 0 einstellen, werden Pixel nur abgeschnitten, wenn sie vollkommen transparent sind. Werte, die näher an 1 liegen, lassen eine größere Transparenzabweichung zu.

      * **Toleranz** — Ziehen Sie den Schieberegler, um eine Toleranz zwischen 0 und 1 anzugeben.

* **FARBPROFILOPTIONEN** — Wählen Sie eine Farbkonvertierung, wenn Sie optimierte Dateien erstellen, die für dynamische dynamische Medien Classic verwendet werden:

   * **Beibehaltung** der Standardfarbe— Behält die Quellbildfarben bei, wenn die Bilder Farbraum-Informationen enthalten; Es gibt keine Farbkonvertierung. Heutzutage ist in fast allen Bildern das entsprechende Farbprofil eingebettet. Wenn jedoch ein CMYK-Quellbild kein eingebettetes Farbprofil enthält, werden die Farben in den sRGB-Farbraum (standardmäßiges Rot Grün Blau) umgewandelt. sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Websites.

   * **Ursprünglichen Farbraum** beibehalten— Behält die ursprünglichen Farben ohne Farbkonvertierung bei, während die Erfassung im Scene 7 Publishing System erfolgt. Bei Bildern ohne eingebettetes Farbprofil finden alle erforderlichen Konvertierungen zum Bearbeiten von Anforderungen für das Bild in den Standardfarbprofilen statt, die in den Veröffentlichungseinstellungen konfiguriert sind. Diese Farbprofile stimmen möglicherweise nicht mit der Farbe in Dateien überein, die mit dieser Option erstellt wurde. Deshalb empfehlen wir, die Option „Beibehaltung der Standardfarbe“ zu verwenden.

   * **Benutzerdefiniert von &gt; Bis** — Öffnet die Menüs "Konvertieren von" und" Konvertieren in" . Diese erweiterte Option überschreibt alle Farbinformationen, die in die Quelldatei eingebettet sind. Sie sollten diese Option nur auswählen, wenn alle gesendeten Bilder falsche oder fehlende Farbprofildaten enthalten.

* **BILDBEARBEITUNGSOPTIONEN** — Sie können die Beschneidungs-&lt; &gt; Masken in Bildern beibehalten und ein Farbprofil auswählen.
Siehe [Bildbearbeitungsoptionen beim Hochladen](image-editing-options-upload.md#image-editing-options-at-upload).

* **Postscript-OPTIONEN** — Sie können postscript®-Dateien rastern, Dateien beschneiden, transparente Hintergründe beibehalten, eine Auflösung auswählen und einen Farbraum auswählen.
Siehe [Arbeiten mit PostScript- und Illustrator-Dateien](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **PHOTOSHOP-OPTIONEN** — Sie können Vorlagen aus Adobe® Photoshop®-Dateien erstellen, Ebenen beibehalten, angeben, wie Ebenen benannt werden, Text extrahieren und angeben, wie Bilder in Vorlagen verankert werden.
Siehe [Optionen für das Hochladen von PSD-Dateien](psd-files.md#psd_upload_options).

* **PDF-OPTIONEN** — Sie können die Dateien rastern, Suchbegriffe und Links extrahieren, automatisch einen E-Katalog generieren, die Auflösung festlegen und einen Farbraum auswählen.
Siehe [Optionen für das Hochladen von PDF-Dateien](pdfs.md#pdf_upload_options).

* **ILLUSTRATOR-OPTIONEN** — Sie können Adobe Illustrator®-Dateien rastern, transparente Hintergründe beibehalten, eine Auflösung auswählen und einen Farbraum auswählen.
Siehe [Arbeiten mit PostScript- und Illustrator-Dateien](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **EVIDEO-OPTIONEN** — Sie können eine Videodatei durch Auswahl einer Video-Vorgabe transkodieren.
Siehe [Arbeiten mit Videokodierungsvorgaben](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **ZUSÄTZLICHE METADATEN** — Geben Sie Suchbegriffe ein, die die hochzuladenden Dateien beschreiben. Trennen Sie Schlüsselwörter mit Kommata. Schlüsselwörter vereinfachen die Suche nach Assets. Siehe [Durchführen einer erweiterten Suche](searching-assets.md#conducting_an_advanced_search).

* **STAPELSATZVORGABEN** — Wenn Sie einen Bildsatz, ein Multiachsen-Rotationsset oder ein Musterset aus den hochgeladenen Dateien erstellen möchten, klicken Sie auf die Spalte "Aktiv" für die gewünschte Vorgabe. Sie können mehrere Vorgaben auswählen. Die Vorgaben werden auf der Seite „Anwendungseinstellungen“ &gt; „Stapelsatzvorgaben“ erstellt. Siehe [Stapelsatzvorgaben](application-setup.md#batch_set_presets).

* **ADVANCED** — Siehe [Hochladen eines weiteren Auftrags](uploading-files.md#follow-an-upload-with-another-job).

## Starten eines weiteren Auftrags im Anschluss an einen Upload-Auftrag {#follow-an-upload-with-another-job}

Wenn Sie Elemente per FTP hochladen, können Sie einen Folgeauftrag unmittelbar nach Abschluss des Uploads beginnen lassen. (Wenn für diesen Zeitpunkt die Ausführung anderer Aufträge geplant ist, wird der hier terminierte Auftrag in der Warteschlange hinter diesen Aufträgen eingereiht.)

Für den neuen Auftrag wird eine Benachrichtigung an die von Ihnen festgelegte Adresse geschickt, sodass Code am vorgesehenen Ort ausgelöst werden kann. Der nachfolgende Veröffentlichungsauftrag erhält den Namen des Upload-Auftrags mit dem Präfix *Pub_*(für Publikation).

**So folgen Sie dem Hochladen mit einem anderen Auftrag**

1. Click **Upload**, then click the **VIA FTP** tab.
1. In the lower-right corner of the Upload page, click **Job Options**.
1. Erweitern Sie im Dialogfeld "Upload-Auftragsoptionen" den Abschnitt **Erweitert** .
1. Wählen Sie eine der folgenden Optionen aus dem **Anschluss nach dem Hochladen mit einer anderen** Dropdownliste:

   * Keine
   * HTTP-Anfrage
   * Veröffentlichung zum Image-Server
   * Mit Image Rendering veröffentlichen
   * Videoveröffentlichung

1. Geben Sie die HTTP-Adresse an.
1. Geben Sie an, ob Sie nur ausführen möchten, wenn Dateien hochgeladen wurden.
1. Geben Sie an, ob die Anfrage jedes Mal nach Abschluss eines Auftrags oder nur nach der Veröffentlichung von Dateien ausgeführt werden soll.

   >[!NOTE]
   >
   >Bei geplanten regelmäßigen Aufträgen werden unter Umständen keine Dateien veröffentlicht.

>[!MORELIKETHIS]
>
>* [Arbeiten mit Asset-Ordnern](asset-folders.md#working_with_asset_folders)
>* [Umgang mit wiederkehrenden Upload-Aufträgen und Veröffentlichungsaufträgen](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Verwenden eines Upload-Auftrags oder Veröffentlichungsauftrags als Auslöser](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

