---
title: Erstellen eines Bildsatzes
description: Erfahren Sie, wie Sie ein Bildset in Adobe Dynamic Media Classic erstellen.
uuid: 689fdc14-4f51-4c94-8515-cd8551e101d8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 3f356410-b30e-4870-ad95-6e5a9dc126c8
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
source-git-commit: fe765d1acfa37e9d13f5ef1b655f8cf04195a8a6
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 59%

---

# Erstellen eines Bildsatzes{#creating-an-image-set}

Um einen Bildsatz mit mehreren Ansichten zu erstellen, benötigen Sie Bilder, die ein Element aus unterschiedlichen Perspektiven zeigen oder verschiedene Aspekte eines Elements darstellen. Das Ziel dabei ist, dem Betrachter Bilder eines Elements zu präsentieren, damit er eine umfassende Vorstellung davon erhält, wie es aussieht und was es leistet.

## Erstellen eines Bildsatzes {#create}

Wenn Sie ein Set erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| **[!UICONTROL Nach dem Speichern veröffentlichen]** vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

>[!NOTE]
>
>Beim Erstellen eines Bildsets empfiehlt Adobe die folgenden Best Practice-Richtlinien und erzwungenen Einschränkungen.
>
>* Anzahl der doppelten Assets pro Bildset
   >   * Best Practice: 20
   >   * Erzwungene Beschränkung: 20
> * Maximale Seitenzahl pro Bildset
   >   * Best Practice: 1000
   >   * Ausgedrückt Grenze: 1000


**So erstellen Sie einen Bildsatz:**

1. Führen Sie einen der folgenden Schritte aus:

   * **Wählen Sie zuerst die Bilder aus** - Wählen Sie im Durchsuchen-Bedienfeld die Bilder aus, die Sie für das Bildset verwenden möchten, und navigieren Sie zu **[!UICONTROL Build]** > **[!UICONTROL Bildsets]**.

   * **Starten Sie im Bildschirm &quot;Bildset&quot;** - Gehen Sie zu **[!UICONTROL Build]** > **[!UICONTROL Bildsets]**. Der Anzeigebereich „Bildsatz“ wird geöffnet. Wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die Bilder, die Sie für den Bildsatz verwenden möchten, in den Anzeigebereich „Bildsatz“.

1. Um die Reihenfolge der Bilder zu ändern, ziehen Sie die Bilder an die gewünschten Positionen.
1. Stellen Sie sicher, dass rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Auswählen **[!UICONTROL Speichern]**, wählen Sie einen Ordner zum Speichern des Bildsets aus, geben Sie einen Namen für das Set ein und wählen Sie dann **[!UICONTROL Speichern]**.
1. Um das Bildset im Bildset-Viewer anzuzeigen, wählen Sie **[!UICONTROL Vorschau]** auf dem Bildschirm &quot;Bildset&quot;angezeigt. Sie können Musterminiaturansichten im Bildset-Viewer auswählen, um zu sehen, wie sie sich verhalten.

## Bearbeiten eines Bildsatzes {#editing-an-image-set}

Unabhängig davon, ob Sie ein veröffentlichtes oder unveröffentlichtes Set bearbeiten, wird die **[!UICONTROL Nach dem Speichern veröffentlichen]** -Option wirkt sich auf die Set- und Set-Mitglieder wie folgt aus:

| Set bereits veröffentlicht? | **[!UICONTROL Nach dem Speichern veröffentlichen]** vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten den Status „veröffentlicht“ bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie einen Bildsatz:**

1. Navigieren Sie in der Rasteransicht zu einem Bildset und wählen Sie unter dem Bild die Option **[!UICONTROL Bearbeiten]**.
1. Führen Sie einen der folgenden Schritte aus:

   * Um ein Bild hinzuzufügen (veröffentlicht oder unveröffentlicht), ziehen Sie es aus einem Ordner in „Assets hinzufügen“ auf die Seite **[!UICONTROL Ansichten]** des Bildsatzes.
   * Um ein Bild zu entfernen, wählen Sie es aus und klicken Sie auf **[!UICONTROL Löschen]** in der Symbolleiste.
   * Um die Bilder neu anzuordnen, ziehen Sie ein Bild in eine neue Position.

1. Wenn Sie die Bearbeitung des Sets abgeschlossen haben, stellen Sie sicher, dass rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Auswählen **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner für das Set aus, geben Sie einen Namen für das Set ein und wählen Sie dann **[!UICONTROL Speichern]**.

## Löschen eines Bildsets {#deleting-an-image-set}

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (bzw. die untergeordneten Elemente) innerhalb des Sets sind davon jedoch nicht betroffen; sie behalten ihren jeweiligen Status „veröffentlicht“ oder „unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie einen Bildsatz:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Bildsets aus.
1. Wechseln Sie in der Leiste &quot;Globale Navigation&quot;zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.
