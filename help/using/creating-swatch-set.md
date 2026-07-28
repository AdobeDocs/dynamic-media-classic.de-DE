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
autotag-review: '2026-05-13T17:44:21.987Z'
TQID: 'https://experienceleague.adobe.com/8nWsAO1rwDZnpj3GkUv7iUEqQR894oeoo81Vtr-uHcs'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 1343214cf19c9cfc6153e3f8b90c8ffc260de999
workflow-type: tm+mt
source-wordcount: 709
ht-degree: 42%

---

# Erstellen eines Mustersets{#creating-a-swatch-set}

Mit einem Farbfeldset können Benutzer ein Element in einer anderen Farbe, einem anderen Muster oder einer anderen Endverarbeitung anzeigen. Wenn Sie ein Musterset mit Farbfeldern erstellen möchten, benötigen Sie für jede Farbe, jedes Muster oder jede Ausführung, die Sie den Benutzern präsentieren möchten, jeweils ein Bild. Darüber hinaus benötigen Sie für jede Farbe, jedes Muster oder jede Ausführung auch jeweils ein entsprechendes Muster.

Beispielsweise können Sie Bilder von Schirmmützen präsentieren, wobei die Schirme rot, grün oder blau sind. In diesem Fall benötigen Sie drei Bilder derselben Kappe. Sie benötigen ein Bild für jeden der roten, grünen und blauen Scheine. Sie benötigen außerdem rote, grüne und blaue Farbfelder. Die Farbmuster dienen als Miniaturen, die Benutzerinnen und Benutzer im Musterset-Viewer auswählen, um die Kappe mit rotem, grünem oder blauem Schirm anzuzeigen.

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
1. Wählen Sie **[!UICONTROL Speichern]**, wählen Sie einen Ordner zum Speichern des Farbfeldsets aus, geben Sie einen Namen für das Set ein und wählen Sie **[!UICONTROL Senden]**.
1. Um das Farbfeldset im Farbfeldset-Viewer anzuzeigen, wählen Sie **[!UICONTROL Vorschau]** auf dem Bildschirm Farbfeldset aus. Sie können im Musterset-Viewer Musterminiaturansichten auswählen, um zu sehen, wie sie funktionieren.

## Bearbeiten eines Mustersets {#editing-a-swatch-set}

Unabhängig davon, ob Sie ein veröffentlichtes oder ein unveröffentlichtes Set bearbeiten, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** auf die Mitglieder des Sets und des Sets wie folgt aus:

| Set bereits veröffentlicht? | **[!UICONTROL Nach dem Speichern veröffentlichen]** Speicheroption vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht. |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten den Status „veröffentlicht“ bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht. |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie ein Musterset:**

1. Navigieren Sie in der Rasteransicht zu einem Musterset und wählen Sie dann unter dem Bild **[!UICONTROL Bearbeiten]** aus.
1. Führen Sie eine der folgenden Aktionen aus:

   * Um ein Bild (veröffentlicht oder unveröffentlicht) hinzuzufügen, ziehen Sie es aus einem Ordner in Assets hinzufügen auf die Seite „Ansichten **[!UICONTROL des]**.
   * Um ein Bild zu entfernen, wählen Sie es aus und klicken Sie in der Symbolleiste **[!UICONTROL Löschen]**.
   * Um die Bilder neu anzuordnen, ziehen Sie ein Bild in eine neue Position.

1. Wenn Sie mit der Bearbeitung des Sets fertig sind, stellen Sie sicher, dass **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **[!UICONTROL Speichern]**.

## Löschen von Mustersets

Wenn Sie ein Set löschen, wird das Set selbst in den Ordner „Gelöschte Elemente“ verschoben. Die Mitglieder in diesem Satz sind davon nicht betroffen, sie behalten ihren bestehenden Status „Veröffentlicht“ oder „Unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie ein Musterset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Mustersets aus.
1. Navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.
