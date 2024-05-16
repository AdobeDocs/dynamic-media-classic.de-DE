---
title: "Schnellstart: gemischtes Medienset"
description: Eine Einführung und ein Schnellstart zu gemischten Mediensets, die Ihnen dabei helfen, in Adobe Dynamic Media Classic schnell einzurichten und auszuführen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 757893ae-7507-42a0-a67b-f6542e7231c7
topic: Content Management
level: Beginner
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 16%

---

# Kurzanleitung: Gemischte Mediensets{#quick-start-mixed-media-sets}

Gemischte Mediensets bieten Benutzern ein integriertes Anzeigeerlebnis. Gemischte Mediensets können Bilder, Bildsätze, Mustersets, Rotationssets und Videos beinhalten. Benutzer können verschiedene Registerkarten im Viewer für gemischte Medien auswählen, um die Elemente in den verschiedenen Viewern anzuzeigen. Falls keine Registerkarten angegeben werden, werden alle Assets gemeinsam in der Musterzeile angezeigt.

Viewer-Vorgaben für gemischte Mediensets enthalten Community-Optionen, mit denen Endbenutzer Code einbetten, URLs kopieren und einen Link zur Haupt-Website erstellen können. Benutzer können diese Optionen verwenden, um Informationen über Produkte auf ihren persönlichen Websites oder Social-Networking-Sites freizugeben.

Dieser Schnellstart für gemischte Mediensets wurde entwickelt, um Sie schnell mit den Techniken für gemischte Mediensets in Adobe Dynamic Media Classic vertraut zu machen.

## 1. Hochladen der Bilder, Musterdateien und Videos

Laden Sie zunächst die Bilder, Musterdateien und Videos für Ihre gemischten Mediensets hoch. Da Benutzer Bilder im Viewer für gemischte Mediensets einzoomen können, achten Sie bei der Auswahl von Bildern auf diese Möglichkeit. Achten Sie darauf, dass die längste Seite der Bilder mindestens 2000 Pixel hat.

Wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Hochladen]** , um Dateien von Ihrem Computer in einen Ordner in Adobe Dynamic Media Classic hochzuladen.

Siehe [Hochladen der Dateien](uploading-files.md#uploading-your-files).

## 2. Erstellen Sie Mediensets für die Verwendung im gemischten Medienset

Sie können Ihrem gemischten Medienset Bilder, Bildsets, Mustersets, Rotationssets und Videos hinzufügen. Bereiten Sie die Mediensets vor, bevor Sie sie zum gemischten Medienset hinzufügen.

Siehe [Erstellen eines Bildsets](creating-image-set.md#creating-an-image-set), [Erstellen eines Mustersets](creating-swatch-set.md#creating-a-swatch-set), und [Erstellen eines Rotationssets](creating-spin-set.md#creating-a-spin-set).

## 3. Erstellen eines gemischten Mediensets

Wechseln Sie in der Symbolleiste für globale Navigation zu **[!UICONTROL Build]** > **[!UICONTROL Gemischte Mediensets]**. Ziehen Sie die Bilder, Mustersets, Bildsets und Videos auf die Seite Gemischtes Medienset . Um einen Soundtrack hinzuzufügen, ziehen Sie eine Audiodatei in das Feld „Tonspur“. 

Siehe [Erstellen eines gemischten Mediensets](creating-mixed-media-set.md#creating-a-mixed-media-set).

## 4. Einrichten von Viewer-Vorgaben für gemischte Medien

Adobe Dynamic Media Classic enthält standardmäßige Viewer-Vorgaben für gemischte Mediensets. Administratoren können Viewer-Vorgaben für gemischte Mediensets erstellen oder ändern.

Fügen Sie beim Einrichten einer Viewer-Vorgabe für gemischte Mediensets die Viewer-Vorgaben für alle anderen Assets in Ihrem Set hinzu. Wenn Ihr Set für gemischte Medien beispielsweise Videos enthält, fügen Sie der Viewer-Vorgabe für gemischte Mediensets eine Video-Viewer-Vorgabe hinzu. Sie können auch einen Soundtrack zum Viewer hinzufügen. Dieser Soundtrack wird abgespielt, wenn der Viewer geöffnet ist. Wenn ein Video abgespielt wird, wird die Soundtrack-Wiedergabe unterbrochen. 

Siehe [Einrichten einer Viewer-Vorgabe für gemischte Mediensets](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) und [Erstellen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding-and-editing-viewer-presets).

Siehe auch [Viewer-Vorgaben](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) Schulungsvideo.

## 5. Vorschau eines gemischten Mediensets

Wählen Sie das gemischte Medienset aus **[!UICONTROL Vorschau]** Schaltfläche. Sie können die Miniaturansichten und Mustersymbole auswählen, um das gemischte Medienset im Viewer für gemischte Mediensets zu untersuchen. Sie können verschiedene Viewer aus den Menüs „Vorgaben“ auswählen. 

Siehe [Asset-Vorschau](previewing-asset.md#previewing-an-asset).

## 6. Veröffentlichen eines gemischten Mediensets

Beim Veröffentlichen eines gemischten Mediensets wird dieses auf Adobe Dynamic Media Classic-Servern platziert und die URL-Zeichenfolge aktiviert.

Gemischte Mediensets müssen sowohl auf dem **Video-Server** als auch auf dem **Image-Server** veröffentlicht werden. Verwendung **Video-Server** um die tatsächlichen Videos zu veröffentlichen, die Sie zur Veröffentlichung markiert haben. Und Sie verwenden **Image-Server** , um verwandte Assets wie die Videominiaturen zu veröffentlichen und Informationen für adaptive Videosets festzulegen.

Siehe [Veröffentlichen eines gemischten Mediensets](publishing-mixed-media-set.md#publishing-a-mixed-media-set).

## 7. Verknüpfen eines gemischten Mediensets mit einer Webseite

Adobe Dynamic Media Classic aktiviert URL-Aufrufe für gemischte Mediensets, nachdem Sie sie veröffentlicht haben. Sie können diese URLs von der Seite &quot;Vorschau&quot;kopieren.

Wählen Sie das gemischte Medienset aus und klicken Sie auf **[!UICONTROL Vorschau]**. Wählen Sie auf der Seite &quot;Vorschau&quot;eine Viewer-Vorgabe für gemischte Mediensets aus und wählen Sie dann die **[!UICONTROL URL kopieren]**. Siehe [Verknüpfen von gemischten Mediensets mit Webseiten](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page).
