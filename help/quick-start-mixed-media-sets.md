---
title: '"Schnellstart: gemischtes Medienset"'
description: Eine Einführung und ein Schnellstart zu gemischten Mediensets, die Ihnen dabei helfen, in Adobe Dynamic Media Classic schnell einzurichten und auszuführen.
uuid: 0ef033d5-b053-4d7c-b1e1-1980f899fd88
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 2708d077-94fc-4045-8992-ad3589ed9cfd
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 757893ae-7507-42a0-a67b-f6542e7231c7
source-git-commit: 36f9aa3c2b4dc66e4cb851c2ce6837ae0ad4f64c
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 38%

---

# Kurzanleitung: Gemischte Mediensets{#quick-start-mixed-media-sets}

Gemischte Mediensets von bieten Benutzern eine integrierte Anzeigeerfahrung. Gemischte Mediensets können Bilder, Bildsätze, Mustersets, Rotationssets und Videos beinhalten. Benutzer können verschiedene Registerkarten im Viewer für gemischte Medien auswählen, um die Elemente in den verschiedenen Viewern anzuzeigen. Falls keine Registerkarten angegeben werden, werden alle Assets gemeinsam in der Musterzeile angezeigt.

Die Viewer-Vorgaben für gemischte Mediensets enthalten Community-Optionen, mit denen Endbenutzer Code einbetten, URLs kopieren und Verknüpfungen zur Haupt-Website erstellen können. Über diese Optionen können Benutzer Produktinformationen auf ihren eigenen Websites oder Social-Networking-Sites zur Verfügung stellen.

Dieser Schnellstart für gemischte Mediensets wurde entwickelt, um schnell mit gemischten Mediensets-Techniken in Adobe Dynamic Media Classic vertraut zu machen.

## 1. Hochladen der Bilder, Musterdateien und Videos

Laden Sie zunächst die Bilder, Musterdateien und Videos für Ihre gemischten Mediensets hoch. Da Benutzer Bilder im Viewer für gemischte Mediensets einzoomen können, achten Sie bei der Auswahl von Bildern auf diese Möglichkeit. Achten Sie darauf, dass die längste Seite der Bilder mindestens 2000 Pixel hat.

Wählen Sie in der Symbolleiste für globale Navigation **[!UICONTROL Upload]** aus, um Dateien von Ihrem Computer in einen Ordner auf Adobe Dynamic Media Classic hochzuladen.

Siehe [Hochladen Ihrer Dateien](uploading-files.md#uploading-your-files).

## 2. Erstellen Sie Mediensets zur Verwendung im gemischten Medienset

Sie können Bilder, Bildsätze, Mustersets, Rotationssets und Videos zu Ihrem gemischten Medienset hinzufügen. Bereiten Sie die Mediensets vor, bevor Sie sie zum gemischten Medienset hinzufügen.

Siehe [Erstellen eines Bildsets](creating-image-set.md#creating-an-image-set), [Erstellen eines Mustersets](creating-swatch-set.md#creating-a-swatch-set) und [Erstellen eines Rotationssets](creating-spin-set.md#creating-a-spin-set).

## 3. Erstellen eines gemischten Mediensets

Wechseln Sie in der globalen Navigationsleiste zu **[!UICONTROL Build]** > **[!UICONTROL Gemischte Mediensets]**. Ziehen Sie die Bilder, Mustersets, Bildsets und Videos auf die Seite &quot;Gemischtes Medienset&quot;. Um einen Soundtrack hinzuzufügen, ziehen Sie eine Audiodatei in das Feld „Tonspur“. 

Siehe [Erstellen eines gemischten Mediensets](creating-mixed-media-set.md#creating-a-mixed-media-set).

## 4. Einrichten von Viewer-Vorgaben für gemischte Medien

Adobe Dynamic Media Classic enthält standardmäßige Viewer-Vorgaben für gemischte Mediensets. Administratoren können Viewer-Vorgaben für gemischte Mediensets erstellen oder ändern.

Fügen Sie beim Einrichten einer Viewer-Vorgabe für gemischte Mediensets die Viewer-Vorgaben für alle anderen Assets in Ihrem Set hinzu. Falls Ihr gemischtes Medienset beispielsweise Videos enthält, fügen Sie eine Video-Viewer-Vorgabe zur Viewer-Vorgabe für gemischte Mediensets hinzu. Sie können auch einen Soundtrack zum Viewer hinzufügen. Dieser Soundtrack wird abgespielt, wenn der Viewer geöffnet ist. Wenn ein Video abgespielt wird, wird die Soundtrack-Wiedergabe unterbrochen. 

Siehe [Einrichten einer Viewer-Vorgabe für gemischte Mediensets](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) und [Erstellen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding-and-editing-viewer-presets).

## 5. Vorschau eines gemischten Mediensets

Wählen Sie die Schaltfläche **[!UICONTROL Vorschau]** des gemischten Mediensets aus. Sie können die Miniaturansichten und Mustersymbole auswählen, um das gemischte Medienset im Viewer für gemischte Mediensets zu untersuchen. Sie können verschiedene Viewer aus den Menüs „Vorgaben“ auswählen. 

Siehe [Asset-Vorschau](previewing-asset.md#previewing-an-asset).

## 6. Veröffentlichen eines gemischten Mediensets

Beim Veröffentlichen eines gemischten Mediensets wird dieses auf Adobe Dynamic Media Classic-Servern platziert und die URL-Zeichenfolge aktiviert.

Gemischte Mediensets müssen sowohl auf dem **Video-Server** als auch auf dem **Image-Server** veröffentlicht werden. Sie verwenden den **Video-Server**, um die eigentlichen Videos zu veröffentlichen, die Sie für die Veröffentlichung markiert haben. Außerdem verwenden Sie **Image-Server**, um verwandte Assets wie die Videominiaturen zu veröffentlichen und Informationen für adaptive Videosets festzulegen.

Siehe [Veröffentlichen eines gemischten Mediensets](publishing-mixed-media-set.md#publishing-a-mixed-media-set).

## 7. Verknüpfen eines gemischten Mediensets mit einer Webseite

Adobe Dynamic Media Classic aktiviert URL-Aufrufe für gemischte Mediensets, nachdem Sie sie veröffentlicht haben. Sie können diese URLs von der Seite &quot;Vorschau&quot;kopieren.

Wählen Sie das gemischte Medienset und dann **[!UICONTROL Vorschau]** aus. Wählen Sie auf der Seite &quot;Vorschau&quot;eine Viewer-Vorgabe für gemischte Mediensets aus und klicken Sie dann auf **[!UICONTROL URL kopieren]**. Siehe [Verknüpfen eines gemischten Mediensets mit einer Webseite](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page).
