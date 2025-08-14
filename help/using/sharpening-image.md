---
title: Bilder scharfzeichnen
description: Erfahren Sie, wie Sie ein Bild in Adobe Dynamic Media Classic scharfzeichnen können.
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

Adobe Dynamic Media Classic empfiehlt dringend, Bildvorgaben für alle Bilder zu verwenden. Sie stellen eine einheitliche Größe sicher, und das Scharfzeichnen wird für jedes Bild erzwungen, das mit einer Bildvorgabe aufgerufen wird. Darüber hinaus können Sie die Scharfzeichnungsparameter einer Bildvorgabe einfach bearbeiten und ändern. Wenn Sie das nächste Mal eine Veröffentlichung vornehmen, erhalten alle Bilder, die mit dieser Vorgabe aufgerufen werden, die neuen Werte.

Adobe Dynamic Media Classic empfiehlt außerdem, den Viewer-Vorgaben Scharfzeichnung hinzuzufügen und dann einen Viewer mit dieser Vorgabe aufzurufen. Dadurch wird sichergestellt, dass die Bilder für Ihre Viewer gestochen scharf und ansprechend sind.

Unabhängig davon, ob Sie Bildvorgaben und Viewer-Vorgaben oder eine Methode zum Scharfzeichnen verwenden, müssen Sie Ihre Bilder letztlich scharfzeichnen. Andernfalls können Ihre Bilder (und die Website) weich und unscharf aussehen.

>[!NOTE]
>
>Mit dem Befehl „Scharfzeichnen“ werden die Einstellungen unter „Bildvorgaben“, einschließlich der dort angegebenen Scharfzeichnungseinstellungen, überschrieben. Eine Bildvorgabe legt die Größe und Formatierung fest, mit der Bilder von Dynamic Media-Bildservern bereitgestellt werden. Adobe Dynamic Media Classic empfiehlt dringend, Bildvorgaben zu verwenden, um alle Bilder bereitzustellen. So stellen Sie sicher, dass die Bilder eine einheitliche Größe aufweisen und scharfgezeichnet sind. Wenn jedoch die Scharfzeichnungseinstellungen für ein einzelnes Bild geändert wurden, gelten die Scharfzeichnungseinstellungen der Bildvorgabe nicht mehr für dieses Bild. Es wird dann ohne Anwendung der Scharfzeichnungseinstellungen der Bildvorgabe gesendet.

Es ist oft notwendig, Bilder scharfzuzeichnen. Adobe Dynamic Media Classic- und Bild-Server bieten mehrere Scharfzeichnungsoptionen. Es ist wichtig zu wissen, was das Scharfzeichnen bei einem Bild bewirkt und wie viel Scharfzeichnung Sie benötigen. Die meisten Bilder müssen etwas scharfgezeichnet werden, aber der Grad der Scharfzeichnung hängt vom Bild ab.

Die Bildschärfung erhöht den Kontrast der Pixel, um den Eindruck zu erwecken, dass die Kanten akzentuiert sind. Menschen nehmen diesen erhöhten Kantenkontrast als Schärfe wahr. Obwohl es einfach ist, ein Bild mithilfe von Scharfzeichnungsfiltern zu verbessern, ist es auch einfach, ein Bild zu stark scharfzuzeichnen.

Das übermäßige Scharfzeichnen eines Bildes erzeugt einen Haloeffekt, d. h. eine Streifenbildung der Kantenlinien.

Es gibt Best Practices, die Sie befolgen können, um das Scharfzeichnen Ihrer Bilder in Adobe Dynamic Media Classic und auf dem Dynamic Media-Bildserver zu optimieren.

Siehe [Best Practices für das Scharfzeichnen von Bildern in Adobe Dynamic Media Classic und auf Dynamic Media Image Server](/help/using/assets/s7_sharpening_images.pdf).

Siehe auch [Scharfzeichnen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) Schulungsvideo.

**So schärfen Sie ein Bild:**

Um ein Bild scharfzuzeichnen, klicken Sie auf die entsprechende **[!UICONTROL Bearbeiten]**-Schaltfläche und wählen **[!UICONTROL Scharfzeichnen]** oder öffnen Sie es im Durchsuchen-Bedienfeld in der Detailansicht und klicken Sie dann auf **[!UICONTROL Scharfzeichnen]**. Die Seite mit dem Scharfzeichnungseditor wird mit Scharfzeichnungsbefehlen geöffnet. Wählen Sie die gewünschten Befehle aus und klicken Sie dann auf **[!UICONTROL Speichern]**.

>[!NOTE]
>
>Bevor Sie ein Bild scharfzeichnen, können Sie im Menü „Vorgabe anwenden“ eine Bildvorgabe auswählen, um deren Effekte für die Scharfzeichnung des Bilds zu sehen. Die Scharfzeichnungseffekte einer Bildvorgabe sind für Ihr Bild geeignet. Das **[!UICONTROL Vorgabe anwenden]** befindet sich unten auf der Seite mit dem Schärfeeditor.

**Scharfzeichnungsoptionen**

Die folgende Tabelle zeigt die Scharfzeichnungsoptionen des Image-Servers.

| Name | URL-Protokoll | Werte | Beispiel |
| --- | --- | --- | --- |
| Einfaches Scharfzeichnen | `op_sharpen` | `0` oder `1` | `op_sharpen=1` |
| Resamplingmodus | `resMode` | `bilin`, `bicub`, `sharp2`, `trilin`<br><br>`bilin`: Wählt die standardmäßige bilineare Interpolation aus. Schnellste Resampling-Methode; einige Aliasing-Artefakte sind häufig auffällig.<br>`bicub`: Wählt die bikubische Interpolation. CPU-intensiver als `bilin`, liefert jedoch schärfere Bilder mit weniger auffälligen Alias-Artefakten.<br><br>`sharp2`: Wählt eine modifizierte Lanczos Windows®-Funktion als Interpolationsalgorithmus aus. Es kann zu einem höheren CPU-Preis etwas schärfere Ergebnisse als bikubisch erzielen.<br><br>`trilin`: Wählt eine modifizierte trilineare Interpolation aus, bei der, sofern verfügbar, sowohl höhere als auch niedrigere Auflösungen verwendet werden. Wird nur bei Problemen mit dem Aliasing empfohlen. Reduziert JPEG-Größen aufgrund der reduzierten Hochfrequenzdaten. | `resMode=sharp2` |
| Unschärfemaske | `op_usm` | `amount`, `radius`, `threshold`, `monochrome`<br><br>`amount`: Filterstärkefaktor (real 0…5)<br><br>`radius`: Filterkernradius in Pixel (real 0…250) <br><br>`threshold`: Filterschwellenwert (int 0…255)<br><br>`monochrome`: `0` auf Unschärfemaske setzen, um jede Farbkomponente separat zu maskieren, `1` auf Unschärfemaske Bildhelligkeit (Intensität) setzen | `op_usm=1,1,10,0` |

Wählen Sie das **[!UICONTROL Scharfzeichnen]** und wählen Sie eine Option aus:

* **None**: Deaktiviert das Scharfzeichnen.

* **Scharfzeichnen**: Führt einen einfachen Scharfzeichnungsvorgang für die Datei aus, nachdem deren Größe geändert wurde. Es ähnelt dem Filter „Scharfzeichnen“ in Adobe Photoshop und unterstützt keine Benutzerparameter. Normalerweise würden Sie diesen Filter oder **[!UICONTROL Unschärfemaske]** verwenden, aber nicht beides. Diese Methode wird nicht als Best Practice empfohlen, sie kann aber verschwommene Bilder kompensieren. (URL: `op_sharpen`)

* **Unschärfemaske**: Hiermit können Sie einen Scharfzeichnungsfiltereffekt für das endgültige Bild nach dem Downsampling optimieren. Sie können die Intensität des Effekts, den Radius des Effekts (gemessen in Pixel) und einen Schwellenwert für den ignorierten Kontrast steuern. Dieser Effekt verwendet dieselben Optionen wie der Photoshop-Filter „Unscharf maskieren“. (URL: `op_usm`)

Wählen Sie diese Optionen aus, um das Scharfzeichnen mit Unschärfemaske anzupassen:

* **Stärke**: Steuert den auf die Kanten-Pixel angewendeten Kontrastwert. Der Standardwert ist 0,0. Für Bilder mit höherer Auflösung können Sie ihn auf bis zu 5,0 erhöhen. Sie können sich die Auswirkung der Option „Betrag“ wie ein Maß für die Filterintensität vorstellen. Die **[!UICONTROL Betrag]** in Adobe Dynamic Media Classic ist nicht identisch mit der Einstellung Betrag in Adobe Photoshop. Adobe Photoshop verwendet einen Wert zwischen 1 % und 500 %, während Adobe Dynamic Media Classic von 0,0 auf 5,0 skaliert werden kann. (5,0 entspricht ungefähr 500 % in Photoshop, 0,9 ungefähr 90 % usw.)

* **Radius**: Bestimmt die Anzahl der Pixel um die Kanten-Pixel, auf die sich die Scharfzeichnung auswirkt. Der Effekt wird auf allen Pixeln im Bild ausgeführt und strahlt in alle Richtungen aus. 

Der beste Radiuswert hängt von der Größe des Bilds ab. Bei einem geringeren Wert werden nur die Kantenpixel scharfgezeichnet, während bei einem hohen Wert ein breiterer Pixelbereich scharfgezeichnet wird.

Um beispielsweise einen ähnlichen Scharfzeichnungseffekt für ein Bild mit 2000 × 2000 Pixel und ein Bild mit 500 × 500 Pixel zu erhalten, können Sie einen Radius-Wert von zwei Pixel auf dem Bild mit 2000 × 2000 Pixel festlegen. Legen Sie dann einen Radius-Wert von einem Pixel auf dem Bild mit 500 × 500 Pixel fest (ein größerer Wert für ein Bild mit mehr Pixel).

* **Schwellenwert**: Bestimmt den Kontrastbereich, der beim Anwenden der Unschärfemaske ignoriert werden soll. Diese Option bestimmt, wie stark sich die scharfgezeichneten Pixel vom Umgebungsbereich unterscheiden müssen, damit die Kantenpixel scharfgezeichnet werden.

Der Schwellenwert verwendet einen Wert zwischen 0 und 255, also die Anzahl der Helligkeitsschritte in einem Graustufenbild. 0=schwarz, 128=50 % grau und 255=weiß. Bei einem Schwellenwert von 12 werden beispielsweise geringfügige Abweichungen in der Helligkeit des Hauttons ignoriert. Dabei wird kein Rauschen hinzugefügt, während gleichzeitig der Kantenkontrast in kontrastreichen Bereichen hinzugefügt wird, z. B. wo Wimpern auf die Haut treffen.

Nehmen wir als Beispiel an, Sie haben ein Foto von jemandes Gesicht. wirkt sich „Unscharf maskieren“ auf die Teile des Bildes mit dem höchsten Kontrast und der glattesten Haut aus. Selbst die glatteste Haut weist subtile Änderungen in Helligkeitswerten auf. Wenn Sie keinen Schwellenwert verwenden, akzentuiert der Filter diese subtilen Änderungen in den Hautpixeln und erzeugt einen Rauscheffekt (der wahrscheinlich unerwünscht ist), während er gleichzeitig den Kontrast an den Wimpern erhöht und somit die Schärfe verbessert (wahrscheinlich wünschenswert). Um dieses Problem zu vermeiden, verwenden Sie einen Schwellenwert, bei dem der Filter Pixel ignoriert, die den Kontrast nicht drastisch ändern, wie z. B. glatte Haut. Um Rauschen oder Posterisierungen in Bildern mit Fleischtönen zu vermeiden, experimentieren Sie beispielsweise mit **[!UICONTROL Schwellenwert]** Werten 2 bis 20. Der Standardwert **[!UICONTROL Schwellenwert]** von 0 schärft alle Pixel im Bild.

* **Anwenden auf**: Wählen Sie **[!UICONTROL Jede Farbe]**, wenn Sie das Scharfzeichnen separat auf jede Farbkomponente anwenden möchten; wählen Sie **[!UICONTROL Helligkeit]**, wenn Sie das Scharfzeichnen auf Bildhelligkeitsbereiche anwenden möchten.

**Resampling**

Wählen Sie das **[!UICONTROL Resampling]**-Menü und dann eine Option aus. Mit diesen Optionen wird ein Bild beim Downsampling scharfgezeichnet:

* **[!UICONTROL None]**: Deaktiviert das Resampling.

* **[!UICONTROL Bilinear]**: Die schnellste Resampling-Methode. Einige Aliasing-Artefakte sind auffällig.

* **[!UICONTROL Bicubic]**: Erhöht die CPU-Nutzung auf dem Bildserver, liefert jedoch schärfere Bilder mit weniger auffälligen Alias-Artefakten.

* **[!UICONTROL `Sharpen 2`]**: Erzeugt etwas schärfere Ergebnisse als **[!UICONTROL Bikubisch]**, aber zu noch höheren CPU-Kosten auf dem Bildserver.

* **[!UICONTROL Trilinear]**: Verwendet sowohl höhere als auch niedrigere Auflösungen, falls verfügbar; nur empfohlen, wenn der Alias ein Problem darstellt. Bei dieser Methode wird die JPEG-Dateigröße durch Reduzierung der Hochfrequenzdaten verringert.

**Bildvorgaben und Scharfzeichnen**

Sie können alle drei Scharfzeichnungseffekte einbeziehen, um das Endergebnis zu erzielen. Diese Methode wird jedoch nicht empfohlen. Adobe Dynamic Media Classic empfiehlt, Scharfzeichnungseffekte als Teil einer Bildvorgabe zu speichern. Mit Bildvorgaben können Sie die am häufigsten verwendeten Bildmodifikatoren verpacken, um ein Bild mit dynamischer Größe in einer kleinen Textzeichenfolge zu erstellen. Eine Bildvorgabe enthält Werte für das Dateiformat (normalerweise JPEG für das Web), die Pixelanzahl und das Scharfzeichnen von Bildern. Anstatt die URL an jeden Bildmodifikator anzuhängen, den Sie verwenden müssen, um einen bestimmten Typ von Bildgröße zu erstellen, erstellen Sie eine Bildvorgabe mit dem Namen „Miniatur“. Konfigurieren Sie dann die Bildvorgabe für die Miniaturansicht mit den entsprechenden Optionen für Größe, Dateiformat und Scharfzeichnung. Rufen Sie das Bild mit dem Namen der Bildvorgabe auf. Bildvorgaben verkürzen die Länge der gesamten URL. Diese beiden URLs erzeugen dasselbe 350 x 350-Grad-JPEG-Bild mit Scharfzeichnung:

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

Bildvorgaben können jederzeit geändert und aktualisiert werden. Sie sehen die Ergebnisse einer Änderung an einer Bildvorgabe nach der Veröffentlichung und nachdem der Cache für die URL gelöscht wurde.

Wenn Sie eine Vorgabe für jedes Bild in einer Größenkategorie verwenden, kann jeder Unternehmensadministrator die Definition dieser Bildvorgabe aktualisieren. Sie können dann Bilder in diesem Format erneut veröffentlichen und sich auf alle Bilder auswirken. Alles, ohne den Web-Code zu ändern. Es empfiehlt sich, eine Bildvorgabe pro Größe auf Ihrer Site zu verwenden. Um eine Bildvorgabe hinzuzufügen, klicken Sie in der globalen Navigationsleiste auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Bildvorgaben]**. Klicken Sie dann auf **[!UICONTROL Hinzufügen]** oder auf **[!UICONTROL Bearbeiten]**, um eine vorhandene Vorgabe zu ändern. Das einzige erforderliche Feld ist der Name der Vorgabe. Es ist jedoch am besten, in jeder Vorgabe einen bestimmten Scharfzeichnungsgrad einzufügen.

**JPG-Qualität**

Die Optionen für „JPG-Qualität“ bestimmen den JPG-Komprimierungsgrad:

* **JPG-Qualität**: Wählen Sie diese Option aus, wenn Sie Komprimierungsgrade und Neuberechnung der Chrominanz steuern möchten.

* **Regler**: Legt den JPG-Komprimierungsgrad fest. Diese Einstellung wirkt sich sowohl auf die Dateigröße als auch die Bildqualität aus. Die JPG-Qualitätsskala reicht von 1 bis 100.

* **JPG-Neuberechnung der Chrominanz aktivieren**: Da das Auge weniger empfindlich auf hochfrequente Farbinformationen reagiert als hochfrequente Luminanz, unterteilen JPEG-Bilder Bildinformationen in Luminanz- und Farbkomponenten. Bei der Komprimierung eines JPEG-Bildes behält die Leuchtdichtekomponente die volle Auflösung, während für die Farbkomponenten ein Downsampling, d. h. eine Mittelwerterstellung für Pixelgruppen, ausgeführt wird. Durch Downsampling wird das Datenvolumen um die Hälfte oder ein Drittel reduziert, ohne dass es zu Qualitätseinbußen kommt. Downsampling kann nicht auf Graustufenbilder angewendet werden. Mit dieser Technik wird der Komprimierungsgrad, der für Bilder mit hohem Kontrast (z. B. Bilder mit überlappendem Text) sinnvoll ist, reduziert.

**Legen Sie unternehmensweite Scharfzeichnungsoptionen fest**

Wenn Sie keine Bildvorgabe verwendet oder bestimmte Scharfzeichnungsprotokolle für Bild-Server entlang der URL-Zeichenfolge übergeben haben, wird das Bild beim Downsampling nicht scharf gemacht. Wenn jedoch diese mangelnde Scharfzeichnung auftritt, können Sie standardmäßige Scharfzeichnungswerte festlegen, um sicherzustellen, dass jedes Bild immer etwas Scharfzeichnung aufweist.

Die standardmäßigen Scharfzeichnungsoptionen für Ihr Unternehmen finden Sie unter **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Veröffentlichungseinstellungen]** > **[!UICONTROL Image-Server]**. Wenn Sie den standardmäßigen Resampling-Modus auf **`Sharp2`** setzen, wird das Bild beim Downsampling immer scharfgezeichnet.

**Scharfzeichnung zu Viewer-Vorgaben hinzufügen**

Wenn Sie der Vorgabe keine Bildmodifikatoren für das Scharfzeichnen hinzugefügt haben, kann das kleine Bild beim ersten Laden weich aussehen, da es heruntergesampelt ist, damit es in das Viewer-Fenster passt, ohne scharfgezeichnet zu werden.

Mit Viewer-Vorgaben (wie Bildvorgaben) können Sie viele Optionen an einer Stelle zentralisieren, einschließlich der Auswahl von Skin- und Viewer-Optionen (z. B. mit einer Druckschaltfläche oder Steuerung der Geschwindigkeit der Zoom-Animation). Viewer-Vorgaben befinden sich im selben Abschnitt wie Bildvorgaben unter **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Viewer-Vorgaben]**.

Siehe [Viewer-Vorgaben](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) Schulungsvideo.

Die Modifiziereroption befindet sich im Bereich „Core-Einstellungen“ aller E-Katalog-, Rotations- und benutzerdefinierter Zoom-Viewer-Vorgaben. Durch Hinzufügen der URL-Scharfzeichnungsbefehle zum Feld Modifikatoren fügen Sie jedes Mal eine Scharfzeichnung hinzu, wenn dieser Viewer mit dieser Viewer-Vorgabe aufgerufen wird.

Um die Viewer-Vorgabe aufzurufen, verwenden Sie den Befehl `config=` auf der Viewer-URL. Im Folgenden finden Sie ein Beispiel für den Aufruf eines Bildsets (Schuhe) mit einer Viewer-Vorgabe (`FantasticoZoom2022`):

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

Diese Vorgabe schärft und ändert die Standardskin des Viewers.

**Erstellen von bildspezifischen Überschreibungen**

Die letzte und am wenigsten empfohlene Scharfzeichnungsmethode besteht darin, Scharfzeichnungsabweichungen auf Bildbasis zu erstellen. Diese Methode überschreibt die Scharfzeichnung in einer Bildvorgabe mit eigenen spezifischen Werten. Diese Methode überschreibt jedoch auch alle anderen Scharfzeichnungsmethoden beliebiger Größe. Der beste Anwendungsfall für diese Methode ist, wenn einige Ihrer Bilder nicht hochauflösend sind und die Werte in den Bildvorgaben für diese kleinen Bilder zu hoch sind. In diesem Fall ist möglicherweise eine Scharfzeichnung pro Bild erforderlich.

Wählen Sie in Adobe Dynamic Media Classic ein Bild aus, wechseln Sie zur Detailansicht (durch Doppelklicken oder Drücken der **[!UICONTROL Detailansicht]**) und wählen Sie **[!UICONTROL Scharfzeichnen]**. Ändern Sie beliebige Parameter und klicken Sie dann auf **[!UICONTROL Speichern]**. Dadurch weiß der Bild-Server, dass diese Scharfzeichnungsparameter anstelle der in der URL angegebenen Befehle verwendet werden sollen (z. B. Scharfzeichnungsmodifikator oder Bildvorgabe). Stellen Sie sicher, dass Sie veröffentlichen, um zu sehen, dass die Änderungen wirksam werden.
