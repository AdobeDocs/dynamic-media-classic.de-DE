---
title: '"Kurzanleitung: Rotationssets"'
description: Eine Einführung in Adobe Dynamic Media Classic und ein Schnellstart zu Rotationssets, die Ihnen den schnellen Einstieg in Classic erleichtern.
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
source-git-commit: 36f9aa3c2b4dc66e4cb851c2ce6837ae0ad4f64c
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 25%

---

# Kurzanleitung: Rotationssets{#quick-start-spin-sets}

Mit einem Rotationsset wird simuliert, wie man ein reales Objekt dreht, um es von allen Seiten betrachten zu können. Rotationssets ermöglichen die Anzeige von Objekten aus einem beliebigen Blickwinkel, um seine wichtigsten visuellen Eigenschaften zu erfassen. Ein Rotationsset simuliert eine 360°-Anzeige. Adobe Dynamic Media Classic bietet eindimensionale Rotationssets, in denen die Betrachter ein Element drehen können, und zweidimensionale Rotationssets, in denen die Betrachter das Element drehen und spiegeln können. Darüber hinaus können Benutzer mit wenigen einfachen Mausklicks beliebige Ansichten &quot;frei&quot;zoomen und schwenken. Auf diese Weise können Benutzer ein Objekt näher und aus einer bestimmten Perspektive betrachten.

![Bilder für ein Rotationsset.](/help/assets/spin_set.png)

Rotationssets akzeptieren auch Imagemaps. Eine Imagemap ist ein Bereich auf einem Bild in einem Rotationsset, mit dessen Hilfe ein Rollover-Bedienfeld mit Text angezeigt werden kann. Wenn der Benutzer auf eine Imagemap klickt, wird eine bestimmte Aktion ausgelöst. Beispielsweise kann eine Website aufgerufen werden, auf der der Benutzer mehr über ein Produkt erfährt. Um auf eine Imagemap in einem Rotationsset zu verweisen, wird um die Imagemap selbst herum ein Umriss angezeigt, wenn der Benutzer den Mauszeiger darüber bewegt.

Siehe [Erstellen von Imagemaps](creating-image-maps.md).

Diese Kurzanleitung für Rotationssets wurde entwickelt, um mit den Rotationssets-Techniken in Adobe Dynamic Media Classic schnell vertraut zu machen. Führen Sie die Schritte 1 bis 7 aus. Am Ende jedes Schritts können Sie einen Themenlink auswählen, um mehr zu erfahren.

## 1. Erstellen und Hochladen der Bilder

Sie benötigen mindestens 8 bis 12 Aufnahmen eines Elements für ein eindimensionales Rotationsset und 16 bis 24 Aufnahmen für ein zweidimensionales Rotationsset. Die Aufnahmen müssen in regelmäßigen Abständen gemacht werden, um den Eindruck von Rotation und Spiegelung zu erwecken. Wenn ein eindimensionales Rotationsset beispielsweise 12 Aufnahmen enthält, drehen Sie das Element für jeden Schuss um 30° (360°/12).

Wählen Sie in der Symbolleiste für globale Navigation **[!UICONTROL Upload]** aus, um Rotationssets von Ihrem Computer oder Netzwerk in Adobe Dynamic Media Classic hochzuladen.

Siehe [Richtlinien für das Aufnehmen von Rotationsset-Bildern](creating-spin-set.md#guidelines-for-shooting-spin-set-images).

## 2. Erstellen eines Rotationssets

Um ein Rotationsset zu erstellen, navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Build]** > **[!UICONTROL Rotationssets]**. Wählen Sie im Dialogfeld &quot;Größe des Rotationssets&quot;die gewünschte Anzahl von Zeilen und Zellen und klicken Sie auf **[!UICONTROL OK]**. Ziehen Sie dann Bilder in das Raster auf der Seite Rotationsset .

Siehe [Erstellen eines Rotationssets](creating-spin-set.md#creating-a-spin-set).

## 3. Bearbeiten von Rotationssets

Um ein Rotationsset zu bearbeiten, navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Setup]** > **[!UICONTROL Viewer-Vorgaben]**. Wählen Sie ein Rotationsset und dann **[!UICONTROL Bearbeiten]** aus. Fügen Sie Bilder hinzu, löschen Sie sie und ändern Sie ihre Position. Sie können die Position der Zeilen in zweidimensionalen Rotationssets ändern. 

Siehe [Rotationsset bearbeiten](creating-spin-set.md#editing-a-spin-set).

## 4. Einrichten von Rotationsset-Viewer-Vorgaben

Administratoren können Rotationsset-Viewer-Vorgaben erstellen. Mit einer solchen Vorgabe wird das Aussehen eines Rotationsset-Viewers festgelegt. Um eine neue Rotationsset-Viewer-Vorgabe einzurichten, gehen Sie in der globalen Navigationsleiste zu **[!UICONTROL Setup]** > **[!UICONTROL Viewer-Vorgaben]**.

Wählen Sie auf der Seite &quot;Viewer-Vorgaben&quot;die Option **[!UICONTROL Hinzufügen]**, wählen Sie dann **[!UICONTROL Rotationsset-Viewer]** aus der Dropdown-Liste und klicken Sie dann auf **[!UICONTROL Hinzufügen]**. Wählen Sie auf der Seite &quot;Viewer konfigurieren&quot;Optionen aus und klicken Sie auf **[!UICONTROL Speichern]**.

Siehe [Einrichten von Rotationsset-Viewer-Vorgaben](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## 5. Vorschau eines Rotationssets

Wählen Sie das Rotationsset im Durchsuchenbedienfeld aus und klicken Sie dann auf **[!UICONTROL Vorschau]**. Halten Sie auf der Seite Vorschau die Maustaste gedrückt und ziehen Sie den Zeiger nach links oder rechts, um das Element visuell zu &quot;drehen&quot;.

Siehe [Vorschau eines Rotationssets](previewing-spin-set.md#previewing-a-spin-set).

## 6. Veröffentlichen eines Rotationssets

Beim Veröffentlichen eines Rotationssets wird es auf Adobe Dynamic Media Classic-Servern platziert, damit es dynamisch für Ihre Website oder Anwendung bereitgestellt werden kann. Außerdem wird die URL-Zeichenfolge aktiviert, mit der das Rotationsset von den Dynamic Media-Bildservern auf Ihre Website oder Anwendung aufgerufen wird.

Um ein Rotationsset zu veröffentlichen, markieren Sie es zur Veröffentlichung, indem Sie im Durchsuchenbedienfeld das Symbol **[!UICONTROL Zur Veröffentlichung markieren]** neben dem Namen auswählen. Wählen Sie in der Symbolleiste für globale Navigation **[!UICONTROL Veröffentlichen]** aus, um eine Veröffentlichung zu starten. Wählen Sie im Bildschirm &quot;Veröffentlichen&quot;die Option **[!UICONTROL Veröffentlichen senden]**.

Siehe [Veröffentlichen eines Rotationssets](publishing-spin-set.md#publishing-a-spin-set).

## 7. Verknüpfen eines Rotationssets mit einer Webseite

Adobe Dynamic Media Classic erstellt URL-Hinweisszeichenfolgen für Rotationssets und aktiviert sie nach der Veröffentlichung. Sie können diese URLs von der Seite &quot;Vorschau&quot;kopieren.

Wählen Sie das Rotationsset aus und klicken Sie dann auf **[!UICONTROL Vorschau]**. Wählen Sie eine Rotationsset-Viewer-Vorgabe aus. Wählen Sie dann **[!UICONTROL URL kopieren]** aus.

Siehe [Verknüpfen eines Rotationssets mit einer Webseite](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
