---
title: Hochladen von Dateien
description: Erfahren Sie, wie Sie Dateien in Adobe Dynamic Media Classic hochladen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '3868'
ht-degree: 25%

---

# Hochladen von Dateien{#uploading-files}

Stellen Sie vor dem Hochladen von Asset-Dateien in Adobe Dynamic Media Classic sicher, dass die Asset-Dateien korrekt benannt sind. Stellen Sie außerdem sicher, dass Ihre Ordnerstruktur so eingerichtet und organisiert ist, wie Sie möchten. Sie können Dateien von einer von Adobe Dynamic Media Classic bereitgestellten FTP-Site oder direkt von Ihrem Computer oder Netzwerk hochladen. Adobe Dynamic Media Classic bietet Optionen zum Optimieren von Dateien beim Hochladen. Wenn Sie das Adobe Dynamic Media Classic Desktop-Programm installiert haben, können Sie Dateien und Ordner hochladen, indem Sie sie direkt von Ihrem Desktop ziehen. Siehe [Allgemeine Programmeinstellungen](application-setup.md#general_settings).

## Vorbereiten von Assets und Ordnern auf das Hochladen {#preparing-your-assets-and-folders-for-uploading}

Stellen Sie vor dem Hochladen von Assets in Adobe Dynamic Media Classic sicher, dass sie das richtige Format und die richtige Größe aufweisen. Außerdem müssen Sie die Adobe Dynamic Media Classic-Regeln für die Benennung von Assets beachten. Indem Sie eine Ordnerorganisation und -struktur konfigurieren, erleichtern Sie sich das Auffinden von Dateien und die Arbeit mit den Dateien.

### Unterstützte Asset-Dateiformate {#supported-asset-file-formats}

In dieser Tabelle werden die von Adobe Dynamic Media Classic unterstützten Asset-Dateiformate aufgeführt. Informationen zu unterstützten Camera Raw-Dateien finden Sie unter [https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html).

| Asset-Dateiformate | Beschreibung |
| --- | --- |
| Audio | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Cascading Stylesheet | CSS |
| Farbprofile | ICC, ICM |
| Schriftarten | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | AI, FXG |
| Bilder | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (nur Windows®), TIF, TIFF |
| InDesign | INDD, INDT |
| MS® Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG und Camera Raw |
| PostScript | EPS, PS |
| Adobe Dynamic Media Classic Image Authoring | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Video | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

Die Upload-Unterstützung von ZIP- und TAR-Archiven umfasst ein Kontrollkästchen, mit dem Sie angeben können, ob die Dateien entpackt werden sollen.

### Nicht unterstützte Bildformate in Dynamic Media {#unsupported-image-formats-dynamic-media}

In der folgenden Liste werden die Untertypen der Rasterbilddateiformate beschrieben, die in Dynamic Media nicht *unterstützt werden.*

Siehe auch [Erkennung nicht unterstützter Dateiformate für Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* PNG-Dateien mit einer IDAT-Blockgröße größer als 100 MB.
* PSB-Dateien.
* PSD-Dateien mit einem anderen Farbraum als CMYK, RGB, Graustufen oder Bitmap werden nicht unterstützt. DuoTone, Lab und indizierte Farbräume werden nicht unterstützt.
* PSD-Dateien mit einer Bittiefe größer als 16.
* TIFF-Dateien mit Gleitkommadaten.
* TIFF-Dateien mit Lab-Farbraum.

### Asset-Typen {#asset-types}

Um mit dem Adobe Dynamic Media Classic-Programm optimale Ergebnisse zu erzielen, sollten Sie die empfohlenen Dateiformate und -größen verwenden. In der folgenden Tabelle sind die empfohlenen Formate und Dateigrößen für häufig verwendete Assets aufgeführt.

| Asset-Typ | Beschreibung/Empfehlungen |
| --- | --- |
| Audio | Zu den Eingabeformaten von Audio-Assets gehören AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3. Sie können Audio-Daten in die folgenden Formate transcodieren: MP3, AAC und HE-AAC. |
| Bilder (für Bildgrößenänderungen, Zoom, Bildsätze, Rotationssets) | Bilder müssen mindestens 2000 Pixel bei der längsten Größe aufweisen. Die typischen Bildgrößen reichen von 1500 bis 2500 Pixel bei der längsten Größe. Verlustfreie Bildformate, z. B. TIFF und PNG, sind zu empfehlen. Bei Verwendung eines JPEG-Bildes sollten Sie die höchste Qualitätseinstellung wählen. Animierte GIF-Dateien werden wie andere statische Inhalte behandelt. |
| E-Kataloge | Verwenden Sie hochauflösende PDF-Dateien, die in Adobe Acrobat erstellt wurden, oder eine Adobe-Creative Suite-Anwendung, die als &quot;druckbereit&quot;gespeichert wurde. PDF enthalten alle benötigten Schriftarten, Bilder und Masken. Schließen Sie alle erforderlichen referenzierten grafischen Elemente ein, entweder als Einzelseiten, doppelseitige Tabellen oder in einem mehrseitigen Format. Sortieren Sie die Seiten, indem Sie die Dateien in alphanumerischer Reihenfolge benennen. Platzieren Sie alle PDF-Dateien für einen E-Katalog in einem einzigen Ordner, um das Hochladen zu vereinfachen. Beim Hochladen können Sie Schnittoptionen auswählen, um die Zuschneidebereiche, einschließlich Schnittmarken, Passermarken oder Farbkontrollstreifen, aus den PDF-Dateien zu entfernen. Da die meisten druckbereiten PDF-Dateien im CMYK-Farbraum gespeichert werden, ist es wichtig, das für die PDF-Dateien verwendete ICC-Farbprofil für CMYK zu ermitteln und abzurufen. |
| Vorlagen | Bild- oder Layoutentwürfe mit Ebenen können Text, Bilder und Ebenen enthalten. Bildebenen, Textzeichenfolgen und Ebenenattribute wie Farbe und Größe können parametrisiert werden, sodass variable Daten angepasst werden können. Die Anforderungen für in Vorlagen verwendete Bilder sind dieselben wie für andere Bilder. Bereiten Sie Grafiken in Photoshop oder einem anderen Bildbearbeitungsprogramm vor. Speichern Sie jede Grafik einzeln als reduzierte, transparente Datei im TIFF- oder PNG-Format. Stellen Sie sicher, dass die Bildauflösung für den beabsichtigten Verwendungszweck geeignet ist. Bilder für den Druck sind 300 ppi. |
| Videos | Adobe Dynamic Media Classic unterstützt Videodateien im OGV- und MP4-Format. Sie können Dateien beim Hochladen in das MP4-Format transkodieren. Siehe [Unterstützte Asset-Dateiformate](#supported-static-file-formats). |
| Schriftarten | Hochgeladen TrueType, `Type1` (nur Windows®), OpenType®-Schriftarten und FotoFonts. |
| Bilder | Bilder und Bilddateien mit mehreren Ebenen. |
| Bildsätze und Mustersets | Sammlungen zusammengehöriger Bilder, die in einem Viewer angezeigt werden können. |
| ICC-Profile | Ein Farbprofil, mit dem Sie ein hochgeladenes Bild aus dem Quellfarbraum in einen anderen Farbraum konvertieren können. |
| Vignetten | Mit dem Image Authoring-Programm erstellte Bilder und zugehörige Dateien. |
| Inhaltsdateien | Adobe InDesign-, Illustrator- oder Photoshop-Inhaltsdateien. |
| FXG-Dateien | Auflösungsunabhängige Grafikformatdateien, mit deren Hilfe Sie anpassbare Vorlagen für die Ausgabe auf Druckern, im Web, als E-Mail, auf einem Desktop und auf anderen Geräten erstellen können. |
| SVG-Dateien | Skalierbare Vektorgrafikdateien, die vom Image-Serving-Server gerendert werden können. |
| XML-Dateien | Dateien, die Vorverarbeitungsregeln zum Verändern der Pfad- und Abfrageabschnitte von Anforderungen festlegen. |
| Cascading Stylesheet-Dateien | Laden Sie CSS-Skins zur Anpassung von HTML5-Viewern hoch. |
| JavaScript-Dateien | JavaScript-Dateien werden für die Viewer-Instrumentierung verwendet, um Kontoinformationen zu speichern. Adobe Security empfiehlt diesen Asset-Typ nur für Client-Konten, die eine separate Domäne für die Bereitstellung verwenden (um Site-übergreifendes Scripting zu vermeiden). |

>[!NOTE]
>
>Wenn Sie Bilddateien und PDF in Adobe Dynamic Media Classic hochladen, konvertiert das System diese Quelldateien in P-TIFF-Dateien (Pyramid TIFF). Diese P-TIFF sind die Dateien, die später auf Dynamic Media-Image-Servern veröffentlicht werden. Adobe Dynamic Media Classic verwendet das Pyramid Tiff-Dateiformat, da es verschiedene Zoomverhältnisse enthält, die eine schnelle Zoomfunktion bei der Anzeige mit einem Adobe Dynamic Media Classic-Zoom-Viewer ermöglichen.

### Unterstützte statische Dateiformate {#supported-static-file-formats}

Adobe Dynamic Media Classic unterstützt mehrere statische Dateiformate. Statischer Inhalt ist ein Asset, das unverändert veröffentlicht wird, z. B. CSS, PDF, SVG und XML.

Die folgenden Dateitypen können veröffentlicht werden:

* Animiertes GIF
* Audiodateien
* CSS
* JavaScript (wenn das Unternehmen mit einer eigenen Domäne konfiguriert wurde)
* Primäres Video
* PDF (wenn PDF nach dem Hochladen zur Veröffentlichung markiert ist, um die Bereitstellung aller PDF für den bestehenden E-Katalog-/PDF-Workflow zu vermeiden)
* PrX-Video
* SVG
* XML
* ZIP

Adobe Dynamic Media Classic bietet keine Option zum Generieren einer Vorschau-URL für statischen Inhalt.

### Dateinamenanforderungen {#filename-requirements}

Da beim Hochladen die Erweiterungen aus den Dateinamen entfernt werden, sind Dateien mit demselben Stammnamen nicht zulässig. Im Adobe Dynamic Media Classic-System wird der Asset-Dateiname abzüglich der Dateinamenerweiterung zur Asset-ID für das Asset. Deshalb muss jedes Asset einen eindeutigen Namen haben.

Stellen Sie sicher, dass alle Benutzer in Ihrem Unternehmen die folgenden Regeln für die Benennung von Dateien verstehen:

* Asset-IDs mit demselben Namen sind im System nicht zulässig.
* Bei Asset-ID-Namen wird zwischen Groß- und Kleinschreibung unterschieden.
* Asset-IDs sollten keine Leerzeichen enthalten (z. B. nicht „Schwarze Jacke.tif“ oder „Blaue Jacke.jpg“). Adobe Dynamic Media Classic ASCII-kodiert leere Leerzeichen in Asset-Namen, wenn es Asset-Namen verwendet, um URL-Zeichenfolgen zu erstellen. Diese ASCII-Codierung beeinträchtigt jedoch die Lesbarkeit der URLs.
* Sprachspezifische Zeichen sind in Dateinamen zulässig. Allerdings dürfen Dateinamen die folgenden Zeichen nicht enthalten:

  `\ ; / ? : @ & = + $ , &#42; " &lt; > | ' { } %`

  Wenn ein Dateiname eines oder mehrere der oben aufgeführten Zeichen enthält, werden die Zeichen beim Hochladen aus dem Dateinamen entfernt.

Normalerweise kann ein Asset-Dateiname mit der Artikelnummer, Produkt-SKU oder einem anderen Namen wie im Folgenden übereinstimmen:

| Element | Dateiname | Asset-ID |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Ordnerorganisation und -struktur {#folder-organization-and-structure}

Organisieren und strukturieren Sie Ordner und Unterordner für Ihre Inhalte in Adobe Dynamic Media Classic, bevor Sie Ihre Inhalte in das System hochladen. Eine solche Vorausplanung hat die folgenden zwei wichtigen Vorteile:

* Wenn Sie Ihre Inhalte über FTP in Adobe Dynamic Media Classic hochladen, können Sie das System anweisen, Ihre Ordnerstruktur während des Uploads zu replizieren. Auf diese Weise werden Ihre Inhalte in denselben Ordnern und Unterordnern wie auf Ihrem Computer oder im Netzwerk in Adobe Dynamic Media Classic organisiert. (Um Ihre Ordnerstruktur in Adobe Dynamic Media Classic zu replizieren, wählen Sie beim Hochladen von Assets über FTP die Option Unterordner einschließen aus.)
* Es ist sehr viel schwieriger, Ordner nach dem Hochladen der Dateien innerhalb des Systems neu zu organisieren, als vorab eine sorgfältig vorbereitete Ordnerstruktur zu erstellen.

Der Ansatz und die Struktur der Ordnerbenennung, die Sie zum Speichern Ihrer Inhalte in der Adobe Dynamic Media Classic wählen, hängt von den Anforderungen Ihres Unternehmens ab. Es folgen einige Beispiele für Ordnerstrukturen:

**SKU-basiert**: Ordner werden gemäß SKUs oder Artikelnummern benannt. Beispielsweise werden separate Ordner für alle Reihen mit 0, 20 und 30 Nummern erstellt.

**Markenbasiert**: Für Hersteller mit mehreren Markenlinien und Einzelhändler, die andere Marken anderer Unternehmen vermarkten, trennen Sie Dateien in Produktordner, die nach verschiedenen Marken benannt sind.

**Projektbasiert**: Ordner sind nach Rollout-/Ablagedatum oder Projektname organisiert. Kunden, die hauptsächlich E-Kataloge erstellen, bevorzugen diese Vorgehensweise.

**Mirror der Ordnerhierarchie der Website**: Diese Ordnerstruktur spiegelt die Ordnerstruktur der Website wider, wobei die Ordner beispielsweise für Produktkategorien benannt sind.

## Über das Hochladen von Dateien {#uploading-your-files}

Sie können einzelne Dateien vom Desktop hochladen oder Ordner über FTP hochladen. Wenn Sie mehr als 100 MB Dateien hochladen oder ganze Ordner und Unterordner hochladen möchten, wählen Sie die Registerkarte **VIA FTP** aus.

Adobe Dynamic Media Classic sendet Ihnen eine E-Mail-Nachricht, um zu bestätigen, wann Ihr Upload-Auftrag beginnt und endet, und Sie über etwaige Probleme zu informieren.

Während (oder unmittelbar danach) eines großen Upload-Auftrags konnten einige neue Elemente die Meldung &quot;Bild noch nicht optimiert&quot;anzeigen. Diese Meldung wird angezeigt, da die Dateien noch nicht vollständig verarbeitet und zu Adobe Dynamic Media Classic hinzugefügt wurden. Sie können die betroffenen Dateien später optimieren. Siehe [Dateien optimieren](application-setup.md#optimize_files).

### Hochladen von Dateien über die Registerkarte Von Desktop {#upload-files-using-sps-desktop-application}

Mit dem Adobe Dynamic Media Classic Desktop-Programm können Sie Dateien und Ordner durch Ziehen hochladen.

1. Wählen Sie in der Adobe Dynamic Media Classic Desktop-Applikation in der Leiste &quot;Globale Navigation&quot;die Option **[!UICONTROL Upload]** aus.
1. Wählen Sie auf der Seite Hochladen die Registerkarte **[!UICONTROL From Desktop]** aus.
1. Wählen Sie auf der linken Seite der Seite &quot;Hochladen&quot;im Bereich **[!UICONTROL Dateien zum Hochladen auswählen]** die Option **[!UICONTROL Durchsuchen]** aus, um die Dateien oder Ordner auszuwählen, die Sie hochladen möchten, und wählen Sie dann **[!UICONTROL Öffnen]**.
1. Navigieren Sie rechts auf der Seite &quot;Hochladen&quot;im ausgewählten Bereich **Ordnerziel** zu einem Zielordner, in dem die hochgeladenen Dateien oder Ordner hinzugefügt werden sollen.
1. (Optional) Geben Sie unten auf der Seite &quot;Hochladen&quot;im Textfeld &quot;Auftragsname&quot;den neuen Namen des Upload-Auftrags ein. Oder Sie können einfach den standardmäßigen, systemgenerierten Namen verwenden, den Adobe Dynamic Media Classic bereitstellt. Upload- und Veröffentlichungsaufträge werden auf der Seite &quot;Aufträge&quot;aufgezeichnet, auf der Sie den Status von Aufträgen überprüfen können. Siehe [Überprüfen von Auftragsdateien](checking-job-files.md#checking_job_files).
1. (Optional) Wählen Sie unten auf der Seite &quot;Hochladen&quot;die Option **[!UICONTROL Publish nach dem Hochladen]** aus, damit Sie die hochgeladenen Assets automatisch veröffentlichen können.
Wenn Sie Dateien veröffentlichen, werden die Dateien an Live-Server gesendet. Die URLs für diese Dateien können dann auf externen Websites und in externen Anwendungen verwendet werden. Diese Option ist auch im Dialogfeld &quot;Auftragsoptionen&quot;verfügbar.
1. (Optional) Wählen Sie unten auf der Seite &quot;Hochladen&quot;die Option &quot;**[!UICONTROL Überschreiben in einem beliebigen Ordner, gleichnamiger Asset-Name unabhängig von der Erweiterung&quot;]**&quot;, wenn Sie möchten, dass die hochgeladenen Dateien bestehende Dateien mit denselben Namen ersetzen. Diese Option ist auch im Dialogfeld &quot;Auftragsoptionen&quot;verfügbar.
Der Name dieser Option kann je nach den Einstellungen unter **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Einstellungen]** > **[!UICONTROL Auf Anwendung hochladen]** > **[!UICONTROL Bilder überschreiben]** unterschiedlich sein.
1. Wählen Sie in der rechten unteren Ecke der Seite &quot;Hochladen&quot;die Option **[!UICONTROL Auftragsoptionen]** und geben Sie dann die gewünschten Optionen an.

   Siehe [Optionen für das Hochladen](uploading-files.md#upload_options).

1. Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL Speichern]**.
1. Wählen Sie in der rechten unteren Ecke der Seite &quot;Hochladen&quot;die Option **[!UICONTROL Upload starten]**.
Um den Upload-Fortschritt anzuzeigen, wählen Sie in der Leiste &quot;Globale Navigation&quot;die Option **[!UICONTROL Aufträge]** aus. Sie können die Arbeit in Adobe Dynamic Media Classic fortsetzen. Kehren Sie jederzeit zur Seite &quot;Aufträge&quot;zurück, um einen laufenden Auftrag zu überprüfen. Wenn Sie einen in Verarbeitung befindlichen Upload-Auftrag stornieren möchten, klicken Sie auf die Schaltfläche **[!UICONTROL Abbrechen]** neben der Angabe „Dauer“.

### Hochladen von Dateien über die Registerkarte &quot;VIA FTP&quot; {#upload-files-using-via-ftp}

1. Melden Sie sich bei der FTP-Site für Adobe Dynamic Media Classic an, die speziell für Ihre Region gilt. Melden Sie sich mit dem von Ihrem Administrator erhaltenen FTP-Benutzernamen und -Kennwort an.
1. Wählen Sie in Adobe Dynamic Media Classic in der Leiste &quot;Globale Navigation&quot;die Option **[!UICONTROL Upload]** aus.
1. Wählen Sie auf der Seite Hochladen die Registerkarte **[!UICONTROL VIA FTP]** aus.
1. Wählen Sie auf der linken Seite der Seite &quot;Hochladen&quot;im Bereich **[!UICONTROL FTP-Ordner zum Hochladen auswählen]** einen FTP-Ordner aus, aus dem Sie Dateien hochladen möchten.
1. Wählen Sie rechts auf der Seite &quot;Hochladen&quot;im ausgewählten Bereich **[!UICONTROL Adobe Dynamic Media Folder Destination]** einen Zielordner in Adobe Dynamic Media Classic aus.
1. (Optional) Geben Sie unten auf der Seite &quot;Hochladen&quot;im Textfeld &quot;Auftragsname&quot;den neuen Namen des Upload-Auftrags ein. Oder Sie können einfach den standardmäßigen, systemgenerierten Namen verwenden, den Adobe Dynamic Media Classic bereitstellt. Upload- und Veröffentlichungsaufträge werden auf der Seite &quot;Aufträge&quot;aufgezeichnet, auf der Sie den Status von Aufträgen überprüfen können.
Siehe [Überprüfen von Auftragsdateien](checking-job-files.md#checking_job_files).
1. (Optional) Wählen Sie unten auf der Seite &quot;Hochladen&quot;die Option **[!UICONTROL Publish nach dem Hochladen]** aus, damit Sie die hochgeladenen Assets automatisch veröffentlichen können.
Wenn Sie Dateien veröffentlichen, werden die Dateien an Live-Server gesendet. Die URLs für diese Dateien können dann auf externen Websites und in externen Anwendungen verwendet werden. Diese Option ist auch im Dialogfeld &quot;Auftragsoptionen&quot;verfügbar.
1. (Optional) Wählen Sie unten auf der Seite &quot;Hochladen&quot;die Option &quot;**[!UICONTROL Überschreiben in einem beliebigen Ordner, gleichnamiger Asset-Name unabhängig von der Erweiterung&quot;]**&quot;, wenn Sie möchten, dass die hochgeladenen Dateien bestehende Dateien mit denselben Namen ersetzen. Diese Option ist auch im Dialogfeld &quot;Auftragsoptionen&quot;verfügbar.
Der Name dieser Option kann je nach den Einstellungen unter **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Einstellungen]** > **[!UICONTROL Auf Anwendung hochladen]** > **[!UICONTROL Bilder überschreiben]** unterschiedlich sein.
1. Optional; nur verfügbar, wenn Sie die Registerkarte **[!UICONTROL VIA FTP]** ausgewählt haben. Wählen Sie unten auf der Seite &quot;Hochladen&quot;die Option **[!UICONTROL Komprimierung der ZIP- oder TAR-Dateien beim Hochladen aufheben]** , damit Sie automatisch alle Dateien aus Ihrer hochgeladenen ZIP- oder TAR-Datei extrahieren können. Diese Option ist auch im Dialogfeld &quot;Auftragsoptionen&quot;verfügbar.
1. Wählen Sie in der rechten unteren Ecke der Seite &quot;Hochladen&quot;die Option **[!UICONTROL Auftragsoptionen]** und geben Sie dann die gewünschten Optionen an.

   Siehe [Optionen für das Hochladen](uploading-files.md#upload_options).

1. Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL Speichern]**.
1. Wählen Sie in der rechten unteren Ecke der Seite &quot;Hochladen&quot;die Option **[!UICONTROL Upload starten]**.

   Um den Upload-Fortschritt anzuzeigen, wählen Sie in der Leiste &quot;Globale Navigation&quot;die Option **[!UICONTROL Aufträge]** aus. Die Seite „Aufträge“ wird eingeblendet. Sie sehen darin den Fortschritt des Hochladevorgangs. Sie können die Arbeit in Adobe Dynamic Media Classic fortsetzen. Kehren Sie jederzeit zur Seite &quot;Aufträge&quot;zurück, um einen laufenden Auftrag zu überprüfen.

Wenn Sie einen in Verarbeitung befindlichen Upload-Auftrag stornieren möchten, klicken Sie auf die Schaltfläche **[!UICONTROL Abbrechen]** neben der Angabe „Dauer“.

## Dialogfeld &quot;Upload-Auftragsoptionen&quot; {#upload-options}

Beim Hochladen von Dateien können Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;eine der folgenden Optionen auswählen:

* **JOB**: Wählen Sie **[!UICONTROL JOB]** aus, um Optionen auszuwählen, die sich auf den gesamten Upload-Auftrag auswirken.

  Sie können auch die Optionen *default* für Upload-Aufträge über das Dialogfeld **[!UICONTROL Standard-Upload-Optionen]** in den allgemeinen Einstellungen auswählen. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Einstellungen]** > **[!UICONTROL Standard-Upload-Optionen]** und legen Sie dann die gewünschten Standardoptionen fest.

   * **[!UICONTROL When]**: Diese Option ist nur verfügbar, wenn Sie die Registerkarte **[!UICONTROL VIA FTP]** ausgewählt haben.
      * **[!UICONTROL Einmalig]**: Geben Sie einen Upload-Auftrag an, der einmal ausgeführt wird. Zu den Optionen gehören:
         * **[!UICONTROL Jetzt]**: Führt den Upload-Auftrag unmittelbar aus, nachdem Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL Speichern]** ausgewählt und auf der Seite &quot;Hochladen&quot;die Option **[!UICONTROL Upload durchführen]** ausgewählt haben.
         * **[!UICONTROL Für später einplanen]**: Wählen Sie Jahr, Monat, Tag und Uhrzeit (in Schritten von 15 Minuten) aus, für die der Upload-Auftrag ausgeführt werden soll.
      * **[!UICONTROL Wiederkehrend]**: Geben Sie einen Upload-Auftrag an, der täglich, wöchentlich oder monatlich ausgeführt wird. Oder passen Sie den Upload-Auftrag an Ihre eigenen Spezifikationen an.
         * **[!UICONTROL Täglich]**: Legen Sie die Zeit fest, zu der der Auftrag täglich ausgeführt werden soll. Wenn der Auftrag nur von Montag bis Freitag ausgeführt werden soll, wählen Sie **[!UICONTROL Nur Wochentage]** aus.
         * **[!UICONTROL Wöchentlich]**: Wählen Sie einen bestimmten Wochentag und eine bestimmte Uhrzeit aus, zu der der Auftrag ausgeführt werden soll.
         * **[!UICONTROL Monatlich]**: Wählen Sie einen bestimmten Tag des Monats oder Tages der Woche aus, einschließlich der Startzeit, für die der Auftrag ausgeführt werden soll.
         * **[!UICONTROL Benutzerdefiniert]**: Passen Sie ein Zeitintervall für Upload- oder Veröffentlichungsaufträge an Ihre eigenen Spezifikationen an. Siehe [Erstellen eines benutzerdefinierten Zeitintervalls für Upload- oder Veröffentlichungsaufträge](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).

   * **[!UICONTROL Publish nach dem Hochladen]**: Verfügbar, wenn Sie die Registerkarte **[!UICONTROL VON DESKTOP]** oder die Registerkarte **[!UICONTROL VIA FTP]** ausgewählt haben. Wählen Sie diese Option aus, damit Sie die hochgeladenen Assets automatisch veröffentlichen können. Wenn Sie Dateien veröffentlichen, werden die Dateien an Live-Server gesendet. Die URLs für diese Dateien können dann auf externen Websites und in externen Anwendungen verwendet werden. Diese Option steht auch auf der Seite „Hochladen“ zur Verfügung.

   * **[!UICONTROL In belieb. Ordner Assets mit ident. Namen unabhängig von Erweiterung überschreiben]**: Verfügbar, wenn Sie die Registerkarte **[!UICONTROL VON DESKTOP]** oder die Registerkarte **[!UICONTROL VIA FTP]** ausgewählt haben. Aktivieren Sie diese Option, wenn die hochgeladenen Dateien vorhandene gleichnamige Dateien ersetzen sollen. Diese Option steht auch auf der Seite „Hochladen“ zur Verfügung. Der Name dieser Option kann je nach den Einstellungen unter **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Einstellungen]** > **[!UICONTROL Auf Anwendung hochladen]** > **[!UICONTROL Bilder überschreiben]** unterschiedlich sein.

   * **[!UICONTROL ZIP- oder TAR-Dateien beim Hochladen entpacken]**: Verfügbar, wenn Sie entweder die Registerkarte **[!UICONTROL VON DESKTOP]** oder die Registerkarte **[!UICONTROL VIA FTP]** ausgewählt haben.
Wählen Sie diese Option aus, damit Sie automatisch alle Dateien aus Ihrer hochgeladenen ZIP- oder TAR-Datei extrahieren können. Diese Option ist auch im Dialogfeld &quot;Auftragsoptionen&quot;verfügbar.

   * **[!UICONTROL Unterordner einschließen]**: Nur verfügbar, wenn Sie die Registerkarte **[!UICONTROL VIA FTP]** ausgewählt haben.
Aktivieren Sie diese Option, wenn Sie auch die Unterordner im hochzuladenden Ordner hochladen möchten. Die Namen des Ordners und der von Ihnen hochgeladenen Unterordner werden automatisch in Adobe Dynamic Media Classic eingegeben.

   * **[!UICONTROL Metadatendateien verarbeiten]**: Nur verfügbar, wenn Sie die Registerkarte **[!UICONTROL VIA FTP]** ausgewählt haben. Wählen Sie diese Option aus, wenn Sie eine tabulatorgetrennte oder XML-Datei hochladen möchten, um mehreren Assets Metadaten hinzuzufügen.
Siehe [Importieren von Metadaten (über FTP)](viewing-adding-exporting-metadata.md#import-metadata).

* **Optionen für das Zuschneiden**: Reduzieren Sie automatisch Leerraum-Pixel aus einem Bild. Öffnen Sie das Menü &quot;**[!UICONTROL Zuschneiden]**&quot;, wählen Sie &quot;**[!UICONTROL Manuell]**&quot;und geben Sie die Pixelmessungen in die Textfelder &quot;Oben&quot;, &quot;Rechts&quot;, &quot;Unten&quot;und &quot;Links&quot;ein, um sie von den Seiten abzuschneiden. Sie können auch **[!UICONTROL Zuschneiden]** im Menü &quot;Zuschneiden&quot;auswählen und die folgenden Optionen auswählen:

   * **[!UICONTROL Entfernen basierend auf]**: Wählen Sie aus, ob das Zuschneiden auf Grundlage von Farbe oder Transparenz erfolgen soll:
      * **[!UICONTROL Farbe]**: Wählen Sie die Option &quot;Farbe&quot;. Wählen Sie dann das Menü &quot;Ecke&quot;aus und wählen Sie die Ecke des Bildes mit der Farbe, die der zu beschnittenen Leerraum-Farbe am besten entspricht.
Beschneiden anhand der Farbe: Geben Sie den Wert 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie genau der Farbe entsprechen, die Sie in der Bildecke ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.
      * **[!UICONTROL Transparenz]**: Wählen Sie die Option **[!UICONTROL Transparenz]** aus.
Auf Transparenz basierendes Zuschneiden: Geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie transparent sind. Werte, die näher an 1 liegen, ermöglichen mehr Transparenz.
      * **[!UICONTROL Toleranz]**: Ziehen Sie den Regler, um eine Toleranz von 0 bis 1 anzugeben.

* **Farbprofiloptionen**: Wählen Sie eine Farbkonvertierung, wenn Sie optimierte Dateien erstellen, die für die dynamische Adobe Dynamic Media Classic-Bereitstellung verwendet werden:

   * **[!UICONTROL Beibehaltung der Standardfarbe]**: Behält die Quellbildfarben bei, wenn die Bilder Farbrauminformationen enthalten. Es gibt keine Farbkonvertierung. Heutzutage ist in fast allen Bildern das entsprechende Farbprofil eingebettet. Wenn jedoch ein CMYK-Quellbild kein eingebettetes Farbprofil enthält, werden die Farben in den sRGB-Farbraum (standardmäßiges Rot Grün Blau) umgewandelt. sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Webseiten.
   * **[!UICONTROL Ursprünglichen Farbraum beibehalten]**: Behält die Originalfarben ohne Farbkonvertierung zum Zeitpunkt der Aufnahme in Adobe Dynamic Media Classic bei. Bei Bildern ohne eingebettetes Farbprofil erfolgt die erforderliche Farbkonvertierung zur Verarbeitung von Bildanforderungen mithilfe der Standardfarbprofile, die in den Veröffentlichungseinstellungen konfiguriert sind. Diese Farbprofile stimmen nicht immer mit den Farben in den mit dieser Option erstellten Dateien überein. Deshalb empfehlen wir, die Option „Beibehaltung der Standardfarbe“ zu verwenden.
   * **[!UICONTROL Benutzerdefiniert von]** > **[!UICONTROL bis]**: Öffnet Menüs, damit Sie einen Farbraum **[!UICONTROL Konvertieren von]** und **[!UICONTROL Konvertieren in]** auswählen können. Diese erweiterte Option überschreibt alle Farbinformationen, die in die Quelldatei eingebettet sind. Wählen Sie diese Option nur, wenn alle Bilder, die Sie senden, falsche oder fehlende Farbprofildaten enthalten.

* **Bildbearbeitungsoptionen**: Sie können die Beschneidungs-&lt;> Masken in Bildern beibehalten und ein Farbprofil auswählen.
Siehe [Optionen zur Feinabstimmung von Bildern beim Hochladen](image-editing-options-upload.md#image-editing-options-at-upload).

* **PostScript® options**: Sie können PostScript® rastern, Dateien beschneiden, transparente Hintergründe beibehalten, eine Auflösung wählen und einen Farbraum auswählen.
Siehe [Arbeiten mit PostScript- und Illustrator-Dateien](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Photoshop-Optionen**: Sie können Vorlagen aus Adobe® Photoshop®-Dateien erstellen, Ebenen beibehalten, angeben, wie Ebenen benannt werden, Text extrahieren und festlegen, wie Bilder in Vorlagen verankert werden.
Siehe [Optionen für das Hochladen von PSD-Dateien](psd-files.md#psd_upload_options).

* **PDF options**: Sie können die Dateien rastern, Suchbegriffe und Links extrahieren, automatisch einen E-Katalog erstellen, die Auflösung festlegen und einen Farbraum auswählen.
Siehe [Optionen für das Hochladen von PDF-Dateien](pdfs.md#pdf_upload_options).

* **Illustrator-Optionen**: Sie können Adobe Illustrator®-Dateien rastern, transparente Hintergründe beibehalten, eine Auflösung wählen und einen Farbraum auswählen.
Siehe [Arbeiten mit PostScript- und Illustrator-Dateien](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **EVIDEO-Optionen**: Sie können eine Videodatei umkodieren, indem Sie eine Videovorgabe auswählen.
Siehe [Arbeiten mit Videokodierungsvorgaben](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **Mehr Metadaten**: Geben Sie Schlüsselwörter ein, die die Dateien beschreiben, die Sie hochladen möchten. Trennen Sie Schlüsselwörter mit Kommata. Schlüsselwörter erleichtern die Suche nach Assets.
Siehe [Durchführen einer erweiterten Suche](searching-assets.md#conducting_an_advanced_search).
Siehe auch Schulungsvideo zum [Hochladen von Keywords](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS) .

* **Stapelsatzvorgaben**: Um ein Bildset, Rotationsset oder Musterset aus den hochgeladenen Dateien zu erstellen, wählen Sie die Spalte **[!UICONTROL Aktiv]** für die Vorgabe aus, die Sie verwenden möchten. Sie können mehrere Vorgaben auswählen. Sie können die Vorgaben auf der Seite &quot;Anwendungseinstellungen&quot;/&quot;Stapelsatzvorgaben&quot;erstellen.
Siehe [Stapelsatzvorgaben](application-setup.md#batch_set_presets).

* **Erweitert**: Siehe [Befolgen Sie einen Upload mit einem anderen Auftrag](uploading-files.md#follow-an-upload-with-another-job).

## Starten eines weiteren Auftrags im Anschluss an einen Upload-Auftrag {#follow-an-upload-with-another-job}

Wenn Sie Elemente per FTP hochladen, können Sie einen nachfolgenden Auftrag planen, der nach Abschluss des Uploads beginnt. Wenn andere Aufträge geplant sind, werden die Aufträge, die Sie hier planen, nach ihnen in die Warteschlange gestellt.

Der neue Auftrag sendet eine Benachrichtigung an die von Ihnen angegebene Adresse, damit der Code an dieser Stelle ausgelöst werden kann. Der nachfolgende Veröffentlichungsauftrag erhält den Namen des Upload-Auftrags mit dem Präfix *Pub_*(für Publikation).

**So folgen Sie einem Upload mit einem anderen Auftrag:**

1. Wählen Sie **[!UICONTROL Upload]** und dann die Registerkarte **[!UICONTROL VIA FTP]** aus.
1. Wählen Sie in der rechten unteren Ecke der Seite &quot;Hochladen&quot;die Option **[!UICONTROL Auftragsoptionen]**.
1. Erweitern Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;den Abschnitt **[!UICONTROL ERWEITERT]** .
1. Wählen Sie aus der Dropdownliste **[!UICONTROL Nach dem Hochladen mit einem anderen Auftrag]** eine der folgenden Optionen aus:

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
   >Regelmäßig geplante Aufträge können manchmal dazu führen, dass keine Dateien veröffentlicht werden.

>[!MORELIKETHIS]
>
>* [Arbeiten mit Asset-Ordnern](asset-folders.md#working_with_asset_folders)
>* [Verarbeiten wiederkehrender Upload- und Veröffentlichungsaufträge](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Verwenden eines Upload- oder Veröffentlichungsauftrags als Trigger](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)
