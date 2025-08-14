---
title: Anwendungseinstellungen
description: Erfahren Sie, wie Sie den Anwendungsbereich von Adobe Dynamic Media Classic einrichten und konfigurieren.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
topic: Administration
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '10899'
ht-degree: 29%

---

# Anwendungseinstellungen{#application-setup}

Auf den Seiten „Anwendungseinstellungen“ können Sie allgemeine Einstellungen eingeben, Bildvorgaben erstellen, Videokodierungsvorgaben, Viewer-Vorgaben festlegen oder Standard-Viewer sowie Metadaten definieren. Sie können Stapelsatzvorgaben einrichten, damit sie die Erstellung von 2D-Rotationssets (z. B.), Veröffentlichungseinstellungen und SEO-Videoeinstellungen automatisieren.

>[!NOTE]
>
>Nur Adobe Dynamic Media Classic-Administratoren können die Einstellungen bei der Einrichtung der Anwendung ändern.

## Allgemeine Einstellungen {#general-settings}

Zum Öffnen der Seite „Allgemeine Programmeinstellungen“ über die globale Navigationsleiste navigieren Sie zu **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine]**.

### Server

Bei der Kontoerstellung stellt Adobe Dynamic Media Classic automatisch die zugeordneten Server für Ihr Unternehmen bereit. Diese Server werden verwendet, um URL-Zeichenfolgen für Ihre Website und Programme zu erstellen. Diese URL-Aufrufe sind spezifisch für Ihr Konto.

Siehe auch [Testen des Secure Testing-](testing-assets-making-them-public.md#testing_the_secure_testing_service).

* **[!UICONTROL Veröffentlichungs-Server-Name]**: Dieser Server ist der Live-CDN-Server (Content Deliver Network), der in allen systemgenerierten URL-Aufrufen verwendet wird, die für Ihr Konto spezifisch sind. Ändern Sie diesen Servernamen nur, wenn Sie von einem Adobe Dynamic Media Classic Support-Techniker dazu aufgefordert werden.

* **[!UICONTROL Ursprungs-Server]** Name: Dieser Server wird nur für Qualitätssicherungstests verwendet. Ändern Sie diesen Servernamen nur, wenn Sie von einem Adobe Dynamic Media Classic Support-Techniker dazu aufgefordert werden.

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by an Adobe DynamicMedia Classic support technician. -->

* **[!UICONTROL Test&amp;Target-Server-Name]**: Die Test&amp;Target-URL, einschließlich `.com`. Anweisungen zum Abrufen dieser URL finden Sie unter Integrieren von [!DNL Adobe Dynamic Media Classic] mit [!DNL Adobe Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL iOS Streaming Server-Name]**: Die URL zu Ihrem [!DNL Adobe Dynamic Media Classic] iOS Streaming-Server. Dieser Server stellt Video-Streaming an iOS-basierte Geräte unter Verwendung des HTTP-Protokolls bereit.

* **[!UICONTROL Name des progressiven Video-Servers]**: Die URL zu Ihrem [!DNL Adobe Dynamic Media Classic] progressiven Video-Server. Dieser Server stellt progressive Videos unter Verwendung des HTTP-Protokolls bereit.

* **[!UICONTROL URL für nicht veröffentlichte Assets anzeigen]**: Wählen Sie diese Option aus, wenn Sie [!DNL Adobe Dynamic Media Classic] möchten, dass eine URL bei der Vorschau eines veröffentlichten oder nicht veröffentlichten Assets angezeigt wird. Falls das Asset noch nicht veröffentlicht wurde, funktioniert die URL nicht. Sie können jedoch die URL für Planungs- oder organisatorische Zwecke verwenden.

<!-- **Allow AIR install** Select this option to allow users to download Adobe Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the Web version of Adobe Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Adobe Dynamic Media Classic AIR. Adobe Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL Vorlage für CDN-]**: Gibt die Vorlage an, die zur Invalidierung des CDN-Cache (Content Delivery Network) verwendet wird.

  Angenommen, Sie geben eine Bild-URL (einschließlich Bildvorgaben oder Modifikatoren) ein, die auf `<ID>` verweist, anstatt einer bestimmten Bild-ID, wie im folgenden Beispiel gezeigt:

  `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

  Wenn die Vorlage nur `<ID>` enthält, füllt Adobe Dynamic Media Classic die `https://<server>/is/image` aus, wobei `<server>` der Veröffentlichungsservername ist, der in den allgemeinen Einstellungen definiert ist.

  Wenn Sie die Vorlage für die CDN-Invalidierung festlegen, ein Bild mit dem Namen Backpack_B auswählen und dann zu **[!UICONTROL Datei]** > **[!UICONTROL CDN-Invalidierung]** gehen, wird die folgende URL in der Benutzeroberfläche zur Invalidierung des CDN generiert:

  `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

  Klicken Sie im URL-Listenfeld auf **[!UICONTROL Weiter]**, um den Cache für diesen bestimmten Bild-URL-Aufruf zu löschen. Sie können URLs auch hinzufügen, indem Sie sie in das URL-Listenfeld eingeben oder einfügen. Sie müssen die Vorlage nicht zuvor festlegen.

  Nachdem Sie Ihre Vorlage für CDN-Invalidierung ausgewählt und eine CDN-Invalidierungsanfrage gestellt haben, wird in der Benutzeroberfläche ein Indikator angezeigt. Dadurch erhalten Sie eine Schätzung, wie lange es dauert, den Cache zu löschen.

  Wenn Sie auf **[!UICONTROL Datei]** > **[!UICONTROL CDN-Invalidierung]** klicken, wird jedes Bild in der gespeicherten Vorlagen-URL referenziert, wenn mehrere Bilder in Dynamic Media Classic ausgewählt sind. Daher können Sie eine Vorlage für die CDN-Invalidierung definieren, die auf alle auf Ihrer Website referenzierten URLs (wie Produktdetails, Suchergebnisse) verweist. Wenn Sie dann Bilder auswählen, die im Cache ungültig gemacht werden sollen, werden die URLs automatisch in der Benutzeroberfläche angezeigt.

  Siehe [Inhalts-Caching](dmc-platform-overview.md#content_caching).

  Siehe [Erneut veröffentlichte Assets und CDN-Verzögerungen](publishing-files.md#republished_assets_and_cdn_delays).

### Durchsuchen

* **[!UICONTROL Projekte anzeigen]**: Legt fest, ob Projekte zur Organisation Ihrer Adobe Dynamic Media Classic-Assets verfügbar sind. Siehe [Organisieren der Arbeit mit Projekten](/help/using/organizing-projects.md).

* **[!UICONTROL E-Video-Beispielinhalt anzeigen]**: Aktivieren oder Deaktivieren der Anzeige von E-Video-Beispielinhalten.

* **[!UICONTROL Erzeugten Inhalt anzeigen]**: In Ordnern werden aus einem Asset generierte Inhalte angezeigt. Wenn beispielsweise eine PDF-Datei beim Hochladen gerastert wird, erstellt Adobe Dynamic Media Classic für jede Seite im Original-PDF ein Bild. Wenn Generierte Inhalte anzeigen ausgewählt ist, wird jedes beim Hochladen des Original-PDF generierte Bild angezeigt. Sie wird zusammen mit der PDF in dem Ordner angezeigt, in den die PDF hochgeladen wurde.

* **[!UICONTROL Kodierte Videos anzeigen]**: Standardmäßig deaktiviert.

  Sie können in Adobe Dynamic Media Classic schnell nach Videos suchen und suchen, ohne durch zahlreiche kodierte Ableitungen desselben Videos navigieren zu müssen. Lassen Sie diese Option deaktiviert (Standard). Es werden nur die Primäre Videominiatur (das Quellvideo, das Sie hochgeladen haben und zum Erstellen der Ableitungen verwendet haben) und die übergeordnete Miniatur des adaptiven Videosets (die die „untergeordneten“ Ableitungen des kodierten Videosets enthält) angezeigt.

  Sie können jedoch weiterhin über das Primäre Video oder das adaptive Videoset auf einzelne kodierte Videos zugreifen. Doppelklicken Sie hierzu auf das Videominiaturbild, um die Detailansicht zu öffnen. Wählen Sie dann **[!UICONTROL Kodierte Videos]** im rechten Bereich aus, damit Sie auf alle „untergeordneten“ Videos zugreifen können.

  Sie können auch zu **[!UICONTROL Datei]** > **[!UICONTROL Erneut verarbeiten]** gehen, um mehr codierte „untergeordnete“ Videos direkt aus einem adaptiven Videoset zu erstellen. Adobe Dynamic Media Classic findet automatisch das „übergeordnete“ Primäre Video des adaptiven Videosets und verwendet dieses als Quellvideo für die Transkodierung. Nachdem Sie die neuen, individuell kodierten Videos gespeichert haben, werden sie jedoch nicht angezeigt, wenn Sie nach ihnen suchen. Sie sind jedoch weiterhin über die Registerkarte „Kodierte Videos“ in der Detailansicht verfügbar.

  Siehe [Hochladen und Transkodieren von Videos](uploading-encoding-videos.md#uploading_and_encoding_videos).

  Um auch im Rahmen einer Suche weiterhin auf alle verschlüsselten Videoableitungen zugreifen zu können, aktivieren Sie die Option **[!UICONTROL „Kodierte Videos anzeigen“]**.

  Das Menü „Erstellen“ enthält bestimmte Aktionen, die nur (oder optional) mit einzelnen Videos verwendet werden. Daher müssen alle kodierten Videoableitungen angezeigt werden, aus denen Sie auswählen können, unabhängig davon, wie Sie die Option **[!UICONTROL „Kodierte Videos anzeigen“]** eingestellt haben. Zu den Build-Aktionen, die die Einstellung **[!UICONTROL Kodierte Videos anzeigen]** überschreiben, gehören **[!UICONTROL Adaptive Videosets]** und **[!UICONTROL eCatalogs]**.

  >[!NOTE]
  >
  >Wenn Sie Adobe Dynamic Media Classic nicht zum Hochladen und Kodieren Ihrer Video-Assets verwendet haben, zeigt Adobe Dynamic Media Classic alle Ihre individuellen kodierten Videos an, selbst wenn diese Option deaktiviert ist.

* **[!UICONTROL Schaltfläche Unterordner aktualisieren]**: Aktivieren oder Deaktivieren der Anzeige der Schaltfläche Unterordner aktualisieren.

### Adobe Dynamic Media Classic FTP-Konto

* **[!UICONTROL Server]**: Listet Ihren FTP-Konto-Server auf.

* **[!UICONTROL Benutzername]**: Listet den Benutzernamen Ihres FTP-Kontos auf.

### Zur Anwendung hochladen

Siehe auch [Optionen für Upload-Aufträge](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/569_Default%20Job%20Options_converted%20renamed_Getting%20Started-AVS) Schulungsvideo.

* **[!UICONTROL Bilder überschreiben]**: Adobe Dynamic Media Classic lässt zwei Dateien mit denselben Namen nicht zu. Die Adobe Dynamic Media Classic-ID jedes Elements (der Bildname abzüglich der Dateinamenerweiterung) muss eindeutig sein. Aufgrund dieser Regel enthält das Dialogfeld „Hochladen“ die Option „Überschreiben“. Die genaue Wirkung dieser Option hängt von der Einstellung der Option „Bilder überschreiben“ ab. Sie legen damit fest, was beim Hochladen von Ersatzbildern geschieht – die Ersatzbilder können die Originalbilder ersetzen oder zu Duplikaten werden. Doppelte Bilder werden mit &quot;-1“ umbenannt (beispielsweise wird chair.tif in chair-1.tif umbenannt). Die Optionen wirken sich auf Bilder aus, die in einen vom Originalspeicherort abweichenden Ordner hochgeladen werden bzw. die eine andere Dateierweiterung haben als das Original (beispielsweise JPG, TIF oder PNG). Siehe [Verwenden der Option „Bilder überschreiben](#using-the-overwrite-images-option).

   * **[!UICONTROL Im aktuellen Ordner Bilder mit demselben Namen oder derselben Erweiterung überschreiben]**: Diese Option stellt die strengste Ersetzungsregel dar. Das Ersatzbild muss in den Ordner des Originalbilds hochgeladen werden und dieselbe Dateierweiterung haben wie das Originalbild. Wenn diese Voraussetzungen nicht erfüllt sind, wird ein Duplikat erstellt.

   * **[!UICONTROL Im aktuellen Ordner Assets mit ident. Namen unabh. von Erweiterung überschreiben]**: Erfordert das Hochladen des Ersatzbilds in denselben Ordner wie das Original, die Dateinamenerweiterung kann jedoch vom Original abweichen. Beispiel: „Sessel.tif“ ersetzt die Datei „Sessel.jpg“.

   * **[!UICONTROL In belieb. Ordner Assets mit ident. Namen oder ident. Erweiterung überschreiben]**: Erfordert, dass das Ersatzbild dieselbe Dateinamenerweiterung wie das Originalbild hat. Beispielsweise muss „chair.jpg“ die Datei „chair.jpg“ ersetzen, und nicht „chair.tif“. Sie können das Ersatzbild jedoch in einen anderen Ordner hochladen als den, in dem sich das Original befindet. Das hochgeladene Bild bleibt dann im neuen Ordner; die Datei befindet sich also nicht mehr am ursprünglichen Speicherort.

   * **[!UICONTROL In belieb. Ordner Assets mit ident. Namen unabh. von Erweit. überschreiben]**: Diese Option stellt die am wenigsten einschränkende Ersetzungsregel dar. Sie können ein Ersatzbild in einen anderen Ordner hochladen als den, in dem sich das Originalbild befindet, und eine Datei mit einer anderen Dateierweiterung verwenden, um die Originaldatei zu ersetzen. Wenn sich die Originaldatei in einem anderen Ordner befindet, bleibt das Ersatzbild in dem neuen Ordner, in den es hochgeladen wurde.

* **[!UICONTROL Veröffentlichung beibehalten]**: Gibt an, ob ein in Adobe Dynamic Media Classic hochgeladenes Ersatzbild die Einstellung „Veröffentlichungsbereit“ des Bildes beibehalten soll, das ersetzt wird. Oder die Einstellung wird beim Hochladen angegeben.

* **[!UICONTROL Standardfarbprofile]**: Gibt die Farbprofile an, die als Teil der Standardfarbprofiloptionen beim Hinzufügen von CMYK-Bildern angewendet werden.

* **[!UICONTROL Standard-Uploadoptionen]**: Öffnet das Dialogfeld Upload-Auftragsoptionen, in dem Sie standardmäßige Upload-Optionen angeben können. Informationen zu diesen Optionen finden Sie unter [Upload-Optionen](/help/using/uploading-files.md#upload_options).

### Imagemap-Editor (für die Anwendung)

* **[!UICONTROL Standard-Bildzuordnung HREF]**: Definiert die Standard-URL, die für die HREF-Spalte bei der Bildzuordnung verwendet wird. Diese URL ist die Standard-URL, die beim Erstellen von Imagemaps angezeigt wird.

* **[!UICONTROL Standard-Bildzuordnungsvorlage]**: Definiert die standardmäßige JavaScript für die HREF-Vorlage in der Bildzuordnung. Sie können hier einen benutzerdefinierten Code festlegen, der ausgeführt wird, wenn Sie eine Imagemap auswählen.

### Andere Einstellungen (für Anwendung)

* **[!UICONTROL Papierkorb-Bereinigungswarnungen]**: Assets im Papierkorb werden innerhalb von sieben Tagen automatisch entfernt. Wählen Sie „E-Mails senden, bevor Papierkorb-Elemente automatisch gelöscht werden“ aus, damit Benachrichtigungen an Unternehmensadministratoren gesendet werden, wenn Assets, die sich im Papierkorb befinden, vier Tage von der endgültigen Löschung entfernt sind. Siehe [Verwalten des Papierkorb-Ordners](/help/using/trash-folder.md).

## Verwenden der Option „Bilder überschreiben“ {#using-the-overwrite-images-option}

Adobe Dynamic Media Classic lässt zwei Dateien mit denselben Namen nicht zu. Die Adobe Dynamic Media Classic-ID jedes Elements (der Bildname abzüglich der Dateinamenerweiterung) muss eindeutig sein. Aufgrund dieser Regel enthält das Dialogfeld „Hochladen“ die Option „Bilder überschreiben“. Wie sich diese Option genau auswirkt, hängt von der Einstellung für die internen Adobe Dynamic Media Classic-Einstellungen jedes Unternehmens ab.

Wenn Sie zuvor Bilder hochgeladen und dann die Originaldateien geändert (oder ersetzt) haben, gibt die ausgewählte Option Überschreiben an, wie Adobe Dynamic Media Classic die Bilder ersetzt. Informationen über das Bild bleiben unverändert, aber das neue Bild ersetzt das alte. Wenn der Ordner auch Bilder enthält, die sich noch nicht in Adobe Dynamic Media Classic befinden, werden diese Bilder hinzugefügt.

Verwenden Sie diese Option, wenn die hochgeladenen Bilder in irgendeiner Weise geändert wurden (das Bild wurde geändert), der Verweis auf das Bild jedoch gleich bleibt. Überschreiben ist auch beim Hochladen und Rippen von Adobe®-PDFs hilfreich. Sie können anpassen, wie Adobe Dynamic Media Classic *Bild*. Sie können auch die ICC-Farbprofiloptionen im Dialogfeld Hochladen anpassen und mit der Überschreibungsfunktion erneut hochladen.

Die Adobe Dynamic Media Classic-IDs, die für den Zugriff auf Bilder von den Produktions-Servern verwendet werden, werden von den Bilddateinamen abgeleitet. Die Verwendung von Groß- und Kleinbuchstaben im Dateinamen ist wichtig, sowohl für die Ersetzung vorhandener Dateien als auch für die Adobe Dynamic Media Classic-IDs, die für den Zugriff auf das Bild verwendet werden. Die Verwendung von Dateinamen mit Groß- und Kleinbuchstaben ist vor dem Hochladen in Adobe Dynamic Media Classic korrekt, um zu vermeiden, dass Adobe Dynamic Media Classic-IDs nur für dasselbe Bild in unterschiedlicher Groß-/Kleinschreibung verwendet werden.

Wenn Sie diese Option deaktivieren, werden alle Bilder, die mit vorhandenen Bildern übereinstimmende Dateinamen haben, als Duplikate betrachtet und daher nicht hinzugefügt.

## Bildvorgaben {#image-presets}

In diesem Anzeigebereich können Bildvorgaben erstellt und bearbeitet werden. Mit Bildvorgaben kann Adobe Dynamic Media Classic Bilder dynamisch in verschiedenen Größen vom gleichen Primärbild bereitstellen. Jede Bildvorgabe stellt eine vordefinierte Zusammenstellung von Größen- und Formatierungsbefehlen zum Anzeigen des Bildes dar. Beim Erstellen einer Bildvorgabe wählen Sie eine Größe für die Bildbereitstellung aus. Sie können auch Formatierungsbefehle auswählen, damit das Erscheinungsbild des Bildes optimiert wird, wenn es zur Anzeige bereitgestellt wird.

Administratoren können Vorgaben für das Exportieren von Assets erstellen. Benutzer können beim Exportieren von Bildern eine Vorgabe auswählen, durch die Bilder entsprechend den Spezifikationen des Administrators umformatiert werden.

Wechseln Sie zum Öffnen des Bildschirms Bildvorgabe in der globalen Navigationsleiste zu **[!UICONTROL Einstellungen]** > **[!UICONTROL Bildvorgaben]**.

Siehe [Smart Imaging](https://experienceleague.adobe.com/de/docs/experience-manager-65/content/assets/dynamic/imaging-faq).

### Erstellen und Bearbeiten von Bildvorgaben {#creating-and-editing-image-presets}

1. Navigieren Sie **[!UICONTROL Setup]** > **[!UICONTROL Bildvorgaben]**.
1. Erstellen Sie eine Vorgabe oder beginnen Sie mit einer vorhandenen:

   * **Erstellen einer Bildvorgabe**: Wählen Sie **[!UICONTROL Hinzufügen]**.
   * **Erstellen einer Bildvorgabe aus einer vorhandenen Vorgabe**: Wählen Sie die Bildvorgabe aus, die der am meisten ähnelt, die Sie erstellen möchten, und klicken Sie dann auf **[!UICONTROL Bearbeiten]**.

1. Geben Sie auf der Seite Vorgabe hinzufügen (oder bearbeiten) einen Namen für die Vorgabe ein.
1. Legen Sie die gewünschten Einstellungen für die Vorgabe fest. 

   Siehe [Bildvorgabeoptionen](application-setup.md#image_preset_options).

1. Wählen Sie **[!UICONTROL Speichern]** oder, wenn Sie mit einer vorhandenen Vorgabe begonnen haben, wählen Sie **[!UICONTROL Speichern unter]**.
1. Um eine Vorschau der Vorgabe mit Ihrem eigenen Bild anzuzeigen, wählen Sie **[!UICONTROL Durchsuchen]** und dann ein Bild aus. Um eine Vorschau mit dem Standardbild anzuzeigen, klicken Sie auf **[!UICONTROL Zurücksetzen]**.

Sie können eine Bildvorgabe bearbeiten, indem Sie auf dem Bildschirm „Bildvorgaben“ auf ihren Namen klicken und dann auf **[!UICONTROL Bearbeiten]** klicken. Um eine Bildvorgabe zu löschen, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Löschen]**.

### Optionen für Bildvorgaben {#image-preset-options}

Der Anzeigebereich „Vorgabe hinzufügen“ bzw. „Vorgabe bearbeiten“ bietet folgende Optionen zum Erstellen bzw. Bearbeiten von Bildvorgaben:

* **[!UICONTROL Vorgabenname]**: Geben Sie einen beschreibenden Namen ohne Leerzeichen ein. Um Benutzenden zu helfen, diese Bildvorgabe zu identifizieren, nehmen Sie die Bildgrößenspezifikation in den Namen auf.

* **[!UICONTROL Breite und Höhe]**: Geben Sie die Größe, mit der das Bild bereitgestellt wird, in Pixeln an.

* **[!UICONTROL Format]**: Wählen Sie im Menü ein Format aus. Wenn Sie das GIF-, JPEG-, PDF- oder TIFF-Format auswählen, werden weitere Optionen angezeigt:

   * GIF-Farbquantisierungsoptionen

      * **[!UICONTROL Typ]**: Wählen Sie „Adaptiv“ (Standard), „Web“ oder &quot;Mac&quot;. Wenn Sie **[!UICONTROL GIF mit Alpha]** auswählen, ist die Option &quot;Mac&quot; nicht verfügbar.

      * **[!UICONTROL Dithering]**: Wählen Sie Diffus oder Aus.

      * **[!UICONTROL Anzahl Farben]**: Ziehen Sie den Schieberegler, um 2-255 einzugeben.

      * **[!UICONTROL Farbliste]**: Geben Sie eine kommagetrennte Liste ein. Geben Sie beispielsweise für Weiß, Grau und Schwarz &quot;`000000,888888,ffffff`&quot; ein.

   * JPEG-Optionen

      * **[!UICONTROL Qualität]**: Steuert den JPEG-Komprimierungsgrad. Diese Einstellung wirkt sich sowohl auf die Dateigröße als auch die Bildqualität aus. Die JPEG-Qualitätsskala reicht von 1 bis 100.

      * **[!UICONTROL JPG-Neuberechnung der Chrominanz aktivieren]**: Da das Auge weniger empfindlich auf hochfrequente Farbinformationen reagiert als hochfrequente Luminanz, unterteilen JPEG-Bilder Bildinformationen in Luminanz- und Farbkomponenten. Bei der Komprimierung eines JPEG-Bildes behält die Leuchtdichtekomponente die volle Auflösung, während für die Farbkomponenten ein Downsampling, d. h. eine Mittelwerterstellung für Pixelgruppen, ausgeführt wird. Durch Downsampling wird das Datenvolumen um die Hälfte oder ein Drittel reduziert, ohne dass es zu Qualitätseinbußen kommt. Downsampling kann nicht auf Graustufenbilder angewendet werden. Mit dieser Technik wird der Komprimierungsgrad, der für Bilder mit hohem Kontrast (z. B. Bilder mit überlappendem Text) sinnvoll ist, reduziert.

   * PDF- und TIFF-Optionen

      * **[!UICONTROL Komprimierung]**: Wählen Sie einen Komprimierungsalgorithmus aus.

* **[!UICONTROL Farbraum]**: Wählen Sie einen Farbraum aus.

* **[!UICONTROL Scharfzeichnen]**: Wählen Sie die Option Einfaches Scharfzeichnen aktivieren aus, um einen einfachen Scharfzeichnungsfilter auf das Bild anzuwenden, nachdem die Skalierung abgeschlossen wurde. Wenn ein Bild in einer anderen Größe verschwommen angezeigt wird, kann dieser Effekt durch Scharfzeichnen kompensiert werden.

  Weitere Informationen zum Scharfzeichnen, zum Resample-Modus und zur Unschärfemaske finden Sie unter [Scharfzeichnen eines Bildes](sharpening-image.md#sharpening_an_image). Siehe auch [Scharfzeichnen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) Schulungsvideo.

* **[!UICONTROL Resampling-Modus]**: Wählen Sie eine Option für den Resampling-Modus aus. Mit diesen Optionen wird ein Bild beim Downsampling scharfgezeichnet:

* **[!UICONTROL B-Linear]**: Die schnellste Resampling-Methode. Einige Aliasing-Artefakte sind auffällig.

* **[!UICONTROL Bi-Cubic]**: Erhöht die CPU-Nutzung auf dem Bildserver, liefert jedoch schärfere Bilder mit weniger auffälligen Aliasing-Artefakten.

* **[!UICONTROL `Sharp 2`]**: Kann etwas schärfere Ergebnisse als die Option „Bi-Cubic“ erzeugen, aber zu noch höheren CPU-Kosten auf dem Bildserver.

* **[!UICONTROL Trilinear]**: Verwendet sowohl höhere als auch niedrigere Auflösungen, falls verfügbar; nur empfohlen, wenn ein Alias-Problem auftritt. Bei dieser Methode wird die JPEG-Dateigröße durch Reduzierung der Hochfrequenzdaten verringert.

* **[!UICONTROL Unscharf maskieren]**: Wählen Sie diese Optionen, um das Scharfzeichnen fein abzustimmen:

* **[!UICONTROL Stärke]**: Steuert den auf die Kanten-Pixel angewendeten Kontrastwert. Der Standardwert ist 1,0. Für Bilder mit höherer Auflösung können Sie ihn auf bis zu 5,0 erhöhen. Sie können sich die Auswirkung der Option „Betrag“ wie ein Maß für die Filterintensität vorstellen.

* **[!UICONTROL Radius]**: Bestimmt die Anzahl der Pixel um die Kanten-Pixel, auf die sich die Scharfzeichnung auswirkt. Geben Sie für Bilder mit hoher Auflösung Werte zwischen 1 und 2 ein. Bei einem geringeren Wert werden nur die Kantenpixel scharfgezeichnet, während bei einem hohen Wert ein breiterer Pixelbereich scharfgezeichnet wird. Der richtige Wert hängt von der Größe des Bilds ab.

* **[!UICONTROL Schwellenwert]**: Bestimmt den Kontrastbereich, der beim Anwenden der Unschärfemaske ignoriert werden soll. Das heißt, sie kann auflösen, wie stark sich die scharfgezeichneten Pixel vom Umgebungsbereich unterscheiden müssen, bevor sie als Kantenpixel eingestuft und scharfgezeichnet werden. Um Rauschen zu vermeiden, experimentieren Sie mit Werten zwischen `.02` und `0.2`. Der Standardwert 6 schärft alle Pixel im Bild.

* **[!UICONTROL Farbraum]**: Bestimmt, ob das Bild den Raum verwendet, in dem das Bild erstellt wurde, normalerweise RGB (Original) oder einen Luminanzraum (Intensität).

* **[!UICONTROL Farbe]** Wählen Sie diese Optionen:

* **[!UICONTROL Ausgabefarbprofil]**: Wählen Sie **[!UICONTROL Standard verwenden]** oder eines der in Adobe Dynamic Media Classic verfügbaren ICC-Farbprofile aus.

  Siehe auch [ICC-Profile](icc-profiles.md#icc_profiles).

* **[!UICONTROL Rendering Intent]**: Wählen Sie eine Option aus, wenn Sie den standardmäßigen Rendering-Intent des Farbprofils überschreiben möchten. Verwenden Sie diese Option, wenn eines der standardmäßigen ICC-Profile der Zielfarbraum einer Farbkonvertierung ist. Oder dieses Profil charakterisiert das Ausgabegerät (Drucker oder Monitor), und der angegebene Rendering-Intent ist für dieses Profil gültig.

* **[!UICONTROL Einbettungsprofil]**: Wählen Sie diese Option aus, damit dieses Profil verwendet wird, wenn Sie dieses Bild in Adobe® Photoshop® öffnen.

* **[!UICONTROL Druckauflösung]**: Wählen Sie eine Auflösung für das Drucken dieses Bildes aus. Der Standardwert lautet 72 Pixel.

* **[!UICONTROL URL-Modifikatoren]**: Wenn Sie eher die URL-Modifikatoren angeben möchten, die Ihre Bildvorgabe definieren, als die Einstellungen, geben Sie die Modifikatoren hier ein.

* **[!UICONTROL Beispielbild-URL]**: Listet die „rohe“ URL-Zeichenfolge auf, die der Dynamic Media-Bildserver verwendet, um Bilder mit der Bildvorgabe bereitzustellen, die Sie hinzufügen oder bearbeiten. Diese URL-Zeichenfolge kodiert alle Formateinstellungen, die Sie auf dem Bildschirm „Vorgabe hinzufügen“ oder „Vorgabe bearbeiten“ auswählen.

### Bearbeiten, Entfernen oder Deaktivieren einer Bildvorgabe {#editing-removing-or-deactivating-an-image-preset}

1. Navigieren Sie **[!UICONTROL Setup]** > **[!UICONTROL Bildvorgaben]**.
1. Wählen Sie im Anzeigebereich „Bildvorgaben“ eine Vorgabe aus der Tabelle aus und führen Sie dann einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Bearbeiten]** aus und geben Sie dann im Dialogfeld „Vorgabe bearbeiten“ neue Optionen an.
   * Wählen Sie **[!UICONTROL Löschen]** aus, um die Vorgabe aus der Liste zu entfernen.
   * Deaktivieren Sie das **[!UICONTROL Aktiv]** neben einem Voreinstellungsnamen, wenn Sie ihn aus der gesamten Adobe Dynamic Media Classic-Benutzeroberfläche für MediaPortal-Benutzer entfernen möchten.

## Aktivieren oder Deaktivieren von adaptiven Videovorgaben {#activating-or-deactivating-adaptive-video-presets}

Adobe Dynamic Media Classic bietet Vorgaben für adaptive Videokodierung. Hierbei handelt es sich um eine primäre Liste von Vorgaben, die 16:9 adaptive Videovorgaben und 4:3 adaptive Videovorgaben in einer Gruppe kombiniert. Diese vordefinierten Vorgaben enthalten die am häufigsten verwendeten Kodierungseinstellungen und sind für die Wiedergabe auf Mobilgeräten, Tablets und Desktops optimiert. 

Standardmäßig sind nur „adaptive Video“-Kodierungsvorgaben aktiviert (aktiviert oder aktiviert). Sie können sie bei Bedarf deaktivieren. Deaktivierte adaptive Video-Vorgaben stehen im eVideo-Abschnitt des Dialogfelds „Upload-Auftragsoptionen“ nicht zur Auswahl. 

Siehe [Hochladen und Kodieren von Videos](uploading-encoding-videos.md#uploading_and_encoding_videos).

Siehe auch [Videovorgaben](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) Schulungsvideo.

**So aktivieren oder deaktivieren Sie adaptive Videovorgaben:**

1. Navigieren Sie oben rechts in Adobe Dynamic Media Classic zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinrichtung]** > **[!UICONTROL Videovorgaben]** > **[!UICONTROL Adaptive Videovorgaben]**.
1. Wenn Sie eine Vorgabe aus der Liste „eVideo-Optionen“ im Dialogfeld „Upload-Auftragsoptionen“ entfernen möchten, deaktivieren Sie auf der Seite „Adaptive Video-Vorgaben“ das Kontrollkästchen neben dem Vorgabenamen.
1. Wählen Sie **[!UICONTROL Schließen]** aus.

## Video-Vorgaben zum Kodieren von Videodateien {#video-presets-for-encoding-video-files}

Um eine Kodierungsvorgabe auszuwählen, wählen Sie in der rechten unteren Ecke der Seite „Hochladen“ **[!UICONTROL Auftragsoptionen]**. Erweitern Sie im Dialogfeld Upload-Auftragsoptionen den Eintrag eVideo-Optionen und wählen Sie die gewünschten Videokodierungsvorgaben aus.

>[!NOTE]
>
>Mit Ausnahme von „Adaptives Video“, das standardmäßig aktiviert ist, können im Dialogfeld Upload-Auftragsoptionen nicht alle anderen Vorgaben für adaptive Videos oder einzelne Videokodierung angezeigt werden. Adobe Dynamic Media Classic-Admins legen fest, welche Videokodierungsvorgaben im Dialogfeld Upload-Auftragsoptionen angezeigt werden.

* Wählen Sie aus den folgenden Vorgaben für adaptive Videokodierung oder Einzelkodierung aus:

   * **[!UICONTROL 16:9 Adaptive Video]**: Erstellen Sie Videos mit einem Seitenverhältnis von 16 :9 für die Bereitstellung auf Desktops, Mobilgeräten (iPhone, iPad, Android™) und Tablets (iPad, Android™), optimiert mit der Auflösung und Bitrate, die der Verbindungsgeschwindigkeit des Viewers am besten entspricht.

   * **[!UICONTROL 4:3 Adaptives Video]**: Erstellen Sie Videos mit einem Seitenverhältnis von 4 :3 für die Bereitstellung auf Desktops, Mobilgeräten (iPhone, iPad, Android™) und Tablets (iPad, Android™), optimiert mit der Auflösung und Bitrate, die der Verbindungsgeschwindigkeit des Viewers am besten entspricht.

   * **[!UICONTROL Adaptives Video]**: Eine Vorgabe für die einzelne Kodierung, die mit jedem Seitenverhältnis verwendet werden kann, um Videos für die Bereitstellung auf Mobilgeräten, Tablets und Desktops zu erstellen. Hochgeladene Quellvideos, die mit dieser Vorgabe kodiert wurden, weisen eine feste Höhe auf. Die Breite wird jedoch automatisch skaliert, um das Seitenverhältnis des Videos beizubehalten.

     Diese Flexibilität der „automatischen Skalierung“ ist auch standardmäßig verfügbar, wenn Sie Ihre eigene benutzerdefinierte Videokodierungsvorgabe erstellen.

     Siehe [Hinzufügen oder Bearbeiten einer Videocodierungsvorgabe](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   * **[!UICONTROL Adaptive Videokodierung (16:9 oder 4:3)]**: Erstellen Sie sowohl :9- als auch :3-Videos für die Bereitstellung auf Desktops, Mobilgeräten (iPhone, iPad, Android™) und Tablets (iPad, Android™). Optimiert mit der Auflösung und Bitrate, die der Verbindungsgeschwindigkeit des Viewers am besten entspricht.

     Siehe [Adaptive Videokodierung (16:9 oder 4:3) ](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets).

   * **[!UICONTROL Einzelne Kodierungsvorgaben]**

     >[!NOTE]
     >
     >Um Videos auf iPads bereitzustellen, können Sie eine Mobile-Kodierungsvorgabe oder eine Tablet-Kodierungsvorgabe auswählen. Tablet-Vorgaben weisen gewöhnlich eine höhere Auflösung und Qualität auf und sind für den iPad mit seinem größeren Display und der hohen Verbindungsgeschwindigkeit optimiert. Damit Videodateien, die mit einer Tablet-Vorgabe kodiert wurden, richtig wiedergegeben werden können, muss die mobile Site bzw. Anwendung über einen Code zur Geräteerkennung verfügen. Dieser Code sorgt dafür, dass, abhängig vom erkannten Wiedergabegerät, das entsprechende Videomaterial für iPhone oder iPad bereitgestellt wird. Durch die Auswahl einer Mobil-Vorgabe für die Wiedergabe von Videodateien auf dem iPad wird der Workflow vereinfacht. Das liegt daran, dass Sie für iPhones und iPads dieselbe Videodatei verwenden können. Allerdings wird dabei die Qualität des Videomaterials an das iPhone mit seiner geringeren Auflösung angepasst.

      * Wählen Sie unter der Gruppe Kodierungsvorgaben in der Dropdown-Liste Kodierungsvorgaben sortieren den Namen oder die Größe aus, um die Vorgaben nach Name oder Auflösungsgröße zu sortieren.
      * Wählen Sie eine Kodierungsvorgabe aus, die auf der Größe der Auflösung und der Bandbreite basiert, mit der Sie das Video abspielen möchten.
      * Sie können „Adaptive Videokodierung“ und eine oder mehrere Kodierungsvorgaben pro Video auswählen. Beispielsweise können Sie eine Datei beim Hochladen gleichzeitig für Desktop und mobile Geräte kodieren.

Wenn Sie auf **[!UICONTROL Upload starten]** klicken, wird die ursprüngliche Primäre Videodatei hochgeladen und kodierte Dateien werden aus der Primärdatei generiert.

### Kodierungsvorgabeoptionen {#about-encoding-preset-options}

Folgende Parameter stehen für die Kodierungsvorgabeoptionen zur Verfügung:

* **[!UICONTROL Target-Verbindungsgeschwindigkeit]**: Die Internetverbindungsgeschwindigkeit des Zielgruppen-Endbenutzers.

* **[!UICONTROL Codiertes Dateisuffix]**: Das Suffix, das zu Identifizierungszwecken an die codierte Videodatei angehängt wird.

* **[!UICONTROL Video-Bitrate (Datenrate)]**: Die Menge an Daten, die für eine Videowiedergabe von einer einzigen Sekunde kodiert wird (in Kilobit pro Sekunde).

* **[!UICONTROL Pixelbreite/-höhe]**: Die Breitendimension des Bildschirmbilds in Pixel; die Höhendimension des Bildschirmbilds (in Pixel).

* **[!UICONTROL Frame pro Sekunde (fps]**: Die Anzahl der Frames oder Standbilder pro Sekunde des Videos. In den USA und Japan werden die meisten Videos mit 29,97 fps aufgenommen und in Europa und Asien (ausgenommen Japan) mit 25 fps. Der Film wird mit 24 fps gedreht.

* **[!UICONTROL Audio-Bitrate]**: Die kodierte Datenmenge, aus der eine einzelne Sekunde der Audiowiedergabe besteht, in Kilobit pro Sekunde.

Die folgende Tabelle enthält empfohlene Verfahren zur Auswahl von Video-Vorgaben und die Namenskonventionen, mit denen kodierte Dateien bezeichnet werden.

### Adaptive Video (Standard) {#adaptive-video-default}

Eine Kodierungsvorgabe, die mit jedem Seitenverhältnis verwendet werden kann, um Videos zur Wiedergabe auf Mobilgeräten, Tablets und Desktops zu erstellen. Hochgeladene Quellvideos, die mit dieser Vorgabe kodiert wurden (Standard und Best Practice), sind auf eine feste Höhe eingestellt, während die Breite automatisch skaliert wird, um das Seitenverhältnis des Videos beizubehalten.

**Adaptives Video (Standard)**

|  | Kodierungsvorgabenname/QuickInfo-Text | Kodierungsdateisuffix | Videodatenrate (Kbit/s) | Breite/Höhe (Pixel) | fps | Audiobitrate (Kbit/s) | Empfehlungen |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Automatische × 360, 800 kBit/s | _Mobile_Auto×360p_800K | 800 | Auto×360 | Gleich Quelle | 64 | Für Mobilgeräte (iPhone, iPad, Android™) |
| 2 | Auto × 480, 1400 kBit/s | _tablet_auto×480p_1400K | 1400 | Auto×480 | Gleich Quelle | 96 | Für Tablets (iPad, Android™) |
| 3 | Automatische × 720, 2600 kBit/s | _Desktop_Auto×720p_2600K | 2600 | Auto×720 | Gleich Quelle | 128 | Für Desktop |

### Adaptive Videokodierungs-(16:9 oder 4:3)-Vorgaben {#adaptive-video-encoding-or-video-presets}

Diese Vorgaben für adaptive Videokodierung kombinieren eine Reihe individueller Kodierungsvorgaben, die automatisch auf Grundlage des Seitenverhältnisses des hochgeladenen Videos ausgewählt werden. Wenn Sie beispielsweise ein 4:3-Video hochladen, wird es automatisch mit allen fünf 4:3-Vorgaben kodiert, die in der Liste der primären Vorgaben in der Option **Adaptive Videokodierung (16:9 oder 4:3)**.

Informationen zu den Parametern für Kodierungsoptionen finden Sie unter [Kodierungsvorgabeoptionen](application-setup.md#about_encoding_preset_options).

**Vorgaben für adaptive Videokodierung (16:9 oder 4 :3)**

|  | Kodierungsvorgabenname/QuickInfo-Text | Zielverbindungsgeschwindigkeit (Kbit/s) | Kodierungsdateisuffix | Videodatenrate (Kbit/s) | Breite/Höhe (Pixel) | fps | Audiobitrate (Kbit/s) | Empfehlungen |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android&trade;), (400 Kbps)` | 500 | _Mobile_512x288_400K | 400 | 512 x 288 | Gleich Quelle | 64 | Niedrige Auflösung, 3G |
| 2 | `4:3, 384x288px, Mobile (iPhone, iPad, Android&trade;), (400 Kbps)` | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Gleich Quelle | 64 | Niedrige Auflösung, 3G |
| 3 | `16:9, 512x288, Mobile (iPhone, iPad, Android&trade;), (600 Kbps)` | 700 | _Mobile_512x288_600K | 600 | 512 x 288 | Gleich Quelle | 64 | Medium-Auflösung, 3G |
| 4 | `4:3, 384x288, Mobile (iPhone, iPad, Android&trade;), (600 Kbps)` | 700 | _Mobile_384x288_600 | 600 | 384 x 288 | Gleich Quelle | 64 | Medium-Auflösung, 3G |
| 5 | `16:9, 640x360, Tablet (iPad, Android&trade;), (800 Kbps)` | 900 | _iPad_640x360_800K | 800 | 640 x 360 | Gleich Quelle | 80 | Medium-Auflösung, WiFi |
| 6 | `4:3, 640x480, Tablet (iPad, Android&trade;), (800 Kbps)` | 900 | _iPad_640x480_800K | 800 | 640 x 480 | Gleich Quelle | 80 | Medium-Auflösung, WiFi |
| 7 | `16:9, 768x432, Tablet (iPad, Android&trade;), (1200 Kbps)` | 1,5 Mbit/s | _iPad_768x432_1200K | 1200 | 768 x 432 | Gleich Quelle | 96 | Hohe Auflösung, WiFi |
| 8 | `4:3, 768x576, Tablet (iPad, Android&trade;), (1200 Kbps)` | 1,5 Mbit/s | _iPad_768x576_1200K | 1200 | 768 x 576 | Gleich Quelle | 96 | Hohe Auflösung, WiFi |
| 9 | `16:9, 1280x720, Desktop, (2000 Kbps)` | 3,0 Mbit/s | _1280x720_2000K | 2000 | 1280 x 720 | Gleich Quelle | 128 | High Definition, Widescreen |
| 10 | `4:3, 1280x960, Desktop, (2000 Kbps)` | 3,0 Mbit/s | _1280x960_2000K | 2000 Kbit/s | 1280 x 960 | Gleich Quelle | 128 | High Definition |

### Vorgaben für die Videokodierung für Desktop-PCs {#desktop-video-encoding-presets}

Vorgaben für die Videokodierung für MP4 und OGV auf Desktopcomputern.

Informationen zu den Parametern für Kodierungsoptionen finden Sie unter [Kodierungsvorgabeoptionen](application-setup.md#about_encoding_preset_options).

**H264 Main 3.2: Audio-AAC-, MP4-Dateierweiterung**

|  | Kodierungsvorgabenname/QuickInfo-Text | Zielverbindungsgeschwindigkeit (Kbit/s) | Kodierungsdateisuffix | Videodatenrate (Kbit/s) | Breite/Höhe (Pixel) | fps | Audiobitrate (Kbit/s) | Empfehlungen |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9 480 x 270 (400 Kbit/s) | 500 | _480x270_400K | 400 | 480 x 270 | Gleich Quelle | 64 | Niedrige Auflösung, Widescreen |
| 2 | 16:9 640 x 360 (800 kBit/s) | 900 | _640x360_800K | 800 | 640 x 360 | Gleich Quelle | 80 | Mittlere Bildauflösung, Widescreen |
| 3 | 16:9 800 x 450 (1200 Kbit/s) | 1,5 Mbit/s | _800x450_1200K | 1200 | 800 x 450 | Gleich Quelle | 96 | Mittelhohe Auflösung |
| 4 | 16:9 1280 x 720 (2000 Kbit/s) | 3,0 Mbit/s | _1280x720_2000K | 2000 | 1280 x 720 | Gleich Quelle | 128 | High Definition, Widescreen |
| 5 | 4:3, 320 x 240 (400 Kbit/s) | 500 | _320X240_400K | 400 | 320 x 240 | Gleich Quelle | 64 | Niedrige Auflösung |
| 6 | 4:3, 480 x 360 (800 kBit/s) | 900 | _480x360_800K | 800 | 480 x 360 | Gleich Quelle | 80 | Mittlere Auflösung |
| 7 | 4 :3 640 x 480 (1200 Kbit/s) | 1,5 Mbit/s | _640x480_1200K | 1200 | 640 x 480 | Gleich Quelle | 96 | Mittlere Auflösung |
| 8 | 4:3, 1280 x 960 (2000 Kbit/s) | 3,0 Mbit/s | _1280x960_2000K | 2000 | 1280 x 960 | Gleich Quelle | 128 | High Definition |

**OGG Theora Vorbis: Dateiendung OGV**

|  | Kodierungsvorgabenname/QuickInfo-Text | Zielverbindungsgeschwindigkeit (Kbit/s) | Kodierungsdateisuffix | Videodatenrate (Kbit/s) | Breite/Höhe (Pixel) | fps | Audiobitrate (Kbit/s) | Empfehlungen |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 480 x 270 (400 Kbit/s), OGG | 500 | _OGG_480x270_400K | 400 | 480 x 270 | Gleich Quelle | 64 | Niedrige Auflösung, Widescreen |
| 2 | 16:9, 640 x 360 (800 Kbit/s), OGG | 900 | _OGG_640x360_800K | 800 | 640 x 360 | Gleich Quelle | 80 | Mittlere Bildauflösung, Widescreen |
| 3 | 16:9, 800 x 450 (1200 Kbit/s), OGG | 1,5 Mbit/s | _OGG_800x450_1200K | 1200 | 800 x 450 | Gleich Quelle | 96 | Mittelhohe Auflösung |
| 4 | 16:9, 1280 x 720 (2000 Kbit/s), OGG | 3,0 Mbit/s | _OGG_1280x720_2000K | 2000 | 1280 x 720 | Gleich Quelle | 128 | High Definition, Widescreen |
| 5 | 4:3, 320 x 240 (400 Kbit/s), OGG | 500 | _OGG_320X240_400K | 400 | 320 x 240 | Gleich Quelle | 64 | Niedrige Auflösung |
| 6 | 4:3, 480 x 360 (800 Kbit/s), OGG | 900 | _OGG_480x360_800K | 800 | 480 x 360 | Gleich Quelle | 80 | Mittlere Auflösung |
| 7 | 4:3, 640 x 480 (1200 Kbit/s), OGG | 1,5 Mbit/s | _OGG_640x480_1200K | 1200 | 640 x 480 | Gleich Quelle | 96 | Mittlere Auflösung |
| 8 | 4:3, 1280 x 960 (2000 Kbit/s), OGG | 3,0 Mbit/s | _OGG_1280x960_2000K | 2000 | 1280 x 960 | Gleich Quelle | 128 | High Definition |

### Vorgaben für die Videokodierung für Mobilgeräte {#mobile-video-encoding-presets}

Gleich wie Bildrate der Quelle. Videokodierungsvorgaben für iPhone, iPad und Android™-Mobilgeräte.

Informationen zu den Parametern für Kodierungsoptionen finden Sie unter [Kodierungsvorgabeoptionen](application-setup.md#about_encoding_preset_options).

**H264 Baseline 2.1: Audio-AAC-, MP4-Dateierweiterung**

|  | Kodierungsvorgabenname/QuickInfo-Text | Zielverbindungsgeschwindigkeit (Kbit/s) | Kodierungsdateisuffix | Videobitrate (Kbit/s) | Pixel Breite/Höhe | fps | Audiobitrate (Kbit/s) | Empfehlungen |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9, 512 x 288, Mobil (400 kBit/s) | 500 | _Mobile_512x288_400K | 400 | 512 x 288 | Gleich Quelle | 64 | Niedrige Auflösung, 3G |
| 2 | 16:9, 512 x 288, Mobil (600 kBit/s) | 700 | _Mobile_512x288_600K | 600 | 512 x 288 | Gleich Quelle | 64 | Medium-Auflösung, 3G |
| 3 | 16:9, 512 x 288, Mobil (800 kBit/s) | 900 | _Mobile_512x288_800K | 800 | 512 x 288 | Gleich Quelle | 80 | Medium-Auflösung, Wi-Fi |
| 4 | 16:9, 512 x 288, Mobil (1000 Kbit/s) | 1,2 Mbit/s | _Mobile_512x288_1000K | 1000 | 512 x 288 | Gleich Quelle | 80 | Hohe Auflösung, Wi-Fi |
| 5 | 16:9, 512 x 288, Mobil (1200 Kbit/s) | 1,5 Mbit/s | _Mobile_512x288_1200K | 1200 | 512 x 288 | Gleich Quelle | 96 | Hohe Auflösung, Wi-Fi |
| 6 | 4:3, 384 x 288, Mobil (400 kBit/s) | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | Gleich Quelle | 64 | Niedrige Auflösung, 3G |
| 7 | 4:3, 384 x 288, Mobil (600 kBit/s) | 700 | _Mobile_384x288_600K | 600 | 384 x 288 | Gleich Quelle | 64 | Medium-Auflösung, 3G |
| 8 | 4:3, 448 x 336, Mobil (800 kBit/s) | 900 | _Mobile_448x336_800K | 800 | 448 x 336 | Gleich Quelle | 80 | Medium-Auflösung, Wi-Fi |
| 9 | 4:3, 448 x 336, mobil (1000 Kbit/s) | 1,2 Mbit/s | _Mobile_448x336_1000K | 1000 | 448 x 336 | Gleich Quelle | 80 | Hohe Auflösung, Wi-Fi |
| 10 | 4:3, 448 x 336, mobil (1200 Kbit/s) | 1,5 Mbit/s | _Mobile_448x336_1200K | 1200 | 448 x 336 | Gleich Quelle | 96 | Hohe Auflösung, Wi-Fi |

## Viewer-Vorgaben {#viewer-presets}

>[!NOTE]
>
>**Hinweis zum Ende der Nutzungsdauer von Flash-Viewern**: Am 31. Januar 2017 hat Adobe Dynamic Media Classic offiziell die Unterstützung für die Flash-Viewer-Plattform beendet.

Eine *Viewer-Vorgabe* ist eine Zusammenstellung von Einstellungen, mit denen die Anzeige von Rich-Media-Assets auf den Computerbildschirmen und Mobilgeräten für die Benutzer festgelegt wird. Sie können als Administrator Viewer-Vorgaben erstellen. Es sind Einstellungen für eine ganze Palette von Viewer-Konfigurationsoptionen verfügbar. Sie können beispielsweise die Viewer-Anzeigegröße, das Zoomverhalten, die Farbschemata, Ränder und Schriftarten ändern.

Verwenden Sie als Best Practice Adobe Dynamic Media Classic HTML5-Video-Viewer. Die in HTML5-Video-Viewern verwendeten Vorgaben sind robuste Video-Player.

Durch die Kombination von Folgendem in einen einzelnen Player:

* Die Möglichkeit, die Wiedergabekomponenten mithilfe von HTML5 und CSS zu entwerfen.
* Eingebettete Wiedergabe
* Verwenden Sie adaptives und progressives Streaming je nach Browser-Funktion.

Sie erweitern die Reichweite Ihrer Rich-Media-Inhalte auf Desktop-, Tablet- und mobile Benutzer und stellen ein optimiertes Videoerlebnis sicher.

Siehe [Über HTML5-Viewer](https://experienceleague.adobe.com/de/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only) im Adobe Viewers-Referenzhandbuch.

Siehe Kompatibilitätsmatrix für Adobe Dynamic Media Classic-Viewer-Vorgaben[.](application-setup.md#scene7_viewer_preset_compatibility_matrix)

Siehe [Optimale Vorgehensweise: Verwenden des HTML5-Video-Viewers](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer).

Abhängig vom Viewer können Sie Community-Funktionen hinzufügen. Zu den Community-Funktionen zählen die Schaltflächen „Einbetten“, „E-Mail an Freunde senden“, „Verknüpfen“ und „Zur Website“. Mit diesen Schaltflächen können Benutzer, die die Viewer verwenden, den Viewer für andere freigeben oder die Adobe Dynamic Media Classic-Website öffnen.

Siehe auch [Adobe Viewers-Referenzbibliotheksbeispiele](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### Viewer-Unterstützung für Web-Seiten mit responsivem Design {#viewer-support-for-responsive-designed-web-pages}

Verschiedene Web-Seiten haben unterschiedliche Anforderungen. Manchmal benötigen Sie eine Web-Seite mit einem Link, über den der HTML5-Viewer in einem separaten Browserfenster geöffnet wird. In anderen Fällen ist es erforderlich, den HTML5-Viewer direkt auf der Hosting-Seite einzubetten. Im letzteren Fall weist die Web-Seite wahrscheinlich ein statisches Layout auf. Oder sie ist „responsiv“ und wird auf verschiedenen Geräten oder in verschiedenen Browser-Fenstergrößen unterschiedlich angezeigt. Um diesen Anforderungen gerecht zu werden, unterstützen die HTML5-Viewer, die mit Adobe Dynamic Media Classic geliefert werden, sowohl statische Web-Seiten als auch Web-Seiten mit responsivem Design.

Weitere Informationen zum Einbetten responsiver Viewer auf Webseiten finden Sie unter [Informationen zur Bibliothek responsiver Bilder](https://experienceleague.adobe.com/de/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library#image-serving-api), [Verwenden der Bibliothek responsiver ](https://experienceleague.adobe.com/de/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library#image-serving-api)) und [Befehlsreferenz: Befehlsattribute](https://experienceleague.adobe.com/de/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library#responsive-static-image-library).

### Viewer-Vorgabentypen {#viewer-preset-types}

Administratoren können die folgenden Arten von Viewer-Vorgaben erstellen und anpassen:

* **[!UICONTROL eCatalog Viewer]**: Simuliert das Lesen eines gedruckten Katalogs. Sie können von Seite zu Seite wechseln, Elemente auf einer Seite vergrößern und verkleinern, Imagemaps verwenden, um weitere Informationen zu Elementen auf der Seite anzuzeigen, oder den Katalog durchsuchen. Sie können auch ein Informationsbedienfeld einbeziehen, um detaillierte Informationen anzuzeigen, und ein bildgemapptes Element, wenn der Zuordnungsbereich ein gültiges rollover_key -Attribut aufweist. Um ein Informationsbedienfeld einzuschließen, geben Sie eine Informationsserver-URL im Bedienfeld „Einstellungen“ des Fensters „eCatalog Viewer-Vorgabe“ an.

* **[!UICONTROL Musterset-Viewer]**: Zeigt ein Bild in einer anderen Farbe, einem anderen Material, einer anderen Textur, einer anderen Oberfläche oder einem anderen Stoff an. Benutzer wählen eine Miniatur aus, um die Varianten im Bild anzuzeigen.

* **[!UICONTROL Viewer für gemischte Mediensets]**: Zeigt verschiedene Medientypen in einem Viewer an. Sie können darin Mustersets, Rotationssets, Bilder und Videos einschließen. Sie können Registerkarten so einrichten, dass sie verschiedene Inhaltstypen enthalten, z. B. eine Registerkarte für Bildsets und eine Registerkarte für Videos. Videos, die von einem gemischten Medienset wiedergegeben werden, verwenden einen standardmäßigen Video-Viewer mit einer Timeline und Video-Steuerelementen wie Stoppen, Pause, Zurückspulen und Abspielen. Beim Einrichten einer Viewer-Vorgabe für gemischte Mediensets geben Sie an, welche Viewer Sie für die verschiedenen Asset-Typen in Ihrem gemischten Medienset verwenden möchten. Sie können auch den Raster-Viewer oder den Karussell-Viewer verwenden, um ein gemischtes Medienset anzuzeigen.

* **[!UICONTROL Rotationsset-Viewer]**: Bietet mehrere Ansichten eines Bildes, sodass Benutzende das Objekt drehen können, um die verschiedenen Seiten und Winkel zu untersuchen.

* **Video-Viewer**: Zeigt Videos anhand der Auflösungsabmessungen der Quelldatei oder einer benutzerdefinierten Größe an. Adobe Dynamic Media Classic verfügt über viele vordefinierte Viewer-Vorgaben für die Videowiedergabe. Wenn Sie Administrator sind, können Sie benutzerdefinierte Video-Viewer-Vorgaben erstellen. Es gibt mehr als 12 verschiedene Einstellungen zum Konfigurieren des Video-Viewers. Sie können die folgenden Optionen konfigurieren:

   * Größe
   * Vordergrund- und Hintergrundfarbe
   * Video- und Audiosteuerelemente
   * Fortschrittsbalken
   * User-Interface Skin
   * Social-Media-Funktionen
   * und Hilfe

* **[!UICONTROL Zoom-Viewer]**: Bietet eine Auswahl von drei Arten von Zoom-Viewer:

* **[!UICONTROL Zoom-Viewer]**: Ermöglicht Benutzern das Zoomen in den Bereich durch Auswahl. Sie können Steuerelemente auswählen, um ein- und auszuzoomen und das Bild auf die Standardgröße zurückzusetzen.

* **[!UICONTROL Zoom-Viewer:]**-Out: Zeigt ein zweites Bild des gezoomten Bereichs neben dem Originalbild an. Der Benutzer hat keine Steuerelemente zur Verfügung. Er bewegt einfach die Auswahl über den Bereich, der angezeigt werden soll.

Bedenken Sie bei der Festlegung der gesamten Bandbreitennutzung für diesen Viewer, dass sowohl das Hauptbild als auch das Flyout-Bild im Viewer geladen werden müssen. Die Größe des Hauptbildes (Anzeigenbreite und -höhe) und der Zoomfaktor bestimmen die Größe des Flyout-Bildes. Setzen Sie diese beiden Werte gut in Relation, damit das Flyout-Bild eine kompakte Dateigröße erhält. Wenn beispielsweise die Hauptbilddatei sehr groß ist, verringern Sie den Wert für den Zoomfaktor. (Die Flyout-Breite und Flyout-Höhe bestimmen die Größe des Flyout-Fensters, aber nicht die Größe des Flyout-Bildes, das in den Viewer geladen wird.)

Wenn die Größe des Hauptbildes beispielsweise 350 x 350 Pixel bei einem Zoomfaktor von 3 beträgt, ist das Flyout-Bild 1050 x 1050 Pixel groß. Wenn die Größe des Hauptbildes 300 x 300 Pixel bei einem Zoomfaktor von 4 beträgt, ist das Flyout-Bild 1200 x 1200 Pixel groß. Über die Einstellung für die JPEG-Qualität (empfohlener Wert: zwischen 80 und 90) können Sie die Dateigröße deutlich reduzieren. Der empfohlene Wert für den Zoomfaktor liegt, je nach Größe des Hauptbildes, zwischen 2,5 und 4.

### Kompatibilitätsmatrix für Adobe Dynamic Media Classic-Viewer-Vorgaben {#scene-viewer-preset-compatibility-matrix}

**Hinweis zum Ende der Nutzungsdauer von Flash-Viewern**: Am 31. Januar 2017 hat Adobe Dynamic Media Classic offiziell die Unterstützung für die Flash-Viewer-Plattform beendet.

In der folgenden Tabelle sind die derzeit verfügbaren Adobe Dynamic Media Classic-Viewer-Vorgaben aufgeführt. Die Tabelle gibt auch die Kompatibilität des Viewers mit Desktop- und Mobilgeräten sowie die für jeden Viewer verwendete Technologie an.

Siehe auch [Adobe Viewers-Referenzbibliotheksbeispiele](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

Informationen zu unterstützten Webbrowser- und Betriebssystemversionen für Viewer finden Sie in den Versionshinweisen zu Viewern .

Siehe [Adobe Viewers-Referenz - Versionshinweise](https://experienceleague.adobe.com/de/docs/dynamic-media-developer-resources).

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Zoom-Viewer |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Bildset-Viewer |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Musterset-Viewer |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| E-Katalog-Viewer |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv(Unterstützt Social Media und die Katalogsuche.) | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog(Unterstützt Social Media und die Katalogsuche.) | HTML5 | X | X | X | X | X |

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Viewer drehen |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**eVideo-Viewer**

Adobe Dynamic Media Classic unterstützt die mobile Videowiedergabe für MP4 H.264-Videos.

* Welche BlackBerry®-Geräte dieses Videoformat unterstützen, können Sie hier einsehen: [Unterstützte Videoformate für BlackBerry®](https://developers.blackberry.com/us/en)
* Welche Windows®-Geräte dieses Videoformat unterstützen, können Sie hier einsehen: [Unterstützte Videoformate unter Windows® Phone](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ Tablet | BlackBerry® Smartphone | Windows® Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video(Enthält Unterstützung für verdeckte Untertitel.) Siehe [Best Practice: Verwenden des universellen HTML5-Video-Viewers.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social(Enthält Unterstützung für verdeckte Untertitel und soziale Medien.) | HTML5 | X | X | X | X | X | X | X |

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Viewer für gemischte Mediensets |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### Übersicht über die unterstützten Gesten für Mobilgeräte-Viewer {#supported-mobile-viewers-gestures-matrix}

In der folgenden Tabelle werden die Mobile-Viewer-Gesten aufgeführt, die auf iOS-, Android™ 2.x- und Android™ 3.x-Geräten unterstützt werden.

|  | Viewer-Technologie | Desktop | Apple iPhone | Apple iPad | Android™ Smartphone | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| Bildset-Viewer |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### Anzeigebereich „Viewer-Vorgaben“ {#about-the-viewer-preset-screen}

Über den Anzeigebereich „Viewer-Vorgaben“ erstellen und verwalten Sie Viewer-Vorgaben. Wechseln Sie zum Öffnen dieses Bildschirms zu **[!UICONTROL Einstellungen]** > **[!UICONTROL Viewer-Vorgaben]**.

Der Anzeigebereich „Viewer-Vorgaben“ umfasst Werkzeuge für die folgenden Aufgaben:

* **Vorgabe hinzufügen**: Wählen Sie **[!UICONTROL Hinzufügen]** und wählen Sie im Dialogfeld „Viewer-Vorgabe hinzufügen“.

      Siehe [Viewer-Vorgaben hinzufügen und bearbeiten](application-setup.md#adding_and_editing_viewer_presets).
  
* **Bearbeiten einer Vorgabe**: Wählen Sie eine Vorgabe aus und klicken Sie dann auf **[!UICONTROL Bearbeiten]**.

      Siehe [Viewer-Vorgaben hinzufügen und bearbeiten](application-setup.md#adding_and_editing_viewer_presets).
  
* **Vorgabe löschen**: Wählen Sie eine Vorgabe aus und klicken Sie dann auf **[!UICONTROL Löschen]**.

* **Eine Vorgabe exportieren**: Wählen Sie eine HTML5-Viewer-Vorgabe aus. Klicken Sie anschließend auf **[!UICONTROL Exportieren]**, um das Viewer-Design herunterzuladen und als Grundlage zum Erstellen und Hinzufügen einer weiteren Viewer-Vorgabe zu verwenden.

      Siehe [Exportieren einer HTML5-Viewer-Vorgabe](application-setup.md#export_an_html5_viewer_preset).
  
* **Viewer-Vorgabeliste filtern**: Verwenden Sie diese Tools, um die Liste zu filtern:

      * Öffnen Sie die Dropdown&#x200B;**Liste „Aktiv/Inaktiv** und wählen Sie eine Option aus, um aktive Vorgaben, inaktive Vorgaben oder alle Vorgaben anzuzeigen.
     * Öffnen Sie die **Viewer**-Dropdown-Liste und wählen Sie eine Option aus, um nur Viewer einer bestimmten Art anzuzeigen. Wählen Sie **[!UICONTROL Alle Viewer]** aus, um alle Viewer anzuzeigen.
  
* **Sortiervorgaben**: Wählen Sie eine Spaltenüberschrift aus (**[!UICONTROL Aktiv]**, **[!UICONTROL Typ]**, **[!UICONTROL Vorgabe]** oder **[!UICONTROL Plattform]**), um die Liste in einer Spalte zu sortieren. Wählen Sie ein zweites Mal eine Spaltenüberschrift aus, um die Liste in absteigender (oder aufsteigender) Reihenfolge zu sortieren.

* **Aktivieren und Deaktivieren von Vorgaben**: Wählen Sie eine Vorgabe aus und wählen Sie dann ihre Option „Aktiv“ aus, um sie zu aktivieren oder zu deaktivieren.

      Siehe [Aktivieren oder Deaktivieren von Viewer-Vorgaben](application-setup.md#activate_or_deactivate_viewer_presets).
  
>[!NOTE]
>
>Wählen Sie **[!UICONTROL Vorschau]** auf der rechten Seite der Seite „Viewer-Vorgaben“ aus, um zu sehen, wie ein Asset in der ausgewählten Viewer-Vorgabe aussieht. Um ein anderes Asset anzuzeigen, wählen Sie **[!UICONTROL Durchsuchen]** auf der Seite „Viewer-Vorgaben“ und wählen Sie im Dialogfeld Asset-Vorschau auswählen ein anderes Asset aus.

### Hinzufügen und Bearbeiten von Viewer-Vorgaben {#adding-and-editing-viewer-presets}

Neben dem Hinzufügen von Viewer-Vorgaben mit **[!UICONTROL Hinzufügen]** in der Benutzeroberfläche können Sie auch **[!UICONTROL Exportieren]** zum Hinzufügen einer Viewer-Vorgabe verwenden. Sie exportieren einfach eine vorhandene HTML5-Viewer-Vorgabe und verwenden diese dann als Grundlage für die neue Vorgabe.

Siehe [Export von HTML5-Viewer-](application-setup.md#exporting_an_html5_viewer_preset).

Siehe auch [Video ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS)Viewer-Vorgaben“.

**So fügen Sie Viewer-Vorgaben hinzu und bearbeiten sie:**

1. Navigieren Sie oben rechts in Adobe Dynamic Media Classic zu **[!UICONTROL Einstellungen]** > **[!UICONTROL Viewer-Vorgaben]**.

   Sie können die Liste der Vorgaben filtern. Wenn nur Vorgaben für Video-Viewer aufgelistet werden sollen, wählen Sie auf der Symbolleiste direkt über der Tabelle in der Dropdown-Liste „Viewer“ die Option „Video-Viewer“ aus.

1. Fügen Sie auf der Seite „Viewer-Vorgaben“ die Viewer-Vorgabe auf dem Bildschirm „Viewer-Vorgaben“ hinzu oder bearbeiten Sie sie.

   * **Hinzufügen**: Wählen Sie in der Symbolleiste **[!UICONTROL Hinzufügen]** aus. Wählen Sie im Dialogfeld Viewer-Vorgabe hinzufügen eine Plattform und anschließend einen Rich-Media-Asset-Typ aus.

         Wählen Sie **[!UICONTROL Speichern unter]**, wenn Sie die Erstellung der Viewer-Vorgabe abgeschlossen haben.
     
   * **Hinzufügen ausgehend von einer vorhandenen Viewer-Vorgabe**: Wählen Sie in der Tabelle eine Video-Viewer-Vorgabe aus und klicken Sie dann in der Symbolleiste auf **[!UICONTROL Bearbeiten]**.

         Nachdem Sie den Video-Viewer neu konfiguriert haben, wählen Sie **[!UICONTROL Speichern unter]** aus, um die Vorgabe unter Verwendung eines anderen Namens im Textfeld „Vorgabenname“ zu speichern.
     
   * **Bearbeiten**: Wählen Sie eine vorhandene Viewer-Vorgabe aus und klicken Sie dann auf **[!UICONTROL Bearbeiten]**.

1. Geben Sie auf der Seite „Viewer konfigurieren“ im Feld „Vorgabenname“ den Namen der Vorgabe ein bzw. bearbeiten Sie ihn.
1. Legen Sie die weiteren gewünschten Optionen fest.

   >[!NOTE]
   >
   >Wählen Sie **[!UICONTROL Wie Source]** aus, um die Größe des Video-Viewers automatisch an die Auflösungsgröße des kodierten Videos anzupassen. Wenn Sie diese Option auswählen, können Sie die Bühnenbreite und Bühnenhöhe nicht eingeben. Stattdessen werden diese Optionen vom Video selbst übernommen. Wenn Sie **[!UICONTROL Wie Source]** auswählen, legen Sie die Option Randgröße fest, um die Hautabmessungen außerhalb des Videowiedergabebereichs widerzuspiegeln. Die Randgröße bezeichnet Höhe und Breite der Video-Steuerelemente in Pixel. Mithilfe der folgenden Abbildung können Sie die gewünschten Randgrößen ermitteln.*

   ![Konfiguration des Bildschirmrands des Video-Viewers](assets/vs_video_viewer_configure_margin.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Speichern unter]**, wenn Sie eine Viewer-Vorgabe hinzugefügt haben, indem Sie mit einer vorhandenen Vorgabe beginnen.
   * Wählen Sie **[!UICONTROL Speichern]**, wenn Sie eine Viewer-Vorgabe hinzugefügt oder bearbeitet haben.

### Exportieren einer HTML5-Viewer-Vorgabe {#exporting-an-html-viewer-preset}

Sie können eine vorhandene HTML5-Viewer-Vorgabe exportieren und als Grundlage für die Erstellung einer HTML5-Viewer-Vorgabe verwenden. Diese Exportoption ist nützlich, da Sie den Viewer auf diese Weise nicht komplett neu erstellen müssen. Stattdessen exportieren Sie eine Vorgabe mit Einstellungen, die Ihren Anforderungen in etwa entsprechen, und verwenden diese dann als Ausgangspunkt für Ihre Design-Anpassungen.

Alle standardmäßigen vorkonfigurierten CSS-Viewer-Vorgabedateien in Adobe Dynamic Media Classic verwenden relative Bildbereitstellungspfade, die auf Assets in `Scene7SharedAssets` verweisen. Im Folgenden finden Sie beispielsweise einen relativen Pfad zu einem Bild-Asset in einer CSS-Datei mit Viewer-Vorgabe für .

`Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

Wenn Sie jedoch Viewer-CSS-Dateien auf Ihrer eigenen Site hosten, müssen Sie diese relativen Bildpfade mithilfe eines expliziten Pfads zum Bild-Server in Ihrer eigenen Umgebung auflösen. Wenn Sie beispielsweise den relativen Pfad oben auf einen expliziten Pfad aktualisiert haben, könnte er wie folgt aussehen, wobei `https://s7d1.scene7.com` der direkte Pfad zu Ihrem Bild-Server ist: `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**So exportieren Sie eine HTML5-Viewer-Vorgabe:**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. Navigieren Sie **[!UICONTROL Setup]** > **[!UICONTROL Viewer-Vorgaben]**.
1. Wählen Sie in der Symbolleiste „Viewer-Vorgaben“ in der zweiten Dropdown-Liste links **[!UICONTROL HTML5]** aus.
1. Wählen Sie in der dritten Dropdown-Liste von links die Option **[!UICONTROL Alle Viewer]** aus.
1. Wählen Sie die Viewer-Vorgabe aus, die Sie als Grundlage für eine neue HTML5-Viewer-Vorgabe verwenden möchten.
1. Wählen Sie in der Symbolleiste **[!UICONTROL Exportieren]** aus.
1. Wählen Sie im Dialogfeld Ausgewählte Assets exportieren die Option **[!UICONTROL Export starten]**.

   Nach dem Export erhalten Sie eine CSS-Datei. Laden Sie die Datei herunter und dekomprimieren Sie sie.

1. Öffnen Sie die CSS-Datei in einem CSS-Editor, nehmen Sie Ihre Änderungen vor und speichern Sie die Datei anschließend.
1. Laden Sie die CSS-Datei in Adobe Dynamic Media Classic hoch.

   Siehe [Dateien hochladen](uploading-files.md#uploading_files).

1. Veröffentlichen Sie die CSS-Datei auf dem Dynamic Media-Bildserver.

   Siehe [Dateien veröffentlichen](publishing-files.md#publishing_files).

1. Fügen Sie die neue Viewer-Vorgabe wie gewohnt hinzu. Wählen Sie die hochgeladene CSS-Datei des Viewers aus.

   Siehe [Hinzufügen und Bearbeiten von Viewer-](application-setup.md#adding_and_editing_viewer_presets).

### Aktivieren oder Deaktivieren von Viewer-Vorgaben {#activating-or-deactivating-viewer-presets}

Um eine URL für die Anzeige von Assets zu erstellen, öffnen Benutzer die Dropdown-Liste „Vorgaben“ im Dialogfeld „Vorschau“, wählen Sie eine Viewer-Vorgabe aus und klicken Sie dann auf **[!UICONTROL URL kopieren]** (siehe [URL einer Viewer-Vorgabe kopieren](application-setup.md#copying_the_url_of_a_viewer_preset)). Diese Vorgabenliste enthält Viewer-Vorgaben, die Administratoren im Anzeigebereich „Viewer-Vorgaben“ hinzufügen und verwalten können. Beispielsweise werden alle aktiven eCatalog-Viewer-Vorgaben auf der Dropdown-Liste „Vorgaben“ im Dialogfeld „Vorschau“ angezeigt, wenn ein Benutzer eine Vorschau eines eCatalog anzeigt.

Wenn Sie Viewer-Vorgaben im Anzeigebereich „Viewer-Vorgaben“ nicht deaktivieren, kann die Dropdown-Liste „Vorgaben“ im Dialogfeld „Vorschau“ sehr viele Einträge umfassen.

**So aktivieren oder deaktivieren Sie Viewer-Vorgaben:**

1. Navigieren Sie **[!UICONTROL Setup]** > **[!UICONTROL Viewer-Vorgaben]**.
1. Wählen Sie auf der Seite „Viewer-Vorgaben“ die Option **[!UICONTROL Aktiv]** aus, um Viewer-Vorgaben zu aktivieren oder zu deaktivieren.

### Kopieren der URL einer Viewer-Vorgabe {#copying-the-url-of-a-viewer-preset}

Nachdem Sie ein Asset veröffentlicht haben, können Sie eine URL kopieren, um das Asset mit den Einstellungen einer bestimmten Viewer-Vorgabe anzuzeigen.

Die URL wird in die Zwischenablage kopiert. Sie können sie nach Bedarf im HTML-Code Ihrer Web-Seite, Ihres Mobilgeräts oder Ihrer Anwendung verwenden.

**So kopieren Sie die URL einer Viewer-Vorgabe:**

1. Wählen Sie das Asset im Durchsuchen-Bedienfeld aus.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld „URLs und Einbettungs-Code“ auf der rechten Seite **[!UICONTROL URL kopieren]** rechts neben dem gewünschten Viewer aus.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

   Klicken Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle auf **[!UICONTROL URL kopieren]**.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und gehen Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

   Klicken Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle auf **[!UICONTROL URL kopieren]**.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Wechseln Sie in der Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

   Klicken Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle auf **[!UICONTROL URL kopieren]**.

### Kopieren des Einbettungs-Codes einer Viewer-Vorgabe {#copying-the-embed-code-of-a-viewer-preset}

Mithilfe der Einbettungscode-Funktion können Sie den Viewer-Code für die ausgewählte Viewer-Vorgabe überprüfen. Sie können den Code auch in die Zwischenablage kopieren, damit Sie ihn zur Bereitstellung des Viewers in Ihre Web-Seiten einfügen können.

Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

**So kopieren Sie den Einbettungs-Code einer Viewer-Vorgabe:**

1. Wählen Sie das Asset im Bedienfeld Asset-Durchsuchen aus.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld „URLs“ auf der rechten Seite **[!UICONTROL Einbettungs-Code]**.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

   Wählen Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle **[!UICONTROL Einbettungs-Code]** aus.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und gehen Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

   Wählen Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle **[!UICONTROL Einbettungs-Code]** aus.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Wechseln Sie in der Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

   Wählen Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle **[!UICONTROL Einbettungs-Code]** aus.

1. Wählen Sie im Dialogfeld „Einbettungs-Code“ die Option **[!UICONTROL In Zwischenablage kopieren]**.
1. Wählen Sie **[!UICONTROL Schließen]** aus.

## Standard-Viewer konfigurieren {#configure-default-viewers}

Sie können Standard-Viewer verwenden, um den Standard-Viewer zu konfigurieren, der einem Asset zugeordnet ist, wenn Sie die Vorschau in Adobe Dynamic Media Classic verwenden. Die Standardvorschau kann für die folgenden Asset-Typen festgelegt werden:

* Bild
* Video
* Rotationsset
* Katalog
* Bildsatz
* Musterset
* Medienset

**So konfigurieren Sie Standard-Viewer:**

1. Wählen Sie in der Dropdown-Liste Setup die Option **[!UICONTROL Anwendungseinstellungen]**.
1. Wechseln Sie im Fenster Setup im linken Bereich zu **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Viewer]**
1. Wählen Sie **[!UICONTROL Standard-Viewer]** aus.
1. Wählen Sie im Fenster „Standard-Viewer“ in der Dropdown-Liste für jeden Asset-Typ den Viewer aus, den Sie mit der Vorschau des Assets verknüpfen möchten.
1. Klicken Sie unten rechts im Fenster „Standard-Viewer“ auf **[!UICONTROL Einstellungen speichern]**.
1. Klicken Sie in der rechten unteren Ecke des Fensters Setup auf **[!UICONTROL Schließen]**, um zum Fenster Asset zurückzukehren.

## Metadaten-Ansichten {#metadata-views}

*Metadaten* sind standardisierte Informationen zu einem Asset. Mit Metadaten können Sie Ihren Arbeitsablauf optimieren, Ihre Assets organisieren und die Suche verbessern. Adobe Dynamic Media Classic unterstützt den IPTC-Standard (International Press Telecommunications Council) und den XMP-Standard (Extensible Metadata Platform). Bevor Benutzer Metadaten zu einem Asset in der Detailansicht anzeigen oder eingeben, können sie das Menü „Metadatenansichten“ öffnen. Dort können sie den Satz von Metadatenfeldern auswählen, die sie anzeigen oder zur Beschreibung des Assets verwenden möchten.

Adobe Dynamic Media Classic verfügt über vordefinierte Metadatenansichten und Admins können eigene Metadatenansichten erstellen, aus denen Benutzende beim Eingeben von Metadaten wählen können.

### Erstellen einer Metadaten-Ansicht {#creating-a-metadata-view}

1. Wechseln Sie **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Metadatenansichten]**.
1. Wählen Sie **[!UICONTROL Hinzufügen]** aus.
1. Geben Sie im Textfeld Vorgabenname einen Namen für die Ansicht ein.
1. (Optional) Aktivieren Sie **[!UICONTROL Standard festlegen]**, damit diese Ansicht die Ansicht ist, die Benutzende sehen, wenn sie das Bedienfeld „Metadaten“ in der Detailansicht öffnen.
1. (Optional) Wählen Sie **[!UICONTROL UDF einschließen]**, um benutzerdefinierte Felder in die Ansicht aufzunehmen. Benutzerdefinierte Felder werden oben im Metadatenbedienfeld in der Detailansicht angezeigt.
1. Wählen Sie die Felder aus, die Sie für die Ansicht anzeigen möchten (wählen Sie **[!UICONTROL Alle auswählen]**, um alle Felder auszuwählen).
1. Wählen Sie **[!UICONTROL Speichern]** aus.

   Die ausgewählten Kategorien und Felder für die Ansicht werden im Vorschaubedienfeld angezeigt.

### Verwalten von Metadaten-Ansichten {#managing-metadata-views}

1. Wechseln Sie **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Metadatenansichten]**.
1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie eine Ansicht aus, um eine Vorschau davon zu erstellen. Die Felder in der Ansicht werden im Vorschaubedienfeld angezeigt.
   * Um eine Ansicht zu bearbeiten, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Bearbeiten]**. Wählen Sie dann Feldnamen im Bedienfeld „Vorschau“ aus bzw. heben Sie die Auswahl auf und wählen oder deaktivieren Sie die Option **[!UICONTROL UDF einschließen]**.
   * Um eine Ansicht zu löschen, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Löschen]**.
   * Um eine Ansicht zum Standard zu machen, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Als Standard festlegen]**. Die Standardansicht ist die Ansicht, die Benutzenden angezeigt wird, wenn sie ein Asset in der Detailansicht öffnen und zum Metadaten-Bedienfeld gehen.

## Metadaten-Vorgaben {#metadata-presets}

Metadatenvorgaben bieten Admins die Möglichkeit, die Metadaten, die Assets zugewiesen sind, zu steuern und zu regulieren. In der Detailansicht kann ein Benutzer Metadaten zu einem Asset in die für diesen Zweck bereitgestellten Felder eingeben. Ein Benutzer kann beispielsweise einen Eigentümernamen, eine Copyrightbeschreibung und eine Adresse eingeben. Um sicherzustellen, dass Benutzer diese Informationen korrekt und vollständig eingeben, können Sie Metadatenvorgaben erstellen. Durch Auswahl einer Metadatenvorgabe in der Detailansicht werden Metadatenfelder mit vordefinierten Werten gefüllt. So werden beispielsweise der Eigentümername, die Copyrightbeschreibung und die Adresse automatisch eingegeben.

Erstellen Sie eine Metadatenvorgabe für jeden Satz von Metadatenwerten, den Benutzerinnen und Benutzer automatisch in die Detailansicht eingeben können sollen, um ein Asset zu beschreiben.

### Erstellen oder Bearbeiten einer Metadaten-Vorgabe {#creating-or-editing-a-metadata-preset}

1. Wechseln Sie **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Metadatenvorgaben]**.
1. Führen Sie im Anzeigebereich „Metadaten-Vorgaben“ einen der folgenden Schritte aus:

   * Um eine Vorgabe zu erstellen, wählen Sie **[!UICONTROL Hinzufügen]** aus. Geben Sie in das Textfeld Name der Metadatenvorlage einen Namen für die Vorgabe ein. Wählen Sie **[!UICONTROL Metadatenansichten]** und wählen Sie dann eine Ansicht aus der Dropdown-Liste aus (siehe [Metadatenansichten](application-setup.md#metadata_views)).
   * Um eine vorhandene Vorgabe zu bearbeiten, wählen Sie die Vorgabe aus der Liste Metadatenvorgaben aus und klicken Sie dann auf **[!UICONTROL Bearbeiten]**.

1. Erweitern Sie Überschriften, die Sie in die Vorgabe einbeziehen möchten, und geben Sie Werte in die verschiedenen Felder ein, die Sie in die Vorgabe einbeziehen möchten.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

   Die ausgewählten Kategorien und Felder für die Vorgabe werden im Vorschaubedienfeld angezeigt.

### Verwalten von Metadaten-Vorgaben {#managing-metadata-presets}

1. Wechseln Sie **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Metadatenvorgaben]**.
1. Führen Sie einen der folgenden Schritte aus:

   * Um eine Vorschau einer Vorgabe anzuzeigen, wählen Sie die entsprechende Vorgabe aus. Die Vorgabeninformationen (Kategorien und Felder) werden im Anzeigebereich „Vorschau“ angezeigt.
   * Um eine Vorgabe zu löschen, wählen Sie die Vorgabe aus und klicken Sie dann auf **[!UICONTROL Löschen]**.

## Benutzerdefinierte Felder {#user-defined-fields}

Ein Medienportal-Administrator bzw. Unternehmensadministrator kann individuelle, benutzerdefinierte Metadatenfelder erstellen. Benutzerdefinierte Felder können Ihnen beim Organisieren von Assets in Adobe Dynamic Media Classic helfen. Sie können die Felder bei Bedarf als Aktiv markieren. Wenn diese Option aktiviert ist, werden die Namen dieser benutzerdefinierten Metadatenfelder im Bedienfeld „Metadaten“ in der Detailansicht angezeigt. Die Benutzer können Informationen zur Beschreibung der Assets in die benutzerdefinierten Metadatenfelder eingeben. Außerdem können Benutzer ein benutzerdefiniertes Metadatenfeld als Suchkriterium angeben.

Eine effektive Nutzung benutzerdefinierter Metadatenfelder besteht darin, die Aktivierungszeit eines Assets für einen bestimmten Launch oder Ausverkauf zu verzögern. Sie definieren ein Feld „Aktivierung“, basierend auf dem Typ *Datum*. Anschließend können Sie über das **[!UICONTROL Metadaten]**-Bedienfeld in der Detailansicht oder **[!UICONTROL Datei]** > **[!UICONTROL Info bearbeiten]** angeben, wann das Asset aktiviert wird. Adobe Dynamic Media Classic überprüft den Veröffentlichungsstatus eines Assets und den Veröffentlichungsverlauf. Wenn es sich nicht innerhalb der Aktivierungszeit befindet, wird der Veröffentlichungsstatus als „Nicht veröffentlicht“ angezeigt.

>[!NOTE]
>
>Damit benutzerdefinierte Felder im Metadaten-Bedienfeld in der Detailansicht angezeigt werden, schließen Sie benutzerdefinierte Felder in Metadatenansichten ein. Wählen Sie im Anzeigebereich „Metadaten-Ansichten“ die Option „UDF einschließen“. Weitere Informationen finden Sie unter [Metadaten-Ansichten](application-setup.md#metadata_views).

>[!NOTE]
>
>Um mithilfe benutzerdefinierter, benutzerdefinierter Felder nach Assets zu suchen, gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Persönliches Setup]** und wählen Sie dann **[!UICONTROL UDFs in die Suche einschließen]** aus. Siehe [Persönliche Einstellungen](personal-setup.md#personal_setup).

### Erstellen eines benutzerdefinierten Metadatenfelds {#creating-a-user-defined-metadata-field}

1. Wechseln Sie **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Benutzerdefinierte Felder]**.
1. Wählen Sie **[!UICONTROL Hinzufügen]** aus
1. Legen Sie im Dialogfeld „Benutzerdefiniertes Feld“ die gewünschten Optionen fest.

   * **[!UICONTROL Name]**: Geben Sie einen Namen für das Metadatenfeld ein.

   * **[!UICONTROL Typ]**: Wählen Sie eine Option aus, die den Typ der Informationen definiert, die Benutzerinnen und Benutzer in das Metadatenfeld eingeben können:

   * **[!UICONTROL String]**: Eine Textzeichenfolge.

   * **[!UICONTROL Int]**: eine Ganzzahl.

   * **[!UICONTROL Float]**: Eine Gleitkommazahl.

   * **[!UICONTROL Ja/Nein]**: Ein boolescher Wert mit Ja/Nein.

   * **[!UICONTROL date]**: Ein Datum. Das Format MM/TT/JJJJ ist zulässig.

   * **[!UICONTROL Dateiname]**: Der Name einer Datei.

   * **[!UICONTROL Color]**: Der Name einer Farbe.

   * **[!UICONTROL Dimension]**: Die Breite und Höhe des Assets.

   * **[!UICONTROL Nicht typisiert]**: Für Abwärtskompatibilität. Wählen Sie diese Option nicht aus.

   * **[!UICONTROL Standardwert]**: Optional. Geben Sie den Wert ein, den Benutzer am ehesten in das Feld eingeben werden. Dieser Wert wird als Standardwert für das neue Feld verwendet.

   * **[!UICONTROL Gilt für]**: Optional. Wählen Sie einen Asset-Typ aus, wenn das Metadatenfeld nur auf einen bestimmten Asset-Typ angewendet werden soll.

     >[!NOTE]
     >
     >Wählen Sie **[!UICONTROL Option „Gilt für]** mit Bedacht aus, da Sie die Option **[!UICONTROL Gilt für]** nach dem Erstellen eines benutzerdefinierten Felds nicht ändern können. Mit Adobe Dynamic Media Classic können Sie den Namen, den Typ und den Standardwert eines benutzerdefinierten Felds bearbeiten, nicht jedoch die Einstellung **[!UICONTROL Gilt für]**. *

1. Wählen Sie **[!UICONTROL Speichern]** aus, wenn Sie die Erstellung des Metadatenfelds abgeschlossen haben.

### Verwalten von benutzerdefinierten Feldern {#manage-user-defined-fields}

Im Anzeigebereich „Benutzerdefinierte Felder“ finden Sie Befehle zum Verwalten eigener, benutzerdefinierter Felder.

Benutzerdefinierte Felder können nur von Media Portal-Administratoren und Unternehmensadministratoren verwaltet werden.

Wechseln Sie zum Öffnen dieses Bildschirms **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Benutzerdefinierte Felder]**.

* **Feld bearbeiten**: Wählen Sie das Feld aus und klicken Sie dann auf **[!UICONTROL Bearbeiten]**.

* **Feld löschen**: Wählen Sie das Feld aus und klicken Sie auf **[!UICONTROL Löschen]**.

* **Feld aktivieren**: Wählen Sie die Option **[!UICONTROL Aktiv]** neben dem Namen eines Felds aus oder heben Sie die Auswahl auf. Wenn Sie sich in der Rolle der Unternehmensverwaltung befinden, wird diese Option nicht angezeigt. Da diese Option mit MediaPortal zusammenhängt, müssen Sie MediaPortal-Funktionen in Personal Setup anzeigen auswählen (einschalten), um die aktivierten Felder anzuzeigen.

## Optimieren von Dateien {#optimize-files}

Wenn Sie Dateien in die Adobe Dynamic Media Classic hochladen, werden sie vom System für die Speicherung und Veröffentlichung optimiert. Wenn das Hochladen jedoch unterbrochen wird, können einige Bilder nicht optimiert werden. In diesem Fall wird die Meldung „Bild noch nicht optimiert“ angezeigt. Als Administrator können Sie jedoch auch diese Dateien optimieren.

Adobe Dynamic Media Classic durchsucht Ihre -Dateien und optimiert nur die Bilder, die zuvor nicht vollständig optimiert wurden.

1. Wechseln Sie **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** und wählen Sie dann **[!UICONTROL Dateien optimieren]**.
1. Geben Sie Informationen für den Optimierungsauftrag ein und wählen Sie **[!UICONTROL Senden]**.

   Wenn Sie mit mehr als einem Unternehmen arbeiten, optimieren Sie Dateien, die zu unterschiedlichen Unternehmen gehören, getrennt.

## Stapelsatzvorgaben {#batch-set-presets}

Verwenden Sie die Stapelsatzvorgaben, um automatisch Bildsets oder Rotationssets zu erstellen, während ein Vorgang ausgeführt wird, um Assets in Adobe Dynamic Media Classic hochzuladen.

Unternehmensadministratoren definieren zunächst Namenskonventionen für die Assets, die sie in einem Satz gruppieren möchten. Anschließend können Sie eine Stapelsatzvorgabe erstellen, um auf diese Bilder zu verweisen. Jede Vorgabe ist ein eindeutig benannter, in sich abgeschlossener Satz von Anweisungen, die definieren, wie der Satz unter Verwendung der Bilder, die den definierten Benennungsregeln im Vorgabenrezept entsprechen, konstruiert werden soll.

Alle aktiven Stapelsatzvorgaben für ein Unternehmen werden im Dialogfeld Upload-Auftragsoption aufgeführt, sodass Sie angeben können, welche Vorgabe bei jeder Upload-Sitzung angewendet werden soll. Unternehmensadministratoren sehen alle aktiven und inaktiven Stapelsatzvorgaben. Beim Hochladen von Dateien erstellt Adobe Dynamic Media Classic automatisch einen Satz mit allen Dateien, die der definierten Namenskonvention in den aktiven Vorgaben entsprechen.

### Standardbenennung {#default-naming}

Der Unternehmensadministrator erstellt eine Standardnamenskonvention, die in jedem Rezept für Stapelsatzvorgaben verwendet wird. Die in der Definition der Stapelsatzvorgabe ausgewählte Standardnamenskonvention kann alles sein, was Ihr Unternehmen für die Batch-Generierung von Sätzen für alle Websites benötigt. Eine Stapelsatzvorgabe wird erstellt, um die von Ihnen definierte Standardnamenskonvention zu verwenden. Sie können beliebig viele Stapelsatzvorgaben mit alternativen, benutzerdefinierten Benennungskonventionen erstellen, die für einen bestimmten Satz von Inhalten erforderlich sind, wenn eine Ausnahme von der im Unternehmen definierten Standardbenennung besteht.

Die Einrichtung einer Standardnamenskonvention ist nicht erforderlich, um die Funktionalität der Stapelsatzvorgaben zu verwenden. Adobe empfiehlt jedoch, eine Standardnamenskonvention zu verwenden, um so viele Elemente Ihrer Namenskonvention zu definieren, wie Sie in einem Satz gruppieren möchten. Dies hilft, die Erstellung von Stapelsätzen zu optimieren.

1. Wechseln Sie **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Stapelsatzvorgaben]** > **[!UICONTROL Standardbenennung]**.
1. Wählen Sie **[!UICONTROL Formular anzeigen]** oder **[!UICONTROL Code anzeigen]**, um die gewünschte Ansicht festzulegen, und geben Sie Informationen zu den einzelnen Elementen ein.

   Sie können das Kontrollkästchen **[!UICONTROL Code anzeigen]** aktivieren, um den Wert des regulären Ausdrucks neben Ihren Formularauswahlen anzuzeigen. Sie können diese Werte eingeben oder ändern, um die Elemente der Namenskonvention zu definieren, wenn die Formularansicht Sie aus irgendeinem Grund einschränkt. Wenn Ihre Werte in der Formularansicht nicht geparst werden können, werden die Formularfelder inaktiv.

   >[!NOTE]
   >
   >Deaktivierte Formularfelder weisen nicht unbedingt auf einen ungültigen regelmäßigen Ausdruck hin. Es gibt keine Möglichkeit zu prüfen, ob Ihre regelmäßigen Ausdrücke korrekt sind. Nach der Zeile Ergebnis werden die Ergebnisse des regulären Ausdrucks angezeigt, den Sie für jedes Element erstellen. Der vollständige regelmäßige Anschluss wird am unteren Seitenrand angezeigt.

1. Erweitern Sie die Elemente bei Bedarf und geben Sie die zu verwendenden Benennungsregeln ein.
1. Wählen Sie bei Bedarf **[!UICONTROL Hinzufügen]**, um eine weitere Namenskonvention für ein Element hinzuzufügen. Oder wählen Sie **[!UICONTROL Entfernen]**, um eine Namenskonvention für ein Element zu löschen.
1. Wählen Sie **[!UICONTROL Speichern unter]** und geben Sie einen Namen für die Vorgabe ein. Oder wählen Sie **[!UICONTROL Speichern]**, wenn Sie eine vorhandene Vorgabe bearbeiten.

Alternativ können Sie „Code anzeigen“ ohne verfügbare Formularfelder verwenden. In dieser Ansicht erstellen Sie Ihre Namenskonventionsdefinitionen vollständig unter Verwendung regulärer Ausdrücke.

Zwei Elemente sind zur Definition verfügbar: Treffer und Grundname. Bei diesen Feldern handelt es sich um alle Elemente, die Sie für eine Namenskonvention definiert haben. Sie können dabei helfen, den Teil der Konvention zu identifizieren, der verwendet wird, um den Satz zu benennen, in dem sie enthalten sind. Die individuelle Namenskonvention eines Unternehmens kann eine oder mehrere Zeilen der Definition für jedes dieser Elemente verwenden. Sie können so viele Zeilen für Ihre eindeutige Definition verwenden und sie in verschiedene Elemente gruppieren, z. B. für Hauptbild, Farbelement, Element der alternativen Ansicht und Farbfeld-Element.

### Erstellen einer Stapelsatzvorgabe {#creating-a-batch-set-preset}

Adobe Dynamic Media Classic verwendet Stapelsatzvorgaben zum Organisieren von Assets, die einige allgemeine Informationen oder Inhalte in Bildsets teilen, um sie in Viewern anzuzeigen. Die Rezepte für Stapelsatzvorgaben werden automatisch zusammen mit den Asset-Importvorgängen ausgeführt, die Sie in Adobe Dynamic Media Classic planen.

Verwenden der Stapelsatzvorgabe zum Erstellen, Bearbeiten und Verwalten von Stapelsatzvorgaben. Sie können so viele Vorgaben wie nötig erstellen, um alle erforderlichen Asset-Aufnahmeaufträge abzudecken. Es gibt zwei Formen von Definitionen von Stapelsatzvorgaben: eine für eine von Ihnen eingerichtete Standardnamenskonvention und eine für benutzerdefinierte Namenskonventionen, die Sie spontan erstellen.

Sie können entweder die Formularfeldmethode verwenden, um eine Stapelsatzvorgabe zu definieren, oder die Codemethode, mit der Sie reguläre Ausdrücke verwenden können. Wie bei **[!UICONTROL Standardbenennung]** können Sie **[!UICONTROL Code-Ansicht]** auswählen, während Sie in der Formularansicht definieren und reguläre Ausdrücke zum Erstellen Ihrer Definitionen verwenden. Alternativ können Sie eine der Ansichten deaktivieren, um ausschließlich die eine oder die andere zu verwenden.

Siehe auch [Erstellen einer Stapelsatzvorgabe für die automatische Erstellung eines 2D-Rotationssets](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

Siehe auch [2D-Rotationsset](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/537_2d-spin_converted%20renamed_Done-AVS) Schulungsvideo.

**So erstellen Sie eine Stapelsatzvorgabe:**

1. Wechseln Sie **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Stapelsatzvorgaben]** > **[!UICONTROL Stapelsatzvorgabe]**. **[!UICONTROL Formular anzeigen]**, wie in der oberen rechten Ecke der Detailseite angezeigt, ist die Standardansicht.
1. Klicken Sie im Bedienfeld Vorgabenliste **[!UICONTROL Hinzufügen]**, um die Definitionsfelder im Detailbereich auf der rechten Seite der Seite zu aktivieren.
1. Geben Sie in der Detailansicht in das Feld „Vorgabenname“ einen Namen für die Vorgabe ein.
1. Wählen Sie im Dropdown-Menü „Stapelsatztyp“ einen Vorgabentyp aus.

   Um automatisch ein 2D-Rotationsset zu erzeugen, wählen Sie in der Dropdownliste „Stapelsatztyp“ die Option **[!UICONTROL Multiachsen-Rotationsset]**.

1. Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie eine Standardnamenskonvention verwenden, die Sie zuvor unter **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Stapelsatzvorgaben]** > **[!UICONTROL Standardbenennung]** eingerichtet haben, erweitern Sie **[!UICONTROL Asset-Namenskonventionen]** und klicken anschließend in der Dropdown-Liste „Dateibenennung“ auf **[!UICONTROL Standard]**.
   * Zum Definieren einer Namenskonvention während der Einrichtung der Vorgabe erweitern Sie **[!UICONTROL Asset-Namenskonventionen]** und klicken Sie anschließend in der Dropdown-Liste „Dateibenennung“ auf **[!UICONTROL Benutzerdefiniert]**.

1. Definieren Sie für die Sequenzreihenfolge die Reihenfolge der Bilder, nachdem der Satz in Adobe Dynamic Media Classic gruppiert wurde. Die Assets werden standardmäßig in alphanumerischer Reihenfolge angeordnet. Sie können jedoch auch eine durch Kommas getrennte Liste mit regulären Ausdrücken verwenden, um die Reihenfolge anzupassen.
1. Geben Sie für „Satzbenennungs- und -erstellungskonvention“ das Suffix bzw. Präfix für den Basisnamen an, den Sie in der Asset-Benennungskonvention definiert haben. Legen Sie außerdem fest, wo das Bildset in der Adobe Dynamic Media Classic-Ordnerstruktur erstellt werden soll.

   Wenn Sie eine große Anzahl von Bildsets definieren, trennen Sie diese Sets von den Ordnern, die die Assets selbst enthalten. Viele Kunden erstellen einen Ordner „Bildsets“ und leiten das Programm weiter, um dort von Stapelsätzen generierte Sets zu platzieren.

1. Wählen **[!UICONTROL Speichern]** im Bedienfeld Details aus.

### Erstellen einer Stapelsatzvorgabe für die automatische Erstellung eines 2D-Rotations-Sets {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

Sie können den Stapelsatztyp (**-Achsen-Rotationsset) verwenden** um ein „Rezept“ zu erstellen, das die Erstellung von 2D-Rotationssets automatisiert. Für die Gruppierung von Bildern werden die regulären Ausdrücke „Zeile“ und „Spalte“ verwendet, sodass die Bild-Assets im multidimensionalen Array korrekt an der entsprechenden Position ausgerichtet werden.

Siehe auch [Erstellen einer Stapelsatzvorgabe](application-setup.md#creating_a_batch_set_preset).

Es gibt keine minimale oder maximale Anzahl von Zeilen oder Spalten, die Sie in einem Mehrachsen-Rotationsset haben müssen.

Angenommen, Sie möchten ein mehrachsiges Rotationsset mit dem Namen *spin-2dspin* erstellen. Sie verfügen über einen Satz von Rotationssetbildern, die drei Zeilen mit 12 Bildern pro Zeile enthalten. Die Bilder haben die folgenden Namen:

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

![Stapelsatzrezept-Bild](assets/se_batch_set_recipe.png)

Die Gruppierung für den Teil des freigegebenen Asset-Namens des Rotationssets wird dem Feld Übereinstimmung hinzugefügt (wie hervorgehoben). Der variable Teil des Asset-Namens, der die Zeile und Spalte enthält, wird den Feldern Zeile bzw. Spalte hinzugefügt.

Wenn das Rotationsset hochgeladen und veröffentlicht wird, aktivieren Sie den Namen des 2D-Rotationsset-Rezepts, der unter **[!UICONTROL Stapelsatzvorgaben)]** Dialogfeld Upload-Auftragsoptionen aufgeführt ist.

**So erstellen Sie eine Stapelsatzvorgabe für die automatische Erstellung eines 2D-Rotations-Sets:**

1. Wechseln Sie **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Stapelsatzvorgaben]** > **[!UICONTROL Stapelsatzvorgabe]**. **[!UICONTROL Formular anzeigen]**, wie in der oberen rechten Ecke der Detailseite angezeigt, ist die Standardansicht.
1. Wählen Sie im Bedienfeld Vorgabenliste **[!UICONTROL Hinzufügen]** aus, um die Definitionsfelder im Detailbereich auf der rechten Seite der Seite zu aktivieren.
1. Geben Sie in der Detailansicht in das Feld „Vorgabenname“ einen Namen für die Vorgabe ein.
1. Wählen Sie im Dropdown-Menü „Stapelsatztyp“ die Option **[!UICONTROL Asset-Set]**.
1. Wählen Sie in der Dropdown-Liste Untertyp die Option **[!UICONTROL Mehrachsen-Rotationsset]** aus.
1. Erweitern Sie **[!UICONTROL Asset-Benennungskonventionen]** und klicken Sie in der Dropdown-Liste „Dateibenennung“ auf **[!UICONTROL Benutzerdefiniert]**.
1. Verwenden Sie die Attribute **[!UICONTROL Entspricht]** und optional **[!UICONTROL Grundname]**, um einen regulären Ausdruck für die Benennung der Bild-Assets zu definieren, aus denen die Gruppierung besteht.

   Ein regulärer Ausdruck für eine wörtliche Übereinstimmung könnte beispielsweise wie folgt aussehen:

   `(\w+)-\w+-\w+`

1. Erweitern Sie **[!UICONTROL Zeilen-/Spaltenposition]** und definieren Sie anschließend den Namen des Formats für die Position des Bild-Assets innerhalb des 2D-Rotationsset-Arrays.

   Setzen Sie die Zeilen- oder Spaltenposition im Dateinamen in Klammern.

   Der reguläre Ausdruck Ihrer Zeile könnte beispielsweise wie folgt aussehen:

   `\w+-R([0-9]+)-\w+`

   oder

   `\w+-(\d+)-\w+`

   Der reguläre Ausdruck für die Spalte könnte wie folgt aussehen:

   `\w+-\w+-C([0-9]+)`

   oder

   `\w+-\w+-C(\d+)`

   Denken Sie daran, dass diese Ausdrücke nur Beispiele sind. Sie können reguläre Ausdrücke Ihren Bedürfnissen entsprechend erstellen.

   >[!NOTE]
   >
   >Wenn die Kombination aus regulären Ausdrücken in Zeilen und Spalten die Position des Assets innerhalb des multidimensionalen Rotationsset-Arrays nicht bestimmen kann, wird dieses Asset dem Set nicht hinzugefügt. Ein Fehler wird protokolliert.

1. Geben Sie für „Satzbenennungs- und -erstellungskonvention“ das Suffix bzw. Präfix für den Basisnamen an, den Sie in der Asset-Benennungskonvention definiert haben. Legen Sie außerdem fest, wo das Bildset in der Adobe Dynamic Media Classic-Ordnerstruktur erstellt werden soll.

   Wenn Sie eine große Anzahl von Bildsets definieren, trennen Sie diese Sets von den Ordnern, die die Assets selbst enthalten. Viele Kunden erstellen einen Ordner „Bildsets“ und leiten das Programm weiter, um dort von Stapelsätzen generierte Sets zu platzieren.

1. Wählen **[!UICONTROL Speichern]** im Bedienfeld Details aus.
1. Laden Sie Ihr Rotationsset wie gewohnt hoch und veröffentlichen Sie es. Stellen Sie dabei sicher, dass Sie den Namen Ihres 2D-Rotationssets im Dialogfeld Optionen für das Laden von Aufträgen unter „Stapelsatzvorgaben“ aktivieren.

>[!MORELIKETHIS]
>
>* [Vorschau eines Assets](previewing-asset.md#previewing_an_asset)
>* [Einrichten von Bildvorgaben](setting-image-presets.md#setting_up_image_presets)
>* [Anzeigen, Hinzufügen und Exportieren von Metadaten](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [Überprüfen Sie die Auftragsdateien](checking-job-files.md#checking_job_files)
