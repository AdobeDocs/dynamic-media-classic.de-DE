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
role: Geschäftspraktiker
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 39%

---


# Schriftarten{#fonts}

In einigen Fällen erfordert Dynamic Media Classic das Hochladen einer Schriftartdatei, um Text in einer bestimmten Schriftart einzugeben oder wiederzugeben. Wenn Sie beispielsweise eine bestimmte Schriftart für Text auf einer Vorlagenebene verwenden möchten, laden Sie die entsprechende Schriftartdatei hoch. Wenn die Seitenzahlen des E-Katalog-Viewers in einer bestimmten Schriftart angezeigt werden sollen, laden Sie die entsprechende Schriftartdatei hoch.

Dynamic Media Classic unterstützt die folgenden Schriftarten:

* Alle TrueType-Schriftarten
* PostScript® Schriftarten
* OpenType/TrueType-Schriftarten
* OpenType/PostScript-Schriftarten
* PhotoFonts

Nachdem eine Schriftartdatei hochgeladen wurde, können Sie die zugehörige Dynamic Media Classic-ID, den Schriftartnamen und die Typinformationen im Bildschirm &quot;Informationen bearbeiten&quot;ändern.

>[!NOTE]
>
>Dynamic Media Classic empfiehlt, alle Schriftschnitte (fett, kursiv, fett/kursiv und normal) hochzuladen, wenn Sie Schriftarten in Vorlagenebenen verwenden möchten. Dynamic Media Classic benötigt diese Schriftschnitte, um Anforderungen zu verarbeiten. Es ist außerdem zu empfehlen, alle PostScript-/Adobe-Type 1-Dateien, die einer Schriftart zugeordnet sind, hochzuladen, weil einige dieser Schriftarten detaillierte Kerning-Daten enthalten.

## Hochladen von Schriftartdateien  {#uploading-font-files}

Schriftartdateien werden genau so wie andere Dateien hochgeladen. Sie können Schriftartdateien in einem beliebigen Dynamic Media Classic-Ordner speichern. Siehe [Hochladen der Dateien](uploading-files.md#uploading_your_files).

## Bearbeiten von Schriftartdateidaten  {#editing-font-file-information}

Sie können den ID-Namen einer Schriftart sowie deren Typdaten ändern. Die Bearbeitung einer Schriftartdatei kann für Suchvorgänge hilfreich sein und das Auffinden von Schriftarten erleichtern.

Wählen Sie die zu bearbeitende Schriftartdatei in der Detailansicht des Durchsuchenbedienfelds und wählen Sie „Datei“ > „Informationen bearbeiten“. Der Anzeigebereich „Informationen bearbeiten“ wird angezeigt. Wählen Sie die folgenden Optionen und klicken Sie anschließend auf „Absenden“.

**Schriftname:** Dieser Name gibt die Schriftart an, wenn sie veröffentlicht wird.

**PostScript-** NameDieser Name ist der vollständige PostScript-Name für die Schriftart. Er gibt normalerweise auch die Stärke und den Schnitt der Schriftart an.

**RTF-** NameDieser Name wird in einem Popupmenü im RTF-Editor angezeigt, in dem Vorlagentextebenen erstellt werden.

**Name der Schriftfamilie** Dieser Name Liste den Schriftartnamen ohne Angabe von Stil, Gewichtung oder Schriftart.

**SchriftschnittDie** Optionen sind &quot;Klein&quot;, &quot;Fett&quot;, &quot;Kursiv&quot;und &quot;Fett-Kursiv&quot;.

**Schriftart** Die Optionen sind TrueType und Adobe Type 1. Wenn Sie diese Schriftarten mit einem anderen Namen bezeichnen, können Sie diesen eingeben.

**Schriftart** AbkürzungDie Optionen lauten wie folgt:

**** TTFTrueType-Schriftartdateien, die für das Rendern und Image Serving von PDF/PostScript verwendet werden.

**** AFMAdobe PostScript-Schriftartdateien, die Adobe Font Metrics Informationen enthalten und für die Image Serving verwendet werden.

**** PFMAdobe PostScript-Schriftartdateien, die Informationen zur binären Schriftartmetrik enthalten.

**** PFBAdobe PostScript-Schriftartdateien, die binäre Schriftartkonturinformationen enthalten und für das Rendern und Image Serving von PDF/PostScript verwendet werden.
