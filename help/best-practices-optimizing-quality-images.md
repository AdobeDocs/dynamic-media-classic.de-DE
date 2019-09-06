---
title: Empfohlene Verfahren zur Optimierung der Bildqualität
seo-title: Empfohlene Verfahren zur Optimierung der Bildqualität
description: 'null'
seo-description: Lernen Sie bewährte Verfahren zum Optimieren der Qualität Ihrer Bilder kennen.
uuid: 102 e 83 fe-ee 2 a -443 b-ba 92-6 ad 5 cc 3 daef 0
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/master_ files
discoiquuid: 8164466 e -2520-482 a -88 ec -6191 fdc 77 ea 3
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Empfohlene Verfahren zur Optimierung der Bildqualität{#best-practices-for-optimizing-the-quality-of-your-images}

Das Optimieren der Bildqualität kann ein sehr zeitaufwendiger Prozess sein, da viele Faktoren dazu beitragen, akzeptable Ergebnisse zu erzielen. Das Ergebnis ist teilweise subjektiv, da jede Person die Bildqualität unterschiedlich wahrnimmt. Strukturiertes Experimentieren ist der Schlüssel zum Erfolg.

Dynamic Media Classic umfasst mehr als 100 Image Serving-Befehle zum Verfeinern und Optimieren von Bildern und zum Rendern von Ergebnissen. Die folgenden Richtlinien sollen Ihnen dabei helfen, den Vorgang zu optimieren und die gewünschten Ergebnisse schnell mit nur einigen wichtigen Befehle und empfohlenen Verfahren zu erzielen.

Siehe [auch Smart-Imaging](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html).

## Empfohlene Verfahren für das Bildformat (&amp;fmt=) {#best-practices-for-image-format-fmt}

* Das JPG- oder das PNG-Format ist die beste Wahl, um Bilder in akzeptabler Qualität und handlicher Größe und Dateigröße bereitzustellen.
* Wenn kein Formatbefehl in der URL angegeben ist, wird standardmäßig das dynamische Medienserver für die Bereitstellung verwendet.
* JPG-Dateien werden in einem Verhältnis von 10:1 komprimiert und produzieren so in der Regel kleinere Bilddateigrößen. PNG-Dateien werden in einem Verhältnis von etwa 2:1 komprimiert, mit Ausnahme von Fällen, bei denen das Bild einen weißen Hintergrund enthält. Dennoch lässt sich sagen, dass PNG-Dateien grundsätzlich größer sind als JPG-Dateien.
* JPG verwendet eine verlustbehaftete Komprimierung. Dies bedeutet, dass Bildelemente (Pixel) bei der Komprimierung verworfen werden. Im Gegensatz dazu verwendet PNG eine verlustfreie Komprimierung.
* JPG komprimiert Fotografien häufig mit einer höheren Genauigkeit als künstliche Bilder mit scharfen Kanten und hohem Kontrast.
* Wenn die Bilder transparente Anteile enthalten, sollte das PNG-Format verwendet werden, da JPG keine Transparenz unterstützt.

As a best practice for image format, start with the most common setting `&fmt=JPG`.

## Empfohlene Verfahren für die Bildgröße {#best-practices-for-image-size}

Die dynamische Verringerung der Bildgröße ist eine der häufigsten Aufgaben, die das Image Serving von dynamischen Medien durchführt. Sie umfasst die Angabe der Größe und, optional, welcher Modus zur Verringerung der Abtastrate (Downsampling) zum Herunterskalieren verwendet werden soll.

* Für die Bildgrößenänderung ist der beste und einfachste Ansatz die Verwendung `&wid=<value>` und `&hei=<value>` einfach `&hei=<value>`. Diese Parameter legen die Bildbreite automatisch in der Übereinstimmung mit dem Seitenverhältnis fest.
* `&resMode=<value>` steuert den Algorithmus, der zum Downsampling verwendet wird. Beginnen `&resMode=sharp2`Sie mit. Dieser Wert bietet die beste Bildqualität. While using the downsampling value `=bilin` is faster, it often results in the aliasing of artifacts.

Als `&wid=<value>&hei=<value>&resMode=sharp2` Best Practice für Bildgrößenänderung, `&hei=<value>&resMode=sharp2`

## Empfohlene Verfahren für das Scharfzeichnen von Bildern {#best-practices-for-image-sharpening}

Das Scharfzeichnen von Bildern ist der komplexeste Aspekt beim Bearbeiten von Bildern für Ihre Website. Hier werden auch die meisten Fehler begangen. Nehmen Sie sich die Zeit, mehr darüber zu erfahren, wie Scharfzeichnen und Unschärfemaske in Dynamic Media Classic funktioniert, indem Sie auf die folgenden hilfreichen Ressourcen verweisen:

Best practices white paper [Sharpening images in Adobe Scene7 Publishing System and on Image Server](https://marketing.adobe.com/resources/help/en_US/s7/sharpening/s7_sharpening_images.pdf).

On Adobe TV, watch [Sharpening an image with unsharp mask](https://tv.adobe.com/watch/visual-design-cs6/sharpening-an-image-with-unsharp-mask/).

Mit Dynamic Media Classic können Sie Bilder beim Erfassen, bei der Auslieferung oder beidem scharfzeichnen. In den meisten Fällen sollten Sie Bilder jedoch nur mit einer der beiden Methoden scharfzeichnen, nicht mit beiden. Das Scharfzeichnen von Bildern bei der Auslieferung, auf einer URL, bietet in der Regel die besten Ergebnisse.

Es gibt zwei Methoden zum Scharfzeichnen:

* Simple sharpening ( `&op_sharpen`) - Similar to the sharpen filter used in Photoshop, simple sharpening applies basic sharpening to the final view of the image following dynamic resizing. Diese Methode kann jedoch nicht vom Benutzer konfiguriert werden. The best practice is to not use `&op_sharpen` unless required.
* Unsharp masking ( `&op_USM`) - Unsharp masking is an industry standard sharpening filter. Wir empfehlen, beim Scharfzeichnen von Bilder mit der Unschärfemaske die folgenden Richtlinien zu beachten. Mit der Unschärfemaske können Sie die folgenden drei Parameter steuern:

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5, Stärke des Effekts.)
      * `radius` (0 bis 250, die Breite der „Scharfzeichnen-Linien“, die um das scharfgezeichnete Objekt gezogen werden, in Pixel gemessen.)

         Keep in mind that the parameters `radius` and `amount` work against each other. Reducing `radius` can be compensated by increasing `amount`. `Radius` ermöglicht eine bessere Kontrolle, da ein geringer Wert nur die Kantenpixel scharfzeichnet, während bei einem hohen Wert ein breiter Pixelbereich scharfgezeichnet wird.

      * `threshold` (0-255, Empfindlichkeit des Effekts.)

         Dieser Parameter legt fest, wie stark sich die scharfgezeichneten Pixel von dem sie umgebenden Bereich unterscheiden müssen, damit sie als Kantenpixel erkannt und vom Filter scharfgezeichnet werden. Der Schwellenwert hilft dabei, das übermäßige Scharfzeichnen von Bereichen mit ähnlichen Farben zu vermeiden, z. B. bei Hauttönen. Beispiel: Bei einem Schwellenwert von 12 werden leichte Variationen der Hauttonhelligkeit ignoriert, um kein Rauschen hinzuzufügen, aber dennoch wird kontrastreichen Bereichen (z. B. wo Wimpern auf die Haut treffen) ein Kantenkontrast hinzugefügt.
      Weitere Informationen, wie Sie diese drei Parameter einrichten, einschließlich den empfohlenen Verfahren für die Verwendung der Filter, finden Sie in den folgenden Ressourcen:

      Dynamisches Media Classic-Hilfethema beim [Scharfzeichnen eines Bildes](https://help.adobe.com/en_US/scene7/using/WS389B162D-2981-41e5-9253-15D22D2ECBC8.html).

      Best practices white paper [Sharpening images in Adobe Scene7 Publishing System and on Image Server](https://marketing.adobe.com/resources/help/en_US/s7/sharpening/s7_sharpening_images.pdf).

   * Mit Dynamic Media Classic können Sie auch einen vierten Parameter steuern: Monochrom ( `0,1`). Dieser Parameter stellt fest, ob die Unschärfemaske unter Verwendung des Werts `0` separat auf jede Farbkomponente oder unter Verwendung des Werts `1` auf die Gesamthelligkeit/Intensität angewendet wurde.


Wir empfehlen, mit dem Parameter „Radius“ der Unschärfemaske zu beginnen. Sie können beispielsweise mit den folgenden Radius-Einstellungen beginnen:

* Website: 0,2 bis 0,3 Pixel
* Fotografischer Druck (250 bis 300 ppi): 0,3 bis 0,5 Pixel
* Offsetdruck (266 bis 300 ppi): 0,7 bis 1,0 Pixel
* Leinwanddruck (150 ppi): 1,5 bis 2,0 Pixel

Erhöhen Sie diesen Wert stufenweise von 1,75 bis 4. Wenn das Ergebnis des Scharfzeichnens Ihre Anforderungen noch nicht erfüllt, erhöhen Sie den Radius-Wert um eine Dezimalstelle und führen Sie den „Betrag“ erneut von 1,75 bis 4 aus. Wiederholen Sie diesen Vorgang bei Bedarf.

Lassen Sie die Parametereinstellung „Monochrom“ auf 0.

## Empfohlene Verfahren für die JPEG-Komprimierung (&amp;qlt=) {#best-practices-for-jpeg-compression-qlt}

* Dieser Parameter steuert die Qualität der JPG-Kodierung. Ein höherer Wert bedeutet eine höhere Bildqualität, jedoch auch eine größere Datei; entsprechend bedeutet ein niedrigerer Wert eine geringere Bildqualität, aber eine kleinere Dateigröße. Der Bereich für diesen Parameter ist 0 bis 100.
* Setzen Sie den Wert zur Optimierung der Qualität nicht auf 100. Der Unterschied zwischen einer Einstellung von 90 oder 95 und 100 ist fast nicht mehr wahrnehmbar, aber der Wert 100 vergrößert die Bilddatei unnötig. Therefore, to optimize for quality but avoid image files becoming too large, set the `qlt=` value to 90 or 95.
* To optimize for a small image file size but keep image quality at an acceptable level, set the `qlt=` value to 80. Werte unter 70 bis 75 führen zu einer deutlichen Verschlechterung der Bildqualität.
* As a best practice, to stay in the middle, set the `qlt=` value to 85 to stay in the middle.
* Verwenden des Chroma-Flags in `qlt=`

   * The `qlt=` parameter has a second setting that lets you turn on RGB chromaticity downsampling using the normal value `,0` (default), or turn it off using the value `,1`.
   * Der Einfachheit halber sollten Sie das RGB-Farbart-Downsampling zunächst deaktivieren ( `,1`). Diese Einstellung führt in der Regel zu einer besseren Bildqualität, insbesondere bei künstlichen Bilder mit vielen scharfen Kanten und hohem Kontrast.

Unsere Empfehlung für die JPG-Komprimierung ist der Wert `&qlt=85,0`.

## Empfohlene Verfahren für die JPEG-Größenanpassung (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

`jpegSize` ist ein sehr nützlicher Parameter, wenn Sie sicherstellen möchten, dass ein Bild für die Bereitstellung für Geräte mit einem begrenzten Speicherplatz eine bestimmte Größe nicht überschreitet.

* Dieser Parameter wird in Kilobytes ( `jpegSize=<size_in_kilobytes>`) festgelegt. Er legt die maximal zulässige Größe für Bildbereitstellung fest.
* `&jpegSize=` mit dem JPG-Komprimierungsparameter `&qlt=`interagiert. If the JPG response with the specified JPG compression parameter ( `&qlt=`) does not exceed the `jpegSize` value, the image is returned with `&qlt=` as defined. Otherwise, `&qlt=` is gradually decreased until the image fits in the maximum allowed size, or until the system determines it cannot fit and returns an error.

As a best practice, set `&jpegSize=` and add the parameter `&qlt=` if you are delivering JPG images to devices with limited memory.

## Zusammenfassung der empfohlenen Verfahren {#best-practices-summary}

Um eine hohe Bildqualität bei einer kleinen Dateigröße zu erreichen, sollten Sie mit der folgenden Parameterkombination beginnen:

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Diese Einstellungskombination führt in den meisten Situationen zu hervorragenden Ergebnissen.

Wenn eine weitere Optimierung für das Bild erforderlich ist, passen die Parameter für das Scharfzeichnen (Unschärfemaske) schrittweise an, indem Sie den Radiuswert auf 0,2 oder 0,3 einstellen. Anschließend können Sie den Betrag schrittweise von 1,75 bis maximal 4 erhöhen (entspricht einer Einstellung von 400 % in Photoshop). Prüfen Sie, ob das gewünschte Ergebnis erzielt wurde.

Wenn die gewünschten Ergebnisse für das Scharfzeichnen noch nicht erreicht wurden, erhöhen Sie den Radius in Dezimalschritten. Beginnen Sie für jeden Dezimalschnitt wieder mit einem Betrag von 1,75 und erhöhen Sie den Wert schrittweise bis maximal 4. Wiederholen Sie diesen Vorgang, bis das gewünschte Ergebnis erreicht ist. Obwohl die oben aufgeführten Werte einen von Kreativstudios erprobten Ansatz bieten, können Sie auch mit anderen Werten beginnen und andere Strategien verfolgen. Die Zufriedenheit mit den erzielten Ergebnisse ist immer subjektiv, aus diesem Grund ist strukturiertes Experimentieren der Schlüssel zum Erfolg.

Wenn Sie experimentieren, können Ihnen die folgenden allgemeinen Empfehlungen helfen, den Vorgang zu optimieren:

* Testen und testen Sie verschiedene Parameter in Echtzeit, entweder direkt auf einer Dynamic Media Classic-URL oder über die Scene 7 Publishing System-Bildkorrekturfunktion, die Echtzeitvorschauen für Anpassungen bereitstellt.
* Denken Sie daran, dass Sie dynamische Medienserver-Image Serving-Befehle in eine Bildvorgabe gruppieren können. An image preset is basically URL command macros with custom preset names such as `$thumb_low$` and `&product_high$`. Der benutzerdefinierte Vorgabename in einem URL-Pfad ruft diese Voreinstellungen auf. Diese Funktionen helfen Ihnen dabei, die Befehls- und Qualitätseinstellungen für verschiedene Verwendungsmuster der Bildern auf Ihrer Website zu verwalten und verkürzen die Gesamtlänge der URLs.
* Dynamic Media Classic bietet zudem erweiterte Möglichkeiten zur Optimierung der Bildqualität, z. B. zum Anwenden von Scharfzeichnen von Bildern beim Erfassen. Für solche Fälle, bei denen dies eine Option zur Feineinstellung und Optimierung der Darstellungsergebnisse ist, bieten die Adobe Professional Services weitere spezielle Tipps und empfohlene Verfahren an.

