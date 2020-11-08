---
title: '"Kurzanleitung: Bildgrößenänderung"'
seo-title: '"Kurzanleitung: Bildgrößenänderung"'
description: 'null'
seo-description: Eine Einführung und ein kurzer Beginn zur Bildgrößenänderung helfen Ihnen, sich schnell mit den Bildgrößentechniken vertraut zu machen.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 54%

---


# Kurzanleitung: Bildgrößenänderung{#quick-start-image-sizing}

Die Bildgrößenänderung bezieht sich auf die Fähigkeit von Dynamic Media Classic, mehrere abgeleitete Bilder zu erstellen, die auf einem einzigen hochauflösenden Bild basieren. Statt mehrere Bilder - z. B. eine Miniaturansicht und eine vergrößerte Ansicht - für Ihre Website oder Anwendung manuell zu erstellen, stellen Sie ein einzelnes Übergeordnete bereit. Dynamic Media Classic generiert alle geänderten Bilder genau wie bei Anforderung. Die dynamische Bereitstellung von Bildern basierend auf nur einem Masterbild ist mit zahlreichen Vorteilen verbunden:

* Sie müssen nicht manuell verschiedene Bildversionen in unterschiedlichen Größen erstellen. Dynamische Medien-Classic liefert ein Übergeordnet-Bild und Dynamic Media Classic erzeugt aus dem Übergeordnet-Bild in unterschiedlicher Größe Ableitungen.
* Sie können schnell die Größe für einen bestimmten Bildtyp in der gesamten Website bzw. Anwendung ändern. Möchten Sie beispielsweise alle Miniaturansichten ändern, bearbeiten Sie dazu die Bildvorgabe „Miniaturansicht“. Eine Bildvorgabe ähnelt einem Makro – mehrere Attribute für Größe und Formatierung sind darin gesammelt. Sie können die Bildvorgabe „Miniaturansicht“ bearbeiten, um die Größe aller in der Website bzw. Anwendung vorhandenen Miniaturansichten zu ändern.
* Es ist nicht erforderlich, die Masterversionen und sämtliche verschiedenen Ableitungen mit Content-Management- oder Asset-Management-Systemen intern oder extern zu verwalten.

![Sie können mehrere abgeleitete Bilder in unterschiedlicher Größe aus derselben hochauflösenden Übergeordnet-Datei erstellen.](/help/assets/is_derivative_sizes_popup.png)

**Quick Beginn**

Dieser Beginn zur Bildgrößenänderung hilft Ihnen, sich schnell mit den Bildgrößentechniken in Dynamic Media Classic vertraut zu machen. Führen Sie die Schritte 1-5 aus. Nach jedem Schritt wird auf ein Thema mit weiteren Informationen verwiesen.

**1. Hochladen von Masterbildern**

Beginn durch Hochladen der Übergeordnet erstellten Bilder in Dynamic Media Classic. Was die Größe betrifft, empfiehlt Dynamic Media Classic die Verwendung von Bildern mit der größten erwarteten Größe auf Ihrer Website oder in Ihrer Anwendung. Möchten Sie beispielsweise, dass Betrachter die Bilder per Zoom vergrößern können, sollten Sie Bilder hochladen, deren längste Abmessung (Breite oder Höhe) mindestens 2000 Pixel beträgt. Dynamic Media Classic unterstützt viele Bilddateiformate, es werden jedoch verlustfreie TIFF- und PNG-Bilder empfohlen.

Klicken Sie in der Symbolleiste für globale Navigation auf die Schaltfläche &quot;Hochladen&quot;, um Dateien von Ihrem Computer in einen Ordner unter &quot;Dynamische Medien - Classic&quot;hochzuladen. Siehe [Hochladen von Masterbildern](uploading-master-images.md#uploading_master_images).

**2. Einstellen von Bildvorgaben**

Ähnlich wie bei einem Makro sind in einer Bildvorgabe vordefinierte Größen- und Formatierungsbefehle unter einem gemeinsamen Namen gespeichert. Eine Bildvorgabe bestimmt die Größe und Formatierung, mit der Bilder von dynamischen Medienbildern bereitgestellt werden. Wenn Sie den Status eines Unternehmensadministrators haben, können Sie Bildvorgaben selbst anlegen. Im Lieferumfang von Dynamic Media Classic sind auch Standard-Bildvorgaben enthalten, mit denen Sie Bilder dynamisch bereitstellen können.

Um als Administrator eine Bildvorgabe zu erstellen, wählen Sie „Einstellungen“ > „Anwendungseinstellungen“. Blenden Sie im Anzeigebereich „Einstellungen“ die Optionen für „Anwendungseinstellungen“ ein und wählen Sie „Bildvorgaben“. Klicken Sie dann auf **Hinzufügen** oder **Bearbeiten** , um eine Bildvorgabe zu erstellen.

Die von Ihnen erstelle Bildvorgabe wird im Anzeigebereich „Vorschau“ in das Menü „Bildvorgabe“ eingefügt. Mithilfe der neuen Bildvorgabe können Sie Bilder auf Ihren Websites und in Ihren Anwendungen dynamisch anzeigen. Siehe [Einstellen von Bildvorgaben](setting-image-presets.md#setting_up_image_presets).

**3. Anzeigen einer Vorschau für Bildvorgaben**

Der nächste Schritt besteht im Anzeigen einer Vorschau der Bildvorgaben, die Ihr Administrator für die unterschiedlichen vorgegebenen Größen eingestellt hat. 

To explore Image Presets, click **Setup** > **Image Presets**, and then browse to an Image Preset.

Experimentieren Sie mit verschiedenen Bildvorgaben. Finden Sie heraus, wie sich die dynamische Ausgabe in verschiedenen Größen auf Ihrer Website bzw. in Ihrer Anwendung auswirkt. 

Siehe [Anzeigen eines Bild-Asset auf Grundlage seiner Bildvorgabe](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

**4. Veröffentlichen von Masterbildern**

Das Veröffentlichen Ihrer Masterbilddateien hat zwei wichtige Auswirkungen:

* Veröffentlichen von Übergeordnet erstellten Bildern auf Dynamic Media-Image-Servern, damit die Bilder dynamisch an Ihre Website und Anwendung übertragen werden können.
* Beim Veröffentlichen werden die URL-Zeichenfolgen aktiviert, mit denen Bilder von den Image-Servern für dynamische Medien auf Ihrer Website oder in Ihrer Anwendung aufgerufen werden können. Nach der Veröffentlichung können Sie die von Dynamic Media Classic generierten URLs kopieren und gegebenenfalls in Ihre Website oder Anwendung einfügen.

Klicken Sie auf der Symbolleiste für globale Navigation auf die Schaltfläche „Veröffentlichen“, um einen Veröffentlichungsvorgang einzuleiten. Klicken Sie im Anzeigebereich „Veröffentlichen“ auf die Schaltfläche „Veröffentlichungsvorgang starten“. Siehe [Veröffentlichen von Masterbildern](publishing-master-images.md#publishing_master_images).

**5. Verknüpfen von URLs mit einer Web-Anwendung**

Dynamic Media Classic erstellt URL-Zeichenfolgen zum Aufrufen von Bildern. Wenn Sie Bilder auf den Image-Servern für dynamische Medien veröffentlichen, werden die URLs aktiv. Sie können diese URL-Zeichenfolgen vom Durchsuchenbedienfeld (in der Detailansicht) oder vom Anzeigebereich „Vorschau“ aus kopieren. Nach dem Kopieren sind die URL-Zeichenfolgen auf der Website und in Anwendungen einsetzbar. Die URL für die Bildgrößenänderung ersetzt den Verweis auf den Namen eines statischen Bildes im Code Ihrer Website. Die URL referenziert einen Masterbildnamen, der über Ihre Datenbank für jedes neue anzuzeigende Bild ersetzt wird.

URL strings generated with Image Presets contain the name of an Image Preset. This name is enclosed in dollar signs (`$`). For example, `$thumbnail$` can be the Image Preset designed to show master images at thumbnail size. Siehe [Verknüpfen von URLs mit einer Web-Anwendung](linking-urls-web-application.md#linking_urls_to_your_web_application).
