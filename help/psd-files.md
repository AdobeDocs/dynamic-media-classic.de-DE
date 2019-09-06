---
title: Arbeiten mit PSD-Dateien
seo-title: Arbeiten mit PSD-Dateien
description: 'null'
seo-description: Erfahren Sie, wie Sie mit PSD-Dateien arbeiten.
uuid: 5836 b 660-6 bca -46 e 7-ab 39-1 a 31 d 1 e 0 cff 2
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/master_ files
discoiquuid: 4086 e 3 db -5 aca -41 a 0-8 f 15-302 afbf 67 ddb
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Arbeiten mit PSD-Dateien{#working-with-psd-files}

PSD-Dateien (Photoshop Document Files) werden meist in Dynamic Media Classic verwendet, um Vorlagen zu erstellen. Wenn Sie eine PSD-Datei hochladen, können Sie eine dynamische Media-Vorlage automatisch aus der Datei erstellen (wählen Sie im Anzeigebereich "Hochladen" die Option" Vorlage erstellen" aus).

Wenn Sie eine PSD-Datei mit mehreren Ebenen zum Erstellen einer Vorlage verwenden, erstellt SPS für jede Ebene ein Bild.

## Optionen für das Hochladen von PSD-Dateien {#psd-upload-options}

Die Optionen zum Hochladen von PSD-Dateien befinden sich unter „Upload-Auftragsoptionen“ &gt; „Photoshop-Optionen“. Sie können dabei eine Datei beschneiden, ein Farbprofil für sie auswählen, sie zum Erstellen einer Vorlage verwenden und einen Anker für sie auswählen.

Beim Hochladen von PSD-Dateien sind folgende Optionen verfügbar:

**Beschneiden** (unter "Beschneidungsoptionen" ) Wählen Sie die Option „Beschneiden“, um die weißen Flächen an den Rändern einer PSD-Datei automatisch abzuschneiden, oder wählen Sie die Option „Manuell“, um die Kanten der PSD-Datei zu beschneiden:

**Beschneiden** Sie das Menü "Beschneiden basierend auf" und wählen Sie Farbe oder Transparenz.

Bei Auswahl der Option „Farbe“ wählen Sie anschließend im Menü „Ecke“ die Ecke in der PSD-Datei aus, deren Farbe mit der Farbe der weißen Flächen, die Sie entfernen möchten, am besten übereinstimmt.

Ziehen Sie den Schieberegler auf einen Toleranzwert zwischen 0 und 1.

Wenn Sie beim Beschneiden basierend auf Farbe den Wert 0 einstellen, werden Pixel nur abgeschnitten, wenn sie exakt der Farbe entsprechen, die Sie in der Ecke der PSD-Datei ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.

Wenn Sie beim Beschneiden basierend auf Transparenz den Wert 0 einstellen, werden Pixel nur abgeschnitten, wenn sie vollkommen transparent sind. Werte, die näher an 1 liegen, lassen eine größere Transparenzabweichung zu.

**Manuell** Geben Sie die Anzahl der Pixel ein, die von jeder Seite oder jeder Kante des Bilds abgeschnitten werden sollen. Wie viel vom Bild abgeschnitten wird, hängt von der ppi-Einstellung (Pixel pro Zoll) in der Bilddatei ab. Wenn das Bild beispielsweise eine Auflösung von 150 ppi hat und Sie in den Textfeldern „Oben“, „Rechts“, „Unten“ und „Links“ jeweils den Wert 75 eingeben, wird an jeder Kante des Bilds ein halber Zoll (ca. 1,75 cm) abgeschnitten.

**Farbprofil** (unter "Farbprofiloptionen" ) Wählen Sie eine der folgenden Optionen:

**In srgb konvertieren (Standard)** Konvertiert in srgb (Standard Red Green Blue). sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Websites.

**Ursprünglicher Farbraum** behält den ursprünglichen Farbraum des Bildes bei.

**Benutzerdefiniert von &gt; Zum** Öffnen der Menüs "Konvertieren von" und" Konvertieren in" . Sie können einen Photoshop-Standardfarbraum auswählen oder einen Farbraum, den Sie in SPS hochgeladen haben. Siehe ICC-Profile.

**" Ebenen** beibehalten" rippt die Ebenen in der PSD-Datei, falls vorhanden, in einzelne Assets. Die Asset-Ebenen bleiben mit der PSD-Datei verknüpft. Zeigen Sie sie an, indem Sie die PSD-Datei in der Detailansicht öffnen und das Ebenenbedienfeld auswählen. Siehe Anzeigen und Bearbeiten von Ebenen in einer PSD-Datei.

**Create Template** Erstellt eine Vorlage aus den Ebenen der PSD-Datei.

**Extrahieren Sie Text** extrahieren, damit Benutzer in einem Viewer nach Text suchen können.

**Ebenen auf Hintergrundgröße erweitern** Erweitert die Größe gerippter Bildebenen auf die Größe der Hintergrundebene.

**Ebenen der Ebenenbenennung** in der PSD-Datei werden als separate Bilder hochgeladen. Wählen Sie eine Option zur Benennung dieser Bilder im Scene7 Publishing System:

**Name der Ebene** Benennen die Bilder nach ihren Ebenennamen in der PSD-Datei. Wenn eine Ebene der PSD-Originaldatei beispielsweise „Preisschild“ heißt, wird auch das zugehörige Bild „Preisschild“ genannt. Wenn es sich bei den Namen der Ebenen in der PSD-Datei jedoch um standardmäßige Photoshop-Ebenennamen handelt („Hintergrund“, „Ebene 1“, Ebene 2“ usw.), werden die Bilder nicht nach den Standardebenennamen, sondern nach den Nummern der Ebenen in der PSD-Datei benannt.

**Photoshop und Nummer der Ebene** Geben die Bilder nach ihren Nummern in der PSD-Datei an und ignoriert die ursprünglichen Ebenennamen. Die Bilder werden mit dem Photoshop-Dateinamen und einer angefügten Nummer der Ebene benannt. Beispielsweise erhält die zweite Ebene der Datei „Frühjahrsannonce.psd“ den Namen „Frühjahrsannonce_2“, auch wenn sie in Photoshop einen nicht standardmäßigen Namen hatte.

**Photoshop und Name der Ebene** Benennen die Bilder nach der PSD-Datei gefolgt vom Namen oder der Nummer der Ebene. Die Nummern der Ebenen werden verwendet, wenn es sich bei den Namen der Ebenen in der PSD-Datei um standardmäßige Photoshop-Ebenennamen handelt. Beispielsweise erhält die Ebene „Preisschild“ in der PSD-Datei „Frühjahrsannonce“ den Namen „Frühjahrsannonce_Preisschild“. Eine Ebene mit dem standardmäßigen Namen „Ebene 2“ erhält den Namen „Frühjahrsannonce_2“.

**Anker** festlegen, wie Bilder in Vorlagen verankert werden, die aus der kompositionen mit Ebenen aus der PSD-Datei generiert wurden. Standardmäßig wird der Anker zentriert. Bei einem zentrierten Anker können Ersatzbilder unabhängig von ihrem Seitenverhältnis denselben Raum am besten ausfüllen. Bilder mit einem anderen Seitenverhältnis, die dieses Bild ersetzen, nehmen effektiv denselben Raum ein, wenn auf die Vorlage verwiesen und der Parametersatz verwendet wird. Wählen Sie eine andere Einstellung, wenn es für Ihre Anwendung erforderlich ist, dass die Ersatzbilder den zugewiesenen Raum in der Vorlage ausfüllen.

## Anzeigen und Bearbeiten von Ebenen in einer PSD-Datei {#viewing-and-editing-layers-in-a-psd-file}

Wenn Sie beim Hochladen der PSD-Datei die Option "Ebenen beibehalten" ausgewählt haben, rippt Dynamic Media Classic die einzelnen Ebenen in Assets. Sie können die zu einer PSD-Datei gehörenden Asset-Ebenen anzeigen und bearbeiten, indem Sie die Datei in der Detailansicht des Durchsuchenbedienfelds öffnen.

1. Doppelklicken Sie auf die vollständige PSD-Datei im Durchsuchenbedienfeld, um diese in der Detailansicht zu öffnen.

   ***Hinweis**: Achten Sie darauf, dass Sie das vollständige Asset und keine der PSD-Ebenen öffnen.*

1. Klicken Sie auf „Ebenen“, um das Bedienfeld „Ebenen“ zu öffnen. Alle Ebenen werden als separate Bilder im Bedienfeld „Ebenen“ angezeigt.
1. Doppelklicken Sie auf eine Ebene, um sie zu öffnen, und führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf das Symbol „Imagemap“, um eine Imagemap auf der Ebene zu erstellen. (Siehe [Erstellen von Imagemaps](creating-image-maps.md#creating_image_maps).)
   * Klicken Sie auf „Zoomziele“, um Zoomziele auf der Ebene zu erstellen. (Siehe [Erstellen von Zoomzielen für geführtes Zoomen](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Klicken Sie auf das Symbol für das Zuschneiden, um die Ebene zu beschneiden. (Siehe [Beschneiden von Bildern](cropping-image.md#cropping_an_image).)
   * Klicken Sie auf „Scharfzeichnen“, um die Ebene scharf zu zeichnen. (Siehe [Scharfzeichnen von Bildern](sharpening-image.md#sharpening_an_image).)
   * Klicken Sie auf „Anpassen“, um die Ebene anzupassen. (Siehe [Anpassen von Bildern](adjusting-image.md#adjusting_an_image).)

1. Klicken Sie auf „Speichern“ oder „Speichern unter“.
1. Um eine andere Ebene anzuzeigen oder zu bearbeiten, klicken Sie auf einen Pfeil am unteren Rand der Ebenenvorschau.
1. Wenn Sie die Ebenen-Detailansicht beenden möchten, klicken Sie auf das Symbol für die Rasteransicht.

