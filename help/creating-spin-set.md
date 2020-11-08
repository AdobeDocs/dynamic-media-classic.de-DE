---
title: Erstellen eines Rotationssets
seo-title: Erstellen eines Rotationssets
description: 'null'
seo-description: Erfahren Sie, wie Sie ein Rotationsset erstellen.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 74%

---


# Erstellen eines Rotationssets{#creating-a-spin-set}

Um ein effektives Rotationsset erstellen zu können, müssen Sie darauf achten, die Bilder korrekt aufzunehmen. Sie können ein Rotationsset in Dynamic Media Classic erstellen, indem Sie auf &quot;Erstellen&quot;klicken und &quot;Rotationssets&quot;wählen. Im Anzeigebereich „Rotationsset“ können Sie Rotationssets bearbeiten.

>[!NOTE]
>
>In früheren Versionen von Dynamic Media Classic wurden keine zweidimensionalen Rotationssets Angebot. Wenn Sie ein Rotationsset in einer früheren Version von Dynamic Media Classic erstellt haben, können Sie das eindimensionale Rotationsset nicht speichern, ohne es zuvor unter einem anderen Namen zu speichern. Klicken Sie im Anzeigebereich &quot;Rotationsset&quot;auf &quot;Speichern unter&quot;und geben Sie einen neuen Namen ein, damit Sie ihn in &quot;Dynamic Media Classic&quot;bearbeiten können.

## Richtlinien für das Aufnehmen von Rotationsset-Bildern {#guidelines-for-shooting-spin-set-images}

Allgemein gilt, je mehr Bilder das Rotationsset hat, desto besser kommt der Rotationseffekt zur Geltung. Eine höhere Anzahl von Rotationsset-Bildern bringt jedoch auch eine längere Ladezeit für die Bilder mit sich. Dynamic Media Classic empfiehlt die folgenden Richtlinien für das Aufnehmen von Bildern zur Verwendung in Rotationssets:

* Verwenden Sie mindestens 8 bis 12 Bilder in einem eindimensionalen Rotationsset und 16 bis 24 Bilder in einem zweidimensionalen Rotationsset.
* Verwenden Sie ein verlustfreies Format. Zu empfehlen sind die Formate TIFF und PNG.
* Maskieren Sie alle Bilder, so dass das Objekt vor einem reinweißen oder anderen kontrastreichen Hintergrund erscheint. Fügen Sie nach Wunsch Schatten hinzu.
* Vergewissern Sie sich, dass die Produktdetails gut ausgeleuchtet und fokussiert sind.
* Nehmen Sie Bilder für Modekleidung mit einer Gliederpuppe oder einem Model auf. Oft wird die Gliederpuppe entweder vollständig maskiert (durch Verwendung einer gläsernen Gliederpuppe) oder das Bild wird mit einer stilisierten Gliederpuppe dargestellt. Sie können ein Rotationsset auch mit einem Model aufnehmen, indem Sie die Anzahl unterschiedlicher Blickwinkel definieren. Markieren Sie jede Winkelposition mit Klebeband auf dem Boden, um dem Model Position und Blickrichtung für die Aufnahmen anzuzeigen.

## Erstellen eines Rotationssets {#create}

Beachten Sie, dass die Reihenfolge, in der das Rotationsset in Dynamic Media Classic erstellt oder verfasst wird, wichtig ist. Je nachdem, in welcher Reihenfolge Sie die Assets anordnen, wenn Sie Bilder auf einem Raster auf der Seite „Rotationsset“ ablegen, dreht sich das Rotationsset in eine bestimmte Richtung. Deshalb entspricht die Reihenfolge, in der es im Konstruktor angezeigt wird, der Drehrichtung des Assets, wenn ein Benutzer den Mauszeiger oder Finger von links nach rechts bewegt.

Wenn Sie ein Set erstellen, wirkt sich die Option **Nach dem Speichern veröffentlichen** wie folgt auf das Set und die Set-Mitglieder aus:

| Option „Nach dem Speichern veröffentlichen“ vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

Nach dem Speichern eines Rotationssets können Sie seine Anzeige im Standard-Viewer mithilfe der Vorschau auf der Seite „Erstellen: Rotationsset“ testen.

**So erstellen Sie ein Rotationsset**

1. Klicken Sie im Dropdown-Menü **Erstellen** auf **Rotationssets**.
1. Legen Sie im Dialogfeld „Größe des Rotationssets“ die gewünschte Anzahl an Zeilen und Zellen fest.

   Wählen Sie für ein eindimensionales Rotationsset nur eine Zeile.

   Wählen Sie für ein zweidimensionales Rotationsset zwei oder mehr Zeilen.

1. Klicken Sie auf **OK**.
1. Ziehen Sie Bilder auf das Raster im Anzeigebereich „Rotationsset“.
1. Wenn Sie fertig sind, stellen Sie sicher, dass rechts unten auf der Seite die Option **Nach dem Speichern veröffentlichen** ausgewählt ist (Standard).
1. Klicken Sie auf **Speichern**.
1. Wählen Sie im Dialogfeld „Speichern“ einen Ordner aus, in dem das Rotationsset gespeichert werden soll. Geben Sie in das Feld „Dateiname“ den Namen des Rotationssets ein.
1. Klicken Sie auf **Speichern**.

## Bearbeiten eines Rotationssets {#editing-a-spin-set}

Je nachdem, ob Sie ein veröffentlichtes oder unveröffentlichtes Set bearbeiten, wirkt sich die Option **Nach dem Speichern veröffentlichen** wie folgt auf das Set und die Set-Mitglieder aus:

| Set bereits veröffentlicht? | Option „Nach dem Speichern veröffentlichen“ vor dem Speichern Ihrer Bearbeitungen ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |--- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren Status &quot;veröffentlicht&quot;bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status &quot;veröffentlicht&quot;oder &quot;unveröffentlicht&quot;bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

**So bearbeiten Sie ein Rotationsset**

1. Klicken Sie auf die Rollover-Schaltfläche **Bearbeiten** des Rotationssets.
1. Führen Sie einen der folgenden Schritte aus:

   * **Entfernen von Bildern** Wählen Sie das Bild aus und klicken Sie auf 
**Löschen**.

   * **Hinzufügen von Bildern** Ziehen Sie das Bild in eine Zelle.

   * **Neuanordnen von Zeilen (zweidimensionale Rotationssets)** Klicken Sie auf ein Zeilenauswahlfeld (links neben der Zeile) und dann auf 
**Zeile nach unten** oder **nach oben** verschieben

   * **Hinzufügen von Zeilen und Zellen** Geben Sie im Feld &quot;Zeilen&quot;und im Feld &quot;Zellen&quot;eine Zahl ein, um die Anzahl der Zeilen und die Anzahl der Zellen in jeder Zeile festzulegen.

1. Wenn Sie die Bearbeitung abgeschlossen haben, stellen Sie sicher, dass  rechts unten auf der Seite die Option **Nach dem Speichern veröffentlichen** ausgewählt ist (Standard).
1. Klicken Sie auf **Speichern**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **Speichern**.

## Löschen eines Rotationssets {#deleting-a-spin-set}

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (bzw. die untergeordneten Elemente) innerhalb des Sets sind davon jedoch nicht betroffen; sie behalten ihren jeweiligen Status „veröffentlicht“ oder „unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

**So löschen Sie ein Rotationsset**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Rotationssets aus.
1. Klicken Sie in der globalen Navigationsleiste auf **Datei** > **Löschen** > **Löschen**.

