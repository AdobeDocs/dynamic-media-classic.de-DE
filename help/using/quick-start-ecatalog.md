---
title: "Schnellstart: E-Kataloge"
description: Eine Einführung in und ein Schnellstart für E-Kataloge, die Ihnen helfen, in Adobe Dynamic Media Classic schnell mit E-Katalog-Techniken umzugehen.
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

Ein eCatalog ist eine digitale, Web-Version des Druckmaterials - z. B. ein Katalog, eine Broschüre, ein Flyer, ein Produkthandbuch oder ein Werbezirkus. Ein E-Katalog wird in einem E-Katalog-Viewer auf einer Website angezeigt. Dieser Viewer simuliert die Erfahrung beim Lesen gedruckter Materialien.

Siehe auch die folgenden Schulungsvideos:

* [Schnellstart 1: E-Kataloge](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [Schnellstart 2: E-Kataloge](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

Je nach den Einstellungen, die Sie für Ihren E-Katalog auswählen, können Sie mit dem Viewer Folgendes tun:

* Suchen Sie im Katalog nach einem oder mehreren Keywords. Die Suchergebnisse werden als Liste von Miniaturansichten in einem Suchbereich auf der linken Seite des Katalogs angezeigt. Jede klickbare Miniaturansicht stellt einen Katalogbereich dar, in dem der markierte Suchbegriff gefunden wurde.

* Geben Sie den Katalog über soziale Medien frei. Laden Sie den Katalog herunter, um ihn offline anzuzeigen. Aktivieren Sie Favoriten, um Elemente zu markieren, zu denen Sie zurückkehren möchten, oder drucken Sie den Katalog.
* Navigieren Sie im Katalog mithilfe des Inhaltsverzeichnisses oder der Seitenrasteransicht, der Seite vorwärts oder rückwärts, indem Sie den mittleren Rand einer Seite auswählen.
* Heranzoomen, Herauszoomen und Schwenken, um bestimmte Elemente auf einer Seite genau zu betrachten
* Bewegen Sie den Mauszeiger über einen Seitenbereich (eine so genannte Imagemap), damit Sie ein Popup-Fenster mit Informationen zu einem Element sehen können.
* Wählen Sie einen Seitenbereich aus, damit eine neue Webseite mit weiteren Informationen zu einem Element geöffnet wird.
* Schreiben und Anbringen eines Klebezettels als Lesezeichen an einer bestimmten E-Katalogseite
* Tippen Sie auf Imagemap-Symbole, wenn Sie zugehörige Webseiten oder kontextbezogene Informationsbedienfelder starten möchten.
* Verwenden von Gesten zur Interaktion, einschließlich der Zangenbewegung zum Zoomen und der Wischbewegung zum Umblättern von Seiten.
* Durchsuchen der Elemente nach bestimmten Schlüsselwörtern

![Der eCatalog, wie er Benutzern angezeigt wird. A) eCatalog zur Seite zum Öffnen. B)eCatalog auf Seite 2 umgestellt.](/help/using/assets/ec_cat_viewer_popup.png)

Um einen E-Katalog zu erstellen, verwenden Sie normalerweise PDF-Dateien mit hoher Auflösung, die in Adobe Acrobat oder einem anderen Druckprogramm erstellt wurden. Sie können jedoch auch einen E-Katalog aus Bilddateien erstellen.

Während der Erstellung des E-Katalogs können Sie Seiten oder Druckbögen in der gewünschten Reihenfolge anordnen. Darüber hinaus können Sie angeben, ob Einzelseiten, doppelseitige Druckbögen oder mehrseitige Druckbögen verwendet werden sollen. Sie können Imagemaps für Seitenbereiche erstellen, sodass Betrachter beispielsweise einen Bereich auf der Seite auswählen und eine neue Seite auf Ihrer Website öffnen können. Der Rollover-Text, der angezeigt wird, kann mithilfe der Infofeldeinstellungen im Anzeigebereich „E-Katalog“ verwaltet werden. Außerdem haben Sie bei der Konfiguration des E-Katalog-Viewers die Möglichkeit, aus mehr als 100 verschiedenen Konfigurationsoptionen zu wählen. Sie können die Funktionen und die Darstellung des Viewers speziell für die gewünschte Zielgruppe anpassen.

>[!NOTE]
>
>Wenn Sie ein Benutzer im Modus Dynamic Media: Scene7 sind und E-Kataloge verwenden möchten, bearbeiten Sie den Wert `pdfbrochure` im CRXDE Lite. Gehen Sie dazu in Adobe Experience Manager zu **[!UICONTROL Tools]** > **[!UICONTROL Allgemein]** > **[!UICONTROL CRXDE Lite]**. Navigieren Sie in der Navigationsstruktur des linken Bedienfelds zu `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>Wählen Sie im unteren rechten Bereich auf der Registerkarte **[!UICONTROL Eigenschaften]** die Zeile `jobParam` aus. Legen Sie den Wert für `pdfbrochure` von `false` auf `true` fest. Wie in `pdfbrochure=true`
>
>Wählen Sie oben links auf der CRXDE Lite-Seite **[!UICONTROL Alle speichern]** aus.
>
>Sie können jetzt E-Kataloge in Adobe Dynamic Media Classic erstellen.

Diese Kurzanleitung für die Erstellung eines E-Katalogs hilft Ihnen, sich schnell mit den E-Katalogfunktionen vertraut zu machen. Führen Sie die Schritte 1 bis 7 aus. Nach jedem Schritt gibt es einen Querverweis zu einer Themenüberschrift, in der Sie weitere Informationen finden können.

## 1. Hochladen der PDF-Dateien

Normalerweise werden Adobe PDF-Dateien als Grundlage für einen E-Katalog verwendet. Da PDF-Dateien speziell zum Drucken vorgesehen sind, enthalten sie normalerweise CMYK-Bilder. Adobe Dynamic Media Classic erkennt diese Bilder und konvertiert sie mithilfe eines standardmäßigen CMYK-Farbprofils. Sie müssen jedoch ein benutzerdefiniertes Farbprofil hochladen und verwenden.

Wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Hochladen]** aus, um mit dem Hochladen von PDF-Dateien oder -Bildern für Ihren E-Katalog zu beginnen. Sie können Dateien von Ihrem Desktop oder via FTP hochladen. FTP wird empfohlen, wenn Sie viele Dateien oder Dateien hochladen, die größer als 100 MB sind.

Im Anzeigebereich „Hochladen“ finden Sie im Bereich „PDF-Optionen“ Einstellungen für das Hochladen von PDF-Dateien mit der angemessenen Auflösung und dem richtigen Farbraum. Eine Auflösung von 150 Pixel pro Zoll wird empfohlen. Sie können die Option **[!UICONTROL E-Katalog automatisch erstellen]** auswählen, um beim Hochladen einer PDF-Datei einen E-Katalog zu erstellen.

Siehe [Hochladen der PDF-Dateien](uploading-pdf-files.md#uploading_the_pdf_files).

## 2. Erstellen eines E-Katalogs

Erstellen Sie Ihren eCatalog, indem Sie im Bedienfeld Durchsuchen PDF- oder Bilddateien auswählen. Wählen Sie **[!UICONTROL Build]** und dann **[!UICONTROL eCatalogs]**.

Wählen Sie auf der eCatalog-Seite auf der Registerkarte **[!UICONTROL Seiten bestellen]** eine Layout-Option: **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]** oder **[!UICONTROL Custom]**. Sie können die Anordnung der Seiten oder Druckbögen durch Ziehen oder, insbesondere in großen E-Katalogen, durch Auswahl eines Seitennamens im Menü „Verschieben nach“ ändern.

Um Seiten hinzuzufügen, wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die gewünschten PDF-Dateien oder Bilddateien aus dem Ordner in den Anzeigebereich „Seiten ordnen“. Anstelle der standardmäßigen Seitenzahlen können Sie benutzerdefinierte Seitennamen angeben oder viele Seitennamen importieren.

Wählen Sie &quot;**[!UICONTROL Speichern]**&quot;, geben Sie einen Namen für den E-Katalog ein, wählen Sie einen Adobe Dynamic Media Classic-Ordner zum Speichern aus und wählen Sie &quot;**[!UICONTROL Speichern]**&quot;. Jedes Mal, wenn Sie die Seitenreihenfolge ändern oder den E-Katalog bearbeiten, speichern Sie Ihre Änderungen, indem Sie **[!UICONTROL Speichern]** auswählen.

Siehe [E-Katalog erstellen](creating-ecatalog.md).

## 3. Erstellen von Imagemaps

Imagemaps fügen eCatalog-Seiten einen weiteren Aspekt hinzu. Eine Imagemap ist ein Seitenbereich, mit dessen Hilfe weitere Informationen zu einem Element angezeigt werden können. Wenn Betrachter der Website den Mauszeiger über eine Imagemap bewegen, wird eine Beschreibung des Elements angezeigt. Durch Klicken auf eine Imagemap wird eine externe Referenz aktiviert, die eine neue Webseite öffnet, auf der Sie mehr über ein Element erfahren können.

Um eine Imagemap zu erstellen, öffnen Sie den Anzeigebereich „E-Katalog“. Navigieren Sie dann zur Registerkarte **[!UICONTROL Seiten zuordnen]** des E-Katalog-Bildschirms und rahmen Sie die Karte mit dem Rechteck-Bild-Map-Tool oder dem Polygon-Imagemap-Tool. Sie können die Position und Größe von Imagemaps anpassen, indem Sie mit dem Werkzeug Schwenken Kartenränder ziehen.

Geben Sie nach dem Frame der Imagemap die URL-Adresse ein, die Sie verwenden möchten, wenn Sie die Imagemap auswählen. Sie können auch den Rollover-Text eingeben, der beim Bewegen des Mauszeigers über die Imagemap angezeigt werden soll. 

Siehe [Erstellen von eCatalog-Imagemaps](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

Siehe [Verwenden von Imagemaps zum Einbetten von Rich Media in einen eCatalog](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Sie können den Text der Imagemap mithilfe der Einstellungen für das Infofeld im E-Katalog-Bildschirm einrichten und verwalten.

Siehe [Verwalten des Informationsbereichsinhalts in E-Katalogen](/help/using/info-panel-content-ecatalog.md).

## 4. E-Katalog-Viewer-Vorgaben einrichten

Den Endbenutzern wird der E-Katalog im E-Katalog-Viewer angezeigt. Wenn Sie ein Administrator sind, können Sie den E-Katalog-Viewer konfigurieren. Sie können die Farbe des Versandentwurfs ändern und eine neue &quot;Skin&quot;auswählen, um Ihren E-Katalog zu markieren. Adobe Dynamic Media Classic enthält mehrere bewährte E-Katalog-Viewer-Vorgaben. Sie können eine dieser Vorgaben für die Anzeige Ihrer E-Kataloge auswählen. Als Administrator können Sie jedoch auch eigene E-Katalog-Viewer-Vorgaben erstellen.

Um eine E-Katalog-Viewer-Vorgabe zu erstellen, wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Einrichtung]** und dann **[!UICONTROL Viewer-Vorgaben]** aus. Wählen Sie &quot;**[!UICONTROL Hinzufügen]**&quot;, wählen Sie eine Plattform und dann &quot;**[!UICONTROL eCatalog]**&quot;> &quot;**[!UICONTROL Betrachter]**&quot;.

Siehe [Einrichten von E-Katalog-Viewer-Vorgaben](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## 5. Anzeigen einer Vorschau von E-Katalogen im E-Katalog-Viewer

Mithilfe von E-Katalog-Viewer-Vorgaben wird der Stil und das Verhalten von E-Katalog-Viewern festgelegt.

Um herauszufinden, wie eCatalog-Viewer-Vorgaben Ihren E-Katalog anzeigen, wählen Sie Ihren eCatalog im Bedienfeld Durchsuchen und dann **[!UICONTROL Vorschau]** aus. Die Vorschau wird in dem als Standard festgelegten Viewer geöffnet.

Achten Sie auf Ausrichtung, Farbschema, Aussehen der Steuerelemente zum Umblättern der Seiten und Aussehen der Seiten beim Umblättern. 

Siehe [Anzeigen einer Vorschau von E-Katalogen im E-Katalog-Viewer](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6. Publish eCatalog und zugehörige PDF

Durch das Veröffentlichen Ihres E-Katalogs und des zugehörigen PDF wird dieser auf Dynamic Media-Bildservern platziert, damit er auf Ihrer Website und in Ihrer Anwendung bereitgestellt werden kann. Im Zuge der Veröffentlichung aktiviert Adobe Dynamic Media Classic die URL-Zeichenfolge für Ihren E-Katalog. Verwenden Sie diese URL, um den eCatalog von Dynamic Media Image-Servern für Ihre Website oder Anwendung aufzurufen.

Nachdem Sie Ihren eCatalog und Ihren PDF zur Veröffentlichung im Bedienfeld Durchsuchen markiert haben, wählen Sie in der Symbolleiste für globale Navigation die Schaltfläche Publish aus, um eine Veröffentlichung zu starten. Wählen Sie auf der Seite &quot;Publishing&quot;die Option **[!UICONTROL Publish übermitteln]**.

Siehe [Publish-E-Kataloge und zugehörige PDF](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7. Verknüpfen eines E-Katalogs mit einer Webseite

Adobe Dynamic Media Classic aktiviert die URL-Aufrufzeichenfolge, die zum Anzeigen des E-Katalogs beim Veröffentlichen auf Dynamic Media-Image-Servern erforderlich ist. Sie können diese URL-Zeichenfolge aus dem Vorschaubildschirm und dem Durchsuchenbedienfeld (in der Detailansicht) kopieren, indem Sie im Bedienfeld URLs auswählen. Nachdem Sie die URL-Zeichenfolge kopiert haben, ist sie für Ihre Websites und Anwendungen verfügbar.

Arbeiten Sie mit Ihrem IT-Team zusammen, um den Link zum eCatalog an der entsprechenden Stelle auf Ihrer Webseite zu platzieren. Wenn Benutzer den Link auswählen, wird der E-Katalog-Viewer angezeigt und Benutzer können Ihren E-Katalog durchsuchen.

Siehe [Verknüpfen eines E-Katalogs mit einer Webseite](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
