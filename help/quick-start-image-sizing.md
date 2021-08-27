---
title: '"Kurzanleitung: Bildgrößenänderung"'
description: Eine Einführung und ein Schnellstart zur Bildgröße, damit Sie schnell mit den Bildgrößetechniken arbeiten können.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 33%

---

# Kurzanleitung: Bildgrößenänderung{#quick-start-image-sizing}

Bildgröße bezieht sich auf die Möglichkeit von Adobe Dynamic Media Classic, mehrere abgeleitete Bilder basierend auf einem einzigen hochauflösenden Bild zu erstellen. Anstatt für Ihre Website oder Anwendung mehrere Bilder - z. B. eine Miniaturansicht und ein vergrößertes Bild - manuell zu erstellen, stellen Sie ein einziges Übergeordnetes Bild bereit. Adobe Dynamic Media Classic generiert alle geänderten Bilder auf die gleiche Weise wie Sie sie anfordern. Die dynamische Bereitstellung von Bildern basierend auf nur einem Masterbild ist mit zahlreichen Vorteilen verbunden:

* Sie müssen nicht manuell verschiedene Bildversionen in unterschiedlichen Größen erstellen. Sie stellen ein Übergeordnetes Bild für Adobe Dynamic Media Classic bereit und Adobe Dynamic Media Classic generiert aus dem Übergeordneten Bild verschiedene Varianten.
* Sie können schnell die Größe für einen bestimmten Bildtyp in der gesamten Website bzw. Anwendung ändern. Möchten Sie beispielsweise alle Miniaturansichten ändern, bearbeiten Sie dazu die Bildvorgabe „Miniaturansicht“. Eine Bildvorgabe ähnelt einem Makro – mehrere Attribute für Größe und Formatierung sind darin gesammelt. Sie können die Bildvorgabe „Miniaturansicht“ bearbeiten, um die Größe aller in der Website bzw. Anwendung vorhandenen Miniaturansichten zu ändern.
* Sie müssen die Master und alle verschiedenen Derivate in keinem Ihrer Inhalts- oder Asset-Management-Systeme intern oder extern verwalten.

![Sie können mehrere abgeleitete Bilder mit unterschiedlicher Größe aus derselben hochauflösenden Übergeordneten Datei erstellen.](/help/assets/is_derivative_sizes_popup.png)

Diese Kurzanleitung zur Bilddimensionierung soll Ihnen dabei helfen, die Bildgrößentechniken in Adobe Dynamic Media Classic einzurichten und schnell auszuführen. Führen Sie die Schritte 1 bis 5 aus. Nach jedem Schritt wird auf ein Thema mit weiteren Informationen verwiesen.

## 1. Hochladen Übergeordneter Bilder

Laden Sie zunächst Ihre Übergeordneten Bilder in Adobe Dynamic Media Classic hoch. Was die Größe anbelangt, empfiehlt Adobe Dynamic Media Classic die Verwendung von Bildern, die die größte Bildgröße aufweisen, die Sie auf Ihrer Website oder in Ihrer Anwendung erwarten. Wenn Sie beispielsweise möchten, dass Betrachter Bilder zoomen, laden Sie Bilder hoch, die mindestens 2000 Pixel in der größten Größe aufweisen. Adobe Dynamic Media Classic unterstützt viele Bilddateiformate, es werden jedoch verlustfreie TIFF- und PNG-Bilder empfohlen.

Klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Upload]** , um Dateien von Ihrem Computer in einen Ordner auf Adobe Dynamic Media Classic hochzuladen. Siehe [Hochladen von Masterbildern](uploading-master-images.md#uploading_master_images).

## 2. Einrichten von Bildvorgaben

Ähnlich wie bei einem Makro sind in einer Bildvorgabe vordefinierte Größen- und Formatierungsbefehle unter einem gemeinsamen Namen gespeichert. Eine Bildvorgabe legt die Größe und Formatierung fest, mit der Bilder von Dynamic Media-Bildservern bereitgestellt werden. Wenn Sie den Status eines Unternehmensadministrators haben, können Sie Bildvorgaben selbst anlegen. Adobe Dynamic Media Classic enthält auch standardmäßige Bildvorgaben, die Sie verwenden können, um Bilder dynamisch bereitzustellen.

Um eine Bildvorgabe zu erstellen (wenn Sie Administrator sind), klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Bildvorgaben]**. Klicken Sie dann auf **[!UICONTROL Hinzufügen]** , um eine Bildvorgabe zu erstellen, oder klicken Sie auf **[!UICONTROL Bearbeiten]** , um eine vorhandene Bildvorgabe zu ändern.

Die von Ihnen erstellte Bildvorgabe wird dem Menü Bildvorgabe auf der Seite Vorschau hinzugefügt. Mithilfe der neuen Bildvorgabe können Sie Bilder auf Ihren Websites und in Ihren Anwendungen dynamisch anzeigen. Siehe [Einstellen von Bildvorgaben](setting-image-presets.md#setting_up_image_presets).

## 3. Anzeigen einer Vorschau für Bildvorgaben

Der nächste Schritt besteht im Anzeigen einer Vorschau der Bildvorgaben, die Ihr Administrator für die unterschiedlichen vorgegebenen Größen eingestellt hat. 

Um Bildvorgaben zu untersuchen, klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Setup]** > **[!UICONTROL Bildvorgaben]** und navigieren Sie dann zu einer Bildvorgabe.

Experimentieren Sie mit verschiedenen Bildvorgaben. Erfahren Sie, wie Ihr Bild angezeigt wird, wenn es dynamisch auf Ihrer Website oder in Ihrer Anwendung mit unterschiedlichen Größen bereitgestellt wird.

Siehe [Anzeigen eines Bild-Asset auf Grundlage seiner Bildvorgabe](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4. Übergeordnete Bilder veröffentlichen

Das Veröffentlichen Ihrer Masterbilddateien hat zwei wichtige Auswirkungen:

* Veröffentlichen Sie Ihre Übergeordneten Bilder auf Dynamic Media-Image-Servern, damit Bilder dynamisch für Ihre Website und Anwendung bereitgestellt werden können.
* Beim Veröffentlichen werden die URL-Zeichenfolgen aktiviert, mit denen Bilder von Dynamic Media-Bildservern auf Ihrer Website oder in Ihrer Anwendung aufgerufen werden können. Nach der Veröffentlichung können Sie die von Dynamic Media Classic generierten URLs kopieren und platzieren, wo dies für Ihre Website oder Anwendung erforderlich ist.

Klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Veröffentlichen]** , um einen Veröffentlichungsauftrag zu starten. Klicken Sie im Dialogfeld &quot;Veröffentlichen&quot;auf **[!UICONTROL Veröffentlichen senden]**. Siehe [Veröffentlichen von Masterbildern](publishing-master-images.md#publishing_master_images).

## 5. Verknüpfen von URLs mit einer Webanwendung

Adobe Dynamic Media Classic erstellt URL-Hinweisseiten für Bilder. Wenn Sie Bilder auf Dynamic Media-Bildservern veröffentlichen, werden die URLs aktiv. Sie können diese URL-Zeichenfolgen aus dem Durchsuchenbedienfeld (in der Detailansicht) oder dem Vorschaubildschirm kopieren. Nach dem Kopieren sind die URL-Zeichenfolgen auf der Website und in Anwendungen einsetzbar. Die URL für die Bildgrößenänderung ersetzt den Verweis auf den Namen eines statischen Bildes im Code Ihrer Website. Die URL referenziert einen Masterbildnamen, der über Ihre Datenbank für jedes neue anzuzeigende Bild ersetzt wird.

Mit Bildvorgaben generierte URL-Zeichenfolgen enthalten den Namen einer Bildvorgabe. Dieser Name ist in Dollarzeichen (`$`) eingeschlossen. Beispielsweise kann `$thumbnail$` die Bildvorgabe sein, die Übergeordnete Bilder in der Größe der Miniaturansichten anzeigt. Siehe [Verknüpfen von URLs mit einer Web-Anwendung](linking-urls-web-application.md#linking_urls_to_your_web_application).
