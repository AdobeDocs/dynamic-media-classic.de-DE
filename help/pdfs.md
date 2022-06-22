---
title: Arbeiten mit PDF
description: Erfahren Sie, wie Sie mit PDF in Adobe Dynamic Media Classic arbeiten.
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: d5dcb990783932f3c5fdd101d1a4c631e73fcdde
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 36%

---

# Arbeiten mit PDF{#working-with-pdfs}

PDF-Dateien (Portable Document Format) werden in Adobe Dynamic Media Classic meist zum Erstellen von E-Katalogen verwendet. Wenn Sie eine PDF-Datei hochladen, rastert Adobe Dynamic Media Classic die Seiten standardmäßig, sodass die Seiten zum Erstellen von Rich-Media-Daten verwendet werden können.

Wenn Sie eine PDF zur Seitenextraktion hochladen, erzwingt Adobe die folgende Einschränkung:

| PDF-Limit-Typ | Implementierte Beschränkung | Änderungen an der Beschränkung vom 31. Dezember 2022 |
| --- | --- | --- |
| Maximale Seitenzahl für eine PDF, die für die Extraktion berücksichtigt werden soll | 5000 (für neue Uploads) | 100 |

Siehe auch [Einschränkungen bei Dynamic Media](/help/limitations.md).

## Optionen für das Hochladen von PDF-Dateien {#pdf-upload-options}

Eine PDF-Datei, die Sie hochladen, können Sie auf verschiedene Weisen formatieren. Sie können Seiten beschneiden, Suchbegriffe extrahieren, eine ppi-Auflösung (Pixel pro Zoll) eingeben und einen Farbraum auswählen. PDF-Dateien enthalten oft einen Beschnittrand, Schnittmarken, Passermarken und sonstige Druckmarken. Sie können diese Marken beim Hochladen der PDF-Datei an den Kanten der Seiten abschneiden.

Die Optionen zum Hochladen von PDF-Dateien finden Sie auf der Seite Hochladen unter PDF-Optionen.

### Verarbeitungsoptionen

**[!UICONTROL Rastern]** - (Standard) Rippt die Seiten in der PDF-Datei und konvertiert Vektorgrafiken in Bitmap-Bilder. Wählen Sie diese Option, um einen eCatalog zu erstellen.

**[!UICONTROL Suchbegriffe extrahieren]** - Extrahiert Wörter aus der PDF-Datei, damit die Datei in einem E-Katalog-Viewer nach Schlüsselwörtern durchsucht werden kann.

**[!UICONTROL Links extrahieren]** - Extrahiert Links aus den PDF-Dateien und konvertiert sie in Imagemaps, die in einem E-Katalog-Viewer verwendet werden.

**[!UICONTROL E-Katalog mit mehrseitigem PDF automatisch erstellen]** - Erstellt automatisch einen eCatalog aus der PDF-Datei. Der E-Katalog erhält denselben Namen wie die hochgeladene PDF-Datei. (Diese Option ist nur verfügbar, wenn Sie die PDF-Datei beim Hochladen rastern.)

### Auflösung

Legt die Auflösungseinstellung fest. Mit dieser Einstellung wird bestimmt, wie viele Pixel pro Zoll in der PDF-Datei angezeigt werden. Der Standardwert ist 150.

### Farbraum optionen

Wählen Sie im Menü „Farbraum“ einen Farbraum für die PDF-Datei aus. Die meisten PDF-Dateien enthalten sowohl RGB- als auch CMYK-Farbbilder. Der RGB-Farbraum eignet sich besonders gut, um die Datei online anzuzeigen.

* **[!UICONTROL Automatisch erkennen]** - Behält den Farbraum der PDF-Datei bei.

* **[!UICONTROL Immer RGB]** - Konvertiert in den RGB-Farbraum.

* **[!UICONTROL Immer CMYK]** - Konvertiert in den CMYK-Farbraum.

* **[!UICONTROL Immer Graustufen]** - Konvertiert in den Graustufen-Farbraum.

### Farbprofiloptionen

* **[!UICONTROL In sRGB konvertieren]** - Konvertiert in sRGB (Standard Red Green Blue). sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Websites.

* **[!UICONTROL Originalfarbraum beibehalten]** - Behält den ursprünglichen Farbraum bei.

* **[!UICONTROL Benutzerdefiniert von]** > **[!UICONTROL nach]** - Öffnet Menüs, damit Sie den Farbraum &quot;Konvertieren von&quot;und &quot;Konvertieren in&quot;auswählen können. Sie können einen standardmäßigen Photoshop-Farbraum oder einen Farbraum auswählen, den Sie in Adobe Dynamic Media Classic hochgeladen haben.

Siehe auch [ICC-Profile](/help/icc-profiles.md#icc_profiles).

## Leerraum aus einer PDF-Datei beschneiden {#cropping-white-space-from-a-pdf-file}

1. Um beim Hochladen einer PDF-Datei Pixel in weißen Flächen automatisch abzuschneiden, wählen Sie im Menü „Beschneiden“ die Option „Beschneiden“.
1. Legen Sie die folgenden Optionen fest:

   * **[!UICONTROL Entfernen basierend auf]** - Wählen Sie anhand von Farbe oder Transparenz aus, ob Zuschnitte vorgenommen werden sollen:

      * **[!UICONTROL Farbe]** - Wählen Sie die Option Farbe aus. Wählen Sie dann die **[!UICONTROL Ecke]** und wählen Sie die Ecke des PDF mit der Farbe aus, die am besten der zu beschneidenden Leerraumfarbe entspricht.

      * **[!UICONTROL Transparenz]** - Wählen Sie die Option Transparenz aus.
   * **[!UICONTROL Toleranz]** - Ziehen Sie den Regler, um eine Toleranz von 0 bis 1 anzugeben.

   * **[!UICONTROL Beschneiden anhand der Farbe]** - Geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie genau der Farbe entsprechen, die Sie in der Ecke des PDF ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.

   * **[!UICONTROL Auf Transparenz basierende Beschneidung]** - Geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie transparent sind. Werte, die näher an 1 liegen, erlauben mehr Transparenz.


## Beschneiden von Seiten auf PDF-Seiten {#cropping-from-the-sides-of-pdf-pages}

Sie können die Druckmarken an den Kanten der Seiten in einer PDF-Datei beim Hochladen manuell entfernen.

1. Wählen Sie im Menü Beschneiden die Option **[!UICONTROL Manuell]**.
1. Geben Sie in die Textfelder „Oben“, „Rechts“, „Unten“ und „Links“ Pixelwerte für den Bereich ein, der am jeweiligen Bildrand abgeschnitten werden soll.

Wie viel von der Seite tatsächlich abgeschnitten wird, hängt davon ab, welchen Wert Sie für die Auflösungseinstellung „Pixel/Zoll“ der PDF-Datei eingeben. Wenn Sie beispielsweise 150 (Standard) als Einstellung für die Auflösung &quot;PX/Inch&quot;eingeben und 75 Pixel von den Seiten abschneiden, wird ein halber Zoll zugeschnitten. bei 150 Pixel pro Zoll 75 Pixel entspricht einem halben Zoll.
