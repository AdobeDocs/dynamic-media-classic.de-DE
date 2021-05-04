---
title: Scharfzeichnen eines Bildes
description: Erfahren Sie, wie Sie ein Bild scharfzeichnen.
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
feature: Dynamic Media Classic, Asset Management
role: Business Practitioner
exl-id: 4b3e8368-f8f5-46d9-9130-361a8273de2c
translation-type: tm+mt
source-git-commit: 9d73e74ffc4a1e7e31c84720a9bae105b6afb1ae
workflow-type: tm+mt
source-wordcount: '2169'
ht-degree: 46%

---

# Scharfzeichnen eines Bildes {#sharpening-an-image}

Mit der Bildbearbeitungstechnik des Scharfzeichnens werden die Umrisse eines digitalen Bilds deutlicher dargestellt. Beim Scharfzeichnen wird der Kontrast zwischen den Randpixeln erhöht und der Übergang zwischen dunklen und hellen Bereichen dadurch hervorgehoben. Durch Scharfzeichnen wird der lokale Kontrast erhöht und die feinen Details kommen deutlicher zur Geltung. Es gibt keine feste Formel für das korrekte Scharfzeichnen aller Bilder. Bei zu geringem Scharfzeichnen können die Konturen des Bilds verschwommen wirken, während zu starkes Scharfzeichnen helle Ränder an den Kanten (Halos), Störungen und Bildrauschen verursachen kann.

Dynamic Media Classic empfiehlt dringend, Bildvorgaben für alle Bilder zu verwenden. Sie stellen eine einheitliche Größe sicher und das Scharfzeichnen wird für jedes Bild erzwungen, das mit einer Bildvorgabe aufgerufen wird. Darüber hinaus können Sie die Scharfzeichnungsparameter einer Bildvorgabe einfach bearbeiten und ändern. Wenn Sie das nächste Mal eine Veröffentlichung vornehmen, erhalten alle Bilder, die mit dieser Vorgabe aufgerufen werden, die neuen Werte.

Dynamic Media Classic empfiehlt außerdem, den Viewer-Vorgaben Scharfzeichnung hinzuzufügen und dann einen Viewer mit dieser Vorgabe aufzurufen. Dadurch wird sichergestellt, dass Bilder in Ihren Viewern klar und ansprechend sind.

Unabhängig davon, ob Sie Bildvorgaben und Viewer-Vorgaben oder eine andere Methode des Scharfzeichnens verwenden, müssen Sie Ihre Bilder scharfzeichnen. Andernfalls können Ihre Bilder (und Websites) verschwommen und verschwommen aussehen.

>[!NOTE]
>
>Mit dem Befehl „Scharfzeichnen“ werden die Einstellungen unter „Bildvorgaben“, einschließlich der dort angegebenen Scharfzeichnungseinstellungen, überschrieben. Eine Bildvorgabe regelt die Größe und Formatierung, mit der Bilder von Dynamic Media-Image-Servern bereitgestellt werden. Dynamic Media Classic empfiehlt die Verwendung von Bildvorgaben, um alle Bilder bereitzustellen, um sicherzustellen, dass sie einheitlich und scharfgezeichnet dargestellt werden. Wenn jedoch die Scharfzeichnungseinstellungen für ein einzelnes Bild geändert wurden, gelten die Scharfzeichnungseinstellungen der Bildvorgabe nicht mehr für dieses Bild. Es wird dann ohne Anwendung der Scharfzeichnungseinstellungen der Bildvorgabe gesendet.

Es ist oft notwendig, Bilder scharfzuzeichnen. Dynamic Media Classic- und Image-Server-Angebot bieten mehrere Scharfzeichnungsoptionen. Es ist wichtig zu wissen, was das Scharfzeichnen bei einem Bild bewirkt und wie viel Scharfzeichnung Sie benötigen. Die meisten Bilder müssen etwas scharfgezeichnet werden, aber der Grad der Scharfzeichnung hängt vom Bild ab.

Die Bildschärfung erhöht den Kontrast der Pixel, um den Eindruck zu erwecken, dass die Kanten akzentuiert sind. Menschen nehmen diesen erhöhten Kantenkontrast als Schärfe wahr. Obwohl es einfach ist, ein Bild mithilfe von Scharfzeichnungsfiltern zu verbessern, ist es auch einfach, ein Bild zu stark scharfzuzeichnen.

Wenn ein Bild zu stark scharfgezeichnet ist, entsteht ein Halo- oder Banding-Effekt.

Es gibt Best Practices, die Sie zur Optimierung der Scharfzeichnung Ihrer Bilder in Dynamic Media Classic und auf Dynamic Media Image Server befolgen können.

Siehe [Bewährte Verfahren zum Scharfzeichnen von Bildern in Dynamic Media Classic und auf Dynamic Media Image Server](/help/assets/s7_sharpening_images.pdf).

**So zeichnen Sie ein Bild scharf:**

Um ein Bild scharfzuzeichnen, klicken Sie auf seine Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** und wählen Sie **[!UICONTROL Scharfzeichnen]** oder öffnen Sie es im Durchsuchenbedienfeld in der Ansicht &quot;Details&quot;und klicken Sie dann auf **[!UICONTROL Scharfzeichnen]**. Die Seite &quot;Schärfe-Editor&quot;wird mit Scharfzeichnungsbefehlen geöffnet. Wählen Sie Befehle und klicken Sie dann auf **[!UICONTROL Speichern]**.

>[!NOTE]
>
>Bevor Sie ein Bild scharfzeichnen, können Sie im Menü „Vorgabe anwenden“ eine Bildvorgabe auswählen, um deren Effekte für die Scharfzeichnung des Bilds zu sehen. Die Scharfzeichnungseffekte einer Bildvorgabe sind für Ihr Bild geeignet. Das Menü **[!UICONTROL Vorgabe anwenden]** befindet sich unten auf der Seite &quot;Schärfe-Editor&quot;.

**Scharfzeichnungsoptionen**

Die folgende Tabelle zeigt die Scharfzeichnungsoptionen des Image-Servers.

| Name | URL-Protokoll | Werte | Beispiel |
|--- |--- |--- |--- |
| Einfaches Scharfzeichnen | op_sharpen | `0 | 1` | op_sharpen=1 |
| Resamplingmodus | resMode | `bilin | bicub | sharp2 | trilin`<br><br>bilin: Wählt bilineare Standardinterpolation aus. Schnellste Neuberechnungsmethode; einige Aliasing-Artefakte sind häufig bemerkbar.<br>bicub: Wählt bikubische Interpolation aus. CPU-intensiver als bilin, erzielt aber schärfere Bilder mit weniger bemerkbaren Aliasing-Artefakten.<br><br>sharp2: Wählt eine geänderte Lanczos Windows®-Funktion als Interpolationsalgorithmus aus. Kann etwas schärfere Ergebnisse als bikubisch bei höheren CPU-Kosten erzielen.<br><br>trilin: Wählt eine modifizierte trilineare Interpolation aus, die sowohl eine höhere als auch eine niedrigere Auflösung verwendet, falls verfügbar. Wird nur bei Problemen mit dem Aliasing empfohlen. Reduziert JPEG-Größen aufgrund der reduzierten Hochfrequenzdaten. | resMode=sharp2 |
| Unschärfemaske | op_usm | Betrag, Radius, Schwellenwert, monochrom<br><br>Betrag: Filterfestigkeitsfaktor (real 0...5)<br><br>Radius: Filterkernradius in Pixel (real 0...250) <br><br>Schwellenwert: Filterschwellenwert (int 0...255)<br><br>Monochrom: auf 0 gesetzt, um jede Farbkomponente separat unscharf zu maskieren, auf 1 eingestellt, um Bildhelligkeit (Intensität) unscharf zu maskieren | op_usm=1,1,10,0 |

Wählen Sie im Menü **[!UICONTROL Scharfzeichnen]** eine Option:

* **Ohne**  - Deaktiviert das Scharfzeichnen.

* **Scharfzeichnen** : Führt einen einfachen Scharfzeichnungsdurchlauf für die Datei aus, nachdem die Größe geändert wurde. Es ähnelt dem Scharfzeichnungsfilter in Adobe Photoshop und unterstützt alle Benutzerparameter. Normalerweise würden Sie diesen Filter oder **[!UICONTROL Unschärfemaske]** verwenden, aber nicht beides. Diese Methode wird nicht als Best Practice empfohlen, sie kann aber verschwommene Bilder kompensieren. (URL: `op_sharpen`)

* **Unscharf maskieren** : Ermöglicht die Feinabstimmung eines Scharfzeichnungsfiltereffekts auf das endgültige neu berechnete Bild. Sie können die Intensität des Effekts, den Radius des Effekts (gemessen in Pixel) und einen Schwellenwert für den Kontrast festlegen, der ignoriert wird. Dieser Effekt verwendet dieselben Optionen wie der Photoshop-Filter „Unscharf maskieren“. (URL: `op_usm`)

Wählen Sie diese Optionen, um das Scharfzeichnen mit &quot;Unscharf maskieren&quot;genauer einzustellen:

* **Stärke** : Steuert den Kontrastgrad, der auf Kantenpixel angewendet wird. Der Standardwert ist 0,0. Für Bilder mit höherer Auflösung können Sie ihn auf bis zu 5,0 erhöhen. Sie können sich die Auswirkung der Option „Betrag“ wie ein Maß für die Filterintensität vorstellen. Die Einstellung **[!UICONTROL Amount]** in Dynamic Media Classic ist nicht mit der Einstellung Amount in Adobe Photoshop identisch. Adobe Photoshop verwendet einen Betrag zwischen 1 % und 500 %, während Dynamic Media Classic zwischen 0,0 und 5,0 skaliert. (5,0 entspricht ungefähr 500 % in Photoshop, 0,9 ungefähr 90 % usw.)

* **Radius** : Bestimmt die Anzahl der Pixel um die Kantenpixel, die sich auf das Scharfzeichnen auswirken. Der Effekt wird auf allen Pixeln im Bild ausgeführt und strahlt in alle Richtungen aus. 

Der beste Radiuswert hängt von der Größe des Bilds ab. Bei einem geringeren Wert werden nur die Kantenpixel scharfgezeichnet, während bei einem hohen Wert ein breiterer Pixelbereich scharfgezeichnet wird.

Wenn Sie beispielsweise einen ähnlichen Scharfzeichnungseffekt für ein Bild mit 2000 x 2000 Pixel und ein Bild mit 500 x 500 Pixel erzielen möchten, können Sie einen Radiuswert von zwei Pixeln für das Bild mit 2000 x 2000 Pixel festlegen. einen Radiuswert von einem Pixel auf dem 500 x 500-Pixelbild (bzw. einen größeren Wert für ein Bild mit mehr Pixeln) festlegen. 

* **** SchwellenwertBestimmt den Kontrastbereich, der ignoriert werden soll, wenn der Filter &quot;Unschärfemaske&quot;angewendet wird. Diese Option legt also fest, wie stark sich die scharfgezeichneten Pixel von dem sie umgebenden Bereich unterscheiden müssen, damit sie als Kantenpixel erkannt und scharfgezeichnet werden.

Der Schwellenwert verwendet einen Wert von 0-255, was für die Anzahl der Helligkeitsschritte in einem Graustufenbild steht. 0=schwarz, 128=50 % grau und 255=weiß. Beispiel: Ein Schwellenwert von 12 ignoriert leichte Variationen der Hauttonhelligkeit, um kein Rauschen hinzuzufügen, fügt aber trotzdem Kantenkontrast zu kontrastreichen Bereichen (z. B. wo Wimpern auf die Haut treffen) hinzu. 

Wenn Sie beispielsweise ein Foto mit einem Gesicht einer Person haben, wirkt sich „Unscharf maskieren“ auf die Teile des Bildes mit dem höchsten Kontrast und der glattesten Haut aus. Selbst die glatteste Haut weist subtile Änderungen in Helligkeitswerten auf. Wenn Sie keinen Schwellenwert verwenden, akzentuiert der Filter diese subtilen Änderungen in den Hautpixeln und erzeugt einen Rauscheffekt (der wahrscheinlich unerwünscht ist), während er gleichzeitig den Kontrast an den Wimpern erhöht und somit die Schärfe verbessert (wahrscheinlich wünschenswert). Um dieses Problem zu vermeiden, verwenden Sie einen Schwellenwert, bei dem der Filter Pixel ignoriert, die den Kontrast nicht drastisch ändern, wie z. B. glatte Haut. Um zu vermeiden, dass Rauschen oder posterisierende Bilder mit Fleischtönen verwendet werden, versuchen Sie beispielsweise mit den Werten **[!UICONTROL Schwellenwert]** zwei bis 20 zu experimentieren. Der Standardwert **[!UICONTROL Threshold]** von 0 schärft alle Pixel im Bild.

* **Anwenden auf** : Wählen Sie  **[!UICONTROL jede]** Farbe aus, auf die Sie die Scharfzeichnung separat auf jede Farbkomponente anwenden möchten. Wählen Sie &quot; **** Helligkeit&quot;, wenn Sie die Scharfzeichnung auf die Helligkeitsbereiche anwenden möchten.

**Resampling**

Klicken Sie auf das Menü **[!UICONTROL Resampling]** und wählen Sie eine Option. Mit diesen Optionen wird ein Bild beim Downsampling scharfgezeichnet:

* **Keine**  - Deaktiviert die Neuberechnung.

* **Bilinear** - Die schnellste Neuberechnungsmethode; einige Aliasing-Artefakte sind bemerkbar.

* **Bikubisch** : Erhöht die CPU-Auslastung auf dem Image-Server, erzielt aber schärfere Bilder mit weniger bemerkbaren Aliasing-Artefakten.

* **Scharfzeichnen2**  - Erzeugt etwas schärfere Ergebnisse als  **[!UICONTROL bikubisch]**, aber bei noch höheren CPU-Kosten auf dem Image-Server.

* **Trilinear**  - Verwendet sowohl höhere als auch niedrigere Auflösungen, sofern verfügbar; wird nur empfohlen, wenn das Aliasing ein Problem darstellt. Bei dieser Methode wird die JPEG-Dateigröße durch Reduzierung der Hochfrequenzdaten verringert.

**Scharfzeichnen und Bildvorgaben**

Sie können alle drei Scharfzeichnungseffekte einbeziehen, um Ihr Endergebnis zu erzielen. Diese Methode wird jedoch nicht empfohlen. Dynamic Media Classic empfiehlt, die Scharfzeichnungseffekte als Teil einer Bildvorgabe zu speichern. Mit Bildvorgaben können Sie die am häufigsten verwendeten Bildmodifikatoren verpacken, um ein dynamisch angepasstes Bild in einer kleinen Textzeichenfolge zu erstellen. Eine Bildvorgabe enthält Werte für das Dateiformat (normalerweise JPEG für das Web), die Pixelanzahl und das Scharfzeichnen von Bildern. Anstatt die URL mit jedem Bildmodifikator anzuhängen, den Sie zum Erstellen eines bestimmten Bildgrößentyps verwenden müssen, erstellen Sie eine benannte Bildvorgabe, z. B. &quot;Miniaturansicht&quot;. Konfigurieren Sie dann die Bildvorgabe für die Miniaturansicht mit den entsprechenden Größen-, Dateiformat- und Scharfzeichnungsoptionen. Rufen Sie das Bild mit dem Namen der Bildvorgabe auf. Bildvorgaben verkürzen die Länge der gesamten URL. Diese beiden URLs erzeugen dasselbe JPEG-Bild im Format 350 x 350 mit Scharfzeichnung:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Bildvorgaben können jederzeit geändert und aktualisiert werden. Die Ergebnisse einer Änderung an einer Bildvorgabe werden angezeigt, nachdem Sie sie veröffentlicht haben und nachdem der Cache für die URL gelöscht wurde.

Wenn Sie eine Vorgabe für jedes Bild in einer Größenkategorie verwenden, kann ein Unternehmensadministrator die Definition der jeweiligen Bildvorgabe aktualisieren, sie erneut veröffentlichen und damit jedes Bild mithilfe dieses Formats ändern, ohne Webcode zu ändern. Es empfiehlt sich, eine Bildvorgabe pro Größe auf Ihrer Site zu verwenden. Um eine Bildvorgabe hinzuzufügen, klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Bildvorgaben]**. Klicken Sie dann auf **[!UICONTROL Hinzufügen]** oder auf **[!UICONTROL Bearbeiten]**, um eine vorhandene Vorgabe zu ändern. Das einzige erforderliche Feld ist der Name der Vorgabe. Es empfiehlt sich jedoch, in jede Vorgabe ein gewisses Maß an Scharfzeichnung aufzunehmen.

**JPG-Qualität**

Die Optionen für „JPG-Qualität“ bestimmen den JPG-Komprimierungsgrad:

* **JPG-Qualität** : Wählen Sie diese Option, wenn Sie Komprimierungsstufen und Chrominanz-Downsampling steuern möchten.

* **Schieberegler** : Bestimmt die JPG-Komprimierungsstufe. Diese Einstellung wirkt sich sowohl auf die Dateigröße als auch die Bildqualität aus. Die JPG-Qualitätsskala ist 1-100.

* **JPG-Chrominanz-Neuberechnung**  aktivieren - Da das Auge für hochfrequente Farbinformationen weniger empfindlich ist als für hochfrequente Leuchtdichte, teilen JPEG-Bilder Bildinformationen in Leuchtdichte- und Farbkomponenten. Bei der Komprimierung eines JPEG-Bildes behält die Leuchtdichtekomponente die volle Auflösung, während für die Farbkomponenten ein Downsampling, d. h. eine Mittelwerterstellung für Pixelgruppen, ausgeführt wird. Obwohl das Datenvolumen beim Downsampling um die Hälfte oder ein Drittel reduziert wird, ist die auftretende Qualitätsminderung kaum wahrnehmbar. Downsampling kann nicht auf Graustufenbilder angewendet werden. Mit dieser Technik wird der Komprimierungsgrad, der für Bilder mit hohem Kontrast (z. B. Bilder mit überlappendem Text) sinnvoll ist, reduziert.

**Festlegen von unternehmensweiten Scharfzeichnungsoptionen**

Wenn Sie keine Bildvorgabe verwenden oder spezifische Image-Server-Scharfzeichnungsprotokolle mit dem URL-String übergeben, wird das Bild beim Downsampling nicht scharfgezeichnet. Tritt diese fehlende Scharfzeichnung auf, können Sie die standardmäßigen Scharfzeichnungswerte festlegen und jedes Bild wird immer scharfgezeichnet.

Um die standardmäßigen Scharfzeichnungsoptionen für Ihre Firma festzulegen, klicken Sie auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Veröffentlichungseinstellungen]** > **[!UICONTROL Image-Server]**. Wenn Sie als Standard-Resamplingmodus **[!UICONTROL Sharp2]** festlegen, wird das Bild beim Downsampling immer scharfgezeichnet.

**Hinzufügen von Scharfzeichnung zu Viewer-Vorgaben**

Wenn Sie der Vorgabe keine Scharfzeichnungs-Bildmodifizierer hinzufügen, kann das kleine, anfänglich geladene Bild verschwommen aussehen, weil ein Downsampling durchgeführt wurde, um es in das Viewer-Fenster einzupassen, ohne scharfgezeichnet zu werden.

Mit Viewer-Vorgaben (z. B. Bildvorgaben) können Sie viele Optionen an einem Ort zentralisieren, z. B. die Auswahl der Haut- und Viewer-Optionen (z. B. die Eingabe einer Drucken-Schaltfläche oder die Steuerung der Zoomanimation). Viewer-Vorgaben befinden sich im selben Abschnitt wie Bildvorgaben unter **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Viewer-Vorgaben]**.

Die Modifiziereroption befindet sich im Bereich „Core-Einstellungen“ aller E-Katalog-, Rotations- und benutzerdefinierter Zoom-Viewer-Vorgaben. Wenn Sie die URL-Scharfzeichnungsbefehle zum Feld „Modifizierer“ hinzufügen, fügen Sie bei jedem Aufruf des Viewers mit der jeweiligen Viewer-Vorgabe Scharfzeichnung hinzu.

Um die Viewer-Vorgabe aufzurufen, verwenden Sie den Befehl `config=` in der Viewer-URL. Hier ist ein Beispiel für das Aufrufen eines Bildsatzes (Schuhe) mit einer Viewer-Vorgabe (`FantasticoZoom2022`):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

Diese Vorgabe schärft und ändert die Standardskin des Viewers.

**Erstellen bildspezifischer Abweichungen**

Die letzte und am wenigsten empfohlene Scharfzeichnungsmethode besteht darin, Scharfzeichnungsabweichungen auf Bildbasis zu erstellen. Diese Methode überschreibt das Scharfzeichnen in einer Bildvorgabe mit ihren eigenen spezifischen Werten. Diese Methode überschreibt jedoch auch alle anderen Scharfzeichnungsmethoden jeder Größe. Der beste Anwendungsfall für diese Methode ist, wenn einige Ihrer Bilder nicht hochauflösend sind und die Werte in den Bildvorgaben für diese kleinen Bilder zu hoch sind. In diesem Fall ist möglicherweise eine einzelne Scharfzeichnung pro Bild erforderlich.

Wählen Sie in Dynamic Media Classic ein beliebiges Bild aus, gehen Sie zur Ansicht &quot;Detail&quot;(durch Klicken auf oder Drücken der Taste **[!UICONTROL Detail-Ansicht]**) und klicken Sie auf **[!UICONTROL Scharfzeichnen]**. Ändern Sie einen beliebigen Parameter und klicken Sie dann auf **[!UICONTROL Speichern]**. Dieser Prozess weist den Image-Server an, diese Scharfzeichnungsparameter anstelle eines Befehls zu verwenden, den Sie in der URL aufrufen, z. B. einen Scharfzeichnungs-Modifikator oder eine Bildvorgabe. Vergewissern Sie sich, dass Sie veröffentlichen, damit die Änderungen wirksam werden.
