---
title: Bildbearbeitungsoptionen beim Hochladen
description: Erfahren Sie mehr über die Bildbearbeitungsoptionen, die beim Hochladen verfügbar sind.
uuid: 0912ae6f-41c9-41b5-94d1-e266face782e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: d3f21cdf-2cb3-46e8-955a-b8daf0b233bc
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 78%

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

* **Entfernen basierend**
auf Beschneiden Wählen Sie, ob basierend auf Farbe oder Transparenz beschnitten werden soll:

* ****
ColorWählen Sie die Option &quot;Farbe&quot;. Wählen Sie anschließend in der Dropdown-Liste „Ecke“ die Bildecke mit der Farbe aus, die der Farbe der weißen Flächen, die Sie beschneiden möchten, am besten entspricht.

* **Transparenz**
Wählen Sie die Option &quot;Transparenz&quot;.

* **Toleranz**
Ziehen Sie den Schieberegler, um eine Toleranz zwischen 0 und 1 festzulegen:

* **Beschneiden basierend auf**
FarbeGeben Sie 0 an, um Pixel nur zu beschneiden, wenn sie exakt der Farbe entsprechen, die Sie in der Bildecke ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.

* **Beschneiden basierend auf**
TransparenzGeben Sie 0 an, um Pixel nur abzuschneiden, wenn sie vollkommen transparent sind. Werte, die näher an 1 liegen, lassen eine größere Transparenz zu.

**Manuelles Beschneiden eines Bilds an den Kanten**

Um ein Bild manuell an den Kanten zu beschneiden, wählen Sie im Menü „Beschneiden“ die Option „Manuell“. Geben Sie dann die Anzahl an Pixeln ein, die an einer oder jeder Kante des Bilds abgeschnitten werden soll. Wie viel vom Bild abgeschnitten wird, hängt von der ppi-Einstellung (Pixel pro Zoll) in der Bilddatei ab. Wenn das Bild beispielsweise eine Auflösung von 150 ppi hat und Sie in den Textfeldern „Oben“, „Rechts“, „Unten“ und „Links“ jeweils den Wert 75 eingeben, wird an jeder Kante ein halber Zoll (ca. 1,75 cm) abgeschnitten.

**Auswählen eines Farbprofils**

Wählen Sie unter „Farbprofil“ eine der folgenden Optionen, um einen Farbraum für das Bild festzulegen:

* **In**
sRGBConverts in sRGB konvertieren (Standard Red Green Blue). sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Websites.

* **&quot;Ursprünglicher Farbraum beibehalten&quot;**
Behält den ursprünglichen Farbraum bei.

* **Benutzerdefiniert von >**
Zu öffnet Menüs, damit Sie einen Farbraum &quot;Konvertieren von&quot;und &quot;Konvertieren in&quot;auswählen können. Sie können einen Photoshop-Standardfarbraum oder einen Farbraum auswählen, den Sie in Dynamic Media Classic hochgeladen haben.

Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

**Erstellen einer Maske aus einem Beschneidungspfad**

Wählen Sie die **Maske aus Beschneidungspfad erstellen**, um basierend auf den Beschneidungspfadinformationen eine Maske für das Bild zu erstellen. Diese Option betrifft Bilder, die unter Verwendung eines Beschneidungspfads erstellt wurden.

**Scharfzeichnen eines Bildes mithilfe der Unschärfemaske**

Dieser Filter ermöglicht es Ihnen, den Scharfzeichnungsfiltereffekt an das endgültige neu berechnete Bild anzupassen. Sie können die Intensität des Effekts, den Radius des Effekts (gemessen in Pixel) und einen Schwellenwert für den Kontrast steuern, der ignoriert wird.

Dieser Effekt verwendet die gleichen Optionen wie der Photoshop-Filter „Unscharf maskieren“. Im Gegensatz zu dem, dass der Name impliziert, ist die „Unschärfemaske“ ein Scharfzeichnungsfilter.

Wählen Sie unter „Unschärfemaske &quot; die gewünschten Optionen aus. Die zur Verfügung stehenden Optionen sind in der folgenden Tabelle aufgeführt:

| Optionen für „Unschärfemaske“ | Beschreibung |
|--- |--- |
| Betrag | Gibt den Kontrastgrad an, der auf die Pixel an den Rändern angewendet wird. <br><br>Sie können sich die Auswirkung der Option „Betrag“ wie ein Maß für die Filterintensität vorstellen. Der Hauptunterschied zwischen den Zahlenwerten von &quot;Unscharf maskieren&quot;in Dynamic Media Classic und den Zahlenwerten in Adobe Photoshop besteht darin, dass Photoshop einen Betrag zwischen 1 % und 500 % hat. Während in Dynamic Media Classic der Wertebereich zwischen 0,0 und 5,0 liegt. Ein Wert von 5,0 in Dynamic Media Classic entspricht ungefähr 500 % in Photoshop. ein Wert von 0,9 entspricht 90 % usw. |
| Radius | Diese Option steuert den Radius des Effekts. <br><br>Der Wertebereich ist 0-250. Der Effekt wird auf allen Pixeln in einem Bild ausgeführt und strahlt von allen Pixeln in alle Richtungen aus. Der Radius wird in Pixel angegeben. Um beispielsweise einen ähnlichen Scharfzeichnungseffekt für ein 2000 x 2000-Pixelbild und ein 500 x 500-Pixelbild zu erhalten, können Sie einen Radiuswert von zwei Pixeln auf dem 2000 x 2000-Pixelbild und einen Radiuswert von einem Pixel auf dem 500 x 500-Pixelbild festlegen. Ein größerer Wert wird entsprechend für ein Bild mit mehr Pixeln verwendet.  |
| Schwelle | Gibt den Kontrastbereich an, der beim Anwenden des Filters „Unschärfemaske“ ignoriert werden soll. Dies ist wichtig, damit kein „Bildrauschen“ entsteht, wenn Sie diesen Filter anwenden. Der Schwellenwert verwendet einen Wert von 0 bis 255, was für die Anzahl der Helligkeitsschritte in einem Graustufenbild steht. 0=schwarz, 128=50 % grau und 255=weiß. <br><br>Beispiel: Ein Schwellenwert von 12 ignoriert leichte Variationen der Hauttonhelligkeit, um kein Rauschen hinzuzufügen, fügt aber trotzdem einen Kantenkontrast zu kontrastreichen Bereichen (z. B. wo Wimpern auf die Haut treffen) hinzu. <br><br>Wenn Sie beispielsweise ein Foto mit einem Gesicht einer Person haben, wirkt sich die „Unschärfemaske“ auf die Teile des Bildes mit dem höchsten Kontrast (z. B. wo die Wimpern auf die Haut treffen), und auf die glatte Haut aus, um einen wünschenswerten Kontrastbereich zu schaffen. Selbst die glatteste Haut weist subtile Änderungen in Helligkeitswerten auf. Wenn Sie keinen Schwellenwert verwenden, akzentuiert der Filter diese subtilen Änderungen in den Hautpixeln. Dies wiederum erzeugt einen Rauscheffekt (der wahrscheinlich unerwünscht ist), während er gleichzeitig den Kontrast an den Wimpern erhöht und somit die Schärfe verbessert (wahrscheinlich wünschenswert)<br><br>Um dieses Problem zu vermeiden, verwenden Sie einen Schwellenwert, bei dem der Filter Pixel ignoriert, die den Kontrast nicht drastisch ändern, wie z. B. glatte Haut. <br><br>Achten Sie in der weiter oben gezeigten Reißverschlussgrafik auf die Textur neben dem Reißverschluss. Hier ist Bildrauschen erkennbar, weil die Schwellenwerte zu niedrig waren, um das Bildrauschen zu unterdrücken. |
| Monochrom | Wählen Sie diese Option, um die „Umschärfemaske“ auf die Gesamthelligkeit (Intensität) des Bildes anzuwenden.<br><br>Deaktivieren Sie diese Option, um die „Unschärfemaske“ separat für jede Farbkomponente anzuwenden. |

Siehe [Scharfzeichnen von Bildern](sharpening-image.md#sharpening_an_image).

Siehe auch [Scharfzeichnen von Bildern im Scene7 Publishing System und auf dem Image-Server](/help/assets/s7_sharpening_images.pdf).

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

