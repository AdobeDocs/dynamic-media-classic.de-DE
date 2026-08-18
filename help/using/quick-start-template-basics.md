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
autotag-review: '2026-05-13T20:10:57.394Z'
TQID: 'https://experienceleague.adobe.com/2DaWdJsCz9f5iXEkMi6N1L7s3eFdvpBc1ECrgbVAueo'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: 604d547f6867b1a7683f6489555bd5932270d873
workflow-type: tm+mt
source-wordcount: 840
ht-degree: 18%

---

# Kurzanleitung: Vorlagen aus Grundelementen{#quick-start-template-basics}

Vorlagen werden dynamisch erstellt und in adressierbaren Bilddateien mit mehreren Ebenen, ähnlich wie in Bildbearbeitungsanwendungen wie Adobe Photoshop, erstellt. Im Unterschied zu einer statischen Datei mit Ebenen, z. B. einer PSD-Datei, kann eine Vorlage auch Parameter enthalten. Mithilfe von Parametern können die verschiedenen Aspekte eines Bilds adressiert und angepasst werden.

Eine Vorlage kann eine beliebige Anzahl von Bildebenen und Textebenen enthalten. Sie können eine statische Datei, die Ebenen enthält, z. B. eine mehrschichtige PSD-Datei, in eine Vorlage konvertieren und Vorlagen in Adobe Dynamic Media Classic erstellen. Mit den in Adobe Dynamic Media Classic hochgeladenen Schriftarten können Sie Textebenen in Vorlagen erstellen. Nachdem Sie einer Vorlage Text hinzugefügt haben, können Sie sie formatieren, indem Sie ihre Ausrichtung, Schriftart, Schriftgröße und Farbe ändern.

Auf der Seite Parameter können Sie jeden Aspekt einer Vorlage in einen adressierbaren Parameter konvertieren. Sie können ändern, welcher Bild- oder Textwert der Ebene in Ihrer Vorlage verwendet werden soll. Parameter werden mit der URL-Zeichenfolge übergeben. Auf diese Weise können Sie beliebige Parameter ändern, damit Sie das resultierende Bild, das vom Bildserver generiert wird, dynamisch anpassen können.

Siehe auch [Vorlagengrundlagen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) Schulungsvideo.

Diese Kurzanleitung soll Ihnen bei der Verwendung von Vorlagengrundlagen helfen.

## &#x200B;1. Hochladen von Dateien

Laden Sie die PSD- oder Grafikdatei für Ihre Vorlage hoch. Adobe Dynamic Media Classic unterstützt neben PSD auch viele andere Bilddateiformate. Für Vorlagen werden jedoch verlustfreie TIFF- und PNG-Bilder empfohlen, da sie Transparenz ermöglichen.

Wenn Sie zum Erstellen Ihrer Vorlage eine PSD-Datei verwenden, wählen Sie **[!UICONTROL Vorlage erstellen]** im Dialogfeld **[!UICONTROL Upload-Auftragsoptionen]** aus, wenn Sie die PSD-Datei hochladen. Wählen Sie auch eine Option **[!UICONTROL Ebenenbenennung]**, damit Adobe Dynamic Media Classic weiß, wie PSD-Ebenen benannt werden, wenn sie in Adobe Dynamic Media Classic hochgeladen werden.

Wenn Sie Bilddateien verwenden, können Sie die Bilder zuschneiden und beim Hochladen auch eine Maske aus den Zuschneidepfaden in den Bildern erstellen.

Wählen Sie in der globalen Navigationsleiste **[!UICONTROL Hochladen]** aus, um eine PSD-Datei oder andere Bilddateien von Ihrem Computer in einen Ordner in Adobe Dynamic Media Classic hochzuladen. Siehe [Hochladen von Vorlagendateien](uploading-template-files.md#uploading_template_files).

## &#x200B;2. Erstellen von Vorlagen

Um eine Vorlage aus einer PSD-Datei zu erstellen, wählen Sie **[!UICONTROL Vorlage erstellen]** aus, wenn Sie die Datei hochladen. Um eine Vorlage aus Bildern zu erstellen, klicken Sie in der globalen Navigationsleiste auf **[!UICONTROL Erstellen]** > **[!UICONTROL Vorlagengrundlagen]**. Geben Sie eine Breite und eine Höhenmessung für die Arbeitsfläche ein. Wählen Sie rechts oben auf der Seite entweder **[!UICONTROL Designer]** oder **[!UICONTROL Developer]** aus und ziehen Sie Bilder auf die Vorlagenseite. Sie können auch die Bilder auswählen *bevor* gehen Sie zu **[!UICONTROL Erstellen]** > **[!UICONTROL Vorlagengrundlagen]**. Die Vorlagenseite bietet Tools für Folgendes:

* Bildebenen hinzufügen. Um eine Ebene hinzuzufügen, ziehen Sie ein Bild in die Vorlagenseite.
* Textebenen hinzufügen. Wählen Sie das Symbol **[!UICONTROL Text-Tool]** aus. Ziehen Sie den Mauszeiger, um ein Feld für die Textebene zu erstellen, und formatieren Sie dann den Text mit Werkzeugen auf der Seite Text .
* Größe und Position von Ebenen ändern.
* Anordnung von Ebenen ändern.
* Schatten- und Schein-Effekte auf Bild- und Textebenen anwenden.

Siehe [Erstellen einer Vorlage](creating-template.md#creating_a_template).

## &#x200B;3. Erstellen von Vorlagenparametern

Im nächsten Schritt werden die Eigenschaften von Ebenen in Parameter umgewandelt, d. h. parametrisiert, um festzulegen, welche Ebeneneigenschaften in die URL-Zeichenfolge aufgenommen werden. Mit Parametern können Sie Vorlagen mit größerer Flexibilität verwenden. Nachdem Sie eine Ebeneneigenschaft parametrisiert haben, können Sie den Parameter dynamisch ändern.

Um eine Ebene zu parametrisieren, öffnen Sie die Vorlage auf der Vorlagenseite und wählen Sie **[!UICONTROL Parameter]** neben einem Ebenennamen aus. Wählen Sie auf der Seite Parameter die Option neben jedem Parameter aus, den Sie hinzufügen möchten. Siehe [Erstellen von ](creating-template-parameters.md#creating_template_parameters).

## &#x200B;4. Veröffentlichen von Vorlagen

Beim Veröffentlichen der Vorlage wird sie auf Dynamic Media-Bildservern platziert, damit sie dynamisch für Ihre Website oder Ihr Programm bereitgestellt werden kann. Beim Veröffentlichen wird auch die URL aktiviert, um die Vorlage von den Dynamic Media-Bildservern auf Ihrer Website oder in Ihrem Programm aufzurufen.

Achten Sie darauf, alle Bilder zu veröffentlichen, die der Vorlage zugeordnet sind.

Um eine Vorlage zu veröffentlichen, markieren Sie sie zur Veröffentlichung und wählen Sie in der Symbolleiste für globale Navigation **[!UICONTROL Veröffentlichen]** aus. Wählen Sie dann **[!UICONTROL Veröffentlichung starten]**. Siehe [Vorlagen veröffentlichen](publishing-templates.md#publishing_templates).

## &#x200B;5. Verknüpfen einer Vorlage mit einer Website

Dynamic Media Classic erstellt URLs für Vorlagen und aktiviert die URLs, wenn Sie Vorlagen auf Dynamic Media-Bildservern veröffentlichen. Sie können diese URL-Zeichenfolgen aus der Vorlagenvorschau kopieren.

Wählen Sie Ihre Vorlage im Durchsuchen-Panel aus und klicken Sie dann auf **[!UICONTROL Vorschau]**, um die Seite „Vorlagenvorschau“ zu öffnen. Wählen Sie eine Bildvorgabe für die Bereitstellung Ihrer Vorlage aus und klicken Sie dann auf die Schaltfläche **[!UICONTROL URL kopieren]**. Nachdem Sie die URL von der Vorschauseite kopiert haben, können Sie sie auf Ihrer Website oder in Ihrem Programm verwenden. Siehe [Verknüpfen einer Vorlage mit einer Webseite](linking-template-web-page.md#linking_a_template_to_a_web_page).
