---
title: Schriftarten
seo-title: Schriftarten
description: 'null'
seo-description: Hier erfahren Sie, wie Sie Schriftarten in Dynamic Media Classic verwenden.
uuid: bddec 9 c 2-8530-4 bbd -8 db 7-1562 a 347 e 482
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/support_ files
discoiquuid: 97 cecd 6 a -30 aa -44 fe-a 611-fd 71 b 02 fd 5 ae
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Schriftarten{#fonts}

In einigen Fällen werden Sie vom Scene7 Publishing System aufgefordert, eine Schriftartdatei hochzuladen, damit Text in einer bestimmten Schriftart eingegeben oder dargestellt werden kann. Wenn Sie beispielsweise eine bestimmte Schriftart für Text auf einer Vorlagenebene verwenden möchten, laden Sie die entsprechende Schriftartdatei hoch. Wenn die Seitenzahlen des E-Katalog-Viewers in einer bestimmten Schriftart angezeigt werden sollen, laden Sie die entsprechende Schriftartdatei hoch.

Dynamic Media Classic unterstützt folgende Schriftarten:

* Alle TrueType-Schriftarten
* Postscript®-Schriftarten
* OpenType/TrueType-Schriftarten
* OpenType/PostScript-Schriftarten
* PhotoFonts

Nachdem eine Schriftartdatei hochgeladen wurde, können Sie im Anzeigebereich „Informationen bearbeiten“ deren SPS-ID, Schriftartnamen und Typdaten ändern.

>[!NOTE]
>
>Dynamic Media Classic empfiehlt, alle Schriftschnitte (fett, kursiv, fett/kursiv und normal) hochzuladen, wenn Sie Schriftarten in Vorlagenebenen verwenden möchten. Dynamic Media Classic benötigt diese Schriftschnitte zum Verarbeiten von Anforderungen. Es ist außerdem zu empfehlen, alle PostScript-/Adobe-Type 1-Dateien, die einer Schriftart zugeordnet sind, hochzuladen, weil einige dieser Schriftarten detaillierte Kerning-Daten enthalten.

## Hochladen von Schriftartdateien {#uploading-font-files}

Schriftartdateien werden genau so wie andere Dateien hochgeladen. Sie können Schriftartdateien in einem beliebigen SPS-Ordner speichern. Siehe [Hochladen der Dateien](uploading-files.md#uploading_your_files).

## Bearbeiten von Schriftartdateidaten {#editing-font-file-information}

Sie können den ID-Namen einer Schriftart sowie deren Typdaten ändern. Die Bearbeitung einer Schriftartdatei kann für Suchvorgänge hilfreich sein und das Auffinden von Schriftarten erleichtern.

Wählen Sie die zu bearbeitende Schriftartdatei in der Detailansicht des Durchsuchenbedienfelds und wählen Sie „Datei“ &gt; „Informationen bearbeiten“. Der Anzeigebereich „Informationen bearbeiten“ wird angezeigt. Wählen Sie die folgenden Optionen und klicken Sie anschließend auf „Absenden“.

**Schriftname** Dieser Name identifiziert die Schriftart, wenn sie veröffentlicht wird.

**Postscript Name** Dieser Name ist der vollständige postscript-Name für die Schriftart. Er gibt normalerweise auch die Stärke und den Schnitt der Schriftart an.

**RTF-Name** Dieser Name wird in einem Popupmenü des RTF-Editors angezeigt, in dem Textebenen der Vorlagentypen erstellt werden.

**Name der Schriftfamilie** : Dieser Name listet den Schriftnamen ohne den Stil, die Gewichtung oder den Schriftarttyp auf.

**Schriftschnitt** Die Optionen sind Einfach, Fett, Kursiv und Fett-Kursiv.

**Schriftart** Die Optionen sind truetype und Adobe Type 1. Wenn Sie diese Schriftarten mit einem anderen Namen bezeichnen, können Sie diesen eingeben.

**Abkürzung für Schriftart** Die Optionen lauten wie folgt:

**TTF** truetype-Schriftartdateien, die für das Rendering und Image Serving von PDF/postscript-Schriftarten verwendet werden.

**AFM** Adobe postscript-Schriftartdateien, die Adobe Font Metrics-Informationen enthalten und für das Image Serving verwendet werden.

**PFM** Adobe postscript-Schriftartdateien, die binäre Schriftartmetrikinformationen enthalten.

**PFB** Adobe postscript-Schriftartdateien, die binäre Informationen zur Schriftartkontur enthalten und für das Rendering und Image Serving von PDF/postscript verwendet werden.
