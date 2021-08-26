---
title: Bildoptimierungsoptionen beim Hochladen
description: Erfahren Sie mehr über die Bildoptimierungsoptionen, die zum Zeitpunkt des Uploads in Dynamic Media Classic verfügbar sind.
uuid: 0912ae6f-41c9-41b5-94d1-e266face782e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: d3f21cdf-2cb3-46e8-955a-b8daf0b233bc
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 2d9fc6d8-973f-4aaa-bc2c-b49cda2cde58
source-git-commit: 20a5e54a9f3fa442d3a993afae07aa5b1b13e9c3
workflow-type: tm+mt
source-wordcount: '1161'
ht-degree: 54%

---

# Bildoptimierungsoptionen beim Hochladen{#image-editing-options-at-upload}

Beim Hochladen von Bilddateien, einschließlich AI-, EPS- und PSD-Dateien, können Sie folgende Bearbeitungsaktionen im Dialogfeld „Upload-Auftragsoptionen“ vornehmen:

* Beschneiden des Bilds zum Entfernen weißer Flächen am Rand.
* Manuelles Beschneiden eines Bilds an den Kanten.
* Auswählen eines Farbprofils.
* Erstellen einer Maske aus einem Beschneidungspfad.
* Scharfzeichnen von Bildern mit Optionen für „Unschärfemaske“
* Hintergrund aussparen

Diese Optionen befinden sich auf der Seite Hochladen unter der Überschrift **[!UICONTROL Bildbearbeitungsoptionen]** .

## Leerraum aus Bildern beschneiden

Um automatisch Leerraum-Pixel aus einem Bild zu beschneiden, wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL Zuschnittsoptionen]** aus. Wählen Sie in der Dropdownliste **[!UICONTROL Zuschneiden]** **[!UICONTROL Zuschneiden]** aus. Anschließend können Sie folgende Optionen wählen:

* **[!UICONTROL Entfernen basierend auf]**  - Wählen Sie aus dieser Dropdownliste aus, ob Sie basierend auf Farbe oder Transparenz zuschneiden möchten:

   * **[!UICONTROL Farbe]**  - Wählen Sie die  **** Farboption aus. Wählen Sie dann aus der Dropdownliste **[!UICONTROL Ecke]** die Ecke des Bildes mit der Farbe aus, die am besten der zu beschneidenden Leerraum-Farbe entspricht.

   * **[!UICONTROL Transparenz]**  - Wählen Sie die Option &quot;Transparenz&quot;.

* **[!UICONTROL Toleranz]**  - Ziehen Sie den Regler, um eine Toleranz von 0 bis 1 festzulegen:

   * **Beschneiden anhand der Farbe**  - Legen Sie den Wert 0 fest, damit Pixel nur dann abgeschnitten werden, wenn sie genau der Farbe entsprechen, die Sie in der Bildecke ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.

   * **Auf Transparenz basierendes Zuschneiden**  - Geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie transparent sind. Werte, die näher an 1 liegen, erlauben mehr Transparenz.

## Manuelles Beschneiden eines Bilds an den Kanten

Um ein Bild manuell an den Kanten zu beschneiden, wählen Sie im Menü „Beschneiden“ die Option „Manuell“. Geben Sie dann die Anzahl an Pixeln ein, die an einer oder jeder Kante des Bilds abgeschnitten werden soll. Wie viel vom Bild abgeschnitten wird, hängt von der ppi-Einstellung (Pixel pro Zoll) in der Bilddatei ab. Wenn das Bild beispielsweise eine Auflösung von 150 ppi hat und Sie in den Textfeldern „Oben“, „Rechts“, „Unten“ und „Links“ jeweils den Wert 75 eingeben, wird an jeder Kante ein halber Zoll (ca. 1,75 cm) abgeschnitten.

## Auswählen eines Farbprofils

Um einen Farbraum für das Bild auszuwählen, wählen Sie eine Farbprofil -Option:

* **[!UICONTROL In sRGB konvertieren]**  - Konvertiert in sRGB (Standard Red Green Blue). sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Websites.

* **[!UICONTROL Originalfarbraum beibehalten]**  - Behält den ursprünglichen Farbraum bei.

* **[!UICONTROL Benutzerdefiniert von]**  >  **[!UICONTROL in]**  - Öffnet die Menüs, damit Sie einen Farbraum vom Typ &quot;Konvertieren von&quot;und &quot;Konvertieren in&quot;auswählen können. Sie können einen standardmäßigen Photoshop-Farbraum oder einen Farbraum auswählen, den Sie in Dynamic Media Classic hochgeladen haben.

Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

## Erstellen einer Maske aus einem Beschneidungspfad

Um eine Maske für das Bild basierend auf den Beschneidungspfadinformationen zu erstellen, wählen Sie **[!UICONTROL Maske aus Beschneidungspfad erstellen]** aus. Diese Option betrifft Bilder, die unter Verwendung eines Beschneidungspfads erstellt wurden.

## Scharfzeichnen eines Bildes mit &quot;Unscharfzeichnen einer Maske&quot;

Mit diesem Filter können Sie einen Scharfzeichnungsfiltereffekt für das endgültige heruntergesampelte Bild optimieren. Auf diese Weise können Sie die Intensität des Effekts, den Radius des Effekts (gemessen in Pixel) und einen Schwellenwert für den ignorierten Kontrast steuern.

Dieser Effekt verwendet die gleichen Optionen wie der Photoshop-Filter „Unscharf maskieren“. Im Gegensatz zu dem, dass der Name impliziert, ist die „Unschärfemaske“ ein Scharfzeichnungsfilter.

Wählen Sie unter „Unschärfemaske &quot; die gewünschten Optionen aus. Die zur Verfügung stehenden Optionen sind in der folgenden Tabelle aufgeführt:

| Optionen für „Unschärfemaske“ | Beschreibung |
| --- | --- |
| Betrag | Gibt den Kontrastgrad an, der auf die Pixel an den Rändern angewendet wird. <br><br>Sie können sich die Auswirkung der Option „Betrag“ wie ein Maß für die Filterintensität vorstellen. Der Hauptunterschied zwischen den Zahlenwerten von Unschärfemaske in Dynamic Media Classic und den Zahlenwerten in Adobe Photoshop besteht darin, dass Photoshop über einen Mengenbereich von 1 % bis 500 % verfügt. In Dynamic Media Classic liegt der Wertebereich zwischen 0,0 und 5,0. Ein Wert von 5,0 in Dynamic Media Classic entspricht ungefähr 500 % in Photoshop. Ein Wert von 0,9 entspricht 90 % usw. |
| Radius | Diese Option steuert den Radius des Effekts. <br><br>Der Wertebereich beträgt 0 bis 250. Der Effekt wird auf allen Pixeln im Bild ausgeführt und strahlt in alle Richtungen aus. Der Radius wird in Pixel angegeben. Um beispielsweise einen ähnlichen Scharfzeichnungseffekt für ein Bild mit 2000 x 2000 Pixel und ein Bild mit 500 x 500 Pixel zu erhalten, legen Sie einen Radius von zwei Pixel auf dem Bild mit 2000 x 2000 Pixel fest. Legen Sie dann einen Radius-Wert von einem Pixel auf dem 500 x 500 Pixelbild fest. Ein größerer Wert wird entsprechend für ein Bild mit mehr Pixeln verwendet.  |
| Schwelle | Gibt den Kontrastbereich an, der beim Anwenden des Filters „Unschärfemaske“ ignoriert werden soll. Dieser Effekt ist wichtig, damit bei Verwendung dieses Filters kein Bildrauschen entsteht. Der Schwellenwert verwendet einen Wert von 0 bis 255, was für die Anzahl der Helligkeitsschritte in einem Graustufenbild steht. 0=schwarz, 128=50 % grau und 255=weiß. <br><br>Beispiel: Ein Schwellenwert von 12 ignoriert leichte Variationen der Hauttonhelligkeit, um kein Rauschen hinzuzufügen, fügt aber trotzdem einen Kantenkontrast zu kontrastreichen Bereichen (z. B. wo Wimpern auf die Haut treffen) hinzu. <br><br>Wenn Sie z. B. ein Foto von jemandes Gesicht haben, wirkt sich die Unschärfemaske auf die kontrastreichen Teile des Bildes aus. Zum Beispiel, wo Wimpern und Haut treffen, um einen offensichtlichen Kontrastbereich zu schaffen, und die glatte Haut selbst. Selbst die glatteste Haut weist subtile Änderungen in Helligkeitswerten auf. Wenn Sie keinen Schwellenwert verwenden, akzentuiert der Filter diese subtilen Änderungen in den Hautpixeln. Dies wiederum erzeugt einen Rauscheffekt (der wahrscheinlich unerwünscht ist), während er gleichzeitig den Kontrast an den Wimpern erhöht und somit die Schärfe verbessert (wahrscheinlich wünschenswert)<br><br>Um dieses Problem zu vermeiden, verwenden Sie einen Schwellenwert, bei dem der Filter Pixel ignoriert, die den Kontrast nicht drastisch ändern, wie z. B. glatte Haut. <br><br>Achten Sie in der weiter oben gezeigten Reißverschlussgrafik auf die Textur neben dem Reißverschluss. Hier ist Bildrauschen erkennbar, weil die Schwellenwerte zu niedrig waren, um das Bildrauschen zu unterdrücken. |
| Monochrom | Wählen Sie diese Option, um die „Umschärfemaske“ auf die Gesamthelligkeit (Intensität) des Bildes anzuwenden.<br><br>Deaktivieren Sie diese Option, um die „Unschärfemaske“ separat für jede Farbkomponente anzuwenden. |

Siehe auch [Scharfzeichnen eines Bildes](sharpening-image.md#sharpening_an_image).

Siehe auch [Scharfzeichnen von Bildern in Adobe Dynamic Media und auf Image-Server](/help/assets/s7_sharpening_images.pdf).

## Hintergrund aussparen

Mit der Option „Hintergrund aussparen“ können Sie den Hintergrund eines Bildes automatisch entfernen, wenn Sie das Bild hochladen. Diese Technik eignet sich dazu, die Aufmerksamkeit auf ein bestimmtes Objekt zu lenken und es von einem stark ablenkenden Hintergrund abzuheben.

| Optionen für „Hintergrund aussparen“ | Beschreibung |
| --- | --- |
| Hintergrund aussparen | Wählen Sie diese Option aus, um die Funktion und die Optionen &quot;Hintergrund aussparen&quot;zu aktivieren bzw. zu aktivieren. |
| Ecke | Erforderlich.<br>Die Ecke des Bildes, mit der die auszusparende Hintergrundfarbe definiert wird.<br>Sie können zwischen <b>Links oben, Links unten, Rechts oben oder Rechts unten</b> wählen.  |
| Füllmethode | Erforderlich. <br>Legt die Pixeltransparenz der von Ihnen gewählten „Ecke“ fest.<br>Sie können aus den folgenden Füllmethoden wählen:<br> ・  <b>Flood Fill</b>  - Macht alle Pixel transparent, die mit der von Ihnen angegebenen Ecke übereinstimmen und mit ihr verbunden sind.<br>• <b>Pixel abgleichen</b> – Macht alle entsprechenden Pixel transparent, unabhängig von ihrer Position auf dem Bild. |
| Toleranz | Optional.<br>Legt den zulässigen Betrag für die Abweichung von der Pixelfarbe fest, basierend von der „Ecke“, die Sie ausgewählt haben.<br>Bei einem Wert von 0,0 muss die Pixelfarbe exakt entsprechen. Ein Wert von 1,0 steht für die größtmögliche Abweichung. |

>[!MORELIKETHIS]
>
>* [Bilder zuschneiden](cropping-image.md#cropping_an_image)

