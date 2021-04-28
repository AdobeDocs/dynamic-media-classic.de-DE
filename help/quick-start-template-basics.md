---
title: '"Kurzanleitung: Vorlagen aus Grundelementen"'
description: Eine Einführung und ein kurzer Beginn zu den Vorlagen aus Grundelementen, die Ihnen helfen, sich schnell aufzumachen.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
translation-type: tm+mt
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 34%

---

# Kurzanleitung: Vorlagen aus Grundelementen{#quick-start-template-basics}

Vorlagen aus Grundelementen sind dynamisch erstellte und adressierbare Bilddateien mit mehreren Ebenen, z. B. in Bildbearbeitungsanwendungen wie Adobe Photoshop. Im Unterschied zu einer statischen Datei mit Ebenen, z. B. einer PSD-Datei, kann eine Vorlage auch Parameter enthalten. Mithilfe von Parametern können die verschiedenen Aspekte eines Bilds adressiert und angepasst werden.

Eine Vorlage kann eine beliebige Anzahl von Bildebenen und Textebenen enthalten. Sie können eine statische Datei, die Ebenen enthält, z. B. eine PSD-Datei mit Ebenen, in eine Vorlage konvertieren und in Dynamic Media Classic Vorlagen erstellen. Sie können Textebenen in Vorlagen mit Schriftarten erstellen, die Sie in Dynamic Media Classic hochgeladen haben. Nachdem Sie einer Vorlage Text hinzugefügt haben, können Sie ihn formatieren, indem Sie Ausrichtung, Schriftart, Schriftgröße und Schriftfarbe ändern.

Auf der Seite &quot;Parameter&quot;können Sie jeden Aspekt einer Vorlage in einen adressierbaren Parameter konvertieren. Auf diese Weise können Sie angeben, welches Bild mit Ebenen bzw. welcher Textwert in der Vorlage verwendet werden soll. Parameter werden mit der URL-Zeichenfolge übergeben, damit Sie das auf dem Image-Server generierte Antwortbild durch dynamisches Ändern eines beliebigen Parameters entsprechend anpassen können.

Diese Kurzanleitung hilft Ihnen, sich schnell mit Vorlagen aus Grundelementen vertraut zu machen.

## 1. Hochladen der Dateien

Laden Sie zunächst die PSD-Datei oder die Bilddatei für Ihre Vorlage hoch. Dynamic Media Classic unterstützt neben PSD viele Bilddateiformate, aber verlustfreie TIFF- und PNG-Bilder werden für Vorlagen empfohlen, da sie Transparenz ermöglichen.

Wenn Sie eine Vorlage mithilfe einer PSD-Datei erstellen, wählen Sie im Dialogfeld **[!UICONTROL Upload-Auftragsoptionen]** die Option **[!UICONTROL Vorlage erstellen]**, wenn Sie die PSD-Datei hochladen. Wählen Sie außerdem die Option **[!UICONTROL Ebenenname]**, damit Dynamic Media Classic weiß, wie PSD-Ebenen benannt werden, wenn sie in Dynamic Media Classic hochgeladen werden.

Wenn Sie Bilddateien verwenden, können Sie die Bilder beim Hochladen beschneiden oder eine Maske aus deren Beschneidungspfaden erstellen.

Klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Hochladen]**, um eine PSD-Datei oder andere Bilddateien von Ihrem Computer in einen Ordner in Dynamic Media Classic hochzuladen. Siehe [Hochladen von Vorlagendateien](uploading-template-files.md#uploading_template_files).

## 2. Erstellen einer Vorlage

Um eine Vorlage aus einer PSD-Datei zu erstellen, wählen Sie beim Hochladen der Datei **[!UICONTROL Vorlage erstellen]**. Um eine Vorlage aus Bildern zu erstellen, klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Erstellen]** > **[!UICONTROL Vorlagen aus Grundelementen]** und geben Sie eine Messung der Breite und Höhe für die Arbeitsfläche ein. Wählen Sie rechts oben auf der Seite entweder **[!UICONTROL Designer]** oder **[!UICONTROL Entwickler]** aus und ziehen Sie die Bilder auf die Seite &quot;Vorlage&quot;. Sie können auch die Bilder *vor* auswählen und auf **[!UICONTROL Erstellen]** > **[!UICONTROL Vorlagen aus Grundelementen]** klicken. Die Vorlagenseite bietet Angebote für:

* Bildebenen hinzufügen. Um eine Ebene hinzuzufügen, ziehen Sie ein Bild auf die Seite &quot;Vorlage&quot;.
* Textebenen hinzufügen. Klicken Sie auf das Symbol **[!UICONTROL Text tool]**. Ziehen Sie den Zeiger, um ein Feld für die Textebene zu erstellen. Formatieren Sie dann den Text mit Werkzeugen auf der Seite Text.
* Größe und Position von Ebenen ändern.
* Anordnung von Ebenen ändern.
* Schatten- und Schein-Effekte auf Bild- und Textebenen anwenden. 

Siehe [Erstellen einer Vorlage](creating-template.md#creating_a_template).

## 3. Erstellen von Vorlagenparametern

Im nächsten Schritt werden die Eigenschaften von Ebenen in Parameter umgewandelt, d. h. parametrisiert, um festzulegen, welche Ebeneneigenschaften in die URL-Zeichenfolge aufgenommen werden. Parameter bieten Ihnen bei der Verwendung von Vorlagen größtmögliche Flexibilität. Nachdem Sie eine Ebeneneigenschaft parametrisiert haben, können Sie den Parameter dynamisch ändern.

Um eine Ebene zu parametrisieren, öffnen Sie die Vorlage auf der Seite &quot;Vorlage&quot;und klicken Sie dann auf **[!UICONTROL Parameter]** neben dem Namen einer Ebene. Wählen Sie auf der Seite &quot;Parameter&quot;die Option neben jedem Parameter, den Sie hinzufügen möchten. Siehe [Erstellen von Vorlagenparametern](creating-template-parameters.md#creating_template_parameters).

## 4. Veröffentlichen von Vorlagen

Beim Veröffentlichen der Vorlage wird diese auf Dynamic Media-Image-Servern gespeichert, damit sie dynamisch an Ihre Website oder Anwendung übertragen werden kann. Bei der Veröffentlichung wird auch die URL aktiviert, mit der die Vorlage von den Dynamic Media-Image-Servern für Ihre Website oder Anwendung aufgerufen werden kann.

Achten Sie darauf, alle Bilder zu veröffentlichen, die der Vorlage zugeordnet sind.

Um eine Vorlage zu veröffentlichen, markieren Sie sie zur Veröffentlichung und klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Veröffentlichen]**. Klicken Sie dann auf **[!UICONTROL Veröffentlichung senden]**. Siehe [Veröffentlichen von Vorlagen](publishing-templates.md#publishing_templates).

## 5. Verknüpfen einer Vorlage mit einer Webseite

Dynamic Media Classic erstellt URLs für Vorlagen und aktiviert die URLs, wenn Sie Vorlagen auf Dynamic Media-Image-Servern veröffentlichen. Sie können diese URL-Zeichenfolgen von der Seite &quot;Vorschau der Vorlage&quot;kopieren.

Wählen Sie die Vorlage im Durchsuchenbedienfeld aus und klicken Sie dann auf **[!UICONTROL Vorschau]**, um die Seite &quot;Vorschau der Vorlage&quot;zu öffnen. Wählen Sie eine Bildvorgabe für die Bereitstellung der Vorlage aus und klicken Sie dann auf **[!UICONTROL URL kopieren]**. Nachdem Sie die URL von der Seite &quot;Vorschau&quot;kopiert haben, können Sie sie auf Ihrer Website oder in Ihrer Anwendung verwenden. Siehe [Verknüpfen einer Vorlage mit einer Website](linking-template-web-page.md#linking_a_template_to_a_web_page).
