---
title: Bildbearbeitungsoptionen beim Hochladen
seo-title: Bildbearbeitungsoptionen beim Hochladen
description: 'null'
seo-description: Erfahren Sie mehr über die Bildbearbeitungsoptionen, die zum Zeitpunkt des Hochladens verfügbar sind.
uuid: 0912 ae 6 f -41 c 9-41 b 5-94 d 1-e 266 face 782 e
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/master_ files
discoiquuid: d 3 f 21 cdf -2 cb 3-46 e 8-955 a-b 8 daf 0 b 233 bc
translation-type: tm+mt
source-git-commit: 0f6c8e6ac69e29aab7a48425aab76c10170d9ddf

---


# Bildbearbeitungsoptionen beim Hochladen{#image-editing-options-at-upload}

Beim Hochladen von Bilddateien, einschließlich AI-, EPS- und PSD-Dateien, können Sie folgende Bearbeitungsaktionen im Dialogfeld „Upload-Auftragsoptionen“ vornehmen:

* Beschneiden des Bilds zum Entfernen weißer Flächen am Rand.
* Manuelles Beschneiden eines Bilds an den Kanten.
* Auswählen eines Farbprofils.
* Erstellen einer Maske aus einem Beschneidungspfad.
* Scharfzeichnen von Bildern mit Optionen für „Unschärfemaske“
* Hintergrund aussparen

Diese Optionen finden Sie im Anzeigebereich „Hochladen“ unter „Bildbearbeitungsoptionen“.

**Beschneiden von Bildern zum Entfernen weißer Flächen**

Um automatisch weiße Pixelflächen von einem Bild abzuschneiden, wählen Sie im Menü „Beschneiden“ die Option „Beschneiden“. Anschließend können Sie folgende Optionen wählen:

**Beschneiden
basierend auf** auswählen, ob die Beschneidung basierend auf Farbe oder Transparenz erfolgen soll:

**Farbe** wählen Sie die Option "Farbe" . Wählen Sie anschließend in der Dropdown-Liste „Ecke“ die Bildecke mit der Farbe aus, die der Farbe der weißen Flächen, die Sie beschneiden möchten, am besten entspricht.

**Transparenz** Wählen Sie die Option "Transparenz" .

**Toleranz** ziehen Sie den Regler, um eine Toleranz zwischen 0 und 1 anzugeben:

**Beschneiden basierend auf Farbe** festlegen, um Pixel nur zu beschneiden, wenn sie exakt der Farbe entsprechen, die Sie in der Ecke des Bilds ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.

**Beschneiden basierend auf Transparenz** Festlegen 0 zum Beschneiden von Pixeln nur, wenn sie vollkommen transparent sind; Werte, die näher an 1 liegen, lassen eine größere Transparenzabweichung zu.

**Manuelles Beschneiden eines Bilds an den Kanten**

Um ein Bild manuell an den Kanten zu beschneiden, wählen Sie im Menü „Beschneiden“ die Option „Manuell“. Geben Sie dann die Anzahl an Pixeln ein, die an einer oder jeder Kante des Bilds abgeschnitten werden soll. Wie viel vom Bild abgeschnitten wird, hängt von der ppi-Einstellung (Pixel pro Zoll) in der Bilddatei ab. Wenn das Bild beispielsweise eine Auflösung von 150 ppi hat und Sie in den Textfeldern „Oben“, „Rechts“, „Unten“ und „Links“ jeweils den Wert 75 eingeben, wird an jeder Kante ein halber Zoll (ca. 1,75 cm) abgeschnitten.

**Auswählen eines Farbprofils**

Wählen Sie unter „Farbprofil“ eine der folgenden Optionen, um einen Farbraum für das Bild festzulegen:

**In srgb** konvertieren: In srgb konvertiert (Standard Red Green Blue). sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Websites.

**Ursprünglicher Farbraum** behält den ursprünglichen Farbraum bei.

**Benutzerdefiniert von &gt; Zum** Öffnen der Menüs "Konvertieren von" und" Konvertieren in" . Sie können einen Photoshop-Standardfarbraum auswählen oder einen Farbraum, den Sie in SPS hochgeladen haben. 

Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

**Erstellen einer Maske aus einem Beschneidungspfad**

Wählen Sie die **Maske aus Beschneidungspfad erstellen**, um basierend auf den Beschneidungspfadinformationen eine Maske für das Bild zu erstellen. Diese Option betrifft Bilder, die unter Verwendung eines Beschneidungspfads erstellt wurden.

**Scharfzeichnen eines Bildes mithilfe der Unschärfemaske**

Dieser Filter ermöglicht es Ihnen, den Scharfzeichnungsfiltereffekt an das endgültige neu berechnete Bild anzupassen. Sie können die Intensität des Effekts, den Radius des Effekts (gemessen in Pixel) und einen Schwellenwert für den Kontrast steuern, der ignoriert wird.

Dieser Effekt verwendet die gleichen Optionen wie der Photoshop-Filter „Unscharf maskieren“. Im Gegensatz zu dem, dass der Name impliziert, ist die „Unschärfemaske“ ein Scharfzeichnungsfilter.

Wählen Sie unter „Unschärfemaske " die gewünschten Optionen aus. Die zur Verfügung stehenden Optionen sind in der folgenden Tabelle aufgeführt:

| Optionen für „Unschärfemaske“ | Beschreibung |
|--- |--- |
| Betrag | Gibt den Kontrastgrad an, der auf die Pixel an den Rändern angewendet wird. <br><br>Sie können sich die Auswirkung der Option „Betrag“ wie ein Maß für die Filterintensität vorstellen. Beachten Sie, dass die Stärke-Einstellung in Scene7 nicht dieselbe wie die Stärke-Einstellung in Photoshop ist. Photoshop verwendet einen Wert im Bereich von 1 % bis 500 %, während Scene7 die Werte von 0,0 bis 5,0 skaliert. (Ein Wert von 5,0 in SPS entspricht ungefähr 500 % in Photoshop, ein Wert von 0,9 ungefähr 90 % usw.) |
| Radius | Diese Option steuert den Radius des Effekts. <br><br>Der Wertebereich ist 0 bis 250. Der Effekt wird auf allen Pixeln in einem Bild ausgeführt und strahlt alle Pixel in allen Richtungen aus. Der Radius wird in Pixel angegeben. Um beispielsweise einen ähnlichen Scharfzeichnungseffekt für ein 2000 x 2000-Pixelbild und ein 500 x 500-Pixelbild zu erhalten, können Sie einen Radiuswert von zwei Pixeln auf dem 2000 x 2000-Pixelbild und einen Radiuswert von einem Pixel auf dem 500 x 500-Pixelbild festlegen. Ein größerer Wert wird entsprechend für ein Bild mit mehr Pixeln verwendet.  |
| Schwelle | Gibt den Kontrastbereich an, der beim Anwenden des Filters „Unschärfemaske“ ignoriert werden soll. Dies ist wichtig, damit kein „Bildrauschen“ entsteht, wenn Sie diesen Filter anwenden. Der Schwellenwert verwendet einen Wert von 0 bis 255, was für die Anzahl der Helligkeitsschritte in einem Graustufenbild steht. 0=schwarz, 128=50 % grau und 255=weiß. <br><br>Beispiel: Ein Schwellenwert von 12 ignoriert leichte Variationen der Hauttonhelligkeit, um kein Rauschen hinzuzufügen, fügt aber trotzdem einen Kantenkontrast zu kontrastreichen Bereichen (z. B. wo Wimpern auf die Haut treffen) hinzu. <br><br>Wenn Sie beispielsweise ein Foto mit einem Gesicht einer Person haben, wirkt sich die „Unschärfemaske“ auf die Teile des Bildes mit dem höchsten Kontrast (z. B. wo die Wimpern auf die Haut treffen), und auf die glatte Haut aus, um einen wünschenswerten Kontrastbereich zu schaffen. Selbst die glatteste Haut weist subtile Änderungen in Helligkeitswerten auf. Wenn Sie keinen Schwellenwert verwenden, akzentuiert der Filter diese subtilen Änderungen in den Hautpixeln. Dies wiederum erzeugt einen Rauscheffekt (der wahrscheinlich unerwünscht ist), während er gleichzeitig den Kontrast an den Wimpern erhöht und somit die Schärfe verbessert (wahrscheinlich wünschenswert)<br><br>Um dieses Problem zu vermeiden, verwenden Sie einen Schwellenwert, bei dem der Filter Pixel ignoriert, die den Kontrast nicht drastisch ändern, wie z. B. glatte Haut. <br><br>Achten Sie in der weiter oben gezeigten Reißverschlussgrafik auf die Textur neben dem Reißverschluss. Hier ist Bildrauschen erkennbar, weil die Schwellenwerte zu niedrig waren, um das Bildrauschen zu unterdrücken. |
| Monochrom | Wählen Sie diese Option, um die „Umschärfemaske“ auf die Gesamthelligkeit (Intensität) des Bildes anzuwenden.<br><br>Deaktivieren Sie diese Option, um die „Unschärfemaske“ separat für jede Farbkomponente anzuwenden. |

Siehe [Scharfzeichnen von Bildern](sharpening-image.md#sharpening_an_image).

See also [Sharpening images in Scene7 Publishing System and on Image Server](https://marketing.adobe.com/resources/help/en_US/s7/sharpening/s7_sharpening_images.pdf).

**Hintergrund aussparen**

Mit der Option „Hintergrund aussparen“ können Sie den Hintergrund eines Bildes automatisch entfernen, wenn Sie das Bild hochladen. Diese Technik eignet sich dazu, die Aufmerksamkeit auf ein bestimmtes Objekt zu lenken und es von einem stark ablenkenden Hintergrund abzuheben.

| Optionen für „Hintergrund aussparen“ | Beschreibung |
|:--- |:--- |
| Hintergrund aussparen | Wählen Sie diese Option, um die Funktionen und Optionen für „Hintergrund ausssparen“ zu aktivieren bzw. „einzuschalten“.  |
| Ecke | Erforderlich.<br><br>Die Ecke des Bildes, mit der die auszusparende Hintergrundfarbe definiert wird.<br><br>Sie können zwischen <b>Links oben, Links unten, Rechts oben oder Rechts unten</b> wählen.  |
| Füllmethode | Erforderlich. <br><br>Legt die Pixeltransparenz der von Ihnen gewählten „Ecke“ fest.<br><br>Sie können zwischen den folgenden Füllmethoden wählen: <ul><li><b>Großflächig füllen</b> – Macht alle Pixel transparent, die der von Ihnen angegebenen „Ecke“ entsprechen und mit ihr verbunden sind.</li><li><b>Pixel abgleichen</b> – Macht alle entsprechenden Pixel transparent, unabhängig von ihrer Position auf dem Bild.</li></ul> |
| Toleranz | Optional.<br><br>Legt den zulässigen Betrag für die Abweichung von der Pixelfarbe fest, basierend von der „Ecke“, die Sie ausgewählt haben.<br><br>Bei einem Wert von 0,0 muss die Pixelfarbe exakt entsprechen. Ein Wert von 1,0 steht für die größtmögliche Abweichung. |

>[!MORELIKETHIS]
>
>* [Beschneiden eines Bildes](cropping-image.md#cropping_an_image)
