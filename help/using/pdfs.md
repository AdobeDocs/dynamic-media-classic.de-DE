---
title: Arbeiten mit PDF
description: Erfahren Sie, wie Sie mit PDF in Adobe Dynamic Media Classic arbeiten.
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

PDF-Dateien (Portable Document Format) werden in Adobe Dynamic Media Classic meist zum Erstellen von E-Katalogen verwendet. Wenn Sie eine PDF-Datei hochladen, rastert Adobe Dynamic Media Classic die Seiten standardmäßig, sodass die Seiten zum Erstellen von Rich-Media-Daten verwendet werden können.

Wenn Sie eine PDF für die Seitenextraktion hochladen, erzwingt Adobe die folgende Einschränkung:

| Begrenzungstyp | Erzwungene Beschränkung | Änderung der Beschränkung am 31. Dezember 2022 |
| --- | --- | --- |
| Maximale Seitenzahl für eine PDF, die für die Extraktion berücksichtigt werden soll | 5000 (für neue Uploads) | 100 (für alle PDF) |

Siehe auch [Dynamic Media-Einschränkungen](/help/using/limitations.md).

## Optionen für das Hochladen von PDF-Dateien {#pdf-upload-options}

Eine PDF-Datei, die Sie hochladen, können Sie auf verschiedene Weisen formatieren. Sie können Seiten beschneiden, Suchbegriffe extrahieren, eine ppi-Auflösung (Pixel pro Zoll) eingeben und einen Farbraum auswählen. PDF-Dateien enthalten oft einen Schnitt-, Zuschnitt-, Registrierungs- und andere Druckermarkierungen. Sie können diese Marken beim Hochladen der PDF-Datei an den Kanten der Seiten abschneiden.

Die Optionen zum Hochladen von PDF-Dateien finden Sie auf der Seite Hochladen unter PDF-Optionen.

### Verarbeitungsoptionen

**[!UICONTROL Rasterize]**: (Standard) Rippt die Seiten in der PDF-Datei und konvertiert Vektorgrafiken in Bitmapbilder. Wählen Sie diese Option, um einen eCatalog zu erstellen.

**[!UICONTROL Suchbegriffe extrahieren]**: Extrahiert Wörter aus der PDF-Datei, damit Suchbegriffe in der in einem E-Katalog-Viewer durchsucht werden können.

**[!UICONTROL Links extrahieren]**: Extrahiert Links aus den PDF-Dateien und konvertiert sie in Imagemaps, die in einem E-Katalog-Viewer verwendet werden.

**[!UICONTROL E-Katalog mit mehrseitigem PDF automatisch erstellen]**: Erstellt automatisch einen eCatalog aus der PDF-Datei. Der E-Katalog erhält denselben Namen wie die hochgeladene PDF-Datei. (Diese Option ist nur verfügbar, wenn Sie die PDF-Datei beim Hochladen rastern.)

### Auflösung

Legt die Auflösungseinstellung fest. Mit dieser Einstellung wird bestimmt, wie viele Pixel pro Zoll in der PDF-Datei angezeigt werden. Der Standardwert ist 150.

### Optionen für Farbraum

Wählen Sie im Menü „Farbraum“ einen Farbraum für die PDF-Datei aus. Die meisten PDF-Dateien enthalten sowohl RGB- als auch CMYK-Farbbilder. Der RGB-Farbraum eignet sich besonders gut, um die Datei online anzuzeigen.

* **[!UICONTROL Automatisch erkennen]**: Behält den Farbraum der PDF-Datei bei.

* **[!UICONTROL Immer RGB]**: Konvertiert in den Farbraum RGB.

* **[!UICONTROL Immer CMYK]**: Konvertiert in den CMYK-Farbraum.

* **[!UICONTROL Immer Graustufen]**: Konvertiert in den Graustufen-Farbraum.

### Farbprofiloptionen

* **[!UICONTROL In sRGB konvertieren]**: Konvertiert in sRGB (Standard Red Green Blue). sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf einer Webseite.

* **[!UICONTROL Ursprünglichen Farbraum beibehalten]**: Behält den ursprünglichen Farbraum bei.

* **[!UICONTROL Benutzerdefiniert von]** > **[!UICONTROL bis]**: Öffnet Menüs, damit Sie einen Farbraum &quot;Konvertieren von&quot;und &quot;Konvertieren in&quot;auswählen können. Sie können einen standardmäßigen Photoshop-Farbraum oder einen Farbraum auswählen, den Sie in Adobe Dynamic Media Classic hochgeladen haben.

Siehe auch [ICC-Profile](/help/using/icc-profiles.md#icc_profiles).

## Leerraum aus einer PDF-Datei beschneiden {#cropping-white-space-from-a-pdf-file}

Sie können während des Uploads von einer PDF-Datei automatisch weiße Leerraum-Pixel beschneiden.

1. Wählen Sie das Menü Zuschneiden und dann Zuschneiden aus.
1. Legen Sie die folgenden Optionen fest:

   * **[!UICONTROL Entfernen basierend auf]**: Wählen Sie aus, ob das Zuschneiden auf Grundlage von Farbe oder Transparenz erfolgen soll:

      * **[!UICONTROL Farbe]**: Wählen Sie die Option &quot;Farbe&quot;. Wählen Sie dann das Menü **[!UICONTROL Ecke]** aus und wählen Sie die Ecke des PDF mit der Farbe aus, die am besten der zu beschneidenden Leerraum-Farbe entspricht.

      * **[!UICONTROL Transparenz]**: Wählen Sie die Option &quot;Transparenz&quot;.

   * **[!UICONTROL Toleranz]**: Ziehen Sie den Regler, um eine Toleranz von 0 bis 1 anzugeben.

   * **[!UICONTROL Beschneiden basierend auf Farbe]**: Geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie genau der Farbe entsprechen, die Sie in der Ecke des PDF ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.

   * **[!UICONTROL Auf Transparenz basierendes Zuschneiden]**: Geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie transparent sind. Werte, die näher an 1 liegen, ermöglichen mehr Transparenz.

## Beschneiden von den Seiten der PDF-Seiten {#cropping-from-the-sides-of-pdf-pages}

Sie können die Druckmarkierungen beim Hochladen manuell von den Seiten in einer PDF-Datei entfernen.

1. Wählen Sie im Menü &quot;Beschneiden&quot;die Option **[!UICONTROL Manuell]**.
1. Geben Sie in die Textfelder „Oben“, „Rechts“, „Unten“ und „Links“ Pixelwerte für den Bereich ein, der am jeweiligen Bildrand abgeschnitten werden soll.

Wie viel von der Seite tatsächlich abgeschnitten wird, hängt davon ab, welchen Wert Sie für die Auflösungseinstellung „Pixel/Zoll“ der PDF-Datei eingeben. Angenommen, Sie geben 150 (Standard) als Einstellung &quot;Auflösung PX/Zoll&quot;ein. Anschließend beschneiden Sie die Seiten um 75 Pixel. In diesem Fall sind es 0,5 Zoll. zugeschnitten ist. Bei 150 Pixel pro Zoll entsprechen 75 Pixel einem halben Zoll.
