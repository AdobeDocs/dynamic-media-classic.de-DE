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

Sie können Assets im Durchsuchen-Bedienfeld verschieben, umbenennen und löschen. Außerdem können Sie mithilfe einer Textdatei viele Assets auf einmal löschen.

## Verschieben von Assets {#move-assets}

Sie können Assets in verschiedene Ordner im Durchsuchen-Panel verschieben.

**So verschieben Sie Assets:**

1. Wählen Sie das Asset bzw. die Assets im Durchsuchen-Bedienfeld aus und führen Sie einen der folgenden Schritte aus:

   * Zeigen Sie den Ordner an, in den Sie die Assets verschieben möchten, und ziehen Sie die Assets in den Ordner.
   * Wechseln Sie **[!UICONTROL Datei]** > **[!UICONTROL Verschieben]**, wählen Sie im Fenster Assets verschieben einen Ordner aus und klicken Sie auf **[!UICONTROL Verschieben]**.

## Umbenennen von Assets {#rename-assets}

1. Wählen Sie das Asset im Durchsuchen-Bedienfeld aus und führen Sie einen der folgenden Schritte aus:

   * Wählen Sie den Namen aus, geben Sie einen neuen Namen ein und drücken Sie **[!UICONTROL Eingabetaste]** oder wählen Sie einen anderen Namen aus.
   * Navigieren Sie **[!UICONTROL Datei]** > **[!UICONTROL Umbenennen]**. Der Name des Assets wird hervorgehoben. Geben Sie einen neuen Namen ein und drücken Sie **[!UICONTROL Eingabetaste]**. Vergewissern Sie sich, dass Sie den Namen eines bestehenden Adobe Dynamic Media Classic-Assets nicht eingeben.

## Löschen von Assets {#delete-assets}

Sie können ausgewählte Assets im Durchsuchen-Bedienfeld löschen und ganze Ordner löschen. Gelöschte Assets und Ordner werden in den Ordner „Papierkorb“ verschoben und nach sieben Tagen endgültig gelöscht.

Wenn Sie ein Asset gelöscht haben, werden auch alle davon abgeleiteten Assets gelöscht. Wenn Sie beispielsweise ein Bild löschen, für das Sie Zoom-Ziele erstellt haben, werden die Zoom-Ziele zusammen mit dem Bild gelöscht.

Zoomziele, Bildattribute und Verlaufseinträge werden endgültig gelöscht, wenn Sie die zugehörigen Assets löschen. Die Elemente werden nicht zusammen mit den Assets in den Ordner „Papierkorb“ verschoben, sie können daher auch nicht wiederhergestellt werden.

>[!IMPORTANT]
>
>Das Massenlöschen ist ein aufwändiger Vorgang. Stellen Sie sicher, dass Sie Massenlöschungen sequenziell und nicht als gleichzeitige, umfangreiche Löschvorgänge ausführen. Adobe empfiehlt, Löschvorgänge auf maximal 5.000 Asset-Löschvorgänge pro Stunde zu beschränken. Jede Zahl über 5000 pro Stunde kann zu einer Ratenbegrenzung führen.

**So löschen Sie Assets:**

1. Führen Sie einen der folgenden Schritte aus:

   * Um ein oder mehrere Assets zu löschen, wählen Sie die Assets im Durchsuchen-Panel aus und drücken Sie **[!UICONTROL Löschen]** oder gehen Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]**.
   * Um einen Ordner zu löschen, wählen Sie den Ordner in der Asset-Bibliothek aus und klicken Sie auf **[!UICONTROL Ordner entfernen]**.

     Beim Löschen eines Ordners werden der Ordner, alle Assets im Ordner und alle Assets in den Unterordnern gelöscht.

Adobe Dynamic Media Classic empfiehlt, Asset-Dateien zu überschreiben, anstatt sie zu löschen, wenn der Grund für das Löschen einer Asset-Datei darin besteht, sie durch eine andere mit demselben Namen zu ersetzen.

## Löschen mehrerer Assets mithilfe einer Textdatei {#delete-multiple-assets-with-a-text-file}

Wenn Sie mehrere Assets gleichzeitig in der Asset-Bibliothek löschen möchten, können Sie die zu löschenden Assets in einer Textdatei auflisten und die Liste an Adobe Dynamic Media Classic senden.

Erstellen Sie die Liste der Adobe Dynamic Media Classic-IDs und speichern Sie sie als Textdatei (.txt). Jede Adobe Dynamic Media Classic-ID muss sich in einer eigenen Zeile befinden (gefolgt von einer harten Rückgabe).

Wenn Sie mit dem Erstellen der Liste fertig sind, führen Sie die folgenden Schritte aus, um die Assets zu löschen:

1. Navigieren Sie **[!UICONTROL Datei]** > **[!UICONTROL Asset-Liste löschen]**.
1. Geben **[!UICONTROL im Dialogfeld Liste gelöschter Assets]** den Pfad zur Textdatei mit der Liste der Assets ein, die Sie löschen möchten.
1. Wählen Sie **[!UICONTROL Löschen]** aus.

Wenn Sie Assets mit einer Textdatei löschen und sich keine Adobe Dynamic Media Classic-ID in der Liste befindet, wird die Meldung „Diese Einträge in Ihrer Liste können nicht validiert werden:“ angezeigt. Die Liste der Einträge wird ebenfalls angezeigt. Adobe Dynamic Media Classic erzeugt jedoch keinen Fehler auf der Auftragsseite.

>[!MORELIKETHIS]
>
>* [Auswählen von Assets im Durchsuchen-Panel](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Bereiten Sie Ihre Assets und Ordner für das Hochladen vor](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Stellen Sie Assets aus dem Papierkorb-Ordner wieder her](trash-folder.md#restoring_assets_from_the_trash_folder)
