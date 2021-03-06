---
title: '"Kurzanleitung: Bildsätze"'
description: Eine Einführung und ein Schnellstart zu Bildsets , die Ihnen helfen, die Bildset-Techniken in Adobe Dynamic Media Classic schnell einzurichten und auszuführen.
uuid: daf17d13-9c06-41f0-8fc5-2e56d460d341
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 612a425f-2840-46c4-8e5a-c0bc5f738f4e
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
source-git-commit: 92a28b7868e03802f4ef1c113ec3f8b34f57ed56
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 21%

---

# Kurzanleitung: Bildsätze{#quick-start-image-sets}

Adobe Dynamic Media Classic-Bildsets bieten Benutzern ein integriertes Anzeigeerlebnis. Im dynamischen Bildsatz-Viewer können die Benutzer verschiedene Ansichten eines Elements anzeigen, indem sie auf eine Miniaturansicht klicken. Mit Bildsets können Sie alternative hochauflösende Ansichten eines Elements darstellen.

Der Bildsatz-Viewer bietet auch Zoomfunktionen zur genauen Betrachtung der Bilder. Sie haben die Möglichkeit, geführte Zoomziele und Imagemaps im Bildsatz zu erstellen. Durch Bildsätze wird das Betrachten der Bilder stimmiger und individueller.

Siehe [Bild- und Rotationssets: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) Schulungsvideo.

Beim Erstellen eines Bildsets empfiehlt Adobe die folgenden Best Practices und setzt die folgenden Einschränkungen um:

| Begrenzungstyp | Optimale Vorgehensweise | Begrenzung auferlegt |
| --- | --- | --- |
| Anzahl der doppelten Assets pro Satz | Keine Duplikate | 20 |
| Maximale Anzahl an Bildern pro Set | 5 - 10 Bilder pro Set | 1000 |

Siehe auch [Einschränkungen bei Dynamic Media](/help/limitations.md).

Der folgende Schnellstart für Bildsets soll Ihnen einen schnellen Einstieg in die Bildset-Techniken in Adobe Dynamic Media Classic ermöglichen.

## 1. Laden Sie die Primärbilder für mehrere Ansichten und Muster hoch.

Laden Sie zuerst die Bilder für die Bildsätze hoch. Da Benutzer Bilder im Bildset-Viewer einzoomen können, müssen Sie diese Möglichkeit bei der Auswahl von Bildern berücksichtigen. Achten Sie darauf, dass die längste Seite der Bilder mindestens 2000 Pixel hat. Adobe Dynamic Media Classic unterstützt viele Bilddateiformate. Es werden jedoch verlustfreie TIFF-, PNG- und EPS-Bilder empfohlen.

Wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Hochladen]** , um Dateien von Ihrem Computer in einen Ordner in Adobe Dynamic Media Classic hochzuladen.

Siehe [Vorbereiten von Bildset-Assets für das Hochladen](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) und [Hochladen der Dateien](uploading-files.md#uploading-your-files).

## 2. Erstellen eines Bildsets

In Bildsets wählen Benutzer Miniaturansichten im Bildset-Viewer aus, um ein Bild von einer anderen Seite oder einem anderen Winkel anzuzeigen.

Um ein Bildset zu erstellen, wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Build]**, wählen Sie **[!UICONTROL Bildsets]**. Ziehen Sie im Fenster Bildset Ihre Bilder auf die Seite, um das Bildset zusammenzustellen. Organisieren und löschen Sie Bilder wie gewünscht und fügen Sie sie hinzu. 

Siehe [Erstellen eines Bildsets](creating-image-set.md#creating-an-image-set).

Siehe auch [Zoomziele und Imagemaps in Bildsets einschließen](/help/including-zoom-targets-image-maps-image-sets.md)

## 3. Bereiten Sie bei Bedarf Bildset-Viewer-Vorgaben vor.

Administratoren können Bildsatz-Viewer-Vorgaben erstellen oder ändern. Adobe Dynamic Media Classic enthält standardmäßige Viewer-Vorgaben für jeden Rich-Media-Typ. Verwenden des Zoom-Viewers: **[!UICONTROL Benutzerdefiniert]** > **[!UICONTROL Bilder]** oder **[!UICONTROL Bildsets]**/**[!UICONTROL Mehrere Ansichten]** Vorgaben, um Ihre Bildsets anzuzeigen.

Sie können Viewer-Vorgaben aus dem Anzeigebereich „Anwendungseinstellungen“ hinzufügen oder bearbeiten. 

Siehe [Erstellen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding-and-editing-viewer-presets).

## 4. Vorschau eines Bildsets

Wählen Sie das Bildset im Durchsuchenbedienfeld aus und wählen Sie dann **[!UICONTROL Vorschau]**. Wählen Sie auf der Seite &quot;Vorschau&quot;die Miniaturansichtssymbole aus, um das Bildset im ausgewählten Viewer zu untersuchen. Sie können auch andere Vorgaben aus dem Menü „Vorgaben“ auswählen. 

Siehe [Asset-Vorschau](previewing-asset.md#previewing-an-asset).

## 5. Veröffentlichen eines Bildsets

Beim Veröffentlichen eines Bildsets wird es auf Adobe Dynamic Media Classic-Servern platziert und die URL-Zeichenfolge aktiviert.

>[!NOTE]
>
>Dieser Schritt ist nicht erforderlich, wenn Sie beim Erstellen und Speichern des Bildsatzes die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** (Standard) ausgewählt haben.

Auswählen **[!UICONTROL Zur Veröffentlichung markieren]** im Durchsuchenbedienfeld links neben dem Namen. Wählen Sie anschließend **[!UICONTROL Veröffentlichen]**. Wählen Sie auf der Seite Veröffentlichen die Option **[!UICONTROL Veröffentlichung übermitteln]**.

Siehe [Veröffentlichen von Dateien](publishing-files.md#publishing-files).

## 6. Verknüpfen eines Bildsets mit Ihrer Website

Adobe Dynamic Media Classic erstellt URL-Aufrufe für Bildsets und aktiviert diese nach der Veröffentlichung. Sie können diese URLs im Anzeigebereich „Vorschau“ kopieren.

Wählen Sie das Bildset aus und klicken Sie auf **[!UICONTROL Vorschau]**. Wählen Sie jetzt eine Bildset-Viewer-Vorgabe aus und wählen Sie **[!UICONTROL URL kopieren]**.

Siehe [Verknüpfen eines Bildsets mit einer Webseite](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
