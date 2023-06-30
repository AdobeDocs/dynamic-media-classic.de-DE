---
title: "Kurzanleitung: Bildgrößenänderung"
description: Eine Einführung und ein Schnellstart zur Bildgröße, damit Sie in Adobe Dynamic Media Classic schnell mit den Bildgrößetechniken arbeiten können.
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
topic: Content Management
level: Beginner
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 21%

---

# Kurzanleitung: Bildgrößenänderung{#quick-start-image-sizing}

Bildgröße bezieht sich auf die Fähigkeit von Adobe Dynamic Media Classic, mehrere abgeleitete Bilder basierend auf einem einzigen hochauflösenden Bild zu erstellen. Anstatt für Ihre Website oder Anwendung mehrere Bilder - z. B. eine Miniaturansicht und ein vergrößertes Bild - manuell zu erstellen, geben Sie ein einziges primäres Bild an. Adobe Dynamic Media Classic generiert alle geänderten Bilder auf die gleiche Weise wie Sie sie anfordern. Die Möglichkeit, Bilder dynamisch aus einem einzigen primären Bild bereitzustellen, bietet viele Vorteile:

* Sie müssen nicht manuell verschiedene Bildversionen in unterschiedlichen Größen erstellen. Sie stellen ein Primärbild für Adobe Dynamic Media Classic bereit und Adobe Dynamic Media Classic generiert aus dem Primärbild verschiedene Varianten.
* Sie können schnell die Größe für einen bestimmten Bildtyp in der gesamten Website bzw. Anwendung ändern. Möchten Sie beispielsweise alle Miniaturansichten ändern, bearbeiten Sie dazu die Bildvorgabe „Miniaturansicht“. Eine Bildvorgabe ähnelt einem Makro – mehrere Attribute für Größe und Formatierung sind darin gesammelt. Sie können die Bildvorgabe „Miniaturansicht“ bearbeiten, um die Größe aller in der Website bzw. Anwendung vorhandenen Miniaturansichten zu ändern.
* Sie müssen die Primärdateien und alle verschiedenen Derivate in keinem Ihrer Inhalts- oder Asset-Management-Systeme intern oder extern verwalten.

![Sie können mehrere abgeleitete Bilder mit unterschiedlicher Größe aus derselben hochauflösenden Primärdatei erstellen.](/help/using/assets/is_derivative_sizes_popup.png)

Siehe [Bildgröße: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) Schulungsvideo.

Der folgende Schnellstart zur Bilddimensionierung soll Ihnen dabei helfen, die Bilddimensionierungsmethoden in Adobe Dynamic Media Classic schnell einzurichten und auszuführen. Führen Sie die Schritte 1 bis 5 aus. Nach jedem Schritt gibt es einen Querverweis, über den Sie bei Bedarf weitere Informationen finden können.

## 1. Hochladen von Primärbildern

Laden Sie zunächst Ihre Primärbilder in Adobe Dynamic Media Classic hoch. Was die Größe angeht, empfiehlt Adobe Dynamic Media Classic die Verwendung von Bildern, die die größte Größe aufweisen, die Sie auf Ihrer Website oder in Ihrer Anwendung erwarten. Wenn Sie beispielsweise möchten, dass Betrachter Bilder zoomen, laden Sie Bilder hoch, die mindestens 2000 Pixel in der größten Größe aufweisen. Adobe Dynamic Media Classic unterstützt viele Bilddateiformate, es werden jedoch verlustfreie TIFF- und PNG-Bilder empfohlen.

Wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Hochladen]** , um Dateien von Ihrem Computer in einen Ordner in Adobe Dynamic Media Classic hochzuladen. Siehe [Hochladen von Primärbildern](uploading-master-images.md#uploading_master_images).

## 2. Einrichten von Bildvorgaben

Ähnlich wie bei einem Makro sind in einer Bildvorgabe vordefinierte Größen- und Formatierungsbefehle unter einem gemeinsamen Namen gespeichert. Eine Bildvorgabe legt die Größe und Formatierung fest, mit der Bilder von Dynamic Media-Bildservern bereitgestellt werden. Wenn Sie den Status eines Unternehmensadministrators haben, können Sie Bildvorgaben selbst anlegen. Adobe Dynamic Media Classic enthält auch standardmäßige Bildvorgaben, die Sie verwenden können, um Bilder dynamisch bereitzustellen.

Um eine Bildvorgabe zu erstellen (falls Sie Administrator sind), navigieren Sie in der Symbolleiste für globale Navigation zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Bildvorgaben]**. Wählen Sie anschließend **[!UICONTROL Hinzufügen]** , um eine Bildvorgabe zu erstellen, oder wählen Sie **[!UICONTROL Bearbeiten]** , um eine vorhandene Bildvorgabe zu ändern.

Die von Ihnen erstellte Bildvorgabe wird dem Menü Bildvorgabe auf der Seite Vorschau hinzugefügt. Mithilfe der neuen Bildvorgabe können Sie Bilder auf Ihren Websites und in Ihren Anwendungen dynamisch anzeigen. Siehe [Einrichten von Bildvorgaben](setting-image-presets.md#setting_up_image_presets).

## 3. Bildvorgaben in der Vorschau anzeigen

Der nächste Schritt besteht im Anzeigen einer Vorschau der Bildvorgaben, die Ihr Administrator für die unterschiedlichen vorgegebenen Größen eingestellt hat. 

Um Bildvorgaben zu erforschen, navigieren Sie in der Symbolleiste für globale Navigation zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Bildvorgaben]** und navigieren Sie dann zu einer Bildvorgabe.

Experimentieren Sie mit verschiedenen Bildvorgaben. Erfahren Sie, wie Ihr Bild angezeigt wird, wenn es dynamisch auf Ihrer Website oder in Ihrer Anwendung mit unterschiedlichen Größen bereitgestellt wird.

Siehe [Vorschau eines Bild-Assets basierend auf seiner Bildvorgabe](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4. Veröffentlichen Sie die Primärbilder

Die Veröffentlichung Ihrer Primärbilddateien dient zwei wichtigen Zwecken:

* Veröffentlichen Sie die Primärbilder auf Dynamic Media-Image-Servern, damit Bilder dynamisch für Ihre Website und Anwendung bereitgestellt werden können.
* Beim Veröffentlichen werden die URL-Zeichenfolgen aktiviert, mit denen Bilder von Dynamic Media-Bildservern auf Ihrer Website oder in Ihrer Anwendung aufgerufen werden können. Nach der Veröffentlichung können Sie die von Adobe Dynamic Media Classic generierten URLs kopieren und gegebenenfalls in Ihre Website oder Anwendung einfügen.

Wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Veröffentlichen]** , um einen Veröffentlichungsauftrag zu starten. Wählen Sie im Dialogfeld Veröffentlichen die Option **[!UICONTROL Veröffentlichung übermitteln]**. Siehe [Primärbilder veröffentlichen](publishing-master-images.md#publishing_master_images).

## 5. Verknüpfen von URLs mit einer Webanwendung

Adobe Dynamic Media Classic erstellt URL-Zeichenfolgen für die Bildberechnung. Wenn Sie Bilder auf Dynamic Media-Bildservern veröffentlichen, werden die URLs aktiv. Sie können diese URL-Zeichenfolgen aus dem Durchsuchenbedienfeld (in der Detailansicht) oder dem Vorschaubildschirm kopieren. Nach dem Kopieren sind die URL-Zeichenfolgen auf der Website und in Anwendungen einsetzbar. Die URL für die Bildgrößenänderung ersetzt den Verweis auf den Namen eines statischen Bildes im Code Ihrer Website. Die URL verweist auf einen primären Bildnamen, der durch Ihre Datenbank ersetzt wird, damit jedes neue Bild angezeigt wird.

Mit Bildvorgaben generierte URL-Zeichenfolgen enthalten den Namen einer Bildvorgabe. Dieser Name ist in Dollarzeichen (`$`). Beispiel: `$thumbnail$` kann die Bildvorgabe sein, mit der Primärbilder in der Größe der Miniaturansichten angezeigt werden. Siehe [Verknüpfen von URLs mit einer Webanwendung](linking-urls-web-application.md#linking_urls_to_your_web_application).
