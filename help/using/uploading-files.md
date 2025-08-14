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
source-git-commit: 1cd516119da23f5ef4c0195273025ddd4b3fa789
workflow-type: tm+mt
source-wordcount: '3858'
ht-degree: 25%

---

# Hochladen von Dateien{#uploading-files}

Stellen Sie vor dem Hochladen von Asset-Dateien in Adobe Dynamic Media Classic sicher, dass die Asset-Dateien korrekt benannt sind. Stellen Sie außerdem sicher, dass Ihre Ordnerstruktur so eingerichtet und organisiert ist, wie Sie möchten. Sie können Dateien von einer von Adobe Dynamic Media Classic bereitgestellten FTP-Site oder direkt von Ihrem Computer oder Netzwerk hochladen. Adobe Dynamic Media Classic bietet Optionen zum Optimieren von Dateien beim Hochladen. Wenn Sie das Adobe Dynamic Media Classic-Desktop-Programm installiert haben, können Sie Dateien und Ordner hochladen, indem Sie sie direkt von Ihrem Desktop ziehen. Siehe [Allgemeine Programmeinstellungen](application-setup.md#general_settings).

## Vorbereiten von Assets und Ordnern für das Hochladen {#preparing-your-assets-and-folders-for-uploading}

Stellen Sie vor dem Hochladen von Assets in Adobe Dynamic Media Classic sicher, dass sie das richtige Format und die richtige Größe aufweisen. Beachten Sie außerdem die Adobe Dynamic Media Classic-Regeln für das Benennen von Assets. Indem Sie eine Ordnerorganisation und -struktur konfigurieren, erleichtern Sie sich das Auffinden von Dateien und die Arbeit mit den Dateien.

### Unterstützte Asset-Dateiformate {#supported-asset-file-formats}

In dieser Tabelle sind die von Adobe Dynamic Media Classic unterstützten Asset-Dateiformate aufgeführt. Informationen zu unterstützten Camera Raw-Dateien finden Sie unter [https://helpx.adobe.com/de/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/de/camera-raw/using/supported-cameras.html).

| Asset-Dateiformate | Beschreibung |
| --- | --- |
| Audio | AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3 |
| Cascading Stylesheet | CSS |
| Farbprofile | ICC, ICM |
| Schriftarten | AFM, OTF, PFB, PFM, PhotoFont, TTC, TTF |
| FXG | FXG |
| Illustrator | KI, FXG |
| Bilder | BMP, FPX, GIF, JPEG, JPG, PNG, PICT (nur Windows®), TIF, TIFF |
| InDesign | INDD, INDT |
| MS® Office | DOC, PPT, RTF, XLS |
| PDF | PDF |
| Photoshop | PSD, FXG und Camera Raw |
| PostScript | EPS, PS |
| Adobe Dynamic Media Classic-Bildbearbeitung | VNC, VNT, VNW |
| SVG | SVG, SVGX |
| TAR | TAR |
| Video | 3GP, AVI, M2P, M2T, M2TS, M2V, M4V, MOV, MP4, MPEG, MPG, MTS, OGV, TS, VOB, WMV/ASF |
| XML | XML |
| ZIP | ZIP |

Die Upload-Unterstützung von ZIP- und TAR-Archiven umfasst ein Kontrollkästchen, mit dem Sie angeben können, ob die Dateien entpackt werden sollen.

### Nicht unterstützte Bildformate in Dynamic Media {#unsupported-image-formats-dynamic-media}

Die folgende Liste beschreibt die Untertypen von Rasterbilddateiformaten, die in Dynamic Media *nicht* unterstützt werden.

* PNG-Dateien mit einer IDAT-Blockgröße größer als 100 MB.
* PSB-Dateien.
* PSD-Dateien mit einem anderen Farbraum als CMYK, RGB, Graustufen oder Bitmap werden nicht unterstützt. DuoTone-, Lab- und indizierte Farbräume werden nicht unterstützt.
* PSD-Dateien mit einer Bittiefe größer als 16.
* TIFF-Dateien mit Gleitkommadaten.
* TIFF-Dateien mit Lab-Farbraum.

### Asset-Typen {#asset-types}

Um mit dem Adobe Dynamic Media Classic-Programm optimale Ergebnisse zu erzielen, sollten Sie die empfohlenen Dateiformate und -größen verwenden. In der folgenden Tabelle sind die empfohlenen Formate und Dateigrößen für häufig verwendete Assets aufgeführt.

| Asset-Typ | Beschreibung/Empfehlungen |
| --- | --- |
| Audio | Zu den Eingabeformaten von Audio-Assets gehören AAC, HE-AAC, AC3, WAV, WMA, AIFF, MP3. Sie können Audio-Daten in die folgenden Formate transcodieren: MP3, AAC und HE-AAC. |
| Bilder (für Bildgrößenänderungen, Zoom, Bildsätze, Rotationssets) | Die längste Bildgröße muss mindestens 2.000 Pixel betragen. Typische Bildgrößen liegen zwischen 1.500 und 2.500 Pixel in der längsten Größe. Verlustfreie Bildformate, z. B. TIFF und PNG, sind zu empfehlen. Bei Verwendung eines JPEG-Bildes sollten Sie die höchste Qualitätseinstellung wählen. Animierte GIF-Dateien werden wie andere statische Inhalte verarbeitet. |
| E-Kataloge | Verwenden Sie hochauflösende PDF-Dateien, die in Adobe Acrobat oder einer Adobe Creative Suite-Anwendung erstellt wurden und als „druckbereit“ gespeichert wurden. PDFs enthalten alle benötigten Schriftarten, Bilder, Masken. Alle referenzierten grafischen Elemente sind enthalten, entweder als Einzelseiten, doppelseitige Doppelseiten oder in einem mehrseitigen Format. Sortieren Sie die Seiten, indem Sie die Dateien in alphanumerischer Reihenfolge benennen. Platzieren Sie alle PDF-Dateien für einen E-Katalog in einem einzigen Ordner, um das Hochladen zu vereinfachen. Beim Hochladen können Sie Schnittoptionen auswählen, um die Zuschneidebereiche, einschließlich Schnittmarken, Passermarken oder Farbkontrollstreifen, aus den PDF-Dateien zu entfernen. Da die meisten druckbereiten PDF-Dateien im CMYK-Farbraum gespeichert werden, ist es wichtig, das für die PDF-Dateien verwendete ICC-Farbprofil für CMYK zu ermitteln und abzurufen. |
| Vorlagen | Bild- oder Layoutentwürfe mit Ebenen können Text, Bilder und Ebenen enthalten. Bildebenen, Textzeichenfolgen und Ebenenattribute wie Farbe und Größe können parametrisiert werden, sodass variable Daten angepasst werden können. Die Anforderungen für in Vorlagen verwendete Bilder sind dieselben wie für andere Bilder. Bereiten Sie Grafiken in Photoshop oder einem anderen Bildbearbeitungsprogramm vor. Speichern Sie jede Grafik einzeln als reduzierte, transparente Datei im TIFF- oder PNG-Format. Stellen Sie sicher, dass die Bildauflösung für den beabsichtigten Verwendungszweck geeignet ist. Bilder für den Druck sind 300 ppi. |
| Videos | Adobe Dynamic Media Classic unterstützt Videodateien im OGV- und MP4-Format. Dateien können beim Hochladen in das MP4-Format transkodiert werden. Siehe [Unterstützte Asset-Dateiformate](#supported-static-file-formats). |
| Schriftarten | Hochgeladene TrueType-, `Type1`- (nur Windows®), OpenType®-Schriftarten und FotoFonts. |
| Bilder | Bilder und Bilddateien mit mehreren Ebenen. |
| Bildsätze und Mustersets | Sammlungen zusammengehöriger Bilder, die in einem Viewer angezeigt werden können. |
| ICC-Profile | Ein Farbprofil, mit dem Sie ein hochgeladenes Bild aus dem Quellfarbraum in einen anderen Farbraum konvertieren können. |
| Vignetten | Mit dem Bildbearbeitungsprogramm erstellte Bilder und zugehörige Dateien. |
| Inhaltsdateien | Adobe InDesign-, Illustrator- oder Photoshop-Inhaltsdateien. |
| FXG-Dateien | Auflösungsunabhängige Grafikformatdateien, mit deren Hilfe Sie anpassbare Vorlagen für die Ausgabe auf Druckern, im Web, als E-Mail, auf einem Desktop und auf anderen Geräten erstellen können. |
| SVG-Dateien | Skalierbare Vektorgrafikdateien, die vom Image-Serving-Server gerendert werden können. |
| XML-Dateien | Dateien, die Vorverarbeitungsregeln zum Verändern der Pfad- und Abfrageabschnitte von Anforderungen festlegen. |
| Cascading Stylesheet-Dateien | Hochladen von CSS-Skins zur Anpassung der HTML5-Viewer. |
| JavaScript-Dateien | JavaScript-Dateien werden für die Viewer-Instrumentierung zum Speichern von Kontoinformationen verwendet. Adobe Security empfiehlt diesen Asset-Typ nur für Client-Konten, die über eine separate Domain für die Bereitstellung verfügen (um Cross-Site-Scripting zu vermeiden). |

>[!NOTE]
>
>Wenn Sie Bilddateien und PDFs in Adobe Dynamic Media Classic hochladen, konvertiert das System diese Quelldateien in P-TIFF-Dateien (Pyramid TIFF). Diese P-TIFFs sind die Dateien, die später auf Dynamic Media-Bildservern veröffentlicht werden. Adobe Dynamic Media Classic verwendet das Pyramid TIFF-Dateiformat, da es verschiedene Zoomverhältnisse enthält, die ein schnelles Zoomen ermöglichen, wenn Sie es mit einem Adobe Dynamic Media Classic-Zoom-Viewer anzeigen.

### Unterstützte statische Dateiformate {#supported-static-file-formats}

Adobe Dynamic Media Classic unterstützt mehrere statische Dateiformate. Statische Inhalte sind alle Assets, die im Istzustand veröffentlicht werden, z. B. CSS, PDF, SVG und XML.

Die folgenden Dateitypen können veröffentlicht werden:

* Animiertes GIF
* Audiodateien
* CSS
* JavaScript (wenn das Unternehmen mit einer eigenen Domäne konfiguriert wurde)
* Primäres Video
* PDF (wenn PDF nach dem Hochladen zur Veröffentlichung markiert ist, um die Bereitstellung aller PDFs für bestehenden E-Katalog/PDF-Workflow zu vermeiden)
* PrX-Video
* SVG
* XML
* ZIP

Adobe Dynamic Media Classic bietet keine Option zum Generieren einer Vorschau-URL mit statischem Inhalt.

### Dateinamenanforderungen {#filename-requirements}

Da beim Hochladen die Erweiterungen aus den Dateinamen entfernt werden, sind Dateien mit demselben Stammnamen nicht zulässig. Im Adobe Dynamic Media Classic-System wird der Asset-Dateiname abzüglich der Dateinamenerweiterung zur Asset-ID für das Asset. Deshalb muss jedes Asset einen eindeutigen Namen haben.

Stellen Sie sicher, dass alle Benutzer in Ihrem Unternehmen diese Regeln für die Benennung von Dateien verstehen:

* Asset-IDs mit demselben Namen sind im System nicht zulässig.
* Bei Asset-ID-Namen wird zwischen Groß- und Kleinschreibung unterschieden.
* Asset-IDs sollten keine Leerzeichen enthalten (z. B. nicht „Schwarze Jacke.tif“ oder „Blaue Jacke.jpg“). Adobe Dynamic Media Classic ASCII kodiert Leerzeichen in Asset-Namen, wenn es Asset-Namen zum Erstellen von URL-Zeichenfolgen verwendet. Diese ASCII-Codierung beeinträchtigt jedoch die Lesbarkeit der URLs.
* Sprachspezifische Zeichen sind in Dateinamen zulässig. Allerdings dürfen Dateinamen die folgenden Zeichen nicht enthalten:

  `\ ; / ? : @ & = + $ , &#42; " &lt; > | ' { } %`

  Wenn ein Dateiname eines oder mehrere der oben aufgeführten Zeichen enthält, werden die Zeichen beim Hochladen aus dem Dateinamen entfernt.

Normalerweise kann der Name einer Asset-Datei mit der Artikelnummer, der Produkt-SKU oder einem anderen Namen übereinstimmen wie in den folgenden:

| Element | Dateiname | Asset-ID |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### Ordnerorganisation und -struktur {#folder-organization-and-structure}

Organisieren und strukturieren Sie Ordner und Unterordner für Ihre Inhalte in Adobe Dynamic Media Classic, bevor Sie Ihre Inhalte in das System hochladen. Eine solche Vorausplanung hat die folgenden zwei wichtigen Vorteile:

* Wenn Sie Ihre Inhalte über FTP in Adobe Dynamic Media Classic hochladen, können Sie das System anweisen, Ihre Ordnerstruktur beim Hochladen zu replizieren. Auf diese Weise sind Ihre Inhalte in Adobe Dynamic Media Classic in denselben Ordnern und Unterordnern organisiert wie auf Ihrem Computer oder Netzwerk. (Um Ihre Ordnerstruktur in Adobe Dynamic Media Classic zu replizieren, wählen Sie beim Hochladen von Assets über FTP die Option Unterordner einschließen aus.)
* Es ist sehr viel schwieriger, Ordner nach dem Hochladen der Dateien innerhalb des Systems neu zu organisieren, als vorab eine sorgfältig vorbereitete Ordnerstruktur zu erstellen.

Der Ansatz und die Struktur der Ordnerbenennung, die Sie für die Speicherung Ihrer Inhalte auf der Adobe Dynamic Media Classic auswählen, hängen von den Anforderungen Ihres Unternehmens ab. Es folgen einige Beispiele für Ordnerstrukturen:

**SKU-basiert**: Ordner werden nach SKUs oder Artikelnummern benannt. Beispielsweise werden separate Ordner für alle 0-, 20- und 30-Zahlenreihen erstellt.

**Markenbasiert**: Für Hersteller mit mehreren Markenlinien und Einzelhändler, die andere Marken anderer Unternehmen vermarkten, trennen Sie die Dateien in Produktordnern, die für verschiedene Marken benannt sind.

**Projektbasiert**: Ordner sind nach Rollout-/Ablagedatum oder Projektname organisiert. Kunden, die hauptsächlich E-Kataloge erstellen, bevorzugen diese Vorgehensweise.

**Spiegelung der Ordnerhierarchie der Website**: Diese Ordnerstruktur spiegelt die Ordnerstruktur der Website wider, wobei die Ordner z. B. für Produktkategorien benannt sind.

## Informationen zum Hochladen von Dateien {#uploading-your-files}

Sie können einzelne Dateien vom Desktop hochladen oder Ordner per FTP hochladen. Wenn Sie mehr als 100 MB Dateien oder ganze Ordner und Unterordner hochladen möchten, wählen Sie die Registerkarte **VIA FTP** aus.

Adobe Dynamic Media Classic sendet Ihnen eine E-Mail-Nachricht, um zu bestätigen, wann Ihr Upload-Auftrag beginnt und endet, und um Sie über Probleme zu informieren.

Während (oder unmittelbar nach) einem großen Upload-Auftrag konnten einige neue Elemente die Meldung „Bild noch nicht optimiert“ anzeigen. Diese Meldung wird angezeigt, da die Dateien noch nicht vollständig verarbeitet und zu Adobe Dynamic Media Classic hinzugefügt wurden. Sie können die betroffenen Dateien später optimieren. Siehe [Dateien optimieren](application-setup.md#optimize_files).

### Hochladen von Dateien über die Registerkarte „Von Desktop“ {#upload-files-using-sps-desktop-application}

Mit dem Adobe Dynamic Media Classic-Desktop-Programm können Sie Dateien und Ordner per Drag-and-Drop hochladen.

1. Wählen Sie im Adobe Dynamic Media Classic-Desktop-Programm in der Leiste Globale Navigation die Option **[!UICONTROL Hochladen]** aus.
1. Wählen Sie auf der Seite Hochladen die Registerkarte **[!UICONTROL Von Desktop]** aus.
1. Wählen Sie links auf der Seite Hochladen im Bereich **[!UICONTROL Dateien zum Hochladen auswählen]** die Option **[!UICONTROL Durchsuchen]** aus, um die Dateien oder Ordner auszuwählen, die Sie hochladen möchten, und klicken Sie dann auf **[!UICONTROL Öffnen]**.
1. Navigieren Sie rechts auf der Seite Hochladen im ausgewählten Bereich **Ordnerziel** zu einem Zielordner, zu dem Sie die hochgeladenen Dateien oder Ordner hinzufügen möchten.
1. (Optional) Geben Sie unten auf der Seite Hochladen im Textfeld Auftragsname den neuen Namen des Upload-Auftrags ein. Sie können auch einfach den von Adobe Dynamic Media Classic bereitgestellten systemgenerierten Standardnamen verwenden. Upload- und Veröffentlichungsaufträge werden auf der Seite „Aufträge“ aufgezeichnet, wo Sie den Status der Aufträge prüfen können. Siehe [Überprüfen von Auftragsdateien](checking-job-files.md#checking_job_files).
1. (Optional) Klicken Sie unten auf der Seite „Hochladen“ auf **[!UICONTROL Nach dem Hochladen veröffentlichen]** damit Sie die hochgeladenen Assets automatisch veröffentlichen können.
Wenn Sie Dateien veröffentlichen, werden die Dateien an Live-Server gesendet. Die URLs für diese Dateien können dann auf externen Websites und in externen Anwendungen verwendet werden. Diese Option ist auch im Dialogfeld Auftragsoptionen verfügbar.
1. (Optional) Wählen Sie unten auf der Seite Hochladen die Option **[!UICONTROL In belieb. Ordner Assets mit ident. Namen unabh. von Erweit. überschreiben]** aus, wenn die hochgeladenen Dateien vorhandene Dateien durch ident. Namen ersetzen sollen. Diese Option ist auch im Dialogfeld Auftragsoptionen verfügbar.
Der Name dieser Option kann je nach den Einstellungen unter **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Einstellungen]** > **[!UICONTROL In Anwendung hochladen]** > **[!UICONTROL Bilder überschreiben]** unterschiedlich sein.
1. Wählen Sie in der rechten unteren Ecke der Seite „Hochladen **[!UICONTROL die Option]** Auftragsoptionen“ aus und geben Sie dann die gewünschten Optionen an.

   Siehe [Optionen für das Hochladen](uploading-files.md#upload_options).

1. Wählen Sie im Dialogfeld Upload-Auftragsoptionen die Option **[!UICONTROL Speichern]**.
1. Wählen Sie in der rechten unteren Ecke der Seite „Hochladen“ **[!UICONTROL Upload starten]**.
Um den Fortschritt des Uploads anzuzeigen, wählen Sie **[!UICONTROL Vorgänge]** in der globalen Navigationsleiste aus. Sie können weiterhin in Adobe Dynamic Media Classic arbeiten. Kehren Sie jederzeit zur Seite „Aufträge“ zurück, um einen gerade verarbeiteten Auftrag zu überprüfen. Wenn Sie einen in Verarbeitung befindlichen Upload-Auftrag stornieren möchten, klicken Sie auf die Schaltfläche **[!UICONTROL Abbrechen]** neben der Angabe „Dauer“.

### Hochladen von Dateien über die Registerkarte VIA FTP {#upload-files-using-via-ftp}

1. Melden Sie sich bei der für Ihre Region spezifischen Adobe Dynamic Media Classic-FTP-Site an. Melden Sie sich mit dem von Ihrem Administrator erhaltenen FTP-Benutzernamen und -Kennwort an.
1. Wählen Sie in Adobe Dynamic Media Classic in der Symbolleiste für globale Navigation **[!UICONTROL Hochladen]** aus.
1. Wählen Sie auf der Seite Hochladen die Registerkarte **[!UICONTROL VIA FTP]** aus.
1. Wählen Sie links auf der Seite Hochladen im Bereich **[!UICONTROL FTP-Ordner für Upload auswählen]** einen FTP-Ordner aus, aus dem Dateien hochgeladen werden sollen.
1. Wählen Sie rechts auf der Seite Hochladen im Bereich **[!UICONTROL Ziel für Adobe Dynamic Media-Ordner]** einen Zielordner in Adobe Dynamic Media Classic aus.
1. (Optional) Geben Sie unten auf der Seite Hochladen im Textfeld Auftragsname den neuen Namen des Upload-Auftrags ein. Sie können auch einfach den von Adobe Dynamic Media Classic bereitgestellten systemgenerierten Standardnamen verwenden. Upload- und Veröffentlichungsaufträge werden auf der Seite „Aufträge“ aufgezeichnet, wo Sie den Status der Aufträge prüfen können.
Siehe [Überprüfen von Auftragsdateien](checking-job-files.md#checking_job_files).
1. (Optional) Klicken Sie unten auf der Seite „Hochladen“ auf **[!UICONTROL Nach dem Hochladen veröffentlichen]** damit Sie die hochgeladenen Assets automatisch veröffentlichen können.
Wenn Sie Dateien veröffentlichen, werden die Dateien an Live-Server gesendet. Die URLs für diese Dateien können dann auf externen Websites und in externen Anwendungen verwendet werden. Diese Option ist auch im Dialogfeld Auftragsoptionen verfügbar.
1. (Optional) Wählen Sie unten auf der Seite Hochladen die Option **[!UICONTROL In belieb. Ordner Assets mit ident. Namen unabh. von Erweit. überschreiben]** aus, wenn die hochgeladenen Dateien vorhandene Dateien durch ident. Namen ersetzen sollen. Diese Option ist auch im Dialogfeld Auftragsoptionen verfügbar.
Der Name dieser Option kann je nach den Einstellungen unter **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Einstellungen]** > **[!UICONTROL In Programm hochladen]** > **[!UICONTROL Bilder überschreiben]** unterschiedlich sein.
1. Optional, nur verfügbar, wenn Sie die Registerkarte **[!UICONTROL VIA FTP]** ausgewählt haben. Wählen Sie unten auf der Seite Hochladen die Option **[!UICONTROL Zip- oder TAR-Dateien beim Hochladen entpacken]** aus, damit Sie automatisch alle Dateien aus Ihrer hochgeladenen ZIP- oder TAR-Datei extrahieren können. Diese Option ist auch im Dialogfeld Auftragsoptionen verfügbar.
1. Wählen Sie in der rechten unteren Ecke der Seite „Hochladen **[!UICONTROL die Option]** Auftragsoptionen“ aus und geben Sie dann die gewünschten Optionen an.

   Siehe [Optionen für das Hochladen](uploading-files.md#upload_options).

1. Wählen Sie im Dialogfeld Upload-Auftragsoptionen die Option **[!UICONTROL Speichern]**.
1. Wählen Sie in der rechten unteren Ecke der Seite „Hochladen“ **[!UICONTROL Upload starten]**.

   Um den Fortschritt des Uploads anzuzeigen, wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Aufträge]** aus. Die Seite „Aufträge“ wird eingeblendet. Sie sehen darin den Fortschritt des Hochladevorgangs. Sie können weiterhin in Adobe Dynamic Media Classic arbeiten. Kehren Sie jederzeit zur Seite „Aufträge“ zurück, um einen gerade verarbeiteten Auftrag zu überprüfen.

Wenn Sie einen in Verarbeitung befindlichen Upload-Auftrag stornieren möchten, klicken Sie auf die Schaltfläche **[!UICONTROL Abbrechen]** neben der Angabe „Dauer“.

## Dialogfeld „Upload-Auftragsoptionen“ {#upload-options}

Beim Hochladen von Dateien können Sie im Dialogfeld Upload-Auftragsoptionen aus den folgenden Optionen auswählen:

* **AUFTRAG**: Wählen Sie **[!UICONTROL AUFTRAG]** aus, um Optionen auszuwählen, die sich auf den gesamten Upload-Auftrag auswirken.

  Sie können die *Standard*-Optionen für das Hochladen von Aufträgen auch über das Dialogfeld **[!UICONTROL Standardmäßige Upload-Optionen]** in den allgemeinen Einstellungen auswählen. Wechseln Sie **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Einstellungen]** > **[!UICONTROL Standard-Uploadoptionen]** und legen Sie die gewünschten Standardoptionen fest.

   * **[!UICONTROL Wenn]**: Diese Option ist nur verfügbar, wenn Sie die Registerkarte **[!UICONTROL VIA FTP]** ausgewählt haben.
      * **[!UICONTROL Einmalig]**: Geben Sie einen Upload-Auftrag an, der einmal ausgeführt werden soll. Zu den Optionen gehören:
         * **[!UICONTROL Jetzt]**: Führt den Upload-Auftrag sofort aus, nachdem Sie im Dialogfeld Upload-**[!UICONTROL die Option]** Speichern **[!UICONTROL ausgewählt haben, und wählen Sie dann auf der]** „Upload starten“ aus.
         * **[!UICONTROL Für später planen]**: Wählen Sie Jahr, Monat, Tag und Uhrzeit (in Intervallen von 15 Minuten) aus, zu denen der Upload-Auftrag ausgeführt werden soll.
      * **[!UICONTROL Wiederkehrend]**: Geben Sie einen Upload-Auftrag an, der täglich, wöchentlich oder monatlich ausgeführt werden soll. Oder passen Sie den Upload-Auftrag an Ihre eigenen Spezifikationen an.
         * **[!UICONTROL Täglich]**: Legen Sie die Zeit fest, zu der der Auftrag täglich ausgeführt werden soll. Wenn der Vorgang nur von Montag bis Freitag ausgeführt werden soll, wählen Sie **[!UICONTROL Nur Wochentage]** aus.
         * **[!UICONTROL Wöchentlich]**: Wählen Sie einen bestimmten Wochentag und eine Uhrzeit aus, zu der der Auftrag ausgeführt werden soll.
         * **[!UICONTROL Monatlich]** Wählen Sie einen bestimmten Tag des Monats oder Wochentags aus, einschließlich der Startzeit, an der der Auftrag ausgeführt werden soll.
         * **[!UICONTROL Benutzerdefiniert]**: Passen Sie das Zeitintervall für Upload- oder Veröffentlichungsaufträge an Ihre eigenen Spezifikationen an. Siehe [Erstellen eines benutzerdefinierten Zeitintervalls für Uploads oder Veröffentlichungsaufträge](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).

   * **[!UICONTROL Nach Hochladen veröffentlichen]**: Verfügbar, wenn Sie entweder die Registerkarte **[!UICONTROL VON DESKTOP]** oder die Registerkarte **[!UICONTROL ÜBER FTP]** ausgewählt haben. Wählen Sie diese Option aus, damit Sie die hochgeladenen Assets automatisch veröffentlichen können. Wenn Sie Dateien veröffentlichen, werden die Dateien an Live-Server gesendet. Die URLs für diese Dateien können dann auf externen Websites und in externen Anwendungen verwendet werden. Diese Option steht auch auf der Seite „Hochladen“ zur Verfügung.

   * **[!UICONTROL In belieb. Ordner Assets mit ident. Namen unabh. von Erweit. überschreiben]** Verfügbar, wenn **[!UICONTROL die Registerkarte VOM DESKTOP]** oder **[!UICONTROL VIA FTP]** ausgewählt haben. Aktivieren Sie diese Option, wenn die hochgeladenen Dateien vorhandene gleichnamige Dateien ersetzen sollen. Diese Option steht auch auf der Seite „Hochladen“ zur Verfügung. Der Name dieser Option kann je nach den Einstellungen unter **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Einstellungen]** > **[!UICONTROL In Programm hochladen]** > **[!UICONTROL Bilder überschreiben]** unterschiedlich sein.

   * **[!UICONTROL Zip- oder TAR-Dateien beim Hochladen entpacken]**: Verfügbar, wenn Sie entweder die Registerkarte **[!UICONTROL VOM DESKTOP]** oder die Registerkarte **[!UICONTROL VIA FTP]** ausgewählt haben.
Wählen Sie diese Option aus, damit Sie automatisch alle Dateien aus Ihrer hochgeladenen ZIP- oder TAR-Datei extrahieren können. Diese Option ist auch im Dialogfeld Auftragsoptionen verfügbar.

   * **[!UICONTROL Unterordner einbeziehen]**: Nur verfügbar, wenn die Registerkarte **[!UICONTROL VIA FTP]** ausgewählt wurde.
Aktivieren Sie diese Option, wenn Sie auch die Unterordner im hochzuladenden Ordner hochladen möchten. Die Namen des hochgeladenen Ordners und der darin enthaltenen Unterordner werden automatisch in Adobe Dynamic Media Classic eingegeben.

   * **[!UICONTROL Metadatendateien verarbeiten]**: Nur verfügbar, wenn Sie auf der Registerkarte **[!UICONTROL VIA FTP]** ausgewählt haben. Wählen Sie diese Option aus, wenn Sie eine tabulatorgetrennte oder XML-Datei hochladen möchten, um mehreren Assets Metadaten hinzuzufügen.
Siehe [Importieren von Metadaten (über FTP)](viewing-adding-exporting-metadata.md#import-metadata).

* **Zuschnittsoptionen**: Automatische Beschneidung von Leerraumpixeln eines Bildes. Öffnen Sie das Menü **[!UICONTROL Zuschneiden]**, wählen Sie **[!UICONTROL Manuell]** aus und geben Sie zum Zuschneiden von den Seiten Pixelwerte in die Textfelder Oben, Rechts, Unten und Links ein. Sie können auch **[!UICONTROL Zuschneiden]** im Menü „Beschneiden“ auswählen und die folgenden Optionen auswählen:

   * **[!UICONTROL Beschneiden basierend auf]**: Wählen Sie, ob der Beschneidungsprozess auf Grundlage von Farbe oder Transparenz durchgeführt werden soll:
      * **[!UICONTROL Farbe]**: Wählen Sie die Option „Farbe“. Wählen Sie anschließend im Menü „Ecke“ die Bildecke mit der Farbe aus, die am besten der Leerraumfarbe entspricht, die Sie beschneiden möchten.
Auf Farbe basierendes Zuschneiden: Geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie genau mit der Farbe übereinstimmen, die Sie in der Bildecke ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.
      * **[!UICONTROL Transparenz]**: Wählen Sie die Option **[!UICONTROL Transparenz]** aus.
Zuschneiden auf der Grundlage der Transparenz: Geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie transparent sind. Zahlen, die näher an 1 liegen, ermöglichen mehr Transparenz.
      * **[!UICONTROL Toleranz]**: Ziehen Sie den Schieberegler, um eine Toleranz von 0 bis 1 festzulegen.

* **Farbprofiloptionen**: Wählen Sie eine Farbkonvertierung aus, wenn Sie optimierte Dateien erstellen, die für die dynamische Bereitstellung von Adobe Dynamic Media Classic verwendet werden:

   * **[!UICONTROL Beibehaltung der Standardfarbe]**: Behält die Farben des Quellbilds bei, wenn die Bilder Farbrauminformationen enthalten. Es findet keine Farbkonvertierung statt. Heutzutage ist in fast allen Bildern das entsprechende Farbprofil eingebettet. Wenn jedoch ein CMYK-Quellbild kein eingebettetes Farbprofil enthält, werden die Farben in den sRGB-Farbraum (standardmäßiges Rot Grün Blau) umgewandelt. sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Web-Seiten.
   * **[!UICONTROL Ursprünglichen Farbraum beibehalten]**: Behält die Originalfarben bei, ohne dass am Ort der Aufnahme in Adobe Dynamic Media Classic eine Farbkonvertierung stattfindet. Bei Bildern ohne eingebettetes Farbprofil wird jede erforderliche Farbkonvertierung zur Verarbeitung von Bildanforderungen mit den Standardfarbprofilen durchgeführt, die in den Veröffentlichungseinstellungen konfiguriert sind. Diese Farbprofile stimmen nicht immer mit den Farben in den mit dieser Option erstellten Dateien überein. Deshalb empfehlen wir, die Option „Beibehaltung der Standardfarbe“ zu verwenden.
   * **[!UICONTROL Benutzerdefiniertes Formular]** > **[!UICONTROL An]**: Öffnet Menüs, in denen Sie einen **[!UICONTROL Konvertieren aus]** und **[!UICONTROL In konvertieren]** auswählen können. Diese erweiterte Option überschreibt alle Farbinformationen, die in die Quelldatei eingebettet sind. Wählen Sie diese Option nur aus, wenn alle Bilder, die Sie senden, falsche oder fehlende Farbprofildaten enthalten.

* **Bildbearbeitungsoptionen**: Sie können die &lt;>-Schnittmasken in Bildern beibehalten und ein Farbprofil auswählen.
Siehe [Optionen zur Bildoptimierung beim Hochladen](image-editing-options-upload.md#image-editing-options-at-upload).

* **PostScript®-Optionen**: Sie können PostScript®-Dateien rastern, Dateien zuschneiden, transparente Hintergründe beibehalten, eine Auflösung und einen Farbraum auswählen.
Siehe [Arbeiten mit PostScript- und Illustrator-](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Photoshop-Optionen**: Sie können Vorlagen aus Adobe® Photoshop®-Dateien erstellen, Ebenen beibehalten, Ebenennamen angeben, Text extrahieren und angeben, wie Bilder in Vorlagen verankert werden.
Siehe [Optionen für das Hochladen von PSD-Dateien](psd-files.md#psd_upload_options).

* **PDF-Optionen**: Sie können die Dateien rastern, Suchbegriffe und Links extrahieren, automatisch einen E-Katalog generieren, die Auflösung festlegen und einen Farbraum auswählen.
Siehe [Optionen für das Hochladen von PDF-Dateien](pdfs.md#pdf_upload_options).

* **Illustrator-Optionen**: Sie können Adobe Illustrator®-Dateien rastern, transparente Hintergründe beibehalten sowie eine Auflösung und einen Farbraum auswählen.
Siehe [Arbeiten mit PostScript- und Illustrator-](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **EVIDEO-Optionen**: Sie können eine Videodatei transkodieren, indem Sie eine Videovorgabe auswählen.
Siehe [Arbeiten mit Videocodierungsvorgaben](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **Weitere Metadaten**: Geben Sie Schlüsselwörter ein, die die Dateien beschreiben, die Sie hochladen möchten. Trennen Sie Schlüsselwörter mit Kommata. Keywords erleichtern die Suche nach Assets.
Siehe [Durchführen einer erweiterten Suche](searching-assets.md#conducting_an_advanced_search).
Siehe auch [Hochladen von Keywords](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS) Schulungsvideo.

* **Stapelsatzvorgaben**: Um ein Bildset, Rotationsset oder Musterset aus den hochgeladenen Dateien zu erstellen, wählen Sie die Spalte **[!UICONTROL Aktiv]** für die gewünschte Vorgabe aus. Sie können mehrere Vorgaben auswählen. Sie können die Vorgaben auf der Seite „Anwendungseinstellungen/Stapelsatzvorgaben“ erstellen.
Siehe [Stapelsatzvorgaben](application-setup.md#batch_set_presets).

* **Erweitert**: Siehe [Hochladen mit einem anderen Auftrag ](uploading-files.md#follow-an-upload-with-another-job).

## Starten eines weiteren Auftrags im Anschluss an einen Upload-Auftrag {#follow-an-upload-with-another-job}

Wenn Sie Elemente per FTP hochladen, können Sie einen weiteren Auftrag planen, der nach Abschluss des Uploads beginnt. Wenn der Beginn anderer Aufträge geplant ist, werden die Aufträge, die Sie hier planen, nach ihnen in die Warteschlange gestellt.

Der neue Auftrag sendet eine Benachrichtigung an die von Ihnen angegebene Adresse, damit der Code an diesem Speicherort ausgelöst werden kann. Der nachfolgende Veröffentlichungsauftrag erhält den Namen des Upload-Auftrags mit dem Präfix *Pub_*(für Publikation).

**So folgen Sie einem Upload mit einem anderen Auftrag:**

1. Wählen Sie **[!UICONTROL Hochladen]** und dann die Registerkarte **[!UICONTROL VIA FTP]** aus.
1. Wählen Sie in der rechten unteren Ecke der Seite „Hochladen“ die Option **[!UICONTROL Auftragsoptionen]** aus.
1. Erweitern Sie im Dialogfeld Upload-Auftragsoptionen den Abschnitt **[!UICONTROL ERWEITERT]**.
1. Wählen Sie eine der folgenden Optionen aus der Dropdown **[!UICONTROL Liste „Upload mit anderem Auftrag]**&quot;:

   * Keine
   * HTTP-Anfrage
   * Veröffentlichung zum Image-Server
   * Mit Image Rendering veröffentlichen
   * Videoveröffentlichung

1. Geben Sie die HTTP-Adresse an.
1. Geben Sie an, ob nur ausgeführt werden soll, wenn Dateien hochgeladen wurden.
1. Geben Sie an, ob die Anfrage jedes Mal nach Abschluss eines Auftrags oder nur nach der Veröffentlichung von Dateien ausgeführt werden soll.

   >[!NOTE]
   >
   >Regelmäßig geplante Aufträge können manchmal dazu führen, dass keine Dateien veröffentlicht werden.

>[!MORELIKETHIS]
>
>* [Arbeiten mit Asset-Ordnern](asset-folders.md#working_with_asset_folders)
>* [Verarbeiten wiederkehrender Upload- und Veröffentlichungsaufträge](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [Verwenden eines Upload- oder Veröffentlichungsauftrags als Trigger ](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)
