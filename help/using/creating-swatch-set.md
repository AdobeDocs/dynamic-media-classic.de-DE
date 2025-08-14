---
title: Erstellen eines Mustersets
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic ein Musterset erstellen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 49%

---

# Erstellen eines Mustersets{#creating-a-swatch-set}

Ein Musterset-Bildsatz ermöglicht den Benutzern die Ansicht eines Objekts in unterschiedlichen Farben, Mustern oder Ausführungen. Wenn Sie ein Musterset mit Farbfeldern erstellen möchten, benötigen Sie für jede Farbe, jedes Muster oder jede Ausführung, die Sie den Benutzern präsentieren möchten, jeweils ein Bild. Darüber hinaus benötigen Sie für jede Farbe, jedes Muster oder jede Ausführung auch jeweils ein entsprechendes Muster.

Beispielsweise können Sie Bilder von Schirmmützen präsentieren, wobei die Schirme rot, grün oder blau sind. In diesem Fall benötigen Sie drei Aufnahmen derselben Mütze: Je eine Aufnahme mit einem roten Schirm, einem grünen und einem blauen Schirm. Darüber hinaus benötigen Sie ein rotes, grünes und blaues Farbfeld. Die Farbmuster dienen als Miniaturen, die Benutzerinnen und Benutzer im Musterset-Viewer auswählen, um die Kappe mit rotem, grünem oder blauem Schirm anzuzeigen.

## Erstellen eines Mustersets {#create}

Wenn Sie einen Satz erstellen, wirkt sich die Option **Nach dem Speichern veröffentlichen** auf die Mitglieder des Satzes und des Satzes wie folgt aus:

| **[!UICONTROL Nach Speichern veröffentlichen]** vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein Musterset:**

1. Führen Sie einen der folgenden Schritte aus:

   * **Zuerst die Bilder auswählen**: Wählen Sie im Durchsuchen-Panel die Bilder aus und navigieren Sie dann zu **[!UICONTROL Erstellen]** > **[!UICONTROL Mustersets]**.

   * **Über den Bildschirm Farbfeldset starten**: Wechseln Sie zu **[!UICONTROL Erstellen]** > **[!UICONTROL Farbfeldsets]**. Wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die Bilder in den Bereich „Ansichten“ auf der Seite „Musterset“.

1. Ziehen Sie Farbfelder, Muster oder Ausführungen in das Platzhalterfeld „Muster“ auf der Seite „Musterset“.

   Vergewissern Sie sich, dass die Musterdateien für Farben, Muster oder Ausführungen, die Sie in die Platzhalter ziehen, tatsächlich den Farben, Mustern oder Ausführungen des zugehörigen Bilds entsprechen.

1. Um die Reihenfolge der Bilder in Ihrem Musterset zu ändern, ziehen Sie die Bilder zu neuen Positionen.
1. Stellen Sie sicher, dass in der rechten unteren Ecke der Seite **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]**, wählen Sie einen Ordner zum Speichern Ihres Farbmustersets aus, geben Sie einen Namen für das Set ein und wählen Sie **[!UICONTROL Senden]**.
1. Um das Farbfeldset im Farbfeldset-Viewer anzuzeigen, wählen Sie **[!UICONTROL Vorschau]** auf dem Bildschirm Farbfeldset aus. Sie können im Musterset-Viewer Musterminiaturansichten auswählen, um zu sehen, wie sie sich verhalten.

## Bearbeiten eines Mustersets {#editing-a-swatch-set}

Unabhängig davon, ob Sie ein veröffentlichtes oder ein unveröffentlichtes Set bearbeiten, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** auf die Mitglieder des Sets und des Sets wie folgt aus:

| Set bereits veröffentlicht? | **[!UICONTROL Nach dem Speichern veröffentlichen]** Speicheroption vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht. |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren veröffentlichten Status bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht. |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie ein Musterset:**

1. Navigieren Sie in der Rasteransicht zu einem Farbfeld-Set und wählen Sie dann unter dem Bild **[!UICONTROL Bearbeiten]** aus.
1. Führen Sie einen der folgenden Schritte aus:

   * Um ein Bild (veröffentlicht oder unveröffentlicht) hinzuzufügen, ziehen Sie es aus einem Ordner in Assets hinzufügen auf die Seite „Ansichten **[!UICONTROL des]**.
   * Um ein Bild zu entfernen, wählen Sie es aus und klicken Sie in der Symbolleiste **[!UICONTROL Löschen]**.
   * Um die Bilder neu anzuordnen, ziehen Sie ein Bild in eine neue Position.

1. Wenn Sie mit der Bearbeitung des Sets fertig sind, stellen Sie sicher, dass **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **[!UICONTROL Speichern]**.

## Löschen von Mustersets

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (oder „untergeordneten Elemente„) in diesem Set sind jedoch nicht betroffen. Stattdessen behalten sie jeweils ihren vorhandenen Status „Veröffentlicht“ oder „Unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie ein Musterset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht mindestens ein Farbfeldset aus.
1. Navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.
