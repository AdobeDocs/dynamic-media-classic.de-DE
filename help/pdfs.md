---
title: Arbeiten mit PDF-Dateien
description: Erfahren Sie, wie Sie mit PDFs in Dynamic Media Classic arbeiten.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 56%

---


# Arbeiten mit PDF-Dateien{#working-with-pdfs}

PDF-Dateien (Portable Dokument Format) werden meist in Dynamic Media Classic zum Erstellen von E-Katalogen verwendet. Wenn Sie eine PDF-Datei hochladen, werden die Seiten von Dynamic Media Classic standardmäßig gerastert oder gerippt, sodass die Seiten zum Erstellen von Rich-Media-Daten verwendet werden können.

## Optionen für das Hochladen von PDF-Dateien {#pdf-upload-options}

Eine PDF-Datei, die Sie hochladen, können Sie auf verschiedene Weisen formatieren. Sie können Seiten beschneiden, Suchbegriffe extrahieren, eine ppi-Auflösung (Pixel pro Zoll) eingeben und einen Farbraum auswählen. PDF-Dateien enthalten oft einen Beschnittrand, Schnittmarken, Passermarken und sonstige Druckmarken. Sie können diese Marken beim Hochladen der PDF-Datei an den Kanten der Seiten abschneiden.

Die Optionen für das Hochladen von PDF-Dateien finden Sie im Anzeigebereich „Hochladen“ unter „PDF-Optionen“.

**Verarbeitung**

Es stehen folgende Verarbeitungsoptionen zur Verfügung:

**Rastern**  (Standard) Rippt die Seiten in der PDF-Datei und konvertiert Vektorgrafiken in Bitmapbilder. Wählen Sie diese Option, wenn Sie einen E-Katalog erstellen möchten.

**Suchbegriffe extrahieren** Extrahiert Wörter aus der PDF-Datei, damit die Datei in einem E-Katalog-Viewer nach Schlüsselwörtern durchsucht werden kann.

**Extrahieren von** LinksExtrahiert Links aus den PDF-Dateien und konvertiert sie in Imagemaps, die in einem E-Katalog-Viewer verwendet werden.

**Automatisches Erstellen eines E-Katalogs mit mehrseitiger** PDFAutomatisch erstellt einen E-Katalog aus der PDF-Datei. Der E-Katalog erhält denselben Namen wie die hochgeladene PDF-Datei. (Diese Option ist nur verfügbar, wenn Sie die PDF-Datei beim Hochladen rastern.)

**Auflösung**

Legt die Auflösungseinstellung fest. Mit dieser Einstellung wird bestimmt, wie viele Pixel pro Zoll in der PDF-Datei angezeigt werden. Der Standardwert ist 150.

**Farbraum**

Wählen Sie im Menü „Farbraum“ einen Farbraum für die PDF-Datei aus. Die meisten PDF-Dateien enthalten sowohl RGB- als auch CMYK-Farbbilder. Der RGB-Farbraum eignet sich besonders gut, um die Datei online anzuzeigen.

**Erkennung** automatischBehält den Farbraum der PDF-Datei bei.

**Immer** RGBConvertiert in den RGB-Farbraum.

**Immer** CMYKConvertiert den CMYK-Farbraum.

**Immer** GraustufenKonvertiert in den Graustufen-Farbraum.

**Farbprofil**

Wählen Sie eine Farbprofil-Option aus:

**In** sRGBConverts in sRGB konvertieren (Standard Red Green Blue). sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Websites.

**&quot;Ursprünglicher Farbraum beibehalten&quot;** Behält den ursprünglichen Farbraum bei.

**Benutzerdefiniert von >** Zu öffnet Menüs, damit Sie einen Farbraum &quot;Konvertieren von&quot;und &quot;Konvertieren in&quot;auswählen können. Sie können einen Photoshop-Standardfarbraum oder einen Farbraum auswählen, den Sie in Dynamic Media Classic hochgeladen haben.

Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

## Beschneiden weißer Flächen in PDF-Dateien  {#cropping-white-space-from-a-pdf-file}

1. Um beim Hochladen einer PDF-Datei Pixel in weißen Flächen automatisch abzuschneiden, wählen Sie im Menü „Beschneiden“ die Option „Beschneiden“.
1. Legen Sie die folgenden Optionen fest:

   **Entfernen basierend** auf Beschneiden Wählen Sie, ob basierend auf Farbe oder Transparenz beschnitten werden soll:

   **** ColorWählen Sie die Option &quot;Farbe&quot;. Wählen Sie anschließend im Menü „Ecke“ die Ecke in der PDF-Datei aus, deren Farbe mit der Farbe der weißen Flächen, die Sie entfernen möchten, am besten übereinstimmt.

   **Transparenz** Wählen Sie die Option &quot;Transparenz&quot;.

   **Toleranz** Ziehen Sie den Schieberegler, um eine Toleranz zwischen 0 und 1 festzulegen:

   **Beschneiden basierend auf** FarbeGeben Sie 0 an, damit Pixel nur abgeschnitten werden, wenn sie exakt der Farbe entsprechen, die Sie in der Ecke der PDF-Datei ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.

   **Beschneiden basierend auf** TransparenzGeben Sie 0 an, um Pixel nur abzuschneiden, wenn sie vollkommen transparent sind. Werte, die näher an 1 liegen, lassen eine größere Transparenz zu.

## Beschneiden der Kanten von PDF-Seiten {#cropping-from-the-sides-of-pdf-pages}

Sie können die Druckmarken an den Kanten der Seiten in einer PDF-Datei beim Hochladen manuell entfernen.

1. Wählen Sie im Menü „Beschneiden“ die Option „Manuell“.
1. Geben Sie in die Textfelder „Oben“, „Rechts“, „Unten“ und „Links“ Pixelwerte für den Bereich ein, der am jeweiligen Bildrand abgeschnitten werden soll.

Wie viel von der Seite tatsächlich abgeschnitten wird, hängt davon ab, welchen Wert Sie für die Auflösungseinstellung „Pixel/Zoll“ der PDF-Datei eingeben. Wenn Sie beispielsweise eine Auflösung von 150 (Standardwert) eingeben und an den Kanten der Seiten 75 Pixel abschneiden, wird ein halber Zoll (ca. 1,75 cm) abgeschnitten, weil 75 Pixel bei einer Auflösung von 150 ppi (Pixel pro Zoll) einem halben Zoll entsprechen.
