---
title: 'Kurzanleitung: Vorlagen aus Grundelementen'
description: Eine Einführung und eine Kurzanleitung zu den Grundlagen von Vorlagen, die Ihnen den schnellen Einstieg in Adobe Dynamic Media Classic erleichtern.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 17%

---

# Kurzanleitung: Vorlagen aus Grundelementen{#quick-start-template-basics}

Vorlagengrundlagen sind dynamisch erstellte und adressierbare Bilddateien mit mehreren Ebenen, wie z. B. mehrschichtige Dateien in Bildbearbeitungsanwendungen wie Adobe Photoshop. Im Unterschied zu einer statischen Datei mit Ebenen, z. B. einer PSD-Datei, kann eine Vorlage auch Parameter enthalten. Mithilfe von Parametern können die verschiedenen Aspekte eines Bilds adressiert und angepasst werden.

Eine Vorlage kann eine beliebige Anzahl von Bildebenen und Textebenen enthalten. Sie können eine statische Datei, die Ebenen enthält, z. B. eine mehrschichtige PSD-Datei, in eine Vorlage konvertieren und Vorlagen in Adobe Dynamic Media Classic erstellen. Mit den in Adobe Dynamic Media Classic hochgeladenen Schriftarten können Sie Textebenen in Vorlagen erstellen. Nachdem Sie einer Vorlage Text hinzugefügt haben, können Sie sie formatieren, indem Sie ihre Ausrichtung, Schriftart, Schriftgröße und Farbe ändern.

Auf der Seite Parameter können Sie jeden Aspekt einer Vorlage in einen adressierbaren Parameter konvertieren. Auf diese Weise können Sie ändern, welches Ebenenbild verwendet werden soll oder welcher Textwert in Ihrer Vorlage verwendet werden soll. Parameter werden mit der URL-Zeichenfolge übergeben, sodass Sie beliebige Parameter ändern können, um das vom Bild-Server generierte Antwortbild dynamisch anzupassen.

Siehe auch [Vorlagengrundlagen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) Schulungsvideo.

Diese Kurzanleitung soll Ihnen den schnellen Einstieg in die Arbeit mit den Vorlagengrundlagen erleichtern.

## &#x200B;1. Dateien hochladen

Laden Sie zunächst die PSD-Datei oder die Bilddatei für Ihre Vorlage hoch. Adobe Dynamic Media Classic unterstützt neben PSD auch viele andere Bilddateiformate. Für Vorlagen werden jedoch verlustfreie TIFF- und PNG-Bilder empfohlen, da sie Transparenz ermöglichen.

Wenn Sie zum Erstellen Ihrer Vorlage eine PSD-Datei verwenden, wählen Sie **[!UICONTROL Vorlage erstellen]** im Dialogfeld **[!UICONTROL Upload-Auftragsoptionen]** aus, wenn Sie die PSD-Datei hochladen. Wählen Sie auch eine Option **[!UICONTROL Ebenenbenennung]**, damit Adobe Dynamic Media Classic weiß, wie PSD-Ebenen benannt werden, wenn sie in Adobe Dynamic Media Classic hochgeladen werden.

Wenn Sie Bilddateien verwenden, können Sie die Bilder zuschneiden und beim Hochladen auch eine Maske aus den Zuschneidepfaden in den Bildern erstellen.

Wählen Sie in der globalen Navigationsleiste **[!UICONTROL Hochladen]** aus, um eine PSD-Datei oder andere Bilddateien von Ihrem Computer in einen Ordner in Adobe Dynamic Media Classic hochzuladen. Siehe [Hochladen von Vorlagendateien](uploading-template-files.md#uploading_template_files).

## &#x200B;2. Erstellen einer Vorlage

Um eine Vorlage aus einer PSD-Datei zu erstellen, wählen Sie **[!UICONTROL Vorlage erstellen]** aus, wenn Sie die Datei hochladen. Um eine Vorlage aus Bildern zu erstellen, klicken Sie in der globalen Navigationsleiste auf **[!UICONTROL Erstellen]** > **[!UICONTROL Vorlagengrundlagen]** und geben Sie eine Breite und eine Höhenmessung für die Arbeitsfläche ein. Wählen Sie rechts oben auf der Seite entweder **[!UICONTROL Designer]** oder **[!UICONTROL Developer]** aus und ziehen Sie Bilder auf die Vorlagenseite. Sie können auch die Bilder auswählen *bevor* gehen Sie zu **[!UICONTROL Erstellen]** > **[!UICONTROL Vorlagengrundlagen]**. Die Vorlagenseite bietet Tools für Folgendes:

* Bildebenen hinzufügen. Um eine Ebene hinzuzufügen, ziehen Sie ein Bild in die Vorlagenseite.
* Textebenen hinzufügen. Wählen Sie das Symbol **[!UICONTROL Text-Tool]** aus. Ziehen Sie den Mauszeiger, um ein Feld für die Textebene zu erstellen, und formatieren Sie dann den Text mit Werkzeugen auf der Seite Text .
* Größe und Position von Ebenen ändern.
* Anordnung von Ebenen ändern.
* Schatten- und Schein-Effekte auf Bild- und Textebenen anwenden. 

Siehe [Erstellen einer Vorlage](creating-template.md#creating_a_template).

## &#x200B;3. Erstellen von Vorlagenparametern

Im nächsten Schritt werden die Eigenschaften von Ebenen in Parameter umgewandelt, d. h. parametrisiert, um festzulegen, welche Ebeneneigenschaften in die URL-Zeichenfolge aufgenommen werden. Parameter bieten Ihnen bei der Verwendung von Vorlagen größtmögliche Flexibilität. Nachdem Sie eine Ebeneneigenschaft parametrisiert haben, können Sie den Parameter dynamisch ändern.

Um eine Ebene zu parametrisieren, öffnen Sie die Vorlage auf der Vorlagenseite und wählen Sie **[!UICONTROL Parameter]** neben einem Ebenennamen aus. Wählen Sie auf der Seite Parameter die Option neben jedem Parameter aus, den Sie hinzufügen möchten. Siehe [Erstellen von &#x200B;](creating-template-parameters.md#creating_template_parameters).

## &#x200B;4. Veröffentlichen von Vorlagen

Beim Veröffentlichen der Vorlage wird sie auf Dynamic Media-Bildservern platziert, damit sie dynamisch für Ihre Website oder Ihr Programm bereitgestellt werden kann. Beim Veröffentlichen wird auch die URL aktiviert, um die Vorlage von den Dynamic Media-Bildservern an Ihre Website oder Anwendung aufzurufen.

Achten Sie darauf, alle Bilder zu veröffentlichen, die der Vorlage zugeordnet sind.

Um eine Vorlage zu veröffentlichen, markieren Sie sie zur Veröffentlichung und wählen Sie in der Symbolleiste für globale Navigation **[!UICONTROL Veröffentlichen]** aus. Wählen Sie dann **[!UICONTROL Veröffentlichung starten]**. Siehe [Vorlagen veröffentlichen](publishing-templates.md#publishing_templates).

## &#x200B;5. Verknüpfen einer Vorlage mit einer Web-Seite

Dynamic Media Classic erstellt URLs für Vorlagen und aktiviert die URLs, wenn Sie Vorlagen auf Dynamic Media-Bildservern veröffentlichen. Sie können diese URL-Zeichenfolgen aus der Vorlagenvorschau kopieren.

Wählen Sie Ihre Vorlage im Durchsuchen-Panel aus und klicken Sie dann auf **[!UICONTROL Vorschau]**, um die Seite „Vorlagenvorschau“ zu öffnen. Wählen Sie eine Bildvorgabe für die Bereitstellung Ihrer Vorlage aus und klicken Sie dann auf die Schaltfläche **[!UICONTROL URL kopieren]**. Nachdem Sie die URL von der Vorschauseite kopiert haben, können Sie sie auf Ihrer Website oder in Ihrem Programm verwenden. Siehe [Verknüpfen von Vorlagen mit Web-Seiten](linking-template-web-page.md#linking_a_template_to_a_web_page).
