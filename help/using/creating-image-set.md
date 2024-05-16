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
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 46%

---

# Erstellen eines Bildsatzes{#creating-an-image-set}

Um einen Bildsatz mit mehreren Ansichten zu erstellen, benötigen Sie Bilder, die ein Element aus unterschiedlichen Perspektiven zeigen oder verschiedene Aspekte eines Elements darstellen. Das Ziel dabei ist, dem Betrachter Bilder eines Elements zu präsentieren, damit er eine umfassende Vorstellung davon erhält, wie es aussieht und was es leistet.

## Erstellen eines Bildsatzes {#create}

Wenn Sie ein Set erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| **[!UICONTROL `Publish after save`]** vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

Beim Erstellen eines Bildsets empfiehlt Adobe die folgenden Best Practices und setzt die folgenden Einschränkungen voraus:

| Begrenzungstyp | Optimale Vorgehensweise | Erzwungene Beschränkung |
| --- | --- | --- |
| Anzahl der doppelten Assets pro Satz | Keine Duplikate | 20 ‡ |
| Maximale Anzahl an Bildern pro Set | 5 - 10 Bilder pro Set | 1000 |

‡ Best Practice ist, keine doppelten Assets in einem Satz zu haben. Die Beschränkung beträgt 20 Duplikate für ein einzelnes Asset. Wenn Sie innerhalb des Sets ein weiteres Duplikat für dieses Asset hinzufügen, gibt die Anforderung entweder einen Fehler aus oder ignoriert das Duplikat.

Siehe auch [Einschränkungen bei Dynamic Media](/help/using/limitations.md).

**So erstellen Sie ein Bildset:**

1. Führen Sie einen der folgenden Schritte aus:

   * **Auswählen der Bilder zuerst**: Wählen Sie im Durchsuchenbedienfeld die Bilder aus, die Sie für das Bildset verwenden möchten, und navigieren Sie zu **[!UICONTROL Build]** > **[!UICONTROL Bildsets]**.

   * **Starten Sie über den Bildschirm &quot;Bildset&quot;**: Gehen Sie zu **[!UICONTROL Build]** > **[!UICONTROL Bildsets]**. Der Anzeigebereich „Bildsatz“ wird geöffnet. Wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die Bilder, die Sie für den Bildsatz verwenden möchten, in den Anzeigebereich „Bildsatz“.

1. Um die Reihenfolge der Bilder zu ändern, ziehen Sie die Bilder an die gewünschten Positionen.
1. Stellen Sie sicher, dass rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Auswählen **[!UICONTROL Speichern]**, wählen Sie einen Ordner zum Speichern des Bildsets aus, geben Sie einen Namen für das Set ein und wählen Sie dann **[!UICONTROL Speichern]**.
1. Um das Bildset im Bildset-Viewer anzuzeigen, wählen Sie **[!UICONTROL Vorschau]** auf dem Bildschirm &quot;Bildset&quot;angezeigt. Sie können Musterminiaturansichten im Bildset-Viewer auswählen, um zu sehen, wie sie sich verhalten.

## Bearbeiten eines Bildsatzes {#editing-an-image-set}

Unabhängig davon, ob Sie ein veröffentlichtes oder unveröffentlichtes Set bearbeiten, wird die **[!UICONTROL Nach dem Speichern veröffentlichen]** -Option wirkt sich auf die Set- und Set-Mitglieder wie folgt aus:

| Set bereits veröffentlicht? | **[!UICONTROL `Publish after save`]** vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren Veröffentlichungsstatus bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie ein Bildset:**

1. Navigieren Sie in der Rasteransicht zu einem Bildset und wählen Sie unter dem Bild die Option **[!UICONTROL Bearbeiten]**.
1. Führen Sie einen der folgenden Schritte aus:

   * Um ein Bild hinzuzufügen (veröffentlicht oder unveröffentlicht), ziehen Sie es aus einem Ordner in &quot;Assets hinzufügen&quot;auf die Bildset-Liste **[!UICONTROL Ansichten]** Seite.
   * Um ein Bild zu entfernen, wählen Sie es aus und klicken Sie auf **[!UICONTROL Löschen]** in der Symbolleiste.
   * Um die Bilder neu anzuordnen, ziehen Sie ein Bild in eine neue Position.

1. Wenn Sie die Bearbeitung des Sets abgeschlossen haben, stellen Sie sicher, dass rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Auswählen **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner für das Set aus, geben Sie einen Namen für das Set ein und wählen Sie dann **[!UICONTROL Speichern]**.

## Löschen eines Bildsets

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (oder &quot;untergeordneten Elemente&quot;) in diesem Satz sind jedoch nicht betroffen. Stattdessen behalten sie ihren vorhandenen Status veröffentlicht oder unveröffentlicht bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie ein Bildset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Bildsets aus.
1. Wechseln Sie in der Leiste Globale Navigation zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.
