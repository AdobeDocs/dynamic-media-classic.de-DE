---
title: '"Schnellstart: eCatalog"'
description: Eine Einführung und ein Schnellstart für E-Kataloge, die Ihnen helfen, die E-Katalog-Techniken schnell einzurichten und auszuführen.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic,Viewers,eCatalog
role: Business Practitioner
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 50%

---

# Schnellstart: E-Kataloge{#quick-start-ecatalogs}

Ein E-Katalog ist eine digitale Webversion von Druckwerbematerial, z. B. von Katalogen, Broschüren, Handzetteln, Produkthandbüchern oder Werberundschreiben. Ein E-Katalog wird auf einer Website in einem E-Katalog-Viewer angezeigt. Dieser Viewer simuliert denselben Leseeindruck wie beim Betrachten von Druckwerbematerial. Je nach den Einstellungen, die Sie für Ihren E-Katalog auswählen, können Sie mit dem Viewer Folgendes tun:

* Suchen Sie im Katalog nach einem oder mehreren Keywords. Die Suchergebnisse werden als Liste von Miniaturansichten in einem Suchbereich auf der linken Seite des Katalogs angezeigt. Jede klickbare Miniaturansicht stellt einen Katalogbereich dar, in dem der markierte Suchbegriff gefunden wurde.

* den Katalog über soziale Medien freigeben; den Katalog herunterladen, um ihn offline anzuzeigen; Aktivieren Sie Favoriten , um Elemente zu markieren, zu denen Sie schnell zurückkehren möchten, oder drucken Sie den Katalog.
* Navigieren Sie im Katalog mit dem Inhaltsverzeichnis oder der Seitenrasteransicht. Seite vorwärts oder rückwärts durch Klicken auf den mittleren Rand einer Seite.
* Heranzoomen, Herauszoomen und Schwenken, um bestimmte Elemente auf einer Seite genau zu betrachten
* Bewegen Sie den Mauszeiger über einen Seitenbereich (eine so genannte Imagemap), damit Sie ein Popup-Fenster mit Informationen zu einem Element sehen können.
* Klicken Sie auf einen Seitenbereich, damit eine neue Webseite mit weiteren Informationen zu einem Element geöffnet wird.
* Schreiben und Anbringen eines Klebezettels als Lesezeichen an einer bestimmten E-Katalogseite
* Tippen Sie auf Imagemap-Symbole, wenn Sie zugehörige Web-Seiten oder kontextbezogene Infofelder starten möchten.
* Verwenden von Gesten zur Interaktion, einschließlich der Zangenbewegung zum Zoomen und der Wischbewegung zum Umblättern von Seiten.
* Durchsuchen der Elemente nach bestimmten Schlüsselwörtern

![Der eCatalog, wie er Benutzern angezeigt wird. A) eCatalog zur Seite zum Öffnen. B)eCatalog, der auf Seite 2.](/help/assets/ec_cat_viewer_popup.png)

Zum Erstellen eines E-Katalogs verwenden Sie normalerweise hoch auflösende PDF-Dateien, die in Adobe® Acrobat® oder einem anderen Druckprogramm erstellt wurden. Sie können jedoch auch einen E-Katalog aus Bilddateien erstellen.

Während der Erstellung des E-Katalogs können Sie Seiten oder Druckbögen in der gewünschten Reihenfolge anordnen. Darüber hinaus können Sie angeben, ob Einzelseiten, doppelseitige Druckbögen oder mehrseitige Druckbögen verwendet werden sollen. Sie können auch Imagemaps erstellen, sodass Benutzer auf bestimmte Seitenbereiche klicken können, um eine zugeordnete Seite Ihrer Website in einem neuen Fenster zu öffnen. Der Rollover-Text, der angezeigt wird, kann mithilfe der Infofeldeinstellungen im Anzeigebereich „E-Katalog“ verwaltet werden. Außerdem haben Sie bei der Konfiguration des E-Katalog-Viewers die Möglichkeit, aus mehr als 100 verschiedenen Konfigurationsoptionen zu wählen. Sie können die Funktionen und die Darstellung des Viewers speziell für die gewünschte Zielgruppe anpassen.

>[!NOTE]
>
>Wenn Sie Benutzer im Modus Dynamic Media - Scene7 sind und E-Kataloge verwenden möchten, müssen Sie den Wert `pdfbrochure` in CRXDE Lite bearbeiten. Klicken Sie dazu in Adobe Experience Manager auf **[!UICONTROL Tools]** > **[!UICONTROL Allgemein]** > **[!UICONTROL CRXDE Lite]**. Navigieren Sie in der Navigationsstruktur des linken Bedienfelds zu `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>Wählen Sie im unteren rechten Bereich auf der Registerkarte **[!UICONTROL Eigenschaften]** die Zeile `jobParam` aus. Legen Sie den Wert für `pdfbrochure` von `false` auf `true` fest. Wie in `pdfbrochure=true`
>
>Klicken Sie oben links auf der CRXDE Lite auf **[!UICONTROL Alle speichern]**.
>
>Sie können jetzt E-Kataloge in Dynamic Media Classic erstellen.

Diese Kurzanleitung für die Erstellung eines E-Katalogs hilft Ihnen, sich schnell mit den E-Katalogfunktionen vertraut zu machen. Führen Sie die Schritte 1 bis 7 aus. Nach jedem Schritt wird auf ein Thema mit weiteren Informationen verwiesen.

## 1. Hochladen der PDF-Dateien

Normalerweise werden Adobe PDF-Dateien als Grundlage für einen E-Katalog verwendet. Da PDF-Dateien speziell zum Drucken vorgesehen sind, enthalten sie normalerweise CMYK-Bilder. Dynamic Media Classic erkennt diese Bilder und konvertiert sie mithilfe eines standardmäßigen CMYK-Farbprofils. Sie müssen jedoch ein benutzerdefiniertes Farbprofil hochladen und verwenden.

Klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Upload]** , um mit dem Hochladen von PDF-Dateien oder Bildern für Ihren E-Katalog zu beginnen. Sie können die Dateien entweder vom Desktop oder per FTP hochladen. FTP ist zu empfehlen, wenn Sie viele Dateien oder Dateien, die größer als 100 MB sind, hochladen möchten.

Im Anzeigebereich „Hochladen“ finden Sie im Bereich „PDF-Optionen“ Einstellungen für das Hochladen von PDF-Dateien mit der angemessenen Auflösung und dem richtigen Farbraum. Eine Auflösung von 150 Pixel pro Zoll wird empfohlen. Wenn unmittelbar nach dem Hochladen einer PDF-Datei automatisch ein E-Katalog erstellt werden soll, wählen Sie die Option „E-Katalog automatisch erstellen“. 

Siehe [Hochladen von PDF-Dateien](uploading-pdf-files.md#uploading_the_pdf_files).

## 2. Erstellen eines E-Katalogs

Erstellen Sie den E-Katalog, indem Sie im Durchsuchenbedienfeld PDF- oder Bilddateien auswählen. Klicken Sie auf **[!UICONTROL Build]** und wählen Sie dann **[!UICONTROL eCatalogs]** aus.

Wählen Sie auf der eCatalog-Seite auf der Registerkarte **[!UICONTROL Seiten sortieren]** eine Layout-Option: **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]** oder **[!UICONTROL Custom]**. Sie können die Anordnung der Seiten oder Druckbögen durch Ziehen oder, insbesondere in großen E-Katalogen, durch Auswahl eines Seitennamens im Menü „Verschieben nach“ ändern.

Um Seiten hinzuzufügen, wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die gewünschten PDF-Dateien oder Bilddateien aus dem Ordner in den Anzeigebereich „Seiten ordnen“. Anstelle der standardmäßigen Seitenzahlen können Sie benutzerdefinierte Seitennamen angeben oder viele Seitennamen importieren.

Klicken Sie auf **[!UICONTROL Speichern]**, geben Sie einen Namen für Ihren E-Katalog ein, wählen Sie einen Ordner in Dynamic Media Classic zum Speichern aus und klicken Sie auf **[!UICONTROL Speichern]**. Jedes Mal, wenn Sie die Seitenreihenfolge ändern oder den E-Katalog bearbeiten, speichern Sie Ihre Änderungen, indem Sie auf **[!UICONTROL Speichern]** klicken.

Siehe [Erstellen eines E-Katalogs](creating-ecatalog.md).

## 3. Erstellen von Imagemaps

Imagemaps fügen eCatalog-Seiten einen weiteren Aspekt hinzu. Eine Imagemap ist ein Seitenbereich, mit dessen Hilfe weitere Informationen zu einem Element angezeigt werden können. Wenn Betrachter der Website den Mauszeiger über eine Imagemap bewegen, wird eine Beschreibung des Elements angezeigt. Durch Klicken auf eine Imagemap wird ein externer Verweis aktiviert, mit dem eine neue Website mit weiteren Informationen zu einem Element geöffnet wird.

Um eine Imagemap zu erstellen, öffnen Sie den Anzeigebereich „E-Katalog“. Gehen Sie dann zum Tab **[!UICONTROL Seiten zuordnen]** des E-Katalog-Bildschirms und rahmen Sie die Karte mit dem Rechteck-Bild-Map-Tool oder dem Polygon-Imagemap-Tool. Durch Ziehen der Ränder mit dem Schwenken-Werkzeug  können Sie die Position und Größe von Imagemaps nachträglich ändern.

Geben Sie nach dem Frame der Imagemap die URL-Adresse ein, die Sie verwenden möchten, wenn Sie auf die Imagemap klicken. Sie können auch den Rollover-Text eingeben, der beim Bewegen des Mauszeigers über die Imagemap angezeigt werden soll. 

Siehe [Erstellen von E-Katalog-Imagemaps](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps). 

Siehe [Verwenden von Imagemaps zum Einbetten von Rich-Media-Daten in einen E-Katalog](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Der Imagemap-Text kann mithilfe der Infofeldeinstellungen im Anzeigebereich „E-Katalog“ eingestellt und verwaltet werden. 

Siehe [ Verwalten des Infofeldinhalts](info-panel-content.md#managing-info-panel-content).

## 4. Einrichten von E-Katalog-Viewer-Vorgaben

Den Endbenutzern wird der E-Katalog im E-Katalog-Viewer angezeigt. Wenn Sie ein Administrator sind, können Sie den E-Katalog-Viewer konfigurieren. Sie können beispielsweise die Rahmenfarbe ändern und eine neue Skin zur Gestaltung des E-Katalogs auswählen. Dynamic Media Classic verfügt über mehrere bewährte eCatalog-Viewer-Vorgaben. Sie können eine dieser Vorgaben für die Anzeige Ihrer E-Kataloge auswählen. Als Administrator können Sie jedoch auch eigene E-Katalog-Viewer-Vorgaben erstellen.

Um eine E-Katalog-Viewer-Vorgabe zu erstellen, klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Einrichtung]** und wählen Sie **[!UICONTROL Viewer-Vorgaben]** aus. Klicken Sie dann auf **[!UICONTROL Hinzufügen]**, wählen Sie eine Plattform aus und klicken Sie dann auf **[!UICONTROL eCatalog > Viewer]**.

Siehe [Konfigurieren von E-Katalog-Viewer-Vorgaben](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## 5. Anzeigen einer Vorschau von E-Katalogen im E-Katalog-Viewer

Mithilfe von E-Katalog-Viewer-Vorgaben wird der Stil und das Verhalten von E-Katalog-Viewern festgelegt.

Um herauszufinden, wie eCatalog-Viewer-Vorgaben Ihren E-Katalog anzeigen, wählen Sie Ihren eCatalog im Durchsuchenbedienfeld aus und klicken Sie auf **[!UICONTROL Vorschau]**. Die Vorschau wird in dem als Standard festgelegten Viewer geöffnet.

Achten Sie auf Ausrichtung, Farbschema, Aussehen der Steuerelemente zum Umblättern der Seiten und Aussehen der Seiten beim Umblättern. 

Siehe [Anzeigen einer Vorschau von E-Katalogen im E-Katalog-Viewer](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6. Veröffentlichen des E-Katalogs und der zugehörigen PDFs

Durch das Veröffentlichen Ihres E-Katalogs und der zugehörigen PDF-Datei wird dieser auf Dynamic Media-Bildservern platziert, damit er auf Ihrer Website und in Ihrer Anwendung bereitgestellt werden kann. Im Zuge der Veröffentlichung aktiviert Dynamic Media Classic die URL-Zeichenfolge für Ihren eCatalog. Verwenden Sie diese URL, um den eCatalog von Dynamic Media Image-Servern für Ihre Website oder Anwendung aufzurufen.

Nachdem Sie Ihren E-Katalog und Ihre PDF-Datei im Durchsuchenbedienfeld zur Veröffentlichung markiert haben, wählen Sie in der Symbolleiste für globale Navigation die Schaltfläche Veröffentlichen aus, um eine Veröffentlichung zu starten. Klicken Sie im Bildschirm &quot;Veröffentlichen&quot;auf **[!UICONTROL Veröffentlichen senden]**.

Siehe [Veröffentlichen von E-Katalogen und zugehörigen PDFs](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7. Verknüpfen eines E-Katalogs mit einer Webseite

Dynamic Media Classic aktiviert die URL-Callout-Zeichenfolge, die zum Anzeigen des E-Katalogs beim Veröffentlichen auf Dynamic Media-Image-Servern erforderlich ist. Sie können diese URL-Zeichenfolge aus dem Anzeigebereich „Vorschau“ sowie aus dem Durchsuchenbedienfeld (in der Detailansicht) kopieren, nachdem Sie im Bedienfeld URLs ausgewählt haben. Nach dem Kopieren ist die URL-Zeichenfolge für Ihre Websites und Anwendungen verfügbar.

Platzieren Sie die Verknüpfung zum E-Katalog an geeigneter Stelle auf Ihrer Website (wenden Sie sich ggf. an die IT-Abteilung Ihres Unternehmens). Wenn Benutzer auf die Verknüpfung klicken, wird der E-Katalog-Viewer angezeigt, damit die Benutzer den E-Katalog durchsuchen können. 

Siehe [Verknüpfen eines E-Katalogs mit einer Website](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
