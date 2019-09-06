---
title: Erstellen von Imagemaps
seo-title: Erstellen von Imagemaps
description: 'null'
seo-description: Erfahren Sie, wie Sie Imagemaps erstellen.
uuid: 0 dcc 4956-006 e -4 a 74-9 d 6 a -6 d 4 bb 23790 ce
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/master_ files
discoiquuid: 4 eddf 883-38 cb -4 f 00-b 3 be -85 c 20 bdd 6 f 69
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Erstellen von Imagemaps{#creating-image-maps}

Eine Imagemap ist ein Bereich auf einem Bild oder einer E-Katalog-Seite oder ein Bild in einem Rotationsset, mit dessen Hilfe ein Bedienfeld mit Rollover-Text angezeigt werden kann. Wenn der Benutzer auf eine Imagemap klickt, wird eine bestimmte Aktion ausgelöst. Beispielsweise kann eine Website aufgerufen werden, auf der der Benutzer mehr über ein Produkt erfährt. Um auf die Imagemaps auf Bildern aufmerksam zu machen, wird die Imagemap umrahmt angezeigt, wenn der Benutzer den Mauszeiger darüber bewegt.

Sie können auch eine Imagemap in Dynamic Media Classic erstellen oder Imagemaps erstellen, wenn Sie einen Katalog in Adobe Acrobat oder Adobe indesign entwerfen.

Beim Erstellen von Imagemaps haben Sie die folgenden Möglichkeiten:

* Rollover-Text eingeben
* JavaScript und URLs zum Starten von Websites eingeben
* URL-Vorlagen für Imagemaps erstellen
* Imagemaps in andere Bilder, E-Katalogseiten oder Rotationssets kopieren
* Imagemaps in CSV- oder XML-Dateien exportieren
* Bildmetadaten aus einer tabulatorgetrennten Datei oder einer XML-Datei importieren
* Andere vom W3C (World Wide Web Consortium) festgelegte Aktionen definieren
* Vorschau der Imagemaps anzeigen

## Zeichnen und Anpassen einer Imagemap {#drawing-and-adjusting-an-image-map}

1. Führen Sie einen der folgenden Schritte aus:

   * If you are working with an image in the Grid View or List View, in the Edit drop-down list click **Image Map**. Or, open it in Detail View, and then click **Image Map** above the image.
   * If you are working with a SpinSet in the Grid View or List View, click **Edit**. Or, open it in Detail View, and then click **Edit**. Select an image asset, and then click **Image Map**.
   * If you are working with an eCatalog, in the Grid View, List View, Detail View, click **Edit**. Click the **Map Pages** tab.
   ![](assets/ma_image_map.png)

1. Sie können eine rechteckige oder polygonale Imagemap zeichnen:

   **Rechteckige Karte** Wählen Sie das Rechteck-Imagemap-Werkzeug aus und ziehen Sie auf die Seite, um das Rechteck zu erstellen. Um einen Punkt zu einer rechteckigen Map hinzuzufügen (und sie so in eine polygonale verweissensitive Grafik zu ändern), drücken Sie die Strg-Taste, platzieren Sie das Einfügen-Werkzeug an der gewünschten Position und klicken Sie.

   **Polygonale Karte** Wählen Sie das Polygon-Imagemap-Werkzeug aus und klicken Sie auf die Punkte am Umfang des Bildbereichs, den Sie anhängen möchten. Verwenden Sie den Regler für die Dichte des Polygons, um die Punktdichte im Polygon zu ändern. Die ursprüngliche Dichte wird wiederhergestellt, wenn Sie andere Maps auswählen. Wenn ein Punkt im Polygon hinzugefügt, gelöscht oder verschoben wird, wird die ursprüngliche Dichte verworfen und der Regler auf den Maximalwert zurückgesetzt.

1. Geben Sie optional in der Imagemap-Liste einen Namen für die Imagemap ein. Nachdem Sie eine Imagemap gezeichnet haben, weist Dynamic Media Classic diesen Namen zu.

   Um den Namen zu erstellen, hängt Dynamisches Media Classic eine sequenzielle Nummer an den Namen des Bilds oder der E-Katalogseite an, mit dem Sie arbeiten. Sie können jedoch auch einen Namen Ihrer Wahl eingeben.

1. Wenn die Benutzer durch Klicken auf die Imagemap eine neue Website öffnen können sollen, geben Sie in der Imagemap-Liste die entsprechende URL ein. 

   Siehe [Eingeben von JavaScript und URLs](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Wenn Rollover-Text angezeigt werden soll, sobald die Benutzer den Mauszeiger über die Imagemap bewegen, geben Sie den Text in der Imagemap-Liste ein. Wählen Sie im Menü „Anzeigen“ der Imagemap-Liste die Option „Rollover-Text“. Geben Sie anschließend den Text ein, der für die Benutzer auf dem Bildschirm angezeigt werden soll. Sie können den Text in einem Textverarbeitungsprogramm schreiben und in das Feld „Rollover-Text“ kopieren.
1. Sie können auch eine andere Aktion definieren, die ausgeführt werden soll, wenn die Benutzer den Mauszeiger über die Imagemap bewegen. Klicken Sie in der Dropdown-Liste „Anzeigen“ auf „Andere Aktionen“. Geben Sie die Attribute der Aktion ein. (Klicken Sie auf „Anzeigen“ &gt; „Beide“, um den Rollover-Text und eine Aktion für eine Imagemap zu erstellen.)

   Siehe [Definieren anderer Aktionen für Imagemaps](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Optional) Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf „Vorschau“, um Imagemaps in der Vorschau anzuzeigen.
   * Um eine Imagemap oder einen Polygonscheitelpunkt zu löschen, wählen Sie die Form auf dem Bild aus und klicken Sie auf „Löschen“. Oder klicken Sie bei einem E-Katalog in der Registerkarte „Seiten ordnen“ auf „Maps löschen“, um Imagemaps aus allen Seiten zu entfernen.
   * Um eine Imagemap vorübergehend von einem Bild, einer E-Katalogseite oder einem Bild in einem Rotationsset zu entfernen, ohne sie zu löschen, deaktivieren Sie in der Imagemap-Liste die entsprechende Option „Ein“.

1. Klicken Sie auf „Speichern“.

### Anpassen der Position, Form und Größe von Imagemaps {#adjusting-the-position-shape-and-size-of-image-maps}

Um die Position, Form und Größe einer Imagemap zu ändern, klicken Sie auf „Imagemap“ . Wählen Sie anschließend das Schwenken-Werkzeug aus und befolgen Sie die folgenden Anweisungen:

**Ändern der Position** : Bewegen Sie den Mauszeiger nahe an den Rand der Imagemap. Wenn der Mauszeiger als Vierfachpfeil dargestellt wird, ziehen Sie die Imagemap an eine andere Position.

**Größe und Form ändern** Wie Sie die Form und Größe einer Imagemap ändern, hängt davon ab, ob Sie mit einer rechteckigen oder polygonalen Imagemap arbeiten:

***Tipp**: Sie können den Schieberegler "Größe" unten im Bildschirm ziehen, um die Ansichten zu ändern und die Imagemap besser zu betrachten.*

**Rechteckige Imagemaps** Bewegen den Mauszeiger über eine Seite oder Ecke der Imagemap. Wenn der Mauszeiger als Doppelpfeil dargestellt wird, ziehen Sie mit der Maus. Halten Sie beim Ziehen die Umschalttaste gedrückt, um die Größe zu ändern, dabei jedoch das Seitenverhältnis (die Form) beizubehalten.

**Polygonale Imagemap** Ziehen Sie einen quadratischen Auswahlziehpunkt. Um einen Auswahlziehpunkt zu erstellen, klicken Sie auf den Rand der Imagemap und beginnen Sie zu ziehen.

### Beheben von überlappenden Imagemaps {#handling-overlapping-image-maps}

Wenn das Bild oder die E-Katalogseite mehrere Imagemaps enthält, die sich überschneiden, können Sie Einstellungen für die Überschneidung festlegen. Ändern Sie dazu in der Imagemap-Liste die Reihenfolge der Imagemaps. Ziehen Sie die Namen zu einer höheren oder niedrigeren Position in der Liste. Die Imagemaps an höheren Positionen überlagern die Imagemaps an niedrigeren Positionen in der Liste.

### Importieren von Imagemap-Daten {#importing-image-map-data}

Anstatt auf jeder Seite Imagemap-Daten einzugeben, können Sie auch die Daten für das Bild, das Rotationsset oder den E-Katalog in den Anzeigebereich mit der Imagemap-Zusammenfassung importieren. Die Imagemap-Daten werden in Form einer tabulatorgetrennten oder XML DTD-Datei importiert. Die Felder in der Datei müssen dieselbe Reihenfolge haben, wie im Anzeigebereich mit der Imagemap-Zusammenfassung dargestellt: „Name“, „Inhaltsverz.“, „Imagemaps“, „URLs“, „Rollover-Text“, „Andere Aktionen“ und „Suchzeichenfolgen“. Indem Sie Imagemap-Daten importieren, können Sie sich die Arbeit beim Eingeben der Daten in der Imagemap-Liste zum Erstellen der einzelnen Imagemaps sparen.

**So importieren Sie Imagemap-Daten**

1. Gehen Sie zur Seite „Imagemap-Editor“ (für Bilder oder Bilder in Rotationssets) oder zur Registerkarte „Imagemap-Seiten“ im Bearbeitungsbildschirm für E-Kataloge.
1. Klicken Sie auf „Metadaten importieren“.
1. Klicken Sie im Dialogfeld „Metadaten hochladen“ auf „Bild“ oder „Imagemap“, um die Metadaten des gewünschten Asset-Eigenschaftstyps hochzuladen.
1. Wählen Sie In der Dropdown-Liste „Datei erstellen“ die Datei aus, die Sie erstellen möchten.
1. (Optional) Klicken Sie auf „Erstellen“, um die erzeugten Daten abhängig von dem von ihnen gewünschten Dateityp in der Vorschau anzuzeigen. Klicken Sie auf „Schließen“, um zum Dialogfeld „Metadaten hochladen“ zurückzukehren.
1. Navigieren Sie zu der Datei, die Sie hochladen möchten. Geben Sie im Textfeld „Dateiname“ den Namen der erstellten Datei an.
1. (Optional) Geben Sie im Feld „Auftragsname“ einen Namen für den Auftrag „Metadaten hochladen“ ein.
1. Klicken Sie auf „Hochladen“.

### Kopieren von Imagemaps {#copying-image-maps}

Sie können Imagemaps zwischen Bildern und E-Katalogseiten kopieren. Kopieren Sie Imagemaps, um sie als Vorlage zum Erstellen anderer Imagemaps zu verwenden. Sie können Imagemaps auch kopieren, um sie auf Bildern oder Seiten mit demselben Layout oder derselben Imagemap-Struktur erneut zu verwenden.

Das Kopieren von Imagemaps in einem E-Katalog ist zum Beispiel eine praktische Möglichkeit, alle Imagemaps in die unterschiedlichen Sprachversionen des gleichen E-Katalogs zu kopieren. Um ein optimales Ergebnis zu erzielen, sollten Sie nach Möglichkeit zwischen E-Katalogen mit derselben Seitenanzahl und den gleichen Bildern kopieren. Falls der E-Katalog, in den Sie Imagemaps kopieren, bereits Imagemaps enthält, werden diese beim Kopiervorgang gelöscht.

**So kopieren Sie Imagemaps**

1. Gehen Sie zur Seite „Imagemap-Editor“ (für Bilder oder Bilder in Rotationssets) oder zur Registerkarte „Imagemap-Seiten“ im Bearbeitungsbildschirm für E-Kataloge.
1. Klicken Sie auf „Imagemaps kopieren zu“.
1. Führen Sie, abhängig davon, ob Sie Imagemaps aus Bildern oder Imagemaps aus einem E-Katalog kopieren möchten, einen der folgenden Schritte aus:

   * (Bilder) Wählen Sie im Bildschirm „Bilder auswählen“ die Bilder aus, die Sie in die Imagemaps kopieren möchten.
   * (E-Katalog) Wählen Sie im Bildschirm „Asset auswählen“ die Bilder oder E-Katalogseiten aus, die Sie in die Imagemaps kopieren möchten.

1. Klicken Sie auf „Auswählen“.

## Eingeben von JavaScript-Code und URLs unter Verwendung einer Vorlage {#using-a-template-to-enter-javascript-and-urls}

Sie können eine URL-Vorlage (auch Href-Vorlage genannt) definieren, um das Eingeben von Imagemap-URLs einfacher und effizienter zu machen. Es ist sinnvoll, eine URL-Vorlage zu definieren, wenn die meisten Ihrer Imagemap-URLs ein gemeinsames festes Format haben. Wenn Sie den gleich bleibenden Teil der URL als Vorlage definieren, brauchen Sie diesen Teil beim Erstellen einer neuen Imagemap-URL nicht jedes Mal erneut einzugeben. Eine URL-Vorlage kann auch JavaScript-Befehle, Pfadnamen und Parameter enthalten. By default, the URL template contains a proprietary Dynamic Media Classic JavaScript handler called `loadProduct` that opens the image in a new window.

>[!NOTE]
>
>Beachten Sie, dass JavaScript-Code, den Sie dem HREF-Attribut Ihrer Imagemap hinzufügen, auf dem Clientcomputer ausgeführt wird. Stellen Sie daher sicher, dass der JavaScript-Code sicher ist.

### URL-Vorlagen {#about-url-templates}

Eine URL-Vorlage funktioniert so, dass der Inhalt der Spalte „URL“ in der Imagemap-Liste durch ein doppeltes Dollarzeichen (‘$$’) in der Vorlage ersetzt wird: 

```as3
Javascript:loadProduct(‘$$’);void(0);
```

Fügen Sie alle Werte, die sich nicht bei jeder Imagemap ändern, in die URL-Vorlage ein. Fügen Sie anschließend nur die Werte hinzu, die sich in der Spalte „URL“ der Imagemap-Liste ändern. Beispiel:

* URL-Vorlage: j `avascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* URL-Wert: `product.htm`
* Tatsächliche URL generiert: `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

By default, the URL template includes a proprietary Dynamic Media Classic JavaScript handler called `loadProduct` that opens a new window with the URL destination. Sie können diesen javascript-Handler jedoch mit beliebigen javascript-Code ersetzen oder einen der folgenden dynamischen Media Classic-Handler verwenden:

* `loadProductCW`

   Zeigt das URL-Ziel an, das in der Spalte „URL“ des aktuellen Fensters angegeben ist. Dieser Handler ist hauptsächlich für E-Kataloge vorgesehen, die in eine Seite innerhalb einer Website integriert sind.

* `loadProductPW`

   Zeigt das URL-Ziel an, das in der Spalte „URL“ des übergeordneten Fensters (d. h. der Seite, über die die aktuelle Seite geöffnet wurde) angegeben ist. Das aktuelle Fenster bleibt geöffnet, während im übergeordneten Fenster das URL-Ziel angezeigt wird.

   ***Hinweis**: Der Handler`loadProductPW`unterstützt keine DHTML- und HTML 5-Viewer.*

### Erstellen einer URL-Vorlage {#creating-a-url-template}

So erstellen Sie eine URL-Vorlage:

1. Klicken Sie im Anzeigebereich „Map-Editor“ (bei Bildern oder Rotationssets) bzw. auf der Registerkarte „Imagemap-Seiten“ des Anzeigebereichs „E-Katalog“ (bei E-Katalogseiten) neben der Option „URL-Vorlage“ auf „Bearbeiten“. Das Dialogfeld „Verweisvorlage bearbeiten“ wird geöffnet.
1. Enter the JavaScript code and the complete URL (with the variable portion replaced by dollar signs [$$]). Sie können den Code einfügen, indem Sie mit der rechten Maustaste klicken und „Einfügen“ wählen.
1. Klicken Sie auf „Speichern“.

### Arbeiten mit URL-Vorlagen {#handling-url-templates}

Auf der Seite „Map-Editor“ (bei Bildern und Rotationssets) bzw. der Registerkarte „Imagemap-Seiten“ des Anzeigebereichs „E-Katalog“ (bei E-Katalogseiten) stehen folgende Befehle zum Einstellen von URL-Vorlagen zur Verfügung:

**Option "URL-Vorlage** " Wählen Sie die Option" URL-Vorlage" , um Ihre URL-Vorlage auf alle Imagemaps auf einem Bild oder einer E-Katalogseite anzuwenden.

**Vorlage** deaktivieren Sie die Option "Vorlage deaktivieren" in der URL-Imagemap-Liste, wenn Sie nicht möchten, dass eine einzelne Imagemap die URL-Vorlage verwendet.

## Festlegen anderer Aktionen für Imagemaps {#defining-other-actions-for-image-maps}

Sie können im Menü „Anzeigen“ die Option „Andere Aktionen“ wählen, um andere Aktionen als die Anzeige von Rollover-Text und den Aufruf von Websites auszulösen. Wenn der Benutzer den Mauszeiger über eine Imagemap bewegt, kann die Aktion ausgelöst werden. Diese Aktionen sind Attribute, die mithilfe der HTML-Spezifikationen des W3C (World Wide Web Consortium) für clientseitige Imagemaps definiert werden. Diese umfassen Folgende:

**accesskey** Löst eine Aktion aus, wenn der Benutzer einen bestimmten Schlüssel auf der Tastatur drückt.

**onfocus** Löst ein Ereignis aus, wenn die Imagemap den Fokus erhält - durch den Cursor, durch Tabulatortaste oder durch Drücken einer Zugriffstaste. Sie können beispielsweise eine Website aufrufen, wenn die Imagemap den Fokus erhält, und sie wieder schließen, wenn die Imagemap den Fokus wieder verliert.

**onblur** Löst ein Ereignis aus, wenn die Imagemap den Fokus verliert, entweder durch den Cursor oder durch Drücken der Tabulatortaste.

**So definieren Sie weitere Aktionen für Imagemaps**

1. Öffnen Sie im Anzeigebereich „Map-Editor“ (bei Bildern und Rotationssets) bzw. auf der Registerkarte „Imagemap-Seiten“ des Anzeigebereichs „E-Katalog“ (bei E-Katalogseiten) das Menü „Anzeigen“ und wählen Sie die Option „Andere Aktionen“.
1. Fügen Sie unter Verwendung der vom W3C-Konsortium spezifizierten Syntax in der Spalte „Andere Aktionen“ der Imagemap-Liste die unterstützten Attribute ein.
1. Klicken Sie auf „**Speichern**“.

Wählen Sie im Menü „Anzeigen“ die Option „Beide“, wenn für eine Imagemap sowohl Rollover-Text angezeigt als auch eine Aktion ausgeführt werden soll.

## Erstellen von Imagemaps in Adobe Acrobat oder InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Sie können Imagemaps während des Entwerfens Ihres E-Katalogs in Adobe Acrobat oder Adobe InDesign erstellen.

Erstellen Sie in Acrobat oder InDesign Hyperlinks an den Stellen, an denen die Imagemaps angezeigt werden sollen. Geben Sie die entsprechende URL für die Imagemaps an. Wenn Sie beim Hochladen der PDF-Datei in Dynamic Media Classic die Option "Links extrahieren" auswählen, werden die Links automatisch in Imagemaps umgewandelt.

Weitere Informationen finden Sie in der InDesign- oder Acrobat-Hilfe.

### So erstellen Sie Imagemaps in Adobe InDesing {#to-create-image-maps-in-adobe-indesign}

1. Wählen Sie in InDesign „Fenster“ &gt; „Interaktiv“ &gt; „Hyperlinks“, um das Bedienfeld „Hyperlinks“ zu öffnen.
1. Markieren Sie den Text, das Bild oder die Grafik, die Sie in eine Imagemap einfügen möchten.
1. Klicken Sie im Bedienfeldmenü des Bedienfelds „Hyperlinks“ auf die Option „Neuer Hyperlink“.
1. Wählen Sie im Dialogfeld „Neuer Hyperlink“ im Menü „Verknüpfen mit“ die Option „URL“.
1. Geben Sie im Feld „URL“ die Produkt-ID ein und klicken Sie auf „OK“. (Dynamic Media Classic vervollständigt die URL mit der URL-Vorlage der Imagemap.)

   >[!NOTE]
   >
   >Sie müssen keine Optionen für das Aussehen in InDesign festlegen. Sie können die Darstellung in Dynamic Media Classic festlegen.

1. Wiederholen Sie Schritt 2 bis 5 für alle Imagemaps, die Sie erstellen möchten.
1. Exportieren Sie die Datei als PDF.
1. Laden Sie die PDF-Datei in dynamisches Media Classic hoch und wählen Sie aus den PDF-Optionen die Option "Links extrahieren" .

### So erstellen Sie Imagemaps in Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. Wählen Sie in Acrobat „Werkzeuge“ &gt; „Erweiterte Bearbeitung“ &gt; „Verknüpfungswerkzeug“.
1. Erstellen Sie die Imagemap durch Ziehen. Das Feld „Verknüpfung erstellen“ wird geöffnet.
1. Wählen Sie „Benutzerdefinierte Verknüpfung“ und klicken Sie auf „Weiter“.

   ***Hinweis**: Sie müssen keine Optionen für die Darstellung in Acrobat festlegen. Sie können die Darstellung in Dynamic Media Classic festlegen.*

1. Klicken Sie im Feld „Verknüpfungseigenschaften“ auf „Aktionen“.
1. Wählen Sie im Menü „Aktion auswählen“ die Option „Web-Verknüpfung öffnen“ und klicken Sie auf „Hinzufügen“.
1. Geben Sie im Feld „URL bearbeiten“ die Produkt-ID der Imagemap ein und klicken Sie auf „OK“. (Dynamic Media Classic vervollständigt die URL mit der URL-Vorlage der Imagemap.)
1. Wiederholen Sie Schritt 1 bis 7 für alle Imagemaps, die Sie erstellen möchten.
1. Speichern Sie die Datei.
1. Laden Sie die PDF-Datei in dynamisches Media Classic hoch und wählen Sie aus den PDF-Optionen die Option "Links extrahieren" .
