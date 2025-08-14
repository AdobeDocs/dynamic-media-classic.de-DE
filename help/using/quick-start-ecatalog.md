---
title: 'Schnellstart: E-Kataloge'
description: Eine Einführung und ein Schnellstart für E-Kataloge, mit denen Sie E-Katalog-Techniken in Adobe Dynamic Media Classic schnell einrichten und ausführen können.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
topic: Integrations
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 25%

---

# Schnellstart: E-Kataloge{#quick-start-ecatalogs}

Ein eCatalog ist eine digitale Web-Version von Druckmaterial, z. B. ein Katalog, eine Broschüre, ein Flyer, ein Produkthandbuch oder ein Werberundschreiben. Ein E-Katalog wird in einem E-Katalog-Viewer auf einer Website angezeigt. Dieser Viewer simuliert das Erlebnis des Lesens von Druckmaterial.

Siehe auch die folgenden Schulungsvideos:

* [Schnellstart 1: E-Kataloge](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [Schnellstart 2: E-Kataloge](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

Je nach den Einstellungen, die Sie für Ihren E-Katalog auswählen, bietet der Viewer folgende Möglichkeiten:

* Suchen Sie im Katalog nach einem Keyword oder Keywords. Die Suchergebnisse werden als Miniaturansichten in einem Suchfeld auf der linken Seite des Katalogs angezeigt. Jedes anklickbare Miniaturbild stellt eine Katalogaufteilung dar, in der der hervorgehobene Suchbegriff gefunden wurde.

* Freigeben des Katalogs über soziale Medien; Herunterladen des Katalogs, um ihn offline anzuzeigen; Aktivieren der Favoriten, um Elemente zu markieren, zu denen Sie schnell zurückkehren möchten, oder Drucken des Katalogs.
* Navigieren Sie im Katalog mithilfe des Inhaltsverzeichnisses oder der Seitenrasteransicht; klicken Sie auf die mittlere Kante einer Seite, um die Seite vorwärts oder rückwärts zu navigieren.
* Heranzoomen, Herauszoomen und Schwenken, um bestimmte Elemente auf einer Seite genau zu betrachten
* Bewegen Sie den Mauszeiger über einen Seitenbereich (eine so genannte Imagemap), damit ein Popup-Fenster mit Informationen zu einem Element angezeigt wird.
* Wählen Sie einen Seitenbereich aus, um eine neue Web-Seite mit weiteren Informationen zu einem Element zu öffnen.
* Schreiben und Anbringen eines Klebezettels als Lesezeichen an einer bestimmten E-Katalogseite
* Tippen Sie auf Imagemap-Symbole, um verwandte Web-Seiten oder kontextbezogene Infobereiche zu starten.
* Verwenden von Gesten zur Interaktion, einschließlich der Zangenbewegung zum Zoomen und der Wischbewegung zum Umblättern von Seiten.
* Durchsuchen der Elemente nach bestimmten Schlüsselwörtern

![Der E-Katalog, wie er den Benutzern angezeigt wird. A) E-Katalog-Startseite. b)eCatalog wurde auf Seite 2.](/help/using/assets/ec_cat_viewer_popup.png) umgestellt

Zum Erstellen eines E-Katalogs verwenden Sie in der Regel hochauflösende PDF-Dateien, die in Adobe Acrobat oder einem anderen Druckprogramm erstellt wurden. Sie können jedoch auch einen E-Katalog aus Bilddateien erstellen.

Während der Erstellung des E-Katalogs können Sie Seiten oder Druckbögen in der gewünschten Reihenfolge anordnen. Darüber hinaus können Sie angeben, ob Einzelseiten, doppelseitige Druckbögen oder mehrseitige Druckbögen verwendet werden sollen. Sie können Imagemaps für Seitenbereiche erstellen, damit Betrachterinnen und Betrachter beispielsweise einen Bereich auf der Seite auswählen und eine neue Seite auf Ihrer Website öffnen können. Der Rollover-Text, der angezeigt wird, kann mithilfe der Infofeldeinstellungen im Anzeigebereich „E-Katalog“ verwaltet werden. Außerdem haben Sie bei der Konfiguration des E-Katalog-Viewers die Möglichkeit, aus mehr als 100 verschiedenen Konfigurationsoptionen zu wählen. Sie können die Funktionen und die Darstellung des Viewers speziell für die gewünschte Zielgruppe anpassen.

>[!NOTE]
>
>Wenn Sie Benutzende des Dynamic Media: Scene7-Modus sind und E-Kataloge verwenden möchten, bearbeiten Sie den `pdfbrochure` in CRXDE Lite. Navigieren Sie dazu in Adobe Experience Manager zu **[!UICONTROL Tools]** > **[!UICONTROL Allgemein]** > **[!UICONTROL CRXDE Lite]**. Navigieren Sie in der Navigationsstruktur des linken Bedienfelds zu `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>Wählen Sie im unteren rechten Bereich auf der Registerkarte **[!UICONTROL Eigenschaften]** die Zeile `jobParam` aus. Legen Sie den Wert für `pdfbrochure` von `false` auf `true` fest. Wie in `pdfbrochure=true`
>
>Klicken Sie oben links auf der Seite &quot;CRXDE Lite&quot; auf **[!UICONTROL Alle speichern]**.
>
>Sie können jetzt E-Kataloge in Adobe Dynamic Media Classic erstellen.

Diese Kurzanleitung für die Erstellung eines E-Katalogs hilft Ihnen, sich schnell mit den E-Katalogfunktionen vertraut zu machen. Führen Sie die Schritte 1 bis 7 aus. Nach jedem Schritt finden Sie einen Querverweis auf eine Themenüberschrift, unter der Sie weitere Informationen finden.

## &#x200B;1. PDF-Dateien hochladen

Normalerweise werden Adobe PDF-Dateien als Grundlage für einen E-Katalog verwendet. Da PDF-Dateien speziell zum Drucken vorgesehen sind, enthalten sie normalerweise CMYK-Bilder. Adobe Dynamic Media Classic erkennt diese Bilder und konvertiert sie mithilfe eines standardmäßigen CMYK-Farbprofils. Sie müssen jedoch ein benutzerdefiniertes Farbprofil hochladen und verwenden.

Wählen Sie in der globalen Navigationsleiste die Option **[!UICONTROL Hochladen]**, um PDF-Dateien oder Bilder für Ihren E-Katalog hochzuladen. Sie können Dateien über Ihren Desktop oder FTP hochladen. FTP wird empfohlen, wenn Sie viele Dateien oder Dateien mit mehr als 100 MB hochladen.

Im Anzeigebereich „Hochladen“ finden Sie im Bereich „PDF-Optionen“ Einstellungen für das Hochladen von PDF-Dateien mit der angemessenen Auflösung und dem richtigen Farbraum. Eine Auflösung von 150 Pixel pro Zoll wird empfohlen. Sie können die Option **[!UICONTROL E-Katalog automatisch erstellen]** auswählen, um beim Hochladen einer PDF-Datei einen E-Katalog zu erstellen.

Siehe [Hochladen der PDF-](uploading-pdf-files.md#uploading_the_pdf_files).

## &#x200B;2. E-Katalog erstellen

Erstellen Sie Ihren E-Katalog, indem Sie im Durchsuchen-Panel PDF oder Bilddateien auswählen. Wählen Sie **[!UICONTROL Erstellen]** und dann **[!UICONTROL E-Kataloge]** aus.

Wählen Sie auf der Seite „E **[!UICONTROL Katalog“ auf der Registerkarte]** Bestellseiten“ eine Layout-Option aus: **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]** oder **[!UICONTROL Custom]**. Sie können die Anordnung der Seiten oder Druckbögen durch Ziehen oder, insbesondere in großen E-Katalogen, durch Auswahl eines Seitennamens im Menü „Verschieben nach“ ändern.

Um Seiten hinzuzufügen, wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die gewünschten PDF-Dateien oder Bilddateien aus dem Ordner in den Anzeigebereich „Seiten ordnen“. Anstelle der standardmäßigen Seitennummern können Sie benutzerdefinierte Seitennamen angeben oder viele Seitennamen importieren.

Wählen Sie **[!UICONTROL Speichern]**, geben Sie einen Namen für Ihren E-Katalog ein, wählen Sie einen Adobe Dynamic Media Classic-Ordner für dessen Speicherung aus und klicken Sie auf **[!UICONTROL Speichern]**. Jedes Mal, wenn Sie die Seitenreihenfolge ändern oder Ihren E-Katalog bearbeiten, speichern Sie Ihre Änderungen, indem Sie **[!UICONTROL Speichern]** auswählen.

Siehe [Erstellen eines E-](creating-ecatalog.md).

## &#x200B;3. Erstellen von Imagemaps

Imagemaps fügen E-Katalog-Seiten einen weiteren Aspekt hinzu. Eine Imagemap ist ein Seitenbereich, mit dessen Hilfe weitere Informationen zu einem Element angezeigt werden können. Wenn Betrachter der Website den Mauszeiger über eine Imagemap bewegen, wird eine Beschreibung des Elements angezeigt. Durch Klicken auf eine Imagemap wird ein externer Verweis aktiviert, der eine neue Webseite öffnet, auf der Sie mehr über ein Element erfahren können.

Um eine Imagemap zu erstellen, öffnen Sie den Anzeigebereich „E-Katalog“. Wechseln Sie dann zur Registerkarte **[!UICONTROL Seiten zuordnen]** des Bildschirms „eCatalog“ und ziehen Sie mit dem Tool „Rechteck-Imagemap“ oder dem Tool „Polygon-Imagemap“ einen Rahmen um die Karte. Sie können die Position und Größe von Imagemaps anpassen, indem Sie mit dem Schwenk -Tool Kartenränder ziehen.

Geben Sie nach dem Frame der Imagemap die URL-Adresse ein, zu der Sie wechseln möchten, wenn Sie die Imagemap auswählen. Sie können auch den Rollover-Text eingeben, der beim Bewegen des Mauszeigers über die Imagemap angezeigt werden soll. 

Siehe [Erstellen von eCatalog-Imagemaps](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Siehe [Verwenden von Imagemaps zum Einbetten von Rich-Media in einen E-Katalog](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Sie können den Imagemap-Text mithilfe der Einstellungen des Infobereichs im E-Katalog-Bildschirm einrichten und verwalten.

Siehe [Inhalt des Infobereichs in E-Katalogen verwalten](/help/using/info-panel-content-ecatalog.md).

## &#x200B;4. Einrichten von E-Katalog-Viewer-Vorgaben

Den Endbenutzern wird der E-Katalog im E-Katalog-Viewer angezeigt. Wenn Sie ein Administrator sind, können Sie den E-Katalog-Viewer konfigurieren. Sie können die Konturfarbe ändern und ein neues „Design“ auswählen, um Ihren E-Katalog mit einem Branding zu versehen. Adobe Dynamic Media Classic verfügt über mehrere „Best Practice“-E-Katalog-Viewer-Vorgaben. Sie können eine dieser Vorgaben zum Anzeigen Ihrer E-Kataloge auswählen. Als Administrator können Sie jedoch auch eigene E-Katalog-Viewer-Vorgaben erstellen.

Um eine Viewer-Vorgabe für E-Kataloge zu erstellen, klicken Sie in der globalen Navigationsleiste auf **[!UICONTROL Setup]** und wählen Sie dann **[!UICONTROL Viewer-Vorgaben]**. Wählen Sie **[!UICONTROL Hinzufügen]**, wählen Sie eine Plattform und dann **[!UICONTROL eCatalog]** > **[!UICONTROL Viewer]**.

Siehe [Einrichten von E-Katalog-Viewer-Vorgaben](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## &#x200B;5. Vorschau von E-Katalogen im E-Katalog-Viewer

Mithilfe von E-Katalog-Viewer-Vorgaben wird der Stil und das Verhalten von E-Katalog-Viewern festgelegt.

Um herauszufinden, wie E-Katalog-Viewer-Vorgaben Ihren E-Katalog anzeigen, wählen Sie Ihren E-Katalog im Durchsuchen-Bedienfeld aus und klicken Sie dann auf **[!UICONTROL Vorschau]**. Die Vorschau wird in dem als Standard festgelegten Viewer geöffnet.

Achten Sie auf Ausrichtung, Farbschema, Aussehen der Steuerelemente zum Umblättern der Seiten und Aussehen der Seiten beim Umblättern. 

Siehe [Vorschau von E-Katalogen im E-Katalog-Viewer](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## &#x200B;6. Veröffentlichen von E-Katalogen und zugehörigen PDFs

Durch das Veröffentlichen des E-Katalogs und der zugehörigen PDF wird er auf Dynamic Media-Bildservern platziert, sodass er auf Ihrer Website und in Ihrem Programm bereitgestellt werden kann. Im Rahmen des Veröffentlichungsprozesses aktiviert Adobe Dynamic Media Classic die URL-Zeichenfolge für Ihren E-Katalog. Verwenden Sie diese URL, um den E-Katalog von Dynamic Media-Bildservern an Ihre Website oder Anwendung aufzurufen.

Nachdem Sie Ihren E-Katalog und PDF im Durchsuchen-Panel zur Veröffentlichung markiert haben, klicken Sie in der globalen Navigationsleiste auf die Schaltfläche Veröffentlichen , um eine Veröffentlichung zu starten. Klicken Sie auf der Seite „Veröffentlichen“ auf **[!UICONTROL Veröffentlichung starten]**.

Siehe [Veröffentlichen von E-Katalogen und zugehörigen PDF-](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## &#x200B;7. Verknüpfen eines E-Katalogs mit einer Web-Seite

Adobe Dynamic Media Classic aktiviert die URL-Legendenzeichenfolge, die für die Anzeige Ihres E-Katalogs erforderlich ist, wenn Sie ihn auf Dynamic Media-Bildservern veröffentlichen. Sie können diese URL-Zeichenfolge aus dem Bildschirm Vorschau und dem Durchsuchen-Panel (in der Detailansicht) kopieren, indem Sie URLs im Panel auswählen. Nachdem Sie die URL-Zeichenfolge kopiert haben, ist sie für Ihre Websites und Programme verfügbar.

Arbeiten Sie mit Ihrem IT-Team zusammen, um den Link zum E-Katalog an der entsprechenden Stelle auf Ihrer Web-Seite zu platzieren. Wenn Benutzer den Link auswählen, wird der E-Katalog-Viewer angezeigt, und Benutzer können Ihren E-Katalog durchsuchen.

Siehe [Verknüpfen eines E-Katalogs mit einer Web-Seite](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
