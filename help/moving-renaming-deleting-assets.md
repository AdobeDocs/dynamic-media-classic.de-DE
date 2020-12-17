---
title: Verschieben, Umbenennen und Löschen von Assets
seo-title: Verschieben, Umbenennen und Löschen von Assets
description: 'null'
seo-description: Erfahren Sie, wie Sie Assets verschieben, umbenennen und löschen.
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 66%

---


# Verschieben, Umbenennen und Löschen von Assets{#moving-renaming-and-deleting-assets}

Sie können Assets über das Durchsuchenbedienfeld verschieben, umbenennen und löschen. Außerdem können Sie mithilfe einer Textdatei viele Assets auf einmal löschen.

## Verschieben von Assets {#move-assets}

Sie können Assets über das Durchsuchenbedienfeld in andere Ordner verschieben.

1. Wählen Sie im Durchsuchenbedienfeld die gewünschten Assets aus und führen Sie dann einen der folgenden Schritte durch:

   * Zeigen Sie den Ordner, in den Sie die Assets verschieben möchten, in der Asset-Bibliothek an und ziehen Sie dann die Assets in den Ordner.
   * Sie können auch auf „Datei“ > „Verschieben“ klicken, im Fenster „Assets verschieben“ einen Ordner auswählen und dann auf „Verschieben“ klicken.

## Umbenennen von Assets  {#rename-assets}

So benennen Sie ein Asset um

1. Wählen Sie im Durchsuchenbedienfeld das Asset aus und führen Sie dann einen der folgenden Schritte durch:

   * Wählen Sie den Namen aus, geben Sie den neuen Namen ein und drücken Sie die Eingabetaste oder klicken Sie auf eine andere Stelle.
   * Wählen Sie „Datei“ > „Umbenennen“. Der Name des Assets wird hervorgehoben. Geben Sie einen neuen Namen ein und drücken Sie die Eingabetaste.

Vergewissern Sie sich, dass Sie nicht den Namen eines vorhandenen Dynamic Media Classic-Assets eingeben.

## Löschen von Assets {#delete-assets}

Sie können im Durchsuchenbedienfeld ausgewählte Assets oder auch ganze Ordner löschen. Gelöschte Assets und Ordner werden in den Ordner „Papierkorb“ verschoben und nach sieben Tagen endgültig gelöscht.

Wenn Sie ein Asset löschen, werden auch alle davon abgeleiteten Assets gelöscht. Beim Löschen eines Bildes, für das Sie Zoomziele erstellt haben, werden beispielsweise auch die Zoomziele gelöscht.

>[!NOTE]
>
>Zoomziele, Bildattribute und Verlaufseinträge werden endgültig gelöscht, wenn Sie die zugehörigen Assets löschen. Die Elemente werden nicht zusammen mit den Assets in den Ordner „Papierkorb“ verschoben, sie können daher auch nicht wiederhergestellt werden.

1. Führen Sie einen der folgenden Schritte aus:

   * Um ein oder mehrere Assets zu löschen, wählen Sie die Assets im Durchsuchenbedienfeld aus und drücken die Entf-Taste oder wählen „Datei“ > „Löschen“.
   * Um einen Ordner zu löschen, wählen Sie ihn in der Asset-Bibliothek aus und klicken Sie auf **Ordner entfernen**.

      Beim Löschen werden die Ordner selbst sowie alle darin (auch in Unterordnern) enthaltenen Assets gelöscht.

>[!NOTE]
>
>Dynamic Media Classic empfiehlt, Asset-Dateien zu überschreiben, anstatt sie zu löschen, wenn der Grund für das Löschen einer Asset-Datei darin besteht, sie durch eine andere Datei mit demselben Namen zu ersetzen.

## Löschen mehrerer Assets mithilfe einer Textdatei {#delete-multiple-assets-with-a-text-file}

Um viele Assets gleichzeitig in der Asset-Bibliothek zu löschen, können Sie die zu löschenden Assets in einer Textdatei Liste und die Liste an Dynamic Media Classic senden.

Erstellen Sie die Liste der Dynamic Media Classic-IDs und speichern Sie sie als Textdatei (.txt). Jede Dynamic Media Classic-ID muss sich in einer eigenen Zeile befinden (gefolgt von einem Zeilenumbruch).

Wenn Sie mit dem Erstellen der Liste fertig sind, führen Sie die folgenden Schritte aus, um die Assets zu löschen:

1. Wählen Sie „Datei“ > „Asset-Liste löschen“.
1. Gehen Sie im Dialogfeld „Asset-Liste löschen“ zu der Textdatei, die die Liste der zu löschenden Assets enthält, oder geben Sie den Pfad zu dieser Datei ein.
1. Klicken Sie auf die Schaltfläche „Löschen“.

Wenn Sie Assets mit einer Textdatei löschen und keine Dynamic Media Classic-ID auf der Liste vorhanden ist, wird eine Meldung angezeigt, die Sie darauf hinweist, dass Dynamic Media Classic neben der Liste der Einträge die Meldung &quot;Diese Einträge in Ihrer Liste können nicht überprüft werden:&quot;enthält. Dynamic Media Classic erzeugt jedoch keinen Fehler im Anzeigebereich &quot;Auftrag&quot;.

>[!MORELIKETHIS]
>
>* [Auswählen von Assets im Durchsuchenbedienfeld](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Vorbereiten von Assets und Ordnern zum Hochladen](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Wiederherstellen von Assets aus dem Ordner „Papierkorb“](trash-folder.md#restoring_assets_from_the_trash_folder)

