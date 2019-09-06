---
title: Verschieben, Umbenennen und Löschen von Assets
seo-title: Verschieben, Umbenennen und Löschen von Assets
description: 'null'
seo-description: Erfahren Sie, wie Sie Assets verschieben, umbenennen und löschen.
uuid: deff 6521-0 ad 0-4 db 9-b 4 e 0-e 3211 ff 97740
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/managing_ assets
discoiquuid: 1 c 9 e 29 f 0-3083-4 d 22-a 439-2 a 01 faf 59683
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Verschieben, Umbenennen und Löschen von Assets{#moving-renaming-and-deleting-assets}

Sie können Assets über das Durchsuchenbedienfeld verschieben, umbenennen und löschen. Außerdem können Sie mithilfe einer Textdatei viele Assets auf einmal löschen.

## Verschieben von Assets {#move-assets}

Sie können Assets über das Durchsuchenbedienfeld in andere Ordner verschieben.

1. Wählen Sie im Durchsuchenbedienfeld die gewünschten Assets aus und führen Sie dann einen der folgenden Schritte durch:

   * Zeigen Sie den Ordner, in den Sie die Assets verschieben möchten, in der Asset-Bibliothek an und ziehen Sie dann die Assets in den Ordner.
   * Sie können auch auf „Datei“ &gt; „Verschieben“ klicken, im Fenster „Assets verschieben“ einen Ordner auswählen und dann auf „Verschieben“ klicken.

## Umbenennen von Assets {#rename-assets}

So benennen Sie ein Asset um

1. Wählen Sie im Durchsuchenbedienfeld das Asset aus und führen Sie dann einen der folgenden Schritte durch:

   * Wählen Sie den Namen aus, geben Sie den neuen Namen ein und drücken Sie die Eingabetaste oder klicken Sie auf eine andere Stelle.
   * Wählen Sie „Datei“ &gt; „Umbenennen“. Der Name des Assets wird hervorgehoben. Geben Sie einen neuen Namen ein und drücken Sie die Eingabetaste.

Geben Sie nicht den Namen eines bereits im Scene7 Publishing System bestehenden Assets ein.

## Löschen von Assets {#delete-assets}

Sie können im Durchsuchenbedienfeld ausgewählte Assets oder auch ganze Ordner löschen. Gelöschte Assets und Ordner werden in den Ordner „Papierkorb“ verschoben und nach sieben Tagen endgültig gelöscht.

Wenn Sie ein Asset löschen, werden auch alle davon abgeleiteten Assets gelöscht. Beim Löschen eines Bildes, für das Sie Zoomziele erstellt haben, werden beispielsweise auch die Zoomziele gelöscht.

>[!NOTE]
>
>Zoomziele, Bildattribute und Verlaufseinträge werden endgültig gelöscht, wenn Sie die zugehörigen Assets löschen. Die Elemente werden nicht zusammen mit den Assets in den Ordner „Papierkorb“ verschoben, sie können daher auch nicht wiederhergestellt werden.

1. Führen Sie einen der folgenden Schritte aus:

   * Um ein oder mehrere Assets zu löschen, wählen Sie die Assets im Durchsuchenbedienfeld aus und drücken die Entf-Taste oder wählen „Datei“ &gt; „Löschen“.
   * To delete a folder, select the folder in the Asset Library, and click **Remove Folder**.

      Beim Löschen werden die Ordner selbst sowie alle darin (auch in Unterordnern) enthaltenen Assets gelöscht.

>[!NOTE]
>
>Dynamic Media Classic empfiehlt, Asset-Dateien zu überschreiben, anstatt sie zu löschen, wenn Sie den Grund für das Löschen einer Asset-Datei durch denselben Namen ersetzen möchten.

## Löschen mehrerer Assets mithilfe einer Textdatei {#delete-multiple-assets-with-a-text-file}

Um viele Assets auf einmal in der Asset-Bibliothek zu löschen, können Sie die zu löschenden Assets in einer Textdatei auflisten und die Liste an dynamisches Media Classic senden.

Erstellen Sie die Liste der Scene7 Publishing System-IDs und speichern Sie sie als Textdatei (.txt). Die einzelnen Scene7 Publishing System-IDs müssen jeweils in einer eigenen Zeile (gefolgt von einem Zeilenumbruch) stehen.

Wenn Sie mit dem Erstellen der Liste fertig sind, führen Sie die folgenden Schritte aus, um die Assets zu löschen:

1. Wählen Sie „Datei“ &gt; „Asset-Liste löschen“.
1. Gehen Sie im Dialogfeld „Asset-Liste löschen“ zu der Textdatei, die die Liste der zu löschenden Assets enthält, oder geben Sie den Pfad zu dieser Datei ein.
1. Klicken Sie auf die Schaltfläche „Löschen“.

Wenn Sie Assets mit einer Textdatei löschen und eine Scene 7 Publishing System-ID nicht in der Liste enthalten ist, wird eine Meldung angezeigt, dass Dynamisches Media Classic "Folgende Einträge in Ihrer Liste nicht validieren kann: " zusammen mit der Liste der Einträge. Im Anzeigebereich "Auftrag" wird jedoch von Dynamic Media Classic kein Fehler ausgegeben.

>[!MORELIKETHIS]
>
>* [Auswählen von Assets im Durchsuchenbedienfeld](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [Vorbereiten von Assets und Ordnern zum Hochladen](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [Wiederherstellen von Assets aus dem Ordner „Papierkorb“](trash-folder.md#restoring_assets_from_the_trash_folder)

