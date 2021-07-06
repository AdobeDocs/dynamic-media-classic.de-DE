---
title: Arbeiten mit PDF-Dateien
description: Erfahren Sie, wie Sie in Dynamic Media Classic mit PDFs arbeiten.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 45%

---

# Arbeiten mit PDF-Dateien{#working-with-pdfs}

PDF-Dateien (Portable Document Format) werden meist in Dynamic Media Classic zum Erstellen von E-Katalogen verwendet. Beim Hochladen einer PDF-Datei rastert Dynamic Media Classic die Seiten standardmäßig, sodass die Seiten zum Erstellen von Rich-Media-Daten verwendet werden können.

## Optionen für das Hochladen von PDF-Dateien {#pdf-upload-options}

Eine PDF-Datei, die Sie hochladen, können Sie auf verschiedene Weisen formatieren. Sie können Seiten beschneiden, Suchbegriffe extrahieren, eine ppi-Auflösung (Pixel pro Zoll) eingeben und einen Farbraum auswählen. PDF-Dateien enthalten oft einen Beschnittrand, Schnittmarken, Passermarken und sonstige Druckmarken. Sie können diese Marken beim Hochladen der PDF-Datei an den Kanten der Seiten abschneiden.

Optionen zum Hochladen von PDF-Dateien finden Sie auf der Seite Hochladen unter PDF-Optionen.

### Verarbeitungsoptionen

**Rastern**  - (Standard) Rippt die Seiten in der PDF-Datei und konvertiert Vektorgrafiken in Bitmap-Bilder. Wählen Sie diese Option, um einen eCatalog zu erstellen.

**Suchbegriffe extrahieren**  - Extrahiert Wörter aus der PDF-Datei, damit die Datei in einem E-Katalog-Viewer nach Schlüsselwörtern durchsucht werden kann.

**Links extrahieren**  - Extrahiert Links aus den PDF-Dateien und konvertiert sie in Imagemaps, die in einem E-Katalog-Viewer verwendet werden.

**eCatalog mit mehrseitiger PDF automatisch erstellen**  - Erstellt automatisch einen eCatalog aus der PDF-Datei. Der E-Katalog erhält denselben Namen wie die hochgeladene PDF-Datei. (Diese Option ist nur verfügbar, wenn Sie die PDF-Datei beim Hochladen rastern.)

### Auflösung

Legt die Auflösungseinstellung fest. Mit dieser Einstellung wird bestimmt, wie viele Pixel pro Zoll in der PDF-Datei angezeigt werden. Der Standardwert ist 150.

### Farbraum optionen

Wählen Sie im Menü „Farbraum“ einen Farbraum für die PDF-Datei aus. Die meisten PDF-Dateien enthalten sowohl RGB- als auch CMYK-Farbbilder. Der RGB-Farbraum eignet sich besonders gut, um die Datei online anzuzeigen.

* **Automatisch erkennen**  - Behält den Farbraum der PDF-Datei bei.

* **Immer RGB**  - Konvertiert in den RGB-Farbraum.

* **Immer CMYK**  - Konvertiert in den CMYK-Farbraum.

* **Immer Graustufen**  - Konvertiert in den Graustufen-Farbraum.

### Farbprofiloptionen

* **In sRGB konvertieren**  - Konvertiert in sRGB (Standard Red Green Blue). sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Websites.

* **Originalfarbraum beibehalten**  - Behält den ursprünglichen Farbraum bei.

* **Benutzerdefiniert von > in**  - Öffnet Menüs, damit Sie einen Farbraum vom Typ &quot;Konvertieren von&quot;und &quot;Konvertieren in&quot;auswählen können. Sie können einen standardmäßigen Photoshop-Farbraum oder einen Farbraum auswählen, den Sie in Dynamic Media Classic hochgeladen haben.

Siehe auch [ICC-Profile](/help/icc-profiles.md#icc_profiles).

## Beschneiden weißer Flächen in PDF-Dateien {#cropping-white-space-from-a-pdf-file}

1. Um beim Hochladen einer PDF-Datei Pixel in weißen Flächen automatisch abzuschneiden, wählen Sie im Menü „Beschneiden“ die Option „Beschneiden“.
1. Legen Sie die folgenden Optionen fest:

   * **Entfernen basierend auf**  - Wählen Sie, ob das Zuschneiden auf Grundlage von Farbe oder Transparenz erfolgen soll:

   * **Farbe**  - Wählen Sie die Option &quot;Farbe&quot;. Wählen Sie anschließend im Menü „Ecke“ die Ecke in der PDF-Datei aus, deren Farbe mit der Farbe der weißen Flächen, die Sie entfernen möchten, am besten übereinstimmt.

   * **Transparenz**  - Wählen Sie die Option &quot;Transparenz&quot;.

   * **Toleranz**  - Ziehen Sie den Regler, um eine Toleranz zwischen 0 und 1 anzugeben.

   * **Beschneiden anhand der Farbe**  - Legen Sie den Wert 0 fest, damit Pixel nur dann abgeschnitten werden, wenn sie genau der Farbe entsprechen, die Sie in der Ecke der PDF-Datei ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.

   * **Auf Transparenz basierendes Zuschneiden**  - Geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie transparent sind. Werte, die näher an 1 liegen, erlauben mehr Transparenz.

## Beschneiden der Kanten von PDF-Seiten {#cropping-from-the-sides-of-pdf-pages}

Sie können die Druckmarken an den Kanten der Seiten in einer PDF-Datei beim Hochladen manuell entfernen.

1. Klicken Sie im Menü Zuschneiden auf **[!UICONTROL Manuell]**.
1. Geben Sie in die Textfelder „Oben“, „Rechts“, „Unten“ und „Links“ Pixelwerte für den Bereich ein, der am jeweiligen Bildrand abgeschnitten werden soll.

Wie viel von der Seite tatsächlich abgeschnitten wird, hängt davon ab, welchen Wert Sie für die Auflösungseinstellung „Pixel/Zoll“ der PDF-Datei eingeben. Wenn Sie beispielsweise 150 (Standard) als Einstellung für die Auflösung &quot;PX/Inch&quot;eingeben und 75 Pixel von den Seiten abschneiden, wird ein halber Zoll zugeschnitten. bei 150 Pixel pro Zoll 75 Pixel entspricht einem halben Zoll.
