---
title: Schriftarten
description: Erfahren Sie, wie Sie Schriftarten in Adobe Dynamic Media Classic verwenden.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 23%

---

# Schriftarten{#fonts}

Manchmal erfordert Adobe Dynamic Media Classic das Hochladen einer Schriftartdatei, um Text in einer bestimmten Schriftart einzugeben oder zu rendern. Wenn Sie beispielsweise eine bestimmte Schriftart für Text auf einer Vorlagenebene verwenden möchten, laden Sie die entsprechende Schriftartdatei hoch. Wenn die Seitenzahlen des E-Katalog-Viewers in einer bestimmten Schriftart angezeigt werden sollen, laden Sie die entsprechende Schriftartdatei hoch.

Adobe Dynamic Media Classic unterstützt die folgenden Schriftarten:

* Alle TrueType-Schriftarten
* PostScript®-Schriftarten
* OpenType/TrueType-Schriftarten
* OpenType/PostScript-Schriftarten
* PhotoFonts

Nachdem eine Schriftartendatei hochgeladen wurde, können Sie ihre Adobe Dynamic Media Classic-ID, ihren Schriftnamen und die Eingabeinformationen auf dem Bildschirm „Info bearbeiten“ ändern.

>[!NOTE]
>
>Adobe Dynamic Media Classic empfiehlt, alle Schriftarten (fett, kursiv, fett/kursiv und normal) hochzuladen, wenn Sie Schriftarten in Vorlagenebenen verwenden möchten. Adobe Dynamic Media Classic benötigt diese Schriftstile, um Anfragen zu verarbeiten. Das Hochladen aller `PostScript/Adobe Type1` einer Schriftart zugeordneten Dateien wird ebenfalls empfohlen, da einige dieser Schriftarten detaillierte Kerning-Informationen enthalten.

## Hochladen von Schriftartendateien {#uploading-font-files}

Schriftartdateien werden genau so wie andere Dateien hochgeladen. Sie können Schriftarten in einem beliebigen Adobe Dynamic Media Classic-Ordner speichern. Siehe [Hochladen der Dateien](uploading-files.md#uploading_your_files).

## Schriftartendateiinformationen bearbeiten {#editing-font-file-information}

Sie können den ID-Namen einer Schriftart und ihre Typinformationen ändern. Die Bearbeitung einer Schriftartdatei kann für Suchvorgänge hilfreich sein und das Auffinden von Schriftarten erleichtern.

Wählen Sie im Durchsuchen-Panel die Schriftartdatei aus, die Sie in der Detailansicht bearbeiten möchten, und wählen Sie „Datei“ > „Informationen bearbeiten“. Der Anzeigebereich „Informationen bearbeiten“ wird angezeigt. Wählen Sie die folgenden Optionen aus und klicken Sie dann auf **[!UICONTROL Senden]**.

* **[!UICONTROL Schriftname]**: Dieser Name identifiziert die Schriftart bei der Veröffentlichung.

* **[!UICONTROL PostScript-Name]**: Dieser Name ist der vollständige PostScript-Name für die Schriftart. Er gibt normalerweise auch die Stärke und den Schnitt der Schriftart an.

* **[!UICONTROL RTF-Name]**: Dieser Name wird in einem Popup-Menü im RTF-Editor angezeigt, in dem Vorlagentextebenen erstellt werden.

* **[!UICONTROL Schriftfamilienname]**: Dieser Name listet den Schriftnamen ohne die Anzeige für Stil, Gewichtung oder Schrifttyp auf.

* **[!UICONTROL Schriftstil]**: Die Optionen sind Normal, Fett, Kursiv und Fett-Kursiv.

* **[!UICONTROL Font Type]**: Die Optionen sind TrueType und Adobe Type 1. Wenn Sie diese Schriftarten mit einem anderen Namen bezeichnen, können Sie diesen eingeben.

* **[!UICONTROL Schriftartabkürzung]**: Folgende Optionen stehen zur Verfügung:

   * **[!UICONTROL TTF]**: TrueType-Schriftartdateien für das PDF/PostScript-Rendering und die Bildbereitstellung.

   * **[!UICONTROL AFM]**: Adobe PostScript-Schriftartdateien, die Informationen zu Adobe-Schriftartmetriken enthalten und für die Bildbereitstellung verwendet werden.

   * **[!UICONTROL PFM]**: Adobe PostScript-Schriftarten-Dateien, die Informationen zur Metrik der binären Schriftarten enthalten.

   * **[!UICONTROL PFB]**: Adobe PostScript-Schriftdateien, die binäre Schriftkonturinformationen enthalten und für das PDF/PostScript-Rendering und die Bildbereitstellung verwendet werden.
