---
title: "Schnellstart: Bildsets"
description: Eine Einführung und ein Schnellstart zu Bildsets , die Ihnen helfen, die Bildset-Techniken in Adobe Dynamic Media Classic schnell einzurichten und auszuführen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
topic: Content Management
level: Beginner
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 10%

---

# Kurzanleitung: Bildsätze{#quick-start-image-sets}

Adobe Dynamic Media Classic-Bildsets bieten Benutzern ein integriertes Anzeigeerlebnis. Im dynamischen Bildset-Viewer können Benutzer unterschiedliche Ansichten eines Elements anzeigen, indem sie ein Miniaturbild auswählen. Mit Bildsets können Sie alternative hochauflösende Ansichten eines Elements darstellen.

Der Bildsatz-Viewer bietet auch Zoomfunktionen zur genauen Betrachtung der Bilder. Sie können bei Bedarf &quot;Geführte Zoom-Ziele&quot;und &quot;Imagemaps&quot;in das Bildset aufnehmen. Durch Bildsätze wird das Betrachten der Bilder stimmiger und individueller.

Siehe Schulungsvideo [Bild- und Rotationssets: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) .

Beim Erstellen eines Bildsets empfiehlt Adobe die folgenden Best Practices und setzt die folgenden Einschränkungen voraus:

| Begrenzungstyp | Optimale Vorgehensweise | Erzwungene Beschränkung |
| --- | --- | --- |
| Anzahl der doppelten Assets pro Satz | Keine Duplikate | 20 ‡ |
| Maximale Anzahl an Bildern pro Set | 5 - 10 Bilder pro Set | 1000 |

‡ Best Practice ist, keine doppelten Assets in einem Satz zu haben. Die Beschränkung beträgt 20 Duplikate für ein einzelnes Asset. Wenn Sie ein weiteres Duplikat für dieses Asset innerhalb dieses Satzes hinzufügen, gibt die Anfrage entweder einen Fehler aus oder ignoriert das Duplikat.

Siehe auch [Dynamic Media-Einschränkungen](/help/using/limitations.md).

Der folgende Schnellstart für Bildsets soll Ihnen einen schnellen Einstieg in die Bildset-Techniken in Adobe Dynamic Media Classic ermöglichen.

## 1. Laden Sie die Primärbilder für mehrere Ansichten und Muster hoch.

Laden Sie zuerst die Bilder für die Bildsätze hoch. Da Benutzer Bilder im Bildset-Viewer einzoomen können, müssen Sie diese Möglichkeit bei der Auswahl von Bildern berücksichtigen. Achten Sie darauf, dass die längste Seite der Bilder mindestens 2000 Pixel hat. Adobe Dynamic Media Classic unterstützt viele Bilddateiformate. Es werden jedoch verlustfreie TIFF-, PNG- und EPS-Bilder empfohlen.

Wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Hochladen]** aus, um Dateien von Ihrem Computer in einen Ordner in Adobe Dynamic Media Classic hochzuladen.

Siehe [Vorbereiten von Bildset-Assets für den Upload](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) und [Hochladen Ihrer Dateien](uploading-files.md#uploading-your-files).

## 2. Erstellen eines Bildsets

In Bildsets wählen Benutzer Miniaturansichten im Bildset-Viewer aus, um ein Bild von einer anderen Seite oder einem anderen Winkel anzuzeigen.

Um ein Bildset zu erstellen, wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Build]** und dann **[!UICONTROL Bildsets]** aus. Ziehen Sie im Fenster Bildset Ihre Bilder auf die Seite, um das Bildset zusammenzustellen. Organisieren und löschen Sie Bilder wie gewünscht und fügen Sie sie hinzu. 

Siehe [Erstellen eines Bildsets](creating-image-set.md#creating-an-image-set).

Siehe auch [Einschließen von Zoomzielen und Imagemaps in Bildsets](/help/using/including-zoom-targets-image-maps-image-sets.md)

## 3. Bereiten Sie bei Bedarf Bildset-Viewer-Vorgaben vor.

Administratoren können Bildsatz-Viewer-Vorgaben erstellen oder ändern. Adobe Dynamic Media Classic enthält standardmäßige Viewer-Vorgaben für jeden Rich-Media-Typ. Verwenden Sie den Zoom-Viewer: Vorgaben für **[!UICONTROL Benutzerdefiniert]** > **[!UICONTROL Bilder]** oder **[!UICONTROL Bildsets]**/**[!UICONTROL Mehrere Ansichten]** , um Ihre Bildsets anzuzeigen.

Sie können Viewer-Vorgaben über den Bildschirm &quot;Anwendungseinstellungen&quot;hinzufügen oder bearbeiten.

Siehe [Erstellen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding-and-editing-viewer-presets).

## 4. Vorschau eines Bildsets

Wählen Sie im Bedienfeld &quot;Durchsuchen&quot;das Bildset und dann **[!UICONTROL Vorschau]** aus. Wählen Sie auf der Seite &quot;Vorschau&quot;die Miniaturansichtssymbole aus, um das Bildset im ausgewählten Viewer zu untersuchen. Sie können auch andere Vorgaben aus dem Menü „Vorgaben“ auswählen. 

Siehe [Vorschau eines Assets anzeigen](previewing-asset.md#previewing-an-asset).

## 5. Publish und Bildset

Beim Veröffentlichen eines Bildsets wird es auf Adobe Dynamic Media Classic-Servern platziert und die URL-Zeichenfolge aktiviert.

>[!NOTE]
>
>Dieser Schritt ist nicht erforderlich, wenn Sie zum Zeitpunkt der Erstellung und Speicherung des Bildsets **[!UICONTROL Publish nach dem Speichern]** (Standard) ausgewählt haben.

Wählen Sie im Bedienfeld &quot;Durchsuchen&quot;links neben dem Namen das Symbol &quot;**[!UICONTROL Für Publish markieren]**&quot;. Wählen Sie dann **[!UICONTROL Publish]** aus. Wählen Sie auf der Seite &quot;Publishing&quot;die Option **[!UICONTROL Publish übermitteln]**.

Siehe [Publish-Dateien](publishing-files.md#publishing-files).

## 6. Verknüpfen eines Bildsets mit Ihrer Website

Adobe Dynamic Media Classic erstellt URL-Aufrufe für Bildsets und aktiviert diese nach der Veröffentlichung. Sie können diese URLs im Anzeigebereich „Vorschau“ kopieren.

Wählen Sie das Bildset und dann **[!UICONTROL Vorschau]** aus. Wählen Sie jetzt eine Bildset-Viewer-Vorgabe aus und klicken Sie dann auf die Schaltfläche **[!UICONTROL URL kopieren]** .

Siehe [Verknüpfen des Bildsets mit einer Webseite](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
