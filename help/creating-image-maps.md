---
title: Erstellen von Imagemaps
description: Erfahren Sie, wie Sie Imagemaps erstellen.
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '2427'
ht-degree: 62%

---

# Erstellen von Imagemaps{#creating-image-maps}

Eine Imagemap ist ein Bereich auf einem Bild oder einer E-Katalog-Seite oder ein Bild in einem Rotationsset, mit dessen Hilfe ein Bedienfeld mit Rollover-Text angezeigt werden kann. Wenn der Benutzer auf eine Imagemap klickt, wird eine bestimmte Aktion ausgelöst. Beispielsweise kann eine Website aufgerufen werden, auf der der Benutzer mehr über ein Produkt erfährt. Um eine Imagemap wird ein Umriss angezeigt, wenn der Benutzer den Mauszeiger darüber bewegt.

Neben der Möglichkeit, in Dynamic Media Classic Imagemaps zu erstellen, können Sie beim Erstellen eines Katalogs in Adobe Acrobat oder Adobe InDesign auch Imagemaps erstellen.

Beim Erstellen von Imagemaps haben Sie folgende Möglichkeiten:

* Rollover-Text eingeben
* Geben Sie JavaScript™ und URLs zum Starten von Webseiten ein.
* URL-Vorlagen für Imagemaps erstellen
* Imagemaps in andere Bilder, E-Katalogseiten oder Rotationssets kopieren
* Imagemaps in CSV- oder XML-Dateien exportieren
* Importieren Sie Bildmetadaten aus einer tabulatorgetrennten Datei oder aus einer XML-Datei.
* Andere vom W3C (World Wide Web Consortium) festgelegte Aktionen definieren
* Vorschau der Imagemaps anzeigen

## Zeichnen und Anpassen einer Imagemap {#drawing-and-adjusting-an-image-map}

1. Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie mit einem Bild in der Rasteransicht oder Listenansicht arbeiten, klicken Sie in der Dropdownliste &quot;Bearbeiten&quot;auf **Imagemap**. Alternativ können Sie es in der Detailansicht öffnen und dann über dem Bild auf **Imagemap** klicken.
   * Wenn Sie in der Rasteransicht oder Listenansicht mit einem Rotationsset arbeiten, klicken Sie auf **Bearbeiten**. Oder öffnen Sie es in der Detailansicht und klicken Sie dann auf **Bearbeiten**. Wählen Sie ein Bild-Asset aus und klicken Sie dann auf **Imagemap**.
   * Wenn Sie mit einem eCatalog arbeiten, klicken Sie in der Rasteransicht, Listenansicht und Detailansicht auf **Bearbeiten**. Klicken Sie auf die Registerkarte **Seiten zuordnen** .

   ![](assets/ma_image_map.png)

1. Sie können eine rechteckige oder polygonale Imagemap zeichnen:

   **Rechteckige** ZuordnungWählen Sie das Rechteck-Bildzuordnungstool aus und ziehen Sie es auf die Seite, um das Rechteck zu erstellen. Um einen Punkt zu einer rechteckigen Map hinzuzufügen (und sie so in eine polygonale verweissensitive Grafik zu ändern), drücken Sie die Strg-Taste, platzieren Sie das Einfügen-Werkzeug an der gewünschten Position und klicken Sie.

   **Polygonale** LandkarteWählen Sie das Polygon-Imagemap-Tool aus und klicken Sie auf Punkte auf den Bereich des Bildes, das Sie umschließen möchten. Verwenden Sie den Regler für die Dichte des Polygons, um die Punktdichte im Polygon zu ändern. Die ursprüngliche Dichte wird wiederhergestellt, wenn Sie andere Maps auswählen. Wenn ein Punkt im Polygon hinzugefügt, gelöscht oder verschoben wird, wird die ursprüngliche Dichte verworfen und der Regler auf den Maximalwert zurückgesetzt.

1. Geben Sie optional in der Imagemap-Liste einen Namen für die Imagemap ein. Nachdem Sie eine Imagemap gezeichnet haben, weist Dynamic Media Classic ihr einen Namen zu.

   Um den Namen zu erstellen, hängt Dynamic Media Classic eine sequenzielle Nummer an den Namen des Bilds oder der E-Katalog-Seite an, mit der Sie arbeiten. Sie können jedoch auch einen Namen Ihrer Wahl eingeben.

1. Wenn die Benutzer durch Klicken auf die Imagemap eine neue Website öffnen können sollen, geben Sie in der Imagemap-Liste die entsprechende URL ein. 

   Siehe [zur Eingabe von JavaScript™ und URLs](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Wenn Rollover-Text angezeigt werden soll, sobald die Benutzer den Mauszeiger über die Imagemap bewegen, geben Sie den Text in der Imagemap-Liste ein. Wählen Sie im Menü „Anzeigen“ der Imagemap-Liste die Option „Rollover-Text“. Geben Sie anschließend den Text ein, der für die Benutzer auf dem Bildschirm angezeigt werden soll. Sie können den Text in einem Textverarbeitungsprogramm schreiben und in das Feld „Rollover-Text“ kopieren.
1. Sie können auch eine andere Aktion definieren, die ausgeführt werden soll, wenn die Benutzer den Mauszeiger über die Imagemap bewegen. Klicken Sie in der Dropdown-Liste „Anzeigen“ auf „Andere Aktionen“. Geben Sie die Attribute der Aktion ein. (Klicken Sie auf „Anzeigen“ > „Beide“, um den Rollover-Text und eine Aktion für eine Imagemap zu erstellen.)

   Siehe [Definieren anderer Aktionen für Imagemaps](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Optional) Führen Sie einen der folgenden Schritte aus:

   * Um eine Vorschau der Imagemaps anzuzeigen, klicken Sie auf **[!UICONTROL Vorschau]**.
   * Um eine Imagemap oder einen Polygon-Vertex zu löschen, wählen Sie eine Form auf dem Bild aus und klicken Sie dann auf **[!UICONTROL Löschen]**. Oder klicken Sie bei einem eCatalog auf der Registerkarte &quot;Seiten bestellen&quot;auf **[!UICONTROL Maps löschen]** , um Imagemaps von allen Seiten zu entfernen.
   * Um eine Imagemap vorübergehend von einem Bild, einer E-Katalogseite oder einem Bild in einem Rotationsset zu entfernen, ohne sie zu löschen, deaktivieren Sie in der Imagemap-Liste die entsprechende Option „Ein“.

1. Klicken Sie auf „**[!UICONTROL Speichern]**“.

### Anpassen der Position, Form und Größe von Imagemaps {#adjusting-the-position-shape-and-size-of-image-maps}

Um die Position, Form und Größe einer Imagemap zu ändern, klicken Sie auf „Imagemap“ . Wählen Sie dann das Tool **[!UICONTROL Schwenken]** aus und befolgen Sie die folgenden Anweisungen:

**Ändern der Position**  - Verschieben Sie den Zeiger in die Nähe, jedoch nicht über den Rahmen der Imagemap. Wenn der Mauszeiger als Vierfachpfeil dargestellt wird, ziehen Sie die Imagemap an eine andere Position.

**Ändern der Größe und Form**  - Wie Sie die Form und Größe einer Imagemap ändern, hängt davon ab, ob Sie mit einer rechteckigen oder polygonalen Imagemap arbeiten:

>[!TIP]
>
>Sie können den Schieberegler „Größe“ unten im Anzeigebereich ziehen, um die Ansichten zu ändern und die Imagemap besser anzeigen zu können.

**Rechteckige Imagemap** : Bewegen Sie den Mauszeiger über eine Seite oder Ecke der Imagemap. Wenn der Mauszeiger als Doppelpfeil dargestellt wird, ziehen Sie mit der Maus. Halten Sie beim Ziehen die Umschalttaste gedrückt, um die Größe zu ändern, dabei jedoch das Seitenverhältnis (die Form) beizubehalten.

**Polygonale Imagemap** : Ziehen Sie einen quadratischen Auswahlpunkt. Um einen Auswahlziehpunkt zu erstellen, klicken Sie auf den Rand der Imagemap und beginnen Sie zu ziehen.

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

Sie können Imagemaps zwischen Bildern und E-Katalogseiten kopieren. Verwenden Sie **[!UICONTROL Imagemap kopieren]**, um einen Vorsprung bei der Erstellung zu erhalten. Sie können Imagemaps auch kopieren, um sie auf Bildern oder Seiten mit demselben Layout oder derselben Imagemap-Struktur erneut zu verwenden.

Das Kopieren von Imagemaps in einem E-Katalog ist zum Beispiel eine praktische Möglichkeit, alle Imagemaps in die unterschiedlichen Sprachversionen des gleichen E-Katalogs zu kopieren. Um ein optimales Ergebnis zu erzielen, sollten Sie nach Möglichkeit zwischen E-Katalogen mit derselben Seitenanzahl und den gleichen Bildern kopieren. Wenn der E-Katalog, in den Sie kopieren, bereits Imagemaps enthält, werden diese Imagemaps beim Kopieren gelöscht.

**So kopieren Sie Imagemaps**

1. Gehen Sie zur Seite „Imagemap-Editor“ (für Bilder oder Bilder in Rotationssets) oder zur Registerkarte „Imagemap-Seiten“ im Bearbeitungsbildschirm für E-Kataloge.
1. Klicken Sie auf „Imagemaps kopieren zu“.
1. Führen Sie, abhängig davon, ob Sie Imagemaps aus Bildern oder Imagemaps aus einem E-Katalog kopieren möchten, einen der folgenden Schritte aus:

   * (Bilder) Wählen Sie im Bildschirm „Bilder auswählen“ die Bilder aus, die Sie in die Imagemaps kopieren möchten.
   * (E-Katalog) Wählen Sie im Bildschirm „Asset auswählen“ die Bilder oder E-Katalogseiten aus, die Sie in die Imagemaps kopieren möchten.

1. Klicken Sie auf „Auswählen“.

## Verwenden einer Vorlage zur Eingabe von JavaScript™ und URLs {#using-a-template-to-enter-javascript-and-urls}

Sie können eine URL-Vorlage (auch Href-Vorlage genannt) definieren, um das Eingeben von Imagemap-URLs einfacher und effizienter zu machen. Es ist sinnvoll, eine URL-Vorlage zu definieren, wenn die meisten Ihrer Imagemap-URLs ein gemeinsames festes Format haben. Wenn Sie den gleich bleibenden Teil der URL als Vorlage definieren, brauchen Sie diesen Teil beim Erstellen einer neuen Imagemap-URL nicht jedes Mal erneut einzugeben. Ihre URL-Vorlage kann auch JavaScript™-Befehle, Pfadnamen und Parameter enthalten. Standardmäßig enthält die URL-Vorlage einen proprietären Dynamic Media Classic JavaScript™-Handler namens `loadProduct`, der das Bild in einem neuen Fenster öffnet.

>[!NOTE]
>
>Wenn Sie den JavaScript™-Code zum HREF-Attribut Ihrer Imagemap hinzufügen, wird der Code auf dem Computer des Kunden ausgeführt. Stellen Sie daher sicher, dass der JavaScript™-Code sicher ist.

### URL-Vorlagen {#about-url-templates}

Eine URL-Vorlage funktioniert so, dass der Inhalt der Spalte „URL“ in der Imagemap-Liste durch ein doppeltes Dollarzeichen (‘$$’) in der Vorlage ersetzt wird: 

```as3
Javascript:loadProduct(‘$$’);void(0);
```

Sie platzieren alle Werte, die sich nicht zwischen Imagemaps ändern, in der URL-Vorlage. Fügen Sie anschließend nur die Werte hinzu, die sich in der Spalte „URL“ der Imagemap-Liste ändern. Beispiel:

* URL-Vorlage: j `avascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* URL-Wert: `product.htm`
* Tatsächliche URL generiert: `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

Standardmäßig enthält die URL-Vorlage einen proprietären Dynamic Media Classic JavaScript™-Handler namens `loadProduct`, der ein neues Fenster mit dem URL-Ziel öffnet. Sie können jedoch einen beliebigen JavaScript™-Code verwenden, um diesen JavaScript™-Handler zu ersetzen, oder einen der folgenden Dynamic Media Classic-Handler verwenden:

* `loadProductCW`

   Zeigt das URL-Ziel an, das in der Spalte „URL“ des aktuellen Fensters angegeben ist. Dieser Handler ist hauptsächlich für E-Kataloge vorgesehen, die in eine Seite innerhalb einer Website integriert sind.

* `loadProductPW`

   Zeigt das URL-Ziel an, das in der Spalte „URL“ des übergeordneten Fensters (d. h. der Seite, über die die aktuelle Seite geöffnet wurde) angegeben ist. Das aktuelle Fenster bleibt geöffnet, während im übergeordneten Fenster das URL-Ziel angezeigt wird.

   >[!NOTE]
   >
   >Der Handler `loadProductPW` unterstützt keine DHTML- und HTML5-Viewer.

### Erstellen einer URL-Vorlage {#creating-a-url-template}

So erstellen Sie eine URL-Vorlage:

1. Klicken Sie im Anzeigebereich „Map-Editor“ (bei Bildern oder Rotationssets) bzw. auf der Registerkarte „Imagemap-Seiten“ des Anzeigebereichs „E-Katalog“ (bei E-Katalogseiten) neben der Option „URL-Vorlage“ auf „Bearbeiten“. Das Dialogfeld „Verweisvorlage bearbeiten“ wird geöffnet.
1. Geben Sie den JavaScript™-Code und die vollständige URL ein (wobei der variable Teil durch die Dollarzeichen [$] ersetzt wird). Sie können den Code einfügen, indem Sie mit der rechten Maustaste klicken und „Einfügen“ wählen.
1. Klicken Sie auf „Speichern“.

### Arbeiten mit URL-Vorlagen {#handling-url-templates}

Auf der Seite „Map-Editor“ (bei Bildern und Rotationssets) bzw. der Registerkarte „Imagemap-Seiten“ des Anzeigebereichs „E-Katalog“ (bei E-Katalogseiten) stehen folgende Befehle zum Einstellen von URL-Vorlagen zur Verfügung:

* **Option &quot;URL-Vorlage&quot;** Wählen Sie die Option URL-Vorlage aus, um Ihre URL-Vorlage auf alle Imagemaps auf einem Bild oder einer E-Katalog-Seite anzuwenden.

* **Vorlagenoption** Deaktivieren Sie eine Vorlagenoption in der URL-Imagemap-Liste, wenn Sie nicht möchten, dass eine einzelne Imagemap die URL-Vorlage verwendet.

## Festlegen anderer Aktionen für Imagemaps {#defining-other-actions-for-image-maps}

Sie können im Menü „Anzeigen“ die Option „Andere Aktionen“ wählen, um andere Aktionen als die Anzeige von Rollover-Text und den Aufruf von Websites auszulösen. Wenn der Benutzer den Mauszeiger über eine Imagemap bewegt, kann die Aktion ausgelöst werden. Diese Aktionen sind Attribute, die mithilfe der HTML-Spezifikationen des W3C (World Wide Web Consortium) für clientseitige Imagemaps definiert werden. Diese umfassen Folgende:

* **accessKey** : Trigger einer Aktion, wenn der Benutzer eine bestimmte Taste auf der Tastatur drückt.

* **onfocus**  - Trigger eines Ereignisses, das beim Fokuswechsel der Imagemap ausgelöst wird, durch Cursor, Tab oder Drücken einer Zugriffstaste. Sie können beispielsweise eine Website aufrufen, wenn die Imagemap den Fokus erhält, und sie wieder schließen, wenn die Imagemap den Fokus wieder verliert.

* **onblur**  - Trigger eines Ereignisses, bei dem die Imagemap den Fokus verliert, entweder durch den Cursor oder durch Tab.

**So definieren Sie weitere Aktionen für Imagemaps:**

1. Öffnen Sie im Anzeigebereich „Map-Editor“ (bei Bildern und Rotationssets) bzw. auf der Registerkarte „Imagemap-Seiten“ des Anzeigebereichs „E-Katalog“ (bei E-Katalogseiten) das Menü „Anzeigen“ und wählen Sie die Option „Andere Aktionen“.
1. Fügen Sie unter Verwendung der vom W3C-Konsortium spezifizierten Syntax in der Spalte „Andere Aktionen“ der Imagemap-Liste die unterstützten Attribute ein.
1. Klicken Sie auf „**[!UICONTROL Speichern]**“.

Wählen Sie das Menü **[!UICONTROL Anzeigen]** und dann **[!UICONTROL Beide]** aus, wenn eine Imagemap über Rollover-Text und eine Aktion verfügen soll.

## Erstellen von Imagemaps in Adobe Acrobat oder InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Sie können Imagemaps während des Entwerfens Ihres E-Katalogs in Adobe Acrobat oder Adobe InDesign erstellen.

Erstellen Sie in Acrobat oder InDesign Hyperlinks an den Stellen, an denen die Imagemaps angezeigt werden sollen. Geben Sie die entsprechende URL für die Imagemaps an. Wenn Sie beim Hochladen der PDF-Datei in Dynamic Media Classic die Option Links extrahieren auswählen, werden die Links automatisch in Imagemaps konvertiert.

Weitere Informationen finden Sie in der Hilfe zu Adobe InDesign oder in der Adobe Acrobat-Hilfe.

### So erstellen Sie Imagemaps in Adobe InDesing {#to-create-image-maps-in-adobe-indesign}

1. Klicken Sie unter InDesign auf **[!UICONTROL Windows®]** > **[!UICONTROL Interactive]** > **[!UICONTROL Hyperlinks]** , um das Bedienfeld &quot;Hyperlinks&quot;zu öffnen.
1. Markieren Sie den Text, das Bild oder die Grafik, die Sie in eine Imagemap einfügen möchten.
1. Klicken Sie im Bedienfeld &quot;Hyperlinks&quot;im Bedienfeldmenü auf **[!UICONTROL Neuer Hyperlink]** .
1. Wählen Sie im Dialogfeld Neuer Hyperlink die Option **[!UICONTROL URL]** aus dem Menü Link zu .
1. Geben oder fügen Sie die Produkt-ID in das URL-Feld ein und klicken Sie auf **[!UICONTROL OK]**. (Dynamic Media Classic vervollständigt die URL mit der URL-Vorlage für Imagemap.)

   >[!NOTE]
   >
   >Sie müssen keine Darstellungsoptionen in Adobe InDesign festlegen. Sie können das Erscheinungsbild in Dynamic Media Classic festlegen.

1. Wiederholen Sie Schritt 2 bis 5 für alle Imagemaps, die Sie erstellen möchten.
1. Exportieren Sie die Datei als PDF.
1. Laden Sie die PDF-Datei in Dynamic Media Classic hoch und wählen Sie aus den PDF-Optionen die Option Links extrahieren aus.

### So erstellen Sie Imagemaps in Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. Klicken Sie in Acrobat auf **[!UICONTROL Tools]** > **[!UICONTROL Erweiterte Bearbeitung]** > **[!UICONTROL Link-Tool]**.
1. Erstellen Sie die Imagemap durch Ziehen. Das Feld „Verknüpfung erstellen“ wird geöffnet.
1. Wählen Sie **[!UICONTROL Benutzerspezifischer Link]** und klicken Sie auf **[!UICONTROL Weiter]**.

>[!NOTE]
>
>Sie müssen keine Darstellungsoptionen in Adobe Acrobat festlegen. Sie können das Erscheinungsbild in Dynamic Media Classic festlegen.

1. Klicken Sie im Feld &quot;Link Properties&quot;auf **[!UICONTROL Actions]**.
1. Wählen Sie **[!UICONTROL Öffnen Sie einen Web-Link]** aus dem Menü Aktion auswählen und klicken Sie dann auf **[!UICONTROL Hinzufügen]**.
1. Geben Sie die Produkt-ID für die Imagemap in das Feld &quot;URL bearbeiten&quot;ein und klicken Sie auf **[!UICONTROL OK]**. (Dynamic Media Classic vervollständigt die URL mit der URL-Vorlage für die Imagemap.)
1. Wiederholen Sie Schritt 1 bis 7 für alle Imagemaps, die Sie erstellen möchten.
1. Speichern Sie die Datei.
1. Laden Sie die PDF-Datei in Dynamic Media Classic hoch und wählen Sie aus den PDF-Optionen die Option Links extrahieren aus.
