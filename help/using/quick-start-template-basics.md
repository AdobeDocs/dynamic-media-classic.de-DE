---
title: 'Kurzanleitung: Vorlagen aus Grundelementen'
description: Eine Einführung und ein Schnellstart zu den Vorlagengrundlagen , mit denen Sie schnell in Adobe Dynamic Media Classic arbeiten können.
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

Vorlagengrundlagen werden dynamisch erstellt und adressierbare Bilddateien mit mehreren Ebenen, wie z. B. Dateien mit mehreren Ebenen in Bildbearbeitungsanwendungen wie Adobe Photoshop. Im Unterschied zu einer statischen Datei mit Ebenen, z. B. einer PSD-Datei, kann eine Vorlage auch Parameter enthalten. Mithilfe von Parametern können die verschiedenen Aspekte eines Bilds adressiert und angepasst werden.

Eine Vorlage kann eine beliebige Anzahl von Bildebenen und Textebenen enthalten. Sie können eine statische Datei mit Ebenen, z. B. eine PSD-Datei mit mehreren Ebenen, in eine Vorlage konvertieren und in Adobe Dynamic Media Classic Vorlagen erstellen. Sie können Textebenen in Vorlagen mit Schriftarten erstellen, die Sie in Adobe Dynamic Media Classic hochgeladen haben. Nachdem Sie einer Vorlage Text hinzugefügt haben, können Sie ihn formatieren, indem Sie die Ausrichtung, Schriftart, Schriftgröße und Farbe ändern.

Auf der Seite Parameter können Sie beliebige Aspekte einer Vorlage in adressierbare Parameter konvertieren. Auf diese Weise können Sie ändern, welches Bild mit Ebenen verwendet werden soll oder welchen Textwert Sie in Ihrer Vorlage verwenden möchten. Parameter werden mit der URL-Zeichenfolge übergeben, sodass Sie jeden Parameter ändern können, damit Sie das vom Image-Server generierte Antwortbild dynamisch anpassen können.

Siehe auch Schulungsvideo zu [Vorlagengrundlagen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) .

Diese Kurzanleitung soll Sie schnell mit den Vorlagengrundlagen vertraut machen.

## 1. Hochladen der Dateien

Laden Sie zunächst die PSD-Datei oder die Bilddatei für Ihre Vorlage hoch. Adobe Dynamic Media Classic unterstützt neben dem PSD viele Bilddateiformate. Für Vorlagen werden jedoch verlustfreie TIFF- und PNG-Bilder empfohlen, da sie Transparenz ermöglichen.

Wenn Sie eine PSD-Datei zum Erstellen Ihrer Vorlage verwenden, wählen Sie beim Hochladen der PSD-Datei im Dialogfeld **[!UICONTROL Upload-Auftragsoptionen]** die Option **[!UICONTROL Vorlage erstellen]** aus. Wählen Sie außerdem die Option **[!UICONTROL Ebenennamen]** , damit Adobe Dynamic Media Classic weiß, wie PSD-Ebenen benannt werden, wenn sie in Adobe Dynamic Media Classic hochgeladen werden.

Wenn Sie Bilddateien verwenden, können Sie die Bilder beschneiden und beim Hochladen eine Maske aus Beschneidungspfaden in den Bildern erstellen.

Wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Hochladen]** aus, um eine PSD-Datei oder andere Bilddateien von Ihrem Computer in einen Ordner auf Adobe Dynamic Media Classic hochzuladen. Siehe [Hochladen von Vorlagendateien](uploading-template-files.md#uploading_template_files).

## 2. Erstellen einer Vorlage

Um eine Vorlage aus einer PSD-Datei zu erstellen, wählen Sie beim Hochladen der Datei **[!UICONTROL Vorlage erstellen]** aus. Um eine Vorlage aus Bildern zu erstellen, gehen Sie in der Leiste &quot;Globale Navigation&quot;zu &quot;**[!UICONTROL Build]**&quot;> &quot;**[!UICONTROL Vorlagengrundlagen]**&quot;, geben Sie eine Breite und Höhe für die Arbeitsfläche ein. Wählen Sie rechts oben auf der Seite entweder **[!UICONTROL Designer]** oder **[!UICONTROL Entwickler]** aus und ziehen Sie Bilder auf die Seite &quot;Vorlage&quot;. Sie können auch die Bilder *vor* auswählen, indem Sie zu **[!UICONTROL Build]** > **[!UICONTROL Vorlagengrundlagen]** navigieren. Die Seite &quot;Vorlage&quot;bietet Tools für:

* Bildebenen hinzufügen. Um eine Ebene hinzuzufügen, ziehen Sie ein Bild auf die Seite Vorlage .
* Textebenen hinzufügen. Wählen Sie das Symbol **[!UICONTROL Text-Tool]** aus. Ziehen Sie den Mauszeiger, um ein Feld für die Textebene zu erstellen. Formatieren Sie dann den Text mit Tools auf der Textseite.
* Größe und Position von Ebenen ändern.
* Anordnung von Ebenen ändern.
* Schatten- und Schein-Effekte auf Bild- und Textebenen anwenden. 

Siehe [Erstellen einer Vorlage](creating-template.md#creating_a_template).

## 3. Vorlagenparameter erstellen

Im nächsten Schritt werden die Eigenschaften von Ebenen in Parameter umgewandelt, d. h. parametrisiert, um festzulegen, welche Ebeneneigenschaften in die URL-Zeichenfolge aufgenommen werden. Parameter bieten Ihnen bei der Verwendung von Vorlagen größtmögliche Flexibilität. Nachdem Sie eine Ebeneneigenschaft parametrisiert haben, können Sie den Parameter dynamisch ändern.

Um eine Ebene zu parametrisieren, öffnen Sie die Vorlage auf der Seite Vorlage und wählen Sie dann **[!UICONTROL Parameter]** neben einem Ebenennamen aus. Wählen Sie auf der Seite Parameter die Option neben jedem Parameter aus, den Sie hinzufügen möchten. Siehe [Vorlagenparameter erstellen](creating-template-parameters.md#creating_template_parameters).

## 4. Publish-Vorlagen

Durch das Veröffentlichen Ihrer Vorlage wird sie auf Dynamic Media-Image-Servern platziert, damit sie dynamisch für Ihre Website oder Anwendung bereitgestellt werden kann. Beim Veröffentlichen wird auch die URL aktiviert, über die die Vorlage von Dynamic Media-Image-Servern für Ihre Website oder Anwendung aufgerufen werden kann.

Achten Sie darauf, alle Bilder zu veröffentlichen, die der Vorlage zugeordnet sind.

Um eine Vorlage zu veröffentlichen, markieren Sie sie zur Veröffentlichung und wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Publish]** aus. Wählen Sie dann **[!UICONTROL Publish übermitteln]** aus. Siehe [Publish-Vorlagen](publishing-templates.md#publishing_templates).

## 5. Verknüpfen einer Vorlage mit einer Webseite

Dynamic Media Classic erstellt URLs für Vorlagen und aktiviert die URLs, wenn Sie Vorlagen auf Dynamic Media-Image-Servern veröffentlichen. Sie können diese URL-Zeichenfolgen von der Seite &quot;Vorlagenvorschau&quot;kopieren.

Wählen Sie Ihre Vorlage im Bedienfeld &quot;Durchsuchen&quot;aus und klicken Sie dann auf **[!UICONTROL Vorschau]** , um die Seite &quot;Vorlagenvorschau&quot;zu öffnen. Wählen Sie eine Bildvorgabe für die Bereitstellung Ihrer Vorlage aus und klicken Sie dann auf die Schaltfläche **[!UICONTROL URL kopieren]** . Nachdem Sie die URL von der Seite &quot;Vorschau&quot;kopiert haben, können Sie sie auf Ihrer Website oder in Ihrer Anwendung verwenden. Siehe [Verknüpfen einer Vorlage mit einer Webseite](linking-template-web-page.md#linking_a_template_to_a_web_page).
