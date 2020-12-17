---
title: Scharfzeichnen eines Bildes
seo-title: Scharfzeichnen eines Bildes
description: 'null'
seo-description: Erfahren Sie, wie Sie ein Bild scharfzeichnen.
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '2159'
ht-degree: 73%

---


# Scharfzeichnen eines Bildes {#sharpening-an-image}

Mit der Bildbearbeitungstechnik des Scharfzeichnens werden die Umrisse eines digitalen Bilds deutlicher dargestellt. Beim Scharfzeichnen wird der Kontrast zwischen den Randpixeln erhöht und der Übergang zwischen dunklen und hellen Bereichen dadurch hervorgehoben. Durch Scharfzeichnen wird der lokale Kontrast erhöht und die feinen Details kommen deutlicher zur Geltung. Es gibt keine feste Formel für das korrekte Scharfzeichnen aller Bilder. Bei zu geringem Scharfzeichnen können die Konturen des Bilds verschwommen wirken, während zu starkes Scharfzeichnen helle Ränder an den Kanten (Halos), Störungen und Bildrauschen verursachen kann.

Dynamic Media Classic empfiehlt die Verwendung von Bildvorgaben für alle Bilder. Hierdurch wird eine einheitliche Größe gewährleistet und die Schärfung wird in jedem Bild erzwungen, das mit einer Bildvorgabe aufgerufen wird. Darüber hinaus können Sie die Schärfungsparameter einer Bildvorgabe ganz einfach bearbeiten und ändern. Wenn Sie das nächste Mal eine Veröffentlichung vornehmen, erhalten alle Bilder, die mit dieser Vorgabe aufgerufen werden, die neuen Werte.

Dynamic Media Classic empfiehlt außerdem, den Viewer-Vorgaben Scharfzeichnung hinzuzufügen und dann einen Viewer mit dieser Vorgabe aufzurufen. Hierdurch wird sichergestellt, dass Bilder in den Viewern klar und ansprechend sind.

Unabhängig davon, ob Sie Bildvorgaben und Viewer-Vorgaben oder eine andere Methode des Scharfzeichnens verwenden, sollten Sie Ihre Bilder scharfzeichnen. Wenn Sie das nicht tun, sehen Ihre Bilder (und Websites) u. U. verschwommen aus.

>[!NOTE]
>
>Mit dem Befehl „Scharfzeichnen“ werden die Einstellungen unter „Bildvorgaben“, einschließlich der dort angegebenen Scharfzeichnungseinstellungen, überschrieben. Eine Bildvorgabe regelt die Größe und Formatierung, mit der Bilder von Dynamic Media-Image-Servern bereitgestellt werden. Dynamic Media Classic empfiehlt die Verwendung von Bildvorgaben, um alle Bilder bereitzustellen, um sicherzustellen, dass sie einheitlich und scharfgezeichnet dargestellt werden. Wenn jedoch die Scharfzeichnungseinstellungen für ein einzelnes Bild geändert wurden, gelten die Scharfzeichnungseinstellungen der Bildvorgabe nicht mehr für dieses Bild. Es wird dann ohne Anwendung der Scharfzeichnungseinstellungen der Bildvorgabe gesendet.

Es ist oft notwendig, Bilder scharfzuzeichnen. Dynamic Media Classic- und Image-Server-Angebot bieten mehrere Scharfzeichnungsoptionen. Es ist wichtig zu wissen, was das Scharfzeichnen bei einem Bild bewirkt und wie viel Scharfzeichnung Sie benötigen. Die meisten Bilder müssen etwas scharfgezeichnet werden, aber der Grad der Scharfzeichnung hängt vom Bild ab.

Die Bildschärfung erhöht den Kontrast der Pixel, um den Eindruck zu erwecken, dass die Kanten akzentuiert sind. Menschen nehmen diesen erhöhten Kantenkontrast als Schärfe wahr. Obwohl es einfach ist, ein Bild mithilfe von Scharfzeichnungsfiltern zu verbessern, ist es auch einfach, ein Bild zu stark scharfzuzeichnen.

Wenn ein Bild zu stark scharfgezeichnet ist, entsteht ein Halo- oder Banding-Effekt.

Es gibt Best Practices, die Sie zur Optimierung der Scharfzeichnung Ihrer Bilder in Dynamic Media Classic und auf Dynamic Media Image Server befolgen können.

Siehe [Bewährte Verfahren zum Scharfzeichnen von Bildern in Dynamic Media Classic und auf Dynamic Media Image Server](/help/assets/s7_sharpening_images.pdf).

**So zeichnen Sie ein Bild scharf**

Um ein Bild scharfzuzeichnen, klicken Sie auf seine Rollover-Schaltfläche **Bearbeiten** und wählen Sie &quot;Scharfzeichnen&quot;oder öffnen Sie es im Durchsuchenbedienfeld in der Ansicht &quot;Details&quot;und klicken Sie dann auf **Scharfzeichnen**. Der Anzeigebereich „Schärfe-Editor“ mit den Scharfzeichnungsbefehlen wird geöffnet. Wählen Sie Befehle und klicken Sie auf **Speichern**.

>[!NOTE]
>
>Bevor Sie ein Bild scharfzeichnen, können Sie im Menü „Vorgabe anwenden“ eine Bildvorgabe auswählen, um deren Effekte für die Scharfzeichnung des Bilds zu sehen. Die Scharfzeichnungseffekte der Bildvorgabe können für das Bild bereits ausreichend sein. Das Menü „Vorgabe anwenden“ befindet sich am unteren Rand des Anzeigebereichs „Schärfe-Editor“.

**Scharfzeichnungsoptionen**

Die folgende Tabelle zeigt die Scharfzeichnungsoptionen des Image-Servers.

| Name | URL-Protokoll | Werte | Beispiel |
|--- |--- |--- |--- |
| Einfaches Scharfzeichnen | op_sharpen | `0 | 1` | op_sharpen=1 |
| Resamplingmodus | resMode | `bilin | bicub | sharp2 | trilin`<br><br>bilin: Wählt bilineare Standardinterpolation aus. Schnellste Neuberechnungsmethode; einige Aliasing-Artefakte sind möglicherweise bemerkbar.<br>bicub: Wählt bikubische Interpolation aus. CPU-intensiver als bilin, erzielt aber schärfere Bilder mit weniger bemerkbaren Aliasing-Artefakten.<br><br>sharp2: Wählt eine modifizierte Lanczos-Fensterfunktion als Interpolationsalgorithmus aus. Kann etwas schärfere Ergebnisse als „bikubisch“ erzeugen, lastet aber die CPU stärker aus.<br><br>trilin: Wählt eine modifizierte trilineare Interpolation aus, die sowohl eine höhere als auch eine niedrigere Auflösung verwendet, falls verfügbar. Wird nur bei Problemen mit dem Aliasing empfohlen. Reduziert JPEG-Größen aufgrund der reduzierten Hochfrequenzdaten. | resMode=sharp2 |
| Unschärfemaske | op_usm | Betrag, Radius, Schwellenwert, monochrom<br><br>Betrag: Filterfestigkeitsfaktor (real 0...5)<br><br>Radius: Filterkernradius in Pixel (real 0...250) <br><br>Schwellenwert: Filterschwellenwert (int 0...255)<br><br>Monochrom: auf 0 gesetzt, um jede Farbkomponente separat unscharf zu maskieren, auf 1 eingestellt, um Bildhelligkeit (Intensität) unscharf zu maskieren | op_usm=1,1,10,0 |

Wählen Sie im Menü „Scharfzeichnen“ eine der folgenden Optionen:

**** KeineDeaktiviert das Scharfzeichnen.

**** ScharfzeichnenFührt einen einfachen Scharfzeichnungsdurchlauf für die Datei aus, nachdem die Größe geändert wurde. Dies ist ähnlich wie der Scharfzeichnungsfilter in Photoshop und unterstützt alle Benutzerparameter. Normalerweise würden Sie diesen Filter oder „Unscharf maskieren“ verwenden, aber nicht beide. Diese Methode wird nicht als Best Practice empfohlen, sie kann aber verschwommene Bilder kompensieren. (URL: op_sharpen)

**Unscharf** maskierenErmöglicht die Feinabstimmung eines Scharfzeichnungsfiltereffekts für das endgültige neu berechnete Bild. Sie können die Intensität des Effekts, den Radius des Effekts (gemessen in Pixel) und einen Schwellenwert für den Kontrast steuern, der ignoriert wird. Dieser Effekt verwendet dieselben Optionen wie der Photoshop-Filter „Unscharf maskieren“. (URL: op_usm)

Wählen Sie diese Optionen, um die Scharfzeichnung mit „Unscharf maskieren“ anzupassen:

**** AmountSteuert den Kontrast, der auf Kantenpixel angewendet wird. Der Standardwert ist 0,0. Für Bilder mit höherer Auflösung können Sie ihn auf bis zu 5,0 erhöhen. Sie können sich die Auswirkung der Option „Betrag“ wie ein Maß für die Filterintensität vorstellen. Beachten Sie, dass die Einstellung &quot;Betrag&quot;in Dynamic Media Classic nicht mit der Einstellung &quot;Betrag&quot;in Photoshop übereinstimmt. Photoshop verwendet einen Betrag zwischen 1 % und 500 %, während Dynamic Media Classic zwischen 0,0 und 5,0 skaliert. (5,0 entspricht ungefähr 500 % in Photoshop, 0,9 ungefähr 90 % usw.)

**** RadiusBestimmt die Anzahl der Pixel um die Kantenpixel, die sich auf das Scharfzeichnen auswirken. Der Effekt wird auf allen Pixeln im Bild ausgeführt und strahlt in alle Richtungen aus. 

Der beste Radiuswert hängt von der Größe des Bilds ab. Bei einem geringeren Wert werden nur die Kantenpixel scharfgezeichnet, während bei einem hohen Wert ein breiterer Pixelbereich scharfgezeichnet wird.

Um beispielsweise einen ähnlichen Scharfzeichnungseffekt für ein 2000 x 2000 Pixel und ein 500 x 2000-Pixelbild zu erhalten, könnten Sie einen Radiuswert von zwei Pixeln auf dem 2000 x 2000 Pixel und einen Radiuswert von einem Pixel auf dem 500 x 500-Pixelbild (bzw. einen größeren Wert für ein Bild mit mehr Pixeln) festlegen. 

**** SchwellenwertBestimmt den Kontrastbereich, der ignoriert werden soll, wenn der Filter &quot;Unschärfemaske&quot;angewendet wird. Diese Option legt also fest, wie stark sich die scharfgezeichneten Pixel von dem sie umgebenden Bereich unterscheiden müssen, damit sie als Kantenpixel erkannt und scharfgezeichnet werden.

Der Schwellenwert verwendet einen Wert von 0-255, was für die Anzahl der Helligkeitsschritte in einem Graustufenbild steht. 0=schwarz, 128=50 % grau und 255=weiß. Beispiel: Ein Schwellenwert von 12 ignoriert leichte Variationen der Hauttonhelligkeit, um kein Rauschen hinzuzufügen, fügt aber trotzdem Kantenkontrast zu kontrastreichen Bereichen (z. B. wo Wimpern auf die Haut treffen) hinzu. 

Wenn Sie beispielsweise ein Foto mit einem Gesicht einer Person haben, wirkt sich „Unscharf maskieren“ auf die Teile des Bildes mit dem höchsten Kontrast und der glattesten Haut aus. Selbst die glatteste Haut weist subtile Änderungen in Helligkeitswerten auf. Wenn Sie keinen Schwellenwert verwenden, akzentuiert der Filter diese subtilen Änderungen in den Hautpixeln und erzeugt einen Rauscheffekt (der wahrscheinlich unerwünscht ist), während er gleichzeitig den Kontrast an den Wimpern erhöht und somit die Schärfe verbessert (wahrscheinlich wünschenswert). Um dieses Problem zu vermeiden, verwenden Sie einen Schwellenwert, bei dem der Filter Pixel ignoriert, die den Kontrast nicht drastisch ändern, wie z. B. glatte Haut. Um beispielsweise Rauschen oder eine Nachbearbeitung in Bildern mit Fruchttönen zu vermeiden, sollten Sie mit Schwellenwerten zwischen 2 und 20 experimentieren. Beim Standardwert &quot;Schwellenwert&quot;von 0 werden alle Pixel im Bild scharfgezeichnet.

**&quot;** ToSelect Jede Farbe&quot;anwenden, um die Scharfzeichnung separat auf jede Farbkomponente anzuwenden; Wählen Sie &quot;Helligkeit&quot;, um das Scharfzeichnen auf die Helligkeitsbereiche des Bildes anzuwenden.

**Resampling**

Wählen Sie im Menü „Resampling“ eine Option. Mit diesen Optionen wird ein Bild beim Downsampling scharfgezeichnet:

**&quot;** Keine&quot;deaktiviert die Neuberechnung.

**** BilinearDie schnellste Neuberechnungsmethode; einige Aliasing-Artefakte sind bemerkbar.

**Bikubisch** Erhöht die CPU-Auslastung auf dem Image-Server, erzielt aber schärfere Bilder mit weniger bemerkbaren Aliasing-Artefakten.

**Scharfzeichnen2**  kann leicht schärfere Ergebnisse als die Option &quot;Bikubisch&quot;erzielen, allerdings zu noch höheren CPU-Kosten auf dem Image-Server.

**** TrilinearVerwendet sowohl eine höhere als auch eine niedrigere Auflösung, sofern verfügbar; wird nur empfohlen, wenn das Aliasing ein Problem darstellt. Bei dieser Methode wird die JPEG-Dateigröße durch Reduzierung der Hochfrequenzdaten verringert.

**Scharfzeichnen und Bildvorgaben**

Sie können alle drei Scharfzeichnungseffekte mischen, um Ihr Endergebnis zu erzielen. Dies wird allerdings nicht empfohlen. Dynamic Media Classic empfiehlt, die Scharfzeichnungseffekte als Teil einer Bildvorgabe zu speichern. Mit Bildvorgaben können Sie die am häufigsten verwendeten Bildmodifikatoren verpacken, um ein dynamisch angepasstes Bild in einer kleinen Textzeichenfolge zu erstellen. Eine Bildvorgabe enthält Werte für das Dateiformat (normalerweise JPEG für das Web), Pixelanzahl und Bildschärfen. Anstatt die URL bei jedem Bildmodifizierer anzuhängen, der benötigt wird, um einen bestimmten Bildgrößentyp zu erstellen, erstellen Sie eine benannte Bildvorgabe wie z. B. „Miniaturansicht“, konfigurieren die Miniaturbildvorgabe mit der gewünschten Größe, dem Dateiformat und den gewünschten Scharfzeichnungsoptionen und rufen dann das Bild mit dem Bildvorgabenamen auf. Bildvorgaben verkürzen die Länge der Gesamt-URL. Diese beiden URLs erzeugen das gleiche 350 x 350-JPEG-Bild mit Scharfzeichnung. 

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Bildvorgaben können jederzeit geändert und aktualisiert werden. Sie sehen die Ergebnisse einer Änderung an einer Bildvorgabe nach der Veröffentlichung und nachdem der Cache für die URL gelöscht worden ist.

Wenn Sie eine Vorgabe für jedes Bild in einer Größenkategorie verwenden, kann ein Unternehmensadministrator die Definition der jeweiligen Bildvorgabe aktualisieren, sie erneut veröffentlichen und damit jedes Bild mithilfe dieses Formats ändern, ohne Webcode zu ändern. Es empfiehlt sich, eine Bildvorgabe pro Größe auf Ihrer Site zu verwenden. Um eine Bildvorgabe hinzuzufügen, gehen Sie zu „Einstellungen“ > „Anwendungseinstellungen“ > „Bildvorgaben“. Fügen Sie dann eine Vorgabe hinzu oder bearbeiten Sie eine vorhandene Vorgabe. Das einzige erforderliche Feld ist der Name der Vorgabe. Sie sollten jedoch einen gewissen Grad der Scharfzeichnung in jede Vorgabe aufnehmen.

**JPG-Qualität**

Die Optionen für „JPG-Qualität“ bestimmen den JPG-Komprimierungsgrad:

**JPG-** QualitätWählen Sie diese Option, wenn Sie Komprimierungsstufen und Chrominanz-Downsampling steuern möchten.

**** SliderBestimmt die JPG-Komprimierungsstufe. Diese Einstellung wirkt sich sowohl auf die Dateigröße als auch die Bildqualität aus. Die JPG-Qualitätsskala ist 1-100.

**JPG-Chrominanz-** Neuberechnung aktivieren Da das Auge für hochfrequente Farbinformationen weniger empfindlich ist als für hochfrequente Leuchtdichte, unterteilen JPEG-Bilder Bildinformationen in Leuchtdichte- und Farbkomponenten. Bei der Komprimierung eines JPEG-Bildes behält die Leuchtdichtekomponente die volle Auflösung, während für die Farbkomponenten ein Downsampling, d. h. eine Mittelwerterstellung für Pixelgruppen, ausgeführt wird. Obwohl das Datenvolumen beim Downsampling um die Hälfte oder ein Drittel reduziert wird, ist die auftretende Qualitätsminderung kaum wahrnehmbar. Downsampling kann nicht auf Graustufenbilder angewendet werden. Mit dieser Technik wird der Komprimierungsgrad, der für Bilder mit hohem Kontrast (z. B. Bilder mit überlappendem Text) sinnvoll ist, reduziert.

**Festlegen von unternehmensweiten Scharfzeichnungsoptionen**

Wenn Sie keine Bildvorgabe verwenden oder spezifische Image-Server-Scharfzeichnungsprotokolle mit dem URL-String übergeben, wird das Bild beim Downsampling nicht scharfgezeichnet. Sie können jedoch in diesem Fall die Standard-Scharfzeichnungswerte festlegen, wodurch jedes Bild immer etwas scharfgezeichnet wird.

Um Standard-Scharfzeichnungsoptionen für Ihr Unternehmen festzulegen, gehen Sie zu „Einstellungen“ > „Anwendungseinstellungen“ > „Veröffentlichungseinstellungen“ > „Image-Server“. Wenn Sie den Standard-Resampling-Modus auf „Scharf2“ einstellen, wird das Bild beim Downsampling immer scharfgezeichnet.

**Hinzufügen von Scharfzeichnung zu Viewer-Vorgaben**

Wenn Sie der Vorgabe keine Scharfzeichnungs-Bildmodifizierer hinzufügen, kann das kleine, anfänglich geladene Bild verschwommen aussehen, weil ein Downsampling durchgeführt wurde, um es in das Viewer-Fenster einzupassen, ohne scharfgezeichnet zu werden.

In Dynamic Media Classic können Sie mit Viewer-Vorgaben (z. B. Bildvorgaben) viele Optionen an einem Ort zentralisieren, z. B. die Auswahl der Skin- und Viewer-Optionen (z. B. die Eingabe einer Drucken-Schaltfläche oder die Steuerung der Zoomanimation). Viewer-Vorgaben befinden sich im selben Bereich wie Bildvorgaben, und zwar unter „Einstellungen“ > „Anwendungseinstellungen“ > „Viewer-Vorgaben“.

Die Modifiziereroption befindet sich im Bereich „Core-Einstellungen“ aller E-Katalog-, Rotations- und benutzerdefinierter Zoom-Viewer-Vorgaben. Wenn Sie die URL-Scharfzeichnungsbefehle zum Feld „Modifizierer“ hinzufügen, fügen Sie bei jedem Aufruf des Viewers mit der jeweiligen Viewer-Vorgabe Scharfzeichnung hinzu.

Um die Viewer-Vorgabe aufzurufen, verwenden Sie den Befehl „config=“ in der Viewer-URL. Hier ist ein Beispiel für das Aufrufen eines Bildsatzes (Schuhe) mit einer Viewer-Vorgabe (FantasticoZoom2009):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2009`

Diese Vorgabe schärft und ändert die Standardskin des Viewers.

**Erstellen bildspezifischer Abweichungen**

Die letzte und am wenigsten empfohlene Scharfzeichnungsmethode besteht darin, Scharfzeichnungsabweichungen auf Bildbasis zu erstellen. Hierdurch wird die Scharfzeichnung in einer Bildvorgabe mit ihren eigenen spezifischen Werten überschrieben. Allerdings werden hierbei alle anderen Scharfzeichnungsmethoden bei einer beliebigen Größe überschrieben. Der beste Anwendungsfall für diese Methode ist, wenn einige Ihrer Bilder nicht hochauflösend sind und die Werte in den Bildvorgaben für diese kleinen Bilder zu hoch sind. In diesem Fall könnte ein bildabhängiges Scharfzeichnen notwendig sein.

Wählen Sie in Dynamic Media Classic ein beliebiges Bild aus, gehen Sie zur Ansicht &quot;Detail&quot;(durch Klicken auf die Dublette oder Drücken der Schaltfläche &quot;Detail-Ansicht&quot;) und klicken Sie auf &quot;Scharfzeichnen&quot;. Ändern Sie die gewünschten Parameter und klicken Sie dann auf „Speichern“. Hierdurch wird dem Image-Server mitgeteilt, diese Scharfzeichnungsparameter anstatt eines Befehls zu verwenden, den Sie in der URL aufrufen, wie z. B. einen Scharfzeichnungsmodifizierer oder eine Bildvorgabe. Sie müssen veröffentlichen, damit die Änderungen wirksam werden.
