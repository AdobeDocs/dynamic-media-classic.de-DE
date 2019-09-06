---
title: Verknüpfen einer Vorlage mit einer Website
seo-title: Verknüpfen einer Vorlage mit einer Website
description: 'null'
seo-description: Erfahren Sie, wie Sie eine Vorlage mit einer Webseite verknüpfen.
uuid: f 111 ef 06-4 afc -454 c -86 ce -5 d 640236 d 40 b
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/template_ basics
discoiquuid: 989 dba 7-448 a -45 b 1-b 157-af 50 abb 359 a a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Verknüpfen einer Vorlage mit einer Website{#linking-a-template-to-a-web-page}

Ihre Websites und Anwendungen greifen über URL-Zeichenfolgen auf den Inhalt dynamischer Medien-Image-Server zu. Nachdem Sie eine Vorlage veröffentlicht haben, aktiviert Dynamic Media Classic eine URL-Zeichenfolge, die auf die Vorlage auf dynamischen Medienservern verweist. Sie können diese URL zum Testen in einem Webbrowser einfügen.

Um URL-Zeichenfolgen in Ihre Websites und Anwendungen einfügen zu können, kopieren Sie die URL-Zeichenfolgen aus dem Scene7 Publishing System. Um die mit einer Bildvorgabe generierte Zeichenfolge einer Vorlagen-URL abzurufen, rufen Sie den Anzeigebereich „Vorschau“ oder das Durchsuchenbedienfeld (in der Detailansicht) auf. Wählen Sie anschließend eine Bildvorgabe aus und klicken Sie auf „URL kopieren“.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Abrufen einer Vorlagen-URL {#obtaining-a-template-url}

Sie können die mit einer Bildvorgabe generierte Zeichenfolge einer Vorlagen-URL im Anzeigebereich „Vorschau für Vorlagen“ abrufen. Sie können die URL in die Zwischenablage kopieren und dann nach Bedarf einfügen. Führen Sie die folgenden Schritte aus, um die mit einer Bildvorgabe generierte Zeichenfolge einer Vorlagen-URL aus dem Anzeigebereich „Vorschau für Vorlagen“ abzurufen:

1. Klicken Sie auf die Rollover-Schaltfläche „Vorschau“ oder wählen Sie „Datei“ &gt; „Vorschau“. Der Anzeigebereich „Vorschau“ wird geöffnet.
1. Wählen Sie in den Menüs der Vorgabe die Bildvorgabe, mit der Sie das Vorlagenbild übertragen möchten. Im Anzeigebereich „Vorschau“ können Sie sehen, wie die Vorlage aussieht, wenn sie vom Server übertragen wird.
1. Klicken Sie auf „URL kopieren“, um die URL in die Zwischenablage zu kopieren.

## Hinzufügen von Vorlagen-URLs zur Webseite {#adding-template-urls-to-your-web-page}

To add a template to your web page, consult with your web page development team to modify the `<IMG>` tag in your HTML web page code using the Dynamic Media Classic URL string to make a request to Dynamic Media Image Servers. Mithilfe einer Commerce-Engine oder des dynamischen Webseiten-Codes wird das Vorlagenbild in der Größe und mit den Formatierungen eingefügt, die Sie in der für die Vorlage ausgewählten Bildvorgabe definiert haben.

>[!MORELIKETHIS]
>
>* [Einfügen dynamischer Bilder in Websites](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

