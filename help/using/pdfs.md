---
title: Arbeiten mit PDF
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic mit PDFs arbeiten.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 25%

---

# Arbeiten mit PDF{#working-with-pdfs}

PDF-Dateien (Portable Document Format) werden am häufigsten in Adobe Dynamic Media Classic zum Erstellen von E-Katalogen verwendet. Wenn Sie eine PDF-Datei hochladen, rastert Adobe Dynamic Media Classic die Seiten oder rippt sie standardmäßig, damit die Seiten zum Erstellen von Rich-Media verwendet werden können.

Beim Hochladen einer PDF zur Seitenextraktion erzwingt Adobe die folgende Begrenzung:

| Art des Limits | Limit | Änderung des Grenzwerts am 31. Dezember 2022 |
| --- | --- | --- |
| Maximale Seitenzahl einer PDF, die für die Extraktion berücksichtigt werden soll | 5.000 (für neue Uploads) | 100 (für alle PDF) |

Siehe auch [Einschränkungen bei Dynamic Media](/help/using/limitations.md).

## Optionen für das Hochladen von PDF-Dateien {#pdf-upload-options}

Eine PDF-Datei, die Sie hochladen, können Sie auf verschiedene Weisen formatieren. Sie können Seiten beschneiden, Suchbegriffe extrahieren, eine ppi-Auflösung (Pixel pro Zoll) eingeben und einen Farbraum auswählen. PDF-Dateien enthalten oft einen Zuschnittrand, Schnittmarken, Registrierungsmarken und andere Druckermarken. Sie können diese Marken beim Hochladen der PDF-Datei an den Kanten der Seiten abschneiden.

Optionen zum Hochladen von PDF-Dateien finden Sie auf der Seite Hochladen unter PDF-Optionen.

### Verarbeitungsoptionen

**[!UICONTROL Rastern]**: (Standard) Teilt die PDF-Datei in einzelne Seiten auf und konvertiert Vektorgrafiken in Bitmap-Bilder. Wählen Sie diese Option, um einen E-Katalog zu erstellen.

**[!UICONTROL Suchbegriffe extrahieren]**: Extrahiert Wörter aus der PDF-Datei, damit Suchbegriffe in der Datei in einem E-Katalog-Viewer durchsucht werden können.

**[!UICONTROL Links extrahieren]**: Extrahiert Links aus den PDF-Dateien und konvertiert sie in Imagemaps, die in einem E-Katalog-Viewer verwendet werden.

**[!UICONTROL E-Katalog mit mehrseitigem PDF automatisch erstellen]**: Erstellt automatisch einen E-Katalog aus der PDF-Datei. Der E-Katalog erhält denselben Namen wie die hochgeladene PDF-Datei. (Diese Option ist nur verfügbar, wenn Sie die PDF-Datei beim Hochladen rastern.)

### Auflösung

Legt die Auflösungseinstellung fest. Mit dieser Einstellung wird bestimmt, wie viele Pixel pro Zoll in der PDF-Datei angezeigt werden. Der Standardwert ist 150.

### Farbraumoptionen

Wählen Sie im Menü „Farbraum“ einen Farbraum für die PDF-Datei aus. Die meisten PDF-Dateien enthalten sowohl RGB- als auch CMYK-Farbbilder. Der RGB-Farbraum eignet sich besonders gut, um die Datei online anzuzeigen.

* **[!UICONTROL Automatisch erkennen]**: Behält den Farbraum der PDF bei.

* **[!UICONTROL Force As RGB]**: Konvertiert in den RGB-Farbraum.

* **[!UICONTROL Immer CMYK]**: Konvertiert in den CMYK-Farbraum.

* **[!UICONTROL Immer Graustufen]**: Konvertiert in den Graustufenfarbraum.

### Farbprofiloptionen

* **[!UICONTROL In sRGB konvertieren]**: Konvertiert in sRGB (Standard Rot Grün Blau). sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf einer Web-Seite.

* **[!UICONTROL Ursprünglichen Farbraum beibehalten]**: Behält den ursprünglichen Farbraum bei.

* **[!UICONTROL Benutzerdefiniertes Formular]** > **[!UICONTROL An]**: Öffnet Menüs, in denen Sie „Konvertieren aus“ und „In Farbraum konvertieren“ auswählen können. Sie können einen standardmäßigen Photoshop-Farbraum oder einen Farbraum auswählen, den Sie in Adobe Dynamic Media Classic hochgeladen haben.

Siehe auch [ICC-Profile](/help/using/icc-profiles.md#icc_profiles).

## Leerraum von einer PDF-Datei beschneiden {#cropping-white-space-from-a-pdf-file}

Sie können Leerraumpixel einer PDF-Datei beim Hochladen automatisch zuschneiden.

1. Wählen Sie im Menü „Beschneiden“ die Option „Zuschneiden“.
1. Legen Sie die folgenden Optionen fest:

   * **[!UICONTROL Beschneiden basierend auf]**: Wählen Sie, ob der Beschneidungsprozess auf Grundlage von Farbe oder Transparenz durchgeführt werden soll:

      * **[!UICONTROL Farbe]**: Wählen Sie die Option „Farbe“. Wählen Sie dann im **[!UICONTROL Ecke]**-Menü die Ecke der PDF mit der Farbe aus, die am besten der Leerraumfarbe entspricht, die Sie beschneiden möchten.

      * **[!UICONTROL Transparenz]**: Wählen Sie die Option „Transparenz“.

   * **[!UICONTROL Toleranz]**: Ziehen Sie den Schieberegler, um eine Toleranz von 0 bis 1 festzulegen.

   * **[!UICONTROL Auf Farbe basierendes Zuschneiden]**: Geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie genau mit der Farbe übereinstimmen, die Sie in der Ecke der PDF ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.

   * **[!UICONTROL Beschneiden auf der Grundlage der Transparenz]**: Geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie transparent sind. Zahlen, die näher an 1 liegen, ermöglichen mehr Transparenz.

## Seitenbeschneidung auf PDF-Seiten {#cropping-from-the-sides-of-pdf-pages}

Sie können die Druckermarkierungen manuell von den Seitenseiten einer PDF-Datei entfernen, während Sie sie hochladen.

1. Wählen Sie im Menü „Beschneiden“ die Option **[!UICONTROL Manuell]** aus.
1. Geben Sie in die Textfelder „Oben“, „Rechts“, „Unten“ und „Links“ Pixelwerte für den Bereich ein, der am jeweiligen Bildrand abgeschnitten werden soll.

Wie viel von der Seite tatsächlich abgeschnitten wird, hängt davon ab, welchen Wert Sie für die Auflösungseinstellung „Pixel/Zoll“ der PDF-Datei eingeben. Angenommen, Sie geben als Auflösungs-PX/Inch-Einstellung 150 (Standard) ein. Anschließend schneiden Sie 75 Pixel an den Seiten der Seiten zu. In diesem Fall 0,5 Zoll. wird abgeschnitten. Bei 150 Pixel pro Zoll entsprechen 75 Pixel einem halben Zoll.
