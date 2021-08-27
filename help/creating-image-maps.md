---
title: Imagemaps erstellen
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic Imagemaps erstellen.
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '2422'
ht-degree: 49%

---

# Imagemaps erstellen {#creating-image-maps}

Eine Imagemap ist ein Bereich auf einem Bild oder einer E-Katalog-Seite oder ein Bild in einem Rotationsset, mit dessen Hilfe ein Bedienfeld mit Rollover-Text angezeigt werden kann. Wenn der Benutzer eine Imagemap auswählt, wird eine Aktion irgendeiner Art ausgelöst. Beispielsweise kann eine Website aufgerufen werden, auf der der Benutzer mehr über ein Produkt erfährt. Um eine Imagemap wird ein Umriss angezeigt, wenn der Benutzer den Mauszeiger darüber bewegt.

Neben der Möglichkeit, in Adobe Dynamic Media Classic Imagemaps zu erstellen, können Sie bei der Erstellung eines Katalogs in Adobe Acrobat oder Adobe InDesign auch Imagemaps erstellen.

Beim Erstellen von Imagemaps haben Sie folgende Möglichkeiten:

* Rollover-Text eingeben
* JavaScript und URLs zum Starten von Websites eingeben
* URL-Vorlagen für Imagemaps erstellen
* Imagemaps in andere Bilder, E-Katalogseiten oder Rotationssets kopieren
* Imagemaps in CSV- oder XML-Dateien exportieren
* Importieren Sie Bildmetadaten aus einer tabulatorgetrennten Datei oder aus einer XML-Datei.
* Andere vom W3C (World Wide Web Consortium) festgelegte Aktionen definieren
* Vorschau der Imagemaps anzeigen

## Zeichnen und Anpassen einer Imagemap {#drawing-and-adjusting-an-image-map}

1. Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie in der Rasteransicht oder Listenansicht mit einem Bild arbeiten, wählen Sie in der Dropdown-Liste Bearbeiten die Option **[!UICONTROL Imagemap]** aus. Alternativ können Sie sie in der Detailansicht öffnen und dann **[!UICONTROL Imagemap]** über dem Bild auswählen.
   * Wenn Sie mit einem Rotationsset in der Rasteransicht oder Listenansicht arbeiten, wählen Sie **[!UICONTROL Bearbeiten]**. Oder öffnen Sie es in der Detailansicht und wählen Sie **[!UICONTROL Bearbeiten]** aus. Wählen Sie ein Bild-Asset aus und klicken Sie dann auf **[!UICONTROL Imagemap]**.
   * Wenn Sie mit einem eCatalog arbeiten, wählen Sie in der Rasteransicht, Listenansicht und Detailansicht **[!UICONTROL Bearbeiten]** aus. Wählen Sie die Registerkarte **[!UICONTROL Seiten zuordnen]** aus.

   ![](assets/ma_image_map.png)

1. Sie können eine rechteckige oder polygonale Imagemap zeichnen:

   * **Rechteckige Karte**  - Wählen Sie das Rechteck-Bildzuordnungstool aus und ziehen Sie auf die Seite, um das Rechteck zu erstellen. Um einen Punkt zu einer rechteckigen Karte hinzuzufügen (und sie so in eine Polygon-Karte zu ändern), drücken Sie die Strg-Taste, platzieren Sie das Einfügewerkzeug an der gewünschten Position und wählen Sie aus.

   * **Polygonale Karte**  - Wählen Sie das Polygon-Imagemap-Tool aus und wählen Sie Punkte auf dem Umfang des Bildbereichs aus, den Sie einschließen möchten. Verwenden Sie den Regler für die Dichte des Polygons, um die Punktdichte im Polygon zu ändern. Die ursprüngliche Dichte wird wiederhergestellt, wenn Sie andere Maps auswählen. Wenn ein Punkt im Polygon hinzugefügt, gelöscht oder verschoben wird, wird die ursprüngliche Dichte verworfen und der Regler auf den Maximalwert zurückgesetzt.

1. Geben Sie optional in der Imagemap-Liste einen Namen für die Imagemap ein. Nachdem Sie eine Imagemap gezeichnet haben, weist Adobe Dynamic Media Classic ihr einen Namen zu.

   Um den Namen zu erstellen, hängt Adobe Dynamic Media Classic eine sequenzielle Nummer an den Namen des Bildes oder der E-Katalog-Seite an, mit der Sie arbeiten. Sie können jedoch auch einen Namen Ihrer Wahl eingeben.

1. Wenn Sie möchten, dass Benutzer beim Auswählen der Imagemap eine neue Webseite öffnen, geben Sie die URL in die Liste &quot;Imagemap&quot;ein.

   Siehe [Eingeben von JavaScript und URLs](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. Wenn Rollover-Text angezeigt werden soll, sobald die Benutzer den Mauszeiger über die Imagemap bewegen, geben Sie den Text in der Imagemap-Liste ein. Wählen Sie in der Liste &quot;Imagemap&quot;das Menü **[!UICONTROL Anzeigen]** und dann **[!UICONTROL Rollover-Text]** aus. Geben Sie anschließend den Text ein, der für die Benutzer auf dem Bildschirm angezeigt werden soll. Sie können den Text in einem Textverarbeitungsprogramm schreiben und in das Feld „Rollover-Text“ kopieren.

1. Sie können auch eine andere Aktion definieren, die ausgeführt werden soll, wenn die Benutzer den Mauszeiger über die Imagemap bewegen. Wählen Sie in der Dropdownliste **[!UICONTROL Anzeigen]** die Option **[!UICONTROL Andere Aktionen]** aus. Geben Sie die Attribute der Aktion ein. (Wechseln Sie zu **[!UICONTROL Anzeigen]** > **[!UICONTROL Beide]** , um Rollover-Text und eine Aktion für eine Imagemap zu erstellen.)

   Siehe [Andere Aktionen für Imagemaps definieren](creating-image-maps.md#defining_other_actions_for_image_maps).

1. (Optional) Führen Sie dann einen der folgenden Schritte aus:

   * Um eine Vorschau von Imagemaps anzuzeigen, wählen Sie **[!UICONTROL Vorschau]** aus.
   * Um eine Imagemap oder einen Polygon-Vertex zu löschen, wählen Sie eine Form auf dem Bild aus und klicken Sie dann auf **[!UICONTROL Löschen]**. Oder wählen Sie für einen eCatalog auf der Registerkarte &quot;Seiten ordnen&quot;die Option **[!UICONTROL Maps löschen]** aus, um Imagemaps von allen Seiten zu entfernen.
   * Um eine Imagemap vorübergehend von einem Bild, einer E-Katalogseite oder einem Bild in einem Rotationsset zu entfernen, ohne sie zu löschen, deaktivieren Sie in der Imagemap-Liste die entsprechende Option „Ein“.

1. Wählen Sie **[!UICONTROL Save]** aus.

### Position, Form und Größe von Imagemaps anpassen {#adjusting-the-position-shape-and-size-of-image-maps}

Um die Position, Form und Größe einer Imagemap zu ändern, klicken Sie auf „Imagemap“ . Wählen Sie dann das Tool **[!UICONTROL Schwenken]** aus und befolgen Sie die folgenden Anweisungen:

* **Position ändern**  - Bewegen Sie den Mauszeiger nahe, jedoch nicht über den Rahmen der Imagemap. Wenn der Mauszeiger als Vierfachpfeil dargestellt wird, ziehen Sie die Imagemap an eine andere Position.

* **Größe und Form ändern**  - Wie Sie die Form und Größe einer Imagemap ändern, hängt davon ab, ob Sie mit einer rechteckigen oder polygonalen Imagemap arbeiten:

>[!TIP]
>
>Sie können den Schieberegler „Größe“ unten im Anzeigebereich ziehen, um die Ansichten zu ändern und die Imagemap besser anzeigen zu können.

* **Rechteckige Imagemap** : Bewegen Sie den Mauszeiger über eine Seite oder Ecke der Imagemap. Wenn der Mauszeiger als Doppelpfeil dargestellt wird, ziehen Sie mit der Maus. Halten Sie beim Ziehen die Umschalttaste gedrückt, um die Größe zu ändern, dabei jedoch das Seitenverhältnis (die Form) beizubehalten.

* **Polygonale Imagemap** : Ziehen Sie einen quadratischen Auswahlpunkt. Um einen Auswahlpunkt zu erstellen, wählen Sie den Rahmen der Imagemap aus und beginnen Sie mit dem Ziehen.

### Überlagerte Imagemaps verwalten {#handling-overlapping-image-maps}

Wenn das Bild oder die E-Katalogseite mehrere Imagemaps enthält, die sich überschneiden, können Sie Einstellungen für die Überschneidung festlegen. Ändern Sie dazu in der Imagemap-Liste die Reihenfolge der Imagemaps. Ziehen Sie die Namen zu einer höheren oder niedrigeren Position in der Liste. Die Imagemaps an höheren Positionen überlagern die Imagemaps an niedrigeren Positionen in der Liste.

### Importieren von Imagemap-Daten {#importing-image-map-data}

Anstatt auf jeder Seite Imagemap-Daten einzugeben, können Sie auch die Daten für das Bild, das Rotationsset oder den E-Katalog in den Anzeigebereich mit der Imagemap-Zusammenfassung importieren. Die Imagemap-Daten werden in Form einer tabulatorgetrennten oder XML DTD-Datei importiert. Die Felder in der Datei müssen dieselbe Reihenfolge haben, wie im Anzeigebereich mit der Imagemap-Zusammenfassung dargestellt: „Name“, „Inhaltsverz.“, „Imagemaps“, „URLs“, „Rollover-Text“, „Andere Aktionen“ und „Suchzeichenfolgen“. Indem Sie Imagemap-Daten importieren, können Sie sich die Arbeit beim Eingeben der Daten in der Imagemap-Liste zum Erstellen der einzelnen Imagemaps sparen.

**So importieren Sie Imagemap-Daten:**

1. Gehen Sie zur Seite „Imagemap-Editor“ (für Bilder oder Bilder in Rotationssets) oder zur Registerkarte „Imagemap-Seiten“ im Bearbeitungsbildschirm für E-Kataloge.
1. Wählen Sie **[!UICONTROL Metadaten importieren]** aus.
1. Wählen Sie im Dialogfeld Metadaten hochladen die Option Bild oder Imagemap aus, um die Metadaten vom gewünschten Asset-Eigenschaftstyp hochzuladen.
1. Wählen Sie In der Dropdown-Liste „Datei erstellen“ die Datei aus, die Sie erstellen möchten.
1. (Optional) Wählen Sie **[!UICONTROL Generate]** aus, um die resultierenden Daten basierend auf dem Dateityp, den Sie erstellen möchten, in der Vorschau anzuzeigen. Wählen Sie **[!UICONTROL Close]** aus, um zum Dialogfeld &quot;Metadaten hochladen&quot;zurückzukehren.
1. Navigieren Sie zu der Datei, die Sie hochladen möchten. Geben Sie im Textfeld „Dateiname“ den Namen der erstellten Datei an.
1. (Optional) Geben Sie im Feld „Auftragsname“ einen Namen für den Auftrag „Metadaten hochladen“ ein.
1. Wählen Sie **[!UICONTROL Upload]** aus.

### Kopieren von Imagemaps {#copying-image-maps}

Sie können Imagemaps zwischen Bildern und E-Katalogseiten kopieren. Verwenden Sie **[!UICONTROL Imagemap kopieren]**, um einen Vorsprung bei der Erstellung zu erhalten. Sie können Imagemaps auch kopieren, um sie in Bildern oder Seiten, die das Layout oder die Zuordnungsstruktur gemeinsam haben, neu zu erstellen.

Das Kopieren von Imagemaps in einem E-Katalog ist zum Beispiel eine praktische Möglichkeit, alle Imagemaps in die unterschiedlichen Sprachversionen des gleichen E-Katalogs zu kopieren. Um ein optimales Ergebnis zu erzielen, sollten Sie nach Möglichkeit zwischen E-Katalogen mit derselben Seitenanzahl und den gleichen Bildern kopieren. Wenn der E-Katalog, in den Sie kopieren, bereits Imagemaps enthält, werden diese Imagemaps beim Kopieren gelöscht.

**So kopieren Sie Imagemaps:**

1. Gehen Sie zur Seite „Imagemap-Editor“ (für Bilder oder Bilder in Rotationssets) oder zur Registerkarte „Imagemap-Seiten“ im Bearbeitungsbildschirm für E-Kataloge.
1. Wählen Sie **[!UICONTROL Zuordnungen kopieren zu]** aus.
1. Führen Sie, abhängig davon, ob Sie Imagemaps aus Bildern oder Imagemaps aus einem E-Katalog kopieren möchten, einen der folgenden Schritte aus:

   * (Bilder) Wählen Sie im Bildschirm „Bilder auswählen“ die Bilder aus, die Sie in die Imagemaps kopieren möchten.
   * (E-Katalog) Wählen Sie im Bildschirm „Asset auswählen“ die Bilder oder E-Katalogseiten aus, die Sie in die Imagemaps kopieren möchten.

1. Wählen Sie **[!UICONTROL Select]**.

## Verwenden Sie eine Vorlage, um JavaScript und URLs einzugeben. {#using-a-template-to-enter-javascript-and-urls}

Sie können eine URL-Vorlage (auch Href-Vorlage genannt) definieren, um das Eingeben von Imagemap-URLs einfacher und effizienter zu machen. Es ist sinnvoll, eine URL-Vorlage zu definieren, wenn die meisten Ihrer Imagemap-URLs ein gemeinsames festes Format haben. Wenn Sie den gleich bleibenden Teil der URL als Vorlage definieren, brauchen Sie diesen Teil beim Erstellen einer neuen Imagemap-URL nicht jedes Mal erneut einzugeben. Eine URL-Vorlage kann auch JavaScript-Befehle, Pfadnamen und Parameter enthalten. Standardmäßig enthält die URL-Vorlage einen proprietären JavaScript-Handler der Adobe Dynamic Media Classic namens `loadProduct` , der das Bild in einem neuen Fenster öffnet.

>[!NOTE]
>
>Wenn Sie den JavaScript-Code zum HREF-Attribut Ihrer Imagemap hinzufügen, wird der Code auf dem Computer des Kunden ausgeführt. Stellen Sie daher sicher, dass der JavaScript-Code sicher ist.

### URL-Vorlagen {#about-url-templates}

Eine URL-Vorlage funktioniert so, dass der Inhalt der Spalte „URL“ in der Imagemap-Liste durch ein doppeltes Dollarzeichen (‘$$’) in der Vorlage ersetzt wird: 

```as3
Javascript:loadProduct(‘$$’);void(0);
```

Sie platzieren alle Werte, die sich nicht zwischen Imagemaps ändern, in der URL-Vorlage. Fügen Sie anschließend nur die Werte hinzu, die sich in der Spalte „URL“ der Imagemap-Liste ändern. Beispiel:

* URL-Vorlage - `javascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* URL-Wert - `product.htm`
* Tatsächliche URL generiert - `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

Standardmäßig enthält die URL-Vorlage einen proprietären JavaScript-Handler der Adobe Dynamic Media Classic namens `loadProduct` , der ein neues Fenster mit dem URL-Ziel öffnet. Sie können jedoch beliebigen JavaScript-Code verwenden, um diesen JavaScript-Handler zu ersetzen, oder einen der folgenden Adoben für Dynamic Media Classic-Handler verwenden:

* `loadProductCW` - Zeigt das URL-Ziel an, das in der Spalte „URL“ des aktuellen Fensters angegeben ist. Dieser Handler ist hauptsächlich für E-Kataloge vorgesehen, die in eine Seite innerhalb einer Website integriert sind.

* `loadProductPW` - Zeigt das in der Spalte URL des übergeordneten Fensters angegebene URL-Ziel an (die Seite, die die aktuelle Seite geöffnet hat). Das aktuelle Fenster bleibt geöffnet, während im übergeordneten Fenster das URL-Ziel angezeigt wird.

   >[!NOTE]
   >
   >Der Handler `loadProductPW` unterstützt keine DHTML- und HTML5-Viewer.

### Erstellen einer URL-Vorlage {#creating-a-url-template}

1. Klicken Sie im Anzeigebereich „Map-Editor“ (bei Bildern oder Rotationssets) bzw. auf der Registerkarte „Imagemap-Seiten“ des Anzeigebereichs „E-Katalog“ (bei E-Katalogseiten) neben der Option „URL-Vorlage“ auf „Bearbeiten“. Das Dialogfeld „Verweisvorlage bearbeiten“ wird geöffnet.
1. Geben Sie den JavaScript-Code und die vollständige URL ein (wobei der variable Teil durch die Dollarzeichen [$] ersetzt wird). Sie können den Code einfügen, indem Sie mit der rechten Maustaste klicken und **[!UICONTROL Einfügen]** auswählen.
1. Wählen Sie **[!UICONTROL Save]** aus.

### Umgang mit URL-Vorlagen {#handling-url-templates}

Auf der Seite „Map-Editor“ (bei Bildern und Rotationssets) bzw. der Registerkarte „Imagemap-Seiten“ des Anzeigebereichs „E-Katalog“ (bei E-Katalogseiten) stehen folgende Befehle zum Einstellen von URL-Vorlagen zur Verfügung:

* **Option &quot;URL-Vorlage&quot;**  - Wählen Sie die Option &quot;URL-Vorlage&quot;, um Ihre URL-Vorlage auf alle Imagemaps auf einem Bild oder einer E-Katalog-Seite anzuwenden.

* **Vorlagenoption** : Heben Sie die Auswahl einer Vorlagenoption in der URL-Imagemap-Liste auf, wenn Sie nicht möchten, dass eine einzelne Imagemap die URL-Vorlage verwendet.

## Andere Aktionen für Imagemaps definieren {#defining-other-actions-for-image-maps}

Sie können das Menü **[!UICONTROL Anzeigen]** auswählen und **[!UICONTROL Andere Aktionen]** auswählen, um andere Trigger-Aktionen als Rollover-Text und Webseitenstarts auszuwählen. Wenn der Benutzer den Mauszeiger über eine Imagemap bewegt, kann die Aktion ausgelöst werden. Diese Aktionen sind Attribute, die mithilfe der HTML-Spezifikationen des W3C (World Wide Web Consortium) für clientseitige Imagemaps definiert werden. Diese umfassen Folgende:

* **`accesskey`** - Löst eine Aktion aus, wenn der Benutzer eine bestimmte Taste der Tastatur drückt.

* **`onfocus`** - Trigger eines Ereignisses, wenn die Imagemap den Fokus erhält - durch Cursor, Tab oder Drücken einer Zugriffstaste. Sie können beispielsweise eine Website aufrufen, wenn die Imagemap den Fokus erhält, und sie wieder schließen, wenn die Imagemap den Fokus wieder verliert.

* **`onblur`** - Löst ein Ereignis aus, wenn die Imagemap den Fokus verliert, entweder durch Betätigung des Cursors oder des Tabulators.

**So definieren Sie weitere Aktionen für Imagemaps:**

1. Wählen Sie im Bildschirm &quot;Map Editor&quot;(Bilder und Rotationssets) oder auf der Registerkarte &quot;Map Pages&quot;des E-Katalog-Bildschirms (E-Kataloge) das Menü **[!UICONTROL Anzeigen]** und danach **[!UICONTROL Andere Aktionen]** aus.
1. Fügen Sie unter Verwendung der vom W3C-Konsortium spezifizierten Syntax in der Spalte „Andere Aktionen“ der Imagemap-Liste die unterstützten Attribute ein.
1. Wählen Sie **[!UICONTROL Save]** aus.

Wählen Sie das Menü **[!UICONTROL Anzeigen]** und dann **[!UICONTROL Beide]** aus, wenn eine Imagemap über Rollover-Text und eine Aktion verfügen soll.

## Erstellen von Imagemaps in Adobe Acrobat oder Adobe InDesign {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

Sie können Imagemaps während des Entwerfens Ihres E-Katalogs in Adobe Acrobat oder Adobe InDesign erstellen.

Erstellen Sie in Acrobat oder InDesign Hyperlinks an den Stellen, an denen die Imagemaps angezeigt werden sollen. Geben Sie die entsprechende URL für die Imagemaps an. Wenn Sie beim Hochladen der PDF-Datei in Adobe Dynamic Media Classic die Option Verknüpfungen extrahieren auswählen, werden die Links automatisch in Imagemaps konvertiert.

Weitere Informationen finden Sie in der Hilfe zu Adobe InDesign oder in der Adobe Acrobat-Hilfe.

### So erstellen Sie Imagemaps in Adobe InDesing {#to-create-image-maps-in-adobe-indesign}

1. Gehen Sie unter InDesign zu **[!UICONTROL Windows®]** > **[!UICONTROL Interactive]** > **[!UICONTROL Hyperlinks]**.
1. Wählen Sie im Bedienfeld &quot;Hyperlinks&quot;den Text, den Rahmen oder die Grafik aus, den/die Sie in eine Imagemap aufnehmen möchten.
1. Wählen Sie **[!UICONTROL Neuer Hyperlink]** aus dem Bedienfeldmenü aus.
1. Wählen Sie im Dialogfeld Neuer Hyperlink im Menü **[!UICONTROL Link zu]** die Option **[!UICONTROL URL]**.
1. Geben Sie die Produkt-ID in das Feld &quot;URL&quot;ein oder fügen Sie sie ein.
1. Wählen Sie **[!UICONTROL OK]** aus. (Adobe Dynamic Media Classic vervollständigt die URL mit der URL-Vorlage &quot;Imagemap&quot;.)

   >[!NOTE]
   >
   >Sie müssen keine Darstellungsoptionen in Adobe InDesign festlegen. Sie können das Erscheinungsbild in Adobe Dynamic Media Classic festlegen.

1. Wiederholen Sie Schritt 2 bis 6 für alle Imagemaps, die Sie erstellen möchten.
1. Exportieren Sie die Datei als PDF.
1. Laden Sie die PDF-Datei in Adobe Dynamic Media Classic hoch.
1. Wählen Sie unter **[!UICONTROL PDF Options]** **[!UICONTROL Extract Links]** aus.

### So erstellen Sie Imagemaps in Adobe Acrobat {#to-create-image-maps-in-adobe-acrobat}

1. Gehen Sie in Acrobat zu **[!UICONTROL Tools]** > **[!UICONTROL Erweiterte Bearbeitung]** > **[!UICONTROL Link-Tool]**.
1. Erstellen Sie die Imagemap durch Ziehen.
1. Wählen Sie im Feld Link erstellen die Option **[!UICONTROL Benutzerspezifischer Link]** und klicken Sie auf **[!UICONTROL Weiter]**.

>[!NOTE]
>
>Sie müssen keine Darstellungsoptionen in Adobe Acrobat festlegen. Sie können das Erscheinungsbild in Adobe Dynamic Media Classic festlegen.

1. Wählen Sie im Feld &quot;Link Properties&quot;die Option **[!UICONTROL Actions]**.
1. Wählen Sie **[!UICONTROL Öffnen Sie einen Web-Link]** aus dem Menü Aktion auswählen und wählen Sie dann **[!UICONTROL Hinzufügen]** aus.
1. Geben Sie die Produkt-ID für die Imagemap in das Feld &quot;URL bearbeiten&quot;ein und wählen Sie **[!UICONTROL OK]** aus. (Adobe Dynamic Media Classic vervollständigt die URL mit der URL-Vorlage für die Imagemap.)
1. Wiederholen Sie Schritt 1 bis 7 für alle Imagemaps, die Sie erstellen möchten.
1. Speichern Sie die Datei.
1. Laden Sie die PDF-Datei in Adobe Dynamic Media Classic hoch und wählen Sie aus den PDF-Optionen die Option Verknüpfungen extrahieren aus.
