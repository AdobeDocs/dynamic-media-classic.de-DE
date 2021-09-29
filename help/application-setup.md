---
title: Anwendungseinstellungen
description: Erfahren Sie, wie Sie den Anwendungsbereich von Adobe Dynamic Media Classic einrichten und konfigurieren. Im Bereich "Anwendung"können Sie allgemeine Einstellungen eingeben, Bild-, Viewer- und Videokodierungsvorgaben erstellen, Standard-Viewer und -Metadaten definieren, Veröffentlichungseinstellungen und SEO-Einstellungen für Videos festlegen. Sie können den Bereich auch verwenden, um Stapelsatzvorgaben einzurichten, um die Erstellung von 2D-Rotationssets zu automatisieren.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
source-git-commit: 0e2271924f49edd6ac424bb7cbd56af1e6afd817
workflow-type: tm+mt
source-wordcount: '11003'
ht-degree: 43%

---

# Anwendungseinstellungen{#application-setup}

Auf den Seiten &quot;Anwendungseinstellungen&quot;können Sie allgemeine Einstellungen eingeben, Bildvorgaben, Videokodierungsvorgaben, Viewer-Vorgaben erstellen oder Standard-Viewer und Metadaten definieren. Sie können Stapelsatzvorgaben einrichten, um auch die Erstellung von 2D-Rotationssets (z. B.), Veröffentlichungseinstellungen und SEO-Einstellungen für Videos zu automatisieren.

>[!NOTE]
>
>Nur Adobe Dynamic Media Classic-Administratoren können die Einstellungen auf den Seiten &quot;Anwendungseinstellungen&quot;ändern.

## Allgemeine Einstellungen {#general-settings}

Um die Seite &quot;Allgemeine Programmeinstellungen&quot;zu öffnen, navigieren Sie in der Symbolleiste für globale Navigation zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Einstellungen]**.

### Server

Bei der Kontoerstellung stellt Adobe Dynamic Media Classic automatisch die zugewiesenen Server für Ihr Unternehmen bereit. Auf Grundlage dieser Server werden URL-Zeichenfolgen für Ihre Websites und Anwendungen erstellt. Diese URL-Aufrufe sind spezifisch für Ihr Konto.

Siehe auch [Testen des Secure Testing Service](testing-assets-making-them-public.md#testing_the_secure_testing_service).

* **[!UICONTROL Veröffentlichter Server-Name]**  - Dieser Server ist der Live Content Deliver Network (CDN)-Server, der in allen systemgenerierten URL-Aufrufen verwendet wird, die für Ihr Konto spezifisch sind. Ändern Sie diesen Servernamen nur, wenn Sie von einem Support-Mitarbeiter der Adobe Dynamic Media Classic angewiesen wurden.

* **[!UICONTROL Origin Server Name]**  - Dieser Server wird nur für Qualitätssicherungstests verwendet. Ändern Sie diesen Servernamen nur, wenn Sie von einem Support-Mitarbeiter der Adobe Dynamic Media Classic dazu aufgefordert werden.

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by an Adobe DynamicMedia Classic support technician. -->

* **[!UICONTROL Test&amp;Target-Server-Name]**  - Ihre Test&amp;Target-URL, bis einschließlich .com. Anweisungen zum Abrufen dieser URL finden Sie unter Integrieren von [!DNL Adobe Dynamic Media Classic] mit [!DNL Adobe Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL iOS Streaming Server Name]**  - Die URL zu Ihrem  [!DNL Adobe Dynamic Media Classic] iOS-Streaming-Server. Dieser Server liefert Streaming-Video für iOS-basierte Geräte über das HTTP-Protokoll.

* **[!UICONTROL Servername für progressives Video]** : Die URL zu Ihrem  [!DNL Adobe Dynamic Media Classic] progressiven Videoserver. Dieser Server liefert Progressive Video über das HTTP-Protokoll.

* **[!UICONTROL URL für unveröffentlichte Assets anzeigen]**  - Wählen Sie diese Option, wenn Sie eine URL bei der Vorschau eines Assets anzeigen möchten, unabhängig davon, ob es veröffentlicht wurde oder nicht.  [!DNL Adobe Dynamic Media Classic] Diese Option ist nicht verfügbar. Falls das Asset noch nicht veröffentlicht wurde, funktioniert die URL nicht. Sie können jedoch die URL für Planungs- oder organisatorische Zwecke verwenden.

<!-- **Allow AIR install** Select this option to allow users to download Adobe Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the web version of Adobe Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Adobe Dynamic Media Classic AIR. Adobe Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL Vorlage für CDN-Invalidierung]**  - Gibt die Vorlage an, die zur Invalidierung des CDN (Content Delivery Network)-Cache verwendet wird.

   Angenommen, Sie geben eine Bild-URL (einschließlich Bildvorgaben oder Modifikatoren) ein, die auf `<ID>` verweist, anstatt auf eine bestimmte Bild-ID wie im folgenden Beispiel:

   `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

   Wenn die Vorlage nur `<ID>` enthält, füllt Adobe Dynamic Media Classic `https://<server>/is/image` aus, wobei `<server>` der Veröffentlichungsservername ist, der in den allgemeinen Einstellungen definiert ist.

   Wenn Sie die Vorlage für CDN-Invalidierung festlegen, wählen Sie ein Bild mit dem Namen Backpack_B aus und gehen Sie dann zu **[!UICONTROL Datei]** > **[!UICONTROL Ungültiges CDN]**, was zu der folgenden generierten URL in der Benutzeroberfläche für CDN-Invalidierung führt:

   `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

   Wählen Sie im URL-Listenfeld **[!UICONTROL Weiter]** aus, um den Cache für diesen spezifischen Bild-URL-Aufruf zu löschen. Sie können URLs auch hinzufügen, indem Sie sie in das URL-Listenfeld eingeben oder einfügen. Sie müssen die Vorlage nicht vorab festlegen.

   Nachdem Sie Ihre Vorlage für CDN-Invalidierung ausgewählt und eine Ungültigmachen-CDN-Anfrage gestellt haben, wird in der Benutzeroberfläche ein Indikator angezeigt. Sie erhalten eine Schätzung, wie lange es dauert, den Cache zu leeren.

   Wenn in Adobe Dynamic Media Classic mehrere Bilder ausgewählt sind, wenn Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Ungültiges CDN]** navigieren, wird jedes Bild in der gespeicherten Vorlagen-URL referenziert. Daher können Sie eine Vorlage für CDN-Invalidierung definieren, die auf jede URL verweist, auf die auf Ihrer Website verwiesen wird (z. B. Produktdetails und Suchergebnisse). Wenn Sie dann mindestens ein Bilder zur Ungültigmachung aus dem Cache auswählen, füllen die URLs die Oberfläche automatisch aus.

   Siehe [Inhalts-Caching](dmc-platform-overview.md#content_caching).

   Siehe [Erneut veröffentlichte Assets und CDN-Verzögerungen](publishing-files.md#republished_assets_and_cdn_delays).

### Durchsuchen

* **[!UICONTROL Projekte anzeigen]**  - Bestimmt, ob Projekte als Mittel zur Organisation Ihrer Adobe Dynamic Media Classic-Assets verfügbar sind. Siehe Verwalten der Arbeit mithilfe von Projekten.

* **[!UICONTROL Beispiel-eVideo-Inhalt anzeigen]**  - Aktivieren oder Deaktivieren der Anzeige von eVideo-Beispielinhalten.

* **[!UICONTROL Erzeugten Inhalt anzeigen]**  - Zeigt in Ordnern den Inhalt an, der von einem Asset generiert wurde. Wenn beispielsweise eine PDF-Datei beim Hochladen gerastert wird, erstellt Adobe Dynamic Media Classic für jede Seite in der Original-PDF-Datei ein Bild. Wenn die Option „Generierten Inhalt anzeigen“ aktiviert ist, erscheint jedes beim Hochladen der Original-PDF generierte Bild zusammen mit der PDF in dem Ordner, in den die PDF hochgeladen wurde.

* **[!UICONTROL Kodierte Videos anzeigen]**  - standardmäßig deaktiviert (aus).

   Wenn Sie Videos in Adobe Dynamic Media Classic suchen und suchen möchten, ohne durch zahlreiche kodierte Varianten desselben Videos navigieren zu müssen, lassen Sie diese Option deaktiviert (Standard). Es werden nur die Miniaturansicht des Übergeordneten Videos (das Quellvideo, das Sie hochgeladen und zum Erstellen der Varianten verwendet haben) und die Miniaturansicht des übergeordneten adaptiven Videosets (das die untergeordneten Varianten des kodierten Videosets enthält) angezeigt.

   Vom Mastervideo oder dem adaptiven Videoset aus können Sie jedoch weiterhin auf einzelne kodierte Videos zugreifen. Doppelklicken Sie hierzu auf das Videominiaturbild, um die Detailansicht zu öffnen. Wählen Sie dann **[!UICONTROL Kodierte Videos]** im rechten Bereich aus, damit Sie auf alle untergeordneten Videos zugreifen können.

   Sie können auch **[!UICONTROL Datei]** > **[!UICONTROL Neu verarbeiten]** aufrufen, um kodiertere &quot;untergeordnete&quot;Videos direkt aus einem adaptiven Videoset zu erstellen. Adobe Dynamic Media Classic findet automatisch das &quot;übergeordnete&quot;Übergeordnete Video des adaptiven Videosets und verwendet es als Quellvideo zur Transkodierung. Nachdem Sie die neuen, individuell kodierten Videos gespeichert haben, werden sie jedoch nicht angezeigt, wenn Sie nach ihnen suchen. Sie sind jedoch weiterhin über die Registerkarte „Kodierte Videos“ in der Detailansicht verfügbar.

   Siehe [Hochladen und Transkodieren von Videos](uploading-encoding-videos.md#uploading_and_encoding_videos).

   Um auch im Rahmen einer Suche weiterhin auf alle verschlüsselten Videoableitungen zugreifen zu können, aktivieren Sie die Option **[!UICONTROL „Kodierte Videos anzeigen“]**.

   Das Menü „Erstellen“ enthält bestimmte Aktionen, die nur (oder optional) mit einzelnen Videos verwendet werden. Daher müssen alle kodierten Videoableitungen angezeigt werden, aus denen Sie auswählen können, unabhängig davon, wie Sie die Option **[!UICONTROL „Kodierte Videos anzeigen“]** eingestellt haben. Zu den Build-Aktionen, die die Einstellung **[!UICONTROL Kodierte Videos anzeigen]** überschreiben, gehören **[!UICONTROL Adaptive Videosets]** und **[!UICONTROL eCatalog]**.

   >[!NOTE]
   >
   >Wenn Sie Ihre Video-Assets nicht mit Adobe Dynamic Media Classic hochgeladen und kodiert haben, zeigt Adobe Dynamic Media Classic alle kodierten Videos an, selbst wenn diese Option deaktiviert ist.

* **[!UICONTROL Schaltfläche]**  Unterordner aktualisieren anzeigen - Aktivieren oder Deaktivieren der Anzeige der Schaltfläche Aktualisieren der Unterordner.

### Adobe Dynamic Media Classic FTP-Konto

* **[!UICONTROL Server]**  - Listet Ihren FTP-Konto-Server auf.

* **[!UICONTROL Benutzername]**  - Listet Ihren FTP-Konto-Benutzernamen auf.

### Zur Anwendung hochladen

* **[!UICONTROL Bilder überschreiben]**  - Adobe Dynamic Media Classic lässt zwei Dateien mit demselben Namen nicht zu. Die Adobe Dynamic Media Classic ID jedes Elements (der Bildname ohne Dateinamenerweiterung) muss eindeutig sein. Aufgrund dieser Regel enthält das Dialogfeld „Hochladen“ die Option „Überschreiben“. Die genaue Wirkung dieser Option hängt von der Einstellung der Option „Bilder überschreiben“ ab. Sie legen damit fest, was beim Hochladen von Ersatzbildern geschieht – die Ersatzbilder können die Originalbilder ersetzen oder zu Duplikaten werden. Duplikate werden durch Anhängen einer Ziffer umbenannt („Sessel.tif“ würde beispielsweise zu „Sessel-1.tif“). Die Optionen wirken sich auf Bilder aus, die in einen vom Originalspeicherort abweichenden Ordner hochgeladen werden bzw. die eine andere Dateierweiterung haben als das Original (beispielsweise JPG, TIF oder PNG). (Siehe Verwenden der Option „Bilder überschreiben“.)

   * **[!UICONTROL Im aktuellen Ordner Bilder mit demselben Namen und derselben Erweiterung überschreiben]**  - Diese Option ist die strengste Ersetzungsregel. Das Ersatzbild muss in den Ordner des Originalbilds hochgeladen werden und dieselbe Dateierweiterung haben wie das Originalbild. Wenn diese Voraussetzungen nicht erfüllt sind, wird ein Duplikat erstellt.

   * **[!UICONTROL Im aktuellen Ordner Assets mit ident. Namen unabhängig von Erweiterung]**  überschreiben - Erfordert das Hochladen des Ersatzbilds in denselben Ordner wie das Original. Die Dateinamenerweiterung kann jedoch vom Original abweichen. Beispiel: „Sessel.tif“ ersetzt die Datei „Sessel.jpg“.

   * **[!UICONTROL In belieb. Ordner Assets mit ident. Namen/Erweiterung]**  überschreiben - Erfordert, dass das Ersatzbild dieselbe Dateierweiterung wie das Originalbild hat (beispielsweise muss chair.jpg die Datei &quot;chair.jpg&quot;ersetzen, nicht jedoch die Datei &quot;chair.tif&quot;). Sie können das Ersatzbild jedoch in einen anderen Ordner hochladen als den, in dem sich das Original befindet. Das hochgeladene Bild bleibt dann im neuen Ordner; die Datei befindet sich also nicht mehr am ursprünglichen Speicherort.

   * **[!UICONTROL In einem beliebigen Ordner Assets mit ident. Namen unabhängig von Erweiterung]**  überschreiben - Diese Option ist die am wenigsten einschränkende Ersetzungsregel. Sie können ein Ersatzbild in einen anderen Ordner hochladen als den, in dem sich das Originalbild befindet, und eine Datei mit einer anderen Dateierweiterung verwenden, um die Originaldatei zu ersetzen. Wenn sich die Originaldatei in einem anderen Ordner befindet, bleibt das Ersatzbild in dem neuen Ordner, in den es hochgeladen wurde.

* **[!UICONTROL Veröffentlichung beibehalten]**  - Gibt an, ob bei einem in Adobe Dynamic Media Classic hochgeladenen Ersatzbild die Einstellung &quot;Veröffentlichungsbereit&quot;für das ersetzte Bild beibehalten wird oder die Einstellung beim Hochladen festgelegt wird.

* **[!UICONTROL Standardfarbprofile]**  - Gibt die Farbprofile an, die beim Hinzufügen von CMYK-Bildern als Teil der Optionen für Standardfarbprofile angewendet werden.

* **[!UICONTROL Standardmäßige Upload-Optionen]**  - Öffnet das Dialogfeld &quot;Upload-Auftragsoptionen&quot;, in dem Sie standardmäßige Upload-Optionen festlegen können. Informationen zu diesen Optionen finden Sie unter Upload-Optionen.

### Imagemap-Editor, an Anwendung

* **[!UICONTROL Standard-HREF für Imagemaps]**  - Definiert die Standard-URL, die für die HREF-Spalte im Bild-Mapping verwendet wird. Diese URL ist die Standard-URL, die beim Erstellen von Imagemaps angezeigt wird.

* **[!UICONTROL Standard-Bildzuordnungsvorlage]**  - Definiert das standardmäßige JavaScript für die HREF-Vorlage im Bild-Mapping. Sie können hier benutzerdefinierten Code festlegen, der immer dann ausgeführt wird, wenn Sie eine Imagemap auswählen.

### Andere Einstellungen, an Anwendung

* **[!UICONTROL Papierkorb kann Warnhinweise bereinigen]**  - Assets im Papierkorb werden automatisch innerhalb von sieben Tagen entfernt. Wählen Sie „E-Mails senden, bevor Elemente im Papierkorb automatisch gelöscht werden“, wenn Unternehmensadministratoren vier Tage vor dem dauerhaften Löschen von Assets im Papierkorb eine Benachrichtigung erhalten sollen. Siehe Verwalten des Ordners „Papierkorb“.

## Verwenden Sie die Option Bilder überschreiben . {#using-the-overwrite-images-option}

Adobe Dynamic Media Classic lässt zwei Dateien mit demselben Namen nicht zu. Die Adobe Dynamic Media Classic ID jedes Elements (der Bildname ohne Dateinamenerweiterung) muss eindeutig sein. Aufgrund dieser Regel enthält das Dialogfeld „Hochladen“ die Option „Bilder überschreiben“. Die genaue Wirkung dieser Option hängt von einer Einstellung für die Adobe Dynamic Media Classic Interne Einstellungen jedes Unternehmens ab.

Wenn Sie zuvor Bilder hochgeladen und dann die Originaldateien geändert (oder ersetzt) haben, gibt die Option Überschreiben an, wie Adobe Dynamic Media Classic die Bilder ersetzt. Informationen über das Bild bleiben unverändert, aber das neue Bild ersetzt das alte. Wenn der Ordner auch Bilder enthält, die sich noch nicht in Adobe Dynamic Media Classic befinden, werden diese Bilder hinzugefügt.

Verwenden Sie diese Option, wenn von Ihnen hochgeladene Bilder geändert wurden, der Verweis auf die Bilder jedoch gleich bleibt. Das Überschreiben ist außerdem beim Hochladen und Extrahieren von Adobe® PDF-Dateien nützlich. Passen Sie die ICC-Farbprofiloptionen im Dialogfeld &quot;Hochladen&quot;an und laden Sie sie mithilfe der Funktion &quot;Überschreiben&quot;erneut hoch, um festzulegen, wie Adobe Dynamic Media Classic *das Bild rips* schneidet.

Die Adobe Dynamic Media Classic IDs, die für den Zugriff auf Bilder von den Produktionsservern verwendet werden, werden von den Bilddateinamen abgeleitet. Die Verwendung von Groß- und Kleinbuchstaben im Dateinamen ist wichtig, sowohl beim Ersetzen vorhandener Dateien als auch für die Adobe Dynamic Media Classic IDs, die für den Zugriff auf das Bild verwendet werden. Achten Sie darauf, dass Dateinamen Groß- und Kleinbuchstaben enthalten, bevor Sie sie in Adobe Dynamic Media Classic hochladen, um die Adobe von Dynamic Media Classic-IDs zu vermeiden, die sich nur im Fall für dasselbe Bild unterscheiden.

Wenn Sie diese Option deaktivieren, werden alle Bilder, die mit vorhandenen Bildern übereinstimmende Dateinamen haben, als Duplikate betrachtet und daher nicht hinzugefügt.

## Bildvorgaben {#image-presets}

In diesem Anzeigebereich können Bildvorgaben erstellt und bearbeitet werden. Anhand von Bildvorgaben kann Adobe Dynamic Media Classic Bilder dynamisch in unterschiedlichen Größen desselben Übergeordneten Bildes bereitstellen. Jede Bildvorgabe stellt eine vordefinierte Zusammenstellung von Größen- und Formatierungsbefehlen zum Anzeigen des Bildes dar. Wenn Sie eine Bildvorgabe erstellen, wählen Sie eine Größe für die Bildbereitstellung aus. Sie wählen auch Formatierungsbefehle aus, damit das Erscheinungsbild des Bildes optimiert wird, wenn das Bild zur Anzeige bereitgestellt wird.

Administratoren können Vorgaben für das Exportieren von Assets erstellen. Benutzer können beim Exportieren von Bildern eine Vorgabe auswählen, die auch Bilder entsprechend den vom Administrator festgelegten Spezifikationen neu formatiert.

Um den Bildschirm &quot;Bildvorgabe&quot;zu öffnen, navigieren Sie in der Symbolleiste für globale Navigation zu **[!UICONTROL Setup]** > **[!UICONTROL Bildvorgaben]**.

Siehe [Intelligente Bildbearbeitung](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic).

### Erstellen und Bearbeiten von Bildvorgaben {#creating-and-editing-image-presets}

1. Gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Bildvorgaben]**.
1. Erstellen Sie eine Vorgabe oder beginnen Sie mit einer vorhandenen:

   * **Bildvorgabe erstellen**  - Wählen Sie  **[!UICONTROL Hinzufügen]** aus.
   * **Erstellen einer Bildvorgabe aus einer vorhandenen Vorgabe**  - Wählen Sie die Bildvorgabe aus, die der Bildvorgabe am ehesten entspricht, die Sie erstellen möchten, und wählen Sie dann  **[!UICONTROL Bearbeiten]** aus.

1. Geben Sie auf der Seite Vorgabe hinzufügen (oder bearbeiten) einen Namen für die Vorgabe ein.
1. Legen Sie die gewünschten Einstellungen für die Vorgabe fest. 

   Siehe [Bildvorgabeoptionen](application-setup.md#image_preset_options).

1. Wählen Sie **[!UICONTROL Save]** oder, wenn Sie mit einer vorhandenen Vorgabe begonnen haben, **[!UICONTROL Save As]**.
1. Um eine Vorschau der Vorgabe mit Ihrem eigenen Bild anzuzeigen, wählen Sie **[!UICONTROL Durchsuchen]** und dann ein Bild aus. Um eine Vorschau mit dem Standardbild anzuzeigen, wählen Sie **[!UICONTROL Zurücksetzen]** aus.

Sie können eine Bildvorgabe bearbeiten, indem Sie ihren Namen auf dem Bildschirm &quot;Bildvorgaben&quot;auswählen und dann **[!UICONTROL Bearbeiten]** auswählen. Um eine Bildvorgabe zu löschen, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Löschen]**.

### Optionen für Bildvorgaben {#image-preset-options}

Der Anzeigebereich „Vorgabe hinzufügen“ bzw. „Vorgabe bearbeiten“ bietet folgende Optionen zum Erstellen bzw. Bearbeiten von Bildvorgaben:

* **[!UICONTROL Vorgabenname]**  - Geben Sie einen beschreibenden Namen ohne Leerzeichen ein. Um Benutzer bei der Identifizierung dieser Bildvorgabe zu unterstützen, fügen Sie die Bildgrößenspezifikation in den Namen ein.

* **[!UICONTROL Breite und Höhe]**  - Geben Sie die Größe in Pixel an, in der das Bild bereitgestellt wird.

* **[!UICONTROL Format]**  - Wählen Sie im Menü ein Format aus. Bei Auswahl des Formats GIF, JPEG, PDF oder TIFF werden weitere Optionen angezeigt:

   * GIF-Farbquantisierungsoptionen

      * **[!UICONTROL Typ]**  - Wählen Sie Adaptiv (Standard), Web oder Macintosh aus. Wenn Sie **[!UICONTROL GIF mit Alpha]** auswählen, ist die Option &quot;Macintosh&quot;nicht verfügbar.

      * **[!UICONTROL Dither]** : Wählen Sie Diffus oder Aus.

      * **[!UICONTROL Anzahl Farben]**  - Ziehen Sie den Regler, um 2-255 einzugeben.

      * **[!UICONTROL Farbliste]**  - Geben Sie eine kommagetrennte Liste ein. Geben Sie beispielsweise für Weiß, Grau und Schwarz `000000,888888,ffffff` ein.
   * JPEG-Optionen

      * **[!UICONTROL Qualität]**  - Steuert die JPEG-Komprimierungsstufe. Diese Einstellung wirkt sich sowohl auf die Dateigröße als auch die Bildqualität aus. Die JPEG-Qualitätsskala ist 1-100.

      * **[!UICONTROL JPG-Chrominanz-Downsampling aktivieren]** : Da das Auge weniger empfindlich gegenüber hochfrequenten Farbinformationen als gegenüber hochfrequenter Luminanz ist, teilen JPEG-Bilder Bildinformationen in Luminanz und Farbkomponenten. Bei der Komprimierung eines JPEG-Bildes behält die Leuchtdichtekomponente die volle Auflösung, während für die Farbkomponenten ein Downsampling, d. h. eine Mittelwerterstellung für Pixelgruppen, ausgeführt wird. Obwohl das Datenvolumen beim Downsampling um die Hälfte oder ein Drittel reduziert wird, ist die auftretende Qualitätsminderung kaum wahrnehmbar. Downsampling kann nicht auf Graustufenbilder angewendet werden. Mit dieser Technik wird der Komprimierungsgrad, der für Bilder mit hohem Kontrast (z. B. Bilder mit überlappendem Text) sinnvoll ist, reduziert.
   * PDF- und TIFF-Optionen

      * **[!UICONTROL Komprimierung]**  - Wählen Sie einen Komprimierungsalgorithmus.



* **[!UICONTROL Farbraum]**  - Wählen Sie einen Farbraum aus.

* **[!UICONTROL Scharfzeichnen]**  - Wählen Sie die Option Einfaches Scharfzeichnen aktivieren aus, um einen einfachen Scharfzeichnungsfilter auf das Bild anzuwenden, nachdem die Skalierung abgeschlossen ist. Wenn ein Bild in einer anderen Größe verschwommen angezeigt wird, kann dieser Effekt durch Scharfzeichnen kompensiert werden.

   Weitere Informationen zu Scharfzeichnen, Resample-Modi und Unschärfemaske finden Sie unter [Scharfzeichnen eines Bildes](sharpening-image.md#sharpening_an_image).

* **[!UICONTROL Resamplingmodus]** : Wählen Sie eine Option für den Resamplingmodus. Mit diesen Optionen wird ein Bild beim Downsampling scharfgezeichnet:

* **[!UICONTROL B-Linear]**  - Die schnellste Resampling-Methode; einige Aliasing-Artefakte sind sichtbar.

* **[!UICONTROL Bikubisch]**  - Erhöht die CPU-Auslastung auf dem Image-Server, liefert jedoch schärfere Bilder mit weniger deutlichen Aliasing-Artefakten.

* **[!UICONTROL Scharf2]**  - Kann etwas schärfere Ergebnisse als die bikubische Option erzeugen, ist jedoch CPU-intensiver auf dem Image-Server.

* **[!UICONTROL Trilinear]**  - Verwendet sowohl höhere als auch niedrigere Auflösungen, sofern verfügbar; wird nur empfohlen, wenn das Aliasing ein Problem darstellt. Bei dieser Methode wird die JPEG-Dateigröße durch Reduzierung der Hochfrequenzdaten verringert.

* **[!UICONTROL Unschärfemaske]**  - Wählen Sie diese Optionen zur Feinabstimmung der Scharfzeichnung:

* **[!UICONTROL Betrag]**  - Steuert den auf die Kantenpixel angewendeten Kontrastwert. Der Standardwert ist 1,0. Für Bilder mit höherer Auflösung können Sie ihn auf bis zu 5,0 erhöhen. Sie können sich die Auswirkung der Option „Betrag“ wie ein Maß für die Filterintensität vorstellen.

* **[!UICONTROL Radius]**  - Bestimmt die Anzahl der Pixel um die Kantenpixel, die sich auf die Scharfzeichnung auswirken. Geben Sie für Bilder mit hoher Auflösung Werte zwischen 1 und 2 ein. Bei einem geringeren Wert werden nur die Kantenpixel scharfgezeichnet, während bei einem hohen Wert ein breiterer Pixelbereich scharfgezeichnet wird. Der richtige Wert hängt von der Größe des Bilds ab.

* **[!UICONTROL Schwellenwert]**  - Bestimmt den Kontrastbereich, der bei Anwendung des Filters &quot;Unschärfemaske&quot;ignoriert werden soll. Anders ausgedrückt legt diese Option fest, wie stark sich die scharfgezeichneten Pixel von dem sie umgebenden Bereich unterscheiden müssen, damit sie als Kantenpixel erkannt und scharfgezeichnet werden. Damit kein Bildrauschen entsteht, sollten Sie mit Werten zwischen 0,02 und 0,2 experimentieren. Beim Standardwert 6 werden alle Pixel im Bild scharfgezeichnet.

* **[!UICONTROL Farbraum]**  - Bestimmt, ob das Bild den Raum verwendet, in dem das Bild erstellt wurde, in der Regel RGB (Original) oder einen Luminanzraum (Intensität).

* **** ColorChoose these options:

* **[!UICONTROL Ausgabefarbprofil]**  - Wählen Sie  **[!UICONTROL Use]** Defaultor aus einem der ICC-Farbprofile, die in der Adobe Dynamic Media Classic verfügbar sind.

   Siehe auch [ICC-Profile](icc-profiles.md#icc_profiles).

* **[!UICONTROL Rendering Intent]**  - Wählen Sie eine Option aus, wenn Sie den standardmäßigen Rendering-Intent des Farbprofils überschreiben möchten. Verwenden Sie diese Option, wenn eines der standardmäßigen ICC-Profile der Zielfarbraum einer Farbkonvertierung ist. Oder ein Ausgabegerät (Drucker oder Monitor) ist durch dieses Profil gekennzeichnet und die angegebene Rendering-Absicht gilt für dieses Profil.

* **[!UICONTROL Profil einbetten]**  - Wählen Sie diese Option aus, damit dieses Profil verwendet wird, wenn Sie dieses Bild in Adobe® Photoshop® öffnen.

* **[!UICONTROL Druckauflösung]**  - Wählen Sie eine Auflösung zum Drucken dieses Bildes aus. Der Standardwert beträgt 72 Pixel.

* **[!UICONTROL URL-Modifikatoren]**  - Wenn Sie lieber die URL-Modifikatoren angeben möchten, die Ihre Bildvorgabe definieren, als die Einstellungen, geben Sie hier die Modifikatoren ein.

* **[!UICONTROL Beispiel-Bild-URL]** : Listet die &quot;rohe&quot;URL-Zeichenfolge auf, die der Dynamic Media-Bildserver verwendet, um Bilder mit der Bildvorgabe bereitzustellen, die Sie hinzufügen oder bearbeiten. Diese URL-Zeichenfolge codiert alle Formateinstellungen, die Sie im Anzeigebereich „Vorgabe hinzufügen“ bzw. „Vorgabe bearbeiten“ auswählen.

### Bearbeiten, Entfernen oder Deaktivieren von Bildvorgaben {#editing-removing-or-deactivating-an-image-preset}

1. Gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Bildvorgaben]**.
1. Wählen Sie im Anzeigebereich „Bildvorgaben“ eine Vorgabe aus der Tabelle aus und führen Sie dann einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Bearbeiten]** und geben Sie dann im Dialogfeld &quot;Vorgabe bearbeiten&quot;neue Optionen an.
   * Wählen Sie **[!UICONTROL Löschen]** aus, um die Vorgabe aus der Liste zu entfernen.
   * Deaktivieren Sie das Kontrollkästchen **[!UICONTROL Aktiv]** neben einem Vorgabennamen, wenn Sie ihn aus der gesamten Adobe Dynamic Media Classic-Benutzeroberfläche für Media Portal-Benutzer entfernen möchten.

## Aktivieren oder Deaktivieren von adaptiven Videovorgaben {#activating-or-deactivating-adaptive-video-presets}

Adobe Dynamic Media Classic bietet Vorgaben für die adaptive Videokodierung. Es handelt sich dabei um eine Masterliste von Vorgaben, in der die Vorgaben für adaptive Videos im Format 16:9 und 4:3 in einer Gruppe zusammengefasst sind. Diese vordefinierten Vorgaben enthalten die am häufigsten verwendeten Kodierungseinstellungen und sind für die Wiedergabe auf Mobilgeräten, Tablets und Desktops optimiert. 

Nur Vorgaben für die adaptive Videokodierung sind standardmäßig aktiviert (bzw. „eigeschaltet“). Sie können sie bei Bedarf deaktivieren. Deaktivierte „Adaptive Video“-Voreinstellungen stehen im eVideo-Abschnitt des Dialogfelds „Upload-Auftragsoptionen“ nicht zur Auswahl. 

Siehe [Hochladen und Kodieren von Videos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**So aktivieren und deaktivieren Sie adaptive Video-Vorgaben:**

1. Navigieren Sie in der rechten oberen Ecke der Adobe Dynamic Media Classic zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Videovorgaben]** > **[!UICONTROL Adaptive Videovorgaben]**.
1. Wenn Sie eine Vorgabe aus der Liste „eVideo-Optionen“ im Dialogfeld „Upload-Auftragsoptionen“ entfernen möchten, deaktivieren Sie auf der Seite „Adaptive Video-Vorgaben“ das Kontrollkästchen neben dem Vorgabenamen.
1. Wählen Sie **[!UICONTROL Close]** aus.

## Video-Vorgaben zum Kodieren von Videodateien {#video-presets-for-encoding-video-files}

Um eine Kodierungsvorgabe auszuwählen, wählen Sie rechts unten auf der Seite &quot;Hochladen&quot;die Option **[!UICONTROL Auftragsoptionen]** aus. Erweitern Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die eVideo-Optionen und wählen Sie die gewünschten Videokodierungsvorgaben aus.

>[!NOTE]
>
>Mit Ausnahme von &quot;Adaptives Video&quot;, das standardmäßig aktiviert ist, können Sie nicht alle anderen Vorgaben für adaptive Videos oder einzelne Videokodierung im Dialogfeld &quot;Upload-Auftragsoptionen&quot;sehen. Adobe Dynamic Media Classic-Administratoren bestimmen, welche Videokodierungsvorgaben im Dialogfeld &quot;Upload-Auftragsoptionen&quot;angezeigt werden.

* Wählen Sie aus den folgenden Vorgaben für adaptive Videokodierung oder einzelne Kodierungsvorgaben aus:

   * **[!UICONTROL 16:9 Adaptives Video]**  - Erstellen Sie Videos mit einem Seitenverhältnis von 16:9 für die Bereitstellung auf Desktops, Mobilgeräten (iPhone, iPad, Android™) und Tablets (iPad, Android™), die mit der Auflösung und Bitrate optimiert sind, die der Verbindungsgeschwindigkeit des Viewers am besten entspricht.

   * **[!UICONTROL 4:3 Adaptives Video]**  - Erstellen Sie Videos mit dem Seitenverhältnis 4:3 für die Bereitstellung auf Desktops, Mobilgeräten (iPhone, iPad, Android™) und Tablets (iPad, Android™), die mit der Auflösung und Bitrate optimiert sind, die der Verbindungsgeschwindigkeit des Viewers am besten entspricht.

   * **[!UICONTROL Adaptives Video]**  - Eine einzelne Kodierungsvorgabe, die mit jedem Seitenverhältnis verwendet werden kann, um Videos für die Bereitstellung auf Mobilgeräten, Tablets und Desktops zu erstellen. Hochgeladene Quellvideos, die mit dieser Vorgabe kodiert wurden, weisen eine feste Höhe auf. Die Breite wird jedoch automatisch skaliert, um das Seitenverhältnis des Videos beizubehalten.

      Die Flexibilität der automatischen Skalierungsfunktion ist ebenfalls standardmäßig verfügbar, wenn Sie eine eigene benutzerdefinierte Vorgabe für die Videokodierung erstellen.

      Siehe [Hinzufügen oder Bearbeiten einer Videokodierungsvorgabe](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   * **[!UICONTROL Adaptive Videokodierung (16:9 oder 4:3)]**  - Erstellen Sie sowohl Videos mit dem Seitenverhältnis 16:9 als auch mit dem Seitenverhältnis 4:3 für die Bereitstellung auf Desktops, Mobilgeräten (iPhone, iPad, Android™) und Tablets (iPad, Android™). Alle optimiert mit der Auflösung und Bitrate, die der Verbindungsgeschwindigkeit des Viewers am besten entspricht.

      Siehe [Vorgaben für die Videokodierung (16:9 oder 16:9: 3)](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets).

   * **[!UICONTROL Einzelne Kodierungsvorgaben]**

      >[!NOTE]
      >
      >Um Videos auf iPads bereitzustellen, können Sie eine Kodierungsvorgabe für Mobilgeräte oder eine Kodierungsvorgabe für Tablets auswählen. Tablet-Vorgaben weisen gewöhnlich eine höhere Auflösung und Qualität auf und sind für den iPad mit seinem größeren Display und der hohen Verbindungsgeschwindigkeit optimiert. Damit Videodateien, die mit einer Tablet-Vorgabe kodiert wurden, richtig wiedergegeben werden können, muss die mobile Site bzw. Anwendung über einen Code zur Geräteerkennung verfügen. Dieser Code sorgt dafür, dass, abhängig vom erkannten Wiedergabegerät, das entsprechende Videomaterial für iPhone oder iPad bereitgestellt wird. Durch die Auswahl einer Mobil-Vorgabe für die Wiedergabe von Videodateien auf dem iPad wird der Workflow vereinfacht. Das liegt daran, dass Sie für iPhones und iPads dieselbe Videodatei verwenden können. Allerdings wird dabei die Qualität des Videomaterials an das iPhone mit seiner geringeren Auflösung angepasst.

      * Wählen Sie unter der Gruppe „Kodierungsvorgaben“ in der Dropdown-Liste „Kodierungsvorgaben sortieren“ entweder „Name“ oder „Größe“, um die Vorgaben nach Name oder Auflösung zu sortieren.
      * Wählen Sie eine Kodierungsvorgabe basierend auf der Auflösung und Bandbreite aus, mit der Sie das Video wiedergeben möchten.
      * Sie können Adaptive Videokodierung und mindestens eine Kodierungsvorgabe pro Video auswählen. Beispielsweise können Sie eine Datei beim Hochladen gleichzeitig für Desktop und mobile Geräte kodieren.

Nachdem Sie **[!UICONTROL Upload starten]** ausgewählt haben, wird die Übergeordnete Originalvideodatei hochgeladen und aus der Übergeordneten Datei werden kodierte Dateien generiert.

### Kodierungsvorgabeoptionen {#about-encoding-preset-options}

Folgende Parameter stehen für die Kodierungsvorgabeoptionen zur Verfügung:

* **[!UICONTROL Zielverbindungsgeschwindigkeit]**  - Die Internetverbindungsgeschwindigkeit des Zielendbenutzers.

* **[!UICONTROL Kodiertes Dateisuffix]**  - Das Suffix, das zur Identifikation an die kodierte Videodatei angehängt wird.

* **[!UICONTROL Video-Bitrate (Datenrate)]**  - Die Datenmenge, die kodiert wird, um eine Sekunde Videowiedergabe auszumachen (in Kilobit pro Sekunde).

* **[!UICONTROL Pixel-Breite/Höhe]**  - Die Breite des Bildschirmbilds in Pixel. die Höhendimension des Bildschirmbilds (in Pixel).

* **[!UICONTROL Frame pro Sekunde (fps)]**  - Die Anzahl der Frames oder Standbilder für jede Sekunde des Videos. In den USA und Japan werden die meisten Videos mit 29,97 fps aufgenommen und in Europa und Asien (ausgenommen Japan) mit 25 fps. Film wird mit 24 fps aufgenommen.

* **[!UICONTROL Audio-Bitrate]**  - Die Menge an kodierten Daten, die für eine Sekunde Audiowiedergabe kodiert wird (in Kilobit pro Sekunde).

Die folgende Tabelle enthält empfohlene Verfahren zur Auswahl von Video-Vorgaben und die Namenskonventionen, mit denen kodierte Dateien bezeichnet werden.

### Adaptive Video (Standard) {#adaptive-video-default}

Eine Kodierungsvorgabe, die mit jedem Seitenverhältnis verwendet werden kann, um Videos zur Wiedergabe auf Mobilgeräten, Tablets und Desktops zu erstellen. Hochgeladene Quellvideos, die mit dieser Vorgabe kodiert werden (Standard und optimales Verfahren), werden auf eine feste Höhe eingestellt, die Breite wird jedoch automatisch so skaliert, dass das Seitenverhältnis des Videos beibehalten wird.

**Adaptive Video (Standard)**

|  | Kodierungsvorgabenname/QuickInfo-Text | Kodierungsdateisuffix | Videodatenrate (Kbit/s) | Breite/Höhe (Pixel) | Einzelbilder pro Sekunde (fps) | Audiobitrate (Kbit/s) | Empfehlungen |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Auto x360, 800 kBit/s | _Mobile_Autox360p_800K | 800 | Autox360 | Gleich Quelle | 64 | Für Mobilgeräte (iPhone, iPad, Android™) |
| 2 | Auto x 480, 1400 kBit/s | _Tablet_Autox480p_1400K | 1400 | Autox480 | Gleich Quelle | 96 | Für Tablet (iPad, Android™) |
| 3 | Auto x 720, 2600 kBit/s | _Desktop_Autox720p_2600K | 2600 | Autox720 | Gleich Quelle | 128 | Für Desktop |

### Vorgaben für die adaptive Videokodierung (16:9 oder 4:3) {#adaptive-video-encoding-or-video-presets}

Diese Vorgaben für die adaptive Videokodierung bestehen aus einer Serie einzelner Kodierungsvorgaben, die basierend auf dem Seitenverhältnis des hochgeladenen Videos automatisch für Sie ausgewählt werden. Wenn Sie z. B. ein 4:3-Video hochladen, wird es automatisch mit allen fünf 4:3-Vorgaben kodiert, die sich in der Master-Vorgabenliste der Option **Adaptive Videokodierung (16:9 oder 4:3)** befinden.

Informationen zu den Parametern für Kodierungsoptionen finden Sie unter [Kodierungsvorgabeoptionen](application-setup.md#about_encoding_preset_options).

**Vorgaben für die adaptive Videokodierung (16:9 oder 4: 3)**

|  | Kodierungsvorgabenname/QuickInfo-Text | Zielverbindungsgeschwindigkeit (Kbit/s) | Kodierungsdateisuffix | Videodatenrate (Kbit/s) | Breite/Höhe (Pixel) | Einzelbilder pro Sekunde (fps) | Audiobitrate (Kbit/s) | Empfehlungen |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android™), (400 Kbps)` | 500 | _Mobile_512x288_400K | 400 | 512 x 288 | Gleich Quelle | 64 | Niedrige Auflösung, 3G |
| 2 | `4:3, 384x288px, Mobile (iPhone, iPad, Android™), (400 Kbps)` | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Gleich Quelle | 64 | Niedrige Auflösung, 3G |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android™), (600 Kbps)` | 700 | _Mobile_512x288_600K | 600 | 512 x 288 | Gleich Quelle | 64 | Mittlere Auflösung, 3G |
| 4 | `4:3, 384x288, Mobile (iPhone, iPad, Android™), (600 Kbps)` | 700 | _Mobile_384x288_600 | 800 | 384 x 288 | Gleich Quelle | 64 | Mittlere Auflösung, 3G |
| 5 | `16:9, 640x360, Tablet (iPad, Android™), (800 Kbps)` | 900 | _iPad_640x360_800K | 800 | 640 x 360 | Gleich Quelle | 80 | Mittlere Auflösung, WiFi |
| 6 | `4:3, 640x480, Tablet (iPad, Android™), (800 Kbps)` | 900 | _iPad_640x480_800K | 800 | 640 x 480 | Gleich Quelle | 80 | Mittlere Auflösung, WiFi |
| 7 | `16:9, 768x432, Tablet (iPad, Android™), (1200 Kbps)` | 1,5 Mbit/s | _iPad_768x432_1200K | 1200 | 768 x 432 | Gleich Quelle | 96 | Hohe Auflösung, WiFi |
| 8 | `4:3, 768x576, Tablet (iPad, Android™), (1200 Kbps)` | 1,5 Mbit/s | _iPad_768x576_1200K | 1200 | 768 x 576 | Gleich Quelle | 96 | Hohe Auflösung, WiFi |
| 9 | `16:9, 1280x720, Desktop, (2000 Kbps)` | 3,0 Mbit/s | _1280x720_2000K | 2000 | 1280 x 720 | Gleich Quelle | 128 | High Definition, Widescreen |
| 10 | `4:3, 1280x960, Desktop, (2000 Kbps)` | 3,0 Mbit/s | _1280x960_2000K | 2000 Kbit/s | 1280 x 960 | Gleich Quelle | 128 | High Definition |

### Vorgaben für die Videokodierung für Desktop-PCs {#desktop-video-encoding-presets}

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
| 6 | 4:3, 480 x 360 (800 Kbit/s) | 900 | _480x360_800K | 800 | 480 x 360 | Gleich Quelle | 80 | Mittlere Auflösung |
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
| 6 | 4:3, 480 x 360 (800 Kbit/s), OGG | 900 | _OGG_480x360_800K | 800 | 480 x 360 | Gleich Quelle | 80 | Mittlere Auflösung |
| 7 | 4:3, 640 x 480 (1200 Kbit/s), OGG | 1,5 Mbit/s | _OGG_640x480_1200K | 1200 | 640 x 480 | Gleich Quelle | 96 | Mittlere Auflösung |
| 8 | 4:3, 1280 x 960 (2000 Kbit/s), OGG | 3,0 Mbit/s | _OGG_1280x960_2000K | 2000 | 1280 x 960 | Gleich Quelle | 128 | High Definition |

### Vorgaben für die Videokodierung für Mobilgeräte {#mobile-video-encoding-presets}

Gleich wie Bildrate der Quelle. Vorgaben für die Videokodierung für iPhone-, iPad- und Android™-Mobilgeräte.

Informationen zu den Parametern für Kodierungsoptionen finden Sie unter [Kodierungsvorgabeoptionen](application-setup.md#about_encoding_preset_options).

**H264 Baseline 2.1 - Audio AAC, Dateierweiterung MP4**

|  | Kodierungsvorgabenname/QuickInfo-Text | Zielverbindungsgeschwindigkeit (Kbit/s) | Kodierungsdateisuffix | Videobitrate (Kbit/s) | Pixel Breite/Höhe | Einzelbilder pro Sekunde (fps) | Audiobitrate (Kbit/s) | Empfehlungen |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512 x 288, Mobil (400 Kbit/s) | 500 | _Mobile_512x288_400K | 400 | 512 x 288 | Gleich Quelle | 64 | Niedrige Auflösung, 3G |
| 2 | 16:9, 512 x 288, Mobil (600 Kbit/s) | 700 | _Mobile_512x288_600K | 800 | 512 x 288 | Gleich Quelle | 64 | Mittlere Auflösung, 3G |
| 1 | 16:9, 512 x 288, Mobil (800 Kbit/s) | 900 | _Mobile_512x288_800K | 800 | 512 x 288 | Gleich Quelle | 80 | Mittlere Auflösung, Wi-Fi |
| 4 | 16:9, 512 x 288, Mobil (1000 Kbit/s) | 1,2 Mbit/s | _Mobile_512x288_1000K | 1000 | 512 x 288 | Gleich Quelle | 80 | Hohe Auflösung, Wi-Fi |
| 5 | 16:9, 512 x 288, Mobil (1200 Kbit/s) | 1,5 Mbit/s | _Mobile_512x288_1200K | 1200 | 512 x 288 | Gleich Quelle | 96 | Hohe Auflösung, Wi-Fi |
| 6 | 4:3, 384 x 288, Mobil (400 Kbit/s) | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Gleich Quelle | 64 | Niedrige Auflösung, 3G |
| 7 | 4:3, 384 x 288, Mobil (600 Kbit/s) | 700 | _Mobile_384x288_600K | 800 | 384 x 288 | Gleich Quelle | 64 | Mittlere Auflösung, 3G |
| 8 | 4:3, 448 x 336, Mobil (800 Kbit/s) | 900 | _Mobile_448x336_800K | 800 | 448 x 336 | Gleich Quelle | 80 | Mittlere Auflösung, Wi-Fi |
| 9 | 4:3, 448 x 336, Mobil (1000 Kbit/s) | 1,2 Mbit/s | _Mobile_448x336_1000K | 1000 | 448 x 336 | Gleich Quelle | 80 | Hohe Auflösung, Wi-Fi |
| 10 | 4:3, 448 x 336, Mobil (1200 Kbit/s) | 1,5 Mbit/s | _Mobile_448x336_1200K | 1200 | 448 x 336 | Gleich Quelle | 96 | Hohe Auflösung, Wi-Fi |

## Viewer-Vorgaben {#viewer-presets}

>[!NOTE]
>
>**Hinweis zur Einstellung der Unterstützung von Flash-Viewern** : Ab dem 31. Januar 2017 hat Adobe Dynamic Media Classic offiziell die Unterstützung für die Flash-Viewer-Plattform eingestellt.

Eine *Viewer-Vorgabe* ist eine Zusammenstellung von Einstellungen, mit denen die Anzeige von Rich-Media-Assets auf den Computerbildschirmen und Mobilgeräten für die Benutzer festgelegt wird. Sie können als Administrator Viewer-Vorgaben erstellen. Es sind Einstellungen für eine ganze Palette von Viewer-Konfigurationsoptionen verfügbar. Sie können beispielsweise die Viewer-Anzeigegröße, das Zoomverhalten, die Farbschemata, Ränder und Schriftarten ändern.

Verwenden Sie als Best Practice Adobe Dynamic Media Classic HTML5 Video-Viewer. Dank der für die HTML5 Video Viewer verwendeten Vorgaben handelt es sich um robuste Video-Player.

Indem Sie Folgendes in einen einzelnen Player kombinieren:

* Die Möglichkeit, die Wiedergabekomponenten mit HTML5 und CSS zu entwerfen.
* Sie verfügen über eingebettete Wiedergabe.
* Verwenden Sie adaptives und progressives Streaming je nach Browserfunktion.

Sie erweitern die Reichweite Ihrer Rich-Media-Inhalte auf Desktop-, Tablet- und Mobilbenutzer und sorgen für ein optimiertes Videoerlebnis.

Siehe [Über HTML5-Viewer](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) im Adobe Viewer-Referenzhandbuch.

Siehe [Adobe Dynamic Media Classic Viewer-Vorgabe-Kompatibilitätsmatrix](application-setup.md#scene7_viewer_preset_compatibility_matrix).

Siehe [Optimale Vorgehensweise: Verwenden des HTML5-Video-Viewers](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

Abhängig vom Viewer können Sie Community-Funktionen hinzufügen. Zu den Community-Funktionen zählen die Schaltflächen „Einbetten“, „E-Mail an Freunde senden“, „Verknüpfen“ und „Zur Website“. Mit diesen Schaltflächen können Benutzer, die die Viewer verwenden, den Viewer für andere freigeben oder die Adobe Dynamic Media Classic-Website öffnen.

Siehe auch [Adobe Viewer-Referenzbibliotheksbeispiele](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### Viewer-Unterstützung für interaktiv entwickelte Webseiten {#viewer-support-for-responsive-designed-web-pages}

Verschiedene Webseiten haben unterschiedliche Anforderungen. Manchmal möchten Sie eine Webseite, die einen Link bereitstellt, der den HTML5-Viewer in einem separaten Browserfenster öffnet. In anderen Fällen ist es erforderlich, den HTML5-Viewer direkt auf der Hosting-Seite einzubetten. Im letzteren Fall weist die Webseite wahrscheinlich ein statisches Layout auf. Oder sie ist &quot;responsiv&quot;und wird auf verschiedenen Geräten oder für verschiedene Browser-Fenstergrößen unterschiedlich angezeigt. Um diese Anforderungen zu erfüllen, unterstützen die HTML5-Viewer, die mit Adobe Dynamic Media Classic bereitgestellt werden, sowohl statische Webseiten als auch responsive Webseiten.

Weitere Informationen zum Einbetten responsiver Viewer auf Webseiten finden Sie unter [Informationen zur Bibliothek responsiver Bilder](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library.html#image-serving-api), [Responsive Bildbibliothek verwenden](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#image-serving-api) und [Befehlsreferenz - Befehlsattribute](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#responsive-static-image-library).

### Viewer-Vorgabentypen {#viewer-preset-types}

Administratoren können die folgenden Arten von Viewer-Vorgaben erstellen und anpassen:

* **[!UICONTROL eCatalog-Viewer]**  - Simuliert das Lesen eines gedruckten Katalogs. Sie können von Seite zu Seite wechseln, Elemente auf einer Seite ein- und auszoomen, Imagemaps verwenden, um weitere Informationen zu Elementen auf der Seite anzuzeigen, oder den Katalog durchsuchen. Sie können auch ein Infofeld einschließen, um detaillierte Informationen zu einem Element und eine verweissensitive Grafik anzuzeigen, wenn dem Bereich ein gültiges rollover_key-Attribut zugeordnet wurde. Zum Einschließen eines Infofelds geben Sie im Anzeigebereich „Infofeldeinstellungen“ des E-Katalog-Viewer-Vorgabe-Fensters die URL eines Infoservers ein.

* **[!UICONTROL Musterset-Viewer]** : Zeigt ein Bild in einer anderen Farbe, einem anderen Material, einer anderen Textur, einer anderen Oberfläche oder einem anderen Stoff an. Benutzer wählen eine Miniaturansicht aus, um die Varianten des Bildes anzuzeigen.

* **[!UICONTROL Viewer für gemischte Mediensets]** : Zeigt verschiedene Medientypen in einem Viewer an. Sie können darin Mustersets, Rotationssets, Bilder und Videos einschließen. Sie können Registerkarten für verschiedene Arten von Inhalten einstellen, beispielsweise eine Registerkarte für Bildsätze und eine für Videos. Videos, die aus einem gemischten Medienset abgespielt werden, verwenden einen standardmäßigen Video-Viewer mit einer Zeitleiste und Video-Steuerelementen wie „Abbrechen“, „Anhalten“, „Zurückspulen“ und „Abspielen“. Wenn Sie eine Viewer-Vorgabe für gemischte Mediensets einstellen, geben Sie an, welche Viewer für die verschiedenen Arten von Assets in Ihrem gemischten Medienset verwendet werden sollen. Sie können auch den Raster-Viewer oder den Karussell-Viewer verwenden, um ein gemischtes Medienset anzuzeigen.

* **[!UICONTROL Rotationsset-Viewer]** : Bietet mehrere Ansichten eines Bildes, damit Benutzer das Objekt drehen können, um die verschiedenen Seiten und Winkel zu untersuchen.

* **Video-Viewer**  - Zeigt Videos mit den Abmessungen der Auflösung der Quelldatei oder einer benutzerdefinierten Größe an. Adobe Dynamic Media Classic enthält viele vordefinierte Viewer-Vorgaben für die Wiedergabe von Videos. Wenn Sie Administrator sind, können Sie benutzerdefinierte Video-Viewer-Vorgaben erstellen. Es stehen mehr als ein Dutzend verschiedener Einstellungen zur Konfiguration des Video-Viewers zur Verfügung. Sie können Größe, Vorder- und Hintergrundfarbe, Video- und Audio-Steuerelemente, Fortschrittsleiste, Skin der Benutzeroberfläche, Sozialfunktionen und Hilfe-Funktionen konfigurieren.

* **[!UICONTROL Zoom-Viewer]**  - Bietet eine Auswahl aus drei Arten von Zoom-Viewern:

* **[!UICONTROL Zoom-Viewer]**  - Ermöglicht Benutzern das Vergrößern des Bereichs durch Auswählen. Sie können Steuerelemente zum Vergrößern, Verkleinern und Zurücksetzen des Bildes auf die Standardgröße auswählen.

* **[!UICONTROL Zoom-Viewer: Fly-out]** : Zeigt ein zweites Bild des gezoomten Bereichs neben dem Originalbild an. Der Benutzer hat keine Steuerelemente zur Verfügung. Er bewegt einfach die Auswahl über den Bereich, der angezeigt werden soll.

Bedenken Sie bei der Festlegung der gesamten Bandbreitennutzung für diesen Viewer, dass sowohl das Hauptbild als auch das Flyout-Bild im Viewer geladen werden müssen. Die Größe des Hauptbildes (Anzeigenbreite und -höhe) und der Zoomfaktor bestimmen die Größe des Flyout-Bildes. Setzen Sie diese beiden Werte gut in Relation, damit das Flyout-Bild eine kompakte Dateigröße erhält. Wenn beispielsweise die Hauptbilddatei sehr groß ist, verringern Sie den Wert für den Zoomfaktor. (Die Flyout-Breite und Flyout-Höhe bestimmen die Größe des Flyout-Fensters, aber nicht die Größe des Flyout-Bildes, das in den Viewer geladen wird.)

Wenn die Größe des Hauptbildes beispielsweise 350 x 350 Pixel bei einem Zoomfaktor von 3 beträgt, ist das Flyout-Bild 1050 x 1050 Pixel groß. Wenn die Größe des Hauptbildes 300 x 300 Pixel bei einem Zoomfaktor von 4 beträgt, ist das Flyout-Bild 1200 x 1200 Pixel groß. Über die Einstellung für die JPEG-Qualität (empfohlener Wert: zwischen 80 und 90) können Sie die Dateigröße deutlich reduzieren. Der empfohlene Wert für den Zoomfaktor liegt, je nach Größe des Hauptbildes, zwischen 2,5 und 4.

### Kompatibilitätsmatrix von Adobe Dynamic Media Classic Viewer-Vorgaben {#scene-viewer-preset-compatibility-matrix}

**Hinweis zur Einstellung der Unterstützung für Flash-Viewer**: Ab dem 31. Januar 2017 hat Adobe Dynamic Media Classic offiziell die Unterstützung für die Flash-Viewer-Plattform eingestellt.

In der folgenden Tabelle ist die derzeit verfügbare Adobe Dynamic Media Classic Viewer-Vorgaben aufgeführt. Außerdem gibt die Tabelle Aufschluss über die Viewer-Kompatibilität mit Desktop- und mobilen Geräten sowie die für jeden Viewer verwendete Technologie.

Siehe auch [Adobe Viewer-Referenzbibliotheksbeispiele](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

Informationen zu unterstützten Webbrowser- und Betriebssystemversionen für Viewer finden Sie in den Viewer-Versionshinweisen. 

Siehe [Adobe Viewer-Versionshinweise](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android™-Smartphone | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Zoom-Viewer |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android™-Smartphone | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Bildsatz-Viewer |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android™-Smartphone | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Musterset-Viewer |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android™-Smartphone | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| E-Katalog-Viewer |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(Enthält Unterstützung für Social Media und Katalogsuche.) | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog(Enthält Unterstützung für Social Media und Katalogsuche.) | HTML5 | X | X | X | X | X |

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android™-Smartphone | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Rotationsset-Viewer |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**eVideo-Viewer**

Adobe Dynamic Media Classic unterstützt die mobile Videowiedergabe für MP4 H.264-Videos.

* BlackBerry®-Geräte, die dieses Videoformat unterstützen, finden Sie hier: [Unterstützte Videoformate auf BlackBerry®](https://developer.blackberry.com/devzone/develop/supported_media/bb10_media_support.html)
* Sie finden auch Windows®-Geräte, die dieses Videoformat unterstützen, unter: [Unterstützte Videoformate unter Windows® Phone](https://docs.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android™-Smartphone | Android™ Tablet | BlackBerry® Smartphone | Windows® Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video(Enthält Unterstützung für die Untertitelung.) Siehe [Optimale Vorgehensweise: Verwenden des universellen HTML5-Video-Viewers.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social(Enthält Unterstützung für Untertitel und soziale Medien.) | HTML5 | X | X | X | X | X | X | X |

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android™-Smartphone | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Viewer für gemischte Mediensets |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Übersicht über die unterstützten Gesten für Mobilgeräte-Viewer {#supported-mobile-viewers-gestures-matrix}

In der folgenden Tabelle sind die Handy-Viewer-Gesten aufgeführt, die auf iOS-, Android™ 2.x- und Android™ 3.x-Geräten unterstützt werden.

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android™-Smartphone | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Bildsatz-Viewer |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### Über den Bildschirm „Viewer-Voreinstellung“  {#about-the-viewer-preset-screen}

Über den Anzeigebereich „Viewer-Vorgaben“ erstellen und verwalten Sie Viewer-Vorgaben. Um diesen Bildschirm zu öffnen, gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Viewer-Vorgaben]**.

Der Anzeigebereich „Viewer-Vorgaben“ umfasst Werkzeuge für die folgenden Aufgaben:

* **Vorgabe hinzufügen**  - Wählen Sie &quot;Hinzufügen&quot;aus und treffen Sie im Dialogfeld &quot;Viewer-Vorgabe hinzufügen&quot;Auswahlen  **** .

       Siehe [Hinzufügen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding_and_editing_viewer_presets).
   
* **Vorgabe bearbeiten**  - Wählen Sie eine Vorgabe aus und klicken Sie auf  **[!UICONTROL Bearbeiten]**.

       Siehe [Hinzufügen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding_and_editing_viewer_presets).
   
* **Vorgabe löschen**  - Wählen Sie eine Vorgabe aus und klicken Sie auf  **[!UICONTROL Löschen]**.

* **Vorgabe exportieren**  - Wählen Sie eine HTML5-Viewer-Vorgabe aus und klicken Sie dann auf  **** Exportieren , um die Viewer-Skin herunterzuladen, damit Sie sie als Grundlage für die Erstellung und das Hinzufügen einer weiteren Viewer-Vorgabe verwenden können.

       Siehe [HTML5-Viewer-Vorgabe exportieren](application-setup.md#exporting_an_html5_viewer_preset).
   
* **Filtern der Viewer-Vorgabenliste**  - Verwenden Sie diese Tools, um die Liste zu filtern:

       * Öffnen Sie die Dropdownliste **Aktiv/Inaktiv** und wählen Sie eine Option aus, um aktive Vorgaben, inaktive Vorgaben oder alle Vorgaben anzuzeigen.
       * Öffnen Sie die Dropdown-Liste **Viewer** und wählen Sie eine Option aus, um nur Viewer einer bestimmten Art anzuzeigen. Wählen Sie **[!UICONTROL Alle Viewer]**, um alle Viewer anzuzeigen.
   
* **Sortieren von Vorgaben**  - Wählen Sie eine Spaltenüberschrift aus (**[!UICONTROL Aktiv]**,  **[!UICONTROL Typ]**,  **[!UICONTROL Vorgabe]** oder  **[!UICONTROL Plattform]**), um die Liste nach einer Spalte zu sortieren. Wählen Sie eine Spaltenüberschrift ein zweites Mal aus, um die Liste in absteigender (oder aufsteigender) Reihenfolge zu sortieren.

* **Voreinstellungen aktivieren und deaktivieren**  - Wählen Sie eine Voreinstellung aus und wählen Sie dann deren Option Aktiv aus, um sie zu aktivieren oder zu deaktivieren.

       Siehe [Aktivieren oder Deaktivieren von Viewer-Vorgaben](application-setup.md#activating_or_deactivating_viewer_presets).
   
>[!NOTE]
>
>Wählen Sie auf der rechten Seite der Seite &quot;Viewer-Vorgaben&quot;die Option **[!UICONTROL Vorschau]** aus, damit Sie sehen können, wie ein Asset in der ausgewählten Viewer-Vorgabe aussieht. Um ein anderes Asset anzuzeigen, wählen Sie **[!UICONTROL Durchsuchen]** auf der Seite &quot;Viewer-Vorgaben&quot;aus und wählen Sie ein anderes Asset im Dialogfeld &quot;Asset-Vorschau auswählen&quot;aus.

### Hinzufügen und Bearbeiten von Viewer-Vorgaben {#adding-and-editing-viewer-presets}

Neben dem Hinzufügen von Viewer-Vorgaben mithilfe von **[!UICONTROL Hinzufügen]** in der Benutzeroberfläche können Sie auch **[!UICONTROL Exportieren]** verwenden, um eine Viewer-Vorgabe hinzuzufügen. Exportieren Sie einfach eine vorhandene HTML5-Viewer-Vorgabe und verwenden Sie diese dann als Grundlage für die neue Vorgabe.

Siehe [HTML5-Viewer-Vorgabe exportieren](application-setup.md#exporting_an_html5_viewer_preset).

**So fügen Sie Viewer-Vorgaben hinzu und bearbeiten sie:**

1. Navigieren Sie in der rechten oberen Ecke von Adobe Dynamic Media Classic zu **[!UICONTROL Setup]** > **[!UICONTROL Viewer-Vorgaben]**.

   Sie können die Liste der Vorgaben filtern. Wenn nur Vorgaben für Video-Viewer aufgelistet werden sollen, wählen Sie auf der Symbolleiste direkt über der Tabelle in der Dropdown-Liste „Viewer“ die Option „Video-Viewer“ aus.

1. Fügen Sie auf der Seite &quot;Viewer-Vorgaben&quot;die Viewer-Vorgabe im Bildschirm &quot;Viewer-Vorgaben&quot;hinzu oder bearbeiten Sie sie.

   * **Hinzufügen**  - Wählen Sie in der Symbolleiste  **[!UICONTROL Hinzufügen]** aus. Wählen Sie im Dialogfeld &quot;Viewer-Vorgabe hinzufügen&quot;eine Plattform aus und wählen Sie einen Rich-Media-Asset-Typ aus.

          Wählen Sie **[!UICONTROL Speichern unter]**, wenn Sie die Erstellung der Viewer-Vorgabe abgeschlossen haben.
      
   * **Hinzufügen ausgehend von einer vorhandenen Viewer-Vorgabe** : Wählen Sie in der Tabelle eine Video-Viewer-Vorgabe aus und wählen Sie dann in der Symbolleiste  **** Bearbeiten aus.

          Nachdem Sie den Video-Viewer neu konfiguriert haben, wählen Sie **[!UICONTROL Speichern unter]**, um die Vorgabe unter einem anderen Namen im Textfeld &quot;Vorgabenname&quot;zu speichern.
      
   * **Bearbeiten**  - Wählen Sie eine vorhandene Viewer-Vorgabe aus und klicken Sie auf  **[!UICONTROL Bearbeiten]**.

1. Geben Sie im Bildschirm &quot;Viewer konfigurieren&quot;im Feld Vorgabenname den Vorgabennamen ein oder bearbeiten Sie ihn.
1. Legen Sie die weiteren gewünschten Optionen fest.

   >[!NOTE]
   >
   >Wählen Sie **[!UICONTROL Gleiche Quelle]** aus, um die Größe des Video-Viewers automatisch auf die Auflösung des kodierten Videos selbst anzupassen. Wenn Sie diese Option auswählen, können Sie die Anzeigebreite und die Bühnenhöhe nicht eingeben. Stattdessen werden diese Optionen vom Video selbst übernommen. Wenn Sie **[!UICONTROL Gleiche Quelle]** auswählen, legen Sie die Option &quot;Randgröße&quot;fest, um die Hautdimensionen außerhalb des Videowiedergabebereichs widerzuspiegeln. Die Randgröße bezeichnet Höhe und Breite der Video-Steuerelemente in Pixel. Sie können das folgende Bild verwenden, um die gewünschten Randgrößen zu bestimmen.*

   ![Randkonfiguration des Video-Viewers](assets/vs_video_viewer_configure_margin.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Speichern unter]** aus, wenn Sie eine Viewer-Vorgabe anhand einer vorhandenen Vorgabe hinzugefügt haben.
   * Wählen Sie **[!UICONTROL Speichern]** aus, wenn Sie eine Viewer-Vorgabe hinzugefügt oder bearbeitet haben.

### HTML5-Viewer-Vorgabe exportieren {#exporting-an-html-viewer-preset}

Sie können eine vorhandene HTML5-Viewer-Vorgabe exportieren, um sie als Grundlage für die Erstellung einer HTML5-Viewer-Vorgabe zu verwenden. Diese Exportoption ist nützlich, da Sie den Viewer auf diese Weise nicht komplett neu erstellen müssen. Stattdessen exportieren Sie eine Vorgabe mit Einstellungen, die Ihren Anforderungen in etwa entsprechen, und verwenden diese dann als Ausgangspunkt für Ihre Design-Anpassungen.

Alle standardmäßigen CSS-Dateien mit Viewer-Vorgaben in Adobe Dynamic Media Classic verwenden relative Bildbereitstellungspfade, die auf Assets unter `Scene7SharedAssets` verweisen. Beispielsweise ist Folgendes ein relativer Pfad zu einem Bild-Asset in einer CSS-Datei für Viewer-Vorgaben in

`Scene7SharedAsset`:  `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

Wenn Sie jedoch Viewer-CSS-Dateien auf Ihrer eigenen Site hosten, müssen Sie diese relativen Bildpfade auflösen, indem Sie einen expliziten Pfad zum Image-Server in Ihrer eigenen Umgebung verwenden. Wenn Sie beispielsweise den relativen Pfad oben auf einen expliziten Pfad aktualisieren würden, könnte er wie folgt aussehen, wobei `https://s7d1.scene7.com` der direkte Pfad zu Ihrem Bildserver ist: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**So exportieren Sie eine HTML5-Viewer-Vorgabe:**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Navigieren Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Viewer-Vorgaben]**.
1. Wählen Sie in der Symbolleiste &quot;Viewer-Vorgaben&quot;in der zweiten Dropdown-Liste von links **[!UICONTROL HTML5]** aus.
1. Wählen Sie in der dritten Dropdown-Liste von links die Option **[!UICONTROL Alle Viewer]** aus.
1. Wählen Sie die Viewer-Vorgabe aus, die Sie als Grundlage für eine neue HTML5-Viewer-Vorgabe verwenden möchten.
1. Wählen Sie in der Symbolleiste **[!UICONTROL Export]** aus.
1. Wählen Sie im Dialogfeld &quot;Ausgewählte Assets exportieren&quot;die Option **[!UICONTROL Export senden]**.

   Nach dem Export erhalten Sie eine CSS-Datei. Laden Sie die Datei herunter und dekomprimieren Sie sie.

1. Öffnen Sie die CSS-Datei in einem CSS-Editor, nehmen Sie Ihre Änderungen vor und speichern Sie die Datei anschließend.
1. Laden Sie die CSS-Datei in Adobe Dynamic Media Classic hoch.

   Siehe [Hochladen von Dateien](uploading-files.md#uploading_files).

1. Veröffentlichen Sie die CSS-Datei auf dem Dynamic Media Image-Server.

   Siehe [Veröffentlichen von Dateien](publishing-files.md#publishing_files).

1. Fügen Sie wie üblich die neue Viewer-Vorgabe hinzu. Wählen Sie die von Ihnen hochgeladene Viewer-CSS-Datei aus.

   Siehe [Hinzufügen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding_and_editing_viewer_presets).

### Aktivieren oder Deaktivieren von Viewer-Vorgaben {#activating-or-deactivating-viewer-presets}

Um eine URL für die Anzeige von Assets zu erstellen, öffnen Benutzer die Dropdownliste &quot;Vorgaben&quot;im Dialogfeld &quot;Vorschau&quot;, wählen eine Viewer-Vorgabe aus und klicken dann auf **[!UICONTROL URL kopieren]** (siehe [URL einer Viewer-Vorgabe kopieren](application-setup.md#copying_the_url_of_a_viewer_preset)). Diese Vorgabenliste enthält Viewer-Vorgaben, die Administratoren im Anzeigebereich „Viewer-Vorgaben“ hinzufügen und verwalten können. Alle aktiven E-Katalog-Viewer-Vorgaben werden beispielsweise im Dialogfeld „Vorschau“ in der Dropdown-Liste „Vorgaben“ angezeigt, wenn ein Benutzer eine Vorschau eines E-Katalogs anzeigt.

Wenn Sie Viewer-Vorgaben im Anzeigebereich „Viewer-Vorgaben“ nicht deaktivieren, kann die Dropdown-Liste „Vorgaben“ im Dialogfeld „Vorschau“ sehr viele Einträge umfassen.

**So aktivieren oder deaktivieren Sie Viewer-Vorgaben:**

1. Navigieren Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Viewer-Vorgaben]**.
1. Aktivieren oder deaktivieren Sie auf der Seite &quot;Viewer-Vorgaben&quot;die Optionen **[!UICONTROL Aktiv]** , um Viewer-Vorgaben zu aktivieren oder zu deaktivieren.

### URL einer Viewer-Vorgabe kopieren {#copying-the-url-of-a-viewer-preset}

Nachdem Sie ein Asset veröffentlicht haben, können Sie eine URL kopieren, um das Asset mit den Einstellungen einer bestimmten Viewer-Vorgabe anzuzeigen.

Die URL wird in die Zwischenablage kopiert. Anschließend können Sie sie nach Bedarf in den HTML-Code Ihrer Website, des Mobilgeräts oder Ihrer Anwendung einfügen.

**So kopieren Sie die URL einer Viewer-Vorgabe:**

1. Markieren Sie das Asset im Durchsuchenbedienfeld.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld URLs und Einbettungscode auf der rechten Seite **[!UICONTROL URL]** kopieren rechts neben dem gewünschten Viewer aus.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

   Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL URL kopieren]** aus.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.
   Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL URL kopieren]** aus.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Navigieren Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.
   Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL URL kopieren]** aus.

### Kopieren des Einbettungscodes einer Viewer-Vorgabe {#copying-the-embed-code-of-a-viewer-preset}

Mithilfe der Einbettungscode-Funktion können Sie den Viewer-Code für die ausgewählte Viewer-Vorgabe überprüfen. Sie können den Code auch in die Zwischenablage kopieren, damit Sie ihn in Webseiten für die Bereitstellung des Viewers einfügen können.

Die Bearbeitung des Codes ist im Dialogfeld Einbettungscode nicht zulässig.

**So kopieren Sie den Einbettungscode einer Viewer-Vorgabe:**

1. Wählen Sie das Asset im Bedienfeld zum Durchsuchen von Assets aus.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld URLs auf der rechten Seite **[!UICONTROL Einbettungscode]** aus.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

   Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL Einbettungscode]** aus.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.
   Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL Einbettungscode]** aus.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Navigieren Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.
   Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL Einbettungscode]** aus.

1. Wählen Sie im Dialogfeld &quot;Einbettungscode&quot;die Option **[!UICONTROL In Zwischenablage kopieren]**.
1. Wählen Sie **[!UICONTROL Close]** aus.

## Standard-Viewer konfigurieren {#configuring-default-viewers}

Sie können &quot;Standard-Viewer&quot;verwenden, um den mit einem Asset verknüpften Standard-Viewer zu konfigurieren, wenn Sie die Vorschau in Adobe Dynamic Media Classic verwenden. Die Standardvorschau kann für die folgenden Asset-Typen festgelegt werden:

* Bild
* Video
* Rotationsset
* Katalog
* Bildsatz
* Musterset
* Medienset

**So konfigurieren Sie Standard-Viewer:**

1. Wählen Sie in der Dropdown-Liste Einstellungen die Option **[!UICONTROL Anwendungseinstellungen]** aus.
1. Gehen Sie im Fenster &quot;Einstellungen&quot;im linken Bereich zu **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Viewer]**
1. Wählen Sie **[!UICONTROL Standard-Viewer]** aus.
1. Wählen Sie im Fenster „Standard-Viewer“ in der Dropdown-Liste für die einzelnen Asset-Typen den Viewer aus, den Sie mit der Asset-Vorschau verknüpfen möchten.
1. Wählen Sie in der rechten unteren Ecke des Fensters Standard-Viewer **[!UICONTROL Speichereinstellungen]** aus.
1. Wählen Sie in der rechten unteren Ecke des Fensters &quot;Einstellungen&quot;die Option **[!UICONTROL Close]** aus, um zum Asset-Fenster zurückzukehren.

## Metadaten-Ansichten {#metadata-views}

*Metadaten* sind standardisierte Informationen zu einem Asset. Mit Metadaten können Sie Ihren Arbeitsablauf optimieren, Ihre Assets organisieren und die Suche verbessern. Adobe Dynamic Media Classic unterstützt den IPTC-Standard (International Press Telecommunications Council) und den XMP (Extensible Metadata Platform) Standard. Bevor Benutzer Metadaten zu einem Asset in der Detailansicht anzeigen oder eingeben, können sie das Menü Metadaten-Ansichten öffnen. Dort können sie den Satz von Metadatenfeldern auswählen, die sie anzeigen oder zum Beschreiben des Assets verwenden möchten.

Adobe Dynamic Media Classic bietet vordefinierte Metadaten-Ansichten und Administratoren können eigene Metadaten-Ansichten erstellen, die Benutzern zur Auswahl stehen, wenn sie Metadaten eingeben.

### Erstellen einer Metadaten-Ansicht {#creating-a-metadata-view}

1. Gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Metadaten-Ansichten]**.
1. Wählen Sie **[!UICONTROL Hinzufügen]**.
1. Geben Sie im Textfeld Vorgabenname einen Namen für die Ansicht ein.
1. (Optional) Aktivieren Sie **[!UICONTROL Als Standard festlegen]**, um diese Ansicht für die Anzeige zu verwenden, die Benutzer beim Öffnen des Metadatenbedienfelds in der Detailansicht sehen.
1. (Optional) Wählen Sie **[!UICONTROL UDF]** einschließen aus, um benutzerdefinierte Felder in die Ansicht einzuschließen. Benutzerdefinierte Felder werden oben im Metadatenbedienfeld in der Detailansicht angezeigt.
1. Wählen Sie die Felder aus, die Sie für die Ansicht verwenden möchten (wählen Sie **[!UICONTROL Alle auswählen]** aus, um alle Felder auszuwählen).
1. Wählen Sie **[!UICONTROL Save]** aus.

   Die ausgewählten Kategorien und Felder für die Ansicht werden im Vorschaubedienfeld angezeigt.

### Verwalten von Metadaten-Ansichten {#managing-metadata-views}

1. Gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Metadaten-Ansichten]**.
1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie eine Ansicht aus, um eine Vorschau davon zu erstellen. Die Felder in der Ansicht werden im Vorschaubedienfeld angezeigt.
   * Um eine Ansicht zu bearbeiten, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Bearbeiten]**. Wählen Sie dann im Vorschaufenster Feldnamen aus oder heben Sie die Auswahl auf und aktivieren oder deaktivieren Sie die Option **[!UICONTROL UDF]** einschließen .
   * Um eine Ansicht zu löschen, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Löschen]**.
   * Um eine Ansicht als Standard festzulegen, wählen Sie sie aus und klicken Sie dann auf **[!UICONTROL Als Standard festlegen]**. Die Standardansicht ist die Ansicht, die Benutzer sehen, wenn sie ein Asset in der Detailansicht öffnen und zum Metadatenbedienfeld wechseln.

## Metadaten-Vorgaben {#metadata-presets}

Metadaten-Vorgaben bieten Administratoren eine Möglichkeit, den Assets zugeordnete Metadaten zu kontrollieren und zu regeln. In der Detailansicht kann ein Benutzer Metadaten zu einem Asset in Feldern eingeben, die zu diesem Zweck bereitgestellt werden. Ein Benutzer kann beispielsweise einen Eigentümernamen, eine Copyrightbeschreibung und eine Adresse eingeben. Um sicherzustellen, dass Benutzer diese Informationen korrekt und vollständig eingeben, können Sie Metadaten-Vorgaben erstellen. Bei Auswahl einer Metadatenvorgabe in der Detailansicht werden Metadatenfelder mit vordefinierten Werten gefüllt. So werden beispielsweise der Eigentümername, die Copyrightbeschreibung und die Adresse automatisch eingegeben.

Erstellen Sie eine Metadatenvorgabe für jeden Satz von Metadatenwerten, die Benutzer automatisch in die Detailansicht eingeben können sollen, um ein Asset zu beschreiben.

### Erstellen oder Bearbeiten einer Metadaten-Vorgabe {#creating-or-editing-a-metadata-preset}

1. Gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Metadatenvorgaben]**.
1. Führen Sie im Anzeigebereich „Metadaten-Vorgaben“ einen der folgenden Schritte aus:

   * Um eine Vorgabe zu erstellen, wählen Sie **[!UICONTROL Hinzufügen]** aus. Geben Sie im Textfeld Metadatenvorlagenname einen Namen für die Vorgabe ein. Wählen Sie **[!UICONTROL Metadaten-Ansichten]** und dann eine Ansicht aus der Dropdownliste aus (siehe [Metadaten-Ansichten](application-setup.md#metadata_views)).
   * Um eine vorhandene Vorgabe zu bearbeiten, wählen Sie die Vorgabe aus der Liste &quot;Metadaten-Vorgaben&quot;aus und klicken Sie dann auf **[!UICONTROL Bearbeiten]**.

1. Blenden Sie die Überschriften ein, die Sie in die Vorgabe aufnehmen möchten, und geben Sie Werte in die verschiedenen Felder ein, die Sie in die Vorgabe aufnehmen möchten.
1. Wählen Sie **[!UICONTROL Save]** aus.

   Die ausgewählten Kategorien und Felder für die Vorgabe werden im Vorschaubedienfeld angezeigt.

### Verwalten von Metadaten-Vorgaben {#managing-metadata-presets}

1. Gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Metadatenvorgaben]**.
1. Führen Sie einen der folgenden Schritte aus:

   * Um eine Vorschau einer Vorgabe anzuzeigen, wählen Sie die entsprechende Vorgabe aus. Die Vorgabeninformationen (Kategorien und Felder) werden im Anzeigebereich „Vorschau“ angezeigt.
   * Um eine Vorgabe zu löschen, wählen Sie die Vorgabe aus und klicken Sie auf **[!UICONTROL Löschen]**.

## Benutzerdefinierte Felder {#user-defined-fields}

Ein Medienportal-Administrator bzw. Unternehmensadministrator kann individuelle, benutzerdefinierte Metadatenfelder erstellen. Mit benutzerdefinierten Feldern können Sie Assets in Adobe Dynamic Media Classic organisieren. Sie können die Felder bei Bedarf als aktiv markieren. Wenn diese benutzerdefinierten Metadatenfelder aktiviert sind, werden sie im Metadatenbedienfeld in der Detailansicht angezeigt. Die Benutzer können Informationen zur Beschreibung der Assets in die benutzerdefinierten Metadatenfelder eingeben. Außerdem können Benutzer ein benutzerdefiniertes Metadatenfeld als Suchkriterium angeben.

Eine effektive Nutzung benutzerdefinierter Metadatenfelder besteht darin, die Aktivierungszeit eines Assets für einen bestimmten Launch oder Ausverkauf zu verzögern. Sie definieren ein Feld &quot;Aktivierung&quot;, das auf dem Typ *Datum* basiert. Mithilfe des Bedienfelds **[!UICONTROL Metadaten]** in der Detailansicht oder **[!UICONTROL Datei]** > **[!UICONTROL Informationen bearbeiten]** können Sie festlegen, wann das Asset aktiviert wird. Adobe Dynamic Media Classic überprüft den Veröffentlichungsstatus eines Assets und den Veröffentlichungsverlauf. Wenn er sich nicht innerhalb der Aktivierungszeit befindet, wird der Veröffentlichungsstatus als &quot;Nicht veröffentlicht&quot;angezeigt.

>[!NOTE]
>
>Damit benutzerdefinierte Felder im Metadatenbedienfeld in der Detailansicht angezeigt werden, schließen Sie benutzerdefinierte Felder in Metadatenansichten ein. Wählen Sie im Anzeigebereich „Metadaten-Ansichten“ die Option „UDF einschließen“. Weitere Informationen finden Sie unter [Metadaten-Ansichten](application-setup.md#metadata_views).

>[!NOTE]
>
>Um mithilfe benutzerdefinierter, benutzerdefinierter Felder nach Assets zu suchen, gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Persönliche Einstellungen]** und wählen Sie dann **[!UICONTROL UDFs in Suche]** einschließen. Siehe [Persönliche Einstellungen](personal-setup.md#personal_setup).

### Erstellen eines benutzerdefinierten Metadatenfelds {#creating-a-user-defined-metadata-field}

1. Gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Benutzerdefinierte Felder]**.
1. Wählen Sie **[!UICONTROL Hinzufügen]**
1. Legen Sie im Dialogfeld „Benutzerdefiniertes Feld“ die gewünschten Optionen fest.

   * **[!UICONTROL Name]**  - Geben Sie einen Namen für das Metadatenfeld ein.

   * **[!UICONTROL Typ]**  - Wählen Sie eine Option, die den Typ der Informationen definiert, die Benutzer in das Metadatenfeld eingeben können:

   * **[!UICONTROL Zeichenfolge]**  - Eine Textzeichenfolge.

   * **[!UICONTROL Int]**  - Eine Ganzzahl.

   * **[!UICONTROL Gleitkommazahl]** : Eine Gleitkommazahl.

   * **[!UICONTROL Ja/Nein]**  - Ein boolescher Ja/Nein-Wert.

   * **[!UICONTROL Datum]**  - Ein Datum. Das Format MM/TT/JJJJ ist zulässig.

   * **[!UICONTROL Dateiname]**  - Der Name einer Datei.

   * **[!UICONTROL Farbe]**  - Der Name einer Farbe.

   * **[!UICONTROL Dimension]**  - Die Breite und Höhe des Assets.

   * **[!UICONTROL Nicht typisiert]**  - Für Abwärtskompatibilität. Wählen Sie diese Option nicht aus.

   * **[!UICONTROL Standardwert]**  - Geben Sie optional den Wert ein, den Benutzer mit hoher Wahrscheinlichkeit in das Feld eingeben. Dieser Wert wird als Standardwert für das neue Feld verwendet.

   * **[!UICONTROL Gilt für]**  - Wählen Sie optional einen Asset-Typ aus, wenn das Metadatenfeld nur auf einen bestimmten Asset-Typ angewendet werden soll.

      >[!NOTE]
      >
      >Wählen Sie die Option **[!UICONTROL Gilt für]** sorgfältig aus, da Sie die Option **[!UICONTROL Gilt für]** nicht ändern können, nachdem Sie ein benutzerdefiniertes Feld erstellt haben. Mit Adobe Dynamic Media Classic können Sie den Namen, den Typ und den Standardwert eines benutzerdefinierten Felds bearbeiten, nicht jedoch die Einstellung **[!UICONTROL Gilt für]**. *

1. Wählen Sie **[!UICONTROL Save]** aus, wenn Sie die Erstellung des Metadatenfelds abgeschlossen haben.

### Verwalten von benutzerdefinierten Feldern {#manage-user-defined-fields}

Im Anzeigebereich „Benutzerdefinierte Felder“ finden Sie Befehle zum Verwalten eigener, benutzerdefinierter Felder.

Benutzerdefinierte Felder können nur von Media Portal-Administratoren und Unternehmensadministratoren verwaltet werden.

Um diesen Bildschirm zu öffnen, gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Benutzerdefinierte Felder]**.

* **Feld bearbeiten**  - Wählen Sie das Feld aus und klicken Sie auf  **[!UICONTROL Bearbeiten]**.

* **Feld löschen**  - Wählen Sie das Feld aus und klicken Sie auf  **[!UICONTROL Löschen]**.

* **Feld aktivieren**  - Aktivieren oder deaktivieren Sie die Option  **** Aktiv neben dem Namen eines Felds. Wenn Sie eine Unternehmensadministrationsrolle innehaben, wird diese Option nicht angezeigt. Da diese Option mit MediaPortal in Zusammenhang steht, müssen Sie die Option MediaPortal-Funktionen anzeigen unter Persönliche Einstellungen auswählen (aktivieren), um die Aktivierungsfelder anzuzeigen.

## Optimieren von Dateien {#optimize-files}

Beim Hochladen von Dateien in die Adobe Dynamic Media Classic optimiert das System diese für die Speicherung und Veröffentlichung. Wenn das Hochladen jedoch unterbrochen wird, können einige Bilder nicht optimiert werden. In diesem Fall wird die Meldung „Bild wurde noch nicht optimiert“ angezeigt. Als Administrator können Sie jedoch auch diese Dateien optimieren.

Adobe Dynamic Media Classic durchsucht Ihre Dateien und optimiert nur die Bilder, die zuvor noch nicht vollständig optimiert wurden.

1. Gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** und wählen Sie **[!UICONTROL Dateien optimieren]** aus.
1. Geben Sie Informationen für den Optimierungsauftrag ein und wählen Sie **[!UICONTROL Submit]** aus.

   Wenn Sie mit mehr als einem Unternehmen arbeiten, optimieren Sie Dateien, die zu unterschiedlichen Unternehmen gehören, getrennt.

## Stapelsatzvorgaben {#batch-set-presets}

Verwenden Sie die Stapelsatzvorgaben, um automatisch Bildsets oder Rotationssets zu erstellen, während ein Auftrag ausgeführt wird, um Assets in Adobe Dynamic Media Classic hochzuladen.

Unternehmensadministratoren definieren zunächst Benennungskonventionen für die Assets, die sie in einem Satz gruppieren möchten. Anschließend können Sie eine Stapelsatzvorgabe erstellen, die auf diese Bilder verweist. Jede Vorgabe ist ein eindeutig benannter, in sich abgeschlossener Satz von Anweisungen, die definieren, wie der Satz unter Verwendung der Bilder, die den definierten Benennungsregeln im Vorgabenrezept entsprechen, konstruiert werden soll.

Alle aktiven Stapelsatzvorgaben für ein Unternehmen werden im Dialogfeld „Upload-Auftragsoptionen“ aufgelistet, sodass Sie bei jedem Hochladevorgang auswählen können, welche Vorgabe angewendet werden soll. Unternehmensadministratoren sehen alle aktiven und inaktiven Stapelsatzvorgaben. Beim Hochladen von Dateien erstellt Adobe Dynamic Media Classic automatisch einen Satz mit allen Dateien, die der definierten Benennungsregel in den aktiven Vorgaben entsprechen.

### Standardbenennung {#default-naming}

Der Unternehmensadministrator erstellt eine Standard-Benennungskonvention, die in einem beliebigen Stapelsatzvorgaben-Rezept verwendet wird. Die in der Definition der Stapelsatzvorgabe ausgewählte Standardbenennungskonvention kann alles sein, was Ihr Unternehmen benötigt, um Sets für Batch-Generationen für alle Websites zu erstellen. Eine Stapelsatzvorgabe wird erstellt, damit die von Ihnen definierte Standardbenennungsregel verwendet werden kann. Sie können so viele Stapelsatzvorgaben mit alternativen, benutzerdefinierten Benennungsregeln erstellen, wie für einen bestimmten Satz von Inhalten notwendig sind, falls eine Ausnahme für eine unternehmensspezifische Standardbenennung existiert.

Die Einrichtung einer Standardbenennungskonvention ist nicht erforderlich, um die Funktionen der Stapelsatzvorgabe zu verwenden. Es empfiehlt sich jedoch, mithilfe einer Standardbenennungsregel so viele Elemente Ihrer Benennungsregel zu definieren, wie Sie in einem Satz gruppieren möchten. Auf diese Weise kann die Erstellung von Stapelsätzen optimiert werden.

1. Gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Stapelsatzvorgaben]** > **[!UICONTROL Standardbenennung]**.
1. Wählen Sie **[!UICONTROL Formular anzeigen]** oder **[!UICONTROL Code anzeigen]**, um anzugeben, wie Sie die Informationen zu den einzelnen Elementen anzeigen und eingeben möchten.

   Sie können das Kontrollkästchen **[!UICONTROL Code anzeigen]** aktivieren, um die Erstellung des regelmäßigen Ausdruckswerts neben Ihren Formularauswahlen anzuzeigen. Sie können diese Werte nach Bedarf eingeben oder ändern. Dies hilft Ihnen bei der Definition der Elemente der Benennungsdefinition, falls Sie aus irgendeinem Grund durch die Formularansicht eingeschränkt werden. Wenn Ihre Werte in der Formularansicht nicht analysiert werden können, werden die Formularfelder inaktiv.

   >[!NOTE]
   >
   >Deaktivierte Formularfelder weisen nicht unbedingt auf einen ungültigen regelmäßigen Ausdruck hin. Es gibt keine Möglichkeit zu prüfen, ob Ihre regelmäßigen Ausdrücke korrekt sind. Sie sehen die Ergebnisse des regelmäßigen Ausdrucks, den Sie für jedes Element erstellen, im Anschluss an die Zeile „Ergebnis“. Der vollständige regelmäßige Anschluss wird am unteren Seitenrand angezeigt.

1. Erweitern Sie die Elemente bei Bedarf und geben Sie die zu verwendenden Benennungsregeln ein.
1. Wählen Sie nach Bedarf **[!UICONTROL Hinzufügen]** aus, um eine weitere Benennungsregel für ein Element hinzuzufügen. Oder wählen Sie **[!UICONTROL Entfernen]** aus, um eine Benennungsregel für ein Element zu löschen.
1. Wählen Sie **[!UICONTROL Speichern unter]** aus und geben Sie einen Namen für die Vorgabe ein. Sie können auch **[!UICONTROL Speichern]** auswählen, wenn Sie eine vorhandene Vorgabe bearbeiten.

Alternativ können Sie „Code anzeigen“ ohne verfügbare Formularfelder verwenden. In dieser Ansicht erstellen Sie Ihre Definitionen von Benennungskonventionen vollständig mit regulären Ausdrücken.

Zwei Elemente sind zur Definition verfügbar: Treffer und Grundname. Anhand dieser Felder können Sie alle Elemente einer Benennungsregel definieren und denjenigen Teil der Regel identifizieren, mit dem Sie den Satz benennen, der diese Elemente enthält. Die individuelle Benennungskonvention eines Unternehmens könnte eine oder mehrere Definitionszeilen für jedes dieser Elemente verwenden. Sie können für Ihre spezifische Definition so viele Zeilen wie erforderlich verwenden und sie zu eindeutigen Elementen gruppieren, beispielsweise Elementen für Hauptbild, Farbe, alternative Ansicht und Muster.

### Erstellen einer Stapelsatzvorgabe {#creating-a-batch-set-preset}

Adobe Dynamic Media Classic verwendet Stapelsatzvorgaben, um Assets zu organisieren, die einige allgemeine Informationen oder Inhalte in Bildsätzen für die Anzeige in Viewern teilen. Die Stapelsatzvorgabenrezepte werden automatisch zusammen mit den Asset-Importvorgängen ausgeführt, die Sie in Adobe Dynamic Media Classic planen.

Verwenden Sie „Stapelsatzvorgaben“ zum Erstellen, Bearbeiten und Verwalten Ihrer Stapelsatzvorgaben. Sie können so viele Vorgaben wie nötig erstellen, um alle gewünschten Asset-Aufnahmeaufträge abzudecken. Es gibt zwei Formen von Definitionen für Stapelsatzvorgaben: eine für eine von Ihnen eingerichtete Standardbenennungsregel und eine für benutzerdefinierte Namenskonventionen, die Sie spontan erstellen.

Sie können entweder die Formularfeldmethode verwenden, um eine Stapelsatzvorgabe zu definieren, oder die Codemethode, mit der Sie reguläre Ausdrücke verwenden können. Wie in **[!UICONTROL Standardbenennung]** können Sie **[!UICONTROL Codeansicht]** auswählen, während Sie in der Formularansicht definieren und Ihre Definitionen mit regulären Ausdrücken erstellen. Alternativ können Sie eine der Ansichten deaktivieren, um ausschließlich die eine oder die andere zu verwenden.

Siehe auch [Erstellen einer Stapelsatzvorgabe für die automatische Erstellung eines 2D-Rotationssets](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

**So erstellen Sie eine Stapelsatzvorgabe:**

1. Gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Stapelsatzvorgaben]** > **[!UICONTROL Stapelsatzvorgabe]**. **[!UICONTROL Formular anzeigen]**, wie in der oberen rechten Ecke der Detailseite angezeigt, ist die Standardansicht.
1. Wählen Sie im Bereich &quot;Vorgabenliste&quot;die Option **[!UICONTROL Hinzufügen]** aus, um die Definitionsfelder im Detailbereich auf der rechten Seite der Seite zu aktivieren.
1. Geben Sie in der Detailansicht in das Feld „Vorgabenname“ einen Namen für die Vorgabe ein.
1. Wählen Sie im Dropdown-Menü „Stapelsatztyp“ einen Vorgabentyp aus.

   Um automatisch ein 2D-Rotationsset zu erzeugen, wählen Sie in der Dropdownliste „Stapelsatztyp“ die Option **[!UICONTROL Multiachsen-Rotationsset]**.

1. Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie eine standardmäßige Benennungskonvention verwenden, die Sie zuvor unter **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Stapelsatzvorgaben]** > **[!UICONTROL Standardbenennung]** eingerichtet haben, erweitern Sie **[!UICONTROL Asset-Benennungskonventionen]** und wählen Sie dann in der Dropdownliste &quot;Dateibenennung&quot;die Option **[!UICONTROL Standard]** aus.
   * Um beim Einrichten der Vorgabe eine Benennungskonvention zu definieren, erweitern Sie **[!UICONTROL Asset-Benennungsregeln]** und wählen Sie dann in der Dropdown-Liste &quot;Dateibenennung&quot;die Option **[!UICONTROL Benutzerdefiniert]** aus.

1. Definieren Sie für die Reihenfolge der Sequenzen die Reihenfolge der Bilder, nachdem das Set in Adobe Dynamic Media Classic gruppiert wurde. Die Assets werden standardmäßig in alphanumerischer Reihenfolge angeordnet. Sie können jedoch auch eine durch Kommas getrennte Liste mit regulären Ausdrücken verwenden, um die Reihenfolge anzupassen.
1. Geben Sie für „Satzbenennungs- und -erstellungsregel“ das Suffix bzw. Präfix für den Basisnamen an, den Sie in der Asset-Benennungsregel definiert haben. Legen Sie außerdem fest, wo das Bildset in der Adobe Dynamic Media Classic-Ordnerstruktur erstellt wird.

   Wenn Sie eine große Anzahl von Bildsets definieren, trennen Sie diese Sets von den Ordnern, die die Assets selbst enthalten. Zahlreiche Kunden erstellen einen Ordner „Bildsätze“ und weisen die Anwendung an, im Stapelsatz generierte Sätze hier abzulegen.

1. Wählen Sie **[!UICONTROL Save]** im Detailbereich aus.

### Erstellen einer Stapelsatzvorgabe für die automatische Erstellung eines 2D-Rotationssets {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

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

Mit diesen Informationen kann Ihr Stapelsatztyp-Rezept wie folgt erstellt werden:

![Stapelsatzrezeptbild](assets/se_batch_set_recipe.png)

Die Gruppierung für den Teil des gemeinsamen Asset-Namens des Rotationssets wird dem Feld Übereinstimmung hinzugefügt (wie hervorgehoben). Der variable Teil des Asset-Namens, der die Zeile und Spalte enthält, wird den Feldern Zeile bzw. Spalte hinzugefügt.

Wenn das Rotationsset hochgeladen und veröffentlicht wird, aktivieren Sie den Namen des 2D-Rotationssets-Rezepts, das unter **[!UICONTROL Batchset-Voreinstellungen]** im Dialogfeld Upload-Auftragsoptionen aufgeführt ist.

**So erstellen Sie eine Stapelsatzvorgabe für die automatische Erstellung eines 2D-Rotationssets:**

1. Gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Stapelsatzvorgaben]** > **[!UICONTROL Stapelsatzvorgabe]**. **[!UICONTROL Formular anzeigen]**, wie in der oberen rechten Ecke der Detailseite angezeigt, ist die Standardansicht.
1. Wählen Sie im Bereich &quot;Vorgabenliste&quot;die Option **[!UICONTROL Hinzufügen]** aus, um die Definitionsfelder im Bereich &quot;Details&quot;auf der rechten Seite der Seite zu aktivieren.
1. Geben Sie in der Detailansicht in das Feld „Vorgabenname“ einen Namen für die Vorgabe ein.
1. Wählen Sie im Dropdownmenü „Batch-Settyp“ die Option **[!UICONTROL Asset-Set]**.
1. Wählen Sie in der Dropdownliste „Untertyp“ die Option **[!UICONTROL Multiachsen-Rotationsset]**.
1. Erweitern Sie **[!UICONTROL Asset-Benennungskonventionen]** und wählen Sie dann in der Dropdown-Liste &quot;Dateibenennung&quot;die Option **[!UICONTROL Benutzerdefiniert]** aus.
1. Verwenden Sie die Attribute **[!UICONTROL Übereinstimmung]** und optional **[!UICONTROL Basisname]**, um einen regulären Ausdruck für die Benennung von Bild-Assets zu definieren, aus denen die Gruppierung besteht.

   Der reguläre Ausdruck &quot;tatsächliche Übereinstimmung&quot;könnte beispielsweise wie folgt aussehen:

   `(\w+)-\w+-\w+`

1. Erweitern Sie **[!UICONTROL Zeilen-/Spaltenposition]** und definieren Sie anschließend den Namen des Formats für die Position des Bild-Assets innerhalb des 2D-Rotationsset-Arrays.

   Setzen Sie die Zeilen- oder Spaltenposition im Dateinamen in Klammern.

   Der reguläre Ausdruck für Ihre Zeile könnte beispielsweise wie folgt aussehen:

   `\w+-R([0-9]+)-\w+`

   oder

   `\w+-(\d+)-\w+`

   Der reguläre Ausdruck Ihrer Spalte könnte wie folgt aussehen:

   `\w+-\w+-C([0-9]+)`

   oder

   `\w+-\w+-C(\d+)`

   Beachten Sie, dass diese Ausdrücke nur Beispiele sind. Sie können reguläre Ausdrücke Ihren Bedürfnissen entsprechend erstellen.

   >[!NOTE]
   >
   >Wenn die Kombination aus regulären Ausdrücken für Zeile und Spalte die Position des Assets im multidimensionalen Rotationsset-Array nicht bestimmen kann, wird dieses Asset nicht zum Satz hinzugefügt und ein Fehler wird protokolliert.

1. Geben Sie für „Satzbenennungs- und -erstellungsregel“ das Suffix bzw. Präfix für den Basisnamen an, den Sie in der Asset-Benennungsregel definiert haben. Legen Sie außerdem fest, wo das Bildset in der Adobe Dynamic Media Classic-Ordnerstruktur erstellt wird.

   Wenn Sie eine große Anzahl von Bildsets definieren, trennen Sie diese Sets von den Ordnern, die die Assets selbst enthalten. Zahlreiche Kunden erstellen einen Ordner „Bildsätze“ und weisen die Anwendung an, im Stapelsatz generierte Sätze hier abzulegen.

1. Wählen Sie **[!UICONTROL Save]** im Detailbereich aus.
1. Gehen Sie beim Hochladen und Veröffentlichen des Rotationssets wie gewohnt vor und stellen Sie sicher, dass Sie den Namen des 2D-Rotationssets im Dialogfeld „Auftragsoptionen“ unter „Stapelsatzvorgaben“ aktivieren.

>[!MORELIKETHIS]
>
>* [Asset-Vorschau](previewing-asset.md#previewing_an_asset)
>* [Einrichten von Bildvorgaben](setting-image-presets.md#setting_up_image_presets)
>* [Anzeigen, Hinzufügen und Exportieren von Metadaten](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [Überprüfen von Auftragsdateien](checking-job-files.md#checking_job_files)

