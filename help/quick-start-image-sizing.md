---
title: '"Kurzanleitung: Bildgrößenänderung"'
description: Eine Einführung und ein kurzer Beginn zur Bildgrößenänderung helfen Ihnen, sich schnell mit den Bildgrößentechniken vertraut zu machen.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic, Asset Management
role: Business Practitioner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
translation-type: tm+mt
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 35%

---

# Kurzanleitung: Bildgrößenänderung{#quick-start-image-sizing}

Bildgrößenänderung bezieht sich auf die Fähigkeit von Dynamic Media Classic, mehrere abgeleitete Bilder zu erstellen, die auf einem einzigen hochauflösenden Bild basieren. Statt mehrere Bilder - z. B. eine Miniaturansicht und eine vergrößerte Ansicht - für Ihre Website oder Anwendung manuell zu erstellen, stellen Sie ein einzelnes Übergeordnete bereit. Dynamic Media Classic generiert alle bearbeiteten Bilder genau wie gewünscht. Die dynamische Bereitstellung von Bildern basierend auf nur einem Masterbild ist mit zahlreichen Vorteilen verbunden:

* Sie müssen nicht manuell verschiedene Bildversionen in unterschiedlichen Größen erstellen. Sie stellen Dynamic Media Classic ein Übergeordnet Bild zur Verfügung, Dynamic Media Classic generiert aus dem Übergeordnet-Bild verschiedene Ableitungen.
* Sie können schnell die Größe für einen bestimmten Bildtyp in der gesamten Website bzw. Anwendung ändern. Möchten Sie beispielsweise alle Miniaturansichten ändern, bearbeiten Sie dazu die Bildvorgabe „Miniaturansicht“. Eine Bildvorgabe ähnelt einem Makro – mehrere Attribute für Größe und Formatierung sind darin gesammelt. Sie können die Bildvorgabe „Miniaturansicht“ bearbeiten, um die Größe aller in der Website bzw. Anwendung vorhandenen Miniaturansichten zu ändern.
* Sie müssen die Master und alle verschiedenen Derivate in keinem Ihrer Content- oder Asset-Management-Systeme intern oder extern verwalten.

![Sie können mehrere abgeleitete Bilder in unterschiedlicher Größe aus derselben hochauflösenden Übergeordnet-Datei erstellen.](/help/assets/is_derivative_sizes_popup.png)

Dieser Beginn zur Bildgrößenänderung hilft Ihnen, sich schnell mit den Bildgrößentechniken in Dynamic Media Classic vertraut zu machen. Führen Sie die Schritte 1-5 aus. Nach jedem Schritt wird auf ein Thema mit weiteren Informationen verwiesen.

## 1. Hochladen von Übergeordnet erstellten Bildern

Beginn durch Hochladen der Übergeordnet erstellten Bilder in Dynamic Media Classic. Was die Größe anbelangt, empfiehlt Dynamic Media Classic die Verwendung von Bildern, die die größte Größe haben, die Sie auf Ihrer Website oder in Ihrer Anwendung erwarten. Wenn Sie beispielsweise möchten, dass Viewer Bilder heranzoomen, laden Sie Bilder hoch, deren Größe mindestens 2000 Pixel beträgt. Dynamic Media Classic unterstützt viele Bilddateiformate, es werden jedoch verlustfreie TIFF- und PNG-Bilder empfohlen.

Klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Hochladen]**, um Dateien von Ihrem Computer in einen Ordner in Dynamic Media Classic hochzuladen. Siehe [Hochladen von Masterbildern](uploading-master-images.md#uploading_master_images).

## 2. Einstellen von Bildvorgaben

Ähnlich wie bei einem Makro sind in einer Bildvorgabe vordefinierte Größen- und Formatierungsbefehle unter einem gemeinsamen Namen gespeichert. Eine Bildvorgabe regelt die Größe und Formatierung, mit der Bilder von Dynamic Media-Image-Servern bereitgestellt werden. Wenn Sie den Status eines Unternehmensadministrators haben, können Sie Bildvorgaben selbst anlegen. Im Lieferumfang von Dynamic Media Classic sind auch Standard-Bildvorgaben enthalten, mit denen Sie Bilder dynamisch bereitstellen können.

Um eine Bildvorgabe zu erstellen (wenn Sie Administrator sind), klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Bildvorgaben]**. Klicken Sie dann auf **[!UICONTROL Hinzufügen]**, um eine Bildvorgabe zu erstellen, oder klicken Sie auf **[!UICONTROL Bearbeiten]**, um eine vorhandene Bildvorgabe zu ändern.

Die von Ihnen erstellte Bildvorgabe wird dem Menü &quot;Bildvorgabe&quot;auf der Seite &quot;Vorschau&quot;hinzugefügt. Mithilfe der neuen Bildvorgabe können Sie Bilder auf Ihren Websites und in Ihren Anwendungen dynamisch anzeigen. Siehe [Einstellen von Bildvorgaben](setting-image-presets.md#setting_up_image_presets).

## 3. Anzeigen einer Vorschau für Bildvorgaben

Der nächste Schritt besteht im Anzeigen einer Vorschau der Bildvorgaben, die Ihr Administrator für die unterschiedlichen vorgegebenen Größen eingestellt hat. 

Um Bildvorgaben zu untersuchen, klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Bildvorgaben]** und navigieren Sie dann zu einer Bildvorgabe.

Experimentieren Sie mit verschiedenen Bildvorgaben. Finden Sie heraus, wie das Bild angezeigt wird, wenn es dynamisch in unterschiedlichen Größen für Ihre Website oder Anwendung bereitgestellt wird.

Siehe [Anzeigen eines Bild-Asset auf Grundlage seiner Bildvorgabe](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4. Veröffentlichen von Übergeordnet erstellten Bildern

Das Veröffentlichen Ihrer Masterbilddateien hat zwei wichtige Auswirkungen:

* Veröffentlichen von Übergeordnet erstellten Bildern auf Dynamic Media-Image-Servern, damit die Bilder dynamisch an Ihre Website und Anwendung übertragen werden können.
* Beim Veröffentlichen werden die URL-Zeichenfolgen aktiviert, mit denen Bilder von den Dynamic Media-Image-Servern für Ihre Website oder Anwendung aufgerufen werden können. Nach der Veröffentlichung können Sie die von Dynamic Media Classic generierten URLs kopieren und gegebenenfalls in Ihre Website oder Anwendung einfügen.

Klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Veröffentlichen]**, um einen Veröffentlichungsauftrag Beginn. Klicken Sie im Dialogfeld &quot;Veröffentlichen&quot;auf **[!UICONTROL Veröffentlichen senden]**. Siehe [Veröffentlichen von Masterbildern](publishing-master-images.md#publishing_master_images).

## 5. Verknüpfen von URLs mit einer Webanwendung

Dynamic Media Classic erstellt URL-Zeichenfolgen zum Aufrufen von Bildern. Wenn Sie Bilder auf Dynamic Media-Image-Servern veröffentlichen, werden die URLs aktiv. Sie können diese URL-Zeichenfolgen vom Durchsuchenbedienfeld (in der Detailansicht) oder vom Anzeigebereich „Vorschau“ aus kopieren. Nach dem Kopieren sind die URL-Zeichenfolgen auf der Website und in Anwendungen einsetzbar. Die URL für die Bildgrößenänderung ersetzt den Verweis auf den Namen eines statischen Bildes im Code Ihrer Website. Die URL referenziert einen Masterbildnamen, der über Ihre Datenbank für jedes neue anzuzeigende Bild ersetzt wird.

Mit Bildvorgaben generierte URL-Zeichenfolgen enthalten den Namen einer Bildvorgabe. Dieser Name ist in Dollarzeichen (`$`) eingeschlossen. Beispielsweise kann `$thumbnail$` die Bildvorgabe sein, mit der Übergeordnet Bilder in Miniaturansicht angezeigt werden. Siehe [Verknüpfen von URLs mit einer Web-Anwendung](linking-urls-web-application.md#linking_urls_to_your_web_application).
