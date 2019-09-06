---
title: '"Kurzanleitung: Bildgrößenänderung"'
seo-title: '"Kurzanleitung: Bildgrößenänderung"'
description: 'null'
seo-description: Eine Einführung und Schnellstart zur Bildgrößenänderung, mit der Sie schnell mit den Techniken zur Bildgrößenänderung vertraut sind.
uuid: 6 c 4 ad 4 b 7-549 d -4 daa-b 6 b 9-5997 a 8427 af 8
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/image_ sizing
discoiquuid: dcaa 9 b 21-b 925-4 dbb -865 e -7918 cdbda 50 c
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Kurzanleitung: Bildgrößenänderung{#quick-start-image-sizing}

Die Bildgrößenänderung bezeichnet die Fähigkeit von Dynamic Media Classic, mehrere Bilder basierend auf einem Bild mit hoher Auflösung zu erstellen. Anstatt mehrere Bilder (z. B. eine Miniaturansicht und ein vergrößertes Bild) für Ihre Website oder Anwendung manuell zu erstellen, geben Sie ein einzelnes Masterbild an. Dynamic Media Classic generiert alle geänderten Bilder, genau wie Sie anfordern. Die dynamische Bereitstellung von Bildern basierend auf nur einem Masterbild ist mit zahlreichen Vorteilen verbunden:

* Sie müssen nicht manuell verschiedene Bildversionen in unterschiedlichen Größen erstellen. Sie stellen ein Masterbild für dynamisches Media Classic bereit, und dynamisches Media Classic erstellt vom Masterbild unterschiedliche Ableitungen.
* Sie können schnell die Größe für einen bestimmten Bildtyp in der gesamten Website bzw. Anwendung ändern. Möchten Sie beispielsweise alle Miniaturansichten ändern, bearbeiten Sie dazu die Bildvorgabe „Miniaturansicht“. Eine Bildvorgabe ähnelt einem Makro – mehrere Attribute für Größe und Formatierung sind darin gesammelt. Sie können die Bildvorgabe „Miniaturansicht“ bearbeiten, um die Größe aller in der Website bzw. Anwendung vorhandenen Miniaturansichten zu ändern.
* Es ist nicht erforderlich, die Masterversionen und sämtliche verschiedenen Ableitungen mit Content-Management- oder Asset-Management-Systemen intern oder extern zu verwalten.

![Sie können mehrere abgeleitete Bilder in unterschiedlichen Größen aus derselben hochauflösenden Masterdatei erstellen.](/help/assets/is_derivative_sizes_popup.png)

**Kurzanleitung**

Diese Kurzanleitung zum Thema Bildgrößenänderung ermöglicht einen schnellen Einstieg in die Technik der Bildgrößenänderung im Scene7 Publishing System. Führen Sie die Schritte 1-5 aus. Nach jedem Schritt wird auf ein Thema mit weiteren Informationen verwiesen.

**1. Hochladen von Masterbildern**

Zunächst laden Sie Ihre Masterbilder in das Scene7 Publishing System hoch. In Bezug auf die Größe empfiehlt Dynamic Media Classic, Bilder zu verwenden, die der größten erwarteten Verwendung auf Ihrer Website oder in Ihrer Anwendung entsprechen. Möchten Sie beispielsweise, dass Betrachter die Bilder per Zoom vergrößern können, sollten Sie Bilder hochladen, deren längste Abmessung (Breite oder Höhe) mindestens 2000 Pixel beträgt. Dynamic Media Classic unterstützt zahlreiche Bilddateiformate, verlustfreie TIFF- und PNG-Bilder werden jedoch empfohlen.

Klicken Sie auf der Symbolleiste für globale Navigation auf die Schaltfläche „Hochladen“, um Dateien von Ihrem Computer in einen Ordner im Scene7 Publishing System hochzuladen. Siehe [Hochladen von Masterbildern](uploading-master-images.md#uploading_master_images).

**2. Einstellen von Bildvorgaben**

Ähnlich wie bei einem Makro sind in einer Bildvorgabe vordefinierte Größen- und Formatierungsbefehle unter einem gemeinsamen Namen gespeichert. Eine Bildvorgabe wirkt sich auf die Größe und Formatierung aus, mit der Bilder von dynamischen Medienservern bereitgestellt werden. Wenn Sie den Status eines Unternehmensadministrators haben, können Sie Bildvorgaben selbst anlegen. Dynamic Media Classic verfügt außerdem über standardmäßige Bildvorgaben, die Sie zum dynamischen Bereitstellen von Bildern verwenden können.

Um als Administrator eine Bildvorgabe zu erstellen, wählen Sie „Einstellungen“ &gt; „Anwendungseinstellungen“. Blenden Sie im Anzeigebereich „Einstellungen“ die Optionen für „Anwendungseinstellungen“ ein und wählen Sie „Bildvorgaben“. Klicken Sie dann auf **"Hinzufügen** «oder **" Bearbeiten** " , um eine Bildvorgabe zu erstellen.

Die von Ihnen erstelle Bildvorgabe wird im Anzeigebereich „Vorschau“ in das Menü „Bildvorgabe“ eingefügt. Mithilfe der neuen Bildvorgabe können Sie Bilder auf Ihren Websites und in Ihren Anwendungen dynamisch anzeigen. Siehe [Einstellen von Bildvorgaben](setting-image-presets.md#setting_up_image_presets).

**3. Anzeigen einer Vorschau für Bildvorgaben**

Der nächste Schritt besteht im Anzeigen einer Vorschau der Bildvorgaben, die Ihr Administrator für die unterschiedlichen vorgegebenen Größen eingestellt hat. 

To explore Image Presets, click **Setup** &gt; **Image Presets**, and then browse to an Image Preset.

Experimentieren Sie mit verschiedenen Bildvorgaben. Finden Sie heraus, wie sich die dynamische Ausgabe in verschiedenen Größen auf Ihrer Website bzw. in Ihrer Anwendung auswirkt. 

Siehe [Anzeigen eines Bild-Asset auf Grundlage seiner Bildvorgabe](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

**4. Veröffentlichen von Masterbildern**

Das Veröffentlichen Ihrer Masterbilddateien hat zwei wichtige Auswirkungen:

* Veröffentlichen der Masterbilder auf dynamischen Medienservern, damit Bilder dynamisch an Ihre Website und Anwendung übertragen werden können.
* Beim Veröffentlichen werden die URL-Zeichenfolgen zum Aufrufen von Bildern von dynamischen Medienservern für Ihre Website oder Anwendung aktiviert. Nach der Veröffentlichung können Sie die mit klassischen Medien generierten urls kopieren und ggf. auf Ihrer Website oder in Ihrer Anwendung platzieren.

Klicken Sie auf der Symbolleiste für globale Navigation auf die Schaltfläche „Veröffentlichen“, um einen Veröffentlichungsvorgang einzuleiten. Klicken Sie im Anzeigebereich „Veröffentlichen“ auf die Schaltfläche „Veröffentlichungsvorgang starten“. Siehe [Veröffentlichen von Masterbildern](publishing-master-images.md#publishing_master_images).

**5. Verknüpfen von URLs mit einer Web-Anwendung**

Dynamic Media Classic erstellt URL-Zeichenfolgen für Bilder. Wenn Sie Bilder auf dynamischen Medienservern veröffentlichen, werden die urls aktiv. Sie können diese URL-Zeichenfolgen vom Durchsuchenbedienfeld (in der Detailansicht) oder vom Anzeigebereich „Vorschau“ aus kopieren. Nach dem Kopieren sind die URL-Zeichenfolgen auf der Website und in Anwendungen einsetzbar. Die URL für die Bildgrößenänderung ersetzt den Verweis auf den Namen eines statischen Bildes im Code Ihrer Website. Die URL referenziert einen Masterbildnamen, der über Ihre Datenbank für jedes neue anzuzeigende Bild ersetzt wird.

URL strings generated with Image Presets contain the name of an Image Preset. This name is enclosed in dollar signs (`$`). For example, `$thumbnail$` can be the Image Preset designed to show master images at thumbnail size. Siehe [Verknüpfen von URLs mit einer Web-Anwendung](linking-urls-web-application.md#linking_urls_to_your_web_application).
