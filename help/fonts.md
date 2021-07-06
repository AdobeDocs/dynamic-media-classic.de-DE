---
title: Schriftarten
description: Erfahren Sie, wie Sie Schriftarten in Dynamic Media Classic verwenden.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 36%

---

# Schriftarten{#fonts}

Manchmal erfordert Dynamic Media Classic, dass Sie eine Schriftartdatei hochladen, um Text in einer bestimmten Schriftart einzugeben oder zu rendern. Wenn Sie beispielsweise eine bestimmte Schriftart für Text auf einer Vorlagenebene verwenden möchten, laden Sie die entsprechende Schriftartdatei hoch. Wenn die Seitenzahlen des E-Katalog-Viewers in einer bestimmten Schriftart angezeigt werden sollen, laden Sie die entsprechende Schriftartdatei hoch.

Dynamic Media Classic unterstützt die folgenden Schriftarten:

* Alle TrueType-Schriftarten
* PostScript® fonts
* OpenType/TrueType-Schriftarten
* OpenType/PostScript-Schriftarten
* PhotoFonts

Nachdem eine Schriftartdatei hochgeladen wurde, können Sie die Dynamic Media Classic-ID, den Schriftnamen und die Informationen im Bildschirm &quot;Informationen bearbeiten&quot;ändern.

>[!NOTE]
>
>Dynamic Media Classic empfiehlt das Hochladen aller Schriftstile (fett, kursiv, fett/kursiv und normal), wenn Sie Schriftarten in Vorlagenschichten verwenden möchten. Dynamic Media Classic benötigt diese Schriftstile, um Anforderungen zu verarbeiten. Es ist außerdem zu empfehlen, alle PostScript-/Adobe-Type 1-Dateien, die einer Schriftart zugeordnet sind, hochzuladen, weil einige dieser Schriftarten detaillierte Kerning-Daten enthalten.

## Hochladen von Schriftartdateien {#uploading-font-files}

Schriftartdateien werden genau so wie andere Dateien hochgeladen. Sie können Schriftartdateien in einem beliebigen Dynamic Media Classic-Ordner speichern. Siehe [Hochladen der Dateien](uploading-files.md#uploading_your_files).

## Bearbeiten von Schriftartdateidaten {#editing-font-file-information}

Sie können den ID-Namen einer Schriftart und deren Typinformationen ändern. Die Bearbeitung einer Schriftartdatei kann für Suchvorgänge hilfreich sein und das Auffinden von Schriftarten erleichtern.

Wählen Sie die zu bearbeitende Schriftartdatei in der Detailansicht des Durchsuchenbedienfelds und wählen Sie „Datei“ > „Informationen bearbeiten“. Der Anzeigebereich „Informationen bearbeiten“ wird angezeigt. Wählen Sie die folgenden Optionen und klicken Sie anschließend auf „Absenden“.

* **Schriftname**  - Dieser Name gibt die Schriftart bei der Veröffentlichung an.

* **PostScript-Name**  - Dieser Name ist der vollständige PostScript-Name für die Schriftart. Er gibt normalerweise auch die Stärke und den Schnitt der Schriftart an.

* **RTF-Name**  - Dieser Name wird in einem Popup-Menü im RTF-Editor angezeigt, in dem Vorlagen-Textebenen erstellt werden.

* **Schriftfamilienname**  - Dieser Name listet den Schriftnamen ohne Stil-, Gewicht- oder Schriftartanzeige auf.

* **Schriftschnitt**  - Die Optionen sind &quot;Nur&quot;, &quot;Fett&quot;, &quot;Kursiv&quot;und &quot;Fett-Kursiv&quot;.

* **Schriftart**  - Die Optionen sind TrueType und Adobe Type 1. Wenn Sie diese Schriftarten mit einem anderen Namen bezeichnen, können Sie diesen eingeben.

* **Schriftartabkürzung**  - Die Optionen lauten wie folgt:

   * **** TTFTrueType-Schriftartendateien, die für die PDF/PostScript-Wiedergabe und Bildbereitstellung verwendet werden.

   * **** AFMAdobe PostScript-Schriftartdateien, die Adobe Font Metrics-Informationen enthalten und für die Bildbereitstellung verwendet werden.

   * **** PFMAdobe PostScript-Schriftartdateien, die Informationen zu binären Schriftartmetriken enthalten.

   * **** PFBAdobe PostScript-Schriftartdateien, die binäre Schriftartentwurfsinformationen enthalten und zum Rendern und Image Serving von PDF/PostScript-Dateien verwendet werden.
