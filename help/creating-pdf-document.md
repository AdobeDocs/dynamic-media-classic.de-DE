---
title: Erstellen eines PDF-Dokuments
seo-title: Erstellen eines PDF-Dokuments
description: 'null'
seo-description: Erfahren Sie, wie Sie ein PDF-Dokument mithilfe des Web-to-Print-Prozesses in Dynamic Media Classic erstellen.
uuid: 274fb06b-320b-40fa-8b61-c224d8aceaa1
contentOwner: admin
content-type: Verweis
products: SG_EXPERIENCEMANAGER/Dynamic Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 87e91e8e-10a2-4fba-87c7-aad2bd798146
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Erstellen eines PDF-Dokuments {#creating-a-pdf-document}

Als letzten Schritt im Web-to-Print-Prozess wird die benutzerdefinierte PDF generiert. Nachdem die Endbenutzer mithilfe der von Ihnen erstellten Webanwendung die Vorlage personalisiert haben, erstellen sie das endgültige PDF-Dokument. Die endgültige PDF wird in der Regel für den Druck von professioneller Güte an eine Druckerei geschickt. Unter Anwendung der richtigen JobOptions-Datei und durch richtiges Einrichten von Schriftarten, Druckermarkierungen und Farben stellen Entwickler sicher, dass die endgültige PDF erwartungsgemäß gedruckt wird.

## Einstellen von PDF-Vorgaben {#setting-up-pdf-presets}

Geben Sie die PDF-Kompatibilitätsstufe und Druckereinstellungen an, indem Sie eine PDF-JobOptions-Datei erstellen und auf den Dynamic Media Classic Server hochladen. Sie können z. B. PDF/X-4-kompatible PDF-Ausgabe wählen (für PDF-Druck-/-Veröffentlichungsworkflows empfohlen). Sie können die JobOptions-Datei in ihrer Authoring Software (wie z. B. Adobe Illustrator) oder in Acrobat erstellen. Konsultieren Sie stets Ihre Druckerei, um die richtigen Auftragsoptionseinstellungen für Ihren Druckauftrag zu erhalten.

Weitere Informationen zum Erstellen von JobOptions-Dateien sowie Informationen zum Erstellen einer JobOptions-Datei in Acrobat finden Sie in der Adobe Acrobat-Hilfe.

So erstellen Sie eine JobOptions-Datei in Illustrator

1. Wählen Sie „Bearbeiten“ &gt; „Adobe PDF-Vorgaben“.
1. Wählen Sie im Dialogfeld die Vorgabe, die Sie verwenden möchten.

   Die folgenden Auftragsoptionseinstellungen werden von Dynamic Media Classic unterstützt:

   | Auftragsoption | Beschreibung |
   |--- |--- |
   | Allgemein | <ul><li>Kompatibilität </li><li>Komprimierung auf Objektebene</li><li>Miniaturansichten einbetten</li><li>Für schnelle Webansicht optimieren</li></ul> |
   | Bilder | <ul><li>Downsampling</li><li>Auflösung</li><li>Schwelle</li><li>Komprimierung für Farbe, Grau und Mono</li></ul> |
   | Schriftarten | <ul><li>Alle Schriftarten einbetten (Schriftarten werden standardmäßig eingebettet)</li><li>OpenType-Schriftarten einbetten</li><li>Subset-Schriften, wenn Prozentsatz der Zeichen kleiner ist als:</li><li>Liste immer einbetten</li><li>Liste niemals einbetten</li></ul> |
   | Farbe | <ul><li>Farbstrategie („Nur Bilder für Farbmanagement kennzeichnen“ wird wie „Alles für Farbmanagement kennzeichnen“ behandelt)</li><li>Dokument-Renderpriorität</li><li>Nur die folgenden Arbeitsfarbräume werden für 4.2.5 unterstützt. Mit Version 4.3 können Sie jedes vom Kunden bereitgestellte Profil verwenden, das zu IPS hochgeladen wurde.</li><li>Als Problemumgehung können Sie den Zielarbeitsfarbraum für das zu konvertierende Bildmaterial unter Anwendung der Standardfarbprofile des Unternehmens angeben.</li></ul> |
   | RGB | <ul><li>e-sRGB </li><li>scRGB with encoding range [-4.0, 4.0]</li><li>Lab D50</li><li>PCS XYZ</li><li>Flat XYZ</li><li>Linear ROMM-RGB</li><li>ROMM-RGB</li><li>sYCC 8-Bit</li><li>e-sYCC 8-Bit</li></ul> |
   | Grau | <ul><li>Grau Gamma 1.8</li><li>Grau Gamma 2.2</li><li>Tonwertzuwachs 10%</li><li>Tonwertzuwachs 15%</li><li>Tonwertzuwachs 20%</li><li>Tonwertzuwachs 25%</li><li>Tonwertzuwachs 30%</li><li>sGray</li></ul> |
   | CMYK-Werte für kalibrierte CMYK-Farbräume beibehalten |  |
   | Erweitert | „OPI-Kommentare beibehalten“ ist immer aktiviert |
   | Standards | Einhaltungsstandard |

   >[!NOTE]
   >
   >Dynamic Media Classic ignoriert Druckermarkierungseinstellungen in der JobOptions-Datei. Stattdessen werden Druckmarken mithilfe der URL-Befehle von Dynamic Media Classic konfiguriert.

1. Klicken Sie auf „Exportieren“, geben Sie einen Namen und Speicherort an, und klicken Sie auf „Speichern“.
1. Laden Sie die JobOptions-Datei als Asset zum Scene7 Publishing System hoch.

   Verwenden Sie sie mit Ihrer veröffentlichten Vorlage, indem Sie sie in der URL referenzieren. Beispiel:

   `https://yourpublishserver.scene7.com/is/agm/SiliconPublishing/PetNews?&fmt=pdf,cmyk&joboption=SPSfilenameid`

## Vorbereitung der PDF für den Druck {#preparing-the-pdf-for-print}

Befolgen Sie die in diesem Abschnitt erläuterten Richtlinien, bevor Sie letzte Vorbereitungen an Ihrer PDF für den Druck treffen.

**Bilder**

Vergewissern Sie sich, dass alle Bilder in Ihrem Veröffentlichungsauftrag auf Ihren Dynamic Media Classic-Server hochgeladen und veröffentlicht wurden.

**Schriftarten**

Vergewissern Sie sich, dass alle Schriftarten in Ihrem Veröffentlichungsauftrag auf Ihren Dynamic Media Classic-Server hochgeladen und veröffentlicht wurden. Vergewissern Sie sich, dass Sie über die rechtlichen Berechtigungen zum Hosten der Schriftarten verfügen, wenn Sie möchten, dass Endbenutzer sie ändern können.

**Bildauflösung (Pixel pro Zoll)**

Die Auflösung von Bitmapbildern wird vom Dynamic Media Classic-Server in generierten druckfertigen PDFs beibehalten. Bei Dynamic Media Classic wird bei Bedarf die Bildauflösung skaliert. Um optimale Ergebnisse zu gewährleisten, belassen Sie die Auflösung bei der Vorschau im Internet auf dem Standardwert (normalerweise 72 DPI). Die Standardauflösung für alle Bilder in Ihrem Unternehmen wird im Fenster „Einstellungen für Veröffentlichungen“/„Image-Server“ im Abschnitt „Standarddruckauflösung“ festgelegt. Höhere Auflösungen (wie z. B. 300 DPI) können eine längere Verarbeitungszeit zur Folge haben und sollten nur bei druckfertigen PDFs angewendet werden. Mit dem Befehl „imageRes=“ in der URL setzen Sie die Standardauflösung für PDF-Aufträge manuell außer Kraft.

**Farbmanagement**

Für Ihre Dokumente und Bilder können Graustufen-, CMYK-, benannte Volltonfarben-, RGB- oder Lab-Farbenmodelle verwendet werden. Jede wird unkalibriert oder kalibriert unter Anwendung eines ICC-Farbprofils verwendet. Die besten Ergebnisse werden durch Einbettung des Profils in die generierte, druckfertige PDF erzielt. Der Server von Dynamic Media Classic führt dies standardmäßig aus. Vergewissern Sie sich, dass alle erforderlichen Farbprofile auf die Dynamic Media Classic-Plattform hochgeladen wurden. Achten Sie vorzugsweise darauf, dass die in Ihrer Designanwendung festgelegten Farbmanagementoptionen mit den in Ihrem Dynamic Media Classic Server festgelegten übereinstimmen:

* **Farbmanagementeinstellungen in der Design-Anwendung:** Geben Sie in den Farbeinstellungen Ihrer Authoring Software (wie z. B. Adobe Illustrator) die RGB- und CMYK-Farbprofile im Arbeitsfarbraumabschnitt an.

* **** Einstellungen für das dynamische Medienklassische Farbmanagement: In der Regel sollten die Farbmanagementeinstellungen in der Designanwendung mit den Standardfarbprofilen in Ihrem Dynamic Media Classic-Server übereinstimmen. Diese Einstellungen finden Sie im Fenster „Veröffentlichungseinstellungen/Image-Server“.

## Anzeigen von Druckmarken {#displaying-printer-marks}

In folgenden Fällen erstellen Sie möglicherweise eine PDF:

* Bei einem fertigen Dokument
* Bei einem Zwischendokument, wie einem Film oder einer Bildtafel, die zur Produktion an die Druckerei gesendet wird

Ein Zwischendokument kann zusätzliche Produktionsinhalte enthalten, wie z. B. Beschnittränder, Druckermarkierungen usw. Diese Inhalte werden in der Regel außerhalb der Grenzen der fertigen Seite angezeigt.

Alle im Anzeigebereich zum Hinzufügen von Druckermarken in Acrobat verfügbaren Marken werden unterstützt. Die Druckermarken werden über den Parameter `printerMark` gesteuert. Die Syntax lautet `&printerMark=trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed`.

* trim marks = 0|1
* bleed marks = 0|1
* registration marks = 0|1
* color bars = 0|1
* page information = 0|1
* style = | Illustrator | IllustratorJ | QuarkXPress
* line weight = 0.125 | 0.25 | 0.50
* layer embed = 0|1

Bei der Vorbereitung eines Dokuments für den Druck sind möglicherweise Druckmarken erforderlich, damit der Druckdienstleister Trennfilme für Proofs besser ausrichten, Filme für die richtige Kalibrierung und Tintendichte besser abmessen, Filme besser auf die richtige Größe zuschneiden kann usw. Druckmarken geben die Begrenzungen von Dokumentrahmen wie Endformatrahmen und Anschnittrahmen an. Zu den produktionsrelevanten Inhalten gehören u. a.:

* **Medienrahmen** Die Grenzen des physischen Mediums, auf dem die Seite gedruckt wird. Inhalte außerhalb des Medienrahmens können ohne Bedenken verworfen werden; die bedeutsamen Dateiinhalte werden nicht beeinträchtigt.

* **Anschnittrahmen** Der Bereich, auf den der Inhalt der Seite bei der Ausgabe in einer Produktionsumgebung abgeschnitten wird. Der Anschnittrahmen kann Bereiche enthalten, die aufgrund der physischen Einschränkungen von Schnitt-, Faltungs- und Zuschnittgeräten erforderlich sind. Der Standardwert ist der Maskenrahmen der Seite.

* **Endformatrahmen** Die vorgesehenen Abmessungen der fertigen Seite nach dem Beschneiden. Der Endformatrahmen kann kleiner als der Medienrahmen sein, um produktionsrelevante Inhalte wie Druckanweisungen, Schnittmarken und Farbbalken zu ermöglichen. Der Standardwert ist der Maskenrahmen der Seite.

* **Objektrahmen** Der Umfang des aussagekräftigen Inhalts der Seite (einschließlich potenzieller Leerraum), wie vom Ersteller der Seite beabsichtigt. Der Standardwert ist der Maskenrahmen der Seite.

Sie können die in der folgenden Tabelle aufgeführten Modifikatoren verwenden, um die in Adobe Illustrator, InDesign und Acrobat verfügbaren Druckmarken zu replizieren:

| Modifikator/Werte | Beschreibung |
|--- |--- |
| bleedMargin=top, left, bottom, right | Dieser wird in Acrobat mit der Option „Seiten beschneiden“ angegeben. Wählen Sie „BleedBox“, und geben Sie die Ränder mit der Option „Randeinstellungen“ an.<br><br>Die Werte stehen für den Abstand des oberen, linken, unteren und rechten Randes von den ursprünglichen Rändern des Bildmaterials (des Medienrahmens) nach innen. Die Werte (0-1000) werden in Punkt angegeben.<br><br>Neue Höhe = ursprüngliche Höhe - (oben + unten)<br><br>Neue Breite = ursprüngliche Breite - (links + rechts) |
| mediaMargin=top, left, bottom, right | Dieser wird in Acrobat mit der Option „Seiten beschneiden“ angegeben. Ändern Sie die benutzerdefinierte Seitengröße unter der Option „Seitengröße ändern“.<br><br>Die Werte stehen für den Abstand des oberen, linken, unteren und rechten Randes von den ursprünglichen Rändern des Bildmaterials (des Medienrahmens) nach außen. Die Werte (0-1000) werden in Punkt angegeben.<br><br>Neue Höhe=oben+unten+ursprüngliche<br><br>HöheNeue Breite=oben+unten+ursprüngliche<br><br>BreiteDie neuen Werte für Höhe und Breite bestimmen die neue Seitengröße der erstellten PDF.<br><br>Sobald ein neuer Medienrahmen definiert wurde, muss bei allen Berechnungen des Endformat- und des Anschnittrahmens der Medienrahmen als Kante des Bildmaterials berücksichtigt werden. |
| trimMargin=top, left, bottom, right | Dieser wird in Acrobat mit der Option „Seiten beschneiden“ angegeben. Wählen Sie „Endformatrahmen“, und geben Sie mit der Option „Randeinstellungen“ die Ränder an.<br><br>Die Werte stehen für den Abstand des oberen, linken, unteren und rechten Randes von den ursprünglichen Rändern des Bildmaterials (des Medienrahmens) nach innen. Die Werte (0-1000) werden in Punkt angegeben.<br><br>Neue Höhe = ursprüngliche Höhe - (oben + unten)<br><br>Neue Breite = ursprüngliche Breite - (links + rechts) |
| printerMark= trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed | Die Werte lauten wie folgt:<br><br>trim marks = 0,1 (Standard: 0)<br><br>bleed marks = 0,1 (Standard: 0)<br><br>registration marks = 0,1 (Standard: 0)<br><br>color bars = 0,1 (Standard: 0)<br><br>page information = 0,1 (Standard: 0)<br><br>style = Default, InDesignJ1, InDesignJ2, Illustrator, J, QuarkXPress (Standard)<br><br>line weight= 0.125-0.2, beide Werte einschließlich (Standard: 0.25)<br><br>layer embed = 0, 1, wobei 1 eine neue Ebene mit allen Druckermarken (Standard: 1)<br><br>Je nach verwendetem Stil erscheinen die Markierungen und Farbleisten unterschiedlich und entsprechen den entsprechenden Stilen, die Acrobat verwendet. |

Folgendes ist zu Druckmarken zu beachten:

* Geben Sie Anschnittränder, Endformatränder und Medienränder beim Festlegen von Druckmarken durch URL-Aufrufe an. Wenn Sie Druckmarken ohne diese Ränder festlegen, werden diese Marken außerhalb des sichtbaren Bereichs der erzeugten PDF angelegt. Außerdem überlappen die Endformat- und Anschnittmarken.
* Wenn Sie dieselben Randwerte für Endformat- und Anschnittränder festlegen, überlappen die Endformat- und Anschnittmarken, wenn beide in `&printerMark` auf 1 gesetzt sind.
* Wenn Sie über URL-Aufrufe als Format SWF („fmt=swf“) oder Bildformate festlegen, enthält die Ausgabe keine Druckmarken oder Ränder, weil es sich um eine Funktion speziell für die PDF-Ausgabe handelt.
* Specifying `&printerMark=`through the URL results in default values being used for all parameters. Specifying `&printerMark=1` results in trim marks being set to 1 and default values for other parameters. Um das n-te Element zu aktivieren, müssen jedoch alle Parameter (n-1) über die URL festgelegt werden.
* Specifying only one value for `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in that value being applied to all the top, bottom, left, and right margins of the original artwork.
* Specifying only the top and left values through `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in the top value being assigned to the bottom value and the left value being equal to the right.
* Not specifying the right value through `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in the left value being assigned to the right.
* Bei mehrseitigen PDFs werden die Druckmarken/-ränder auf alle Seiten angewendet (in Acrobat können Benutzer Seitenbereiche für Druckmarken/-ränder auswählen).
* Die Ausgabe einer PDF mit aktivierten Druckmarken/Rändern stimmt exakt mit Acrobat X überein, wenn nicht anders angegeben.

Wenn Sie über den &amp;joboption-Modifikator in der URL eine PDF/X-4-kompatible PDF erstellen möchten, beachten Sie die Einschränkungen im Hinblick auf Druckermarkierungen, die in der PDF ISO_15930-7-2008.pdf angegeben sind:

* Jedes Seitenobjekt einer PDF-Datei enthält einen Medienrahmen. Jedes Seitenobjekt in einer PDF/X-4-kompatiblen Datei sollte einen Endformatrahmen oder einen Objektrahmen enthalten, nicht jedoch beides. Der Medienrahmen kann durch Vererbung eingeschlossen werden.
* Wenn es einen Anschnittrahmen gibt, dürfen der Objektrahmen oder der Endformatrahmen nicht über die Grenzen des Anschnittrahmens hinausgehen. Wenn es einen Maskenrahmen gibt, dürfen weder der Objektrahmen, noch der Endformatrahmen oder der Anschnittrahmen über die Grenzen des Maskenrahmens hinausgehen.
* Weder der Objektrahmen, noch der Endformatrahmen, der Maskenrahmen oder der Anschnittrahmen darf über die Grenzen des Medienrahmens hinausgehen.
* In einigen industriellen Anwendungen ist die Verwendung eines Anschnittrahmens erforderlich. Dabei sollten angemessene Handelspraktiken angewandt werden.
* Die Verwendung eines Endformatrahmens sollte der Verwendung eines Objektrahmens vorgezogen werden.
* Alle anderen Annotationen als TrapNet und PrinterMark müssen einen Wert für Rect haben, der vollständig außerhalb des Anschnittrahmens liegt (bzw. des Endformatrahmens oder Objektrahmens, wenn es keinen Anschnittrahmen gibt). Alle PrinterMark-Annotationen müssen einen Wert für Rect haben, der vollständig außerhalb des Endformatrahmens bzw. des Objektrahmens liegt. Ein PDF/X-4-kompatibler Reader kann Annotationen vollständig ignorieren, außer PDF TrapNet-Annotationen.
* Ein Rect gilt als vollständig außerhalb eines Begrenzungsrahmens, wenn alle Koordinaten des Rect außerhalb oder auf der Kante des Begrenzungsrahmens liegen. Die Überschneidung der beiden Rechtecke muss gleich Null sein.
* Wenn das ViewerPreferences-Wörterbuch die Schlüssel ViewArea, ViewClip, PrintArea oder PrintClip enthält, müssen diese Schlüssel den Wert MediaBox oder (wenn es in allen Seitenobjekten der Datei einen Anschnittrahmen gibt) oder BleedBox haben.

