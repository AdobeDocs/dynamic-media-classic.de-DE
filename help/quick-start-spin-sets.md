---
title: '"Kurzanleitung: Rotationssets"'
description: Eine Einführung und ein Schnellstart für das Rotationsset, damit Sie in Adobe Dynamic Media Classic schnell arbeiten können.
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
source-git-commit: d5dcb990783932f3c5fdd101d1a4c631e73fcdde
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 22%

---

# Kurzanleitung: Rotationssets{#quick-start-spin-sets}

Mit einem Rotationsset wird simuliert, wie man ein reales Objekt dreht, um es von allen Seiten betrachten zu können. Rotationssets ermöglichen die Anzeige von Objekten aus einem beliebigen Blickwinkel, um seine wichtigsten visuellen Eigenschaften zu erfassen. Ein Rotationsset simuliert eine 360°-Anzeige. Adobe Dynamic Media Classic bietet eindimensionale Rotationssets, in denen die Viewer ein Element drehen können, und zweidimensionale Rotationssets, in denen die Viewer das Element drehen und spiegeln können. Darüber hinaus können Benutzer mit wenigen einfachen Mausklicks beliebige Ansichten &quot;frei&quot;zoomen und schwenken. Auf diese Weise können Benutzer ein Objekt näher und aus einer bestimmten Perspektive betrachten.

![Bilder für ein Rotationsset.](/help/assets/spin_set.png)

Rotationssets akzeptieren auch Imagemaps. Eine Imagemap ist ein Bereich auf einem Bild in einem Rotationsset, mit dessen Hilfe ein Rollover-Bedienfeld mit Text angezeigt werden kann. Wenn der Benutzer auf eine Imagemap klickt, wird eine bestimmte Aktion ausgelöst. Beispielsweise kann eine Website aufgerufen werden, auf der der Benutzer mehr über ein Produkt erfährt. Um auf eine Imagemap in einem Rotationsset zu verweisen, wird um die Imagemap selbst herum ein Umriss angezeigt, wenn der Benutzer den Mauszeiger darüber bewegt.

Siehe [Erstellen von Imagemaps](creating-image-maps.md).

Siehe [Bild- und Rotationssets: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) Schulungsvideo.

Beim Erstellen eines Rotationssets empfiehlt Adobe die folgenden Best Practices und erzwingt die folgende Beschränkung:

| Rotationsset-Begrenzungstyp | Optimale Vorgehensweise | Implementierte Beschränkung |
| --- | --- | --- |
| Maximale Anzahl von Zeilen/Spalten pro 2D-Satz | 12-18 Bilder pro Set | 1000 |

Siehe auch [Einschränkungen bei Dynamic Media](/help/limitations.md).

Diese Kurzanleitung für Rotationssets soll Sie in Adobe Dynamic Media Classic schnell mit den Rotationssets-Techniken vertraut machen. Führen Sie die Schritte 1 bis 7 aus. Am Ende jedes Schritts können Sie einen Themenlink auswählen, um mehr zu erfahren.

## 1. Erstellen und Hochladen der Bilder

Sie benötigen mindestens 8 bis 12 Aufnahmen eines Elements für ein eindimensionales Rotationsset und 16 bis 24 Aufnahmen für ein zweidimensionales Rotationsset. Die Aufnahmen müssen in regelmäßigen Abständen gemacht werden, um den Eindruck von Rotation und Spiegelung zu erwecken. Wenn ein eindimensionales Rotationsset beispielsweise 12 Aufnahmen enthält, drehen Sie das Element für jeden Schuss um 30° (360°/12).

Wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Hochladen]** , um Rotations-Bilder von Ihrem Computer oder Netzwerk in Adobe Dynamic Media Classic hochzuladen.

Siehe [Richtlinien für das Aufnehmen von Rotationsset-Bildern](creating-spin-set.md#guidelines-for-shooting-spin-set-images).

## 2. Erstellen eines Rotationssets

Um ein Rotationsset zu erstellen, navigieren Sie in der Symbolleiste für globale Navigation zu **[!UICONTROL Build]** > **[!UICONTROL Rotationssets]**. Wählen Sie im Dialogfeld &quot;Größe des Rotationssets&quot;aus, wie viele Zeilen und Zellen Sie benötigen, und wählen Sie **[!UICONTROL OK]**. Ziehen Sie dann Bilder in das Raster auf der Seite Rotationsset .

Siehe [Erstellen eines Rotationssets](creating-spin-set.md#creating-a-spin-set).

## 3. Bearbeiten von Rotationssets

Um ein Rotationsset zu bearbeiten, navigieren Sie in der Symbolleiste für globale Navigation zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Viewer-Vorgaben]**. Wählen Sie ein Rotationsset aus und klicken Sie auf **[!UICONTROL Bearbeiten]**. Fügen Sie Bilder hinzu, löschen Sie sie und ändern Sie ihre Position. Sie können die Position der Zeilen in zweidimensionalen Rotationssets ändern. 

Siehe [Bearbeiten eines Rotationssets](creating-spin-set.md#editing-a-spin-set).

## 4. Einrichten von Rotationsset-Viewer-Vorgaben

Administratoren können Rotationsset-Viewer-Vorgaben erstellen. Mit einer solchen Vorgabe wird das Aussehen eines Rotationsset-Viewers festgelegt. Um eine neue Rotationsset-Viewer-Vorgabe einzurichten, navigieren Sie in der Symbolleiste für globale Navigation zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Viewer-Vorgaben]**.

Wählen Sie auf der Seite &quot;Viewer-Vorgaben&quot;die Option **[!UICONTROL Hinzufügen]**, wählen Sie **[!UICONTROL Rotationsset-Viewer]** aus der Dropdownliste aus und wählen Sie dann **[!UICONTROL Hinzufügen]**. Wählen Sie auf der Seite &quot;Viewer konfigurieren&quot;Optionen aus und klicken Sie auf **[!UICONTROL Speichern]**.

Siehe [Einrichten von Rotationsset-Viewer-Vorgaben](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## 5. Vorschau eines Rotationssets

Wählen Sie das Rotationsset im Durchsuchenbedienfeld aus und wählen Sie dann **[!UICONTROL Vorschau]**. Halten Sie auf der Seite Vorschau die Maustaste gedrückt und ziehen Sie den Zeiger nach links oder rechts, um das Element visuell zu &quot;drehen&quot;.

Siehe [Vorschau eines Rotationssets](previewing-spin-set.md#previewing-a-spin-set).

## 6. Veröffentlichen eines Rotationssets

Durch das Veröffentlichen eines Rotationssets wird es auf Adobe Dynamic Media Classic-Servern platziert, damit es dynamisch auf Ihrer Website oder in Ihrer Anwendung bereitgestellt werden kann. Außerdem wird die URL-Zeichenfolge aktiviert, mit der das Rotationsset von den Dynamic Media-Bildservern auf Ihre Website oder Anwendung aufgerufen wird.

Um ein Rotationsset zu veröffentlichen, markieren Sie es zur Veröffentlichung, indem Sie die **[!UICONTROL Zur Veröffentlichung markieren]** im Durchsuchenbedienfeld neben dem Namen angezeigt. Wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Veröffentlichen]** , um eine Veröffentlichung zu initiieren. Wählen Sie im Bildschirm &quot;Veröffentlichen&quot;die Option **[!UICONTROL Veröffentlichung übermitteln]**.

Siehe [Veröffentlichen eines Rotationssets](publishing-spin-set.md#publishing-a-spin-set).

## 7. Verknüpfen eines Rotationssets mit einer Webseite

Adobe Dynamic Media Classic erstellt URL-Callout-Zeichenfolgen für Rotationssets und aktiviert sie nach der Veröffentlichung. Sie können diese URLs von der Seite &quot;Vorschau&quot;kopieren.

Wählen Sie das Rotationsset aus und klicken Sie auf **[!UICONTROL Vorschau]**. Wählen Sie eine Rotationsset-Viewer-Vorgabe aus. Wählen Sie anschließend **[!UICONTROL URL kopieren]**.

Siehe [Verknüpfen eines Rotationssets mit einer Webseite](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
