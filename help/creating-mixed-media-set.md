---
title: Erstellen eines gemischten Mediensets
description: Erfahren Sie, wie Sie ein gemischtes Medienset erstellen.
uuid: a0c6e5fa-7a85-4376-b9a3-b72ae63d3d95
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0ff9e763-897c-4ba5-b606-a95d5e45f35e
feature: Dynamic Media Classic,Viewer,Mix-Mediensets
role: Business Practitioner
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 91%

---

# Erstellen eines gemischten Mediensets{#creating-a-mixed-media-set}

Erstellen Sie ein gemischtes Medienset, wenn Sie mehrere Arten von Viewern in einer Präsentation kombinieren möchten. Stellen Sie dabei sicher, dass die Bildsätze, Mustersets und Rotationssets für die Veröffentlichung bereit sind, bevor Sie sie zu dem gemischten Medienset hinzufügen.

![Gemischtes Medienset](/help/assets/mm_mixed_media_set.png)

## Erstellen eines gemischten Mediensets {#create-a-mixed-media-set}

Wenn Sie ein Set erstellen, wirkt sich die Option **Nach dem Speichern veröffentlichen** wie folgt auf das Set und die Set-Mitglieder aus:

| Option „Nach dem Speichern veröffentlichen“ vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein gemischtes Medienset:**

1. Klicken Sie auf **[!UICONTROL Erstellen]** > **[!UICONTROL Gemischte Mediensets]**.
1. Ziehen Sie die Videos, Bildsätze, Rotationssets und Muster aus der Asset-Bibliothek in den Anzeigebereich „Gemischte Mediensets“.

   >[!NOTE]
   >
   >Gemischte Mediensets unterstützen keine Assets mit Dateinamen, die eines der folgenden Zeichen enthalten: `( ) { }`.

1. Führen Sie einen der folgenden Schritte aus:

   * Um einen Soundtrack hinzuzufügen, ziehen Sie eine Audiodatei aus der Asset-Bibliothek in das Feld „Soundtrack“. Der Soundtrack wird während der Anzeige der Bilder angespielt. Er stoppt, wenn das Video abgespielt wird.
   * Sie können die Reihenfolge der Sets ändern, indem Sie sie im Anzeigebereich „Gemischte Mediensets“ an neue Positionen ziehen. Die Reihenfolge der Sets im Anzeigebereich entspricht der Reihenfolge von links nach rechts, in der den Benutzern die Sets im gemischten Medienset-Viewer angezeigt werden.
   * (Optional) Um eine benutzerdefinierte Miniaturansicht für ein Video im Viewer hinzuzufügen, ziehen Sie eine Bilddatei aus der Asset-Bibliothek in das Platzhalterfeld für die Miniaturansicht.

1. Stellen Sie sicher, dass rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Klicken Sie auf **[!UICONTROL Speichern]**, wählen Sie einen Ordner zum Speichern des gemischten Mediensets aus, geben Sie einen Namen für das Set ein und klicken Sie auf **[!UICONTROL Speichern]**.

   Um zu sehen, wie das kombinierte Bildset in einem Bildset-Viewer aussieht, klicken Sie auf **[!UICONTROL Vorschau]**.

## Bearbeiten eines gemischten Mediensets {#edit-a-mixed-media-set}

Sie können ein gemischtes Medienset bearbeiten. Falls Sie ein Set innerhalb eines gemischten Mediensets bearbeiten möchten, öffnen Sie dieses Set für sich allein, bearbeiten und speichern Sie es. Die Änderungen werden im gemischten Medienset angezeigt.

Unabhängig davon, ob Sie einen veröffentlichten oder unveröffentlichten Satz bearbeiten, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf den Satz und die Setmitglieder aus:

| Set bereits veröffentlicht? | Option „Nach dem Speichern veröffentlichen“ vor dem Speichern Ihrer Bearbeitungen ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |--- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten den Status „veröffentlicht“ bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie ein gemischte Medienset:**

1. Klicken Sie auf die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** des gemischten Mediensets.
1. Führen Sie einen der folgenden Schritte aus:

   * Um Elemente zu entfernen, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Löschen]**.
   * Um Elemente neu anzuordnen, ziehen Sie sie an die gewünschten Positionen.

1. Wenn Sie die Bearbeitung des Sets abgeschlossen haben, stellen Sie sicher, dass rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Klicken Sie auf **[!UICONTROL Speichern]** oder **[!UICONTROL Speicher unter]**.

## Löschen eines gemischten Mediensets {#deleting-a-mixed-media-set}

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (bzw. die untergeordneten Elemente) innerhalb des Sets sind davon jedoch nicht betroffen; sie behalten ihren jeweiligen Status „veröffentlicht“ oder „unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie ein gemischtes Medienset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere gemischte Mediensets aus.
1. Klicken Sie in der globalen Navigationsleiste auf **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.
