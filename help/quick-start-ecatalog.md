---
title: '"Beginn: E-Kataloge"'
description: Einführung und Quick Beginn zu E-Katalogen, mit denen Sie sich schnell mit E-Katalog-Techniken vertraut machen können.
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic, Viewer, E-Katalog
role: Geschäftspraktiker
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1453'
ht-degree: 63%

---


# Quick Beginn: E-Kataloge{#quick-start-ecatalogs}

Ein E-Katalog ist eine digitale Webversion von Druckwerbematerial, z. B. von Katalogen, Broschüren, Handzetteln, Produkthandbüchern oder Werberundschreiben. Ein E-Katalog wird auf einer Website in einem E-Katalog-Viewer angezeigt. Dieser Viewer simuliert denselben Leseeindruck wie beim Betrachten von Druckwerbematerial. Je nach den Einstellungen, die Sie für Ihren E-Katalog auswählen, können Sie im Viewer Folgendes ausführen:

* Suchen Sie im Katalog nach einem oder mehreren Suchbegriffen. Die Suchergebnisse werden als Liste von Miniaturansichten in einem Suchfeld auf der linken Seite des Katalogs angezeigt. Jede klickbare Miniaturansicht stellt einen Katalogbogen dar, in dem der markierte Suchbegriff gefunden wurde.

* Freigeben des Katalogs über soziale Medien; den Katalog offline in die Ansicht herunterladen; Aktivieren Sie Favoriten, um Elemente zu markieren, zu denen Sie schnell zurückkehren möchten, oder den Katalog zu drucken.
* Navigieren Sie zum Katalog mit dem Inhaltsverzeichnis oder der Ansicht des Seitenrasters. Seite vorwärts oder rückwärts durch Klicken auf den mittleren Rand einer Seite.
* Heranzoomen, Herauszoomen und Schwenken, um bestimmte Elemente auf einer Seite genau zu betrachten
* Bewegen des Mauszeigers über bestimmte Seitenbereiche (so genannte Imagemaps), um ein Popup-Fenster mit Informationen zu den Elementen anzuzeigen
* Klicken auf einen bestimmten Seitenbereich, um eine neue Website mit weiteren Informationen zu einem Element zu öffnen.
* Schreiben und Anbringen eines Klebezettels als Lesezeichen an einer bestimmten E-Katalogseite
* Tippen auf Imagemap-Symbole, um zugehörige Websites oder Kontext-Infofelder anzuzeigen.
* Verwenden von Gesten zur Interaktion, einschließlich der Zangenbewegung zum Zoomen und der Wischbewegung zum Umblättern von Seiten.
* Durchsuchen der Elemente nach bestimmten Schlüsselwörtern

![Der E-Katalog, wie er für Benutzer angezeigt wird. A) Öffnen des E-Katalogs. B)E-Katalog auf Seite 2 umgestellt.](/help/assets/ec_cat_viewer_popup.png)

Zum Erstellen eines E-Katalogs verwenden Sie normalerweise hoch auflösende PDF-Dateien, die in Adobe® Acrobat® oder einem anderen Druckprogramm erstellt wurden. Sie können jedoch auch einen E-Katalog aus Bilddateien erstellen.

Während der Erstellung des E-Katalogs können Sie Seiten oder Druckbögen in der gewünschten Reihenfolge anordnen. Darüber hinaus können Sie angeben, ob Einzelseiten, doppelseitige Druckbögen oder mehrseitige Druckbögen verwendet werden sollen. Sie können auch Imagemaps erstellen, sodass Benutzer auf bestimmte Seitenbereiche klicken können, um eine zugeordnete Seite Ihrer Website in einem neuen Fenster zu öffnen. Der Rollover-Text, der angezeigt wird, kann mithilfe der Infofeldeinstellungen im Anzeigebereich „E-Katalog“ verwaltet werden. Außerdem haben Sie bei der Konfiguration des E-Katalog-Viewers die Möglichkeit, aus mehr als 100 verschiedenen Konfigurationsoptionen zu wählen. Sie können die Funktionen und die Darstellung des Viewers speziell für die gewünschte Zielgruppe anpassen.

>[!NOTE]
>
>Wenn Sie im AEM Dynamic Media - Scene7-Modus arbeiten und E-Kataloge verwenden möchten, müssen Sie den `pdfbrochure`-Wert in der CRXDE Lite bearbeiten. Klicken Sie dazu in AEM auf **[!UICONTROL Tools > Allgemein > CRXDE Lite]**. Navigieren Sie in der Navigationsstruktur des linken Bedienfelds zu `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>Wählen Sie im unteren rechten Bereich auf der Registerkarte **[!UICONTROL Eigenschaften]** die Zeile `jobParam` aus. Legen Sie den Wert für `pdfbrochure` von `false` auf `true` fest. Wie in `pdfbrochure=true`
>
>Klicken Sie oben links auf der Seite &quot;CRXDE Lite&quot;auf **[!UICONTROL Alle speichern]**.
>
>Sie können jetzt E-Kataloge in Dynamic Media Classic erstellen.

**Quick Beginn**

Diese Kurzanleitung für die Erstellung eines E-Katalogs hilft Ihnen, sich schnell mit den E-Katalogfunktionen vertraut zu machen. Führen Sie die Schritte 1 bis 7 aus. Nach jedem Schritt wird auf ein Thema mit weiteren Informationen verwiesen.

**1. Hochladen der PDF-Dateien**

Normalerweise werden Adobe PDF-Dateien als Grundlage für einen E-Katalog verwendet. Da PDF-Dateien speziell zum Drucken vorgesehen sind, enthalten sie normalerweise CMYK-Bilder. Dynamic Media Classic erkennt diese Bilder und konvertiert sie mithilfe eines standardmäßigen CMYK-Profils. Es ist jedoch möglich, dass Sie ein benutzerdefiniertes Farbprofil verwenden und zu diesem Zweck hochladen müssen.

Klicken Sie in der Symbolleiste für globale Navigation auf &quot;Hochladen&quot;, um Beginn beim Hochladen von PDF-Dateien oder -Bildern für Ihren E-Katalog zu erhalten. Sie können die Dateien entweder vom Desktop oder per FTP hochladen. FTP ist zu empfehlen, wenn Sie viele Dateien oder Dateien, die größer als 100 MB sind, hochladen möchten.

Im Anzeigebereich „Hochladen“ finden Sie im Bereich „PDF-Optionen“ Einstellungen für das Hochladen von PDF-Dateien mit der angemessenen Auflösung und dem richtigen Farbraum. Eine Auflösung von 150 Pixel pro Zoll wird empfohlen. Wenn unmittelbar nach dem Hochladen einer PDF-Datei automatisch ein E-Katalog erstellt werden soll, wählen Sie die Option „E-Katalog automatisch erstellen“. 

Siehe [Hochladen von PDF-Dateien](uploading-pdf-files.md#uploading_the_pdf_files).

**2. Erstellen eines E-Katalogs**

Sie können einen E-Katalog erstellen, indem Sie im Durchsuchenbedienfeld PDF-Dateien oder Bilddateien markieren, dann auf „Erstellen“ klicken und schließlich „E-Kataloge“ wählen. Der Anzeigebereich „E-Katalog“ wird geöffnet.

Klicken Sie auf der Registerkarte „Seiten ordnen“ auf eine der Layout-Schaltflächen „1-fach“, „2-fach“ oder „Benutzerdefiniert“, um festzulegen, ob einseitige, doppelseitige oder benutzerdefinierte Druckbögen verwendet werden sollen. Sie können die Anordnung der Seiten oder Druckbögen durch Ziehen oder, insbesondere in großen E-Katalogen, durch Auswahl eines Seitennamens im Menü „Verschieben nach“ ändern.

Um Seiten hinzuzufügen, wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die gewünschten PDF-Dateien oder Bilddateien aus dem Ordner in den Anzeigebereich „Seiten ordnen“. Anstelle der Standardseitenzahlen können Sie benutzerdefinierte Seitennamen angeben oder eine große Anzahl von Seitennamen importieren.

Klicken Sie auf **[!UICONTROL Speichern]**, geben Sie einen Namen für den E-Katalog ein, wählen Sie einen Dynamic Media Classic-Ordner zum Speichern aus und klicken Sie auf **[!UICONTROL Speichern]**. Wenn Sie die Seitenreihenfolge ändern oder den E-Katalog bearbeiten, speichern Sie die Änderungen, indem Sie auf **[!UICONTROL Speichern]** klicken.

Siehe [Erstellen eines E-Katalogs](creating-ecatalog.md).

**3. Erstellen von Imagemaps**

Imagemaps erweitern E-Katalogseiten um eine weitere Dimension. Eine Imagemap ist ein Seitenbereich, mit dessen Hilfe weitere Informationen zu einem Element angezeigt werden können. Wenn Betrachter der Website den Mauszeiger über eine Imagemap bewegen, wird eine Beschreibung des Elements angezeigt. Durch Klicken auf eine Imagemap wird ein externer Verweis aktiviert, mit dem eine neue Website mit weiteren Informationen zu einem Element geöffnet wird.

Um eine Imagemap zu erstellen, öffnen Sie den Anzeigebereich „E-Katalog“. Rufen Sie dann die Registerkarte **[!UICONTROL Imagemap-Seiten]** des Anzeigebereichs &quot;E-Katalog&quot;auf und zeichnen Sie die Imagemap mit dem Rechteck-Imagemap-Werkzeug oder dem Polygon-Imagemap-Werkzeug. Durch Ziehen der Ränder mit dem Schwenken-Werkzeug  können Sie die Position und Größe von Imagemaps nachträglich ändern.

Nachdem Sie die Imagemap gezeichnet haben, geben Sie die URL-Adresse ein, die mit der Imagemap verknüpft sein soll. Sie können auch den Rollover-Text eingeben, der beim Bewegen des Mauszeigers über die Imagemap angezeigt werden soll. 

Siehe [Erstellen von E-Katalog-Imagemaps](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps). 

Siehe [Verwenden von Imagemaps zum Einbetten von Rich-Media-Daten in einen E-Katalog](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

Der Imagemap-Text kann mithilfe der Infofeldeinstellungen im Anzeigebereich „E-Katalog“ eingestellt und verwaltet werden. 

Siehe [ Verwalten des Infofeldinhalts](info-panel-content.md#managing-info-panel-content).

**4. Konfigurieren von E-Katalog-Viewer-Vorgaben**

Den Endbenutzern wird der E-Katalog im E-Katalog-Viewer angezeigt. Wenn Sie ein Administrator sind, können Sie den E-Katalog-Viewer konfigurieren. Sie können beispielsweise die Rahmenfarbe ändern und eine neue Skin zur Gestaltung des E-Katalogs auswählen. Im Lieferumfang von Dynamic Media Classic sind verschiedene bewährte E-Katalog-Viewer-Vorgaben enthalten. Sie können eine dieser Vorgaben zur Anzeige Ihrer E-Kataloge auswählen. Als Administrator können Sie jedoch auch eigene E-Katalog-Viewer-Vorgaben erstellen.

Um eine E-Katalog-Viewer-Vorgabe zu erstellen, klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Setup]** und wählen Sie **[!UICONTROL Viewer-Vorgaben]**. Klicken Sie dann auf **[!UICONTROL Hinzufügen]**, wählen Sie eine Plattform und klicken Sie dann auf **[!UICONTROL E-Katalog > Viewer]**.

Siehe [Konfigurieren von E-Katalog-Viewer-Vorgaben](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

**5. Anzeigen einer Vorschau von E-Katalogen im E-Katalog-Viewer**

Mithilfe von E-Katalog-Viewer-Vorgaben wird der Stil und das Verhalten von E-Katalog-Viewern festgelegt.

Um herauszufinden, wie der E-Katalog mit den E-Katalog-Viewer-Vorgaben angezeigt wird, wählen Sie den E-Katalog im Durchsuchenbedienfeld aus und klicken Sie auf **[!UICONTROL Vorschau]**. Die Vorschau wird in dem als Standard festgelegten Viewer geöffnet.

Achten Sie auf Ausrichtung, Farbschema, Aussehen der Steuerelemente zum Umblättern der Seiten und Aussehen der Seiten beim Umblättern. 

Siehe [Anzeigen einer Vorschau von E-Katalogen im E-Katalog-Viewer](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

**6. Veröffentlichen eines E-Katalogs und dazugehöriger PDFs**

Beim Veröffentlichen des E-Katalogs und der zugehörigen PDF-Datei wird dieser auf Dynamic Media-Image-Servern gespeichert, damit er an Ihre Website und Anwendung gesendet werden kann. Während des Veröffentlichungsvorgangs aktiviert Dynamic Media Classic die URL-Zeichenfolge für Ihren E-Katalog. Verwenden Sie diese URL, um den E-Katalog von den Dynamic Media-Image-Servern für Ihre Website oder Anwendung aufzurufen.

Nachdem Sie den E-Katalog und das PDF-Dokument zur Veröffentlichung markiert haben, klicken Sie im Durchsuchenbedienfeld in der Symbolleiste für globale Navigation auf &quot;Veröffentlichen&quot;, um eine Veröffentlichung zu starten. Klicken Sie im Anzeigebereich &quot;Veröffentlichen&quot;auf **[!UICONTROL Beginn Publish]**.

Siehe [Veröffentlichen von E-Katalogen und zugehörigen PDFs](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

**7. Verknüpfen eines E-Katalogs mit einer Website**

Dynamic Media Classic aktiviert die URL-Zeichenfolge, die zum Anzeigen des E-Katalogs beim Veröffentlichen auf Dynamic Media-Image-Servern erforderlich ist. Sie können diese URL-Zeichenfolge aus dem Anzeigebereich „Vorschau“ sowie aus dem Durchsuchenbedienfeld (in der Detailansicht) kopieren, nachdem Sie im Bedienfeld URLs ausgewählt haben. Nach dem Kopieren ist die URL-Zeichenfolge für Ihre Websites und Anwendungen verfügbar.

Platzieren Sie die Verknüpfung zum E-Katalog an geeigneter Stelle auf Ihrer Website (wenden Sie sich ggf. an die IT-Abteilung Ihres Unternehmens). Wenn Benutzer auf die Verknüpfung klicken, wird der E-Katalog-Viewer angezeigt, damit die Benutzer den E-Katalog durchsuchen können. 

Siehe [Verknüpfen eines E-Katalogs mit einer Website](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
