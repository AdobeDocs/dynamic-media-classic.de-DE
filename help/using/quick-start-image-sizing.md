---
title: 'Kurzanleitung: Bildgrößenänderung'
description: Eine Einführung und eine Kurzanleitung zur Bildgröße, damit Sie die Verfahren zur Bildgröße in Adobe Dynamic Media Classic schnell einrichten und ausführen können.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
topic: Content Management
level: Beginner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
autotag-review: '2026-05-13T20:09:57.533Z'
TQID: 'https://experienceleague.adobe.com/VGp4OQ03iRiobXKWuUERNtFwUMQ4z7a19wyOgHWuv3w'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 202f477d78272c66d0ac490e3a5041839b3e4f4d
workflow-type: tm+mt
source-wordcount: 870
ht-degree: 5%

---

# Kurzanleitung: Bildgrößenänderung{#quick-start-image-sizing}

Bildgröße bezieht sich auf die Fähigkeit von Adobe Dynamic Media Classic, mehrere abgeleitete Bilder basierend auf einem einzelnen hochauflösenden Bild zu erstellen. Anstatt mehrere Bilder für Ihre Website oder Ihr Programm manuell zu erstellen, stellen Sie ein einzelnes primäres Bild bereit. Adobe Dynamic Media Classic generiert alle geänderten Bilder, wenn Sie sie anfordern. Die dynamische Bereitstellung von Bildern aus einem einzelnen primären Bild bietet viele Vorteile:

* Das manuelle Erstellen mehrerer Kopien des Bildes in verschiedenen Größen ist nicht erforderlich. Sie stellen Adobe Dynamic Media Classic ein Primärbild zur Verfügung und es generiert Ableitungen unterschiedlicher Größe vom Primärbild.
* Sie können die Größe eines Bildes auf Ihrer Website oder in Ihrem Programm schnell ändern. Um beispielsweise alle Miniaturen zu ändern, können Sie die Bildvorgabe „Miniatur“ ändern. Eine Bildvorgabe ist eine Sammlung von Größenattributen und Formatierungsattributen. Um die Größe aller Miniaturbilder auf Ihrer Website oder in Ihrer Anwendung zu ändern, können Sie die Bildvorgabe „Miniaturansicht“ ändern.
* Sie müssen die Primärdateien oder alle Ableitungen in keinem Ihrer Content- oder Asset-Management-Systeme verwalten.

![Sie können mehrere abgeleitete Bilder mit unterschiedlicher Größe aus derselben hochauflösenden Primärdatei erstellen](/help/using/assets/is_derivative_sizes_popup.png).

Siehe [Bildgröße: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) Schulungsvideo.

Der folgende Schnellstart zur Bildgröße soll Ihnen dabei helfen, in Adobe Dynamic Media Classic mit der Verwendung von Verfahren zur Bildgröße zu beginnen. Führen Sie die Schritte 1 bis 5 aus. Nach jedem Schritt gibt es einen Querverweis, in dem Sie weitere Informationen finden können, falls Sie sie benötigen.

## &#x200B;1. Primäre Bilder hochladen

Laden Sie die Primärbilder in Adobe Dynamic Media Classic hoch. Adobe Dynamic Media Classic empfiehlt, Bilder zu verwenden, die die maximale Größe aufweisen, die Sie auf Ihrer Website oder in Ihrem Programm erwarten. Wenn Sie beispielsweise möchten, dass Betrachter Bilder zoomen, laden Sie Bilder mit einer Größe von mindestens 2.000 Pixel hoch. Adobe Dynamic Media Classic unterstützt viele Bilddateiformate, empfohlen werden jedoch verlustfreie TIFF- und PNG-Bilder.

Wählen Sie in der globalen Navigationsleiste **[!UICONTROL Hochladen]** aus, um Dateien von Ihrem Computer in einen Ordner in Adobe Dynamic Media Classic hochzuladen. Siehe [Hochladen primärer Bilder](uploading-master-images.md#uploading_master_images).

## &#x200B;2. Konfigurieren von Bildvorgaben

Eine Bildvorgabe ist eine Sammlung vordefinierter Befehle für Größe und Formatierung, die unter einem Namen gespeichert wird. Eine Bildvorgabe legt die Größe und Formatierung fest, mit der Bilder von Dynamic Media-Bildservern bereitgestellt werden. Sie können Bildvorgaben unabhängig konfigurieren, wenn Sie den Status „Unternehmensadministrator“ haben. Sie können Bilder mithilfe der in Adobe Dynamic Media Classic enthaltenen Standardbildvorgaben dynamisch bereitstellen.

Wenn Sie eine Bildvorgabe erstellen möchten (wenn Sie Administrator sind), klicken Sie in der globalen Navigationsleiste auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Bildvorgaben]**. Klicken Sie dann auf **[!UICONTROL Hinzufügen]**, um eine Bildvorgabe zu erstellen, oder klicken Sie auf **[!UICONTROL Bearbeiten]**, um eine vorhandene Bildvorgabe zu ändern.

Die erstellte Bildvorgabe wird dem Menü Bildvorgabe auf der Seite Vorschau hinzugefügt. Mithilfe der neuen Bildvorgabe können Sie Bilder auf Ihren Websites und in Ihren Anwendungen dynamisch anzeigen. Siehe [Einrichten von ](setting-image-presets.md#setting_up_image_presets).

## &#x200B;3. Vorschau von Bildvorgaben

Der nächste Schritt besteht im Anzeigen einer Vorschau der Bildvorgaben, die Ihr Administrator für die unterschiedlichen vorgegebenen Größen eingestellt hat.

Bildvorgaben finden Sie in der globalen Navigationsleiste unter **[!UICONTROL Einstellungen]** > **[!UICONTROL Bildvorgaben]** und navigieren Sie dann zu einer Bildvorgabe.

Testen Sie die verschiedenen Bildvorgaben. Legen Sie fest, wie das Bild angezeigt wird, wenn es dynamisch auf Ihrer Website oder in Ihrem Programm in unterschiedlichen Größen bereitgestellt wird.

Siehe [Vorschau eines Bild-Assets basierend auf seiner Bildvorgabe](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## &#x200B;4. Veröffentlichen der primären Bilder

Die Veröffentlichung Ihrer primären Bilddateien dient zwei wichtigen Zwecken:

* Veröffentlichen Sie Ihre primären Bilder auf Dynamic Media-Bildservern, damit Bilder dynamisch für Ihre Website und Ihr Programm bereitgestellt werden können.
* Beim Veröffentlichen werden die URL-Zeichenfolgen zum Aufrufen von Bildern von Dynamic Media-Bildservern an Ihre Website oder Anwendung aktiviert. Nach der Veröffentlichung können Sie die von Adobe Dynamic Media Classic generierten URLs kopieren und bei Bedarf in Ihre Website oder Ihr Programm einfügen.

Wählen Sie in der globalen Navigationsleiste die Option **[!UICONTROL Veröffentlichen]**, um einen Veröffentlichungsauftrag zu starten. Wählen Sie im Dialogfeld „Veröffentlichen“ die Option **[!UICONTROL Veröffentlichen starten]**. Siehe [Veröffentlichen primärer Bilder](publishing-master-images.md#publishing_master_images).

## &#x200B;5. Verknüpfen von URLs mit einer Web-Anwendung

Adobe Dynamic Media Classic erstellt URL-Legendenzeichenfolgen für Bilder. Wenn Sie Bilder auf Dynamic Media-Bildservern veröffentlichen, werden die URLs aktiv. Sie können diese URL-Zeichenfolgen aus dem Durchsuchen-Panel (in der Detailansicht) oder dem Bildschirm Vorschau kopieren. Nachdem Sie die URL-Zeichenfolgen kopiert haben, können Sie sie auf Ihrer Website oder in Ihrem Programm verwenden. Die URL für die Bildgröße ersetzt den Verweis auf einen statischen Bildnamen in Ihrem Web-Seiten-Code. Die URL verweist auf einen primären Bildnamen, den die Datenbank für jedes neue angezeigte Bild ersetzt.

Mit Bildvorgaben generierte URL-Zeichenfolgen enthalten den Namen einer Bildvorgabe. Dieser Name ist in Dollarzeichen (`$`) eingeschlossen. Beispielsweise kann `$thumbnail$` die Bildvorgabe sein, die dazu konzipiert ist, primäre Bilder in der Größe von Miniaturansichten anzuzeigen. Siehe [Verknüpfen von URLs mit einer Web-Anwendung](linking-urls-web-application.md#linking_urls_to_your_web_application).
