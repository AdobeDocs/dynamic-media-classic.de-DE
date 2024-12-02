---
title: 'Kurzanleitung: Rotationssets'
description: Eine Einführung und ein Schnellstart für das Rotationsset, damit Sie in Adobe Dynamic Media Classic schnell arbeiten können.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
topic: Content Management
level: Beginner
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 22%

---

# Kurzanleitung: Rotationssets{#quick-start-spin-sets}

Mit einem Rotationsset wird simuliert, wie man ein reales Objekt dreht, um es von allen Seiten betrachten zu können. Rotationssets ermöglichen die Anzeige von Objekten aus einem beliebigen Blickwinkel, um seine wichtigsten visuellen Eigenschaften zu erfassen. Ein Rotationsset simuliert eine 360°-Rundumansicht des Objekts. Adobe Dynamic Media Classic bietet eindimensionale Rotationssets, in denen die Viewer ein Element drehen können, und zweidimensionale Rotationssets, in denen die Viewer das Element drehen und spiegeln können. Darüber hinaus können Benutzer mit wenigen einfachen Mausklicks beliebige Ansichten &quot;frei&quot;zoomen und schwenken. Auf diese Weise können Benutzer ein Objekt näher und aus einer bestimmten Perspektive betrachten.

![Bilder für ein Rotationsset.](/help/using/assets/spin_set.png)

Rotationssets akzeptieren auch Imagemaps. Eine Imagemap ist ein Bereich auf einem Bild in einem Rotationsset, mit dessen Hilfe ein Rollover-Bedienfeld mit Text angezeigt werden kann. Wenn der Benutzer eine Imagemap auswählt, wird eine Aktion irgendeiner Art ausgelöst. Beispielsweise wird eine Webseite gestartet, damit der Benutzer mehr über ein Produkt erfahren kann. Um auf eine Imagemap in einem Rotationsset zu verweisen, wird um die Imagemap selbst herum ein Umriss angezeigt, wenn der Benutzer den Mauszeiger darüber bewegt.

Siehe [Erstellen von Imagemaps](creating-image-maps.md).

Siehe Schulungsvideo [Bild- und Rotationssets: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) .

Beim Erstellen eines Rotationssets empfiehlt Adobe die folgende Best Practice und setzt die folgenden Einschränkungen voraus:

| Rotationsset-Begrenzungstyp | Optimale Vorgehensweise | Erzwungene Beschränkung |
| --- | --- | --- |
| Maximale Anzahl von Zeilen/Spalten pro 2D-Satz | 12-18 Bilder pro Set | 1000 |

Siehe auch [Dynamic Media-Einschränkungen](/help/using/limitations.md).

Diese Kurzanleitung für Rotationssets soll Sie in Adobe Dynamic Media Classic schnell mit den Rotationssets-Techniken vertraut machen. Führen Sie die Schritte 1 bis 7 aus. Am Ende jedes Schritts können Sie einen Themenlink auswählen, um mehr zu erfahren.

## 1. Erstellen und Hochladen der Bilder

Sie benötigen mindestens 8 bis 12 Aufnahmen eines Objekts für eindimensionale und 16 bis 24 Aufnahmen für zweidimensionale Rotationssets. Die Aufnahmen müssen in regelmäßigen Abständen gemacht werden, um den Eindruck von Rotation und Spiegelung zu erwecken. Wenn ein eindimensionales Rotationsset beispielsweise 12 Aufnahmen enthält, drehen Sie das Element für jeden Schuss um 30° (360/12).

Wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Hochladen]** aus, um Rotationssets von Ihrem Computer oder Netzwerk in Adobe Dynamic Media Classic hochzuladen.

Siehe [Richtlinien für das Aufnehmen von Rotationsset-Bildern](creating-spin-set.md#guidelines-for-shooting-spin-set-images).

## 2. Erstellen eines Rotationssets

Um ein Rotationsset zu erstellen, navigieren Sie in der Symbolleiste für globale Navigation zu **[!UICONTROL Build]** > **[!UICONTROL Rotationssets]**. Wählen Sie im Dialogfeld &quot;Größe des Rotationssets&quot;die gewünschte Anzahl von Zeilen und Zellen und dann **[!UICONTROL OK]** aus. Ziehen Sie dann die Bilder in das Raster auf der Seite Rotationsset .

Siehe [Erstellen eines Rotationssets](creating-spin-set.md#creating-a-spin-set).

## 3. Bearbeiten von Rotationssets

Um ein Rotationsset zu bearbeiten, navigieren Sie in der Leiste &quot;Globale Navigation&quot;zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Viewer-Vorgaben]**. Wählen Sie ein Rotationsset und dann **[!UICONTROL Bearbeiten]** aus. Fügen Sie Bilder hinzu, löschen Sie sie und ändern Sie ihre Position. Sie können die Position der Zeilen in zweidimensionalen Rotationssets ändern.

Siehe [Bearbeiten eines Rotationssets](creating-spin-set.md#editing-a-spin-set).

## 4. Einrichten von Rotationsset-Viewer-Vorgaben

Administratoren können Rotationsset-Viewer-Vorgaben erstellen. Mit einer solchen Vorgabe wird das Aussehen eines Rotationsset-Viewers festgelegt. Um eine neue Rotationsset-Viewer-Vorgabe einzurichten, gehen Sie in der Symbolleiste für globale Navigation zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Viewer-Vorgaben]**.

Wählen Sie auf der Seite &quot;Viewer-Vorgaben&quot;die Option **[!UICONTROL Hinzufügen]**, wählen Sie dann **[!UICONTROL Rotationsset-Viewer]** aus der Dropdownliste und klicken Sie dann auf **[!UICONTROL Hinzufügen]**. Wählen Sie Optionen auf der Seite `Configure Viewer` und dann **[!UICONTROL Speichern]** aus.

Siehe [Einrichten von Rotationsset-Viewer-Vorgaben](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## 5. Vorschau eines Rotationssets

Wählen Sie das Rotationsset im Bedienfeld &quot;Durchsuchen&quot;aus und wählen Sie dann **[!UICONTROL Vorschau]** aus. Halten Sie auf der Seite Vorschau die Maustaste gedrückt und ziehen Sie den Zeiger nach links oder rechts, um das Element visuell zu &quot;drehen&quot;.

Siehe [Vorschau eines Rotationssets anzeigen](previewing-spin-set.md#previewing-a-spin-set).

## 6. Publish-Rotationsset

Beim Veröffentlichen eines Rotationssets wird es auf Adobe Dynamic Media Classic-Servern platziert, damit es dynamisch auf Ihrer Website oder in Ihrer Anwendung bereitgestellt werden kann. Außerdem wird die URL-Zeichenfolge aktiviert, die das Rotationsset von Dynamic Media-Bildservern auf Ihre Website oder Anwendung aufruft.

Um ein Rotationsset zu veröffentlichen, markieren Sie es zur Veröffentlichung, indem Sie im Bedienfeld &quot;Durchsuchen&quot;das Symbol &quot;**[!UICONTROL Für Publish markieren]**&quot;neben seinem Namen auswählen. Wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Publish]** aus, um eine Veröffentlichung zu starten. Wählen Sie auf der Seite &quot;Publishing&quot;die Option **[!UICONTROL Publish übermitteln]**.

Siehe [Publish eines Rotationssets](publishing-spin-set.md#publishing-a-spin-set).

## 7. Verknüpfen eines Rotationssets mit einer Webseite

Adobe Dynamic Media Classic erstellt URL-Callout-Zeichenfolgen für Rotationssets und aktiviert sie nach der Veröffentlichung. Sie können diese URLs von der Seite &quot;Vorschau&quot;kopieren.

Wählen Sie das Rotationsset und dann **[!UICONTROL Vorschau]** aus. Wählen Sie eine Rotationsset-Viewer-Vorgabe aus. Wählen Sie dann **[!UICONTROL URL kopieren]** aus.

Siehe [Verknüpfen eines Rotationssets mit einer Webseite](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
