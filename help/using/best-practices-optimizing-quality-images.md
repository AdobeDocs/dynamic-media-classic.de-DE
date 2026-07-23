---
title: Best Practices für die Optimierung der Bildqualität
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
autotag-review: '2026-05-13T17:39:42.316Z'
TQID: 'https://experienceleague.adobe.com/kw-spdqv6ArVEWk8ID4mnQjYrS25RZntKOJ7-tESasY'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: bcc5edb5-84c3-4940-9f84-ed88b6c16274
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: b29d7cc6962ca9e7724bb43987947b08af5cd4d7
workflow-type: tm+mt
source-wordcount: 1591
ht-degree: 27%

---

# Empfohlene Verfahren zur Optimierung der Bildqualität{#best-practices-for-optimizing-the-quality-of-your-images}

Die Optimierung der Bildqualität kann zeitaufwendig sein. Viele Faktoren tragen dazu bei, akzeptable Ergebnisse zu erzielen. Das Ergebnis ist teilweise subjektiv, da jede Person die Bildqualität unterschiedlich wahrnimmt. Strukturierte Experimente sind unerlässlich.

Adobe Dynamic Media Classic umfasst mehr als 100 Bildbereitstellungsbefehle zum Optimieren und Optimieren von Bildern und zum Rendern von Ergebnissen. Die folgenden Richtlinien sollen Ihnen dabei helfen, den Vorgang zu optimieren und die gewünschten Ergebnisse schnell mit nur einigen wichtigen Befehle und empfohlenen Verfahren zu erzielen.

Siehe auch [Smart Imaging](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/imaging-faq).

>[!TIP]
>
>Probieren Sie die Vorteile von Dynamic Media-Bildmodifikatoren und der intelligenten Bildbearbeitung mithilfe von Dynamic Media ([_)_](https://snapshot.scene7.com/).
>
> „Momentaufnahme“ ist ein visuelles Demonstrations-Tool, das die Funktionen von Dynamic Media für eine optimierte und dynamische Bildbereitstellung veranschaulicht. Experimentieren Sie mit Testbildern oder Dynamic Media-URLs, damit Sie die Ausgabe verschiedener Dynamic Media-Bildmodifikatoren visuell beobachten können, und optimieren Sie die intelligente Bildbearbeitung auf Folgendes:
>
>* Dateigröße (mit WebP- und AVIF-Bereitstellung)
>* Netzwerkbandbreite
>* DPR (Device Pixel Ratio)
>
>Informationen zur Verwendung von Momentaufnahme finden Sie im [Schulungsvideo zu Momentaufnahmen](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot) (3 Minuten und 17 Sekunden).


## Empfohlene Verfahren für das Bildformat (&amp;fmt=) {#best-practices-for-image-format-fmt}

* Das JPG- oder das PNG-Format ist die beste Wahl, um Bilder in akzeptabler Qualität und handlicher Größe und Dateigröße bereitzustellen.
* Wenn in der URL kein Formatbefehl angegeben ist, wird für die Bereitstellung standardmäßig JPG verwendet.
* JPG-Dateien werden in einem Verhältnis von 10:1 komprimiert und produzieren so in der Regel kleinere Bilddateigrößen. PNG-Dateien werden mit einem Verhältnis von etwa 2:1 komprimiert, es sei denn, Bilder enthalten transparente Hintergründe. Normalerweise sind PNG-Dateien größer als JPG-Dateien.
* JPG verwendet eine verlustbehaftete Komprimierung. Dies bedeutet, dass Bildelemente (Pixel) bei der Komprimierung verworfen werden. Im Gegensatz dazu verwendet PNG eine verlustfreie Komprimierung.
* JPG komprimiert Fotografien häufig mit einer höheren Genauigkeit als künstliche Bilder mit scharfen Kanten und hohem Kontrast.
* Wenn die Bilder transparente Anteile enthalten, sollte das PNG-Format verwendet werden, da JPG keine Transparenz unterstützt.

Beginnen Sie als Best Practice für das Bildformat mit den häufigsten `&fmt=JPG`.

## Empfohlene Verfahren für die Bildgröße {#best-practices-for-image-size}

Die dynamische Reduzierung der Bildgröße ist eine der häufigsten Aufgaben, die von Dynamic Media Image Serving ausgeführt werden. Sie umfasst die Angabe der Größe und, optional, welcher Modus zur Verringerung der Abtastrate (Downsampling) zum Herunterskalieren verwendet werden soll.

* Verwenden Sie für die Bildgröße `&wid=<value>` und `&hei=<value>`. Diese Parameter legen die Bildbreite automatisch entsprechend dem Seitenverhältnis fest.
* `&resMode=<value>` Steuert den Algorithmus für die Neuberechnung. Beginnen Sie mit `&resMode=sharp2`. Dieser Wert bietet die beste Bildqualität. Die Verwendung des `bilin` für die Neuberechnung ist zwar schneller, führt aber häufig zu Alias-Artefakten.

Verwenden Sie `&wid=<value>&hei=<value>&resMode=sharp2` als Best Practice für die Bildgröße. `&hei=<value>&resMode=sharp2`

## Empfohlene Verfahren für das Scharfzeichnen von Bildern {#best-practices-for-image-sharpening}

Das Scharfzeichnen von Bildern ist der komplexeste Aspekt bei der Steuerung von Bildern auf Ihrer Website und bei dem viele Fehler auftreten. Weitere Informationen zur Funktionsweise von Scharfzeichnung und Unschärfemaske in Adobe Dynamic Media Classic finden Sie in den folgenden hilfreichen Ressourcen:

Whitepaper mit Best Practices für PDF [Scharfzeichnen von Bildern in Adobe Dynamic Media Classic und auf Image Server](/help/using/assets/s7_sharpening_images.pdf).

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

In Adobe Dynamic Media Classic können Sie Bilder während der Aufnahme, Bereitstellung oder beides scharfzeichnen. Normalerweise können Sie Bilder jedoch mit einer Methode scharfzeichnen, jedoch nicht mit beiden. Das Scharfzeichnen von Bildern bei der Bereitstellung über eine URL liefert in der Regel die besten Ergebnisse.

Es gibt zwei Methoden zum Scharfzeichnen von Bildern:

* Einfaches Scharfzeichnen (`&op_sharpen`): Ähnlich wie der in Adobe Photoshop verwendete Scharfzeichnungsfilter wird beim einfachen Scharfzeichnen nach der dynamischen Größenanpassung das endgültige Bild einfach scharfgezeichnet. Diese Methode kann jedoch nicht vom Benutzer konfiguriert werden. Es empfiehlt sich, die Verwendung von `&op_sharpen` zu vermeiden, sofern dies nicht erforderlich ist.
* Unschärfemaske ( `&op_USM`): Unschärfemaske ist ein Branchenstandard-Filter für das Scharfzeichnen. Wir empfehlen, beim Scharfzeichnen von Bilder mit der Unschärfemaske die folgenden Richtlinien zu beachten. Mit der Unschärfemaske können Sie die folgenden drei Parameter steuern:

  * `&op_sharpen=amount,radius,threshold`

    * `amount` (0-5, Stärke des Effekts.)
    * `radius` (0-250, Breite der „Scharfzeichnungslinien“, die um das scharfgezeichnete Objekt gezeichnet werden, gemessen in Pixel.)

      Beachten Sie, dass die Parameter `radius` und `amount` eine umgekehrte Beziehung aufweisen. Eine Verringerung der `radius` kann durch eine Erhöhung der `amount` ausgeglichen werden. `Radius` ermöglicht eine feinere Steuerung, da ein niedrigerer Wert nur die Kanten-Pixel schärft, während ein höherer Wert einen größeren Bereich von Pixeln schärft.

    * `threshold` (0-255, Empfindlichkeit der Wirkung.)

      Dieser Parameter legt fest, wie stark sich die scharfgezeichneten Pixel von dem sie umgebenden Bereich unterscheiden müssen, damit sie als Kantenpixel erkannt und vom Filter scharfgezeichnet werden. Der Schwellenwert hilft dabei, das übermäßige Scharfzeichnen von Bereichen mit ähnlichen Farben zu vermeiden, z. B. bei Hauttönen. Bei einem Schwellenwert von 12 werden beispielsweise leichte Variationen der Hauttonhelligkeit ignoriert, um kein „Rauschen“ zu erzeugen, trotzdem wird kontrastreichen Bereichen, z. B. wo Wimpern auf die Haut treffen, Kantenkontrast hinzugefügt.

      Weitere Informationen zum Festlegen dieser drei Parameter, einschließlich Best Practices für den Filter, finden Sie unter [Scharfzeichnen von Bildern in Adobe Dynamic Media Classic und auf dem Bildserver](/help/using/assets/s7_sharpening_images.pdf).

    * Mit Adobe Dynamic Media Classic können Sie auch einen vierten Parameter steuern: monochrome ( `0,1`). Dieser Parameter bestimmt, ob die Unschärfemaske auf jede Farbkomponente separat (mit dem Wert `0`) oder auf die Bildhelligkeit/-intensität (mit dem Wert `1`) angewendet wird.

Wir empfehlen, mit dem Parameter „Radius“ der Unschärfemaske zu beginnen. Sie können beispielsweise mit den folgenden Radius-Einstellungen beginnen:

* Website: 0,2 bis 0,3 Pixel
* Fotografischer Druck (250 bis 300 ppi): 0,3 bis 0,5 Pixel
* Offsetdruck (266 bis 300 ppi): 0,7 bis 1,0 Pixel
* Leinwanddruck (150 ppi): 1,5 bis 2,0 Pixel

Erhöhen Sie diesen Wert stufenweise von 1,75 bis 4. Wenn das Scharfzeichnen immer noch nicht das gewünschte Ergebnis ist, erhöhen Sie den Radius um eine Dezimalinkrementierung und stellen Sie den Betrag erneut von 1,75 auf 4 ein. Wiederholen Sie diesen Vorgang bei Bedarf.

Lassen Sie die Parametereinstellung „Monochrom“ auf 0.

## Best Practices für die JPEG-Komprimierung (`&qlt=`) {#best-practices-for-jpeg-compression-qlt}

* Dieser Parameter steuert die Qualität der JPG-Kodierung. Ein höherer Wert bedeutet eine höhere Bildqualität, jedoch auch eine größere Datei; entsprechend bedeutet ein niedrigerer Wert eine geringere Bildqualität, aber eine kleinere Dateigröße. Der Bereich für diesen Parameter ist 0 bis 100.
* Setzen Sie den Wert zur Optimierung der Qualität nicht auf 100. Der Unterschied zwischen 90 bzw. 95 und 100 ist kaum wahrnehmbar. 100 erhöht jedoch unnötigerweise die Größe der Bilddatei. Um die Qualität zu optimieren, aber zu große Bilddateien zu vermeiden, setzen Sie daher den `qlt=` auf 90 oder 95.
* Um eine kleine Bilddateigröße zu optimieren, aber die Bildqualität auf einem akzeptablen Niveau zu halten, setzen Sie den `qlt=` auf 80. Werte unter 70 bis 75 führen zu einer signifikanten Verschlechterung der Bildqualität.
* Um in der Mitte zu bleiben, empfiehlt es sich, den `qlt=` auf 85 festzulegen.
* Verwenden der Chroma-Flag-`qlt=`

  * Der Parameter &quot;`qlt=`&quot; verfügt über eine zweite Einstellung, mit der Sie die Neuberechnung der RGB-Chromatizität mit der `,0` „Normalwert“ (Standard) aktivieren oder mit der `,1` Wert deaktivieren können.
  * Beginnen Sie mit der Deaktivierung der RGB-Chromatizitäts-Downsampling ( `,1`). Diese Einstellung führt in der Regel zu einer besseren Bildqualität, insbesondere bei künstlichen Bilder mit vielen scharfen Kanten und hohem Kontrast.

Als Best Practice für die Komprimierung von JPG `&qlt=85,0`.

## Empfohlene Verfahren für die JPEG-Größenanpassung (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

Der Parameter `jpegSize` ist nützlich, wenn Sie garantieren möchten, dass ein Bild eine bestimmte Größe nicht überschreitet. Dieser Parameter ist für die Bereitstellung an Geräten mit begrenztem Speicher vorgesehen.

* Dieser Parameter wird in Kilobyte ( `jpegSize=<size_in_kilobytes>`) festgelegt. Er legt die maximal zulässige Größe für Bildbereitstellung fest.
* `&jpegSize=` Interagiert mit dem JPG-Komprimierungsparameter `&qlt=`. Wenn die JPG-Antwort mit dem angegebenen JPG-Komprimierungsparameter (`&qlt=`) den `jpegSize` Wert nicht überschreitet, wird das Bild mit dem definierten `&qlt=` zurückgegeben. Andernfalls wird die `&qlt=` schrittweise verringert, bis das Bild in die maximal zulässige Größe passt. Alternativ gibt das System einen Fehler zurück, wenn es nicht in das Bild passt.

Als Best Practice empfiehlt es sich, bei der Bereitstellung von JPG-Bildern an Geräten mit begrenztem Speicher den `&qlt=` zu `&jpegSize=` und einzuschließen.

## Zusammenfassung der empfohlenen Verfahren {#best-practices-summary}

Um eine hohe Bildqualität und eine geringe Dateigröße zu erzielen, empfiehlt es sich, mit der folgenden Kombination von Parametern zu beginnen:

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

Diese Kombination von Einstellungen liefert unter den meisten Umständen hervorragende Ergebnisse.

Wenn das Bild weiter optimiert werden muss, können Sie die Schärfungsparameter (Unschärfemaske) schrittweise optimieren, indem Sie mit einem Radius von 0,2 oder 0,3 beginnen. Erhöhen Sie dann schrittweise die Menge von 1,75 auf maximal 4 (entspricht 400 % in [!DNL Adobe Photoshop]). Prüfen Sie, ob das gewünschte Ergebnis erzielt wurde.

Wenn die gewünschten Ergebnisse für das Scharfzeichnen noch nicht erreicht wurden, erhöhen Sie den Radius in Dezimalschritten. Setzen Sie für jedes Dezimalinkrement den Betrag auf 1,75 zurück und erhöhen Sie ihn allmählich auf 4. Wiederholen Sie diesen Vorgang, bis das gewünschte Ergebnis erreicht ist. Obwohl die oben genannten Werte ein Ansatz sind, den Creative Studios validiert haben, beachten Sie, dass Sie andere Werte verwenden und andere Verfahren befolgen können. Ob die Ergebnisse für Sie zufriedenstellend sind oder nicht, ist eine subjektive Frage; daher ist ein strukturiertes Experimentieren erforderlich.

Beim Experimentieren sind die folgenden allgemeinen Vorschläge hilfreich, um Ihren Workflow zu optimieren:

* Testen Sie verschiedene Parameter in Echtzeit direkt auf einer URL oder mit [!DNL Adobe Dynamic Media Classic] Bildanpassungs-Tools. Letztere bietet Echtzeitvorschauen für Anpassungsvorgänge.
* Als Best Practice empfiehlt es sich, Dynamic Media-Bildbereitstellungsbefehle in einer Bildvorgabe zu gruppieren. Eine Bildvorgabe ist ein Satz von URL-Befehlsmakros mit benutzerdefinierten Vorgabennamen wie `$thumb_low$` und `$product_high$`. Der benutzerdefinierte Vorgabenname in einem URL-Pfad ruft diese Vorgaben auf. Diese Funktionen helfen Ihnen dabei, die Befehls- und Qualitätseinstellungen für verschiedene Verwendungsmuster der Bildern auf Ihrer Website zu verwalten und verkürzen die Gesamtlänge der URLs.
* Adobe Dynamic Media Classic bietet außerdem erweiterte Möglichkeiten zur Optimierung der Bildqualität, wie das Scharfzeichnen von Bildern bei der Aufnahme. Für erweiterte Anwendungsfälle, bei denen eine weitere Optimierung der gerenderten Ergebnisse eine Option ist, kann Adobe Professional Services Ihnen mit benutzerdefinierten insight- und Best Practices helfen.
