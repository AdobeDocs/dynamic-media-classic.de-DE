---
title: Verschieben, Umbenennen und Löschen von Assets
description: Erfahren Sie, wie Sie Assets in Adobe Dynamic Media Classic verschieben, umbenennen und löschen können.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 37%

---

# Verschieben, Umbenennen und Löschen von Assets{#moving-renaming-and-deleting-assets}

Sie können Assets über das Durchsuchenbedienfeld verschieben, umbenennen und löschen. Außerdem können Sie mithilfe einer Textdatei viele Assets auf einmal löschen.

## Verschieben von Assets {#move-assets}

Sie können Assets über das Durchsuchenbedienfeld in andere Ordner verschieben.

1. Wählen Sie im Durchsuchenbedienfeld die gewünschten Assets aus und führen Sie dann einen der folgenden Schritte durch:

   * Zeigen Sie den Ordner, in den Sie die Assets verschieben möchten, in der Asset-Bibliothek an und ziehen Sie dann die Assets in den Ordner.
   * Gehen Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Verschieben]**, wählen Sie einen Ordner im Fenster &quot;Assets verschieben&quot;aus und wählen Sie **[!UICONTROL Verschieben]** aus.

## Umbenennen von Assets {#rename-assets}

1. Wählen Sie im Durchsuchenbedienfeld das Asset aus und führen Sie dann einen der folgenden Schritte durch:

   * Wählen Sie den Namen aus, geben Sie einen neuen Namen ein und drücken Sie **[!UICONTROL Enter]** oder wählen Sie weg vom Namen aus.
   * Gehen Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Umbenennen]**. Der Name des Assets wird hervorgehoben. Geben Sie einen neuen Namen ein und drücken Sie **[!UICONTROL Enter]**.

Vergewissern Sie sich, dass Sie den Namen eines vorhandenen Adobe Dynamic Media Classic-Assets nicht eingeben.

## Löschen von Assets {#delete-assets}

Sie können ausgewählte Assets im Durchsuchenbedienfeld löschen und ganze Ordner löschen. Gelöschte Assets und Ordner werden in den Ordner „Papierkorb“ verschoben und nach sieben Tagen endgültig gelöscht.

Wenn Sie ein Asset löschen, werden auch alle davon abgeleiteten Assets gelöscht. Beim Löschen eines Bildes, für das Sie Zoomziele erstellt haben, werden beispielsweise auch die Zoomziele gelöscht.

>[!NOTE]
>
>Zoomziele, Bildattribute und Verlaufseinträge werden endgültig gelöscht, wenn Sie die zugehörigen Assets löschen. Die Elemente werden nicht zusammen mit den Assets in den Ordner „Papierkorb“ verschoben, sie können daher auch nicht wiederhergestellt werden.

1. Führen Sie einen der folgenden Schritte aus:

   * Um ein oder mehrere Assets zu löschen, wählen Sie die Assets im Durchsuchenbedienfeld aus und drücken Sie die Taste **[!UICONTROL Löschen]** oder gehen Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]**.
   * Um einen Ordner zu löschen, wählen Sie ihn in der Asset-Bibliothek aus und klicken Sie auf **[!UICONTROL Ordner entfernen]**.

      Beim Löschen eines Ordners werden der Ordner, alle Assets im Ordner und alle Assets in den zugehörigen Unterordnern gelöscht.

>[!NOTE]
>
>Adobe Dynamic Media Classic empfiehlt, Asset-Dateien zu überschreiben, anstatt sie zu löschen, wenn der Grund für das Löschen einer Asset-Datei darin besteht, sie durch eine andere mit demselben Namen zu ersetzen.

## Löschen mehrerer Assets mithilfe einer Textdatei {#delete-multiple-assets-with-a-text-file}

Um viele Assets gleichzeitig in der Asset-Bibliothek zu löschen, können Sie die Assets, die Sie löschen möchten, in einer Textdatei auflisten und die Liste an Adobe Dynamic Media Classic senden.

Erstellen Sie die Liste der Adobe Dynamic Media Classic IDs und speichern Sie sie als Textdatei (.txt). Jede Adobe Dynamic Media Classic-ID muss sich in einer eigenen Zeile befinden (gefolgt von einer festen Rückkehr).

Wenn Sie mit dem Erstellen der Liste fertig sind, führen Sie die folgenden Schritte aus, um die Assets zu löschen:

1. Gehen Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Liste der Assets löschen]**.
1. Suchen Sie im Dialogfeld &quot;Asset-Liste löschen&quot;den Pfad zur Textdatei mit der Liste der Assets, die Sie löschen möchten, oder geben Sie ihn ein.
1. Wählen Sie **[!UICONTROL Löschen]** aus.

Wenn Sie Assets mit einer Textdatei löschen und keine Adobe der Dynamic Media Classic-ID auf der Liste steht, wird die Meldung &quot;Diese Einträge in Ihrer Liste können nicht überprüft werden:&quot;und die Liste der Einträge angezeigt. Adobe Dynamic Media Classic generiert jedoch keinen Fehler auf der Auftragsseite.

>[!MORELIKETHIS]
>
>* [Auswählen von Assets im Bedienfeld &quot;Durchsuchen&quot;](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Vorbereiten der Assets und Ordner auf das Hochladen](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Wiederherstellen von Assets aus dem Ordner &quot;Papierkorb&quot;](trash-folder.md#restoring_assets_from_the_trash_folder)

