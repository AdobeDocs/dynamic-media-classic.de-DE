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

Beispielsweise können Sie Bilder von Schirmmützen präsentieren, wobei die Schirme rot, grün oder blau sind. In diesem Fall benötigen Sie drei Aufnahmen derselben Mütze: Je eine Aufnahme mit einem roten Schirm, einem grünen und einem blauen Schirm. Darüber hinaus benötigen Sie ein rotes, grünes und blaues Farbfeld. Die Farbmuster dienen als Miniaturansichten, die Benutzer im Musterset-Viewer auswählen, um die rote, grüne oder blaue Kappe anzuzeigen.

## Erstellen eines Mustersets {#create}

Wenn Sie einen Satz erstellen, wirkt sich die Option **Publish nach dem Speichern** wie folgt auf den Satz und die Setmitglieder aus:

| **[!UICONTROL Publish nach einer Speicheroption]** ausgewählt, bevor sie gespeichert wird? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein Musterset:**

1. Führen Sie einen der folgenden Schritte aus:

   * **Wählen Sie die Bilder zuerst aus**: Wählen Sie im Durchsuchenbedienfeld die Bilder aus und gehen Sie dann zu **[!UICONTROL Build]** > **[!UICONTROL Mustersets]**.

   * **Starten Sie vom Bildschirm &quot;Musterset&quot;**: Wechseln Sie zu &quot;**[!UICONTROL Build]**&quot;> &quot;**[!UICONTROL Mustersets]**&quot;. Wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die Bilder in den Bereich „Ansichten“ auf der Seite „Musterset“.

1. Ziehen Sie Farbfelder, Muster oder Ausführungen in das Platzhalterfeld „Muster“ auf der Seite „Musterset“.

   Vergewissern Sie sich, dass die Musterdateien für Farben, Muster oder Ausführungen, die Sie in die Platzhalter ziehen, tatsächlich den Farben, Mustern oder Ausführungen des zugehörigen Bilds entsprechen.

1. Um die Reihenfolge der Bilder in Ihrem Musterset zu ändern, ziehen Sie die Bilder zu neuen Positionen.
1. Stellen Sie in der rechten unteren Ecke der Seite sicher, dass **[!UICONTROL Publish nach dem Speichern]** ausgewählt ist (Standard).
1. Wählen Sie &quot;**[!UICONTROL Speichern]**&quot;, wählen Sie einen Ordner zum Speichern Ihres Farbmuster-Mustersets aus, geben Sie einen Namen für das Set ein und wählen Sie &quot;**[!UICONTROL Senden]**&quot;.
1. Um das Musterset im Musterset-Viewer anzuzeigen, wählen Sie **[!UICONTROL Vorschau]** auf dem Bildschirm &quot;Musterset&quot;. Sie können Musterminiaturansichten im Musterset-Viewer auswählen, um zu sehen, wie sie sich verhalten.

## Bearbeiten eines Mustersets {#editing-a-swatch-set}

Unabhängig davon, ob Sie einen veröffentlichten oder nicht veröffentlichten Satz bearbeiten, wirkt sich die Option **[!UICONTROL Publish nach dem Speichern]** wie folgt auf das Set und die Setmitglieder aus:

| Set bereits veröffentlicht? | **[!UICONTROL Publish nach einer Speicheroption]** vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht. |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren Veröffentlichungsstatus bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht. |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie ein Musterset:**

1. Navigieren Sie in der Rasteransicht zu einem Musterset und wählen Sie unter dem Bild **[!UICONTROL Bearbeiten]** aus.
1. Führen Sie einen der folgenden Schritte aus:

   * Um ein Bild hinzuzufügen (veröffentlicht oder unveröffentlicht), ziehen Sie es aus einem Ordner in &quot;Assets hinzufügen&quot;auf die Seite **[!UICONTROL Ansichten]** des Mustersets.
   * Um ein Bild zu entfernen, wählen Sie es aus und klicken Sie dann in der Symbolleiste auf **[!UICONTROL Löschen]** .
   * Um die Bilder neu anzuordnen, ziehen Sie ein Bild in eine neue Position.

1. Wenn Sie mit der Bearbeitung des Sets fertig sind, stellen Sie sicher, dass rechts unten auf der Seite **[!UICONTROL Publish nach dem Speichern]** ausgewählt ist (Standard).
1. Wählen Sie &quot;**[!UICONTROL Speichern]**&quot;, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und wählen Sie dann &quot;**[!UICONTROL Speichern]**&quot;.

## Löschen eines Mustersets

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (oder &quot;untergeordneten Elemente&quot;) in diesem Satz sind jedoch nicht betroffen. Stattdessen behalten sie ihren vorhandenen Status veröffentlicht oder unveröffentlicht bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie ein Musterset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht mindestens ein Musterset aus.
1. Wechseln Sie in der Leiste &quot;Globale Navigation&quot;zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.
