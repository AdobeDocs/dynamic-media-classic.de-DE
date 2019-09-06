---
title: Scharfzeichnen eines Bildes
seo-title: Scharfzeichnen eines Bildes
description: 'null'
seo-description: Hier erfahren Sie, wie Sie ein Bild scharfzeichnen.
uuid: d 86 af 74 a -89 c 5-4 f 2 b -96 ba-f 2 e 7 da 600 bca
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/master_ files
discoiquuid: 11 cd 5362-d 90 a -4 c 1 e-bfbd -46 a 65 a 554409
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Scharfzeichnen eines Bildes {#sharpening-an-image}

Mit der Bildbearbeitungstechnik des Scharfzeichnens werden die Umrisse eines digitalen Bilds deutlicher dargestellt. Beim Scharfzeichnen wird der Kontrast zwischen den Randpixeln erhöht und der Übergang zwischen dunklen und hellen Bereichen dadurch hervorgehoben. Durch Scharfzeichnen wird der lokale Kontrast erhöht und die feinen Details kommen deutlicher zur Geltung. Es gibt keine feste Formel für das korrekte Scharfzeichnen aller Bilder. Bei zu geringem Scharfzeichnen können die Konturen des Bilds verschwommen wirken, während zu starkes Scharfzeichnen helle Ränder an den Kanten (Halos), Störungen und Bildrauschen verursachen kann.

Dynamic Media Classic empfiehlt dringend, Bildvorgaben für alle Bilder zu verwenden. Hierdurch wird eine einheitliche Größe gewährleistet und die Schärfung wird in jedem Bild erzwungen, das mit einer Bildvorgabe aufgerufen wird. Darüber hinaus können Sie die Schärfungsparameter einer Bildvorgabe ganz einfach bearbeiten und ändern. Wenn Sie das nächste Mal eine Veröffentlichung vornehmen, erhalten alle Bilder, die mit dieser Vorgabe aufgerufen werden, die neuen Werte.

Dynamic Media Classic empfiehlt auch das Hinzufügen von Scharfzeichnung zu Viewer-Vorgaben und das Aufrufen eines Viewers mit dieser Vorgabe. Hierdurch wird sichergestellt, dass Bilder in den Viewern klar und ansprechend sind.

Unabhängig davon, ob Sie Bildvorgaben und Viewer-Vorgaben oder eine andere Methode des Scharfzeichnens verwenden, sollten Sie Ihre Bilder scharfzeichnen. Wenn Sie das nicht tun, sehen Ihre Bilder (und Websites) u. U. verschwommen aus.

>[!NOTE]
>
>Mit dem Befehl „Scharfzeichnen“ werden die Einstellungen unter „Bildvorgaben“, einschließlich der dort angegebenen Scharfzeichnungseinstellungen, überschrieben. Eine Bildvorgabe wirkt sich auf die Größe und Formatierung aus, mit der Bilder von dynamischen Medienservern bereitgestellt werden. Dynamic Media Classic empfiehlt dringend die Verwendung von Bildvorgaben, um alle Bilder bereitzustellen, um sicherzustellen, dass Bilder in einheitlicher Größe und Schärfe bereitgestellt werden. Wenn jedoch die Scharfzeichnungseinstellungen für ein einzelnes Bild geändert wurden, gelten die Scharfzeichnungseinstellungen der Bildvorgabe nicht mehr für dieses Bild. Es wird dann ohne Anwendung der Scharfzeichnungseinstellungen der Bildvorgabe gesendet.

Es ist oft notwendig, Bilder scharfzuzeichnen. Dynamic Media Classic SPS und Image Server bieten mehrere Scharfzeichnungsoptionen. Es ist wichtig zu wissen, was das Scharfzeichnen bei einem Bild bewirkt und wie viel Scharfzeichnung Sie benötigen. Die meisten Bilder müssen etwas scharfgezeichnet werden, aber der Grad der Scharfzeichnung hängt vom Bild ab.

Die Bildschärfung erhöht den Kontrast der Pixel, um den Eindruck zu erwecken, dass die Kanten akzentuiert sind. Menschen nehmen diesen erhöhten Kantenkontrast als Schärfe wahr. Obwohl es einfach ist, ein Bild mithilfe von Scharfzeichnungsfiltern zu verbessern, ist es auch einfach, ein Bild zu stark scharfzuzeichnen.

Wenn ein Bild zu stark scharfgezeichnet ist, entsteht ein Halo- oder Banding-Effekt.

Es gibt Best Practices, mit denen Sie das Scharfzeichnen Ihrer Bilder im Scene 7 Publishing System und auf dem Dynamic Media Image Server optimieren können.

Siehe [Bewährte Verfahren zum Scharfzeichnen von Bildern im Scene 7 Publishing System und auf dem dynamischen Medienserver](https://marketing.adobe.com/resources/help/en_US/s7/sharpening/s7_sharpening_images.pdf).

**So zeichnen Sie ein Bild scharf**

To sharpen an image, click its rollover **Edit** button and choose Sharpen, or open it in the Browse Panel in Detail view, then click **Sharpen**. Der Anzeigebereich „Schärfe-Editor“ mit den Scharfzeichnungsbefehlen wird geöffnet. Wählen Sie die gewünschten Befehle aus und klicken Sie auf **"Speichern**«.

>[!NOTE]
>
>Bevor Sie ein Bild scharfzeichnen, können Sie im Menü „Vorgabe anwenden“ eine Bildvorgabe auswählen, um deren Effekte für die Scharfzeichnung des Bilds zu sehen. Die Scharfzeichnungseffekte der Bildvorgabe können für das Bild bereits ausreichend sein. Das Menü „Vorgabe anwenden“ befindet sich am unteren Rand des Anzeigebereichs „Schärfe-Editor“.

**Scharfzeichnungsoptionen**

Die folgende Tabelle zeigt die Scharfzeichnungsoptionen des Image-Servers.

| Name | URL-Protokoll | Werte | Beispiel |
|--- |--- |--- |--- |
| Einfaches Scharfzeichnen | op_sharpen | `0 | 1` | op_sharpen=1 |
| Resamplingmodus | resMode | `bilin | bicub | sharp2 | trilin`<br><br>bilin: Wählt bilineare Standardinterpolation aus. Schnellste Neuberechnungsmethode; einige Aliasing-Artefakte sind möglicherweise bemerkbar.<br>bicub: Wählt bikubische Interpolation aus. CPU-intensiver als bilin, erzielt aber schärfere Bilder mit weniger bemerkbaren Aliasing-Artefakten.<br><br>sharp2: Wählt eine modifizierte Lanczos-Fensterfunktion als Interpolationsalgorithmus aus. Kann etwas schärfere Ergebnisse als „bikubisch“ erzeugen, lastet aber die CPU stärker aus.<br><br>trilin: Wählt eine modifizierte trilineare Interpolation aus, die sowohl eine höhere als auch eine niedrigere Auflösung verwendet, falls verfügbar. Wird nur bei Problemen mit dem Aliasing empfohlen. Reduziert JPEG-Größen aufgrund der reduzierten Hochfrequenzdaten. | resMode=sharp2 |
| Unschärfemaske | op_usm | Betrag, Radius, Schwellenwert, Monochromebetrag<br><br>: Filterstärkefaktor (real 0 bis 5)<br><br>Radius: Filterkernradius im <br><br>Pixel-Schwellenwert (real 0 bis 250): Filterschwellenwert (int 0 bis 255)<br><br>Monochrom: auf 0 eingestellt, um jede Farbkomponente separat unscharf zu maskieren, auf 1 eingestellt, um die Bildhelligkeit (Intensität) unscharf zu maskieren | op_usm=1,1,10,0 |

Wählen Sie im Menü „Scharfzeichnen“ eine der folgenden Optionen:

**Keine** deaktiviert Scharfzeichnung.

**Scharfzeichnen** Führt einen einfachen Scharfzeichnungspass für die Datei aus, nachdem die Größe geändert wurde. Dies ist ähnlich wie der Scharfzeichnungsfilter in Photoshop und unterstützt alle Benutzerparameter. Normalerweise würden Sie diesen Filter oder „Unscharf maskieren“ verwenden, aber nicht beide. Diese Methode wird nicht als Best Practice empfohlen, sie kann aber verschwommene Bilder kompensieren. (URL: op_sharpen)

**Unscharf maskieren** Ermöglicht es Ihnen, einen Scharfzeichnungsfiltereffekt auf das endgültige neu berechnete Bild anzupassen. Sie können die Intensität des Effekts, den Radius des Effekts (gemessen in Pixel) und einen Schwellenwert für den Kontrast steuern, der ignoriert wird. Dieser Effekt verwendet die gleichen Optionen wie der Photoshop-Filter „Unscharf maskieren“. (URL: op_usm)

Wählen Sie diese Optionen, um die Scharfzeichnung mit „Unscharf maskieren“ anzupassen:

**Betrag** Steuert den Kontrastgrad, der auf die Kantenpixel angewendet wird. Der Standardwert ist 0,0. Für Bilder mit höherer Auflösung können Sie ihn auf bis zu 5,0 erhöhen. Sie können sich die Auswirkung der Option „Betrag“ wie ein Maß für die Filterintensität vorstellen. Beachten Sie, dass die Einstellung "Betrag" in Dynamic Media Classic nicht mit der Einstellung" Betrag" in Photoshop identisch ist. Photoshop verwendet einen Betrag zwischen 1% und 500%, während dynamischer Media Classic zwischen 0,0 und 5,0 skaliert. (5,0 entspricht ungefähr 500 % in Photoshop, 0,9 ungefähr 90 % usw.)

**Radius** Bestimmt die Anzahl der Pixel um die Kantenpixel, die sich auf das Scharfzeichnen auswirken. Der Effekt wird auf allen Pixeln im Bild ausgeführt und strahlt in alle Richtungen aus. 

Der beste Radiuswert hängt von der Größe des Bilds ab. Bei einem geringeren Wert werden nur die Kantenpixel scharfgezeichnet, während bei einem hohen Wert ein breiterer Pixelbereich scharfgezeichnet wird.

Um beispielsweise einen ähnlichen Scharfzeichnungseffekt für ein 2000 x 2000 Pixel und ein 500 x 2000-Pixelbild zu erhalten, könnten Sie einen Radiuswert von zwei Pixeln auf dem 2000 x 2000 Pixel und einen Radiuswert von einem Pixel auf dem 500 x 500-Pixelbild (bzw. einen größeren Wert für ein Bild mit mehr Pixeln) festlegen. 

**Schwellenwert** Bestimmt den Kontrastbereich, der ignoriert werden soll, wenn der Filter "Unschärfemaske" angewendet wird. Diese Option legt also fest, wie stark sich die scharfgezeichneten Pixel von dem sie umgebenden Bereich unterscheiden müssen, damit sie als Kantenpixel erkannt und scharfgezeichnet werden.

Der Schwellenwert verwendet einen Wert von 0-255, was für die Anzahl der Helligkeitsschritte in einem Graustufenbild steht. 0=schwarz, 128=50 % grau und 255=weiß. Beispiel: Ein Schwellenwert von 12 ignoriert leichte Variationen der Hauttonhelligkeit, um kein Rauschen hinzuzufügen, fügt aber trotzdem Kantenkontrast zu kontrastreichen Bereichen (z. B. wo Wimpern auf die Haut treffen) hinzu. 

Wenn Sie beispielsweise ein Foto mit einem Gesicht einer Person haben, wirkt sich „Unscharf maskieren“ auf die Teile des Bildes mit dem höchsten Kontrast und der glattesten Haut aus. Selbst die glatteste Haut weist subtile Änderungen in Helligkeitswerten auf. Wenn Sie keinen Schwellenwert verwenden, akzentuiert der Filter diese subtilen Änderungen in den Hautpixeln und erzeugt einen Rauscheffekt (der wahrscheinlich unerwünscht ist), während er gleichzeitig den Kontrast an den Wimpern erhöht und somit die Schärfe verbessert (wahrscheinlich wünschenswert). Um dieses Problem zu vermeiden, verwenden Sie einen Schwellenwert, bei dem der Filter Pixel ignoriert, die den Kontrast nicht drastisch ändern, wie z. B. glatte Haut. So vermeiden Sie ein Rauschen oder eine Tontrennung—in Bildern mit Flesh-Tönen—experimentieren Sie mit den Schwellenwertwerten zwischen 2 und 20. Beim Standardschwellenwert von 0 werden alle Pixel im Bild scharfgezeichnet.

**Anwenden,** um jede Farbe auszuwählen, um Scharfzeichnung auf jede Farbkomponente anzuwenden; Wählen Sie "Helligkeit" , um die Scharfzeichnung auf die Helligkeitsbereiche des Bilds anzuwenden.

**Resampling**

Wählen Sie im Menü „Resampling“ eine Option. Mit diesen Optionen wird ein Bild beim Downsampling scharfgezeichnet:

**" Ohne** " deaktiviert die Neuberechnung.

**Bilinear** Die schnellste Neuberechnungsmethode; Einige Aliasing-Artefakte sind bemerkenswert.

**Bikubisch** erhöht die CPU-Auslastung auf dem Image-Server, erzielt jedoch schärfere Bilder mit weniger bemerkbaren Aliasing-Artefakten.

**Sharpen 2** kann etwas schärfere Ergebnisse erzielen als die bikubische Option, aber mit noch höheren CPU-Kosten auf dem Image-Server.

**Trilinear** verwendet sowohl höhere als auch niedrigere Auflösungen, falls verfügbar; wird nur empfohlen, wenn das Aliasing ein Problem ist. Bei dieser Methode wird die JPEG-Dateigröße durch Reduzierung der Hochfrequenzdaten verringert.

**Scharfzeichnen und Bildvorgaben**

Sie können alle drei Scharfzeichnungseffekte mischen, um Ihr Endergebnis zu erzielen. Dies wird allerdings nicht empfohlen. Dynamic Media Classic empfiehlt, Ihre Scharfzeichnungseffekte als Teil einer Bildvorgabe zu speichern. Bildvorgaben ermöglichen es Ihnen, die am häufigsten verwendeten Bildmodifikatoren zu verpacken, um ein dynamisch verkleinertes Bild in einer kleinen Textzeichenfolge zu erstellen. Eine Bildvorgabe enthält Werte für das Dateiformat (normalerweise JPEG für das Web), Pixelanzahl und Bildschärfen. Anstatt die URL bei jedem Bildmodifizierer anzuhängen, der benötigt wird, um einen bestimmten Bildgrößentyp zu erstellen, erstellen Sie eine benannte Bildvorgabe wie z. B. „Miniaturansicht“, konfigurieren die Miniaturbildvorgabe mit der gewünschten Größe, dem Dateiformat und den gewünschten Scharfzeichnungsoptionen und rufen dann das Bild mit dem Bildvorgabenamen auf. Bildvorgaben verkürzen die Länge der Gesamt-URL. Diese beiden URLs erzeugen das gleiche 350 x 350-JPEG-Bild mit Scharfzeichnung. 

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Bildvorgaben können jederzeit geändert und aktualisiert werden. Sie sehen die Ergebnisse einer Änderung an einer Bildvorgabe nach der Veröffentlichung und nachdem der Cache für die URL gelöscht worden ist.

Wenn Sie eine Vorgabe für jedes Bild in einer Größenkategorie verwenden, kann ein Unternehmensadministrator die Definition der jeweiligen Bildvorgabe aktualisieren, sie erneut veröffentlichen und damit jedes Bild mithilfe dieses Formats ändern, ohne Webcode zu ändern. Es empfiehlt sich, eine Bildvorgabe pro Größe auf Ihrer Site zu verwenden. Um eine Bildvorgabe hinzuzufügen, gehen Sie zu „Einstellungen“ &gt; „Anwendungseinstellungen“ &gt; „Bildvorgaben“. Fügen Sie dann eine Vorgabe hinzu oder bearbeiten Sie eine vorhandene Vorgabe. Das einzige erforderliche Feld ist der Name der Vorgabe. Sie sollten jedoch einen gewissen Grad der Scharfzeichnung in jede Vorgabe aufnehmen.

**JPG-Qualität**

Die Optionen für „JPG-Qualität“ bestimmen den JPG-Komprimierungsgrad:

**JPG-Qualität** Wählen Sie diese Option, wenn Sie die Komprimierungsstufen und das Chrominanz-Downsampling steuern möchten.

**Schieberegler** Bestimmt die JPG-Komprimierungsstufe. Diese Einstellung wirkt sich sowohl auf die Dateigröße als auch die Bildqualität aus. Die JPG-Qualitätsskala ist 1-100.

**JPG Chrominanz-Neuberechnung aktivieren** Da das Auge gegenüber Hochfrequenzfarbinformationen weniger empfindlich ist als Hochfrequenzleuchtdichte, teilen JPEG-Bilder Bildinformationen in Leuchtdichte- und Farbkomponenten. Bei der Komprimierung eines JPEG-Bildes behält die Leuchtdichtekomponente die volle Auflösung, während für die Farbkomponenten ein Downsampling, d. h. eine Mittelwerterstellung für Pixelgruppen, ausgeführt wird. Obwohl das Datenvolumen beim Downsampling um die Hälfte oder ein Drittel reduziert wird, ist die auftretende Qualitätsminderung kaum wahrnehmbar. Downsampling kann nicht auf Graustufenbilder angewendet werden. Mit dieser Technik wird der Komprimierungsgrad, der für Bilder mit hohem Kontrast (z. B. Bilder mit überlappendem Text) sinnvoll ist, reduziert.

**Festlegen von unternehmensweiten Scharfzeichnungsoptionen**

Wenn Sie keine Bildvorgabe verwenden oder spezifische Image-Server-Scharfzeichnungsprotokolle mit dem URL-String übergeben, wird das Bild beim Downsampling nicht scharfgezeichnet. Sie können jedoch in diesem Fall die Standard-Scharfzeichnungswerte festlegen, wodurch jedes Bild immer etwas scharfgezeichnet wird.

Um Standard-Scharfzeichnungsoptionen für Ihr Unternehmen festzulegen, gehen Sie zu „Einstellungen“ &gt; „Anwendungseinstellungen“ &gt; „Veröffentlichungseinstellungen“ &gt; „Image-Server“. Wenn Sie den Standard-Resampling-Modus auf „Scharf2“ einstellen, wird das Bild beim Downsampling immer scharfgezeichnet.

**Hinzufügen von Scharfzeichnung zu Viewer-Vorgaben**

Wenn Sie der Vorgabe keine Scharfzeichnungs-Bildmodifizierer hinzufügen, kann das kleine, anfänglich geladene Bild verschwommen aussehen, weil ein Downsampling durchgeführt wurde, um es in das Viewer-Fenster einzupassen, ohne scharfgezeichnet zu werden.

In SPS können Sie mit Viewer-Vorgaben (genau wie mit Bildvorgaben) viele Optionen an einem Ort zentralisieren, z. B. Wahl von Haut- und Viewer-Optionen. (Sie könnten beispielsweise eine Druckschaltfläche einfügen oder die Geschwindigkeit der Zoomanimation steuern.) Viewer-Vorgaben befinden sich im selben Bereich wie Bildvorgaben, und zwar unter „Einstellungen“ &gt; „Anwendungseinstellungen“ &gt; „Viewer-Vorgaben“.

Die Modifiziereroption befindet sich im Bereich „Core-Einstellungen“ aller E-Katalog-, Rotations- und benutzerdefinierter Zoom-Viewer-Vorgaben. Wenn Sie die URL-Scharfzeichnungsbefehle zum Feld „Modifizierer“ hinzufügen, fügen Sie bei jedem Aufruf des Viewers mit der jeweiligen Viewer-Vorgabe Scharfzeichnung hinzu.

Um die Viewer-Vorgabe aufzurufen, verwenden Sie den Befehl „config=“ in der Viewer-URL. Hier ist ein Beispiel für das Aufrufen eines Bildsatzes (Schuhe) mit einer Viewer-Vorgabe (FantasticoZoom2009):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2009`

Diese Vorgabe schärft und ändert die Standardskin des Viewers.

**Erstellen bildspezifischer Abweichungen**

Die letzte und am wenigsten empfohlene Scharfzeichnungsmethode besteht darin, Scharfzeichnungsabweichungen auf Bildbasis zu erstellen. Hierdurch wird die Scharfzeichnung in einer Bildvorgabe mit ihren eigenen spezifischen Werten überschrieben. Allerdings werden hierbei alle anderen Scharfzeichnungsmethoden bei einer beliebigen Größe überschrieben. Der beste Anwendungsfall für diese Methode ist, wenn einige Ihrer Bilder nicht hochauflösend sind und die Werte in den Bildvorgaben für diese kleinen Bilder zu hoch sind. In diesem Fall könnte ein bildabhängiges Scharfzeichnen notwendig sein.

Wählen Sie in SPS ein Bild aus, gehen Sie zur Detailansicht (per Doppelklick oder Klick auf die Schaltfläche „Detailansicht“) und klicken Sie auf „Scharfzeichnen“. Ändern Sie die gewünschten Parameter und klicken Sie dann auf „Speichern“. Hierdurch wird dem Image-Server mitgeteilt, diese Scharfzeichnungsparameter anstatt eines Befehls zu verwenden, den Sie in der URL aufrufen, wie z. B. einen Scharfzeichnungsmodifizierer oder eine Bildvorgabe. Sie müssen veröffentlichen, damit die Änderungen wirksam werden.
