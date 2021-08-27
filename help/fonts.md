---
title: Schriftarten
description: Erfahren Sie, wie Sie Schriftarten in Adobe Dynamic Media Classic verwenden.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 28%

---

# Schriftarten{#fonts}

Manchmal erfordert es Adobe Dynamic Media Classic, dass Sie eine Schriftartdatei hochladen, um Text in einer bestimmten Schriftart einzugeben oder zu rendern. Wenn Sie beispielsweise eine bestimmte Schriftart für Text auf einer Vorlagenebene verwenden möchten, laden Sie die entsprechende Schriftartdatei hoch. Wenn die Seitenzahlen des E-Katalog-Viewers in einer bestimmten Schriftart angezeigt werden sollen, laden Sie die entsprechende Schriftartdatei hoch.

Adobe Dynamic Media Classic unterstützt diese Schrifttypen:

* Alle TrueType-Schriftarten
* PostScript® fonts
* OpenType/TrueType-Schriftarten
* OpenType/PostScript-Schriftarten
* PhotoFonts

Nachdem eine Schriftartdatei hochgeladen wurde, können Sie die Adobe Dynamic Media Classic ID, den Schriftnamen und die Informationen auf dem Bildschirm &quot;Informationen bearbeiten&quot;ändern.

>[!NOTE]
>
>Adobe Dynamic Media Classic empfiehlt das Hochladen aller Schriftstile (fett, kursiv, fett/kursiv und normal), wenn Sie Schriftarten in Vorlagenschichten verwenden möchten. Adobe Dynamic Media Classic benötigt diese Schriftstile, um Anforderungen verarbeiten zu können. Es ist außerdem zu empfehlen, alle PostScript-/Adobe-Type 1-Dateien, die einer Schriftart zugeordnet sind, hochzuladen, weil einige dieser Schriftarten detaillierte Kerning-Daten enthalten.

## Hochladen von Schriftartdateien {#uploading-font-files}

Schriftartdateien werden genau so wie andere Dateien hochgeladen. Sie können Schriftartdateien in jedem beliebigen Adobe Dynamic Media Classic-Ordner speichern. Siehe [Hochladen der Dateien](uploading-files.md#uploading_your_files).

## Informationen zu Schriftartdateien bearbeiten {#editing-font-file-information}

Sie können den ID-Namen einer Schriftart und deren Typinformationen ändern. Die Bearbeitung einer Schriftartdatei kann für Suchvorgänge hilfreich sein und das Auffinden von Schriftarten erleichtern.

Wählen Sie im Durchsuchenbedienfeld in der Detailansicht die Schriftartdatei aus, die Sie bearbeiten möchten, und wählen Sie &quot;Datei&quot;> &quot;Informationen bearbeiten&quot;. Der Anzeigebereich „Informationen bearbeiten“ wird angezeigt. Wählen Sie die folgenden Optionen und dann **[!UICONTROL Submit]** aus.

* **[!UICONTROL Schriftname]**  - Dieser Name gibt die Schriftart bei der Veröffentlichung an.

* **[!UICONTROL PostScript-Name]**  - Dieser Name ist der vollständige PostScript-Name für die Schriftart. Er gibt normalerweise auch die Stärke und den Schnitt der Schriftart an.

* **[!UICONTROL RTF-Name]**  - Dieser Name wird in einem Popup-Menü im RTF-Editor angezeigt, in dem Vorlagen-Textebenen erstellt werden.

* **[!UICONTROL Schriftfamilienname]**  - Dieser Name listet den Schriftnamen ohne Stil-, Gewicht- oder Schriftartanzeige auf.

* **[!UICONTROL Schriftschnitt]**  - Die Optionen sind &quot;Nur&quot;, &quot;Fett&quot;, &quot;Kursiv&quot;und &quot;Fett-Kursiv&quot;.

* **[!UICONTROL Schriftart]**  - Die Optionen sind TrueType und Adobe Type 1. Wenn Sie diese Schriftarten mit einem anderen Namen bezeichnen, können Sie diesen eingeben.

* **[!UICONTROL Schriftartabkürzung]**  - Die Optionen lauten wie folgt:

   * **[!UICONTROL TTF]**  - TrueType-Schriftartendateien, die für die PDF/PostScript-Wiedergabe und Bildbereitstellung verwendet werden.

   * **[!UICONTROL AFM]**  - Adobe PostScript-Schriftartdateien, die Informationen zu Adobe Font Metrics enthalten und für die Bildbereitstellung verwendet werden.

   * **[!UICONTROL PFM]**  - Adobe PostScript-Schriftartdateien, die Informationen zu binären Schriftartmetriken enthalten.

   * **[!UICONTROL PFB]**  - Adobe PostScript-Schriftartdateien, die binäre Schriftartentwurfsinformationen enthalten und zum Rendern und Bereitstellen von PDF/PostScript-Dateien verwendet werden.
