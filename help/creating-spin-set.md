---
title: Erstellen eines Rotationssets
seo-title: Erstellen eines Rotationssets
description: 'null'
seo-description: Hier erfahren Sie, wie Sie ein Rotationsset erstellen.
uuid: 697 bd 78 f -5 e 39-46 bf-aa 6 d-ad 8 ab 99 fe 40 e
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/spin_ sets
discoiquuid: 735 b 5867-e 249-4627-a 5 a 5-25 c 19 c 2255 bf
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Erstellen eines Rotationssets{#creating-a-spin-set}

Um ein effektives Rotationsset erstellen zu können, müssen Sie darauf achten, die Bilder korrekt aufzunehmen. Sie können in Dynamic Media Classic ein Rotationsset erstellen, indem Sie auf "Erstellen" klicken und" Rotationssets" auswählen. Im Anzeigebereich „Rotationsset“ können Sie Rotationssets bearbeiten.

>[!NOTE]
>
>In früheren Versionen von Dynamic Media Classic wurden zweidimensionale Rotationssets nicht angeboten. Wenn Sie ein Rotationsset in einer früheren Version von Dynamic Media Classic erstellt haben, können Sie das eindimensionale Rotationsset nicht unter einem neuen Namen speichern. Klicken Sie im Anzeigebereich "Rotationsset" auf" Speichern unter" und geben Sie einen neuen Namen ein, damit Sie ihn in Dynamic Media Classic bearbeiten können.

## Richtlinien für das Aufnehmen von Rotationsset-Bildern {#guidelines-for-shooting-spin-set-images}

Allgemein gilt, je mehr Bilder das Rotationsset hat, desto besser kommt der Rotationseffekt zur Geltung. Eine höhere Anzahl von Rotationsset-Bildern bringt jedoch auch eine längere Ladezeit für die Bilder mit sich. Dynamic Media Classic empfiehlt diese Richtlinien für das Aufnehmen von Bildern für die Verwendung in Rotationssets:

* Verwenden Sie mindestens 8-12 Bilder in einem eindimensionalen Rotationsset und 16 bis 24 Bilder in zweidimensionalen Rotationssets.
* Verwenden Sie ein verlustfreies Format. Zu empfehlen sind die Formate TIFF und PNG.
* Maskieren Sie alle Bilder, so dass das Objekt vor einem reinweißen oder anderen kontrastreichen Hintergrund erscheint. Fügen Sie nach Wunsch Schatten hinzu.
* Vergewissern Sie sich, dass die Produktdetails gut ausgeleuchtet und fokussiert sind.
* Nehmen Sie Bilder für Modekleidung mit einer Gliederpuppe oder einem Model auf. Oft wird die Gliederpuppe entweder vollständig maskiert (durch Verwendung einer gläsernen Gliederpuppe) oder das Bild wird mit einer stilisierten Gliederpuppe dargestellt. Sie können ein Rotationsset auch mit einem Model aufnehmen, indem Sie die Anzahl unterschiedlicher Blickwinkel definieren. Markieren Sie jede Winkelposition mit Klebeband auf dem Boden, um dem Model Position und Blickrichtung für die Aufnahmen anzuzeigen.

## Erstellen eines Rotationssets {#create}

Beachten Sie, dass die Reihenfolge, in der das Rotationsset in Scene7 Publishing System verfasst oder erstellt wird, von Bedeutung ist. Je nachdem, in welcher Reihenfolge Sie die Assets anordnen, wenn Sie Bilder auf einem Raster auf der Seite „Rotationsset“ ablegen, dreht sich das Rotationsset in eine bestimmte Richtung. Deshalb entspricht die Reihenfolge, in der es im Konstruktor angezeigt wird, der Drehrichtung des Assets, wenn ein Benutzer den Mauszeiger oder Finger von links nach rechts bewegt.

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
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren veröffentlichten Status bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten den Status "Veröffentlicht" oder" Unveröffentlicht" bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

**So bearbeiten Sie ein Rotationsset**

1. Klicken Sie auf die Rollover-Schaltfläche **Bearbeiten** des Rotationssets.
1. Führen Sie einen der folgenden Schritte aus:

   **Entfernen von Bildern**

   Wählen Sie das Bild aus und klicken Sie dann auf **Löschen**.

   **Hinzufügen von Bildern**

   Ziehen Sie das Bild in eine Zelle.

   **Ändern der Zeilenreihenfolge (zweidimensionale Rotationssets)**

   Klicken Sie auf das Auswahlfeld links neben einer Zeile und klicken Sie dann auf **Zeile nach unten verschieben** bzw. **Zeile nach oben verschieben**.

   **Hinzufügen von Zeilen und Zellen**

   Geben Sie in die Felder „Zeilen“ und „Zellen“ die gewünschte Anzahl von Zeilen und von Zellen pro Zeile ein.

1. Wenn Sie die Bearbeitung abgeschlossen haben, stellen Sie sicher, dass rechts unten auf der Seite die Option **Nach dem Speichern veröffentlichen** ausgewählt ist (Standard).
1. Klicken Sie auf **Speichern**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **Speichern**.

## Löschen eines Rotationssets {#deleting-a-spin-set}

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (bzw. die untergeordneten Elemente) innerhalb des Sets sind davon jedoch nicht betroffen; sie behalten ihren jeweiligen Status „veröffentlicht“ oder „unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

**So löschen Sie ein Rotationsset**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Rotationssets aus.
1. Klicken Sie in der globalen Navigationsleiste auf **Datei** &gt; **Löschen** &gt; **Löschen**.

