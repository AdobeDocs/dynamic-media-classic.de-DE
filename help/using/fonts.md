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

Manchmal erfordert Adobe Dynamic Media Classic, dass Sie eine Schriftartdatei hochladen, um Text in einer bestimmten Schriftart einzugeben oder zu rendern. Wenn Sie beispielsweise eine bestimmte Schriftart für Text auf einer Vorlagenebene verwenden möchten, laden Sie die entsprechende Schriftartdatei hoch. Wenn die Seitenzahlen des E-Katalog-Viewers in einer bestimmten Schriftart angezeigt werden sollen, laden Sie die entsprechende Schriftartdatei hoch.

Adobe Dynamic Media Classic unterstützt diese Schrifttypen:

* Alle TrueType-Schriftarten
* PostScript® fonts
* OpenType/TrueType-Schriftarten
* OpenType/PostScript-Schriftarten
* PhotoFonts

Nachdem eine Schriftartdatei hochgeladen wurde, können Sie die Adobe Dynamic Media Classic-ID und den Schriftartnamen ändern und Informationen auf dem Bildschirm &quot;Informationen bearbeiten&quot;eingeben.

>[!NOTE]
>
>Adobe Dynamic Media Classic empfiehlt das Hochladen aller Schriftstile (fett, kursiv, fett/kursiv und normal), wenn Sie Schriftarten in Vorlagenschichten verwenden möchten. Adobe Dynamic Media Classic benötigt diese Schriftstile, um Anforderungen zu verarbeiten. Das Hochladen aller mit einer Schrift verknüpften `PostScript/Adobe Type1`-Dateien wird ebenfalls empfohlen, da einige dieser Schriftarten detaillierte Kerning-Informationen enthalten.

## Hochladen von Schriftartdateien {#uploading-font-files}

Schriftartdateien werden genau so wie andere Dateien hochgeladen. Sie können Schriftartdateien in einem beliebigen Adobe Dynamic Media Classic-Ordner speichern. Siehe [Hochladen der Dateien](uploading-files.md#uploading_your_files).

## Informationen zu Schriftartdateien bearbeiten {#editing-font-file-information}

Sie können den ID-Namen einer Schriftart und deren Typinformationen ändern. Die Bearbeitung einer Schriftartdatei kann für Suchvorgänge hilfreich sein und das Auffinden von Schriftarten erleichtern.

Wählen Sie im Bedienfeld &quot;Durchsuchen&quot;die Schriftartdatei, die Sie bearbeiten möchten, in der Detailansicht und dann &quot;Datei&quot;> &quot;Informationen bearbeiten&quot;. Der Anzeigebereich „Informationen bearbeiten“ wird angezeigt. Wählen Sie die folgenden Optionen und dann **[!UICONTROL Senden]** aus.

* **[!UICONTROL Schriftname]**: Dieser Name gibt die Schriftart an, wenn sie veröffentlicht wird.

* **[!UICONTROL PostScript-Name]**: Dieser Name ist der vollständige PostScript-Name für die Schriftart. Er gibt normalerweise auch die Stärke und den Schnitt der Schriftart an.

* **[!UICONTROL RTF-Name]**: Dieser Name wird in einem Popup-Menü im RTF-Editor angezeigt, in dem Vorlagen-Textebenen erstellt werden.

* **[!UICONTROL Schriftfamilienname]**: Dieser Name listet den Schriftnamen ohne Stil-, Gewicht- oder Schriftartanzeige auf.

* **[!UICONTROL Schriftstil]**: Die Optionen sind &quot;Nur&quot;, &quot;Fett&quot;, &quot;Kursiv&quot;und &quot;Fett-Kursiv&quot;.

* **[!UICONTROL Schrifttyp]**: Die Optionen sind TrueType und Adobe Type 1. Wenn Sie diese Schriftarten mit einem anderen Namen bezeichnen, können Sie diesen eingeben.

* **[!UICONTROL Schriftartabkürzung]**: Die Optionen lauten wie folgt:

   * **[!UICONTROL TTF]**: TrueType-Schriftartendateien, die für die Wiedergabe und das Image-Serving von PDF/PostScript verwendet werden.

   * **[!UICONTROL AFM]**: Adobe PostScript-Schriftartendateien, die Adobe-Schriftmetriken enthalten und für die Bildbereitstellung verwendet werden.

   * **[!UICONTROL PFM]**: Adobe PostScript-Schriftartendateien, die Informationen zur Schriftartenmetrik enthalten.

   * **[!UICONTROL PFB]**: Adobe PostScript-Schriftartdateien, die binäre Schriftartentwurfsinformationen enthalten und zum Rendern und Bereitstellen von PDF/PostScript-Bildern verwendet werden.
