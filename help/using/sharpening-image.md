---
title: Bilder scharfzeichnen
description: Erfahren Sie, wie Sie ein Bild in Adobe Dynamic Media Classic scharfzeichnen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3e8368-f8f5-46d9-9130-361a8273de2c
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '2207'
ht-degree: 30%

---

# Bilder scharfzeichnen {#sharpening-an-image}

Mit der Bildbearbeitungstechnik des Scharfzeichnens werden die Umrisse eines digitalen Bilds deutlicher dargestellt. Beim Scharfzeichnen wird der Kontrast zwischen den Randpixeln erhöht und der Übergang zwischen dunklen und hellen Bereichen dadurch hervorgehoben. Durch Scharfzeichnen wird der lokale Kontrast erhöht und die feinen Details kommen deutlicher zur Geltung. Es gibt keine feste Formel für das korrekte Scharfzeichnen aller Bilder. Bei zu geringem Scharfzeichnen können die Konturen des Bilds verschwommen wirken, während zu starkes Scharfzeichnen helle Ränder an den Kanten (Halos), Störungen und Bildrauschen verursachen kann.

Adobe Dynamic Media Classic empfiehlt dringend die Verwendung von Bildvorgaben für alle Bilder. Sie stellen sicher, dass eine einheitliche Größe vorliegt und die Scharfzeichnung für jedes Bild erzwungen wird, das mit einer Bildvorgabe aufgerufen wird. Darüber hinaus können Sie die Scharfzeichnungsparameter einer Bildvorgabe einfach bearbeiten und ändern. Wenn Sie das nächste Mal eine Veröffentlichung vornehmen, erhalten alle Bilder, die mit dieser Vorgabe aufgerufen werden, die neuen Werte.

Adobe Dynamic Media Classic empfiehlt auch, Scharfzeichnung zu Viewer-Vorgaben hinzuzufügen und dann einen Viewer mit dieser Vorgabe aufzurufen. Dadurch wird sichergestellt, dass die Bilder für Ihre Betrachter scharf und attraktiv sind.

Unabhängig davon, ob Sie Bildvorgaben und Viewer-Vorgaben oder eine Methode der Scharfzeichnung verwenden, besteht das Endergebnis darin, dass Sie Ihre Bilder scharfzeichnen müssen. Wenn Sie dies nicht tun, können Ihre Bilder (und die Website) weich und unscharf aussehen.

>[!NOTE]
>
>Mit dem Befehl „Scharfzeichnen“ werden die Einstellungen unter „Bildvorgaben“, einschließlich der dort angegebenen Scharfzeichnungseinstellungen, überschrieben. Eine Bildvorgabe legt die Größe und Formatierung fest, mit der Bilder von Dynamic Media-Bildservern bereitgestellt werden. Adobe Dynamic Media Classic empfiehlt dringend die Verwendung von Bildvorgaben, um alle Bilder bereitzustellen, um sicherzustellen, dass Bilder in einheitlicher Größe und Scharfzeichnung bereitgestellt werden. Wenn jedoch die Scharfzeichnungseinstellungen für ein einzelnes Bild geändert wurden, gelten die Scharfzeichnungseinstellungen der Bildvorgabe nicht mehr für dieses Bild. Es wird dann ohne Anwendung der Scharfzeichnungseinstellungen der Bildvorgabe gesendet.

Es ist oft notwendig, Bilder scharfzuzeichnen. Adobe Dynamic Media Classic- und Image-Server bieten mehrere Scharfzeichnungsoptionen. Es ist wichtig zu wissen, was das Scharfzeichnen bei einem Bild bewirkt und wie viel Scharfzeichnung Sie benötigen. Die meisten Bilder müssen etwas scharfgezeichnet werden, aber der Grad der Scharfzeichnung hängt vom Bild ab.

Die Bildschärfung erhöht den Kontrast der Pixel, um den Eindruck zu erwecken, dass die Kanten akzentuiert sind. Menschen nehmen diesen erhöhten Kantenkontrast als Schärfe wahr. Obwohl es einfach ist, ein Bild mithilfe von Scharfzeichnungsfiltern zu verbessern, ist es auch einfach, ein Bild zu stark scharfzuzeichnen.

Das übermäßige Scharfzeichnen eines Bildes erzeugt einen Halo-Effekt oder das Banding der Kantenlinien.

Es gibt Best Practices, die Sie anwenden können, um die Scharfzeichnung Ihrer Bilder in Adobe Dynamic Media Classic und auf dem Dynamic Media Image Server zu optimieren.

Siehe [Best Practices für das Scharfzeichnen von Bildern in Adobe Dynamic Media Classic und auf Dynamic Media Image Server](/help/using/assets/s7_sharpening_images.pdf).

Siehe auch Schulungsvideo zum [Scharfzeichnen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) .

**So scharfzeichnen Sie ein Bild:**

Um ein Bild scharfzuzeichnen, klicken Sie auf die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** und wählen Sie **[!UICONTROL Scharfzeichnen]**, öffnen Sie es im Durchsuchenbedienfeld in der Detailansicht und wählen Sie dann **[!UICONTROL Scharfzeichnen]** aus. Die Seite mit dem Scharfzeichnungseditor wird mit Scharfzeichnungsbefehlen geöffnet. Wählen Sie die gewünschten Befehle aus und klicken Sie dann auf **[!UICONTROL Speichern]**.

>[!NOTE]
>
>Bevor Sie ein Bild scharfzeichnen, können Sie im Menü „Vorgabe anwenden“ eine Bildvorgabe auswählen, um deren Effekte für die Scharfzeichnung des Bilds zu sehen. Die Scharfzeichnungseffekte einer Bildvorgabe sind für Ihr Bild geeignet. Das Menü **[!UICONTROL Voreinstellung anwenden]** befindet sich unten auf der Seite &quot;Schärfe-Editor&quot;.

**Scharfzeichnungsoptionen**

Die folgende Tabelle zeigt die Scharfzeichnungsoptionen des Image-Servers.

| Name | URL-Protokoll | Werte | Beispiel |
| --- | --- | --- | --- |
| Einfaches Scharfzeichnen | `op_sharpen` | `0` oder `1` | `op_sharpen=1` |
| Resamplingmodus | `resMode` | `bilin`, `bicub`, `sharp2`, `trilin`<br><br>`bilin`: Wählt die standardmäßige bilineare Interpolation aus. Schnellste Resampling-Methode; einige Aliasing-Artefakte sind häufig sichtbar.<br>`bicub`: Wählt bikubische Interpolation aus. CPU-intensiver als `bilin`, liefert jedoch schärfere Bilder mit weniger deutlichen Aliasing-Artefakten.<br><br>`sharp2`: Wählt eine geänderte Windows®-Funktion von Lanczos als Interpolationsalgorithmus aus. Es kann etwas schärfere Ergebnisse als bikubisch bei höheren CPU-Kosten erzielen.<br><br>`trilin`: Wählt eine modifizierte trilineare Interpolation aus, die sowohl eine höhere als auch eine niedrigere Auflösung verwendet, sofern verfügbar. Wird nur bei Problemen mit dem Aliasing empfohlen. Reduziert JPEG-Größen aufgrund der reduzierten Hochfrequenzdaten. | `resMode=sharp2` |
| Unschärfemaske | `op_usm` | `amount`, `radius`, `threshold`, `monochrome`<br><br>`amount`: Filterstärke Faktor (real 0...5)<br><br>`radius`: Filterkernel-Radius in Pixel (real 0...250) <br><br>`threshold`: Filterschwellenwert (int 0...255)<br><br>`monochrome`: auf `0` eingestellt, um die Unschärfemaske für jede Farbkomponente einzeln festzulegen, auf `1` (Intensität) | `op_usm=1,1,10,0` |

Wählen Sie das Menü **[!UICONTROL Scharfzeichnen]** aus und wählen Sie eine Option:

* **None**: Deaktiviert die Scharfzeichnung.

* **Scharfzeichnen**: Führt einen einfachen Scharfzeichnungsdurchlauf für die Datei aus, nachdem die Größe geändert wurde. Sie ähnelt dem Filter &quot;Scharfzeichnen&quot;in Adobe Photoshop und unterstützt alle Benutzerparameter. Normalerweise würden Sie diesen Filter oder **[!UICONTROL Unschärfemaske]** verwenden, aber nicht beides. Diese Methode wird nicht als Best Practice empfohlen, sie kann aber verschwommene Bilder kompensieren. (URL: `op_sharpen`)

* **Unschärfemaske**: Hiermit können Sie einen Scharfzeichnungsfiltereffekt für das endgültige heruntergesampelte Bild optimieren. Sie können die Intensität des Effekts, den Radius des Effekts (gemessen in Pixel) und einen Schwellenwert für den ignorierten Kontrast festlegen. Dieser Effekt verwendet dieselben Optionen wie der Photoshop-Filter &quot;Unschärfemaske&quot;. (URL: `op_usm`)

Wählen Sie diese Optionen aus, damit Sie die Scharfzeichnung mit der Unschärfemaske optimieren können:

* **Betrag**: Steuert den auf Kantenpixel angewendeten Kontrastwert. Der Standardwert ist 0,0. Für Bilder mit höherer Auflösung können Sie ihn auf bis zu 5,0 erhöhen. Sie können sich die Auswirkung der Option „Betrag“ wie ein Maß für die Filterintensität vorstellen. Die Einstellung **[!UICONTROL Amount]** in Adobe Dynamic Media Classic ist nicht die gleiche wie die Einstellung Amount in Adobe Photoshop. Adobe Photoshop verwendet einen Betrag zwischen 1 % und 500 %, während Adobe Dynamic Media Classic zwischen 0,0 und 5,0 skaliert. (5,0 entspricht ungefähr 500 % in Photoshop, 0,9 ungefähr 90 % usw.)

* **Radius**: Bestimmt die Anzahl der Pixel um die Kantenpixel, die sich auf die Scharfzeichnung auswirken. Der Effekt wird auf allen Pixeln im Bild ausgeführt und strahlt in alle Richtungen aus. 

Der beste Radiuswert hängt von der Größe des Bilds ab. Bei einem geringeren Wert werden nur die Kantenpixel scharfgezeichnet, während bei einem hohen Wert ein breiterer Pixelbereich scharfgezeichnet wird.

Um beispielsweise einen ähnlichen Scharfzeichnungseffekt für ein 2000 × 2000 Pixelbild und ein 500 × 500 Pixelbild zu erhalten, können Sie einen Radius-Wert von zwei Pixel auf dem 2000 × 2000 Pixelbild festlegen. Legen Sie dann einen Radius-Wert von einem Pixel auf dem Bild mit 500 × 500 Pixel fest (ein größerer Wert für ein Bild mit mehr Pixel).

* **Schwellenwert**: Bestimmt den Kontrastbereich, der bei Anwendung des Filters &quot;Unschärfemaske&quot;ignoriert werden soll. Diese Option bestimmt, wie stark sich die scharfgezeichneten Pixel vom Umgebungsbereich unterscheiden müssen, damit die Kantenpixel scharfgezeichnet werden.

Der Schwellenwert verwendet einen Wert zwischen 0 und 255, was der Anzahl der Helligkeitsschritte in einem Graustufenbild entspricht. 0=schwarz, 128=50 % grau und 255=weiß. Bei einem Schwellenwert von 12 werden beispielsweise leichte Variationen der Hauttonhelligkeit ignoriert. Dadurch wird kein Rauschen hinzugefügt, während kontrastreichen Bereichen, z. B. wo Wimpern auf die Haut treffen, Kantenkontrast hinzugefügt wird.

Angenommen, Sie haben ein Foto von jemandes Gesicht. wirkt sich „Unscharf maskieren“ auf die Teile des Bildes mit dem höchsten Kontrast und der glattesten Haut aus. Selbst die glatteste Haut weist subtile Änderungen in Helligkeitswerten auf. Wenn Sie keinen Schwellenwert verwenden, akzentuiert der Filter diese subtilen Änderungen in den Hautpixeln und erzeugt einen Rauscheffekt (der wahrscheinlich unerwünscht ist), während er gleichzeitig den Kontrast an den Wimpern erhöht und somit die Schärfe verbessert (wahrscheinlich wünschenswert). Um dieses Problem zu vermeiden, verwenden Sie einen Schwellenwert, bei dem der Filter Pixel ignoriert, die den Kontrast nicht drastisch ändern, wie z. B. glatte Haut. Um Rauschen oder posterisierende Bilder mit Fleischtönen zu vermeiden, experimentieren Sie beispielsweise mit den Werten **[!UICONTROL Schwellenwert]** zwischen zwei und 20. Mit dem Standardwert **[!UICONTROL Schwellenwert]** von 0 werden alle Pixel im Bild scharfgezeichnet.

* **Anwenden auf**: Wählen Sie **[!UICONTROL Jede Farbe]** aus, wenn Sie die Scharfzeichnung separat auf jede Farbkomponente anwenden möchten. Wählen Sie **[!UICONTROL Helligkeit]**, wenn Sie die Scharfzeichnung auf die Bildhelligkeitsbereiche anwenden möchten.

**Resampling**

Wählen Sie das Menü **[!UICONTROL Resampling]** aus und wählen Sie eine Option. Mit diesen Optionen wird ein Bild beim Downsampling scharfgezeichnet:

* **[!UICONTROL None]**: Deaktiviert die Neuberechnung.

* **[!UICONTROL Bilinear]**: Die schnellste Resampling-Methode; einige Aliasing-Artefakte sind sichtbar.

* **[!UICONTROL Bikubisch]**: Erhöht die CPU-Auslastung auf dem Image-Server, liefert jedoch schärfere Bilder mit weniger deutlichen Aliasing-Artefakten.

* **[!UICONTROL `Sharpen 2`]**: Erzeugt etwas schärfere Ergebnisse als **[!UICONTROL Bikubisch]**, jedoch zu noch höheren CPU-Kosten auf dem Image-Server.

* **[!UICONTROL Trilinear]**: Verwendet sowohl höhere als auch niedrigere Auflösungen, sofern verfügbar. Wird nur empfohlen, wenn das Aliasing ein Problem darstellt. Bei dieser Methode wird die JPEG-Dateigröße durch Reduzierung der Hochfrequenzdaten verringert.

**Bildvorgaben und Scharfzeichnen**

Sie können alle drei Scharfzeichnungseffekte integrieren, um Ihr Endergebnis zu erzielen. Diese Methode wird jedoch nicht empfohlen. Adobe Dynamic Media Classic empfiehlt, die Scharfzeichnungseffekte als Teil einer Bildvorgabe zu speichern. Mit Bildvorgaben können Sie die am häufigsten verwendeten Bild-Modifikatoren verpacken, um ein dynamisch in der Größe angepasstes Bild in einer kleinen Textzeichenfolge zu erstellen. Eine Bildvorgabe enthält Werte für das Dateiformat (normalerweise JPEG für das Web), die Pixelanzahl und die Bildschärfe. Anstatt die URL mit jedem Bild-Modifikator anzuhängen, den Sie zum Erstellen eines bestimmten Typs der Bildgröße verwenden müssen, erstellen Sie eine benannte Bildvorgabe, z. B. &quot;Miniaturansicht&quot;. Konfigurieren Sie dann die Bildvorgabe für die Miniaturansicht mit den entsprechenden Größe, dem Dateiformat und den Scharfzeichnungsoptionen. Rufen Sie das Bild mit dem Namen der Bildvorgabe auf. Bildvorgaben verkürzen die Länge der gesamten URL. Diese beiden URLs erzeugen dasselbe 350 x 350 JPEG-Bild mit Scharfzeichnung:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Bildvorgaben können jederzeit geändert und aktualisiert werden. Sie sehen die Ergebnisse einer Änderung an einer Bildvorgabe, nachdem Sie sie veröffentlicht haben und nachdem der Cache für die URL gelöscht wurde.

Wenn Sie für jedes Bild in einer Größenkategorie eine Vorgabe verwenden, kann jeder Unternehmensadministrator die Definition dieser Bildvorgabe aktualisieren. Sie können dann jedes Bild erneut veröffentlichen und mit diesem Format bearbeiten. Alle ohne Änderung eines Webcodes. Es empfiehlt sich, eine Bildvorgabe pro Größe auf Ihrer Site zu verwenden. Um eine Bildvorgabe hinzuzufügen, gehen Sie in der Leiste &quot;Globale Navigation&quot;zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Bildvorgaben]**. Wählen Sie dann **[!UICONTROL Hinzufügen]** oder **[!UICONTROL Bearbeiten]** aus, um eine vorhandene Vorgabe zu ändern. Das einzige erforderliche Feld ist der Name der Vorgabe. Es ist jedoch am besten, eine gewisse Scharfzeichnungsebene in jede Vorgabe aufzunehmen.

**JPG-Qualität**

Die Optionen für „JPG-Qualität“ bestimmen den JPG-Komprimierungsgrad:

* **JPG-Qualität**: Wählen Sie diese Option, wenn Sie die Komprimierungsstufen und das Chrominanz-Downsampling steuern möchten.

* **Regler**: Bestimmt die JPG-Komprimierungsstufe. Diese Einstellung wirkt sich sowohl auf die Dateigröße als auch die Bildqualität aus. Die JPG-Qualitätsskala reicht von 1 bis 100.

* **Aktivieren Sie JPG Chrominance Downsampling**: Da das Auge weniger empfindlich gegenüber hochfrequenten Farbinformationen ist als gegenüber hochfrequenter Luminanz, teilen JPEG-Bilder Bildinformationen in Luminanz und Farbkomponenten. Bei der Komprimierung eines JPEG-Bildes behält die Leuchtdichtekomponente die volle Auflösung, während für die Farbkomponenten ein Downsampling, d. h. eine Mittelwerterstellung für Pixelgruppen, ausgeführt wird. Durch Downsampling wird das Datenvolumen um die Hälfte oder ein Drittel reduziert, ohne dass sich dies auf die wahrgenommene Qualität auswirkt. Downsampling kann nicht auf Graustufenbilder angewendet werden. Mit dieser Technik wird der Komprimierungsgrad, der für Bilder mit hohem Kontrast (z. B. Bilder mit überlappendem Text) sinnvoll ist, reduziert.

**Festlegen unternehmensweiter Scharfzeichnungsoptionen**

Wenn Sie keine Bildvorgabe verwendet oder bestimmte Image Server-Scharfzeichnungsprotokolle entlang der URL-Zeichenfolge übergeben haben, tritt beim Downsampling keine Scharfzeichnung des Bildes auf. Tritt diese fehlende Scharfzeichnung jedoch auf, können Sie Standardwerte für die Scharfzeichnung festlegen, um sicherzustellen, dass jedes Bild immer eine gewisse Scharfzeichnung aufweist.

Um die standardmäßigen Scharfzeichnungsoptionen Ihres Unternehmens festzulegen, gehen Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Publish-Einrichtung]** > **[!UICONTROL Image-Server]**. Wenn Sie den standardmäßigen Resampling-Modus auf **`Sharp2`** festlegen, wird das Bild beim Downsampling immer scharfgezeichnet.

**Scharfzeichnen zu Viewer-Vorgaben hinzufügen**

Wenn Sie der Vorgabe keine Scharfzeichnungsbildmodifikatoren hinzugefügt haben, kann das kleine anfängliche Ladebild weich aussehen, da es heruntergesampelt wird, um es in das Viewer-Fenster zu passen, ohne scharfgezeichnet zu werden.

Mit Viewer-Vorgaben (wie Bildvorgaben) können Sie viele Optionen an einem Ort zentralisieren, einschließlich der Auswahl der Haut- und Viewer-Optionen (z. B. durch Eingabe einer Drucken-Schaltfläche oder Steuerung der Geschwindigkeit der Zoom-Animation). Viewer-Vorgaben befinden sich im selben Abschnitt wie Bildvorgaben unter **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Viewer-Vorgaben]**.

Siehe Schulungsvideo zu [Viewer-Vorgaben](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) .

Die Modifiziereroption befindet sich im Bereich „Core-Einstellungen“ aller E-Katalog-, Rotations- und benutzerdefinierter Zoom-Viewer-Vorgaben. Durch Hinzufügen der URL-Scharfzeichnungsbefehle zum Feld &quot;Modifikatoren&quot;fügen Sie die Scharfzeichnung jedes Mal hinzu, wenn dieser Viewer mit dieser Viewer-Vorgabe aufgerufen wird.

Verwenden Sie zum Aufrufen der Viewer-Vorgabe den Befehl `config=` in der Viewer-URL. Im Folgenden finden Sie ein Beispiel für den Aufruf eines Bildsets (Schuhe) mit einer Viewer-Vorgabe (`FantasticoZoom2022`):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

Diese Vorgabe schärft und ändert die Standardskin des Viewers.

**Erstellen bildspezifischer Überschreibungen**

Die letzte und am wenigsten empfohlene Scharfzeichnungsmethode besteht darin, Scharfzeichnungsabweichungen auf Bildbasis zu erstellen. Diese Methode überschreibt die Scharfzeichnung in einer Bildvorgabe mit ihren eigenen spezifischen Werten. Diese Methode überschreibt jedoch auch alle anderen Scharfzeichnungsmethoden bei beliebiger Größe. Der beste Anwendungsfall für diese Methode ist, wenn einige Ihrer Bilder nicht hochauflösend sind und die Werte in den Bildvorgaben für diese kleinen Bilder zu hoch sind. In diesem Fall ist möglicherweise eine gewisse Scharfzeichnung pro Bild erforderlich.

Wählen Sie in Adobe Dynamic Media Classic ein Bild aus, wechseln Sie zur Detailansicht (durch Doppelklicken oder Drücken der Schaltfläche **[!UICONTROL Detailansicht]** ) und wählen Sie **[!UICONTROL Scharfzeichnen]** aus. Ändern Sie einen beliebigen Parameter und wählen Sie dann **[!UICONTROL Speichern]** aus. Dieser Prozess weist den Image-Server an, diese Scharfzeichnungsparameter anstelle eines Befehls zu verwenden, den Sie in der URL aufrufen, z. B. einen Scharfzeichnungsmodifikator oder eine Bildvorgabe. Vergewissern Sie sich, dass Sie veröffentlichen, um zu sehen, dass die Änderungen wirksam werden.
