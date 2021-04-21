---
title: Erstellen eines Rotationssets
description: Erfahren Sie, wie Sie ein Rotationsset erstellen.
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
feature: Dynamic Media Classic, Viewer, Rotationssets
role: Business Practitioner
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
translation-type: tm+mt
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 66%

---

# Erstellen eines Rotationssets{#creating-a-spin-set}

Um ein effektives Rotationsset erstellen zu können, müssen Sie darauf achten, die Bilder korrekt aufzunehmen. Sie können ein Rotationsset in Dynamic Media Classic erstellen, indem Sie auf &quot;Erstellen&quot;klicken und dann &quot;Rotationssets&quot;wählen. Im Anzeigebereich „Rotationsset“ können Sie Rotationssets bearbeiten.

>[!NOTE]
>
>In früheren Versionen von Dynamic Media Classic wurden keine zweidimensionalen Rotationssets Angebot. Wenn Sie ein Rotationsset in einer früheren Version von Dynamic Media Classic erstellt haben, können Sie das eindimensionale Rotationsset nicht ohne vorherige Speicherung unter einem anderen Namen speichern. Klicken Sie im Anzeigebereich &quot;Rotationsset&quot;auf &quot;Speichern unter&quot;und geben Sie einen neuen Namen ein, damit Sie ihn in Dynamic Media Classic bearbeiten können.

## Richtlinien für das Aufnehmen von Rotationsset-Bildern {#guidelines-for-shooting-spin-set-images}

Allgemein gilt, je mehr Bilder das Rotationsset hat, desto besser kommt der Rotationseffekt zur Geltung. Eine höhere Anzahl von Rotationsset-Bildern bringt jedoch auch eine längere Ladezeit für die Bilder mit sich. Dynamic Media Classic empfiehlt die folgenden Richtlinien für das Aufnehmen von Bildern zur Verwendung in Rotationssets:

* Verwenden Sie mindestens 8 bis 12 Bilder in einem eindimensionalen Rotationsset und 16 bis 24 Bilder in einem zweidimensionalen Rotationsset.
* Verwenden Sie ein verlustfreies Format. Zu empfehlen sind die Formate TIFF und PNG.
* Maskieren Sie alle Bilder, so dass das Objekt vor einem reinweißen oder anderen kontrastreichen Hintergrund erscheint. Fügen Sie nach Wunsch Schatten hinzu.
* Vergewissern Sie sich, dass die Produktdetails gut ausgeleuchtet und fokussiert sind.
* Nehmen Sie Bilder für Modekleidung mit einer Gliederpuppe oder einem Model auf. Oft wird das Mannequin entweder maskiert (mit einem Glasmannequin) oder eine stilisierte Mannequin/Dressform im Bild dargestellt. Sie können ein Rotationsset auch mit einem Model aufnehmen, indem Sie die Anzahl unterschiedlicher Blickwinkel definieren. Markieren Sie jede Winkelposition mit Klebeband auf dem Boden, um dem Model Position und Blickrichtung für die Aufnahmen anzuzeigen.

## Erstellen eines Rotationssets  {#create}

Die Reihenfolge, in der das Rotationsset in Dynamic Media Classic verfasst oder erstellt wird, ist wichtig. Je nachdem, in welcher Reihenfolge Sie die Assets anordnen, wenn Sie Bilder auf einem Raster auf der Seite „Rotationsset“ ablegen, dreht sich das Rotationsset in eine bestimmte Richtung. Daher wird das Asset in der Reihenfolge, in der es visuell angezeigt wird, gedreht, wenn ein Benutzer den Mauszeiger oder Finger von links nach rechts bewegt.

Wenn Sie ein Set erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| **[!UICONTROL Nach]** Auswahl der Option &quot;Nach dem Speichern veröffentlichen&quot;vor dem Speichern veröffentlichen? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

Nach dem Speichern eines Rotationssets können Sie seine Anzeige im Standard-Viewer mithilfe der Vorschau auf der Seite „Erstellen: Rotationsset“ testen.

**So erstellen Sie ein Rotationsset:**

1. Klicken Sie im Dropdown-Menü **[!UICONTROL Erstellen]** auf **[!UICONTROL Rotationssets]**.
1. Legen Sie im Dialogfeld „Größe des Rotationssets“ die gewünschte Anzahl an Zeilen und Zellen fest.

   Wählen Sie für ein eindimensionales Rotationsset nur eine Zeile.

   Wählen Sie für ein zweidimensionales Rotationsset zwei oder mehr Zeilen.

1. Klicken Sie auf **[!UICONTROL OK]**.
1. Ziehen Sie Bilder auf das Raster im Anzeigebereich „Rotationsset“.
1. Wenn Sie fertig sind, stellen Sie sicher, dass rechts unten auf der Seite die Option **Nach dem Speichern veröffentlichen** ausgewählt ist (Standard).
1. Klicken Sie auf **[!UICONTROL Speichern]**.
1. Wählen Sie im Dialogfeld „Speichern“ einen Ordner aus, in dem das Rotationsset gespeichert werden soll. Geben Sie in das Feld „Dateiname“ den Namen des Rotationssets ein.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Bearbeiten eines Rotationssets  {#editing-a-spin-set}

Unabhängig davon, ob Sie einen veröffentlichten oder unveröffentlichten Satz bearbeiten, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| Set bereits veröffentlicht? | **[!UICONTROL Nach]** Auswahl der Option &quot;Nach dem Speichern veröffentlichen&quot;veröffentlichen, bevor Sie Ihre Bearbeitung speichern? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |--- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten den Status „veröffentlicht“ bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

**So bearbeiten Sie ein Rotationsset:**

1. Klicken Sie auf die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** des Rotationssets.
1. Führen Sie einen der folgenden Schritte aus:

   * **Bilder**  entfernen: Wählen Sie das Bild aus und klicken Sie auf  **[!UICONTROL Löschen]**.

   * **Hinzufügen von Bildern** : Ziehen Sie das Bild in eine Zelle.

   * **Neuanordnen von Zeilen (zweidimensionale Rotationssets)**  - Klicken Sie auf ein Zeilenauswahlfeld (links neben der Zeile) und klicken Sie dann auf &quot;Zeile  **[!UICONTROL nach]** unten verschieben&quot;oder &quot;Zeile nach oben  **[!UICONTROL verschieben&quot;]**.

   * **Hinzufügen von Zeilen und Zellen** : Geben Sie im Feld &quot;Zeilen&quot;und &quot;Zellen&quot;eine Zahl ein, um die Anzahl der Zeilen und die Anzahl der Zellen in jeder Zeile festzulegen.

1. Wenn Sie die Bearbeitung abgeschlossen haben, stellen Sie sicher, dass  rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Klicken Sie auf **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **[!UICONTROL Speichern]**.

## Löschen eines Rotationssets  {#deleting-a-spin-set}

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (bzw. die untergeordneten Elemente) innerhalb des Sets sind davon jedoch nicht betroffen; sie behalten ihren jeweiligen Status „veröffentlicht“ oder „unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually-publishing-assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually-unpublishing-assets).

**So löschen Sie ein Rotationsset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Rotationssets aus.
1. Klicken Sie in der globalen Navigationsleiste auf **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.
