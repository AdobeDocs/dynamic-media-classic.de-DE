---
title: '"Kurzanleitung: Vorlagen aus Grundelementen"'
seo-title: '"Kurzanleitung: Vorlagen aus Grundelementen"'
description: 'null'
seo-description: Eine Einführung und ein kurzer Beginn zu den Vorlagen aus Grundelementen, die Ihnen helfen, sich schnell aufzumachen.
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 71%

---


# Kurzanleitung: Vorlagen aus Grundelementen{#quick-start-template-basics}

Vorlagen aus Grundelementen sind dynamisch erstellte und adressierbare Bilddateien mit mehreren Ebenen, z. B. in Bildbearbeitungsanwendungen wie Adobe Photoshop. Im Unterschied zu einer statischen Datei mit Ebenen, z. B. einer PSD-Datei, kann eine Vorlage auch Parameter enthalten. Mithilfe von Parametern können die verschiedenen Aspekte eines Bilds adressiert und angepasst werden.

Eine Vorlage kann eine beliebige Anzahl von Bildebenen und Textebenen enthalten. Sie können eine statische Datei, die Ebenen enthält, z. B. eine PSD-Datei mit Ebenen, in eine Vorlage konvertieren und in Dynamic Media Classic Vorlagen erstellen. Sie können Textebenen in Vorlagen mit Schriftarten erstellen, die Sie in Dynamic Media Classic hochgeladen haben. Nachdem Sie einer Vorlage Text hinzugefügt haben, können Sie ihn formatieren, indem Sie Ausrichtung, Schriftart, Schriftgröße und Schriftfarbe ändern.

Im Anzeigebereich „Parameter“ lassen sich beliebige Aspekte der Vorlage in adressierbare Parameter konvertieren. Auf diese Weise können Sie angeben, welches Bild mit Ebenen bzw. welcher Textwert in der Vorlage verwendet werden soll. Parameter werden mit der URL-Zeichenfolge übergeben, damit Sie das auf dem Image-Server generierte Antwortbild durch dynamisches Ändern eines beliebigen Parameters entsprechend anpassen können.

**Quick Beginn**

Diese Kurzanleitung hilft Ihnen, sich schnell mit Vorlagen aus Grundelementen vertraut zu machen.

**1. Hochladen von Dateien**

Laden Sie zunächst die PSD-Datei oder die Bilddatei für Ihre Vorlage hoch. Dynamic Media Classic unterstützt neben PSD viele Bilddateiformate, aber verlustfreie TIFF- und PNG-Bilder werden für Vorlagen empfohlen, da sie Transparenz ermöglichen.

Wenn Sie eine Vorlage basierend auf einer PSD-Datei erstellen möchten, wählen Sie beim Hochladen der PSD-Datei im Dialogfeld „Upload-Auftragsoptionen“ die Option „Vorlage erstellen“. Wählen Sie außerdem eine Option für die Ebenenbenennung, um Dynamic Media Classic anzugeben, wie PSD-Ebenen benannt werden, wenn sie in Dynamic Media Classic hochgeladen werden.

Wenn Sie Bilddateien verwenden, können Sie die Bilder beim Hochladen beschneiden oder eine Maske aus deren Beschneidungspfaden erstellen.

Klicken Sie in der Symbolleiste für globale Navigation auf &quot;Hochladen&quot;, um eine PSD-Datei oder andere Bilddateien von Ihrem Computer in einen Ordner unter &quot;Dynamic Media Classic&quot;hochzuladen. Siehe [Hochladen von Vorlagendateien](uploading-template-files.md#uploading_template_files).

**2. Erstellen von Vorlagen**

Um eine Vorlage basierend auf einer PSD-Datei zu erstellen, wählen Sie beim Hochladen der Datei die Option „Vorlage erstellen“. Um eine Vorlage basierend auf Bildern zu erstellen, wählen Sie „Erstellen“ > „Vorlagen aus Grundelementen“, geben Sie einen Wert für die Breite und Höhe der Arbeitsfläche ein, wählen Sie „Designer“ oder „Entwickler“ und ziehen Sie die Bilder in den Anzeigebereich „Vorlagen“. Sie können die Bilder auch auswählen, bevor Sie „Erstellen“ > „Vorlagen aus Grundelementen“ wählen. Der Anzeigebereich „Vorlagen aus Grundelementen“ enthält Werkzeuge für folgende Aktivitäten:

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

Beim Veröffentlichen der Vorlage wird diese auf den Image-Servern für dynamische Medien gespeichert, damit sie dynamisch an Ihre Website oder Anwendung übertragen werden kann. Bei der Veröffentlichung wird auch die URL aktiviert, mit der die Vorlage von den Dynamic Media-Image-Servern für Ihre Website oder Anwendung aufgerufen werden kann.

Achten Sie darauf, alle Bilder zu veröffentlichen, die der Vorlage zugeordnet sind.

Um eine Vorlage zu veröffentlichen, markieren Sie sie zur Veröffentlichung und klicken in der Symbolleiste für globale Navigation auf „Veröffentlichen“. Klicken Sie anschließend auf „Veröffentlichungsvorgang starten“. Siehe [Veröffentlichen von Vorlagen](publishing-templates.md#publishing_templates).

**5. Verknüpfen einer Vorlage mit einer Website**

Dynamic Media Classic erstellt URLs für Vorlagen und aktiviert die URLs, wenn Sie Vorlagen auf den Image-Servern für dynamische Medien veröffentlichen. Sie können diese URL-Zeichenfolgen im Anzeigebereich „Vorschau für Vorlagen“ kopieren.

Wählen Sie im Durchsuchenbedienfeld die Vorlage aus und klicken Sie auf „Vorschau“, um den Anzeigebereich „Vorschau für Vorlagen“ zu öffnen. Wählen Sie anschließend eine Bildvorgabe zum Übertragen der Vorlage aus und klicken Sie auf „URL kopieren“. Die URL, die Sie im Anzeigebereich „Vorschau“ kopiert haben, können Sie anschließend auf Ihrer Website oder in Ihrer Anwendung verwenden. Siehe [Verknüpfen einer Vorlage mit einer Website](linking-template-web-page.md#linking_a_template_to_a_web_page).
