---
title: Erstellen eines Rotationssets
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic ein Rotationsset erstellen.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 55%

---

# Erstellen eines Rotationssets{#creating-a-spin-set}

Um ein effektives Rotationsset erstellen zu können, müssen Sie darauf achten, die Bilder korrekt aufzunehmen. Sie können ein Rotationsset in Adobe Dynamic Media Classic erstellen, indem Sie auf die Schaltfläche Erstellen klicken und Rotationssets auswählen. Im Anzeigebereich „Rotationsset“ können Sie Rotationssets bearbeiten.

>[!NOTE]
>
>Frühere Versionen von Adobe Dynamic Media Classic boten keine zweidimensionalen Rotationssets an. Wenn Sie ein Rotationsset in einer früheren Version von Adobe Dynamic Media Classic erstellt haben, können Sie das eindimensionale Rotationsset nicht speichern, ohne es zuvor unter einem anderen Namen zu speichern. Wählen Sie im Bildschirm &quot;Rotationsset&quot;die Option **[!UICONTROL Speichern unter]** und geben Sie einen neuen Namen ein, damit Sie ihn in Adobe Dynamic Media Classic bearbeiten können.

## Richtlinien für das Aufnehmen von Rotationsset-Bildern {#guidelines-for-shooting-spin-set-images}

Allgemein gilt, je mehr Bilder das Rotationsset hat, desto besser kommt der Rotationseffekt zur Geltung. Eine höhere Anzahl von Rotationsset-Bildern bringt jedoch auch eine längere Ladezeit für die Bilder mit sich. Adobe Dynamic Media Classic empfiehlt die folgenden Richtlinien für das Fotografieren von Bildern zur Verwendung in Rotationssets:

* Verwenden Sie mindestens 8 bis 12 Bilder in einem eindimensionalen Rotationsset und 16 bis 24 Bilder in einem zweidimensionalen Rotationsset.
* Verwenden Sie ein verlustfreies Format. Zu empfehlen sind die Formate TIFF und PNG.
* Maskieren Sie alle Bilder, so dass das Objekt vor einem reinweißen oder anderen kontrastreichen Hintergrund erscheint. Fügen Sie nach Wunsch Schatten hinzu.
* Vergewissern Sie sich, dass die Produktdetails gut ausgeleuchtet und fokussiert sind.
* Nehmen Sie Bilder für Modekleidung mit einer Gliederpuppe oder einem Model auf. Häufig ist das Mannequin entweder maskiert (mit einem Glasmannequin) oder eine stilisierte Mannequin/Dressform wird im Bild gezeigt. Sie können ein Rotationsset auch mit einem Model aufnehmen, indem Sie die Anzahl unterschiedlicher Blickwinkel definieren. Markieren Sie jeden Winkel mit Band auf dem Boden, damit Sie das Modell zu Schritt und Blick in die Richtung jedes Schusses führen können.

## Erstellen eines Rotationssets {#create}

Die Reihenfolge, in der das Rotationsset in Adobe Dynamic Media Classic erstellt oder erstellt wird, ist wichtig. Je nachdem, in welcher Reihenfolge Sie die Assets anordnen, wenn Sie Bilder auf einem Raster auf der Seite „Rotationsset“ ablegen, dreht sich das Rotationsset in eine bestimmte Richtung. Daher wird das Asset in der visuell angezeigten Reihenfolge angezeigt, wenn ein Benutzer seinen Mauszeiger bewegt oder seinen Finger von links nach rechts bewegt.

Wenn Sie ein Set erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| **[!UICONTROL Nach der]** Speicheroption Veröffentlichen vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

Nach dem Speichern eines Rotationssets können Sie seine Anzeige im Standard-Viewer mithilfe der Vorschau auf der Seite „Erstellen: Rotationsset“ testen.

**So erstellen Sie ein Rotationsset:**

1. Wählen Sie im Dropdown-Menü **[!UICONTROL Build]** die Option **[!UICONTROL Rotationssets]** aus.
1. Legen Sie im Dialogfeld „Größe des Rotationssets“ die gewünschte Anzahl an Zeilen und Zellen fest.

   Wählen Sie für ein eindimensionales Rotationsset nur eine Zeile.

   Wählen Sie für ein zweidimensionales Rotationsset zwei oder mehr Zeilen.

1. Wählen Sie **[!UICONTROL OK]** aus.
1. Ziehen Sie Bilder auf das Raster im Anzeigebereich „Rotationsset“.
1. Wenn Sie fertig sind, stellen Sie sicher, dass rechts unten auf der Seite die Option **Nach dem Speichern veröffentlichen** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Save]** aus.
1. Wählen Sie im Dialogfeld „Speichern“ einen Ordner aus, in dem das Rotationsset gespeichert werden soll. Geben Sie in das Feld „Dateiname“ den Namen des Rotationssets ein.
1. Wählen Sie **[!UICONTROL Save]** aus.

## Bearbeiten eines Rotationssets {#editing-a-spin-set}

Unabhängig davon, ob Sie einen veröffentlichten oder einen nicht veröffentlichten Satz bearbeiten, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf den Satz und die Setmitglieder aus:

| Set bereits veröffentlicht? | **[!UICONTROL Nach der]** Speicheroption veröffentlichen vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten den Status „veröffentlicht“ bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

**So bearbeiten Sie ein Rotationsset:**

1. Wählen Sie die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** des Rotationssets aus.
1. Führen Sie einen der folgenden Schritte aus:

   * **Entfernen von Bildern**  - Wählen Sie das Bild aus und klicken Sie auf  **[!UICONTROL Löschen]**.

   * **Bilder hinzufügen**  - Ziehen Sie das Bild in eine Zelle.

   * **Neuanordnen von Zeilen (zweidimensionale Rotationssets)**  - Wählen Sie ein Zeilenauswahlfeld (links neben der Zeile) aus und wählen Sie dann  **[!UICONTROL Zeile]** nach unten verschieben oder Zeile nach oben  **[!UICONTROL verschieben]** aus.

   * **Zeilen und Zellen hinzufügen**  - Geben Sie in das Feld &quot;Zeilen&quot;und in das Feld &quot;Zellen&quot;eine Zahl ein, um die Anzahl der Zeilen und die Anzahl der Zellen in jeder Zeile zu bestimmen.

1. Wenn Sie die Bearbeitung abgeschlossen haben, stellen Sie sicher, dass  rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Save]**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für den Satz ein und wählen Sie **[!UICONTROL Save]** aus.

## Löschen eines Rotationssets {#deleting-a-spin-set}

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (bzw. die untergeordneten Elemente) innerhalb des Sets sind davon jedoch nicht betroffen; sie behalten ihren jeweiligen Status „veröffentlicht“ oder „unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

**So löschen Sie ein Rotationsset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Rotationssets aus.
1. Wechseln Sie in der globalen Navigationsleiste zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.
