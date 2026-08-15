---
title: 'Kurzanleitung: Rotationssets'
description: Eine Einführung und ein Schnellstart-Rotationsset, mit dem Sie in Adobe Dynamic Media Classic schnell loslegen können.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
topic: Content Management
level: Beginner
autotag-review: '2026-05-13T20:10:31.990Z'
TQID: 'https://experienceleague.adobe.com/dYjjsyvPAPOS5icw4Yi6Kpo93Nh2qvnCiW5-ih2hmDk'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 1c15d2395e62ce41a298d25b973920963eef3a7a
workflow-type: tm+mt
source-wordcount: 820
ht-degree: 11%

---

# Kurzanleitung: Rotationssets{#quick-start-spin-sets}

Ein Rotationsset bietet eine 360-Grad-Ansicht eines Objekts. Rotationssets ermöglichen es, Elemente aus jedem Blickwinkel anzuzeigen und visuelle Details aus jeder Perspektive zu erhalten. Ein Rotationsset simuliert eine 360°-Rundumansicht des Objekts. Adobe Dynamic Media Classic bietet eindimensionale Rotationssets, in denen Betrachter ein Element drehen können, und zweidimensionale Rotationssets, in denen Betrachter das Element drehen und spiegeln können. Darüber hinaus können Benutzer alle Ansichten zoomen und schwenken. Benutzer können ein Element genauer aus einem bestimmten Blickwinkel betrachten.

![Bilder für ein Rotationsset](/help/using/assets/spin_set.png)

Rotationssets akzeptieren auch Imagemaps. Eine Imagemap ist ein Bereich auf einem Bild innerhalb des Rotationssets, der ein Rollover-Bedienfeld mit Text anzeigt. Wenn der Benutzer eine Imagemap auswählt, wird eine Aktion ausgelöst. Beispielsweise kann eine Website aufgerufen werden, auf der der Benutzer mehr über ein Produkt erfährt. Um eine Imagemap in einem Rotationsset anzugeben, wird ein Umriss um die Imagemap selbst angezeigt, wenn der Benutzer den Mauszeiger darüber bewegt.

Siehe [Erstellen von Imagemaps](creating-image-maps.md).

Siehe [Bild- und Rotationssets: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/556_Image%20&%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) Schulungsvideo.

Beim Erstellen eines Rotationssets empfiehlt Adobe die folgenden Richtlinien und erzwingt die folgenden Beschränkungen:

| Art des Rotationssets-Limits | Optimale Vorgehensweise | Limit |
| --- | --- | --- |
| Maximale Anzahl von Zeilen/Spalten pro 2D-Set | 12-18 Bilder pro Set | 1000 |

Siehe auch [Grenzwerte für Dynamic Media](/help/using/limitations.md).

Dieses Handbuch soll Ihnen dabei helfen, schnell mit der Verwendung von Rotationssettechniken in Adobe Dynamic Media Classic zu beginnen. Führen Sie die Schritte 1 bis 7 aus. Am Ende jedes Schritts können Sie einen Themen-Link auswählen, um mehr zu erfahren.

## &#x200B;1. Erstellen und Hochladen der Bilder

Sie benötigen mindestens 8-12 Aufnahmen eines Artikels für ein eindimensionales Rotationsset und 16-24 Aufnahmen für ein zweidimensionales Rotationsset. Die Aufnahmen müssen in regelmäßigen Abständen gemacht werden, um zu zeigen, dass sich der Gegenstand dreht und gedreht wird. Wenn beispielsweise ein eindimensionales Rotationsset 12 Aufnahmen enthält, drehen Sie den Artikel für jede Aufnahme um 30 Grad (360/12).

Wählen Sie in der globalen Navigationsleiste **[!UICONTROL Hochladen]** aus, um Rotationssymbole von Ihrem Computer oder Netzwerk in Adobe Dynamic Media Classic hochzuladen.

Siehe [Richtlinien für das Aufnehmen von Rotationsset-Bildern](creating-spin-set.md#guidelines-for-shooting-spin-set-images).

## &#x200B;2. Erstellen eines Rotationssets

Zum Erstellen eines Rotationssets navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Erstellen]** > **[!UICONTROL Rotationssets]**. Wählen Sie im Dialogfeld Größe des Rotationssets aus, wie viele Zeilen und Zellen Sie benötigen, und klicken Sie auf **[!UICONTROL OK]**. Ziehen Sie dann die Bilder in das Raster auf der Seite „Rotationsset“.

Siehe [Erstellen eines Rotationssets](creating-spin-set.md#creating-a-spin-set).

## &#x200B;3. Bearbeiten eines Rotationssets

Zum Bearbeiten eines Rotationssets navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Einstellungen]** > **[!UICONTROL Viewer-Vorgaben]**. Wählen Sie ein Rotationsset und dann **[!UICONTROL Bearbeiten]** aus. Fügen Sie Bilder hinzu, löschen Sie sie und ändern Sie ihre Position. Sie können die Position von Zeilen in zweidimensionalen Rotationssets ändern.

Siehe [Bearbeiten eines Rotationssets](creating-spin-set.md#editing-a-spin-set).

## &#x200B;4. Einrichten von Viewer-Vorgaben für Rotationssets

Administratoren können Rotationsset-Viewer-Vorgaben erstellen. Mit einer solchen Vorgabe wird das Aussehen eines Rotationsset-Viewers festgelegt. Um eine neue Viewer-Vorgabe für Rotationssets einzurichten, klicken Sie in der globalen Navigationsleiste auf **[!UICONTROL Einrichtung]** > **[!UICONTROL Viewer-Vorgaben]**.

Klicken Sie auf der Seite „Viewer **[!UICONTROL Vorgaben“ auf]** Hinzufügen“ und wählen Sie dann **[!UICONTROL Rotationsset-Viewer]** aus der Dropdown-Liste aus und klicken Sie **[!UICONTROL Hinzufügen]**. Wählen Sie Optionen auf der Seite `Configure Viewer` aus und klicken Sie dann auf **[!UICONTROL Speichern]**.

Siehe [Einrichten von Viewer-Vorgaben für Rotationssets](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## &#x200B;5. Anzeigen einer Vorschau für ein Rotationsset

Wählen Sie das Rotationsset im Durchsuchen-Bedienfeld aus und klicken Sie dann auf **[!UICONTROL Vorschau]**. Halten Sie auf der Seite Vorschau die Schaltfläche gedrückt, und ziehen Sie den Mauszeiger nach links oder rechts, um das Element visuell zu drehen.

Siehe [Vorschau eines Rotationssets](previewing-spin-set.md#previewing-a-spin-set).

## &#x200B;6. Veröffentlichen eines Rotationssets

Beim Veröffentlichen eines Rotationssets wird es auf Adobe Dynamic Media Classic-Servern platziert, damit es dynamisch für Ihre Website oder Ihr Programm bereitgestellt werden kann. Außerdem wird die URL-Zeichenfolge aktiviert, die das Rotationsset von den Dynamic Media-Bildservern an Ihre Website oder Ihr Programm aufruft.

Um ein Rotationsset zu veröffentlichen, markieren Sie es zur Veröffentlichung, indem Sie im Durchsuchen **[!UICONTROL Bedienfeld das Symbol]** Zur Veröffentlichung markieren“ neben dem Namen auswählen. Klicken Sie in der globalen Navigationsleiste auf **[!UICONTROL Veröffentlichen]**, um die Veröffentlichung zu starten. Klicken Sie auf der Seite „Veröffentlichen **[!UICONTROL auf „Veröffentlichen]**.

Siehe [Veröffentlichen eines Rotationssets](publishing-spin-set.md#publishing-a-spin-set).

## &#x200B;7. Verknüpfen eines Rotationssets mit einer Web-Seite

Adobe Dynamic Media Classic erstellt URL-Legendenzeichenfolgen für Rotationssets und aktiviert diese nach deren Veröffentlichung. Sie können diese URLs von der Vorschauseite kopieren.

Wählen Sie das Rotationsset aus und klicken Sie dann auf **[!UICONTROL Vorschau]**. Wählen Sie eine Rotationsset-Viewer-Vorgabe aus. Klicken Sie dann auf **[!UICONTROL URL kopieren]**.

Siehe [Verknüpfen von Rotationssets mit Web-Seiten](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
