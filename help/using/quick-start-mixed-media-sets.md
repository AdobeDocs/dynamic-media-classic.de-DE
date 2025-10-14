---
title: 'Schnellstart: Gemischtes Medienset'
description: Eine Einführung und eine Kurzanleitung zu gemischten Mediensets, mit denen Sie in Adobe Dynamic Media Classic schnell loslegen können.
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

Gemischte Mediensets bieten Benutzenden ein integriertes Anzeigeerlebnis. Gemischte Mediensets können Bilder, Bildsätze, Mustersets, Rotationssets und Videos beinhalten. Benutzer können verschiedene Registerkarten im Viewer für gemischte Medien auswählen, um die Elemente in den verschiedenen Viewern anzuzeigen. Falls keine Registerkarten angegeben werden, werden alle Assets gemeinsam in der Musterzeile angezeigt.

Viewer-Vorgaben für gemischte Mediensets enthalten Community-Optionen für Endbenutzer zum Einbetten von Code, Kopieren von URLs und Verknüpfen mit der Haupt-Website. Benutzer können diese Optionen verwenden, um Informationen über Produkte auf ihren persönlichen Websites oder in sozialen Netzwerken auszutauschen.

Dieser Schnellstart für gemischte Mediensets soll Ihnen den schnellen Einstieg in die Arbeit mit gemischten Mediensets in Adobe Dynamic Media Classic erleichtern.

## &#x200B;1. Hochladen von Bildern, Musterdateien und Videos

Laden Sie zunächst die Bilder, Musterdateien und Videos für Ihre gemischten Mediensets hoch. Da Benutzer Bilder im Viewer für gemischte Mediensets einzoomen können, sollten Sie diese Funktion bei der Auswahl von Bildern berücksichtigen. Achten Sie darauf, dass die längste Seite der Bilder mindestens 2.000 Pixel hat.

Wählen Sie in der globalen Navigationsleiste **[!UICONTROL Hochladen]** aus, um Dateien von Ihrem Computer in einen Ordner in Adobe Dynamic Media Classic hochzuladen.

Siehe [Hochladen von Dateien](uploading-files.md#uploading-your-files).

## &#x200B;2. Erstellen Sie Mediensets zur Verwendung im gemischten Medienset

Sie können Bilder, Bildsets, Mustersets, Rotationssets und Videos zu Ihrem gemischten Medienset hinzufügen. Bereiten Sie die Mediensets vor, bevor Sie sie zum gemischten Medienset hinzufügen.

Siehe [Erstellen eines Bildsets](creating-image-set.md#creating-an-image-set), [Erstellen eines &#x200B;](creating-swatch-set.md#creating-a-swatch-set) und [Erstellen eines Rotationssets](creating-spin-set.md#creating-a-spin-set).

## &#x200B;3. Erstellen eines gemischten Mediensets

Navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Erstellen]** > **[!UICONTROL Gemischte Mediensets]**. Ziehen Sie die Bilder, Mustersets, Bildsets und Videos auf die Seite Gemischtes Medienset . Um einen Soundtrack hinzuzufügen, ziehen Sie eine Audiodatei in das Feld „Tonspur“. 

Siehe [Erstellen eines gemischten Mediensets](creating-mixed-media-set.md#creating-a-mixed-media-set).

## &#x200B;4. Einrichten von Viewer-Vorgaben für gemischte Medien

Adobe Dynamic Media Classic verfügt über standardmäßige Viewer-Vorgaben für gemischte Mediensets. Admins können Viewer-Vorgaben für gemischte Mediensets erstellen oder ändern.

Fügen Sie beim Einrichten einer Viewer-Vorgabe für ein gemischtes Medienset die Viewer-Vorgaben für alle anderen Assets in Ihrem Set hinzu. Wenn Ihr gemischtes Medienset beispielsweise Videos enthält, fügen Sie eine Video-Viewer-Vorgabe zur Viewer-Vorgabe für gemischtes Medienset hinzu. Sie können auch einen Soundtrack zum Viewer hinzufügen. Dieser Soundtrack wird abgespielt, wenn der Viewer geöffnet ist. Wenn ein Video abgespielt wird, wird die Soundtrack-Wiedergabe unterbrochen. 

Siehe [Einrichten einer Viewer-Vorgabe für ein gemischtes Medienset](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) und [Erstellen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding-and-editing-viewer-presets).

Siehe auch [Viewer-Vorgaben](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) Schulungsvideo.

## &#x200B;5. Vorschau eines gemischten Mediensets

Klicken Sie auf die Schaltfläche **[!UICONTROL Vorschau]** des gemischten Mediensets. Sie können auf die Miniaturansichten und Mustersymbole klicken, um das gemischte Medienset im Viewer für das gemischte Medienset zu überprüfen. Sie können verschiedene Viewer aus den Menüs „Vorgaben“ auswählen. 

Siehe [Vorschau eines Assets](previewing-asset.md#previewing-an-asset).

## &#x200B;6. Veröffentlichen eines gemischten Mediensets

Beim Veröffentlichen eines gemischten Mediensets wird es auf Adobe Dynamic Media Classic-Servern platziert und die URL-Zeichenfolge aktiviert.

Gemischte Mediensets müssen sowohl auf dem **Video-Server** als auch auf dem **Image-Server** veröffentlicht werden. Verwenden Sie **Videoserver**, um die tatsächlichen Videos zu veröffentlichen, die Sie zur Veröffentlichung markiert haben. Darüber hinaus verwenden Sie **Bild-Server**, um zugehörige Assets wie die Videominiaturen zu veröffentlichen und Informationen für beliebige adaptive Videosets festzulegen.

Siehe [Veröffentlichen eines gemischten Mediensets](publishing-mixed-media-set.md#publishing-a-mixed-media-set).

## &#x200B;7. Verknüpfen eines gemischten Mediensets mit einer Web-Seite

Adobe Dynamic Media Classic aktiviert URL-Aufrufe für gemischte Mediensets nach deren Veröffentlichung. Sie können diese URLs von der Vorschauseite kopieren.

Wählen Sie das gemischte Medienset und dann **[!UICONTROL Vorschau]** aus. Wählen Sie auf der Seite Vorschau eine Viewer-Vorgabe für gemischte Mediensets und dann die **[!UICONTROL URL kopieren]** aus. Siehe [Verknüpfen von gemischten Mediensets mit Webseiten](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page).
