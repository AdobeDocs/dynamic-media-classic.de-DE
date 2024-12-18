---
title: Empfohlene Verfahren zur Optimierung der Bildqualität
description: Erfahren Sie mehr über Best Practices zur Optimierung der Bildqualität.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 3c50e706-b9ed-49db-8c08-f179de52b9cf
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 40%

---

# Empfohlene Verfahren zur Optimierung der Bildqualität{#best-practices-for-optimizing-the-quality-of-your-images}

Die Optimierung der Bildqualität kann viel Zeit in Anspruch nehmen. Viele Faktoren tragen dazu bei, akzeptable Ergebnisse zu erzielen. Das Ergebnis ist teilweise subjektiv, da jede Person die Bildqualität unterschiedlich wahrnimmt. Strukturiertes Experimentieren ist der Schlüssel zum Erfolg.

Adobe Dynamic Media Classic umfasst mehr als 100 Bildbereitstellungsbefehle zum Optimieren und Optimieren von Bildern und zum Rendern von Ergebnissen. Die folgenden Richtlinien sollen Ihnen dabei helfen, den Vorgang zu optimieren und die gewünschten Ergebnisse schnell mit nur einigen wichtigen Befehle und empfohlenen Verfahren zu erzielen.

Siehe auch [Smart Imaging](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/imaging-faq).

>[!TIP]
>
>Probieren Sie die Vorteile von Dynamic Media-Bildmodifikatoren und der intelligenten Bildbearbeitung mithilfe von Dynamic Media ([_)_](https://snapshot.scene7.com/).
>
> „Momentaufnahme“ ist ein visuelles Demonstrationswerkzeug, das die Leistungsfähigkeit von Dynamic Media für eine optimierte und dynamische Bildbereitstellung veranschaulicht. Experimentieren Sie mit Testbildern oder Dynamic Media-URLs, damit Sie die Ausgabe verschiedener Dynamic Media-Bildmodifikatoren visuell beobachten können, und optimieren Sie die intelligente Bildbearbeitung auf Folgendes:
>
>* Dateigröße (mit WebP- und AVIF-Bereitstellung)
>* Netzwerkbandbreite
>* DPR (Device Pixel Ratio)
>
>Um zu erfahren, wie einfach es ist, „Momentaufnahme“ zu verwenden[ spielen Sie das Schulungsvideo zu Momentaufnahmen ](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot) (3 Minuten und 17 Sekunden).


## Empfohlene Verfahren für das Bildformat (&amp;fmt=) {#best-practices-for-image-format-fmt}

* Das JPG- oder das PNG-Format ist die beste Wahl, um Bilder in akzeptabler Qualität und handlicher Größe und Dateigröße bereitzustellen.
* Wenn in der URL kein Formatbefehl angegeben wird, wird für die Bereitstellung standardmäßig JPG für Dynamic Media Image Serving verwendet.
* JPG-Dateien werden in einem Verhältnis von 10:1 komprimiert und produzieren so in der Regel kleinere Bilddateigrößen. PNG wird mit einem Verhältnis von etwa 2:1 komprimiert, außer manchmal, wenn Bilder einen leeren Hintergrund enthalten. Dennoch lässt sich sagen, dass PNG-Dateien grundsätzlich größer sind als JPG-Dateien.
* JPG verwendet eine verlustbehaftete Komprimierung. Dies bedeutet, dass Bildelemente (Pixel) bei der Komprimierung verworfen werden. Im Gegensatz dazu verwendet PNG eine verlustfreie Komprimierung.
* JPG komprimiert Fotografien häufig mit einer höheren Genauigkeit als künstliche Bilder mit scharfen Kanten und hohem Kontrast.
* Wenn die Bilder transparente Anteile enthalten, sollte das PNG-Format verwendet werden, da JPG keine Transparenz unterstützt.

Beginnen Sie als Best Practice für das Bildformat mit den häufigsten `&fmt=JPG`.

## Empfohlene Verfahren für die Bildgröße {#best-practices-for-image-size}

Die dynamische Reduzierung der Bildgröße ist eine der häufigsten Aufgaben, die von Dynamic Media Image Serving ausgeführt werden. Sie umfasst die Angabe der Größe und, optional, welcher Modus zur Verringerung der Abtastrate (Downsampling) zum Herunterskalieren verwendet werden soll.

* Für die Bildgröße ist der beste und einfachste Ansatz die Verwendung von `&wid=<value>` und `&hei=<value>` oder einfach nur `&hei=<value>`. Diese Parameter legen die Bildbreite automatisch in der Übereinstimmung mit dem Seitenverhältnis fest.
* `&resMode=<value>` steuert den Algorithmus für die Neuberechnung. Beginnen Sie mit `&resMode=sharp2`. Dieser Wert bietet die beste Bildqualität. Während die Verwendung des Downsampling-Werts `=bilin` schneller ist, führt dies oft zum Aliasing von Artefakten.

Verwenden Sie als Best Practice für die Bildgröße `&wid=<value>&hei=<value>&resMode=sharp2` oder `&hei=<value>&resMode=sharp2`

## Empfohlene Verfahren für das Scharfzeichnen von Bildern {#best-practices-for-image-sharpening}

Das Scharfzeichnen von Bildern ist der komplexeste Aspekt beim Bearbeiten von Bildern für Ihre Website. Hier werden auch die meisten Fehler begangen. Nehmen Sie sich die Zeit und machen Sie sich mit der Funktionsweise von Scharfzeichnung und Unschärfemaske in Adobe Dynamic Media Classic vertraut, indem Sie die folgenden hilfreichen Ressourcen lesen:

Whitepaper mit Best Practices [Scharfzeichnen von Bildern in Adobe Dynamic Media Classic und auf Image Server](/help/using/assets/s7_sharpening_images.pdf).

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

Mit Adobe Dynamic Media Classic können Sie Bilder bei der Aufnahme, bei der Bereitstellung oder bei beidem scharfzeichnen. Normalerweise können Sie Bilder jedoch nur mit der einen oder der anderen Methode scharfzeichnen, jedoch nicht mit beiden. Das Scharfzeichnen von Bildern bei der Auslieferung, auf einer URL, bietet in der Regel die besten Ergebnisse.

Es gibt zwei Methoden zum Scharfzeichnen von Bildern:

* Einfaches Scharfzeichnen (`&op_sharpen`): Ähnlich wie der in Photoshop verwendete Scharfzeichnungsfilter wird beim einfachen Scharfzeichnen nach der dynamischen Größenanpassung eine einfache Scharfzeichnung auf die endgültige Ansicht des Bildes angewendet. Diese Methode kann jedoch nicht vom Benutzer konfiguriert werden. Es empfiehlt sich, die Verwendung von `&op_sharpen` zu vermeiden, sofern dies nicht erforderlich ist.
* Unschärfemaske ( `&op_USM`): Unschärfemaske ist ein Branchenstandard-Filter für das Scharfzeichnen. Wir empfehlen, beim Scharfzeichnen von Bilder mit der Unschärfemaske die folgenden Richtlinien zu beachten. Mit der Unschärfemaske können Sie die folgenden drei Parameter steuern:

   * `&op_sharpen=amount,radius,threshold`

      * `amount` (0-5, Stärke des Effekts.)
      * `radius` (0-250, Breite der „Scharfzeichnungslinien“, die um das scharfgezeichnete Objekt gezeichnet werden, gemessen in Pixel.)

        Beachten Sie, dass die Parameter `radius` und `amount` gegeneinander arbeiten. Eine Verringerung der `radius` kann durch eine Erhöhung der `amount` ausgeglichen werden. `Radius` ermöglicht eine feinere Steuerung, da ein niedrigerer Wert nur die Kanten-Pixel schärft, während ein höherer Wert ein breiteres Pixelband schärft.

      * `threshold` (0-255, Empfindlichkeit der Wirkung.)

        Dieser Parameter legt fest, wie stark sich die scharfgezeichneten Pixel von dem sie umgebenden Bereich unterscheiden müssen, damit sie als Kantenpixel erkannt und vom Filter scharfgezeichnet werden. Der Schwellenwert hilft dabei, das übermäßige Scharfzeichnen von Bereichen mit ähnlichen Farben zu vermeiden, z. B. bei Hauttönen. Bei einem Schwellenwert von 12 werden beispielsweise leichte Variationen der Hauttonhelligkeit ignoriert, um kein „Rauschen“ zu erzeugen, trotzdem wird kontrastreichen Bereichen, z. B. wo Wimpern auf die Haut treffen, Kantenkontrast hinzugefügt.

        Weitere Informationen zum Festlegen dieser drei Parameter, einschließlich Best Practices für den Filter, finden Sie unter [Scharfzeichnen von Bildern in Adobe Dynamic Media Classic und auf dem Bildserver](/help/using/assets/s7_sharpening_images.pdf).

      * Mit Adobe Dynamic Media Classic können Sie auch einen vierten Parameter steuern: monochrome ( `0,1`). Dieser Parameter bestimmt, ob die Unschärfemaske auf jede Farbkomponente separat (mit dem Wert `0`) oder auf die Bildhelligkeit/-intensität (mit dem Wert `1`) angewendet wird.

Wir empfehlen, mit dem Parameter „Radius“ der Unschärfemaske zu beginnen. Sie können beispielsweise mit den folgenden Radius-Einstellungen beginnen:

* Website: 0,2 bis 0,3 Pixel
* Fotografischer Druck (250 bis 300 ppi): 0,3 bis 0,5 Pixel
* Offsetdruck (266 bis 300 ppi): 0,7 bis 1,0 Pixel
* Leinwanddruck (150 ppi): 1,5 bis 2,0 Pixel

Erhöhen Sie diesen Wert stufenweise von 1,75 bis 4. Wenn das Ergebnis des Scharfzeichnens Ihre Anforderungen noch nicht erfüllt, erhöhen Sie den Radius-Wert um eine Dezimalstelle und führen Sie den „Betrag“ erneut von 1,75 bis 4 aus. Wiederholen Sie diesen Vorgang bei Bedarf.

Lassen Sie die Parametereinstellung „Monochrom“ auf 0.

## Best Practices für die JPEG-Komprimierung (`&qlt=`) {#best-practices-for-jpeg-compression-qlt}

* Dieser Parameter steuert die Qualität der JPG-Kodierung. Ein höherer Wert bedeutet eine höhere Bildqualität, jedoch auch eine größere Datei; entsprechend bedeutet ein niedrigerer Wert eine geringere Bildqualität, aber eine kleinere Dateigröße. Der Bereich für diesen Parameter ist 0 bis 100.
* Setzen Sie den Wert zur Optimierung der Qualität nicht auf 100. Der Unterschied zwischen 90 bzw. 95 und 100 ist kaum wahrnehmbar. 100 erhöht jedoch unnötigerweise die Größe der Bilddatei. Um die Qualität zu optimieren, aber zu große Bilddateien zu vermeiden, setzen Sie daher den `qlt=` auf 90 oder 95.
* Um eine kleine Bilddateigröße zu optimieren, aber die Bildqualität auf einem akzeptablen Niveau zu halten, setzen Sie den `qlt=` auf 80. Werte unter 70 bis 75 führen zu einer deutlichen Verschlechterung der Bildqualität.
* Um in der Mitte zu bleiben, empfiehlt es sich, den `qlt=` auf 85 festzulegen, damit die Mitte beibehalten wird.
* Verwenden der Chroma-Markierung in `qlt=`

   * Der `qlt=` Parameter verfügt über eine zweite Einstellung, mit der Sie das RGB-Chromatizitäts-Downsampling mit der `,0` Normalwert (Standard) aktivieren oder mit der `,1` Wert ausschalten können.
   * Um die Sache zu vereinfachen, starten Sie mit RGB-Chromatizitäts-Downsampling ausgeschaltet ( `,1`). Diese Einstellung führt in der Regel zu einer besseren Bildqualität, insbesondere bei künstlichen Bilder mit vielen scharfen Kanten und hohem Kontrast.

Als Best Practice für die JPG-Komprimierung verwenden Sie `&qlt=85,0`.

## Empfohlene Verfahren für die JPEG-Größenanpassung (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

Der Parameter `jpegSize` ist nützlich, wenn Sie garantieren möchten, dass ein Bild eine bestimmte Größe für die Bereitstellung an Geräten mit begrenztem Speicher nicht überschreitet.

* Dieser Parameter wird in Kilobyte ( `jpegSize=<size_in_kilobytes>`) festgelegt. Er legt die maximal zulässige Größe für Bildbereitstellung fest.
* `&jpegSize=` interagiert mit dem JPG-Komprimierungsparameter `&qlt=`. Wenn die JPG-Antwort mit dem angegebenen JPG-Komprimierungsparameter (`&qlt=`) den `jpegSize` nicht überschreitet, wird das Bild mit dem definierten `&qlt=` zurückgegeben. Andernfalls wird die `&qlt=` schrittweise verringert, bis das Bild in die maximal zulässige Größe passt. Oder, bis das System feststellt, dass es nicht passt und einen Fehler zurückgibt.

Als Best Practice empfiehlt es sich, `&jpegSize=` festzulegen und den `&qlt=` hinzuzufügen, wenn Sie JPG-Images an Geräte mit begrenztem Speicher bereitstellen.

## Zusammenfassung der empfohlenen Verfahren {#best-practices-summary}

Um eine hohe Bildqualität und eine geringe Dateigröße zu erzielen, empfiehlt es sich, mit der folgenden Kombination von Parametern zu beginnen:

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Diese Kombination von Einstellungen liefert unter den meisten Umständen hervorragende Ergebnisse.

Wenn eine weitere Optimierung für das Bild erforderlich ist, passen die Parameter für das Scharfzeichnen (Unschärfemaske) schrittweise an, indem Sie den Radiuswert auf 0,2 oder 0,3 einstellen. Anschließend können Sie den Betrag schrittweise von 1,75 bis maximal 4 erhöhen (entspricht einer Einstellung von 400 % in Photoshop). Prüfen Sie, ob das gewünschte Ergebnis erzielt wurde.

Wenn die gewünschten Ergebnisse für das Scharfzeichnen noch nicht erreicht wurden, erhöhen Sie den Radius in Dezimalschritten. Beginnen Sie für jeden Dezimalschnitt wieder mit einem Betrag von 1,75 und erhöhen Sie den Wert schrittweise bis maximal 4. Wiederholen Sie diesen Vorgang, bis das gewünschte Ergebnis erreicht ist. Obwohl die oben aufgeführten Werte einen von Kreativstudios erprobten Ansatz bieten, können Sie auch mit anderen Werten beginnen und andere Strategien verfolgen. Die Zufriedenheit mit den erzielten Ergebnisse ist immer subjektiv, aus diesem Grund ist strukturiertes Experimentieren der Schlüssel zum Erfolg.

Beim Experimentieren sind die folgenden allgemeinen Vorschläge hilfreich, um Ihren Workflow zu optimieren:

* Testen Sie verschiedene Parameter in Echtzeit, entweder direkt über eine URL oder mithilfe der Bildanpassungsfunktion von Adobe Dynamic Media Classic. Letztere bietet Echtzeitvorschauen für Anpassungsvorgänge.
* Als Best Practice empfiehlt es sich, Dynamic Media-Bildbereitstellungsbefehle in einer Bildvorgabe zu gruppieren. Bei einer Bildvorgabe handelt es sich im Grunde um URL-Befehlsmakros mit benutzerdefinierten Vorgabennamen wie `$thumb_low$` und `&product_high$`. Der benutzerdefinierte Vorgabenname in einem URL-Pfad ruft diese Vorgaben auf. Diese Funktionen helfen Ihnen dabei, die Befehls- und Qualitätseinstellungen für verschiedene Verwendungsmuster der Bildern auf Ihrer Website zu verwalten und verkürzen die Gesamtlänge der URLs.
* Adobe Dynamic Media Classic bietet außerdem erweiterte Möglichkeiten zur Optimierung der Bildqualität, wie das Scharfzeichnen von Bildern bei der Aufnahme. Für erweiterte Anwendungsfälle, bei denen eine weitere Optimierung der gerenderten Ergebnisse eine Option ist, kann Adobe Professional Services Ihnen mit benutzerdefinierten Einblicken und Best Practices helfen.
