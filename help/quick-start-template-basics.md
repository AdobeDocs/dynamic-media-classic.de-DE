---
title: '"Kurzanleitung: Vorlagen aus Grundelementen"'
description: Eine Einführung und ein Schnellstart zu den Vorlagengrundlagen , die Ihnen helfen, in Adobe Dynamic Media Classic schnell einzurichten und auszuführen.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
source-git-commit: 36f9aa3c2b4dc66e4cb851c2ce6837ae0ad4f64c
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 32%

---

# Kurzanleitung: Vorlagen aus Grundelementen{#quick-start-template-basics}

Vorlagengrundlagen werden dynamisch erstellt und adressierbare Bilddateien mit mehreren Ebenen, wie z. B. Dateien mit mehreren Ebenen in Bildbearbeitungsanwendungen wie Adobe Photoshop. Im Unterschied zu einer statischen Datei mit Ebenen, z. B. einer PSD-Datei, kann eine Vorlage auch Parameter enthalten. Mithilfe von Parametern können die verschiedenen Aspekte eines Bilds adressiert und angepasst werden.

Eine Vorlage kann eine beliebige Anzahl von Bildebenen und Textebenen enthalten. Sie können eine statische Datei mit Ebenen, z. B. eine PSD-Datei mit mehreren Ebenen, in eine Vorlage konvertieren und in Adobe Dynamic Media Classic Vorlagen erstellen. Sie können Textebenen in Vorlagen erstellen, indem Sie Schriftarten verwenden, die Sie in Adobe Dynamic Media Classic hochgeladen haben. Nachdem Sie einer Vorlage Text hinzugefügt haben, können Sie ihn formatieren, indem Sie Ausrichtung, Schriftart, Schriftgröße und Schriftfarbe ändern.

Auf der Seite Parameter können Sie beliebige Aspekte einer Vorlage in adressierbare Parameter konvertieren. Auf diese Weise können Sie angeben, welches Bild mit Ebenen bzw. welcher Textwert in der Vorlage verwendet werden soll. Parameter werden mit der URL-Zeichenfolge übergeben, damit Sie das auf dem Image-Server generierte Antwortbild durch dynamisches Ändern eines beliebigen Parameters entsprechend anpassen können.

Diese Kurzanleitung hilft Ihnen, sich schnell mit Vorlagen aus Grundelementen vertraut zu machen.

## 1. Hochladen der Dateien

Laden Sie zunächst die PSD-Datei oder die Bilddatei für Ihre Vorlage hoch. Adobe Dynamic Media Classic unterstützt neben PSD viele Bilddateiformate, aber verlustfreie TIFF- und PNG-Bilder werden für Vorlagen empfohlen, da sie Transparenz ermöglichen.

Wenn Sie eine PSD-Datei zum Erstellen Ihrer Vorlage verwenden, wählen Sie **[!UICONTROL Vorlage erstellen]** im Dialogfeld **[!UICONTROL Upload-Auftragsoptionen]** aus, wenn Sie die PSD-Datei hochladen. Wählen Sie außerdem die Option **[!UICONTROL Ebenenbenennung]** aus, damit Adobe Dynamic Media Classic weiß, wie PSD-Ebenen benannt werden, wenn sie in Adobe Dynamic Media Classic hochgeladen werden.

Wenn Sie Bilddateien verwenden, können Sie die Bilder beim Hochladen beschneiden oder eine Maske aus deren Beschneidungspfaden erstellen.

Wählen Sie in der Symbolleiste für globale Navigation **[!UICONTROL Upload]** aus, um eine PSD-Datei oder andere Bilddateien von Ihrem Computer in einen Ordner auf Adobe Dynamic Media Classic hochzuladen. Siehe [Hochladen von Vorlagendateien](uploading-template-files.md#uploading_template_files).

## 2. Erstellen einer Vorlage

Um eine Vorlage aus einer PSD-Datei zu erstellen, wählen Sie beim Hochladen der Datei **[!UICONTROL Vorlage erstellen]** aus. Um eine Vorlage aus Bildern zu erstellen, gehen Sie in der Symbolleiste für globale Navigation zu **[!UICONTROL Build]** > **[!UICONTROL Vorlagengrundlagen]** und geben Sie eine Breite und Höhe für die Arbeitsfläche ein. Wählen Sie in der rechten oberen Ecke der Seite entweder **[!UICONTROL Designer]** oder **[!UICONTROL Entwickler]** aus und ziehen Sie Bilder auf die Seite &quot;Vorlage&quot;. Sie können auch die Bilder *auswählen, bevor* Sie zu **[!UICONTROL Build]** > **[!UICONTROL Vorlagengrundlagen]** navigieren. Die Seite &quot;Vorlage&quot;bietet Tools für:

* Bildebenen hinzufügen. Um eine Ebene hinzuzufügen, ziehen Sie ein Bild auf die Seite Vorlage .
* Textebenen hinzufügen. Wählen Sie das Symbol **[!UICONTROL Text-Tool]** aus. Ziehen Sie den Mauszeiger, um ein Feld für die Textebene zu erstellen. Formatieren Sie dann den Text mit Tools auf der Seite Text .
* Größe und Position von Ebenen ändern.
* Anordnung von Ebenen ändern.
* Schatten- und Schein-Effekte auf Bild- und Textebenen anwenden. 

Siehe [Erstellen einer Vorlage](creating-template.md#creating_a_template).

## 3. Erstellen von Vorlagenparametern

Im nächsten Schritt werden die Eigenschaften von Ebenen in Parameter umgewandelt, d. h. parametrisiert, um festzulegen, welche Ebeneneigenschaften in die URL-Zeichenfolge aufgenommen werden. Parameter bieten Ihnen bei der Verwendung von Vorlagen größtmögliche Flexibilität. Nachdem Sie eine Ebeneneigenschaft parametrisiert haben, können Sie den Parameter dynamisch ändern.

Um eine Ebene zu parametrisieren, öffnen Sie die Vorlage auf der Seite Vorlage und wählen Sie dann **[!UICONTROL Parameter]** neben einem Ebenennamen aus. Wählen Sie auf der Seite Parameter die Option neben jedem Parameter aus, den Sie hinzufügen möchten. Siehe [Vorlagenparameter erstellen](creating-template-parameters.md#creating_template_parameters).

## 4. Veröffentlichungsvorlagen

Durch das Veröffentlichen Ihrer Vorlage wird sie auf Dynamic Media-Image-Servern platziert, damit sie dynamisch für Ihre Website oder Anwendung bereitgestellt werden kann. Beim Veröffentlichen wird auch die URL aktiviert, über die die Vorlage von Dynamic Media-Image-Servern für Ihre Website oder Anwendung aufgerufen werden kann.

Achten Sie darauf, alle Bilder zu veröffentlichen, die der Vorlage zugeordnet sind.

Um eine Vorlage zu veröffentlichen, markieren Sie sie zur Veröffentlichung und wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Publish]** aus. Wählen Sie dann **[!UICONTROL Veröffentlichen senden]** aus. Siehe [Veröffentlichungsvorlagen](publishing-templates.md#publishing_templates).

## 5. Verknüpfen einer Vorlage mit einer Webseite

Dynamic Media Classic erstellt URLs für Vorlagen und aktiviert die URLs, wenn Sie Vorlagen auf Dynamic Media-Image-Servern veröffentlichen. Sie können diese URL-Zeichenfolgen von der Seite &quot;Vorlagenvorschau&quot;kopieren.

Wählen Sie Ihre Vorlage im Durchsuchenbedienfeld aus und klicken Sie dann auf **[!UICONTROL Vorschau]** , um die Seite &quot;Vorlagenvorschau&quot;zu öffnen. Wählen Sie eine Bildvorgabe für die Bereitstellung Ihrer Vorlage und dann **[!UICONTROL URL kopieren]**. Nachdem Sie die URL von der Seite &quot;Vorschau&quot;kopiert haben, können Sie sie auf Ihrer Website oder in Ihrer Anwendung verwenden. Siehe [Verknüpfen einer Vorlage mit einer Webseite](linking-template-web-page.md#linking_a_template_to_a_web_page).
