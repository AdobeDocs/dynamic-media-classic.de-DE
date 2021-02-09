---
title: Anwendungseinstellungen
description: Erfahren Sie, wie Sie den Anwendungsbereich von Dynamic Media Classic einrichten.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
translation-type: tm+mt
source-git-commit: c6160315007fa1658f88a857589ec11ac3f0d5ae
workflow-type: tm+mt
source-wordcount: '10925'
ht-degree: 68%

---


# Anwendungseinstellungen{#application-setup}

Auf den Seiten &quot;Anwendungseinstellungen&quot;können Sie allgemeine Einstellungen eingeben, Bildvorgaben, Videokodierungsvorgaben, Viewer-Vorgaben erstellen oder Standard-Viewer und Metadaten definieren. Sie können auch Stapelsatzvorgaben einrichten, um die Erstellung von (beispielsweise) 2D-Rotationssets, Veröffentlichungseinstellungen und Video SEO-Einstellungen zu automatisieren.

>[!NOTE]
>
>Nur Dynamic Media Classic-Administratoren können Einstellungen auf den Seiten &quot;Anwendungseinstellungen&quot;ändern.

## Allgemeine Einstellungen {#general-settings}

Um den Anzeigebereich „Allgemeine Programmeinstellungen“ in der Symbolleiste für globale Navigation zu öffnen, klicken Sie auf **[!UICONTROL „Einstellungen“ > „Anwendungseinstellungen“ > „Allgemeine Einstellungen“]**.

### Server

Bei der Kontoerstellung stellt Dynamic Media Classic die zugewiesenen Server automatisch für Ihre Firma bereit. Auf Grundlage dieser Server werden URL-Zeichenfolgen für Ihre Websites und Anwendungen erstellt. Diese URL-Aufrufe sind spezifisch für Ihr Konto.

Siehe auch [Testen des Secure Testing-Dienstes](testing-assets-making-them-public.md#testing_the_secure_testing_service).

* **Veröffentlichter Servername** : Dieser Server ist der Live-CDN-Server, der in allen systemspezifischen URL-Aufrufen für Ihr Konto verwendet wird. Ändern Sie diesen Servernamen nur, wenn Sie von einem Dynamic Media Classic-Support-Mitarbeiter dazu aufgefordert werden.

* **Servername**  der Herkunft: Dieser Server dient nur zum Testen der Qualitätssicherung. Ändern Sie diesen Servernamen nur, wenn Sie von einem Dynamic Media Classic-Support-Mitarbeiter dazu aufgefordert werden.

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by a Dynamic Media Classic support technician. -->

* **Test&amp;Zielgruppe-Servername**  - Ihre Test&amp;Zielgruppe-URL bis einschließlich .com. Anweisungen zum Abrufen dieser URL finden Sie unter Integrieren von [!DNL Dynamic Media Classic] mit [!DNL Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **Servername**  für iOS-Streaming - Die URL für Ihren  [!DNL Dynamic Media Classic] iOS-Streaming-Server. Dieser Server liefert Streaming-Video für iOS-basierte Geräte über das HTTP-Protokoll.

* **Servername**  für progressives Video - Die URL für Ihren  [!DNL Dynamic Media Classic] progressiven Videoserver. Dieser Server liefert Progressive Video über das HTTP-Protokoll.

* **URL für unveröffentlichte Assets**  anzeigen: Wählen Sie diese Option, wenn bei der Vorschau eines Assets eine URL angezeigt werden  [!DNL Dynamic Media Classic] soll (unabhängig davon, ob es veröffentlicht wurde oder nicht). Falls das Asset noch nicht veröffentlicht wurde, funktioniert die URL nicht. Sie können jedoch die URL für Planungs- oder organisatorische Zwecke verwenden.

<!-- **Allow AIR install** Select this option to allow users to download Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the web version of Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Dynamic Media Classic AIR. Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **Vorlage**  zur Ungültigmachung des CDN-Cache (Content Versand Network): Gibt die Vorlage an, mit der der CDN-Cache ungültig gemacht wird.

   Angenommen, Sie geben eine Bild-URL (einschließlich Bildvorgaben oder Modifikatoren) ein, die auf `<ID>` verweist, anstatt einer bestimmten Bild-ID wie im folgenden Beispiel:

   `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

   Wenn die Vorlage nur `<ID>` enthält, füllt Dynamic Media Classic das Element `https://<server>/is/image` aus, wobei `<server>` der Name des Veröffentlichungsservers ist, der in den allgemeinen Einstellungen definiert ist.

   Wenn Sie die Vorgabe „Ungültiges CDN“ einrichten, ein Bild namens „Backpack_B“ auswählen und dann auf **Datei** > **Ungültiges CDN** klicken, wird die folgende URL in der Benutzeroberfläche für ungültige CDNs generiert:

   `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

   Klicken Sie im URL-Listenfeld auf **Weiter**, um den Cache für diesen Aufruf dieser speziellen Bild-URL zu löschen. Beachten Sie, dass Sie URLs auch hinzufügen können, indem Sie sie in das URL-Listenfeld eingeben oder einfügen. Sie müssen nicht zuvor die Vorlage festlegen.

   Nachdem Sie die Vorlage für das Ungültigmachen des CDN-Cache ausgewählt und eine Anforderung zum Ungültigmachen des CDN gestellt haben, wird die Zeit, die geschätzt zum Löschen des Cache benötigt wird, in einem Popup angezeigt.

   Wenn in Dynamic Media Classic mehrere Bilder ausgewählt sind, wenn Sie auf **Datei** > **Ungültiges CDN** klicken, wird jedes Bild in der gespeicherten Vorlagen-URL referenziert. Daher können Sie eine Vorlage für „Ungültiges CDN“ mit Verweis auf jede URL definieren, auf die auf Ihrer Website verwiesen wird (z. B. Produktdetails, Suchergebnisse usw.). Wenn Sie dann mindestens ein Bilder zur Ungültigmachung aus dem Cache auswählen, füllen die URLs die Oberfläche automatisch aus.

   Siehe [Inhalts-Caching](dmc-platform-overview.md#content_caching).

   Siehe [Erneut veröffentlichte Assets und CDN-Verzögerungen](publishing-files.md#republished_assets_and_cdn_delays).

### Durchsuchen

* **Projekte**  anzeigen: Bestimmt, ob Projekte als Organisationsmöglichkeit für Ihre Dynamic Media Classic-Assets verfügbar sind. Siehe Verwalten der Arbeit mithilfe von Projekten.

* **Beispielinhalt**  für eVideo anzeigen: Aktivieren oder deaktivieren Sie die Anzeige von Beispielinhalten für eVideo.

* **Generierten Inhalt**  anzeigen: Zeigt in Ordnern den Inhalt an, der aus einem Asset generiert wurde. Wenn beispielsweise eine PDF-Datei beim Hochladen gerastert wird, erstellt Dynamic Media Classic für jede Seite der Original-PDF ein Bild. Wenn die Option „Generierten Inhalt anzeigen“ aktiviert ist, erscheint jedes beim Hochladen der Original-PDF generierte Bild zusammen mit der PDF in dem Ordner, in den die PDF hochgeladen wurde.

* **Kodierte Videos**  anzeigen - standardmäßig deaktiviert (deaktiviert).

   Wenn Sie Videos in Dynamic Media Classic schnell suchen und suchen möchten, ohne durch zahlreiche kodierte Ableitungen desselben Videos navigieren zu müssen, lassen Sie diese Option deaktiviert (Standard). In der Benutzeroberfläche werden nur die Miniaturansicht des Mastervideos (das Ausgangsvideo, das Sie hochgeladen und zum Erstellen aller Varianten verwendet haben) und die Miniaturansicht des übergeordneten adaptiven Videosets angezeigt, das alle untergeordneten Varianten des kodierten Videosets enthält.

   Vom Mastervideo oder dem adaptiven Videoset aus können Sie jedoch weiterhin auf einzelne kodierte Videos zugreifen. Doppelklicken Sie hierzu auf das Videominiaturbild, um die Detailansicht zu öffnen. Klicken Sie dann im rechten Bedienfeld auf **„Kodierte Videos“**, um auf alle untergeordneten Videos zuzugreifen.

   Sie können auch den Befehl **„Datei“ > „Neu verarbeiten“** wählen, um direkt aus einem adaptiven Videoset weitere kodierte untergeordnete Videos zu erstellen. Dynamic Media Classic findet automatisch das übergeordnete Übergeordnet-Video des adaptiven Videosets und verwendet es als Quellvideo zum Transkodieren. Nachdem Sie die neuen, individuell kodierten Videos gespeichert haben, werden sie jedoch nicht angezeigt, wenn Sie nach ihnen suchen. Sie sind jedoch weiterhin über die Registerkarte „Kodierte Videos“ in der Detailansicht verfügbar.

   Siehe [Hochladen und Transkodieren von Videos](uploading-encoding-videos.md#uploading_and_encoding_videos).

   Um auch im Rahmen einer Suche weiterhin auf alle verschlüsselten Videoableitungen zugreifen zu können, aktivieren Sie die Option **„Kodierte Videos anzeigen“**.

   Das Menü „Erstellen“ enthält bestimmte Aktionen, die nur (oder optional) mit einzelnen Videos verwendet werden. Daher müssen alle kodierten Videoableitungen angezeigt werden, aus denen Sie auswählen können, unabhängig davon, wie Sie die Option **„Kodierte Videos anzeigen“** eingestellt haben. Zu den Erstellungsaktionen, die die Einstellung **Kodierte Videos anzeigen** überschreiben, zählen **Adaptive Videosets** und **eCatalogs**.

   >[!NOTE]
   >
   >Wenn Sie Ihre Video-Assets nicht mit Dynamic Media Classic hochgeladen und kodiert haben, zeigt Dynamic Media Classic alle kodierten Videos an, selbst wenn diese Option deaktiviert ist.

* **Schaltfläche**  &quot;Unterordner aktualisieren&quot;anzeigen: Aktivieren oder deaktivieren Sie die Anzeige der Schaltfläche zum Aktualisieren der Unterordner.

### Dynamic Media Classic FTP-Konto

* **Server**  - Liste des FTP-Kontoservers.

* **Benutzername**  - Liste des Benutzernamens Ihres FTP-Kontos.

### Zur Anwendung hochladen

* **Bilder**  überschreiben: Dynamic Media Classic lässt nicht zu, dass zwei Dateien denselben Namen haben. Die Dynamic Media Classic-ID jedes Elements (der Bildname ohne Dateinamenerweiterung) muss eindeutig sein. Aufgrund dieser Regel enthält das Dialogfeld „Hochladen“ die Option „Überschreiben“. Die genaue Wirkung dieser Option hängt von der Einstellung der Option „Bilder überschreiben“ ab. Sie legen damit fest, was beim Hochladen von Ersatzbildern geschieht – die Ersatzbilder können die Originalbilder ersetzen oder zu Duplikaten werden. Duplikate werden durch Anhängen einer Ziffer umbenannt („Sessel.tif“ würde beispielsweise zu „Sessel-1.tif“). Die Optionen wirken sich auf Bilder aus, die in einen vom Originalspeicherort abweichenden Ordner hochgeladen werden bzw. die eine andere Dateierweiterung haben als das Original (beispielsweise JPG, TIF oder PNG). (Siehe Verwenden der Option „Bilder überschreiben“.)

   * **Im aktuellen Ordner überschreiben, gleicher Name/Erweiterung**  des Basisbilds - Diese Option ist die strengste Ersatzregel. Das Ersatzbild muss in den Ordner des Originalbilds hochgeladen werden und dieselbe Dateierweiterung haben wie das Originalbild. Wenn diese Voraussetzungen nicht erfüllt sind, wird ein Duplikat erstellt.

   * **Im aktuellen Ordner überschreiben, Name des Basisassets unabhängig von der Erweiterung**  - Erfordert, dass Sie das Ersatzbild in denselben Ordner hochladen wie das Original, jedoch kann die Dateinamenerweiterung vom Original abweichen. Beispiel: „Sessel.tif“ ersetzt die Datei „Sessel.jpg“.

   * **In einem beliebigen Ordner überschreiben, Name/Erweiterung**  des Basisassets - Erfordert, dass das Ersatzbild dieselbe Dateinamenerweiterung wie das Originalbild hat (z. B. &quot;Sessel.jpg&quot;muss &quot;Sessel.jpg&quot;ersetzen, nicht &quot;Sessel.tif&quot;). Sie können das Ersatzbild jedoch in einen anderen Ordner hochladen als den, in dem sich das Original befindet. Das hochgeladene Bild bleibt dann im neuen Ordner; die Datei befindet sich also nicht mehr am ursprünglichen Speicherort.

   * **In jedem Ordner mit demselben Asset-Namen unabhängig von der Erweiterung**  überschreiben - Diese Option ist die am meisten einschließende Ersatzregel. Sie können ein Ersatzbild in einen anderen Ordner hochladen als den, in dem sich das Originalbild befindet, und eine Datei mit einer anderen Dateierweiterung verwenden, um die Originaldatei zu ersetzen. Wenn sich die Originaldatei in einem anderen Ordner befindet, bleibt das Ersatzbild in dem neuen Ordner, in den es hochgeladen wurde.

* **Veröffentlichung**  beibehalten: Gibt an, ob bei einem nach Dynamic Media Classic hochgeladenen Ersatzbild die Einstellung &quot;Bereit zum Veröffentlichen&quot;des ersetzten Bilds beibehalten wird oder ob die Einstellung beim Hochladen festgelegt wurde.

* **Standardfarbbilder** : Gibt die Profil an, die beim Hinzufügen von CMYK-Profilen als Teil der Profil-Standardoptionen angewendet werden.

* **Standardmäßige Upload-Optionen** : Öffnet das Dialogfeld &quot;Upload-Auftragsoptionen&quot;, in dem Sie die standardmäßigen Upload-Optionen festlegen können. Informationen zu diesen Optionen finden Sie unter Upload-Optionen.

### Imagemap-Editor, an Anwendung

* **Standard-HREF**  für Imagemaps: Definiert die Standard-URL, die für die HREF-Spalte für die Imagemaps verwendet wird. Dabei handelt es sich um die Standard-URL, die beim Erstellen neuer Imagemaps angezeigt wird.

* **Standardvorlage**  für Imagemaps: Definiert das standardmäßige JavaScript für die HREF-Vorlage für die Imagemaps. Sie haben die Möglichkeit, benutzerdefinierten Code einzustellen, der beim Klicken auf eine Imagemap ausgeführt wird.

### Andere Einstellungen, an Anwendung

* **Warnungen**  zum Bereinigen des Papierkorbs: Assets im Papierkorb werden innerhalb von sieben Tagen automatisch entfernt. Wählen Sie „E-Mails senden, bevor Elemente im Papierkorb automatisch gelöscht werden“, wenn Unternehmensadministratoren vier Tage vor dem dauerhaften Löschen von Assets im Papierkorb eine Benachrichtigung erhalten sollen. Siehe Verwalten des Ordners „Papierkorb“.

## Verwendung der Option zum Überschreiben der Bilder {#using-the-overwrite-images-option}

Dynamic Media Classic lässt nicht zu, dass zwei Dateien denselben Namen haben. Die Dynamic Media Classic-ID jedes Elements (der Bildname ohne Dateinamenerweiterung) muss eindeutig sein. Aufgrund dieser Regel enthält das Dialogfeld „Hochladen“ die Option „Bilder überschreiben“. Die genaue Wirkung dieser Option hängt von einer Einstellung für die internen Dynamic Media Classic-Einstellungen jeder Firma ab.

Wenn Sie zuvor Bilder hochgeladen und dann die Originaldateien geändert (bzw. ersetzt) haben, wird mit der Option &quot;Überschreiben&quot;angegeben, wie Dynamic Media Classic die Bilder ersetzt. Informationen über das Bild bleiben unverändert, aber das neue Bild ersetzt das alte. Wenn der Ordner auch Bilder enthält, die nicht bereits in Dynamic Media Classic vorliegen, werden diese Bilder hinzugefügt.

Verwenden Sie diese Option, wenn von Ihnen hochgeladene Bilder geändert wurden, der Verweis auf die Bilder jedoch gleich bleibt. Das Überschreiben ist außerdem beim Hochladen und Extrahieren von Adobe® PDF-Dateien nützlich. Passen Sie die ICC-Farboptionen im Dialogfeld &quot;Hochladen&quot;an und laden Sie sie mithilfe der Funktion &quot;Überschreiben&quot;erneut hoch, um genau festzulegen, wie Dynamic Media Classic *rips* funktioniert.

Die Dynamic Media Classic-IDs, die für den Zugriff auf Bilder von den Produktionsservern verwendet werden, werden von den Bilddateinamen abgeleitet. Die Verwendung von Groß- und Kleinbuchstaben im Dateinamen ist wichtig, sowohl beim Ersetzen vorhandener Dateien als auch bei den Dynamic Media Classic-IDs, die für den Zugriff auf das Bild verwendet werden. Achten Sie darauf, dass Dateinamen mit Groß- und Kleinbuchstaben korrekt geschrieben werden, bevor Sie sie in Dynamic Media Classic hochladen, um zu vermeiden, dass sich Dynamic Media Classic-IDs, die sich nur für dasselbe Bild unterscheiden, nur in Groß- und Kleinschreibung unterscheiden.

Wenn Sie diese Option deaktivieren, werden alle Bilder, die mit vorhandenen Bildern übereinstimmende Dateinamen haben, als Duplikate betrachtet und daher nicht hinzugefügt.

## Bildvorgaben  {#image-presets}

In diesem Anzeigebereich können Bildvorgaben erstellt und bearbeitet werden. Mit Bildvorgaben kann Dynamic Media Classic Bilder dynamisch in unterschiedlichen Größen und Übergeordnet bereitstellen. Jede Bildvorgabe stellt eine vordefinierte Zusammenstellung von Größen- und Formatierungsbefehlen zum Anzeigen des Bildes dar. Wenn Sie eine Bildvorgabe erstellen, wählen Sie eine Größe, in der das Bild gesendet werden soll. Darüber hinaus wählen Sie Formatierungsbefehle, mit denen die Darstellung des Bildes für den Sendevorgang optimiert wird.

Administratoren können Vorgaben für das Exportieren von Assets erstellen. Benutzer können beim Exportieren von Bildern eine Vorgabe auswählen, die die Bilder gemäß den Spezifikationen des Administrators neu formatiert.

Um den Anzeigebereich &quot;Bildvorgaben&quot;zu öffnen, klicken Sie in der Symbolleiste für globale Navigation auf **Einstellungen** > **Bildvorgaben**.

Siehe [Smart Imaging](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic).

### Erstellen und Bearbeiten von Bildvorgaben {#creating-and-editing-image-presets}

1. Klicken Sie auf **„Einstellungen“** > **„Bildvorgaben“**.
1. Sie können eine völlig neue Bildvorgabe erstellen oder eine bereits vorhandene als Vorlage verwenden:
   * **Erstellen einer Bildvorgabe**  - Klicken Sie auf  **Hinzufügen**.
   * **Erstellen einer Bildvorgabe aus einer vorhandenen Vorgabe** : Wählen Sie die Bildvorgabe aus, die der zu erstellenden am ähnlichsten ist, und klicken Sie dann auf Bearbeiten.

1. Geben Sie im Anzeigebereich „Vorgabe hinzufügen“ oder „Vorgabe bearbeiten“ einen Namen für die Vorgabe ein.
1. Legen Sie die gewünschten Einstellungen für die Vorgabe fest. 

   Siehe [Bildvorgabeoptionen](application-setup.md#image_preset_options).

1. Klicken Sie auf **Speichern** oder, wenn Sie mit einer vorhandenen Vorgabe begonnen haben, auf **Speichern unter**.
1. Um die Vorgabe mit Ihrem eigenen Bild Vorschau, klicken Sie auf **Durchsuchen** und wählen Sie dann ein Bild aus. Um mit dem Standardbild Vorschau, klicken Sie auf **Zurücksetzen**.

Sie können eine Bildvorgabe bearbeiten, indem Sie im Anzeigebereich „Bildvorgaben“ deren Namen markieren und auf „Bearbeiten“ klicken. Um eine Bildvorgabe zu löschen, wählen Sie diese aus und klicken Sie auf „Löschen“.

### Optionen für Bildvorgaben  {#image-preset-options}

Der Anzeigebereich „Vorgabe hinzufügen“ bzw. „Vorgabe bearbeiten“ bietet folgende Optionen zum Erstellen bzw. Bearbeiten von Bildvorgaben:

**Vorgabenname** Geben Sie einen beschreibenden Namen ohne Leerzeichen ein. Fügen Sie eine Bildgrößenangabe in den Namen ein, um Benutzern die Identifizierung der Bildvorgabe zu erleichtern.

**Breite und** HöheGeben Sie in Pixel die Größe ein, in der das Bild bereitgestellt wird.

**Format** Wählen Sie ein Format aus dem Menü. Bei Auswahl der Formate GIF, JPEG, PDF oder TIFF werden weitere Optionen angezeigt:

* GIF-Farbquantisierungsoptionen

   **Typ**

   Wählen Sie „Adaptiv“ (Standard), „Web“ oder „Macintosh“. Wenn Sie „GIF mit Alpha“ wählen, ist die Option „Macintosh®“ nicht verfügbar.

   **Dithering**

   Wählen Sie zwischen „Diffus“ und „Aus“.

   **Anzahl Farben**

   Ziehen Sie den Schieberegler, um 2 bis 255 einzugeben.

   **Farbliste**

   Geben Sie eine kommagetrennte Liste ein. Geben Sie beispielsweise für Weiß, Grau und Schwarz Folgendes ein: 000000,888888,ffffff.

* JPEG-Optionen

   **Qualität**

   Steuert den JPEG-Komprimierungsgrad. Diese Einstellung wirkt sich sowohl auf die Dateigröße als auch die Bildqualität aus. Die JPEG-Qualitätsskala ist 1-100.

   **JPG-Chrominanz-Downsampling aktivieren**

   Da das menschliche Auge gegenüber Hochfrequenzfarbinformationen weniger empfindlich ist als gegenüber Hochfrequenzleuchtdichte, werden die Bildinformationen bei JPEG-Bildern in Leuchtdichte- und Farbkomponenten aufgeteilt. Bei der Komprimierung eines JPEG-Bildes behält die Leuchtdichtekomponente die volle Auflösung, während für die Farbkomponenten ein Downsampling, d. h. eine Mittelwerterstellung für Pixelgruppen, ausgeführt wird. Obwohl das Datenvolumen beim Downsampling um die Hälfte oder ein Drittel reduziert wird, ist die auftretende Qualitätsminderung kaum wahrnehmbar. Downsampling kann nicht auf Graustufenbilder angewendet werden. Mit dieser Technik wird der Komprimierungsgrad, der für Bilder mit hohem Kontrast (z. B. Bilder mit überlappendem Text) sinnvoll ist, reduziert.

* PDF- und TIFF-Optionen

   **Komprimierung**

   Wählen Sie einen Komprimierungsalgorithmus.

**** FarbraumWählen Sie einen Farbraum.

**** ScharfzeichnenWählen Sie die Option &quot;Einfaches Scharfzeichnen aktivieren&quot;, um nach der Skalierung einen grundlegenden Scharfzeichnungsfilter auf das Bild anzuwenden. Wenn ein Bild in einer anderen Größe verschwommen angezeigt wird, kann dieser Effekt durch Scharfzeichnen kompensiert werden.

Weitere Informationen zu Scharfzeichnen, Resamplingmodi und Unschärfemaske finden Sie im Abschnitt [Scharfzeichnen eines Bildes](sharpening-image.md#sharpening_an_image).

**Resamplingmodus** Wählen Sie eine Option für den Resamplingmodus. Mit diesen Optionen wird ein Bild beim Downsampling scharfgezeichnet:

**B-** LinearDie schnellste Resamplingmethode; einige Aliasing-Artefakte sind bemerkbar.

**Bi-** CubicErhöht die CPU-Auslastung auf dem Image-Server, erzielt aber schärfere Bilder mit weniger bemerkbaren Aliasing-Artefakten.

**Sharp2** kann etwas schärfere Ergebnisse als die bikubische Option erzielen, allerdings mit noch höheren CPU-Kosten für den Image-Server.

**Tri-** LinearVerwendet sowohl eine höhere als auch eine niedrigere Auflösung, sofern verfügbar; wird nur empfohlen, wenn das Aliasing ein Problem darstellt. Bei dieser Methode wird die JPEG-Dateigröße durch Reduzierung der Hochfrequenzdaten verringert.

**Unschärfemaske** Wählen Sie diese Optionen, um das Scharfzeichnen zu optimieren:

**** AmountSteuert den Kontrast, der auf Kantenpixel angewendet wird. Der Standardwert ist 1,0. Für Bilder mit höherer Auflösung können Sie ihn auf bis zu 5,0 erhöhen. Sie können sich die Auswirkung der Option „Betrag“ wie ein Maß für die Filterintensität vorstellen.

**** RadiusBestimmt die Anzahl der Pixel um die Kantenpixel, die sich auf das Scharfzeichnen auswirken. Geben Sie für Bilder mit hoher Auflösung Werte zwischen 1 und 2 ein. Bei einem geringeren Wert werden nur die Kantenpixel scharfgezeichnet, während bei einem hohen Wert ein breiterer Pixelbereich scharfgezeichnet wird. Der richtige Wert hängt von der Größe des Bilds ab.

**** SchwellenwertBestimmt den Kontrastbereich, der ignoriert werden soll, wenn der Filter &quot;Unschärfemaske&quot;angewendet wird. Anders ausgedrückt legt diese Option fest, wie stark sich die scharfgezeichneten Pixel von dem sie umgebenden Bereich unterscheiden müssen, damit sie als Kantenpixel erkannt und scharfgezeichnet werden. Damit kein Bildrauschen entsteht, sollten Sie mit Werten zwischen 0,02 und 0,2 experimentieren. Beim Standardwert 6 werden alle Pixel im Bild scharfgezeichnet.

**Color** SpaceBestimmt, ob das Bild den Raum, in dem das Bild erstellt wurde, verwendet, in der Regel RGB (Original) oder einen Luminanzraum (Intensität).

**** ColorWählen Sie folgende Optionen:

**Ausgabefarbprofil** Wählen Sie &quot;Standard verwenden&quot;oder eines der ICC-Profile, die in Dynamic Media Classic verfügbar sind.

Siehe auch [ICC-Profile](icc-profiles.md#icc_profiles).

**Rendering** IntentWählen Sie eine Option, wenn Sie die standardmäßige Renderpriorität des Profils überschreiben möchten. Die Verwendung dieser Option ist sinnvoll, wenn eines der Standard-ICC-Profile Zielfarbraum einer Farbumwandlung ist, ein Ausgabegerät (Drucker oder Bildschirm) durch dieses Profil bestimmt wird und die angegebene Renderpriorität für dieses Profil gültig ist.

**Profil** einbettenWählen Sie diese Option, damit dieses Profil verwendet wird, wenn Sie dieses Bild in Adobe® Photoshop® öffnen.

**Druckauflösung** Wählen Sie eine Auflösung für den Druck dieses Bildes. Der Standardwert ist 72 Pixel.

**URL-** Modifikatoren Wenn Sie lieber die URL-Modifikatoren angeben, die Ihre Bildvorgabe definieren, anstatt die Einstellungen einzugeben, geben Sie die Modifikatoren hier ein.

**Beispiel-Bild-** URLs enthalten die URL-Zeichenfolge &quot;unformatiert&quot;, die der Dynamic Media-Image-Server verwendet, um Bilder mit der Bildvorgabe bereitzustellen, die Sie hinzufügen oder bearbeiten. Diese URL-Zeichenfolge codiert alle Formateinstellungen, die Sie im Anzeigebereich „Vorgabe hinzufügen“ bzw. „Vorgabe bearbeiten“ auswählen.

### Bearbeiten, Entfernen oder Deaktivieren einer Bildvorgabe  {#editing-removing-or-deactivating-an-image-preset}

1. Klicken Sie auf **„Einstellungen“** > **„Bildvorgaben“**.
1. Wählen Sie im Anzeigebereich „Bildvorgaben“ eine Vorgabe aus der Tabelle aus und führen Sie dann einen der folgenden Schritte aus:

   * Klicken Sie auf **Bearbeiten** und geben Sie dann im Dialogfeld &quot;Vorgabe bearbeiten&quot;neue Optionen ein.
   * Klicken Sie auf **Löschen**, um die Vorgabe aus der Liste zu entfernen.
   * Deaktivieren Sie das Kontrollkästchen &quot;Aktiv&quot;neben einem Vorgabennamen, um ihn für MediaPortal-Benutzer aus der gesamten Dynamic Media Classic-Benutzeroberfläche zu entfernen.

## Aktivieren und Deaktivieren von adaptiven Video-Vorgaben {#activating-or-deactivating-adaptive-video-presets}

Vorgaben für die adaptive Videokodierung für Dynamic Media Classic-Angebot. Es handelt sich dabei um eine Masterliste von Vorgaben, in der die Vorgaben für adaptive Videos im Format 16:9 und 4:3 in einer Gruppe zusammengefasst sind. Diese vordefinierten Vorgaben enthalten die am häufigsten verwendeten Kodierungseinstellungen und sind für die Wiedergabe auf Mobilgeräten, Tablets und Desktops optimiert. 

Nur Vorgaben für die adaptive Videokodierung sind standardmäßig aktiviert (bzw. „eigeschaltet“). Sie können sie bei Bedarf deaktivieren. Deaktivierte „Adaptive Video“-Voreinstellungen stehen im eVideo-Abschnitt des Dialogfelds „Upload-Auftragsoptionen“ nicht zur Auswahl. 

Siehe [Hochladen und Kodieren von Videos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**So aktivieren und deaktivieren Sie adaptive Video-Vorgaben**

1. Klicken Sie in der rechten oberen Ecke von Dynamic Media Classic auf **Setup** > **Anwendungseinstellungen** > **Video-Vorgaben** > **Adaptive Video-Vorgaben**.
1. Wenn Sie eine Vorgabe aus der Liste „eVideo-Optionen“ im Dialogfeld „Upload-Auftragsoptionen“ entfernen möchten, deaktivieren Sie auf der Seite „Adaptive Video-Vorgaben“ das Kontrollkästchen neben dem Vorgabenamen.
1. Klicken Sie auf **Schließen**.

## Video-Vorgaben zum Kodieren von Videodateien  {#video-presets-for-encoding-video-files}

Klicken Sie in der rechten unteren Ecke der Seite „Upload“ auf die Option „Auftragsoptionen“, um eine Kodierungsvorgabe auszuwählen. Erweitern Sie in dem Dialogfeld „Upload-Auftragsoptionen“ die eVideo-Optionen und wählen Sie die gewünschten Vorgaben für die Videokodierung aus.

>[!NOTE]
>
>Mit Ausnahme von „Adaptive Video“, das standardmäßig aktiviert ist, werden im Dialogfeld „Upload-Auftragsoptionen“ möglicherweise nicht alle adaptiven oder einzelnen Videokodierungsvorgaben angezeigt. Dynamic Media Classic-Administratoren legen fest, welche Videokodierungsvorgaben im Dialogfeld &quot;Upload-Auftragsoptionen&quot;angezeigt werden.

* Wählen Sie aus den folgenden Vorgaben für die adaptive Kodierung bzw. für die einzelne Kodierung:

   **16:9 Adaptive Video**

   Erstellen Sie Videos mit dem Seitenverhältnis von 16:9 für Versand zu Desktops, Mobilgeräten (iPhone, iPad, Android) und Tablets (iPad, Android), deren Auflösung und Bitrate am besten mit der Verbindungsgeschwindigkeit des Viewers übereinstimmt.

   **4:3 Adaptive Video**

   Erstellen Sie Videos mit dem Seitenverhältnis von 4:3 für Versand zu Desktops, Mobilgeräten (iPhone, iPad, Android) und Tablets (iPad, Android), die mit der Auflösung und Bitrate optimiert wurden, die der Verbindungsgeschwindigkeit des Viewers am besten entspricht.

   **Adaptives Video**

   Eine einzelne Kodierungsvorgabe, die mit jedem Seitenverhältnis verwendet werden kann, um Videos zur Wiedergabe auf Mobilgeräten, Tablets und Desktops zu erstellen. Hochgeladene Quellvideos, die mit dieser Vorgabe kodiert wurden, weisen eine feste Höhe auf. Die Breite wird jedoch automatisch skaliert, um das Seitenverhältnis des Videos beizubehalten.

   Die Flexibilität der automatischen Skalierungsfunktion ist ebenfalls standardmäßig verfügbar, wenn Sie eine eigene benutzerdefinierte Vorgabe für die Videokodierung erstellen.

   Siehe [Hinzufügen oder Bearbeiten einer Videokodierungsvorgabe](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   **Adaptive Videokodierung (16:9 oder 4:3)**

   Erstellen Sie Videos mit dem Seitenverhältnis 16:9 und 4:3 für Versand zu Desktop-PCs, Mobilgeräten (iPhone, iPad, Android) und Tablets (iPad, Android), die mit der Auflösung und Bitrate optimiert wurden, die der Verbindungsgeschwindigkeit des Viewers am besten entspricht.

   Siehe [Vorgaben für die Videokodierung (16:9 oder 16:9: 3)](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets).

   **Einzelne Kodierungsvorgaben**

   >[!NOTE]
   >
   >Um Videos auf iPads auszugeben, können Sie eine der Kodierungsvorgaben unter „Mobil“ oder „Tablet“ auswählen. Tablet-Vorgaben weisen gewöhnlich eine höhere Auflösung und Qualität auf und sind für den iPad mit seinem größeren Display und der hohen Verbindungsgeschwindigkeit optimiert. Damit Videodateien, die mit einer Tablet-Vorgabe kodiert wurden, richtig wiedergegeben werden können, muss die mobile Site bzw. Anwendung über einen Code zur Geräteerkennung verfügen. Dieser Code sorgt dafür, dass, abhängig vom erkannten Wiedergabegerät, das entsprechende Videomaterial für iPhone oder iPad bereitgestellt wird. Durch die Auswahl einer Mobil-Vorgabe für die Wiedergabe von Videodateien auf dem iPad wird der Workflow vereinfacht. Das liegt daran, dass Sie für iPhones und iPads dieselbe Videodatei verwenden können. Allerdings wird dabei die Qualität des Videomaterials an das iPhone mit seiner geringeren Auflösung angepasst.

   * Wählen Sie unter der Gruppe „Kodierungsvorgaben“ in der Dropdown-Liste „Kodierungsvorgaben sortieren“ entweder „Name“ oder „Größe“, um die Vorgaben nach Name oder Auflösung zu sortieren.
   * Wählen Sie eine für die Auflösung und Bandbreite der geplanten Videowiedergabe geeignete Kodierungsvorgabe.
   * Sie können die adaptive Videokodierung und eine oder mehrere Kodierungsvorgaben pro Video auswählen. Beispielsweise können Sie eine Datei beim Hochladen gleichzeitig für Desktop und mobile Geräte kodieren.

Nach dem Klicken auf **Hochladen starten** wird die ursprüngliche Mastervideodatei hochgeladen, und daraus werden kodierte Dateien generiert.

### Kodierungsvorgabeoptionen  {#about-encoding-preset-options}

Folgende Parameter stehen für die Kodierungsvorgabeoptionen zur Verfügung:

**Verbindungsgeschwindigkeit der Zielgruppe** Die Internetverbindungsgeschwindigkeit des Endbenutzers.

**Encoded file** suffixDas Suffix, das zur Identifizierung an die kodierte Videodatei angehängt wird.

**Video-Bitrate (Datenrate)**  Die Menge an kodierten Daten, die eine Sekunde Videowiedergabe ausmachen (in Kilobit pro Sekunde).

**Pixelbreite/-** höheDie Breite des Bildschirmbilds in Pixel; die Höhe des Bildschirmbilds (in Pixel).

**Einzelbild pro Sekunde (fps)** Die Anzahl der Einzelbilder oder Standbilder pro Sekunde des Videos. In den USA und Japan werden die meisten Videos mit 29,97 fps aufgenommen und in Europa und Asien (ausgenommen Japan) mit 25 fps. Film wird mit 24 fps aufgenommen.

**Audio-** BitrateDie Menge der kodierten Daten, die eine Sekunde Audiowiedergabe ausmachen, in Kilobit pro Sekunde.

Die folgende Tabelle enthält empfohlene Verfahren zur Auswahl von Video-Vorgaben und die Namenskonventionen, mit denen kodierte Dateien bezeichnet werden.

### Adaptive Video (Standard)  {#adaptive-video-default}

Eine Kodierungsvorgabe, die mit jedem Seitenverhältnis verwendet werden kann, um Videos zur Wiedergabe auf Mobilgeräten, Tablets und Desktops zu erstellen. Hochgeladene Quellvideos, die mit dieser Vorgabe kodiert werden (Standard und optimales Verfahren), werden auf eine feste Höhe eingestellt, die Breite wird jedoch automatisch so skaliert, dass das Seitenverhältnis des Videos beibehalten wird.

**Adaptive Video (Standard)**

|  | Kodierungsvorgabenname/QuickInfo-Text | Kodierungsdateisuffix | Videodatenrate (Kbit/s) | Breite/Höhe (Pixel) | Einzelbilder pro Sekunde (fps) | Audiobitrate (Kbit/s) | Empfehlungen |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Auto x360, 800 kBit/s | _Mobile_Autox360p_800K | 800 | Autox360 | Gleich Quelle | 64 | Für Mobilgeräte (iPhone, iPad, Android) |
| 2 | Auto x 480, 1400 kBit/s | _Tablet_Autox480p_1400K | 1400 | Autox480 | Gleich Quelle | 96 | Für Tablet (iPad, Android) |
| 3 | Auto x 720, 2600 kBit/s | _Desktop_Autox720p_2600K | 2600 | Autox720 | Gleich Quelle | 128 | Für Desktop |

### Vorgaben für die adaptive Videokodierung (16:9 oder 4:3){#adaptive-video-encoding-or-video-presets}

Diese Vorgaben für die adaptive Videokodierung bestehen aus einer Serie einzelner Kodierungsvorgaben, die basierend auf dem Seitenverhältnis des hochgeladenen Videos automatisch für Sie ausgewählt werden. Wenn Sie z. B. ein 4:3-Video hochladen, wird es automatisch mit allen fünf 4:3-Vorgaben kodiert, die sich in der Master-Vorgabenliste der Option **Adaptive Videokodierung (16:9 oder 4:3)** befinden.

Informationen zu den Parametern für Kodierungsoptionen finden Sie unter [Kodierungsvorgabeoptionen](application-setup.md#about_encoding_preset_options).

**Vorgaben für die adaptive Videokodierung (16:9 oder 4: 3)**

|  | Kodierungsvorgabenname/QuickInfo-Text | Zielverbindungsgeschwindigkeit (Kbit/s) | Kodierungsdateisuffix | Videodatenrate (Kbit/s) | Breite/Höhe (Pixel) | Einzelbilder pro Sekunde (fps) | Audiobitrate (Kbit/s) | Empfehlungen |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512x288, Mobil (iPhone, iPad, Android), (400 KBit/s) | 500 | _Mobile_512x288_400K | 400 | 512 x 288 | Gleich Quelle | 64 | Niedrige Auflösung, 3G |
| 2 | 4:3, 384x288, Mobil (iPhone, iPad, Android), (400 KBit/s) | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Gleich Quelle | 64 | Niedrige Auflösung, 3G |
| 1 | 16:9, 512x288, Mobil (iPhone, iPad, Android), (600 KBit/s) | 700 | _Mobile_512x288_600K | 600 | 512 x 288 | Gleich Quelle | 64 | Mittlere Auflösung, 3G |
| 4 | 4:3, 384x288, Mobil (iPhone, iPad, Android), (600 KBit/s) | 700 | _Mobile_384x288_600 | 800 | 384 x 288 | Gleich Quelle | 64 | Mittlere Auflösung, 3G |
| 5 | 16:9, 640x360, Tablet (iPad, Android), (800 KBit/s) | 900 | _iPad_640x360_800K | 800 | 640 x 360 | Gleich Quelle | 80 | Mittlere Auflösung, WiFi |
| 6 | 4:3, 640x480, Tablet (iPad, Android), (800 KBit/s) | 900 | _iPad_640x480_800K | 600 | 640 x 480 | Gleich Quelle | 80 | Mittlere Auflösung, WiFi |
| 7 | 16:9, 768x432, Tablet (iPad, Android), (1200 KBit/s) | 1,5 Mbit/s | _iPad_768x432_1200K | 1200 | 768 x 432 | Gleich Quelle | 96 | Hohe Auflösung, WiFi |
| 8 | 4:3, 768x576, Tablet (iPad, Android), (1200 KBit/s) | 1,5 Mbit/s | _iPad_768x576_1200K | 1200 | 768 x 576 | Gleich Quelle | 96 | Hohe Auflösung, WiFi |
| 9 | 16:9, 1280 x 720, Desktop, (2000 Kbit/s) | 3,0 Mbit/s | _1280x720_2000K | 2000 | 1280 x 720 | Gleich Quelle | 128 | High Definition, Widescreen |
| 10 | 4:3, 1280 x 960, Desktop, (2000 Kbit/s) | 3,0 Mbit/s | _1280x960_2000K | 2000 Kbit/s | 1280 x 960 | Gleich Quelle | 128 | High Definition |

### Vorgaben für die Videokodierung für Desktop-PCs  {#desktop-video-encoding-presets}

Vorgaben für die Videokodierung für MP4 und OGV auf Desktopcomputern.

Informationen zu den Parametern für Kodierungsoptionen finden Sie unter [Kodierungsvorgabeoptionen](application-setup.md#about_encoding_preset_options).

**H264 Main 3.2 - Audio AAC, Dateierweiterung MP4**

|  | Kodierungsvorgabenname/QuickInfo-Text | Zielverbindungsgeschwindigkeit (Kbit/s) | Kodierungsdateisuffix | Videodatenrate (Kbit/s) | Breite/Höhe (Pixel) | Einzelbilder pro Sekunde (fps) | Audiobitrate (Kbit/s) | Empfehlungen |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480 x 270 (400 Kbit/s) | 500 | _480x270_400K | 400 | 480 x 270 | Gleich Quelle | 64 | Niedrige Auflösung, Widescreen |
| 2 | 16:9, 640 x 360 (800 Kbit/s) | 900 | _640x360_800K | 800 | 640 x 360 | Gleich Quelle | 80 | Mittlere Bildauflösung, Widescreen |
| 1 | 16:9, 800 x 450 (1200 Kbit/s) | 1,5 Mbit/s | _800x450_1200K | 1200 | 800 x 450 | Gleich Quelle | 96 | Mittelhohe Auflösung |
| 4 | 16:9, 1280 x 720 (2000 Kbit/s) | 3,0 Mbit/s | _1280x720_2000K | 2000 | 1280 x 720 | Gleich Quelle | 128 | High Definition, Widescreen |
| 5 | 4:3, 320 x 240 (400 Kbit/s) | 500 | _320X240_400K | 400 | 320 x 240 | Gleich Quelle | 64 | Niedrige Auflösung |
| 6 | 4:3, 480 x 360 (800 Kbit/s) | 900 | _480x360_800K | 600 | 480 x 360 | Gleich Quelle | 80 | Mittlere Auflösung |
| 7 | 4:3, 640 x 480 (1200 Kbit/s) | 1,5 Mbit/s | _640x480_1200K | 1200 | 640 x 480 | Gleich Quelle | 96 | Mittlere Auflösung |
| 8 | 4:3, 1280 x 960 (2000 Kbit/s) | 3,0 Mbit/s | _1280x960_2000K | 2000 | 1280 x 960 | Gleich Quelle | 128 | High Definition |

**OGG Theora Vorbis - Dateierweiterung OGV**

|  | Kodierungsvorgabenname/QuickInfo-Text | Zielverbindungsgeschwindigkeit (Kbit/s) | Kodierungsdateisuffix | Videodatenrate (Kbit/s) | Breite/Höhe (Pixel) | Einzelbilder pro Sekunde (fps) | Audiobitrate (Kbit/s) | Empfehlungen |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480 x 270 (400 Kbit/s), OGG | 500 | _OGG_480x270_400K | 400 | 480 x 270 | Gleich Quelle | 64 | Niedrige Auflösung, Widescreen |
| 2 | 16:9, 640 x 360 (800 Kbit/s), OGG | 900 | _OGG_640x360_800K | 800 | 640 x 360 | Gleich Quelle | 80 | Mittlere Bildauflösung, Widescreen |
| 1 | 16:9, 800 x 450 (1200 Kbit/s), OGG | 1,5 Mbit/s | _OGG_800x450_1200K | 1200 | 800 x 450 | Gleich Quelle | 96 | Mittelhohe Auflösung |
| 4 | 16:9, 1280 x 720 (2000 Kbit/s), OGG | 3,0 Mbit/s | _OGG_1280x720_2000K | 2000 | 1280 x 720 | Gleich Quelle | 128 | High Definition, Widescreen |
| 5 | 4:3, 320 x 240 (400 Kbit/s), OGG | 500 | _OGG_320X240_400K | 400 | 320 x 240 | Gleich Quelle | 64 | Niedrige Auflösung |
| 6 | 4:3, 480 x 360 (800 Kbit/s), OGG | 900 | _OGG_480x360_800K | 600 | 480 x 360 | Gleich Quelle | 80 | Mittlere Auflösung |
| 7 | 4:3, 640 x 480 (1200 Kbit/s), OGG | 1,5 Mbit/s | _OGG_640x480_1200K | 1200 | 640 x 480 | Gleich Quelle | 96 | Mittlere Auflösung |
| 8 | 4:3, 1280 x 960 (2000 Kbit/s), OGG | 3,0 Mbit/s | _OGG_1280x960_2000K | 2000 | 1280 x 960 | Gleich Quelle | 128 | High Definition |

### Vorgaben für die Videokodierung für Mobilgeräte  {#mobile-video-encoding-presets}

Gleich wie Bildrate der Quelle. Vorgaben für die Videokodierung für iPhone, iPad und Android-Mobilgeräte

Informationen zu den Parametern für Kodierungsoptionen finden Sie unter [Kodierungsvorgabeoptionen](application-setup.md#about_encoding_preset_options).

**H264 Baseline 2.1 - Audio AAC, Dateierweiterung MP4**

|  | Kodierungsvorgabenname/QuickInfo-Text | Zielverbindungsgeschwindigkeit (Kbit/s) | Kodierungsdateisuffix | Videobitrate (Kbit/s) | Pixel Breite/Höhe | Einzelbilder pro Sekunde (fps) | Audiobitrate (Kbit/s) | Empfehlungen |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512 x 288, Mobil (400 Kbit/s) | 500 | _Mobile_512x288_400K | 400 | 512 x 288 | Gleich Quelle | 64 | Niedrige Auflösung, 3G |
| 2 | 16:9, 512 x 288, Mobil (600 Kbit/s) | 700 | _Mobile_512x288_600K | 600 | 512 x 288 | Gleich Quelle | 64 | Mittlere Auflösung, 3G |
| 1 | 16:9, 512 x 288, Mobil (800 Kbit/s) | 900 | _Mobile_512x288_800K | 800 | 512 x 288 | Gleich Quelle | 80 | Mittlere Auflösung, Wi-Fi |
| 4 | 16:9, 512 x 288, Mobil (1000 Kbit/s) | 1,2 Mbit/s | _Mobile_512x288_1000K | 1000 | 512 x 288 | Gleich Quelle | 80 | Hohe Auflösung, Wi-Fi |
| 5 | 16:9, 512 x 288, Mobil (1200 Kbit/s) | 1,5 Mbit/s | _Mobile_512x288_1200K | 1200 | 512 x 288 | Gleich Quelle | 96 | Hohe Auflösung, Wi-Fi |
| 6 | 4:3, 384 x 288, Mobil (400 Kbit/s) | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Gleich Quelle | 64 | Niedrige Auflösung, 3G |
| 7 | 4:3, 384 x 288, Mobil (600 Kbit/s) | 700 | _Mobile_384x288_600K | 800 | 384 x 288 | Gleich Quelle | 64 | Mittlere Auflösung, 3G |
| 8 | 4:3, 448 x 336, Mobil (800 Kbit/s) | 900 | _Mobile_448x336_800K | 800 | 448 x 336 | Gleich Quelle | 80 | Mittlere Auflösung, Wi-Fi |
| 9 | 4:3, 448 x 336, Mobil (1000 Kbit/s) | 1,2 Mbit/s | _Mobile_448x336_1000K | 1000 | 448 x 336 | Gleich Quelle | 80 | Hohe Auflösung, Wi-Fi |
| 10 | 4:3, 448 x 336, Mobil (1200 Kbit/s) | 1,5 Mbit/s | _Mobile_448x336_1200K | 1200 | 448 x 336 | Gleich Quelle | 96 | Hohe Auflösung, Wi-Fi |

## Viewer-Vorgaben  {#viewer-presets}

>[!NOTE]
>
>**Hinweis**  zum Lebenszyklusende für Flash-Viewer: Ab dem 31. Januar 2017 hat Adobe Dynamic Media Classic offiziell die Unterstützung für die Flash-Viewer-Plattform eingestellt.

Eine *Viewer-Vorgabe* ist eine Zusammenstellung von Einstellungen, mit denen die Anzeige von Rich-Media-Assets auf den Computerbildschirmen und Mobilgeräten für die Benutzer festgelegt wird. Sie können als Administrator Viewer-Vorgaben erstellen. Es sind Einstellungen für eine ganze Palette von Viewer-Konfigurationsoptionen verfügbar. Sie können beispielsweise die Viewer-Anzeigegröße, das Zoomverhalten, die Farbschemata, Ränder und Schriftarten ändern.

Als Best Practice sollten Sie die HTML5-Video-Viewer von Dynamic Media Classic verwenden. Dank der für die HTML5 Video Viewer verwendeten Vorgaben handelt es sich um robuste Video-Player. Durch Kombination der Gestaltungsmöglichkeit der Wiedergabekomponenten mit HTML5 und CSS, der eingebetteten Wiedergabe und der Verwendung von adaptivem und progressivem Streaming je nach Browserfähigkeiten in einem einzigen Player, erweitern Sie die Reichweite ihrer Rich Media-Inhalte auf Desktop-, Tablet- und Mobilgerätebenutzer und stellen eine optimierte Videoerfahrung sicher.

Siehe [Informationen zu HTML5-Viewern](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) im Adobe Viewer-Referenzhandbuch.

Siehe Kompatibilitätsmatrix [Dynamic Media Classic Viewer-Vorgabe](application-setup.md#scene7_viewer_preset_compatibility_matrix).

Siehe [Optimale Vorgehensweise: Verwenden des HTML5-Video-Viewers](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

Abhängig vom Viewer können Sie Community-Funktionen hinzufügen. Zu den Community-Funktionen zählen die Schaltflächen „Einbetten“, „E-Mail an Freunde senden“, „Verknüpfen“ und „Zur Website“. Mit diesen Schaltflächen können Benutzer den Viewer für andere freigeben oder die Dynamic Media Classic-Website öffnen.

Siehe auch [Adobe Viewer-Referenzbibliotheksbeispiele](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### Viewer-Unterstützung für interaktiv entwickelte Webseiten {#viewer-support-for-responsive-designed-web-pages}

Verschiedene Webseiten haben unterschiedliche Anforderungen. Eventuell möchten Sie eine Webseite erstellen, die einen Link bereitstellt, der den HTML5-Viewer in einem separaten Browserfenster angezeigt. In anderen Fällen kann es erforderlich sein, den HTML5-Viewer direkt auf der Hosting-Seite einzubetten. Im letzteren Fall hat der Webseite möglicherweise ein statisches Layout. Sie kann auch „Interaktiv“ sein und auf verschiedenen Geräten unterschiedlich oder für verschiedene Fenstergrößen im Browser angezeigt werden. Um diese Anforderungen zu erfüllen, unterstützen die HTML5-Viewer, die mit Dynamic Media Classic geliefert werden, sowohl statische Webseiten als auch reaktionsfähige Webseiten.

Weitere Informationen zum Einbetten von interaktiven Viewern in Ihre Webseiten finden Sie unter [Bibliothek für responsive Bilder](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library.html#image-serving-api), [Verwenden der Bibliothek für responsive Bilder](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#image-serving-api) und [Befehlsreferenz - Befehlsattribute](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#responsive-static-image-library).

### Viewer-Vorgabentypen {#viewer-preset-types}

Administratoren können die folgenden Arten von Viewer-Vorgaben erstellen und anpassen:

**E-Katalog-** ViewerSimuliert das Lesen eines gedruckten Katalogs. Sie können von Seite zu Seite wechseln, Elemente auf einer Seite vergrößern oder verkleinern, Imagemaps verwenden, um weitere Informationen zu Elementen auf der Seite anzuzeigen oder den Katalog zu durchsuchen. Sie können auch ein Infofeld einschließen, um detaillierte Informationen zu einem Element und eine verweissensitive Grafik anzuzeigen, wenn dem Bereich ein gültiges rollover_key-Attribut zugeordnet wurde. Zum Einschließen eines Infofelds geben Sie im Anzeigebereich „Infofeldeinstellungen“ des E-Katalog-Viewer-Vorgabe-Fensters die URL eines Infoservers ein.

**Musterset-** ViewerZeigt ein Bild in einer anderen Farbe, einem anderen Material, einer anderen Textur, einer anderen Ausführung oder einem anderen Stoff an. Über eine Miniaturansicht können Benutzer die Unterschiede im Bild anzeigen.

**Viewer für gemischte Mediensets** Zeigt verschiedene Medientypen in einem Viewer an. Sie können darin Mustersets, Rotationssets, Bilder und Videos einschließen. Sie können Registerkarten für verschiedene Arten von Inhalten einstellen, beispielsweise eine Registerkarte für Bildsätze und eine für Videos. Videos, die aus einem gemischten Medienset abgespielt werden, verwenden einen standardmäßigen Video-Viewer mit einer Zeitleiste und Video-Steuerelementen wie „Abbrechen“, „Anhalten“, „Zurückspulen“ und „Abspielen“. Wenn Sie eine Viewer-Vorgabe für gemischte Mediensets einstellen, geben Sie an, welche Viewer für die verschiedenen Arten von Assets in Ihrem gemischten Medienset verwendet werden sollen. Sie können auch den Raster-Viewer oder den Karussell-Viewer verwenden, um ein gemischtes Medienset anzuzeigen.

**Rotationsset-** ViewerStellt mehrere Ansichten eines Bildes bereit, damit die Benutzer das Objekt drehen können, um die verschiedenen Seiten und Winkel zu untersuchen.

**Video-** ViewerZeigt Videos mit den Abmessungen der Quelldatei oder einer benutzerdefinierten Größe an. Im Lieferumfang von Dynamic Media Classic sind viele vordefinierte Viewer-Vorgaben für die Videowiedergabe enthalten. Als Administrator können Sie auch benutzerdefinierte Video-Viewer-Vorgaben erstellen. Es stehen mehr als ein Dutzend verschiedener Einstellungen zur Konfiguration des Video-Viewers zur Verfügung. Sie können Größe, Vorder- und Hintergrundfarbe, Video- und Audio-Steuerelemente, Fortschrittsleiste, Skin der Benutzeroberfläche, Sozialfunktionen und Hilfe-Funktionen konfigurieren.

**Zoom-** ViewerBietet drei Arten von Zoom-Viewern:

**Zoom-** ViewerErmöglicht Benutzern das Zoomen in den Bereich, indem sie darauf klicken. Sie können auf Steuerelemente klicken, um heran- und herauszuzoomen und das Bild auf seine Standardgröße zurücksetzen.

**Zoom-Viewer: Fly-** outZeigt ein zweites Bild des gezoomten Bereichs neben dem Originalbild an. Der Benutzer hat keine Steuerelemente zur Verfügung. Er bewegt einfach die Auswahl über den Bereich, der angezeigt werden soll.

Bedenken Sie bei der Festlegung der gesamten Bandbreitennutzung für diesen Viewer, dass sowohl das Hauptbild als auch das Flyout-Bild im Viewer geladen werden müssen. Die Größe des Hauptbildes (Anzeigenbreite und -höhe) und der Zoomfaktor bestimmen die Größe des Flyout-Bildes. Setzen Sie diese beiden Werte gut in Relation, damit das Flyout-Bild eine kompakte Dateigröße erhält. Wenn beispielsweise die Hauptbilddatei sehr groß ist, verringern Sie den Wert für den Zoomfaktor. (Die Flyout-Breite und Flyout-Höhe bestimmen die Größe des Flyout-Fensters, aber nicht die Größe des Flyout-Bildes, das in den Viewer geladen wird.)

Wenn die Größe des Hauptbildes beispielsweise 350 x 350 Pixel bei einem Zoomfaktor von 3 beträgt, ist das Flyout-Bild 1050 x 1050 Pixel groß. Wenn die Größe des Hauptbildes 300 x 300 Pixel bei einem Zoomfaktor von 4 beträgt, ist das Flyout-Bild 1200 x 1200 Pixel groß. Über die Einstellung für die JPEG-Qualität (empfohlener Wert: zwischen 80 und 90) können Sie die Dateigröße deutlich reduzieren. Der empfohlene Wert für den Zoomfaktor liegt, je nach Größe des Hauptbildes, zwischen 2,5 und 4.

### Kompatibilitätsmatrix für Dynamic Media Classic Viewer-Vorgaben {#scene-viewer-preset-compatibility-matrix}

**Hinweis** zum Lebenszyklusende von Flashs: Ab dem 31. Januar 2017 hat Adobe Dynamic Media Classic offiziell die Unterstützung für die Flash-Viewer-Plattform eingestellt.

Die folgende Tabelle zeigt die derzeit verfügbaren Dynamic Media Classic Viewer-Vorgaben. Außerdem gibt die Tabelle Aufschluss über die Viewer-Kompatibilität mit Desktop- und mobilen Geräten sowie die für jeden Viewer verwendete Technologie.

Siehe auch [Adobe Viewer-Referenzbibliotheksbeispiele](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

Informationen zu unterstützten Webbrowser- und Betriebssystemversionen für Viewer finden Sie in den Viewer-Versionshinweisen. 

Siehe [Adobe Viewer-Versionshinweise](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/home.html).

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android Smartphone | Android Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Zoom-Viewer |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android Smartphone | Android Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Bildsatz-Viewer |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android Smartphone | Android Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Musterset-Viewer |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android Smartphone | Android Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| E-Katalog-Viewer |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(Enthält Unterstützung für Social Media und Katalogsuche.) | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog(Enthält Unterstützung für Social Media und Katalogsuche.) | HTML5 | X | X | X | X | X |

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android Smartphone | Android Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Rotationsset-Viewer |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**eVideo-Viewer**

Dynamic Media Classic unterstützt die Wiedergabe von mobilen Videos für MP4 H.264-Videos.

* Blackberry-Geräte, die dieses Videoformat unterstützen, finden Sie hier: [Unterstützte Videoformate bei Blackberry](https://developer.blackberry.com/devzone/develop/supported_media/bb10_media_support.html)
* Windows-Geräte, die dieses Videoformat unterstützen, finden Sie unter den folgenden Adressen:[Unterstützte Videoformate unter Windows Phone](https://docs.microsoft.com/en-us/previous-versions/windows/apps/ff462087(v=vs.105)?redirectedfrom=MSDN)

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android Smartphone | Android Tablet | Blackberry-Smartphone | Windows Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video(Enthält Unterstützung für Untertitel.) Siehe [Optimale Vorgehensweise: Verwenden des universellen HTML5-Video-Viewers.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social(Enthält Unterstützung für Untertitel und soziale Medien.) | HTML5 | X | X | X | X | X | X | X |

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android Smartphone | Android Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Viewer für gemischte Mediensets |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Übersicht über die unterstützten Gesten für Mobilgeräte-Viewer {#supported-mobile-viewers-gestures-matrix}

Die folgende Tabelle enthält die Gesten für Mobilgeräte-Viewer, die von iOS-, Android 2.x- und Android 3.x-Geräten unterstützt werden.

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android Smartphone | Android Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Bildsatz-Viewer |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### Über den Bildschirm „Viewer-Voreinstellung“ {#about-the-viewer-preset-screen}

Über den Anzeigebereich „Viewer-Vorgaben“ erstellen und verwalten Sie Viewer-Vorgaben. Klicken Sie auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Viewer-Vorgaben]**, um diesen Bildschirm zu öffnen.

Der Anzeigebereich „Viewer-Vorgaben“ umfasst Werkzeuge für die folgenden Aufgaben:

**Hinzufügen einer** VorgabeKlicken Sie auf Hinzufügen und treffen Sie im Dialogfeld &quot;Hinzufügen Viewer-Vorgabe&quot;eine Auswahl.

Siehe [Hinzufügen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding_and_editing_viewer_presets).

**Bearbeiten einer** VorgabeWählen Sie eine Vorgabe aus und klicken Sie dann auf  **Bearbeiten**.

Siehe [Hinzufügen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding_and_editing_viewer_presets).

**Löschen einer** VorgabeWählen Sie eine Vorgabe aus und klicken Sie dann auf  **Löschen**.

**Exportieren einer** VorgabeWählen Sie eine HTML5-Viewer-Vorgabe und klicken Sie dann auf &quot;Exportieren&quot;, um die Viewer-Skin herunterzuladen, damit Sie sie als Grundlage für das Erstellen und Hinzufügen einer neuen Viewer-Vorgabe verwenden können.

Siehe [Exportieren einer HTML5-Viewer-Vorgabe](application-setup.md#exporting_an_html5_viewer_preset).

**Filtern der** Liste &quot;Viewer-Vorgaben&quot;Mit den folgenden Werkzeugen können Sie die Liste filtern:

* Öffnen Sie die Dropdown-Liste **Aktiv/Inaktiv** und wählen Sie eine Option, um die aktiven Vorgaben, inaktiven Vorgaben oder alle Vorgabe anzuzeigen.
* Öffnen Sie die Dropdown-Liste **Viewer** und wählen Sie eine Option, um nur bestimmte Viewer-Typen anzuzeigen. Wählen Sie **[!UICONTROL Alle Viewer]**, um alle Viewer anzuzeigen.

**Sortieren von** VorgabenKlicken Sie auf eine Spaltenüberschrift (Aktiv, Typ, Vorgabe oder Plattform), um die Liste auf einer Spalte zu sortieren. Klicken Sie nochmals auf einen Spaltentitel, um die Liste in absteigender (oder aufsteigender) Reihenfolge zu sortieren. 

**Aktivieren und Deaktivieren von** VorgabenWählen Sie eine Vorgabe aus und klicken Sie auf die Option &quot;Aktiv&quot;, um sie zu aktivieren oder zu deaktivieren.

Siehe [Aktivieren und Deaktivieren von Viewer-Vorgaben](application-setup.md#activating_or_deactivating_viewer_presets).

>[!NOTE]
>
>Klicken Sie auf „Vorschau“ rechts im Anzeigebereich „Viewer-Vorgaben“, um zu sehen, wie ein Asset in der von Ihnen gewählten Viewer-Vorgabe aussieht. Wenn ein anderes Asset angezeigt werden soll, können Sie im Anzeigebereich „Viewer-Vorgaben“ auf „Durchsuchen“ klicken und im Dialogfeld „Asset für Vorschau auswählen“ das gewünschte Asset auswählen.

### Hinzufügen und Bearbeiten von Viewer-Vorgaben  {#adding-and-editing-viewer-presets}

Neben dem Hinzufügen von Viewer-Vorgaben mithilfe der Option „Hinzufügen“ in der Benutzeroberfläche können Sie auch die Option „Exportieren“ verwenden, um eine Viewer-Vorgabe hinzuzufügen. Exportieren Sie einfach eine vorhandene HTML5-Viewer-Vorgabe und verwenden Sie diese dann als Grundlage für die neue Vorgabe.

Siehe [Exportieren einer HTML5-Viewer-Vorgabe](application-setup.md#exporting_an_html5_viewer_preset).

**So fügen Sie Viewer-Vorgaben hinzu und bearbeiten sie**

1. Klicken Sie in der rechten oberen Ecke von Dynamic Media Classic auf **Setup** > **Viewer-Vorgaben**.

   Sie können die Liste der Vorgaben filtern. Wenn nur Vorgaben für Video-Viewer aufgelistet werden sollen, wählen Sie auf der Symbolleiste direkt über der Tabelle in der Dropdown-Liste „Viewer“ die Option „Video-Viewer“ aus.

1. Fügen Sie im Bildschirm „Viewer-Vorgaben“ die Viewer-Vorgabe hinzu oder bearbeiten Sie sie.

   **Hinzufügen** Klicken Sie auf der Symbolleiste Hinzufügen. Wählen Sie im Dialogfeld „Viewer-Vorgabe hinzufügen“ eine Plattform und anschließend einen Rich-Media-Asset-Typ.

   Klicken Sie auf **Speichern unter**, wenn Sie die Viewer-Vorgabe erstellt haben.

   **Hinzufügen auf Grundlage einer vorhandenen Viewer-** Vorgabe Wählen Sie in der Tabelle eine Video-Viewer-Vorgabe aus und klicken Sie dann in der Symbolleiste auf Bearbeiten.

   Klicken Sie nach der Neukonfiguration des Video-Viewers auf **Speichern unter**, um die Vorgabe unter einem anderen Namen im Textfeld „Vorgabename“ zu speichern.

   **** BearbeitenWählen Sie eine vorhandene Viewer-Vorgabe aus und klicken Sie dann auf  **Bearbeiten**.

1. Geben Sie im Anzeigebereich „Viewer konfigurieren“ im Feld „Vorgabename“ den Namen der Vorgabe ein oder bearbeiten Sie den bereits vorhandenen Namen im Feld.
1. Legen Sie die weiteren gewünschten Optionen fest.

   >[!NOTE]
   >
   >Wenn Sie „Gleich Quelle“ wählen, wird die Größe des Video-Viewers automatisch an die Abmessungen des kodierten Videos angepasst. Wenn Sie diese Option wählen, können Sie nicht die Anzeigenbreite oder -höhe eingeben. Stattdessen werden diese Optionen vom Video selbst übernommen. Wenn Sie „Gleich Quelle“ wählen, müssen Sie die Randgröße an die Abmessungen der Skin außerhalb des Wiedergabebereichs anpassen. Die Randgröße bezeichnet Höhe und Breite der Video-Steuerelemente in Pixel. Anhand der folgenden Abbildung können Sie Ihre gewünschte Randgröße bestimmen.*

   ![Randkonfiguration des Video-Viewers](assets/vs_video_viewer_configure_margin.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **Speichern unter**, wenn Sie eine Viewer-Vorgabe auf Grundlage einer bereits vorhandenen Vorgabe erstellen.
   * Klicken Sie auf **Speichern**, wenn Sie eine Viewer-Vorgabe hinzugefügt oder bearbeitet haben.

### Exportieren einer HTML5-Viewer-Vorgabe {#exporting-an-html-viewer-preset}

Sie können eine vorhandene HTML5-Viewer-Vorgabe exportieren, um sie als Grundlage für die Erstellung einer neuen HTML5-Viewer-Vorgabe zu verwenden. Diese Exportoption ist nützlich, da Sie den Viewer auf diese Weise nicht komplett neu erstellen müssen. Stattdessen exportieren Sie eine Vorgabe mit Einstellungen, die Ihren Anforderungen in etwa entsprechen, und verwenden diese dann als Ausgangspunkt für Ihre Design-Anpassungen.

Beachten Sie, dass alle standardmäßigen CSS-Vorgabendateien für Viewer in Dynamic Media Classic relative Image Serving-Pfade verwenden, die auf Elemente unter `Scene7SharedAssets` verweisen. Beispiel: Der folgende Pfad ist ein relativer Pfad zu einem Bild-Asset in einer CSS-Vorgabe-Vorgabe-Datei unter `Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`Wenn Sie jedoch Viewer-CSS-Dateien auf Ihrer eigenen Site hosten, müssen Sie diesen relativen Bildpfad auflösen, indem Sie einen expliziten Pfad zum Image-Server in Ihrer eigenen Umgebung verwenden. Wenn Sie zum Beispiel den relativen Pfad über einem expliziten Pfad aktualisieren möchten, könnte er wie folgt aussehen, wobei `https://s7d1.scene7.com` der direkte Pfad zum Image-Server ist: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**So exportieren Sie eine HTML5-Viewer-Vorgabe**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Klicken Sie auf **Einstellungen** > **Viewer-Vorgaben**.
1. Wählen Sie in der Symbolleiste &quot;Viewer-Vorgaben&quot;in der zweiten Dropdown-Liste von links **HTML5**.
1. Wählen Sie in der dritten Dropdown-Liste von links die Option **Alle Viewer** aus.
1. Wählen Sie die Viewer-Vorgabe aus, die Sie als Grundlage für eine neue HTML5-Viewer-Vorgabe verwenden möchten.
1. Klicken Sie auf der Symbolleiste auf **Exportieren**.
1. Klicken Sie im Dialogfeld „Ausgewählte Assets exportieren“ auf **Export starten**.

   Nach dem Export erhalten Sie eine CSS-Datei. Laden Sie die Datei herunter und dekomprimieren Sie sie.

1. Öffnen Sie die CSS-Datei in einem CSS-Editor, nehmen Sie Ihre Änderungen vor und speichern Sie die Datei anschließend.
1. Laden Sie die CSS-Datei in Dynamic Media Classic hoch.

   Siehe [Hochladen von Dateien](uploading-files.md#uploading_files).

1. Veröffentlichen Sie die CSS-Datei auf dem Dynamic Media Image Server.

   Siehe [Veröffentlichen von Dateien](publishing-files.md#publishing_files).

1. Fügen Sie wie üblich die neue Viewer-Vorgabe hinzu. Wählen Sie die hochgeladene Viewer-CSS-Datei aus.

   Siehe [Hinzufügen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding_and_editing_viewer_presets).

### Aktivieren oder Deaktivieren von Viewer-Vorgaben  {#activating-or-deactivating-viewer-presets}

Wenn Benutzer eine URL zum Anzeigen von Assets erstellen möchten, öffnen Sie im Dialogfeld „Vorschau“ die Dropdown-Liste „Vorgaben“, wählen eine Viewer-Vorgabe aus und klicken auf die Schaltfläche „URL kopieren“ (siehe [Kopieren der URL einer Viewer-Vorgabe](application-setup.md#copying_the_url_of_a_viewer_preset)). Diese Vorgabenliste enthält Viewer-Vorgaben, die Administratoren im Anzeigebereich „Viewer-Vorgaben“ hinzufügen und verwalten können. Alle aktiven E-Katalog-Viewer-Vorgaben werden beispielsweise im Dialogfeld „Vorschau“ in der Dropdown-Liste „Vorgaben“ angezeigt, wenn ein Benutzer eine Vorschau eines E-Katalogs anzeigt.

Wenn Sie Viewer-Vorgaben im Anzeigebereich „Viewer-Vorgaben“ nicht deaktivieren, kann die Dropdown-Liste „Vorgaben“ im Dialogfeld „Vorschau“ sehr viele Einträge umfassen.

**So aktivieren oder deaktivieren Sie Viewer-Vorgaben**

1. Wählen Sie **Setup** > **Viewer-Vorgaben**, um den Anzeigebereich &quot;Viewer-Vorgaben&quot;zu öffnen.
1. Aktivieren oder deaktivieren Sie die Optionen „Aktiv“, um die Viewer-Vorgaben zu aktivieren oder zu deaktivieren.

### Kopieren der URL einer Viewer-Vorgabe {#copying-the-url-of-a-viewer-preset}

Nachdem Sie ein Asset veröffentlicht haben, können Sie eine URL kopieren, um das Asset mit den Einstellungen einer bestimmten Viewer-Vorgabe anzuzeigen.

Die URL wird in die Zwischenablage kopiert. Anschließend können Sie sie nach Bedarf in den HTML-Code Ihrer Website, des Mobilgeräts oder Ihrer Anwendung einfügen.

**So kopieren Sie die URL einer Viewer-Vorgabe**

1. Markieren Sie das Asset im Durchsuchenbedienfeld.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Klicken Sie auf „**Rasteransicht**“. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Klicken Sie im URLs- und Code-einbetten-Bedienfeld auf der rechten Seite rechts neben dem gewünschten Viewer auf „**URL kopieren**“.
   * Klicken Sie auf „**Rasteransicht**“. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und klicken Sie anschließend unterhalb des Miniaturbilds auf „**Vorschau**“ > „**Viewer-Liste**“.

   Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**URL kopieren**“.

   * Klicken Sie auf „**Listenansicht**“. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und klicken Sie dann rechts neben dem Miniaturbild auf „**Vorschau**“ > „**Viewer-Liste**“.

   Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**URL kopieren**“.

   * Klicken Sie auf „**Rasteransicht**“, „**Listenansicht**“ oder „**Detailansicht**“. Klicken Sie in der gleichen Symbolleiste auf „**Vorschau**“ > „**Viewer-Liste**“.

   Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**URL kopieren**“.

### Kopieren von Einbettungscode einer Viewer-Vorgabe  {#copying-the-embed-code-of-a-viewer-preset}

Mithilfe der Einbettungscode-Funktion können Sie den Viewer-Code für die ausgewählte Viewer-Vorgabe überprüfen. Sie können den Code auch in die Zwischenablage kopieren, damit Sie ihn in Webseiten für die Bereitstellung des Viewers einfügen können.

Die Bearbeitung des Codes ist im Dialogfeld Einbettungscode nicht zulässig.

**So kopieren Sie den Einbettungscode einer Viewer-Vorgabe**

1. Wählen Sie das Asset im Bedienfeld zum Durchsuchen von Assets aus.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Klicken Sie auf „**Rasteransicht**“. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Klicken Sie im URLs-Bedienfeld auf der rechten Seite auf „**Code einbetten**“.
   * Klicken Sie auf „**Rasteransicht**“. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und klicken Sie anschließend unterhalb des Miniaturbilds auf „**Vorschau**“ > „**Viewer-Liste**“.

   Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**Code einbetten**“.

   * Klicken Sie auf „**Listenansicht**“. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und klicken Sie dann rechts neben dem Miniaturbild auf „**Vorschau**“ > „**Viewer-Liste**“.

   Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**Code einbetten**“.

   * Klicken Sie auf „**Rasteransicht**“, „**Listenansicht**“ oder „**Detailansicht**“. Klicken Sie in der gleichen Symbolleiste auf „**Vorschau**“ > „**Viewer-Liste**“.

   Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**Code einbetten**“.

1. Klicken Sie im Dialogfeld „Code einbetten“ auf „**In Zwischenablage kopieren**“.
1. Klicken Sie auf „**Schließen**“.

## Konfigurieren von Standard-Viewern  {#configuring-default-viewers}

Mit Standard-Viewern können Sie den Standard-Viewer konfigurieren, der mit einem Asset verknüpft ist, wenn Sie Vorschau in Dynamic Media Classic verwenden. Die Standardvorschau kann für die folgenden Asset-Typen festgelegt werden:

* Bild
* Video
* Rotationsset
* Katalog
* Bildsatz
* Musterset
* Medienset

**So konfigurieren Sie Standard-Viewer**

1. Klicken Sie in der Dropdown-Liste &quot;Einstellungen&quot;auf **Anwendungseinstellungen**.
1. Erweitern Sie im Fenster &quot;Einstellungen&quot;im linken Bereich **Anwendungseinstellungen** > **Viewer**
1. Klicken Sie auf **Standard-Viewer**.
1. Wählen Sie im Fenster „Standard-Viewer“ in der Dropdown-Liste für die einzelnen Asset-Typen den Viewer aus, den Sie mit der Asset-Vorschau verknüpfen möchten.
1. Klicken Sie in der rechten unteren Ecke des Fensters &quot;Standard-Viewer&quot;auf **Speichereinstellungen**.
1. Klicken Sie in der rechten unteren Ecke des Fensters &quot;Einstellungen&quot;auf **Schließen**, um zum Fenster &quot;Asset&quot;zurückzukehren.

## Metadaten-Ansichten {#metadata-views}

*Metadaten* sind standardisierte Informationen zu einem Asset. Mit Metadaten können Sie Ihren Arbeitsablauf optimieren, Ihre Assets organisieren und die Suche verbessern. Dynamic Media Classic unterstützt den Standard IPTC (International Press Telecommunications Council) und den Standard XMP (Extensible Metadata Platform). Vor der Anzeige oder Eingabe von Asset-Metadaten in der Detailansicht können Benutzer im Menü „Metadaten-Ansichten“ den Metadatenfeldersatz auswählen, den sie anzeigen oder zur Beschreibung des Assets verwenden möchten.

Im Lieferumfang von Dynamic Media Classic sind vordefinierte Metadaten-Ansichten enthalten. Administratoren können eigene Metadaten-Ansichten erstellen, die sie bei der Eingabe von Metadaten auswählen können.

### Erstellen einer Metadaten-Ansicht {#creating-a-metadata-view}

1. Klicken Sie auf **Setup** > **Anwendungseinstellungen** > **Metadaten** > **Metadaten-Ansichten**.
1. Klicken Sie auf **„Hinzufügen“**.
1. Geben Sie im Textfeld &quot;Vorgabenname&quot;einen Namen für die Ansicht ein.
1. (Optional) Markieren Sie **Als Standard**, um diese Ansicht als Standard festzulegen, die Benutzern angezeigt wird, wenn sie das Metadatenbedienfeld in der Ansicht &quot;Details&quot;öffnen.
1. (Optional) Wählen Sie **UDF** einschließen, um benutzerdefinierte Felder in die Ansicht einzuschließen. Benutzerdefinierte Felder werden oben im Metadatenbedienfeld in der Detailansicht angezeigt.
1. Wählen Sie die gewünschten Felder für die Ansicht aus (klicken Sie auf **Alle auswählen**, um alle Felder auszuwählen).
1. Klicken Sie auf „**Speichern**“.

   Die ausgewählten Kategorien und Felder für die Ansicht werden im Vorschaubedienfeld angezeigt.

### Verwalten von Metadaten-Ansichten  {#managing-metadata-views}

1. Klicken Sie auf **Setup** > **Anwendungseinstellungen** > **Metadaten** > **Metadaten-Ansichten**.
1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie eine Ansicht aus, um eine Vorschau davon zu erstellen. Die Felder in der Ansicht werden im Vorschaubedienfeld angezeigt.
   * Um eine Ansicht zu bearbeiten, wählen Sie sie aus und klicken Sie dann auf **Bearbeiten**. Wählen Sie dann im Bedienfeld &quot;Vorschau&quot;Feldnamen aus oder heben Sie die Auswahl auf und aktivieren oder deaktivieren Sie die Option **UDF** einschließen.
   * Um eine Ansicht zu löschen, wählen Sie sie aus und klicken Sie dann auf **Löschen**.
   * Um eine Ansicht als Standard festzulegen, wählen Sie sie aus und klicken Sie dann auf **Als Standard** festlegen. Die Standardansicht ist die Ansicht, die Benutzern standardmäßig angezeigt wird, wenn sie ein Asset in der Detailansicht öffnen und zum Metadatenbedienfeld wechseln.

## Metadaten-Vorgaben  {#metadata-presets}

Metadaten-Vorgaben bieten Administratoren eine Möglichkeit, den Assets zugeordnete Metadaten zu kontrollieren und zu regeln. In der Detail-Ansicht kann ein Benutzer Metadaten eines Assets in den zu diesem Zweck bereitgestellten Feldern eingeben. Ein Benutzer kann beispielsweise einen Eigentümernamen, eine Copyrightbeschreibung und eine Adresse eingeben. Um sicherzustellen, dass Benutzer Informationen genau und vollständig eingeben, können Sie Metadaten-Vorgaben erstellen. Wenn Sie in der Detail-Ansicht Metadaten-Vorgaben wählen, werden die Metadatenfelder mit vordefinierten Werten gefüllt. So werden beispielsweise der Eigentümername, die Copyrightbeschreibung und die Adresse automatisch eingegeben.

Erstellen Sie eine Metadaten-Vorgabe für jeden Satz mit Metadatenwerten, die die Benutzer automatisch in der Detail-Ansicht zur Beschreibung eines Assets eingeben können.

### Erstellen oder Bearbeiten einer Metadaten-Vorgabe {#creating-or-editing-a-metadata-preset}

1. Klicken Sie auf **Setup** > **Anwendungseinstellungen** > **Metadaten** > **Metadaten-Vorgaben**.
1. Führen Sie im Anzeigebereich „Metadaten-Vorgaben“ einen der folgenden Schritte aus:

   * Um eine Vorgabe zu erstellen, klicken Sie auf **Hinzufügen**. Geben Sie im Textfeld Name der Metadatenvorlage einen Namen für die Vorgabe ein, klicken Sie auf **Metadaten-Ansichten** und wählen Sie eine Ansicht aus der Dropdown-Liste aus (siehe [Metadaten-Ansichten](application-setup.md#metadata_views)).
   * Um eine vorhandene Vorgabe zu bearbeiten, wählen Sie die Vorgabe in der Liste &quot;Metadaten-Vorgaben&quot;aus und klicken Sie dann auf **Bearbeiten**.

1. Blenden Sie die Überschriften ein, die Sie in die Vorgabe aufnehmen möchten, und geben Sie Werte in die verschiedenen Felder ein, die Sie in die Vorgabe aufnehmen möchten.
1. Klicken Sie auf „**Speichern**“.

   Die ausgewählten Kategorien und Felder für die Vorgabe werden im Vorschaubedienfeld angezeigt.

### Verwalten von Metadaten-Vorgaben  {#managing-metadata-presets}

1. Klicken Sie auf **Setup** > **Anwendungseinstellungen** > **Metadaten** > **Metadaten-Vorgaben**.
1. Führen Sie einen der folgenden Schritte aus:

   * Um eine Vorschau einer Vorgabe anzuzeigen, wählen Sie die entsprechende Vorgabe aus. Die Vorgabeninformationen (Kategorien und Felder) werden im Anzeigebereich „Vorschau“ angezeigt.
   * Um eine Vorgabe zu löschen, wählen Sie die Vorgabe aus und klicken Sie dann auf **Löschen**.

## Benutzerdefinierte Felder {#user-defined-fields}

Ein Medienportal-Administrator bzw. Unternehmensadministrator kann individuelle, benutzerdefinierte Metadatenfelder erstellen. Mit benutzerdefinierten Feldern können Sie Assets in Dynamic Media Classic organisieren. Sie können die Felder bei Bedarf als aktiv markieren. Wenn die Felder aktiviert sind, erscheinen die Namen dieser benutzerdefinierten Metadatenfelder im Metadatenbedienfeld in der Detailansicht. Die Benutzer können Informationen zur Beschreibung der Assets in die benutzerdefinierten Metadatenfelder eingeben. Außerdem können Benutzer ein benutzerdefiniertes Metadatenfeld als Suchkriterium angeben.

Eine effektive Nutzung benutzerdefinierter Metadatenfelder besteht darin, die Aktivierungszeit eines Assets für einen bestimmten Launch oder Ausverkauf zu verzögern. Sie definieren ein Feld &quot;Aktivierung&quot;basierend auf dem Typ *Date*. Anschließend können Sie mit dem Bedienfeld **Metadaten** in der Ansicht **Detail** oder **Datei** > **Informationen bearbeiten** angeben, wann das Asset aktiviert wird. Dynamic Media Classic prüft den Veröffentlichungsstatus eines Assets und den Veröffentlichungsverlauf. Wenn sich der Veröffentlichungsstatus nicht innerhalb der Aktivierung befindet, wird als &quot;Nicht veröffentlicht&quot;angezeigt.

>[!NOTE]
>
>Damit benutzerdefinierte Felder im Metadatenbedienfeld der Detailansicht angezeigt werden, schließen Sie benutzerdefinierte Felder in die Metadaten-Ansichten ein. Wählen Sie im Anzeigebereich „Metadaten-Ansichten“ die Option „UDF einschließen“. Weitere Informationen finden Sie unter [Metadaten-Ansichten](application-setup.md#metadata_views).

>[!NOTE]
>
>Um über eigene, benutzerdefinierte Felder nach Assets zu suchen, klicken Sie auf **Einstellungen** > **Persönliche Einstellungen** und wählen Sie dann **Benutzerdefinierte Felder in Suche einschließen** aus. Siehe [Persönliche Einstellungen](personal-setup.md#personal_setup).

### Erstellen eines benutzerdefinierten Metadatenfelds  {#creating-a-user-defined-metadata-field}

1. Klicken Sie auf **„Einstellungen“** > **„Anwendungseinstellungen“** > **„Metadaten“** > **„Benutzerdefinierte Felder“**.
1. Klicken Sie auf „**Hinzufügen**“.
1. Legen Sie im Dialogfeld „Benutzerdefiniertes Feld“ die gewünschten Optionen fest.

   **** NameGeben Sie einen Namen für das Metadatenfeld ein.

   **** TypWählen Sie eine Option, die den Informationstyp definiert, den Benutzer in das Metadatenfeld eingeben können:

   **** StringEine Textzeichenfolge.

   **Eine** Ganzzahl.

   **Gleitkommazahl** Eine Gleitkommazahl.

   **Ja/** NeinA, Ja/Nein, boolescher Wert.

   **Datum** A. Das Format MM/TT/JJJJ ist zulässig.

   **Dateiname** Der Name einer Datei.

   **** FarbeDer Name einer Farbe.

   **** DimensionDie Breite und Höhe des Assets.

   **** UntypedFür Abwärtskompatibilität. Wählen Sie diese Option nicht aus.

   **Standardwert** ValueOptional geben Sie den Wert ein, den Benutzer mit der größten Wahrscheinlichkeit in das Feld eingeben. Dieser Wert wird als Standardwert für das neue Feld verwendet.

   **Gilt** für: Wählen Sie optional einen Asset-Typ, wenn das Metadatenfeld nur auf einen bestimmten Asset-Typ angewendet werden soll.

   ***Hinweis**: Wählen Sie die Option **Gilt für** sorgfältig aus, da Sie die Option **Gilt für** nicht ändern können, nachdem Sie ein benutzerdefiniertes Feld erstellt haben. Mit Dynamic Media Classic können Sie den Namen, den Typ und den Standardwert eines benutzerdefinierten Felds bearbeiten, nicht jedoch die Einstellung **Gilt für**. *

1. Klicken Sie auf **„Speichern“**, wenn Sie das Metadatenfeld erstellt haben.

### Verwalten von benutzerdefinierten Feldern  {#manage-user-defined-fields}

Im Anzeigebereich „Benutzerdefinierte Felder“ finden Sie Befehle zum Verwalten eigener, benutzerdefinierter Felder.

Benutzerdefinierte Felder können nur von Media Portal-Administratoren und Unternehmensadministratoren verwaltet werden.

Um diesen Bildschirm zu öffnen, klicken Sie auf **„Einstellungen“** > **„Anwendungseinstellungen“** > **„Metadaten“** > **„Benutzerdefinierte Felder“**.

**Bearbeiten eines** FeldsWählen Sie das Feld aus und klicken Sie dann auf  **Bearbeiten**.

**Löschen eines** FeldsWählen Sie das Feld aus und klicken Sie dann auf  **Löschen**.

**Aktivieren Sie** fieldClick, um die Option Aktiv neben dem Namen eines Felds auszuwählen oder die Auswahl aufzuheben. Wenn Sie eine Administratorfunktion in Ihrer Organisation innehaben, wird diese Option eventuell nicht angezeigt. Da diese Option mit MediaPortal in Zusammenhang steht, müssen Sie unter &quot;Persönliche Einstellungen&quot;die Option &quot;MediaPortal-Funktionen anzeigen&quot;auswählen (aktivieren), um die Aktivierungsfelder anzuzeigen.

## Optimieren von Dateien {#optimize-files}

Beim Hochladen von Dateien in Dynamic Media Classic optimiert das System diese für die Datenspeicherung und Veröffentlichung. Wenn das Hochladen jedoch unterbrochen wird, können einige Bilder nicht optimiert werden. In diesem Fall wird die Meldung „Bild wurde noch nicht optimiert“ angezeigt. Als Administrator können Sie jedoch auch diese Dateien optimieren.

Dynamic Media Classic durchsucht Ihre Dateien und optimiert nur die Bilder, die zuvor noch nicht vollständig optimiert wurden.

1. Wählen Sie **Setup** > **Anwendungseinstellungen** und dann &quot;O **Dateien** timisieren&quot;.
1. Geben Sie Informationen für den Optimierungsauftrag ein und klicken Sie auf **Senden**.

   Wenn Sie mit mehr als einem Unternehmen arbeiten, optimieren Sie Dateien, die zu unterschiedlichen Unternehmen gehören, getrennt.

## Stapelsatzvorgaben {#batch-set-presets}

Verwenden Sie die Stapelsatzvorgaben, um automatisch Bildsätze oder Rotationssets zu erstellen, während ein Auftrag ausgeführt wird, um Assets nach Dynamic Media Classic hochzuladen.

Unternehmensadministratoren legen zuerst Namenskonventionen für die Assets fest, die sie in einem Satz gruppieren möchten. Sie können dann eine Stapelsatzvorgabe erstellen, um diese Bilder zu referenzieren. Jede Vorgabe ist ein eindeutig benannter, in sich abgeschlossener Satz von Anweisungen, die definieren, wie der Satz unter Verwendung der Bilder, die den definierten Benennungsregeln im Vorgabenrezept entsprechen, konstruiert werden soll.

Alle aktiven Stapelsatzvorgaben für ein Unternehmen werden im Dialogfeld „Upload-Auftragsoptionen“ aufgelistet, sodass Sie bei jedem Hochladevorgang auswählen können, welche Vorgabe angewendet werden soll. Unternehmensadministratoren sehen alle aktiven und inaktiven Stapelsatzvorgaben. Wenn Sie Dateien hochladen, erstellt Dynamic Media Classic automatisch einen Satz mit allen Dateien, die der definierten Benennungsregel in den aktiven Vorgaben entsprechen.

### Standardbenennung {#default-naming}

Der Unternehmensadministrator erstellt eine Standard-Benennungskonvention, die in einem beliebigen Stapelsatzvorgaben-Rezept verwendet wird. Die in der Definition der Stapelsatzvorgabe verwendete Standardbenennungsregel ist möglicherweise alles, was Ihr Unternehmen benötigt, um Stapelsätze für alle Websites zu generieren. Eine Stapelsatzvorgabe wird erstellt, damit die von Ihnen definierte Standardbenennungsregel verwendet werden kann. Sie können so viele Stapelsatzvorgaben mit alternativen, benutzerdefinierten Benennungsregeln erstellen, wie für einen bestimmten Satz von Inhalten notwendig sind, falls eine Ausnahme für eine unternehmensspezifische Standardbenennung existiert.

Die Einrichtung einer Standardbenennungsregel ist keine Voraussetzung für die Verwendung der Funktionen von Stapelsatzvorgaben. Es hat sich jedoch bewährt, mithilfe der Standardbenennungsregel so viele Elemente Ihrer Benennungsregel wie möglich zu erstellen, die Sie in einem Satz gruppieren möchten, um die Erstellung von Stapelsätzen zu vereinfachen.

1. Klicken Sie auf **Einstellungen** > **Anwendungseinstellungen** > **Stapelsatzvorgaben** > **Standardbenennung**.
1. Wählen Sie **Formular anzeigen** oder **Code anzeigen**, um anzugeben, wie Sie die Informationen zu den einzelnen Elementen anzeigen und eingeben möchten.

   Sie können das Kontrollkästchen „Code anzeigen“ aktivieren, um die Erstellung des regelmäßigen Ausdruckswerts neben Ihren Formularauswahlen anzuzeigen. Sie können diese Werte nach Bedarf eingeben oder ändern. Dies hilft Ihnen bei der Definition der Elemente der Benennungsdefinition, falls Sie aus irgendeinem Grund durch die Formularansicht eingeschränkt werden. Falls Ihre Werte in der Formularansicht nicht analysiert werden können, werden die Formularfelder inaktiv.

   >[!NOTE]
   >
   >Deaktivierte Formularfelder weisen nicht unbedingt auf einen ungültigen regelmäßigen Ausdruck hin. Es gibt keine Möglichkeit zu prüfen, ob Ihre regelmäßigen Ausdrücke korrekt sind. Sie sehen die Ergebnisse des regelmäßigen Ausdrucks, den Sie für jedes Element erstellen, im Anschluss an die Zeile „Ergebnis“. Der vollständige regelmäßige Anschluss wird am unteren Seitenrand angezeigt.

1. Erweitern Sie die Elemente bei Bedarf und geben Sie die zu verwendenden Benennungsregeln ein.
1. Klicken Sie bei Bedarf auf **Hinzufügen**, um einem Element eine weitere Benennungsregel hinzuzufügen. Klicken Sie auf **Entfernen**, um eine Benennungsregel für ein Element zu löschen.
1. Klicken Sie auf **Speichern unter** und geben Sie einen Namen für die Vorgabe ein. Wenn Sie eine vorhandene Vorgabe bearbeiten, klicken Sie auf **Speichern**.

Alternativ können Sie „Code anzeigen“ ohne verfügbare Formularfelder verwenden. In dieser Ansicht können Sie Ihre Benennungsregeldefinitionen vollständig unter Verwendung regelmäßiger Ausdrücke erstellen. 

Zwei Elemente sind zur Definition verfügbar: Treffer und Grundname. Anhand dieser Felder können Sie alle Elemente einer Benennungsregel definieren und denjenigen Teil der Regel identifizieren, mit dem Sie den Satz benennen, der diese Elemente enthält. Die Benennungsregel eines Unternehmens kann eine oder mehrere Zeilen der Definition für jedes dieser Elemente verwenden. Sie können für Ihre spezifische Definition so viele Zeilen wie erforderlich verwenden und sie zu eindeutigen Elementen gruppieren, beispielsweise Elementen für Hauptbild, Farbe, alternative Ansicht und Muster.

### Erstellen einer Stapelsatzvorgabe  {#creating-a-batch-set-preset}

Dynamic Media Classic verwendet Stapelsatzvorgaben, um Assets, die einige allgemeine Informationen oder Inhalte gemeinsam verwenden, in Bildsätzen für die Anzeige in Viewern zu organisieren. Die Stapelsatzvorgabenrezepte werden automatisch zusammen mit den Asset-Importaufträgen ausgeführt, die Sie in Dynamic Media Classic planen.

Verwenden Sie „Stapelsatzvorgaben“ zum Erstellen, Bearbeiten und Verwalten Ihrer Stapelsatzvorgaben. Sie können so viele Stapelsatzvorgaben wie nötig erstellen, um alle benötigten Asset-Importaufträge abzudecken. Es gibt zwei Formen von Stapelsatzvorgabendefinitionen, eine für eine von Ihnen eingerichtete Standardbenennungsregel und eine für benutzerdefinierte Standardbenennungsregeln, die Sie spontan erstellen.

Sie können zum Definieren einer Stapelsatzvorgabe die Formularfeldmethode oder aber die Code-Methode verwenden, welche Ihnen die Verwendung regelmäßiger Ausdrücke gestattet. Ebenso wie bei der Standardbenennung können Sie „Code anzeigen“ zur gleichen Zeit verwenden, wie Sie Definitionen in der Formularansicht vornehmen und mithilfe von regelmäßigen Ausdrücken Ihre Definitionen erstellen. Alternativ können Sie eine der Ansichten deaktivieren, um ausschließlich die eine oder die andere zu verwenden.

Siehe auch [Erstellen einer Stapelsatzvorgabe für die automatische Erstellung eines 2D-Rotationssets](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

**So erstellen Sie eine Stapelsatzvorgabe**

1. Klicken Sie auf **Einstellungen** > **Anwendungseinstellungen** > **Stapelsatzvorgaben** > **Stapelsatzvorgabe**. **Formular anzeigen**, wie in der oberen rechten Ecke der Detailseite angezeigt, ist die Standardansicht.
1. Klicken Sie im Bedienfeld „Vorgabenliste“ auf **Hinzufügen**, um die Definitionsfelder in der Detailansicht auf der rechten Seite des Bildschirms zu aktivieren.
1. Geben Sie in der Detailansicht in das Feld „Vorgabenname“ einen Namen für die Vorgabe ein.
1. Wählen Sie im Dropdown-Menü „Stapelsatztyp“ einen Vorgabentyp aus.

   Um automatisch ein 2D-Rotationsset zu erzeugen, wählen Sie in der Dropdownliste „Stapelsatztyp“ die Option **Multiachsen-Rotationsset**.

1. Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie eine Standard-Benennungskonvention verwenden, die Sie zuvor unter „Anwendungseinstellungen“ > „Stapelsatzvorgaben“ > „Standardbenennung“ eingerichtet haben, erweitern Sie **Asset-Benennungsregeln** und klicken Sie anschließend in der Dropdownliste „Dateibenennung“ auf **Standard**.
   * Um eine Benennungskonvention während der Einrichtung der Vorgabe zu definieren, erweitern Sie **Asset-Benennungsregeln** und klicken Sie anschließend in der Dropdownliste „Dateibenennung“ auf **Standard**.

1. Legen Sie für die Reihenfolge der Sequenz die Reihenfolge der Bilder fest, nachdem das Set in Dynamic Media Classic gruppiert wurde. Die Assets werden standardmäßig in alphanumerischer Reihenfolge angeordnet. Sie können jedoch auch eine durch Kommas getrennte Liste mit regulären Ausdrücken verwenden, um die Reihenfolge anzupassen.
1. Geben Sie für „Satzbenennungs- und -erstellungsregel“ das Suffix bzw. Präfix für den Basisnamen an, den Sie in der Asset-Benennungsregel definiert haben. Legen Sie außerdem fest, wo der Bildsatz in der Dynamic Media Classic-Ordnerstruktur erstellt werden soll.

   Falls Sie eine große Anzahl von Bildsätzen definieren, sollten Sie diese von den Ordnern, die die Assets selbst enthalten, getrennt halten. Zahlreiche Kunden erstellen einen Ordner „Bildsätze“ und weisen die Anwendung an, im Stapelsatz generierte Sätze hier abzulegen.

1. Klicken Sie im Detailbedienfeld auf **Speichern**.

### Erstellen einer Stapelsatzvorgabe für die automatische Erstellung eines 2D-Rotationssets  {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

Sie können den Stapelsatztyp **Multiachsen-Rotationsset** verwenden, um ein „Rezept“ zu erstellen, das die Erstellung von 2D-Rotationssets automatisiert. Für die Gruppierung von Bildern werden die regulären Ausdrücke „Zeile“ und „Spalte“ verwendet, sodass die Bild-Assets im multidimensionalen Array korrekt an der entsprechenden Position ausgerichtet werden.

Siehe auch [Erstellen einer Stapelsatzvorgabe](application-setup.md#creating_a_batch_set_preset).

Es gibt keine Mindest- oder Maximalzahl an Reihen und Spalten, die in einem Multiachsen-Rotationsset vorhanden sein müssen.

Beispiel: Sie möchten ein Multiachsen-Rotationsset mit dem Namen *spin-2dspin* erstellen. Sie haben einen Satz von Rotationsset-Bildern, die drei Zeilen mit 12 Bildern pro Zeile enthalten. Die Bilder haben die folgenden Namen:

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

Mit diesen Informationen können Sie Ihr Stapelsatztyp-Rezept wie folgt erstellen:

![](assets/se_batch_set_recipe.png)

Die Gruppierung für den Teil des gemeinsamen Asset-Namens des Rotationssets wird dem Feld **Übereinstimmung** hinzugefügt (wie hervorgehoben). Der variable Teil des Asset-Namens, der die Zeile und Spalte enthält, wird den Feldern **Zeile** bzw. **Spalte** hinzugefügt.

Wenn das Rotationsset hochgeladen und veröffentlicht wird, aktivieren Sie den Namen des 2D-Rotationssets-Rezepts, das unter **Batchset-Voreinstellungen** im Dialogfeld **Upload-Auftragsoptionen** aufgeführt ist.

**So erstellen Sie eine Stapelsatzvorgabe für die automatische Erstellung eines 2D-Rotationssets**

1. Wählen Sie **Einstellungen** > **Anwendungseinstellungen** > **Stapelsatzvorgaben** > **Stapelsatzvorgabe**. **Formular anzeigen**, wie in der oberen rechten Ecke der Detailseite angezeigt, ist die Standardansicht.
1. Klicken Sie im Bedienfeld „Vorgabenliste“ auf **Hinzufügen**, um die Definitionsfelder in der Detailansicht auf der rechten Seite des Bildschirms zu aktivieren.
1. Geben Sie in der Detailansicht in das Feld „Vorgabenname“ einen Namen für die Vorgabe ein.
1. Wählen Sie im Dropdownmenü „Batch-Settyp“ die Option **Asset-Set**.
1. Wählen Sie in der Dropdownliste „Untertyp“ die Option **Multiachsen-Rotationsset**.
1. Erweitern Sie **Asset-Benennungskonventionen** und klicken Sie in der Dropdownliste „Dateibenennung“ auf **Benutzerdefiniert**.
1. Verwenden Sie die Attribute **Übereinstimmung** und optional **Basisname**, um einen regulären Ausdruck für die Benennung von Bild-Assets zu definieren, aus denen die Gruppierung besteht.

   Ein regulärer Ausdruck für einen genauen Treffer könnte z. B. wie folgt aussehen:

   `(\w+)-\w+-\w+`

1. Erweitern Sie **Zeilen-/Spaltenposition** und definieren Sie anschließend den Namen des Formats für die Position des Bild-Assets innerhalb des 2D-Rotationsset-Arrays.

   Setzen Sie die Zeilen- oder Spaltenposition im Dateinamen in Klammern.

   Ein regulärer Ausdruck für die Zeile könnte beispielsweise wie folgt aussehen:

   `\w+-R([0-9]+)-\w+`

   oder

   `\w+-(\d+)-\w+`

   Ein regulärer Ausdruck für die Spalte könnte wie folgt aussehen:

   `\w+-\w+-C([0-9]+)`

   oder

   `\w+-\w+-C(\d+)`

   Beachten Sie, dass dies nur Beispiele sind. Sie können reguläre Ausdrücke Ihren Bedürfnissen entsprechend erstellen.

   >[!NOTE]
   >
   >Wenn anhand der Kombination aus regulärem Ausdruck für Zeile und Spalte diese Position des Assets innerhalb des multidimensionalen Rotationsset-Arrays nicht ermittelt werden kann, wird das Asset nicht dem Set hinzugefügt und ein Fehler wird protokolliert.

1. Geben Sie für „Satzbenennungs- und -erstellungsregel“ das Suffix bzw. Präfix für den Basisnamen an, den Sie in der Asset-Benennungsregel definiert haben. Legen Sie außerdem fest, wo der Bildsatz in der Dynamic Media Classic-Ordnerstruktur erstellt werden soll.

   Falls Sie eine große Anzahl von Bildsätzen definieren, sollten Sie diese von den Ordnern, die die Assets selbst enthalten, getrennt halten. Zahlreiche Kunden erstellen einen Ordner „Bildsätze“ und weisen die Anwendung an, im Stapelsatz generierte Sätze hier abzulegen.

1. Klicken Sie im Detailbedienfeld auf **Speichern**.
1. Gehen Sie beim Hochladen und Veröffentlichen des Rotationssets wie gewohnt vor und stellen Sie sicher, dass Sie den Namen des 2D-Rotationssets im Dialogfeld „Auftragsoptionen“ unter „Stapelsatzvorgaben“ aktivieren.

>[!MORELIKETHIS]
>
>* [Anzeigen einer Asset-Vorschau](previewing-asset.md#previewing_an_asset)
>* [Einstellen von Bildvorgaben](setting-image-presets.md#setting_up_image_presets)
>* [Anzeigen, Hinzufügen und Exportieren von Metadaten](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [Überprüfen von Auftragsdateien](checking-job-files.md#checking_job_files)

