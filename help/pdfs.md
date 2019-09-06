---
title: Arbeiten mit PDF-Dateien
seo-title: Arbeiten mit PDF-Dateien
description: 'null'
seo-description: Erfahren Sie, wie Sie mit pdfs in Dynamic Media Classic arbeiten.
uuid: 26 d 70 d 28-9393-49 b 1-9051-d 70456 deca 67
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/master_ files
discoiquuid: 5 a 073 de 3-6 b 1 d -4 c 3 e -8 c 03-9182 f 9 f 3874 a
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Arbeiten mit PDF-Dateien{#working-with-pdfs}

PDF-Dateien (Portable Document Format) werden meist in Dynamic Media Classic verwendet, um E-Kataloge zu erstellen. Wenn Sie eine PDF-Datei hochladen, werden die Seiten standardmäßig von dynamischen Medien Classic gerastert oder gerippt, damit die Seiten zum Erstellen von Rich-Media-Daten verwendet werden können.

## Optionen für das Hochladen von PDF-Dateien {#pdf-upload-options}

Eine PDF-Datei, die Sie hochladen, können Sie auf verschiedene Weisen formatieren. Sie können Seiten beschneiden, Suchbegriffe extrahieren, eine ppi-Auflösung (Pixel pro Zoll) eingeben und einen Farbraum auswählen. PDF-Dateien enthalten oft einen Beschnittrand, Schnittmarken, Passermarken und sonstige Druckmarken. Sie können diese Marken beim Hochladen der PDF-Datei an den Kanten der Seiten abschneiden.

Die Optionen für das Hochladen von PDF-Dateien finden Sie im Anzeigebereich „Hochladen“ unter „PDF-Optionen“.

**Verarbeitung**

Es stehen folgende Verarbeitungsoptionen zur Verfügung:

**Rastern** (Standard) Gerippt die Seiten in der PDF-Datei und konvertiert Vektorgrafiken in Bitmapbilder. Wählen Sie diese Option, wenn Sie einen E-Katalog erstellen möchten.

**Extrahieren Sie Suchbegriffe** aus der PDF-Datei, damit die Datei in einem E-Katalog-Viewer nach Schlüsselwörtern durchsucht werden kann.

**Links extrahieren Links** aus den PDF-Dateien und decken sie in Imagemaps ab, die in einem E-Katalog-Viewer verwendet werden.

**E-Katalog automatisch mit Mehrseitiger PDF-Datei** erstellen, erstellt automatisch einen E-Katalog aus der PDF-Datei. Der E-Katalog erhält denselben Namen wie die hochgeladene PDF-Datei. (Diese Option ist nur verfügbar, wenn Sie die PDF-Datei beim Hochladen rastern.)

**Auflösung**

Legt die Auflösungseinstellung fest. Mit dieser Einstellung wird bestimmt, wie viele Pixel pro Zoll in der PDF-Datei angezeigt werden. Der Standardwert ist 150.

**Farbraum**

Wählen Sie im Menü „Farbraum“ einen Farbraum für die PDF-Datei aus. Die meisten PDF-Dateien enthalten sowohl RGB- als auch CMYK-Farbbilder. Der RGB-Farbraum eignet sich besonders gut, um die Datei online anzuzeigen.

**Der Farbraum der PDF-Datei** wird automatisch beibehalten.

**Immer RGB** -Konvertierung in RGB-Farbraum.

**Immer CMYK** Konvertiert den CMYK-Farbraum.

**Immer Graustufen-** Konvertierung in den Graustufen-Farbraum.

**Farbprofil**

Wählen Sie eine Farbprofil-Option aus:

**In srgb** konvertieren: In srgb konvertiert (Standard Red Green Blue). sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Websites.

**Ursprünglicher Farbraum** behält den ursprünglichen Farbraum bei.

**Benutzerdefiniert von &gt; Zum** Öffnen der Menüs "Konvertieren von" und" Konvertieren in" . Sie können einen Photoshop-Standardfarbraum auswählen oder einen Farbraum, den Sie in SPS hochgeladen haben. 

Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

## Beschneiden weißer Flächen in PDF-Dateien {#cropping-white-space-from-a-pdf-file}

1. Um beim Hochladen einer PDF-Datei Pixel in weißen Flächen automatisch abzuschneiden, wählen Sie im Menü „Beschneiden“ die Option „Beschneiden“.
1. Legen Sie die folgenden Optionen fest:

   **Beschneiden
basierend auf** auswählen, ob die Beschneidung basierend auf Farbe oder Transparenz erfolgen soll:

   **Farbe** wählen Sie die Option "Farbe" . Wählen Sie anschließend im Menü „Ecke“ die Ecke in der PDF-Datei aus, deren Farbe mit der Farbe der weißen Flächen, die Sie entfernen möchten, am besten übereinstimmt.

   **Transparenz** Wählen Sie die Option "Transparenz" .

   **Toleranz** ziehen Sie den Regler, um eine Toleranz zwischen 0 und 1 anzugeben:

   **Beschneiden basierend auf Farbe** festlegen, um Pixel nur zu beschneiden, wenn sie exakt der Farbe entsprechen, die Sie in der Ecke der PDF-Datei ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.

   **Beschneiden basierend auf Transparenz** Festlegen 0 zum Beschneiden von Pixeln nur, wenn sie vollkommen transparent sind; Werte, die näher an 1 liegen, lassen eine größere Transparenzabweichung zu.

## Beschneiden der Kanten von PDF-Seiten {#cropping-from-the-sides-of-pdf-pages}

Sie können die Druckmarken an den Kanten der Seiten in einer PDF-Datei beim Hochladen manuell entfernen.

1. Wählen Sie im Menü „Beschneiden“ die Option „Manuell“.
1. Geben Sie in die Textfelder „Oben“, „Rechts“, „Unten“ und „Links“ Pixelwerte für den Bereich ein, der am jeweiligen Bildrand abgeschnitten werden soll.

Wie viel von der Seite tatsächlich abgeschnitten wird, hängt davon ab, welchen Wert Sie für die Auflösungseinstellung „Pixel/Zoll“ der PDF-Datei eingeben. Wenn Sie beispielsweise eine Auflösung von 150 (Standardwert) eingeben und an den Kanten der Seiten 75 Pixel abschneiden, wird ein halber Zoll (ca. 1,75 cm) abgeschnitten, weil 75 Pixel bei einer Auflösung von 150 ppi (Pixel pro Zoll) einem halben Zoll entsprechen.
