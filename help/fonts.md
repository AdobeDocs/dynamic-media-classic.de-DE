---
title: Schriftarten
seo-title: Schriftarten
description: 'null'
seo-description: Erfahren Sie, wie Sie Schriftarten in Dynamic Media Classic verwenden.
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 40%

---


# Schriftarten{#fonts}

In einigen Fällen erfordert Dynamic Media Classic das Hochladen einer Schriftartdatei, um Text in einer bestimmten Schriftart einzugeben oder wiederzugeben. Wenn Sie beispielsweise eine bestimmte Schriftart für Text auf einer Vorlagenebene verwenden möchten, laden Sie die entsprechende Schriftartdatei hoch. Wenn die Seitenzahlen des E-Katalog-Viewers in einer bestimmten Schriftart angezeigt werden sollen, laden Sie die entsprechende Schriftartdatei hoch.

Dynamic Media Classic unterstützt die folgenden Schriftarten:

* Alle TrueType-Schriftarten
* PostScript® Schriftarten
* OpenType/TrueType-Schriftarten
* OpenType/PostScript-Schriftarten
* PhotoFonts

Nachdem eine Schriftartdatei hochgeladen wurde, können Sie die zugehörige Dynamic Media Classic-ID, den Schriftartnamen und die Typinformationen im Anzeigebereich &quot;Informationen bearbeiten&quot;ändern.

>[!NOTE]
>
>Dynamic Media Classic empfiehlt das Hochladen aller Schriftschnitte (fett, kursiv, fett/kursiv und normal), wenn Sie Schriftarten in Vorlagenebenen verwenden möchten. Für die Verarbeitung von Anforderungen benötigt Dynamic Media Classic diese Schriftschnitte. Es ist außerdem zu empfehlen, alle PostScript-/Adobe-Type 1-Dateien, die einer Schriftart zugeordnet sind, hochzuladen, weil einige dieser Schriftarten detaillierte Kerning-Daten enthalten.

## Hochladen von Schriftartdateien {#uploading-font-files}

Schriftartdateien werden genau so wie andere Dateien hochgeladen. Sie können Schriftartdateien in jedem Ordner von Dynamic Media Classic speichern. Siehe [Hochladen der Dateien](uploading-files.md#uploading_your_files).

## Bearbeiten von Schriftartdateidaten {#editing-font-file-information}

Sie können den ID-Namen einer Schriftart sowie deren Typdaten ändern. Die Bearbeitung einer Schriftartdatei kann für Suchvorgänge hilfreich sein und das Auffinden von Schriftarten erleichtern.

Wählen Sie die zu bearbeitende Schriftartdatei in der Detailansicht des Durchsuchenbedienfelds und wählen Sie „Datei“ > „Informationen bearbeiten“. Der Anzeigebereich „Informationen bearbeiten“ wird angezeigt. Wählen Sie die folgenden Optionen und klicken Sie anschließend auf „Absenden“.

**Schriftname** Dieser Name gibt die Schriftart an, wenn sie veröffentlicht wird.

**PostScript-Name** Dieser Name ist der vollständige PostScript-Name für die Schriftart. Er gibt normalerweise auch die Stärke und den Schnitt der Schriftart an.

**RTF-Name** Dieser Name wird in einem Popupmenü im RTF-Editor angezeigt, in dem Vorlagentextebenen erstellt werden.

**Name** der Schriftfamilie Dieser Name Liste den Schriftartnamen ohne Angabe von Stil, Gewichtung oder Schriftart.

**Schriftschnitt** Die Optionen sind &quot;Klein&quot;, &quot;Fett&quot;, &quot;Kursiv&quot;und &quot;Fett-Kursiv&quot;.

**Schriftart** Die Optionen sind TrueType und Adobe Type 1. Wenn Sie diese Schriftarten mit einem anderen Namen bezeichnen, können Sie diesen eingeben.

**Schriftartabkürzung** Die Optionen lauten wie folgt:

**TTF** TrueType-Schriftartdateien, die für das Rendern und Image Serving von PDF/PostScript verwendet werden.

**AFM** Adobe PostScript-Schriftartdateien, die Adobe-Schriftmetriken enthalten und für die Image Serving verwendet werden.

**PFM** -Adobe PostScript-Schriftartdateien, die Informationen zur binären Schriftartmetrik enthalten.

**PFB** -Adobe PostScript-Schriftartdateien, die binäre Schriftartkonturinformationen enthalten und zum Rendern und Bereitstellen von Bildern in PDF/PostScript verwendet werden.
