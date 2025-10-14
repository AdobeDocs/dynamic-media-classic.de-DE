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
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 5%

---

# Kurzanleitung: Bildgrößenänderung{#quick-start-image-sizing}

Bildgröße bezieht sich auf die Fähigkeit von Adobe Dynamic Media Classic, mehrere abgeleitete Bilder basierend auf einem einzelnen hochauflösenden Bild zu erstellen. Anstatt mehrere Bilder für Ihre Website oder Anwendung manuell zu erstellen, z. B. eine Miniaturansicht und ein Bild mit vergrößerter Ansicht, stellen Sie ein einzelnes Primärbild bereit. Adobe Dynamic Media Classic generiert alle geänderten Bilder genau so, wie Sie sie anfordern. Die Möglichkeit, Bilder dynamisch von einem einzelnen primären Bild bereitzustellen, hat viele Vorteile:

* Das manuelle Erstellen mehrerer Kopien des Bildes in verschiedenen Größen ist nicht erforderlich. Sie stellen ein Primärbild für Adobe Dynamic Media Classic bereit, und Adobe Dynamic Media Classic generiert Ableitungen unterschiedlicher Größe vom Primärbild.
* Sie können die Größe eines Bildtyps auf der gesamten Website oder in der Anwendung schnell ändern. Um beispielsweise alle Miniaturen zu ändern, können Sie die Bildvorgabe „Miniatur“ ändern. Eine Bildvorgabe, die einem Makro ähnelt, ist eine Sammlung von Größenattributen und Formatierungsattributen. Sie können die Bildvorgabe „Miniaturansicht“ ändern, um die Größe aller Miniaturbilder auf der gesamten Website oder in der Anwendung zu ändern.
* Sie müssen die Primärdateien und alle Ableitungen in keinem Ihrer Content- oder Asset-Management-Systeme intern oder extern verwalten.

![Sie können mehrere abgeleitete Bilder mit unterschiedlicher Größe aus derselben primären Datei mit hoher Auflösung erstellen.](/help/using/assets/is_derivative_sizes_popup.png)

Siehe [Bildgröße: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) Schulungsvideo.

Die folgende Kurzanleitung zur Bildgröße soll Ihnen den schnellen Einstieg in die Bildgröße in Adobe Dynamic Media Classic erleichtern. Führen Sie die Schritte 1 bis 5 aus. Nach jedem Schritt gibt es einen Querverweis, in dem Sie weitere Informationen finden können, falls Sie sie benötigen.

## &#x200B;1. Hochladen der primären Bilder

Laden Sie zunächst Ihre Primärbilder in Adobe Dynamic Media Classic hoch. Hinsichtlich der Größe empfiehlt Adobe Dynamic Media Classic die Verwendung von Bildern, die die größte Größe aufweisen, die Sie auf Ihrer Website oder in Ihrem Programm erwarten. Wenn Sie beispielsweise möchten, dass Betrachter Bilder zoomen, laden Sie Bilder mit einer Größe von mindestens 2.000 Pixel hoch. Adobe Dynamic Media Classic unterstützt viele Bilddateiformate, empfohlen werden jedoch verlustfreie TIFF- und PNG-Bilder.

Wählen Sie in der globalen Navigationsleiste **[!UICONTROL Hochladen]** aus, um Dateien von Ihrem Computer in einen Ordner in Adobe Dynamic Media Classic hochzuladen. Siehe [Hochladen primärer Bilder](uploading-master-images.md#uploading_master_images).

## &#x200B;2. Einrichten von Bildvorgaben

Ähnlich wie bei einem Makro sind in einer Bildvorgabe vordefinierte Größen- und Formatierungsbefehle unter einem gemeinsamen Namen gespeichert. Eine Bildvorgabe legt die Größe und Formatierung fest, mit der Bilder von Dynamic Media-Bildservern bereitgestellt werden. Sie können Bildvorgaben selbst einrichten, wenn Sie den Status „Unternehmensadministrator“ haben. Sie können Bilder dynamisch mit den bereits in Adobe Dynamic Media Classic bereitgestellten Standardbildvorgaben bereitstellen.

Wenn Sie eine Bildvorgabe erstellen möchten (wenn Sie Administrator sind), klicken Sie in der globalen Navigationsleiste auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Bildvorgaben]**. Klicken Sie dann auf **[!UICONTROL Hinzufügen]**, um eine Bildvorgabe zu erstellen, oder klicken Sie auf **[!UICONTROL Bearbeiten]**, um eine vorhandene Bildvorgabe zu ändern.

Die erstellte Bildvorgabe wird dem Menü Bildvorgabe auf der Seite Vorschau hinzugefügt. Sie können Ihre neue Bildvorgabe verwenden, um Bilder auf Ihren Websites und in Anwendungen dynamisch anzuzeigen. Siehe [Einrichten von &#x200B;](setting-image-presets.md#setting_up_image_presets).

## &#x200B;3. Vorschau von Bildvorgaben

Der nächste Schritt besteht im Anzeigen einer Vorschau der Bildvorgaben, die Ihr Administrator für die unterschiedlichen vorgegebenen Größen eingestellt hat. 

Bildvorgaben finden Sie in der globalen Navigationsleiste unter **[!UICONTROL Einstellungen]** > **[!UICONTROL Bildvorgaben]** und navigieren Sie dann zu einer Bildvorgabe.

Experimentieren Sie mit verschiedenen Bildvorgaben. Erfahren Sie, wie das Bild angezeigt wird, wenn es dynamisch auf einer Website oder in einer Anwendung in unterschiedlichen Größen bereitgestellt wird.

Siehe [Vorschau eines Bild-Assets basierend auf seiner Bildvorgabe](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## &#x200B;4. Veröffentlichen der primären Bilder

Die Veröffentlichung Ihrer primären Bilddateien dient zwei wichtigen Zwecken:

* Veröffentlichen Sie Ihre primären Bilder auf Dynamic Media-Bildservern, damit Bilder dynamisch für Ihre Website und Ihr Programm bereitgestellt werden können.
* Beim Veröffentlichen werden die URL-Zeichenfolgen zum Aufrufen von Bildern von Dynamic Media-Bildservern an Ihre Website oder Anwendung aktiviert. Nach der Veröffentlichung können Sie die von Adobe Dynamic Media Classic generierten URLs kopieren und an die gewünschte Stelle in Ihrer Website oder Anwendung einfügen.

Wählen Sie in der globalen Navigationsleiste **[!UICONTROL Veröffentlichen]** aus, um einen Veröffentlichungsauftrag zu starten. Wählen Sie im Dialogfeld „Veröffentlichen“ die Option **[!UICONTROL Veröffentlichen starten]**. Siehe [Veröffentlichen primärer Bilder](publishing-master-images.md#publishing_master_images).

## &#x200B;5. Verknüpfen von URLs mit einer Web-Anwendung

Adobe Dynamic Media Classic erstellt URL-Legendenzeichenfolgen für Bilder. Wenn Sie Bilder auf Dynamic Media-Bildservern veröffentlichen, werden die URLs aktiv. Sie können diese URL-Zeichenfolgen aus dem Durchsuchen-Panel (in der Detailansicht) oder dem Bildschirm Vorschau kopieren. Nachdem Sie die URL-Zeichenfolgen kopiert haben, können Sie sie auf Ihrer Website und in Programmen verwenden. Die URL für die Bildgröße ersetzt den Verweis auf einen statischen Bildnamen in Ihrem Web-Seiten-Code. Die URL verweist auf einen primären Bildnamen, den die Datenbank für jedes neue anzuzeigende Bild ersetzt.

Mit Bildvorgaben generierte URL-Zeichenfolgen enthalten den Namen einer Bildvorgabe. Dieser Name ist in Dollarzeichen (`$`) eingeschlossen. Beispielsweise kann `$thumbnail$` die Bildvorgabe sein, die dazu konzipiert ist, primäre Bilder in der Größe von Miniaturansichten anzuzeigen. Siehe [Verknüpfen von URLs mit einer Web-Anwendung](linking-urls-web-application.md#linking_urls_to_your_web_application).
