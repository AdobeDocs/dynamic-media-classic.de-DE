---
title: Verschieben, Umbenennen und Löschen von Assets
description: Erfahren Sie, wie Sie Assets in Adobe Dynamic Media Classic verschieben, umbenennen und löschen können.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 17%

---

# Verschieben, Umbenennen und Löschen von Assets{#moving-renaming-and-deleting-assets}

Sie können Assets aus dem Bedienfeld &quot;Durchsuchen&quot;verschieben, umbenennen und löschen. Außerdem können Sie mithilfe einer Textdatei viele Assets auf einmal löschen.

## Verschieben von Assets {#move-assets}

Sie können Assets im Bedienfeld &quot;Durchsuchen&quot;in verschiedene Ordner verschieben.

**So verschieben Sie Assets:**

1. Wählen Sie die Assets im Bedienfeld &quot;Durchsuchen&quot;aus und führen Sie einen der folgenden Schritte aus:

   * Zeigen Sie den Ordner an, in den Sie die Assets verschieben möchten, und ziehen Sie die Assets in den Ordner.
   * Wechseln Sie zu &quot;**[!UICONTROL Datei]**&quot;> &quot;**[!UICONTROL Verschieben]**&quot;, wählen Sie einen Ordner im Fenster &quot;Assets verschieben&quot;aus und wählen Sie &quot;**[!UICONTROL Verschieben]**&quot;.

## Umbenennen von Assets {#rename-assets}

1. Wählen Sie das Asset im Bedienfeld &quot;Durchsuchen&quot;aus und führen Sie einen der folgenden Schritte aus:

   * Wählen Sie den Namen aus, geben Sie einen neuen Namen ein und drücken Sie **[!UICONTROL Enter]** oder wählen Sie weg vom Namen aus.
   * Wechseln Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Umbenennen]**. Der Name des Assets wird hervorgehoben. Geben Sie einen neuen Namen ein und drücken Sie **[!UICONTROL Enter]**. Vergewissern Sie sich, dass Sie nicht den Namen eines vorhandenen Adobe Dynamic Media Classic-Assets eingeben.

## Löschen von Assets {#delete-assets}

Sie können ausgewählte Assets im Bedienfeld &quot;Durchsuchen&quot;löschen und ganze Ordner löschen. Gelöschte Assets und Ordner werden in den Ordner „Papierkorb“ verschoben und nach sieben Tagen endgültig gelöscht.

Wenn Sie ein Asset gelöscht haben, werden auch alle daraus abgeleiteten Assets gelöscht. Wenn Sie beispielsweise ein Bild löschen, für das Sie Zoomziele erstellt haben, werden die Zoomziele zusammen mit dem Bild gelöscht.

Zoomziele, Bildattribute und Verlaufseinträge werden endgültig gelöscht, wenn Sie die zugehörigen Assets löschen. Die Elemente werden nicht zusammen mit den Assets in den Ordner „Papierkorb“ verschoben, sie können daher auch nicht wiederhergestellt werden.

>[!IMPORTANT]
>
>Die Massenlöschung ist ein intensiver Vorgang. Stellen Sie sicher, dass Sie Massenlöschungen sequenziell anstatt als gleichzeitige, schwere Löschvorgänge ausführen. Adobe empfiehlt, Löschvorgänge auf 5000 oder weniger Asset-Löschungen pro Stunde zu beschränken. Jede Zahl, die größer als 5.000 pro Stunde ist, kann zu einer Ratenbegrenzung führen.

**Löschen von Assets:**

1. Führen Sie einen der folgenden Schritte aus:

   * Um ein oder mehrere Assets zu löschen, wählen Sie die Assets im Bedienfeld &quot;Durchsuchen&quot;aus und drücken Sie die Taste &quot;**[!UICONTROL Löschen]**&quot;oder wechseln Sie zu &quot;**[!UICONTROL Datei]**&quot;> &quot;**[!UICONTROL Löschen]**&quot;.
   * Um einen Ordner zu löschen, wählen Sie den Ordner in der Asset-Bibliothek aus und klicken Sie auf **[!UICONTROL Ordner entfernen]**.

     Beim Löschen eines Ordners werden der Ordner, alle Assets im Ordner und alle Assets in den zugehörigen Unterordnern gelöscht.

Adobe Dynamic Media Classic empfiehlt, Asset-Dateien zu überschreiben, anstatt sie zu löschen, wenn der Grund für das Löschen einer Asset-Datei darin besteht, sie durch andere Dateien mit demselben Namen zu ersetzen.

## Löschen mehrerer Assets mithilfe einer Textdatei {#delete-multiple-assets-with-a-text-file}

Um viele Assets gleichzeitig in der Asset-Bibliothek zu löschen, können Sie die Assets, die Sie löschen möchten, in einer Textdatei auflisten und die Liste an Adobe Dynamic Media Classic senden.

Erstellen Sie die Liste der Adobe Dynamic Media Classic IDs und speichern Sie sie als Textdatei (.txt). Jede Adobe Dynamic Media Classic-ID muss sich in einer eigenen Zeile befinden (gefolgt von einem Hard Return).

Wenn Sie mit dem Erstellen der Liste fertig sind, führen Sie die folgenden Schritte aus, um die Assets zu löschen:

1. Wechseln Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Asset-Liste löschen]**.
1. Geben Sie im Dialogfeld **[!UICONTROL Liste mit gelöschten Assets]** den Pfad zur Textdatei mit der Liste der Assets ein, die Sie löschen möchten.
1. Wählen Sie **[!UICONTROL Löschen]** aus.

Wenn Sie Assets mit einer Textdatei löschen und keine Adobe Dynamic Media Classic-ID auf der Liste steht, wird die Meldung &quot;Diese Einträge in Ihrer Liste können nicht überprüft werden:&quot;angezeigt. Die Liste der Einträge wird ebenfalls angezeigt. Adobe Dynamic Media Classic generiert jedoch keinen Fehler auf der Auftragsseite.

>[!MORELIKETHIS]
>
>* [Assets im Bedienfeld &quot;Durchsuchen&quot;auswählen](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Vorbereiten Ihrer Assets und Ordner auf das Hochladen](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Wiederherstellen von Assets aus dem Ordner &quot;Papierkorb&quot;](trash-folder.md#restoring_assets_from_the_trash_folder)
