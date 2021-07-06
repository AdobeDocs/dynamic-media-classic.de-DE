---
title: '"Kurzanleitung: Vorlagen aus Grundelementen"'
description: Eine Einführung und ein Schnellstart zu den Vorlagengrundlagen , die Ihnen dabei helfen, schnell zu arbeiten.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 34%

---

# Kurzanleitung: Vorlagen aus Grundelementen{#quick-start-template-basics}

Vorlagengrundlagen werden dynamisch erstellt und adressierbare Bilddateien mit mehreren Ebenen, wie z. B. Dateien mit mehreren Ebenen in Bildbearbeitungsanwendungen wie Adobe Photoshop. Im Unterschied zu einer statischen Datei mit Ebenen, z. B. einer PSD-Datei, kann eine Vorlage auch Parameter enthalten. Mithilfe von Parametern können die verschiedenen Aspekte eines Bilds adressiert und angepasst werden.

Eine Vorlage kann eine beliebige Anzahl von Bildebenen und Textebenen enthalten. Sie können eine statische Datei mit Ebenen, z. B. eine PSD-Datei mit Ebenen, in eine Vorlage konvertieren und in Dynamic Media Classic Vorlagen erstellen. Sie können Textebenen in Vorlagen mit Schriftarten erstellen, die Sie in Dynamic Media Classic hochgeladen haben. Nachdem Sie einer Vorlage Text hinzugefügt haben, können Sie ihn formatieren, indem Sie Ausrichtung, Schriftart, Schriftgröße und Schriftfarbe ändern.

Auf der Seite Parameter können Sie beliebige Aspekte einer Vorlage in adressierbare Parameter konvertieren. Auf diese Weise können Sie angeben, welches Bild mit Ebenen bzw. welcher Textwert in der Vorlage verwendet werden soll. Parameter werden mit der URL-Zeichenfolge übergeben, damit Sie das auf dem Image-Server generierte Antwortbild durch dynamisches Ändern eines beliebigen Parameters entsprechend anpassen können.

Diese Kurzanleitung hilft Ihnen, sich schnell mit Vorlagen aus Grundelementen vertraut zu machen.

## 1. Hochladen der Dateien

Laden Sie zunächst die PSD-Datei oder die Bilddatei für Ihre Vorlage hoch. Dynamic Media Classic unterstützt neben PSD viele Bilddateiformate, verlustfreie TIFF- und PNG-Bilder werden jedoch für Vorlagen empfohlen, da sie Transparenz ermöglichen.

Wenn Sie eine PSD-Datei zum Erstellen Ihrer Vorlage verwenden, wählen Sie **[!UICONTROL Vorlage erstellen]** im Dialogfeld **[!UICONTROL Upload-Auftragsoptionen]** aus, wenn Sie die PSD-Datei hochladen. Wählen Sie außerdem die Option **[!UICONTROL Ebenenbenennung]**, damit Dynamic Media Classic weiß, wie PSD-Ebenen benannt werden, wenn sie in Dynamic Media Classic hochgeladen werden.

Wenn Sie Bilddateien verwenden, können Sie die Bilder beim Hochladen beschneiden oder eine Maske aus deren Beschneidungspfaden erstellen.

Klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Upload]** , um eine PSD-Datei oder andere Bilddateien von Ihrem Computer in einen Ordner in Dynamic Media Classic hochzuladen. Siehe [Hochladen von Vorlagendateien](uploading-template-files.md#uploading_template_files).

## 2. Erstellen einer Vorlage

Um eine Vorlage aus einer PSD-Datei zu erstellen, wählen Sie beim Hochladen der Datei **[!UICONTROL Vorlage erstellen]** aus. Um eine Vorlage aus Bildern zu erstellen, klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Build]** > **[!UICONTROL Vorlagengrundlagen]** und geben Sie eine Breite und Höhe für die Arbeitsfläche ein. Wählen Sie in der rechten oberen Ecke der Seite entweder **[!UICONTROL Designer]** oder **[!UICONTROL Entwickler]** aus und ziehen Sie Bilder auf die Seite &quot;Vorlage&quot;. Sie können auch die Bilder *vor* auswählen, indem Sie auf **[!UICONTROL Build]** > **[!UICONTROL Vorlagengrundlagen]** klicken. Die Seite &quot;Vorlage&quot;bietet Tools für:

* Bildebenen hinzufügen. Um eine Ebene hinzuzufügen, ziehen Sie ein Bild auf die Seite Vorlage .
* Textebenen hinzufügen. Klicken Sie auf das Symbol **[!UICONTROL Text-Tool]**. Ziehen Sie den Mauszeiger, um ein Feld für die Textebene zu erstellen. Formatieren Sie dann den Text mit Tools auf der Seite Text .
* Größe und Position von Ebenen ändern.
* Anordnung von Ebenen ändern.
* Schatten- und Schein-Effekte auf Bild- und Textebenen anwenden. 

Siehe [Erstellen einer Vorlage](creating-template.md#creating_a_template).

## 3. Erstellen von Vorlagenparametern

Im nächsten Schritt werden die Eigenschaften von Ebenen in Parameter umgewandelt, d. h. parametrisiert, um festzulegen, welche Ebeneneigenschaften in die URL-Zeichenfolge aufgenommen werden. Parameter bieten Ihnen bei der Verwendung von Vorlagen größtmögliche Flexibilität. Nachdem Sie eine Ebeneneigenschaft parametrisiert haben, können Sie den Parameter dynamisch ändern.

Um eine Ebene zu parametrisieren, öffnen Sie die Vorlage auf der Seite Vorlage und klicken Sie dann neben einem Ebenennamen auf **[!UICONTROL Parameter]** . Wählen Sie auf der Seite Parameter die Option neben jedem Parameter aus, den Sie hinzufügen möchten. Siehe [Erstellen von Vorlagenparametern](creating-template-parameters.md#creating_template_parameters).

## 4. Veröffentlichungsvorlagen

Durch das Veröffentlichen Ihrer Vorlage wird sie auf Dynamic Media-Image-Servern platziert, damit sie dynamisch für Ihre Website oder Anwendung bereitgestellt werden kann. Beim Veröffentlichen wird auch die URL aktiviert, über die die Vorlage von Dynamic Media-Image-Servern für Ihre Website oder Anwendung aufgerufen werden kann.

Achten Sie darauf, alle Bilder zu veröffentlichen, die der Vorlage zugeordnet sind.

Um eine Vorlage zu veröffentlichen, markieren Sie sie zur Veröffentlichung und klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Veröffentlichen]**. Klicken Sie dann auf **[!UICONTROL Veröffentlichen senden]**. Siehe [Veröffentlichen von Vorlagen](publishing-templates.md#publishing_templates).

## 5. Verknüpfen einer Vorlage mit einer Webseite

Dynamic Media Classic erstellt URLs für Vorlagen und aktiviert die URLs, wenn Sie Vorlagen auf Dynamic Media-Image-Servern veröffentlichen. Sie können diese URL-Zeichenfolgen von der Seite &quot;Vorlagenvorschau&quot;kopieren.

Wählen Sie Ihre Vorlage im Durchsuchenbedienfeld aus und klicken Sie dann auf **[!UICONTROL Vorschau]** , um die Seite &quot;Vorlagenvorschau&quot;zu öffnen. Wählen Sie eine Bildvorgabe für die Bereitstellung Ihrer Vorlage aus und klicken Sie auf **[!UICONTROL URL kopieren]**. Nachdem Sie die URL von der Seite &quot;Vorschau&quot;kopiert haben, können Sie sie auf Ihrer Website oder in Ihrer Anwendung verwenden. Siehe [Verknüpfen einer Vorlage mit einer Website](linking-template-web-page.md#linking_a_template_to_a_web_page).
