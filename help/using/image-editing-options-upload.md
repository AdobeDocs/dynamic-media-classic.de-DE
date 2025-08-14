---
title: Optionen zur Bildoptimierung beim Hochladen
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
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 28%

---

# Optionen zur Bildoptimierung beim Hochladen{#image-editing-options-at-upload}

Beim Hochladen von Bilddateien, einschließlich AI-, EPS- und PSD-Dateien, können Sie folgende Bearbeitungsaktionen im Dialogfeld „Upload-Auftragsoptionen“ vornehmen:

* Beschneiden Sie den Leerraum am Rand der Bilder.
* Manuelles Beschneiden eines Bilds an den Kanten.
* Auswählen eines Farbprofils.
* Erstellen einer Maske aus einem Beschneidungspfad.
* Scharfzeichnen von Bildern mit Optionen für „Unschärfemaske“
* Hintergrund aussparen

Diese Optionen befinden sich auf der Seite Hochladen unter der Überschrift **[!UICONTROL Bildbearbeitungsoptionen]** .

## Leerraum von Bildern beschneiden

Sie können Leerraumpixel eines Bildes automatisch zuschneiden. Wählen Sie im Dialogfeld Upload-Auftragsoptionen die Option **[!UICONTROL Zuschnittsoptionen]**. Wählen Sie in **[!UICONTROL Dropdown]** Liste „Zuschneiden“ die Option **[!UICONTROL Zuschneiden]**. Anschließend können Sie folgende Optionen wählen:

* **[!UICONTROL Beschneiden basierend auf]**: Wählen Sie aus dieser Dropdown-Liste aus, ob ein Beschneiden auf Grundlage von Farbe oder Transparenz durchgeführt werden soll:

   * **[!UICONTROL Color]**: Wählen Sie die Option **[!UICONTROL Color]** aus. Wählen Sie dann aus **[!UICONTROL Dropdown-Liste]** Ecke“ die Bildecke mit der Farbe aus, die am besten der Leerraumfarbe entspricht, die Sie beschneiden möchten.

   * **[!UICONTROL Transparenz]**: Wählen Sie die Option „Transparenz“.

* **[!UICONTROL Toleranz]**: Ziehen Sie den Regler, um eine Toleranz von 0 bis 1 festzulegen:

   * **Auf Farbe basierendes Zuschneiden**: Geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie genau mit der Farbe übereinstimmen, die Sie in der Bildecke ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.

   * **Beschneiden auf der Grundlage der Transparenz**: Geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie transparent sind. Zahlen, die näher an 1 liegen, ermöglichen mehr Transparenz.

## Manuelles Zuschneiden von den Seiten der Bilder

Um ein Bild manuell an den Kanten zu beschneiden, wählen Sie im Menü „Beschneiden“ die Option „Manuell“. Geben Sie dann die Anzahl an Pixeln ein, die an einer oder jeder Kante des Bilds abgeschnitten werden soll. Wie viel vom Bild abgeschnitten wird, hängt von der ppi-Einstellung (Pixel pro Zoll) in der Bilddatei ab. Angenommen, das Bild zeigt 150 ppi. Geben Sie 75 in die Textfelder Oben, Rechts, Unten und Links ein. An dieser Stelle wird jede Seite um 0,5 Zoll abgeschnitten.

## Farbprofil auswählen

Um einen Farbraum für das Bild auszuwählen, wählen Sie eine Option Farbprofil :

* **[!UICONTROL In sRGB konvertieren]**: Konvertiert in sRGB (Standard Rot Grün Blau). sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Web-Seiten.

* **[!UICONTROL Ursprünglichen Farbraum beibehalten]**: Behält den ursprünglichen Farbraum bei.

* **[!UICONTROL Benutzerdefiniertes Formular]** > **[!UICONTROL An]**: Öffnet Menüs, in denen Sie „Konvertieren aus“ und „In Farbraum konvertieren“ auswählen können. Sie können einen standardmäßigen Photoshop-Farbraum oder einen Farbraum auswählen, den Sie in Adobe Dynamic Media Classic hochgeladen haben.

Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

## Erstellen einer Maske aus einem Schnittpfad

Um eine Maske für das Bild basierend auf den Informationen zum Schnittpfad zu erstellen, wählen Sie **[!UICONTROL Maske aus Schnittpfad erstellen]** aus. Diese Option betrifft Bilder, die unter Verwendung eines Beschneidungspfads erstellt wurden.

## Scharfzeichnen eines Bildes mit der Unscharfzeichnung „Maske“

Mit diesem Filter können Sie einen Scharfzeichnungsfiltereffekt für das endgültige, heruntergesampelte Bild fein abstimmen. Damit können Sie die Intensität des Effekts, den Radius des Effekts (gemessen in Pixel) und einen Schwellenwert für den ignorierten Kontrast steuern.

Dieser Effekt verwendet dieselben Optionen wie der Photoshop-Filter Unscharf maskieren . Im Gegensatz zu dem, dass der Name impliziert, ist die „Unschärfemaske“ ein Scharfzeichnungsfilter.

Wählen Sie unter „Unschärfemaske &quot; die gewünschten Optionen aus. Die zur Verfügung stehenden Optionen sind in der folgenden Tabelle aufgeführt:

| Optionen für „Unschärfemaske“ | Beschreibung |
| --- | --- |
| Betrag | Stärke steuert den auf die Kanten-Pixel angewendeten Kontrastwert.<br><br>Betrachten Sie dies als Intensität des Effekts. Es gibt einen Unterschied zwischen den Werten von „Unscharf maskieren“ in Dynamic Media Classic und in Adobe Photoshop. Der Hauptunterschied besteht darin, dass Photoshop einen Wertebereich von 1 % bis 500 % hat. In Adobe Dynamic Media Classic liegt der Wertebereich dagegen zwischen 0,0 und 5,0. Ein Wert von 5,0 in Adobe Dynamic Media Classic entspricht 500 % in Photoshop. Ein Wert von 0,9 entspricht 90 % usw. |
| Radius | Diese Option steuert den Radius des Effekts. <br><br>Der Wertebereich ist 0-250. Der Effekt wird auf allen Pixeln im Bild ausgeführt und strahlt in alle Richtungen aus. Der Radius wird in Pixel angegeben. Um beispielsweise einen ähnlichen Scharfzeichnungseffekt für ein Bild mit 2000 × 2000 Pixel und ein Bild mit 500 × 500 Pixel zu erhalten, legen Sie einen Radius von zwei Pixel auf dem Bild mit 2000 × 2000 Pixel fest. Legen Sie dann einen Radius-Wert von einem Pixel auf dem Bild mit 500 × 500 Pixel fest. Ein größerer Wert wird entsprechend für ein Bild mit mehr Pixeln verwendet.  |
| Schwelle | Gibt den Kontrastbereich an, der beim Anwenden des Filters „Unschärfemaske“ ignoriert werden soll. Dieser Effekt ist wichtig, damit bei Verwendung dieses Filters kein „Rauschen“ in ein Bild eintritt. Der Schwellenwert verwendet einen Wert von 0 bis 255, was für die Anzahl der Helligkeitsschritte in einem Graustufenbild steht. 0=schwarz, 128=50 % grau und 255=weiß. <br><br>Bei einem Schwellenwert von 12 werden beispielsweise leichte Variationen der Hauttonhelligkeit ignoriert, um Bildrauschen zu vermeiden, trotzdem wird kontrastreichen Bereichen, z. B. wo Wimpern auf die Haut treffen, Kantenkontrast hinzugefügt.<br><br>Wenn Sie beispielsweise ein Foto von jemandes Gesicht haben, wirkt sich die Unschärfemaske auf die kontrastreichen Teile des Bildes aus. Zum Beispiel, wo Wimpern und Haut sich treffen, um einen offensichtlichen Kontrastbereich zu schaffen, und die glatte Haut selbst. Selbst die glatteste Haut weist subtile Änderungen in Helligkeitswerten auf. Wenn Sie keinen Schwellenwert verwenden, akzentuiert der Filter diese subtilen Änderungen in den Hautpixeln. Dies wiederum erzeugt einen Rauscheffekt (der wahrscheinlich unerwünscht ist), während er gleichzeitig den Kontrast an den Wimpern erhöht und somit die Schärfe verbessert (wahrscheinlich wünschenswert)<br><br>Zur Vermeidung dieses Problems wird ein Schwellenwert verwendet, der den Filter anweist, die Pixel zu ignorieren, die den Kontrast nicht wesentlich ändern, beispielsweise bei glatter Haut. <br><br>Beachten Sie in der weiter oben gezeigten Reißverschlussgrafik die Textur neben dem Reißverschluss. Das Bildrauschen tritt auf, weil die Schwellenwerte zu niedrig sind, um das Bildrauschen zu unterdrücken. |
| Monochrom | Wählen Sie diese Option, um die „Umschärfemaske“ auf die Gesamthelligkeit (Intensität) des Bildes anzuwenden.<br><br>Deaktivieren Sie diese Option, um die Unschärfemaske auf jede Farbkomponente einzeln anzuwenden. |

Siehe auch [Scharfzeichnen eines Bildes](sharpening-image.md#sharpening_an_image).

Siehe auch [Scharfzeichnen von Bildern in Adobe Dynamic Media und Image Server](/help/using/assets/s7_sharpening_images.pdf).

## Hintergrund aussparen

Verwenden Sie den Knock-out-Hintergrund, damit Sie den Hintergrund eines Bildes beim Hochladen automatisch entfernen können. Diese Technik eignet sich dazu, die Aufmerksamkeit auf ein bestimmtes Objekt zu lenken und es von einem stark ablenkenden Hintergrund abzuheben.

| Optionen für „Hintergrund aussparen“ | Beschreibung |
| --- | --- |
| Hintergrund aussparen | Wählen Sie aus, um die Knock-out-Hintergrundfunktion und die Optionen zu aktivieren oder zu aktivieren. |
| Ecke | Erforderlich.<br>Die Bildecke, die zum Definieren der Hintergrundfarbe für den K.-o.-Effekt verwendet wird.<br>Sie können zwischen <b>oben links, unten links, oben rechts oder unten rechts</b> wählen. |
| Füllmethode | Erforderlich. <br>Steuert die Pixeltransparenz von der festgelegten Eckposition aus.<br>Sie können aus den folgenden Füllmethoden auswählen:<br>・ <b>Flutfüllung</b>: Aktiviert die Transparenz aller Pixel, die der angegebenen Ecke entsprechen und mit dieser verbunden sind.<br>・ <b>Match Pixel</b>: Macht alle übereinstimmenden Pixel transparent, unabhängig von ihrer Position auf dem Bild. |
| Toleranz | Optional.<br>Steuert den zulässigen Grad der Variation beim Farbabgleich in Pixel basierend auf der von Ihnen festgelegten Eckposition.<br>Verwenden Sie einen Wert von 0,0, um Pixelfarben genau zuzuordnen. Verwenden Sie alternativ einen Wert von 1,0, um die größte Variation zu ermöglichen. |

>[!MORELIKETHIS]
>
>* [Beschneiden eines Bildes](cropping-image.md#cropping_an_image)
