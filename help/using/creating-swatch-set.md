---
title: Erstellen eines Mustersets
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic ein Musterset erstellen.
uuid: 250b3525-310d-4481-b0bc-f9057e823e0b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 631d2b2d-9e69-4b96-8392-17e00a1a8de0
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
topic: Content Management
level: Intermediate
source-git-commit: a9bd472705bce32f63a5710c3266e51256d17a00
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 58%

---

# Erstellen eines Mustersets{#creating-a-swatch-set}

Ein Musterset-Bildsatz ermöglicht den Benutzern die Ansicht eines Objekts in unterschiedlichen Farben, Mustern oder Ausführungen. Wenn Sie ein Musterset mit Farbfeldern erstellen möchten, benötigen Sie für jede Farbe, jedes Muster oder jede Ausführung, die Sie den Benutzern präsentieren möchten, jeweils ein Bild. Darüber hinaus benötigen Sie für jede Farbe, jedes Muster oder jede Ausführung auch jeweils ein entsprechendes Muster.

Beispielsweise können Sie Bilder von Schirmmützen präsentieren, wobei die Schirme rot, grün oder blau sind. In diesem Fall benötigen Sie drei Aufnahmen derselben Mütze: Je eine Aufnahme mit einem roten Schirm, einem grünen und einem blauen Schirm. Darüber hinaus benötigen Sie ein rotes, grünes und blaues Farbfeld. Die Farbmuster dienen als Miniaturansichten, die Benutzer im Musterset-Viewer auswählen, um die rote, grüne oder blaue Kappe anzuzeigen.

## Erstellen eines Mustersets {#create}

Wenn Sie ein Set erstellen, wirkt sich die Option **Nach dem Speichern veröffentlichen** wie folgt auf das Set und die Set-Mitglieder aus:

| **[!UICONTROL Nach dem Speichern veröffentlichen]** vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein Musterset:**

1. Führen Sie einen der folgenden Schritte aus:

   * **Auswählen der Bilder zuerst** - Wählen Sie im Durchsuchenbedienfeld die Bilder aus und navigieren Sie zu **[!UICONTROL Build]** > **[!UICONTROL Mustersets]**.

   * **Starten Sie über den Bildschirm &quot;Musterset&quot;** - Gehen Sie zu **[!UICONTROL Build]** > **[!UICONTROL Mustersets]**. Wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die Bilder in den Bereich „Ansichten“ auf der Seite „Musterset“.

1. Ziehen Sie Farbfelder, Muster oder Ausführungen in das Platzhalterfeld „Muster“ auf der Seite „Musterset“.

   Vergewissern Sie sich, dass die Musterdateien für Farben, Muster oder Ausführungen, die Sie in die Platzhalter ziehen, tatsächlich den Farben, Mustern oder Ausführungen des zugehörigen Bilds entsprechen.

1. Um die Reihenfolge der Bilder in Ihrem Musterset zu ändern, ziehen Sie die Bilder zu neuen Positionen.
1. Stellen Sie sicher, dass rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Auswählen **[!UICONTROL Speichern]**, wählen Sie einen Ordner zum Speichern Ihres Farbmuster-Mustersets aus, geben Sie einen Namen für das Set ein und wählen Sie **[!UICONTROL Einsenden]**.
1. Um das Musterset im Musterset-Viewer anzuzeigen, wählen Sie **[!UICONTROL Vorschau]** auf dem Bildschirm &quot;Musterset&quot;angezeigt. Sie können Musterminiaturansichten im Musterset-Viewer auswählen, um zu sehen, wie sie sich verhalten.

## Bearbeiten eines Mustersets {#editing-a-swatch-set}

Unabhängig davon, ob Sie ein veröffentlichtes oder unveröffentlichtes Set bearbeiten, wird die **[!UICONTROL Nach dem Speichern veröffentlichen]** -Option wirkt sich auf die Set- und Set-Mitglieder wie folgt aus:

| Set bereits veröffentlicht? | **[!UICONTROL Veröffentlichen nach]** Speicheroption ausgewählt, bevor Sie Ihre Bearbeitung speichern? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht. |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren Veröffentlichungsstatus bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht. |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie ein Musterset:**

1. Navigieren Sie in der Rasteransicht zu einem Musterset und wählen Sie unter dem Bild die Option **[!UICONTROL Bearbeiten]**.
1. Führen Sie einen der folgenden Schritte aus:

   * Um ein Bild hinzuzufügen (veröffentlicht oder unveröffentlicht), ziehen Sie es aus einem Ordner in &quot;Assets hinzufügen&quot;auf das Musterset. **[!UICONTROL Ansichten]** Seite.
   * Um ein Bild zu entfernen, wählen Sie es aus und klicken Sie auf **[!UICONTROL Löschen]** in der Symbolleiste.
   * Um die Bilder neu anzuordnen, ziehen Sie ein Bild in eine neue Position.

1. Wenn Sie die Bearbeitung des Sets abgeschlossen haben, stellen Sie sicher, dass rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Auswählen **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und wählen Sie dann **[!UICONTROL Speichern]**.

## Löschen eines Mustersets {#deleting-a-swatch-set}

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (oder &quot;untergeordneten Elemente&quot;) in diesem Satz sind jedoch nicht betroffen. Stattdessen behalten sie ihren vorhandenen Status veröffentlicht oder unveröffentlicht bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie ein Musterset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht mindestens ein Musterset aus.
1. Wechseln Sie in der Leiste Globale Navigation zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.
