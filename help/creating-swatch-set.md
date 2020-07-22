---
title: Erstellen eines Mustersets
seo-title: Erstellen eines Mustersets
description: 'null'
seo-description: Erfahren Sie, wie Sie ein Musterset erstellen.
uuid: 250b3525-310d-4481-b0bc-f9057e823e0b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 631d2b2d-9e69-4b96-8392-17e00a1a8de0
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 84%

---


# Erstellen eines Mustersets{#creating-a-swatch-set}

Ein Musterset-Bildsatz ermöglicht den Benutzern die Ansicht eines Objekts in unterschiedlichen Farben, Mustern oder Ausführungen. Wenn Sie ein Musterset mit Farbfeldern erstellen möchten, benötigen Sie für jede Farbe, jedes Muster oder jede Ausführung, die Sie den Benutzern präsentieren möchten, jeweils ein Bild. Darüber hinaus benötigen Sie für jede Farbe, jedes Muster oder jede Ausführung auch jeweils ein entsprechendes Muster.

Beispielsweise können Sie Bilder von Schirmmützen präsentieren, wobei die Schirme rot, grün oder blau sind. In diesem Fall benötigen Sie drei Aufnahmen derselben Mütze: Je eine Aufnahme mit einem roten Schirm, einem grünen und einem blauen Schirm. Darüber hinaus benötigen Sie ein rotes, grünes und blaues Farbfeld. Die Farbfelder dienen als Miniaturansichten, auf die die Benutzer im Musterset-Viewer klicken können, um die Mütze mit rotem, grünem oder blauem Schirm anzuzeigen.

## Erstellen eines Mustersets {#create}

Wenn Sie einen Satz erstellen, wirkt sich die Option Nach dem Speichern **veröffentlichen** wie folgt auf das Set und die Set-Mitglieder aus:
| Option &quot;Nach dem Speichern veröffentlichen&quot;vor dem Speichern ausgewählt?|Status des Sets nach dem Speichern|Status der Set-Mitglieder nach dem Speichern|
|— |— |— |
|Ja|Veröffentlicht|Veröffentlicht|
|Nein|Unveröffentlicht|Set-Mitglieder behalten ihren Status &quot;veröffentlicht&quot;oder &quot;unveröffentlicht&quot;bei.|

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein Musterset**

1. Führen Sie einen der folgenden Schritte aus:

   **Wählen Sie die Bilder zuerst** im Durchsuchenbedienfeld aus, wählen Sie die Bilder aus und klicken Sie dann auf &quot;Erstellen&quot;> &quot;Mustersets&quot;.

   **Klicken Sie im Anzeigebereich** &quot;Musterset&quot;auf &quot;Erstellen&quot;> &quot;Mustersets&quot;. Wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die Bilder in den Bereich „Ansichten“ auf der Seite „Musterset“.

1. Ziehen Sie Farbfelder, Muster oder Ausführungen in das Platzhalterfeld „Muster“ auf der Seite „Musterset“.

   Vergewissern Sie sich, dass die Musterdateien für Farben, Muster oder Ausführungen, die Sie in die Platzhalter ziehen, tatsächlich den Farben, Mustern oder Ausführungen des zugehörigen Bilds entsprechen.

1. Um die Reihenfolge der Bilder in Ihrem Musterset zu ändern, ziehen Sie die Bilder zu neuen Positionen.
1. Stellen Sie sicher, dass rechts unten auf der Seite die Option **Nach dem Speichern veröffentlichen** ausgewählt ist (Standard).
1. Klicken Sie auf **Speichern**, wählen Sie einen Ordner aus, in dem Sie Ihr Farbfeld-Musterset ablegen wollen, geben Sie einen Namen für das Set ein und klicken Sie auf „Senden“.
1. Um Ihr Musterset im Musterset-Viewer anzuzeigen, klicken Sie im Anzeigebereich „Musterset“ auf **Vorschau**. Sie können auf die Muster-Miniaturansichten im Anzeigebereich „Musterset“ klicken, um zu sehen, wie sie sich verhalten.

## Bearbeiten eines Mustersets {#editing-a-swatch-set}

Abhängig davon, ob Sie ein veröffentlichtes oder unveröffentlichtes Set bearbeiten, wirkt sich die Option **Nach dem Speichern veröffentlichen** wie folgt auf das Set und die Set-Mitglieder aus:

| Set bereits veröffentlicht? | Option „Nach dem Speichern veröffentlichen“ vor dem Speichern Ihrer Bearbeitungen ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |--- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren Status &quot;veröffentlicht&quot;bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status &quot;veröffentlicht&quot;oder &quot;unveröffentlicht&quot;bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie ein Musterset**

1. Wählen Sie in der Rasteransicht das gewünschte Musterset und klicken Sie unterhalb des Bildes auf **Bearbeiten**.
1. Führen Sie einen der folgenden Schritte aus:

   * Um ein Bild hinzuzufügen (veröffentlicht oder unveröffentlicht), ziehen Sie es aus einem Ordner in „Assets hinzufügen“ auf die Seite **Ansichten** des Mustersets.
   * Um ein Bild zu entfernen, wählen Sie es aus und klicken Sie in der Symbolleiste auf **Löschen**.
   * Um die Bilder neu anzuordnen, ziehen Sie ein Bild in eine neue Position.

1. Wenn Sie die Bearbeitung des Sets abgeschlossen haben, stellen Sie sicher, dass rechts unten auf der Seite die Option **Nach dem Speichern veröffentlichen** ausgewählt ist (Standard).
1. Klicken Sie auf **Speichern**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **Speichern**.

## Löschen eines Mustersets {#deleting-a-swatch-set}

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (bzw. die untergeordneten Elemente) innerhalb des Sets sind davon jedoch nicht betroffen; sie behalten ihren jeweiligen Status „veröffentlicht“ oder „unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie ein Musterset**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Mustersets aus.
1. Klicken Sie in der globalen Navigationsleiste auf **Datei** > **Löschen** > **Löschen**.

