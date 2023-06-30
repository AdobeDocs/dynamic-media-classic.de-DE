---
title: Erstellen eines Rotationssets
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic ein Rotationsset erstellen.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 50%

---

# Erstellen eines Rotationssets{#creating-a-spin-set}

Um ein effektives Rotationsset erstellen zu können, müssen Sie darauf achten, die Bilder korrekt aufzunehmen. Sie können ein Rotationsset in Adobe Dynamic Media Classic erstellen, indem Sie auf die Schaltfläche Erstellen klicken und Rotationssets auswählen. Im Anzeigebereich „Rotationsset“ können Sie Rotationssets bearbeiten.

>[!NOTE]
>
>Frühere Versionen von Adobe Dynamic Media Classic boten keine zweidimensionalen Rotationssets an. Wenn Sie ein Rotationsset in einer früheren Version von Adobe Dynamic Media Classic erstellt haben, können Sie das eindimensionale Rotationsset nicht speichern, ohne es zuvor unter einem anderen Namen zu speichern. Auswählen **[!UICONTROL Speichern unter]** Geben Sie im Bildschirm &quot;Rotationsset&quot;einen neuen Namen ein, damit Sie ihn in Adobe Dynamic Media Classic bearbeiten können.

## Richtlinien für das Aufnehmen von Rotationsset-Bildern {#guidelines-for-shooting-spin-set-images}

Im Allgemeinen gilt: Je mehr Bilder Sie in einem Rotationsset haben, desto besser ist der Bilddreheffekt. Eine höhere Anzahl von Rotationsset-Bildern bringt jedoch auch eine längere Ladezeit für die Bilder mit sich. Adobe Dynamic Media Classic empfiehlt die folgenden Richtlinien für die Aufnahme von Bildern zur Verwendung in Rotationssets:

* Verwenden Sie mindestens 8 bis 12 Bilder in einem eindimensionalen Rotationsset und 16 bis 24 Bilder in einem zweidimensionalen Rotationsset.
* Verwenden Sie ein verlustfreies Format. Zu empfehlen sind die Formate TIFF und PNG.
* Maskieren Sie alle Bilder, so dass das Objekt vor einem reinweißen oder anderen kontrastreichen Hintergrund erscheint. Fügen Sie nach Wunsch Schatten hinzu.
* Vergewissern Sie sich, dass die Produktdetails gut ausgeleuchtet und fokussiert sind.
* Nehmen Sie Bilder für Modekleidung mit einer Gliederpuppe oder einem Model auf. Häufig ist das Mannequin entweder maskiert (mit einem Glasmannequin) oder eine stilisierte Mannequin/Dressform wird im Bild gezeigt. Sie können ein On-Modell-Rotationsset erstellen, indem Sie die Anzahl der Winkel definieren. Markieren Sie jeden Winkel mit Band auf dem Boden, damit Sie das Modell zu Schritt und Blick in die Richtung jedes Schusses führen können.

## Erstellen eines Rotationssets {#create}

Die Reihenfolge, in der das Rotationsset in Adobe Dynamic Media Classic erstellt oder erstellt wird, ist wichtig. Je nachdem, in welcher Reihenfolge Sie die Assets anordnen, wenn Sie Bilder auf einem Raster auf der Seite „Rotationsset“ ablegen, dreht sich das Rotationsset in eine bestimmte Richtung. Daher wird das Asset in der visuell angezeigten Reihenfolge angezeigt, wenn ein Benutzer seinen Mauszeiger bewegt oder seinen Finger von links nach rechts bewegt.

Wenn Sie ein Set erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| **[!UICONTROL Nach dem Speichern veröffentlichen]** vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

Beim Erstellen eines Rotationssets empfiehlt Adobe die folgenden Best Practices und erzwingt die folgende Beschränkung:

| Rotationsset-Begrenzungstyp | Optimale Vorgehensweise | Begrenzung auferlegt |
| --- | --- | --- |
| Maximale Anzahl von Zeilen/Spalten pro 2D-Satz | 12-18 Bilder pro Set | 1000 |

Siehe auch [Einschränkungen bei Dynamic Media](/help/using/limitations.md).

Nach dem Speichern eines Rotationssets können Sie seine Anzeige im Standard-Viewer mithilfe der Vorschau auf der Seite „Erstellen: Rotationsset“ testen.

**So erstellen Sie ein Rotationsset:**

1. Im **[!UICONTROL Build]** Dropdown-Menü auswählen **[!UICONTROL Rotationssets]**.
1. Legen Sie im Dialogfeld „Größe des Rotationssets“ die gewünschte Anzahl an Zeilen und Zellen fest.

   Wählen Sie für ein eindimensionales Rotationsset nur eine Zeile.

   Wählen Sie für ein zweidimensionales Rotationsset zwei oder mehr Zeilen.

1. Auswählen **[!UICONTROL OK]**.
1. Ziehen Sie Bilder auf das Raster im Anzeigebereich „Rotationsset“.
1. Wenn Sie fertig sind, stellen Sie sicher, dass rechts unten auf der Seite die Option **Nach dem Speichern veröffentlichen** ausgewählt ist (Standard).
1. Auswählen **[!UICONTROL Speichern]**.
1. Wählen Sie im Dialogfeld „Speichern“ einen Ordner aus, in dem das Rotationsset gespeichert werden soll. Geben Sie in das Feld „Dateiname“ den Namen des Rotationssets ein.
1. Auswählen **[!UICONTROL Speichern]**.

## Bearbeiten eines Rotationssets {#editing-a-spin-set}

Unabhängig davon, ob Sie ein veröffentlichtes Set oder ein nicht veröffentlichtes Set bearbeiten, wird die **[!UICONTROL Nach dem Speichern veröffentlichen]** -Option wirkt sich auf die Set- und Set-Mitglieder wie folgt aus:

| Set bereits veröffentlicht? | **[!UICONTROL Nach dem Speichern veröffentlichen]** vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten den Status „veröffentlicht“ bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

**So bearbeiten Sie ein Rotationsset:**

1. Rollover des Rotationssets auswählen **[!UICONTROL Bearbeiten]** Schaltfläche.
1. Führen Sie einen der folgenden Schritte aus:

   * **Entfernen von Bildern** - Wählen Sie das Bild aus und klicken Sie auf **[!UICONTROL Löschen]**.

   * **Bilder hinzufügen** - Ziehen Sie das Bild in eine Zelle.

   * **Neuanordnen von Zeilen (zweidimensionale Rotationssets)** - Wählen Sie ein Zeilenauswahlfeld (links neben der Zeile) aus und wählen Sie dann **[!UICONTROL Zeile nach unten]** oder **[!UICONTROL Zeile nach oben]**.

   * **Zeilen und Zellen hinzufügen** - Geben Sie in die Felder Zeilen und Zellen eine Zahl ein, um die Anzahl der Zeilen und die Anzahl der Zellen in jeder Zeile zu bestimmen.

1. Wenn Sie die Bearbeitung abgeschlossen haben, stellen Sie sicher, dass  rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Auswählen **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und wählen Sie dann **[!UICONTROL Speichern]**.

## Löschen eines Rotationssets {#deleting-a-spin-set}

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (bzw. die untergeordneten Elemente) innerhalb des Sets sind davon jedoch nicht betroffen; sie behalten ihren jeweiligen Status „veröffentlicht“ oder „unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

**So löschen Sie ein Rotationsset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Rotationssets aus.
1. Wechseln Sie in der Leiste &quot;Globale Navigation&quot;zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.
