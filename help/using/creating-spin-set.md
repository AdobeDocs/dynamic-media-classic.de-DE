---
title: Erstellen eines Rotationssets
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic ein Rotationsset erstellen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 32%

---

# Erstellen eines Rotationssets{#creating-a-spin-set}

Um ein effektives Rotationsset erstellen zu können, müssen Sie darauf achten, die Bilder korrekt aufzunehmen. Sie können ein Rotationsset in Adobe Dynamic Media Classic erstellen, indem Sie auf die Schaltfläche Erstellen klicken und Rotationssets auswählen. Im Anzeigebereich „Rotationsset“ können Sie Rotationssets bearbeiten.

>[!NOTE]
>
>In früheren Versionen von Adobe Dynamic Media Classic gab es keine zweidimensionalen Rotationssets. Wenn Sie ein Rotationsset in einer früheren Version von Adobe Dynamic Media Classic erstellt und unter einem anderen Namen gespeichert haben, können Sie Ihr eindimensionales Rotationsset speichern. Wählen **[!UICONTROL im Bildschirm „Rotationsset]** die Option „Speichern unter“ aus und geben Sie einen neuen Namen ein, damit Sie ihn in Adobe Dynamic Media Classic bearbeiten können.

## Richtlinien für das Aufnehmen von Rotationsset-Bildern {#guidelines-for-shooting-spin-set-images}

Im Allgemeinen gilt: Je mehr Bilder Sie in einem Rotationsset haben, desto besser ist der Effekt des Bilddrehens. Eine höhere Anzahl von Rotationsset-Bildern bringt jedoch auch eine längere Ladezeit für die Bilder mit sich. Adobe Dynamic Media Classic empfiehlt die folgenden Richtlinien für die Aufnahme von Bildern zur Verwendung in Rotationssets:

* Verwenden Sie mindestens 8 bis 12 Bilder in einem eindimensionalen Rotationsset und 16 bis 24 Bilder in einem zweidimensionalen Rotationsset.
* Verwenden Sie ein verlustfreies Format. Zu empfehlen sind die Formate TIFF und PNG.
* Maskieren Sie alle Bilder, so dass das Objekt vor einem reinweißen oder anderen kontrastreichen Hintergrund erscheint. Fügen Sie nach Wunsch Schatten hinzu.
* Vergewissern Sie sich, dass die Produktdetails gut ausgeleuchtet und fokussiert sind.
* Nehmen Sie Bilder für Modekleidung mit einer Gliederpuppe oder einem Model auf. Oft wird die Schaufensterpuppe entweder maskiert (mit einer Schaufensterpuppe aus Glas) oder es wird eine stilisierte Schaufensterpuppe im Bild gezeigt. Sie können ein Modell-Rotationsset erstellen, indem Sie die Anzahl der Winkel definieren. Markieren Sie jeden Winkel mit Klebeband auf dem Boden, damit Sie das Modell zum Schritt führen und in die Richtung jeder Aufnahme schauen können.

## Erstellen eines Rotationssets {#create}

Die Reihenfolge, in der das Rotationsset in Adobe Dynamic Media Classic erstellt oder verfasst wird, ist wichtig. Je nachdem, wie Sie die Assets anordnen, wenn Sie Bilder per Drag-and-Drop in das Raster auf der Seite mit dem Rotationsset ziehen, dreht sich das Rotationsset in eine bestimmte Richtung. Daher wird das Asset in der Reihenfolge, in der es im Builder visuell angezeigt wird, so gedreht, wie es gedreht wird, wenn ein Benutzer den Mauszeiger oder seinen Finger von links nach rechts bewegt.

Wenn Sie einen Satz erstellen, wirkt sich die Option **[!UICONTROL Publish nach dem Speichern]** auf die Mitglieder des Satzes und des Satzes wie folgt aus:

| **[!UICONTROL Publish nach einem Speichern]** vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

Beim Erstellen eines Rotationssets empfiehlt Adobe die folgende Best Practice und erzwingt die folgende Beschränkung:

| Art des Rotationssets-Limits | Optimale Vorgehensweise | Limit |
| --- | --- | --- |
| Maximale Anzahl von Zeilen/Spalten pro 2D-Set | 12-18 Bilder pro Set | 1000 |

Siehe auch [Einschränkungen bei Dynamic Media](/help/using/limitations.md).

Nach dem Speichern eines Rotationssets können Sie seine Anzeige im Standard-Viewer mithilfe der Vorschau auf der Seite „Erstellen: Rotationsset“ testen.

**So erstellen Sie ein Rotationsset:**

1. Wählen **[!UICONTROL im Dropdown]** Menü „Erstellen“ die Option **[!UICONTROL Rotationssets]**.
1. Legen Sie im Dialogfeld „Größe des Rotationssets“ die gewünschte Anzahl an Zeilen und Zellen fest.

   Um ein eindimensionales Rotationsset zu erstellen, wählen Sie nur eine Zeile aus.

   Wählen Sie für ein zweidimensionales Rotationsset zwei oder mehr Zeilen.

1. Klicken Sie **[!UICONTROL OK]**.
1. Ziehen Sie Bilder auf das Raster im Anzeigebereich „Rotationsset“.
1. Wenn Sie fertig sind, stellen Sie sicher, dass **Publish nach dem Speichern** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]** aus.
1. Wählen Sie im Dialogfeld Speichern einen Ordner zum Speichern des Rotationssets aus. Geben Sie im Feld Dateiname den Namen des Rotationssets ein.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

## Bearbeiten eines Rotationssets {#editing-a-spin-set}

Unabhängig davon, ob Sie ein veröffentlichtes Set oder ein unveröffentlichtes Set bearbeiten, wirkt sich die Option **[!UICONTROL Publish nach dem Speichern]** auf die Mitglieder des Sets und des Sets wie folgt aus:

| Set bereits veröffentlicht? | **[!UICONTROL Publish nach einer Speicherung]** Option vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren veröffentlichten Status bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

**So bearbeiten Sie ein Rotationsset:**

1. Wählen Sie die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** des Rotationssets aus.
1. Führen Sie einen der folgenden Schritte aus:

   * **Entfernen von Bildern**: Wählen Sie das Bild aus und klicken Sie dann auf **[!UICONTROL Löschen]**.

   * **Bilder hinzufügen**: Ziehen Sie das Bild in eine Zelle.

   * **Zeilen neu anordnen (zweidimensionale Rotationssets)**: Wählen Sie ein Zeilenauswahlfeld (links neben der Zeile) aus und klicken Sie dann auf **[!UICONTROL Zeile nach unten]** oder **[!UICONTROL Zeile nach oben]**.

   * **Zeilen und Zellen hinzufügen**: Geben Sie eine Zahl in die Felder „Zeilen“ und „Zellen“ ein, um die Anzahl der Zeilen und die Anzahl der Zellen in jeder Zeile zu bestimmen.

1. Wenn Sie die Bearbeitung abgeschlossen haben, stellen Sie sicher, dass **[!UICONTROL Publish nach dem Speichern]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **[!UICONTROL Speichern]**.

## Löschen eines Rotationssets

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (oder „untergeordneten Elemente„) in diesem Set sind jedoch nicht betroffen. Stattdessen behalten sie jeweils ihren vorhandenen Status „Veröffentlicht“ oder „Unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

**So löschen Sie ein Rotationsset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Rotationssets aus.
1. Navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.
