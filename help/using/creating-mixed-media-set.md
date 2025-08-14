---
title: Erstellen eines gemischten Mediensets
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic ein gemischtes Medienset erstellen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 56%

---

# Erstellen eines gemischten Mediensets{#creating-a-mixed-media-set}

Erstellen Sie ein gemischtes Medienset, wenn Sie mehrere Arten von Viewern in einer Präsentation kombinieren möchten. Stellen Sie dabei sicher, dass die Bildsätze, Mustersets und Rotationssets für die Veröffentlichung bereit sind, bevor Sie sie zu dem gemischten Medienset hinzufügen.

![Gemischtes Medienset](/help/using/assets/mm_mixed_media_set.png)

## Erstellen eines gemischten Mediensets {#create-a-mixed-media-set}

Wenn Sie einen Satz erstellen, wirkt sich die Option **Nach dem Speichern veröffentlichen** auf die Mitglieder des Satzes und des Satzes wie folgt aus:

| Vor dem Speichern die Option „Nach dem Speichern veröffentlichen“ ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein gemischtes Medienset:**

1. Navigieren Sie **[!UICONTROL Erstellen]** > **[!UICONTROL Gemischte Mediensets]**.
1. Ziehen Sie die Videos, Bildsätze, Rotationssets und Muster aus der Asset-Bibliothek in den Anzeigebereich „Gemischte Mediensets“.

   >[!NOTE]
   >
   >Ein gemischtes Medienset unterstützt keine Assets mit Dateinamen, die eines der folgenden Zeichen enthalten: `( ) { }`.

1. Führen Sie einen der folgenden Schritte aus:

   * Um einen Soundtrack hinzuzufügen, ziehen Sie eine Audiodatei aus der Asset-Bibliothek in das Feld „Soundtrack“. Der Soundtrack wird während der Anzeige der Bilder angespielt. Er stoppt, wenn ein Video wiedergegeben wird.
   * Sie können die Reihenfolge der Sets ändern, indem Sie sie im Anzeigebereich „Gemischte Mediensets“ an neue Positionen ziehen. Die Reihenfolge der Sets im Anzeigebereich entspricht der Reihenfolge von links nach rechts, in der den Benutzern die Sets im gemischten Medienset-Viewer angezeigt werden.
   * (Optional) Um eine benutzerdefinierte Miniaturansicht für ein Video im Viewer hinzuzufügen, ziehen Sie eine Bilddatei aus der Asset-Bibliothek in das Platzhalterfeld für die Miniaturansicht.

1. Stellen Sie sicher, dass in der rechten unteren Ecke der Seite **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]** aus.
1. Wählen Sie einen Ordner für das Speichern des gemischten Mediensets aus und geben Sie dann einen Namen für das Set ein.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

   Um anzuzeigen, wie das Kombinationsbildset in einem Bildset-Viewer aussieht, wählen Sie **[!UICONTROL Vorschau]** aus.

## Bearbeiten eines gemischten Mediensets {#edit-a-mixed-media-set}

Sie können ein gemischtes Medienset bearbeiten. Falls Sie ein Set innerhalb eines gemischten Mediensets bearbeiten möchten, öffnen Sie dieses Set für sich allein, bearbeiten und speichern Sie es. Die Bearbeitungen werden im gemischten Medienset angezeigt.

Unabhängig davon, ob Sie ein veröffentlichtes oder ein unveröffentlichtes Set bearbeiten, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** auf die Mitglieder des Sets und des Sets wie folgt aus:

| Set bereits veröffentlicht? | **[!UICONTROL Nach dem Speichern veröffentlichen]** Option vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- |--- |--- |--- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren veröffentlichten Status bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie ein gemischtes Medienset:**

1. Klicken Sie auf die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** für das gemischte Medienset.
1. Führen Sie einen der folgenden Schritte aus:

   * Um Elemente zu entfernen, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Löschen]**.
   * Um Elemente neu anzuordnen, ziehen Sie sie an die gewünschten Positionen.

1. Wenn Sie mit der Bearbeitung des Sets fertig sind, stellen Sie sicher, dass **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]** oder **[!UICONTROL Speichern unter]**.

## Löschen eines gemischten Mediensets

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (oder „untergeordneten Elemente„) in diesem Set sind jedoch nicht betroffen. Stattdessen behalten sie jeweils ihren vorhandenen Status „Veröffentlicht“ oder „Unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie ein gemischtes Medienset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere gemischte Mediensets aus.
1. Navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.
