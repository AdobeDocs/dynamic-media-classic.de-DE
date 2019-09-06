---
title: '"Kurzanleitung: Vorlagen aus Grundelementen"'
seo-title: '"Kurzanleitung: Vorlagen aus Grundelementen"'
description: 'null'
seo-description: Eine Einführung und Schnellstart zu Vorlagen, die Ihnen helfen, schnell zu arbeiten.
uuid: 16 d 78 cbb-f 762-4263-aea 9-5712 eb 933693
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/template_ basics
discoiquuid: dd 0 fbb 39-3 f 6 a -496 b-a 9 b 6-63 b 11 dcb 823 a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Kurzanleitung: Vorlagen aus Grundelementen{#quick-start-template-basics}

Vorlagen aus Grundelementen sind dynamisch erstellte und adressierbare Bilddateien, wie z. B. Dateien mit Ebenen in Bildbearbeitungsanwendungen wie Adobe Photoshop. Im Unterschied zu einer statischen Datei mit Ebenen, z. B. einer PSD-Datei, kann eine Vorlage auch Parameter enthalten. Mithilfe von Parametern können die verschiedenen Aspekte eines Bilds adressiert und angepasst werden.

>[!NOTE]
>
>Sie können Vorlagen aus layoutbasierten Entwürfen erstellen, indem Sie Vorlagen für Veröffentlichungen und Dateien aus Adobe Illustrator und Adobe indesign verwenden. Siehe [Vorlagen für Veröffentlichungen](quick-start-template-publishing.md) .

Eine Vorlage kann eine beliebige Anzahl von Bildebenen und Textebenen enthalten. Sie können eine statische Datei mit Ebenen wie einer PSD-Datei mit Ebenen in eine Vorlage konvertieren sowie Vorlagen in Dynamic Media Classic erstellen. Sie können in Vorlagen auch Textebenen mit den Schriftarten erstellen, die Sie in das Scene7 Publishing System (SPS) hochgeladen haben. Nachdem Sie einer Vorlage Text hinzugefügt haben, können Sie ihn formatieren, indem Sie Ausrichtung, Schriftart, Schriftgröße und Schriftfarbe ändern.

Im Anzeigebereich „Parameter“ lassen sich beliebige Aspekte der Vorlage in adressierbare Parameter konvertieren. Auf diese Weise können Sie angeben, welches Bild mit Ebenen bzw. welcher Textwert in der Vorlage verwendet werden soll. Parameter werden mit der URL-Zeichenfolge übergeben, damit Sie das auf dem Image-Server generierte Antwortbild durch dynamisches Ändern eines beliebigen Parameters entsprechend anpassen können.

**Kurzanleitung**

Diese Kurzanleitung hilft Ihnen, sich schnell mit Vorlagen aus Grundelementen vertraut zu machen.

**1. Hochladen von Dateien**

Laden Sie zunächst die PSD-Datei oder die Bilddatei für Ihre Vorlage hoch. Dynamic Media Classic unterstützt viele Bilddateiformate zusätzlich zu PSD, verlustfreie TIFF- und PNG-Bilder werden jedoch für Vorlagen empfohlen, da sie Transparenz ermöglichen.

Wenn Sie eine Vorlage basierend auf einer PSD-Datei erstellen möchten, wählen Sie beim Hochladen der PSD-Datei im Dialogfeld „Upload-Auftragsoptionen“ die Option „Vorlage erstellen“. Wählen Sie außerdem eine Option für die Ebenenbenennung aus, um dynamisches Media Classic anzugeben, wie PSD-Ebenen benannt werden sollen, wenn sie in das Scene 7 Publishing System hochgeladen werden.

Wenn Sie Bilddateien verwenden, können Sie die Bilder beim Hochladen beschneiden oder eine Maske aus deren Beschneidungspfaden erstellen.

Klicken Sie in der Symbolleiste für globale Navigation auf „Hochladen“, um eine PSD-Datei oder andere Bilddateien von Ihrem Computer in einen Ordner in SPS hochzuladen. Siehe [Hochladen von Vorlagendateien](uploading-template-files.md#uploading_template_files).

**2. Erstellen von Vorlagen**

Um eine Vorlage basierend auf einer PSD-Datei zu erstellen, wählen Sie beim Hochladen der Datei die Option „Vorlage erstellen“. Um eine Vorlage basierend auf Bildern zu erstellen, wählen Sie „Erstellen“ &gt; „Vorlagen aus Grundelementen“, geben Sie einen Wert für die Breite und Höhe der Arbeitsfläche ein, wählen Sie „Designer“ oder „Entwickler“ und ziehen Sie die Bilder in den Anzeigebereich „Vorlagen“. Sie können die Bilder auch auswählen, bevor Sie „Erstellen“ &gt; „Vorlagen aus Grundelementen“ wählen. Der Anzeigebereich „Vorlagen aus Grundelementen“ enthält Werkzeuge für folgende Aktivitäten:

* Bildebenen hinzufügen. Um eine Ebene hinzuzufügen, ziehen Sie ein Bild in den Anzeigebereich „Vorlage“.
* Textebenen hinzufügen. Wählen Sie das Text-Werkzeug  aus und ziehen Sie damit einen Rahmen für die Textebene auf. Anschließend können Sie den Text mit den Werkzeugen im Anzeigebereich „Text“ formatieren.
* Größe und Position von Ebenen ändern.
* Anordnung von Ebenen ändern.
* Schatten- und Schein-Effekte auf Bild- und Textebenen anwenden. 

Siehe [Erstellen einer Vorlage](creating-template.md#creating_a_template).

**3. Erstellen von Vorlagenparametern**

Im nächsten Schritt werden die Eigenschaften von Ebenen in Parameter umgewandelt, d. h. parametrisiert, um festzulegen, welche Ebeneneigenschaften in die URL-Zeichenfolge aufgenommen werden. Parameter bieten Ihnen bei der Verwendung von Vorlagen größtmögliche Flexibilität. Nachdem Sie eine Ebeneneigenschaft parametrisiert haben, können Sie den Parameter dynamisch ändern.

Um eine Ebene zu parametrisieren, öffnen Sie die Vorlage im Anzeigebereich „Vorlage“ und klicken Sie neben dem Namen der Ebene auf „Parameter“. Wählen Sie im Anzeigebereich „Parameter“ jeweils die Option neben den Parametern, die Sie hinzufügen möchten. Siehe [Erstellen von Vorlagenparametern](creating-template-parameters.md#creating_template_parameters).

**4. Veröffentlichen von Vorlagen**

Beim Veröffentlichen der Vorlage wird sie auf dynamischen Medienservern gespeichert, damit sie dynamisch an Ihre Website oder Anwendung übertragen werden kann. Die Veröffentlichung aktiviert auch die URL, um die Vorlage von den dynamischen Medienservern für Ihre Website oder Anwendung aufzurufen.

Achten Sie darauf, alle Bilder zu veröffentlichen, die der Vorlage zugeordnet sind.

Um eine Vorlage zu veröffentlichen, markieren Sie sie zur Veröffentlichung und klicken in der Symbolleiste für globale Navigation auf „Veröffentlichen“. Klicken Sie anschließend auf „Veröffentlichungsvorgang starten“. Siehe [Veröffentlichen von Vorlagen](publishing-templates.md#publishing_templates).

**5. Verknüpfen einer Vorlage mit einer Website**

Dynamic Media Classic erstellt urls für Vorlagen und aktiviert die urls, wenn Sie Vorlagen auf dynamischen Medien-Image-Servern veröffentlichen. Sie können diese URL-Zeichenfolgen im Anzeigebereich „Vorschau für Vorlagen“ kopieren.

Wählen Sie im Durchsuchenbedienfeld die Vorlage aus und klicken Sie auf „Vorschau“, um den Anzeigebereich „Vorschau für Vorlagen“ zu öffnen. Wählen Sie anschließend eine Bildvorgabe zum Übertragen der Vorlage aus und klicken Sie auf „URL kopieren“. Die URL, die Sie im Anzeigebereich „Vorschau“ kopiert haben, können Sie anschließend auf Ihrer Website oder in Ihrer Anwendung verwenden. Siehe [Verknüpfen einer Vorlage mit einer Website](linking-template-web-page.md#linking_a_template_to_a_web_page).
