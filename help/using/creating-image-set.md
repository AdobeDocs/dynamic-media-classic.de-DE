---
title: Erstellen eines Bildsatzes
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic ein Bildset erstellen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 38%

---

# Erstellen eines Bildsatzes{#creating-an-image-set}

Um einen Bildsatz mit mehreren Ansichten zu erstellen, benötigen Sie Bilder, die ein Element aus unterschiedlichen Perspektiven zeigen oder verschiedene Aspekte eines Elements darstellen. Das Ziel dabei ist, dem Betrachter Bilder eines Elements zu präsentieren, damit er eine umfassende Vorstellung davon erhält, wie es aussieht und was es leistet.

## Erstellen eines Bildsatzes {#create}

Wenn Sie einen Satz erstellen, wirkt sich die Option **[!UICONTROL Publish nach dem Speichern]** auf die Mitglieder des Satzes und des Satzes wie folgt aus:

| **[!UICONTROL `Publish after a save`]** Option vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

Beim Erstellen eines Bildsets empfiehlt Adobe die folgenden Best Practices und erzwingt die folgenden Beschränkungen:

| Art des Limits | Optimale Vorgehensweise | Limit |
| --- | --- | --- |
| Anzahl der doppelten Assets pro Set | Keine Duplikate | 20 ‡ |
| Maximale Anzahl von Bildern pro Set | 5-10 Bilder pro Set | 1000 |

‡ Best Practice ist es, keine doppelten Assets in einem Satz zu haben. Für ein einzelnes Asset sind maximal 20 Duplikate zulässig. Wenn Sie innerhalb des Sets ein weiteres Duplikat für dieses Asset hinzufügen, gibt die Anfrage entweder einen Fehler aus oder ignoriert das Duplikat.

Siehe auch [Einschränkungen bei Dynamic Media](/help/using/limitations.md).

**So erstellen Sie ein Bildset:**

1. Führen Sie einen der folgenden Schritte aus:

   * **Zuerst die Bilder auswählen**: Wählen Sie im Durchsuchen-Panel die Bilder aus, die Sie für Ihr Bildset benötigen, und navigieren Sie zu **[!UICONTROL Erstellen]** > **[!UICONTROL Bildsets]**.

   * **Im Bildschirm für Bildsets starten**: Gehen Sie zu **[!UICONTROL Erstellen]** > **[!UICONTROL Bildsets]**. Der Anzeigebereich „Bildsatz“ wird geöffnet. Wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die Bilder, die Sie für den Bildsatz verwenden möchten, in den Anzeigebereich „Bildsatz“.

1. Um die Reihenfolge der Bilder zu ändern, ziehen Sie die Bilder an die gewünschten Positionen.
1. Stellen Sie sicher, dass **[!UICONTROL Publish nach dem Speichern in der rechten unteren Ecke]** Standard) ausgewählt ist.
1. Klicken Sie **[!UICONTROL Speichern]**, wählen Sie einen Ordner zum Speichern des Bildsets aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **[!UICONTROL Speichern]**.
1. Um das Bildset im Bildset-Viewer anzuzeigen, wählen Sie **[!UICONTROL Bildschirm Bildset]** Vorschau“ aus. Sie können im Bildset-Viewer Miniaturansichten auswählen, um ihr Verhalten zu überprüfen.

## Bearbeiten eines Bildsatzes {#editing-an-image-set}

Unabhängig davon, ob Sie ein veröffentlichtes oder ein unveröffentlichtes Set bearbeiten, wirkt sich die Option **[!UICONTROL Publish nach einem Speichern]** auf die Mitglieder des Sets und des Sets wie folgt aus:

| Set bereits veröffentlicht? | **[!UICONTROL `Publish after a save`]** Option vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren veröffentlichten Status bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie ein Bildset:**

1. Navigieren Sie in der Rasteransicht zu einem ImageSet und wählen Sie dann unter dem Bild **[!UICONTROL Bearbeiten]** aus.
1. Führen Sie einen der folgenden Schritte aus:

   * Um ein Bild (veröffentlicht oder unveröffentlicht) hinzuzufügen, ziehen Sie es aus einem Ordner in Assets hinzufügen auf die Seite **[!UICONTROL Ansichten]** des Bildsets.
   * Um ein Bild zu entfernen, wählen Sie es aus und klicken Sie in der Symbolleiste **[!UICONTROL Löschen]**.
   * Um die Bilder neu anzuordnen, ziehen Sie ein Bild in eine neue Position.

1. Wenn Sie die Bearbeitung des Sets abgeschlossen haben, stellen Sie sicher, dass **[!UICONTROL Publish nach dem Speichern]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner für Ihr Set aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **[!UICONTROL Speichern]**.

## Löschen von Bildsets

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (oder „untergeordneten Elemente„) in diesem Set sind jedoch nicht betroffen. Stattdessen behalten sie jeweils ihren vorhandenen Status „Veröffentlicht“ oder „Unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie ein Bildset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht mindestens ein Bildset aus.
1. Navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.
