---
title: Bildoptimierungsoptionen beim Hochladen
description: Erfahren Sie mehr über die Optionen zur Bildoptimierung, die zum Zeitpunkt des Uploads in Adobe Dynamic Media Classic verfügbar sind.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 2d9fc6d8-973f-4aaa-bc2c-b49cda2cde58
topic: Administration, Content Management
level: Intermediate
source-git-commit: 163eb32112ec6fbefd1dacf48212353ff3053d54
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 29%

---

# Bildoptimierungsoptionen beim Hochladen{#image-editing-options-at-upload}

Beim Hochladen von Bilddateien, einschließlich AI-, EPS- und PSD-Dateien, können Sie folgende Bearbeitungsaktionen im Dialogfeld „Upload-Auftragsoptionen“ vornehmen:

* Beschneiden Sie den Leerraum vom Rand der Bilder.
* Manuelles Beschneiden eines Bilds an den Kanten.
* Auswählen eines Farbprofils.
* Erstellen einer Maske aus einem Beschneidungspfad.
* Scharfzeichnen von Bildern mit Optionen für „Unschärfemaske“
* Hintergrund aussparen

Diese Optionen befinden sich auf der Seite &quot;Hochladen&quot;unter der **[!UICONTROL Bildbearbeitungsoptionen]** -Überschrift.

## Leerraum aus Bildern beschneiden

Sie können automatisch weiße Leerraum-Pixel aus einem Bild beschneiden. Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL Optionen zum Zuschneiden]**. Im **[!UICONTROL Zuschneiden]** Dropdown-Liste auswählen **[!UICONTROL Zuschneiden]**. Anschließend können Sie folgende Optionen wählen:

* **[!UICONTROL Entfernen basierend auf]** - Wählen Sie aus dieser Dropdownliste aus, ob das Zuschneiden auf Grundlage von Farbe oder Transparenz erfolgen soll:

   * **[!UICONTROL Farbe]** - Wählen Sie die **[!UICONTROL Farbe]** -Option. Dann aus dem **[!UICONTROL Ecke]** in der Dropdown-Liste die Ecke des Bildes mit der Farbe auswählen, die der Farbe des Leerraums, die Sie zuschneiden möchten, am besten entspricht.

   * **[!UICONTROL Transparenz]** - Wählen Sie die Option Transparenz aus.

* **[!UICONTROL Toleranz]** - Ziehen Sie den Schieberegler, um eine Toleranz zwischen 0 und 1 festzulegen:

   * **Beschneiden anhand der Farbe** - Geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie genau der Farbe entsprechen, die Sie in der Bildecke ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.

   * **Auf Transparenz basierende Beschneidung** - Geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie transparent sind. Werte, die näher an 1 liegen, ermöglichen mehr Transparenz.

## Manuelles Zuschneiden von den Seiten der Bilder

Um ein Bild manuell an den Kanten zu beschneiden, wählen Sie im Menü „Beschneiden“ die Option „Manuell“. Geben Sie dann die Anzahl an Pixeln ein, die an einer oder jeder Kante des Bilds abgeschnitten werden soll. Wie viel vom Bild abgeschnitten wird, hängt von der ppi-Einstellung (Pixel pro Zoll) in der Bilddatei ab. Angenommen, das Bild zeigt 150 ppi. Geben Sie dann die Zahl 75 in die Textfelder oben, rechts, unten und links ein. An dieser Stelle wird jede Seite zugeschnitten.

## Farbprofil auswählen

Um einen Farbraum für das Bild auszuwählen, wählen Sie eine Farbprofil -Option:

* **[!UICONTROL In sRGB konvertieren]** - Konvertiert in sRGB (Standard Red Green Blue). sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Websites.

* **[!UICONTROL Originalfarbraum beibehalten]** - Behält den ursprünglichen Farbraum bei.

* **[!UICONTROL Benutzerdefiniert von]** > **[!UICONTROL nach]** - Öffnet Menüs, damit Sie den Farbraum &quot;Konvertieren von&quot;und &quot;Konvertieren in&quot;auswählen können. Sie können einen standardmäßigen Photoshop-Farbraum oder einen Farbraum auswählen, den Sie in Adobe Dynamic Media Classic hochgeladen haben.

Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

## Masken aus Beschneidungspfad erstellen

Um eine Maske für das Bild basierend auf den Beschneidungspfadinformationen zu erstellen, wählen Sie **[!UICONTROL Maske aus Beschneidungspfad erstellen]**. Diese Option betrifft Bilder, die unter Verwendung eines Beschneidungspfads erstellt wurden.

## Scharfzeichnen eines Bildes mit Unscharfzeichnen einer Maske

Mit diesem Filter können Sie einen Scharfzeichnungsfiltereffekt für das endgültige heruntergesampelte Bild optimieren. Auf diese Weise können Sie die Intensität des Effekts, den Radius des Effekts (gemessen in Pixel) und einen Schwellenwert für den Kontrast, der ignoriert wird, steuern.

Bei diesem Effekt werden dieselben Optionen wie im Filter &quot;Unschärfemaske&quot;von Photoshop verwendet. Im Gegensatz zu dem, dass der Name impliziert, ist die „Unschärfemaske“ ein Scharfzeichnungsfilter.

Wählen Sie unter „Unschärfemaske &quot; die gewünschten Optionen aus. Die zur Verfügung stehenden Optionen sind in der folgenden Tabelle aufgeführt:

| Optionen für „Unschärfemaske“ | Beschreibung |
| --- | --- |
| Betrag | Betrag steuert den Kontrastwert, der auf die Kantenpixel angewendet wird.<br><br>Stellen Sie sich das als Intensität des Effekts vor. Es gibt einen Unterschied zwischen den Zahlenwerten von Unschärfemaske in Dynamic Media Classic und in Adobe Photoshop. Der Hauptunterschied besteht darin, dass Photoshop einen Betrag zwischen 1 % und 500 % hat. In Adobe Dynamic Media Classic liegt der Wertebereich zwischen 0,0 und 5,0. Der Wert 5,0 in Adobe Dynamic Media Classic entspricht ungefähr 500 % in Photoshop, der Wert 0,9 entspricht 90 % usw. |
| Radius | Diese Option steuert den Radius des Effekts. <br><br>Der Wertebereich ist 0-250. Der Effekt wird auf allen Pixeln im Bild ausgeführt und strahlt in alle Richtungen aus. Der Radius wird in Pixel angegeben. Um beispielsweise einen ähnlichen Scharfzeichnungseffekt für ein Bild mit 2000 × 2000 Pixel und 500 × 500 Pixel zu erhalten, legen Sie einen Radius von zwei Pixel auf dem Bild mit 2000 × 2000 Pixel fest. Legen Sie dann einen Radius-Wert von einem Pixel auf dem Bild mit 500 × 500 Pixel fest. Ein größerer Wert wird entsprechend für ein Bild mit mehr Pixeln verwendet.  |
| Schwelle | Gibt den Kontrastbereich an, der beim Anwenden des Filters „Unschärfemaske“ ignoriert werden soll. Dieser Effekt ist wichtig, damit bei Verwendung dieses Filters kein Bildrauschen entsteht. Der Schwellenwert verwendet einen Wert von 0 bis 255, was für die Anzahl der Helligkeitsschritte in einem Graustufenbild steht. 0=schwarz, 128=50 % grau und 255=weiß. <br><br>Bei einem Schwellenwert von 12 werden beispielsweise leichte Variationen der Hauttonhelligkeit ignoriert, um Rauschen zu vermeiden. Gleichzeitig wird kontrastreichen Bereichen, z. B. wo Wimpern auf die Haut treffen, Kantenkontrast hinzugefügt.<br><br>Wenn Sie z. B. ein Foto von jemandes Gesicht haben, wirkt sich die Unschärfemaske auf die kontrastreichen Teile des Bildes aus. Zum Beispiel, wo Wimpern und Haut treffen, um einen offensichtlichen Kontrastbereich zu schaffen, und die glatte Haut selbst. Selbst die glatteste Haut weist subtile Änderungen in Helligkeitswerten auf. Wenn Sie keinen Schwellenwert verwenden, akzentuiert der Filter diese subtilen Änderungen in den Hautpixeln. Dies wiederum erzeugt einen Rauscheffekt (der wahrscheinlich unerwünscht ist), während er gleichzeitig den Kontrast an den Wimpern erhöht und somit die Schärfe verbessert (wahrscheinlich wünschenswert)<br><br>Um dieses Problem zu vermeiden, wird ein Schwellenwert eingeführt, der den Filter anweist, Pixel zu ignorieren, die den Kontrast nicht wesentlich ändern, wie glatte Haut. <br><br>Beachten Sie in der zuvor gezeigten Reißverschlussgrafik die Textur neben dem Reißverschluss. Bildrauschen wird angezeigt, da die Schwellenwerte zu niedrig sind, um das Rauschen zu unterdrücken. |
| Monochrom | Wählen Sie diese Option, um die „Umschärfemaske“ auf die Gesamthelligkeit (Intensität) des Bildes anzuwenden.<br><br>Heben Sie die Auswahl auf, um die Unschärfemaske für jede Farbkomponente separat auszuwählen. |

Siehe auch [Scharfzeichnen von Bildern](sharpening-image.md#sharpening_an_image).

Siehe auch [Scharfzeichnen von Bildern in Adobe Dynamic Media und auf dem Image-Server](/help/using/assets/s7_sharpening_images.pdf).

## Hintergrund aussparen

Verwenden Sie &quot;Hintergrund aussparen&quot;, damit Sie beim Hochladen automatisch den Hintergrund eines Bildes entfernen können. Diese Technik eignet sich dazu, die Aufmerksamkeit auf ein bestimmtes Objekt zu lenken und es von einem stark ablenkenden Hintergrund abzuheben.

| Optionen für „Hintergrund aussparen“ | Beschreibung |
| --- | --- |
| Hintergrund aussparen | Wählen Sie diese Option aus, um die Funktion und die Optionen &quot;Hintergrund aussparen&quot;zu aktivieren bzw. zu aktivieren. |
| Ecke | Erforderlich.<br>Die Ecke des Bildes, mit der die auszuschneidende Hintergrundfarbe definiert wird.<br>Sie können aus <b>Oben links, unten links, Oben rechts oder unten rechts</b>. |
| Füllmethode | Erforderlich. <br>Steuert die Pixeltransparenz von der Ecke, die Sie festlegen.<br>Sie können aus den folgenden Füllmethoden wählen:<br>・ <b>Flood Fill</b> - Macht alle Pixel transparent, die der von Ihnen angegebenen Ecke entsprechen und mit ihr verbunden sind.<br>・ <b>Pixel abgleichen</b> - macht alle übereinstimmenden Pixel transparent, unabhängig von ihrer Position auf dem Bild. |
| Toleranz | Optional.<br>Steuert die zulässige Abweichung der Pixelfarbe basierend auf der Ecke, die Sie festgelegt haben.<br>Verwenden Sie den Wert 0,0, um die Pixelfarben exakt abzugleichen. Oder verwenden Sie den Wert 1,0, um die größte Variante zu ermöglichen. |

>[!MORELIKETHIS]
>
>* [Zuschneiden eines Bildes](cropping-image.md#cropping_an_image)
