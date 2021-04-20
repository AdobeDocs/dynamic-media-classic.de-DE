---
title: Verknüpfen einer Vorlage mit einer Website
description: Erfahren Sie, wie Sie eine Vorlage mit einer Webseite verknüpfen.
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 68%

---


# Verknüpfen einer Vorlage mit einer Website{#linking-a-template-to-a-web-page}

Ihre Websites und Anwendungen greifen über URL-Zeichenfolgen auf den Inhalt von Dynamic Media Image Server zu. Nachdem Sie eine Vorlage veröffentlicht haben, aktiviert Dynamic Media Classic eine URL-Zeichenfolge, die auf den Dynamic Media-Image-Servern auf die Vorlage verweist. Sie können diese URL zum Testen in einem Webbrowser einfügen.

Um URL-Zeichenfolgen in Ihre Webseiten und Anwendungen einzufügen, kopieren Sie sie aus Dynamic Media Classic. Um die mit einer Bildvorgabe generierte Zeichenfolge einer Vorlagen-URL abzurufen, rufen Sie den Anzeigebereich „Vorschau“ oder das Durchsuchenbedienfeld (in der Detailansicht) auf. Wählen Sie anschließend eine Bildvorgabe aus und klicken Sie auf „URL kopieren“.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Abrufen einer Vorlagen-URL  {#obtaining-a-template-url}

Sie können die mit einer Bildvorgabe generierte Zeichenfolge einer Vorlagen-URL im Anzeigebereich „Vorschau für Vorlagen“ abrufen. Sie können die URL in die Zwischenablage kopieren und dann nach Bedarf einfügen. Führen Sie die folgenden Schritte aus, um die mit einer Bildvorgabe generierte Zeichenfolge einer Vorlagen-URL aus dem Anzeigebereich „Vorschau für Vorlagen“ abzurufen:

1. Klicken Sie auf die Rollover-Schaltfläche „Vorschau“ oder wählen Sie „Datei“ > „Vorschau“. Der Anzeigebereich „Vorschau“ wird geöffnet.
1. Wählen Sie in den Menüs der Vorgabe die Bildvorgabe, mit der Sie das Vorlagenbild übertragen möchten. Im Anzeigebereich „Vorschau“ können Sie sehen, wie die Vorlage aussieht, wenn sie vom Server übertragen wird.
1. Klicken Sie auf „URL kopieren“, um die URL in die Zwischenablage zu kopieren.

## Hinzufügen von Vorlagen-URLs zur Webseite  {#adding-template-urls-to-your-web-page}

Um Ihrer Webseite eine Vorlage hinzuzufügen, wenden Sie sich an Ihr Webseitenentwicklungsteam, um das `<IMG>`-Tag im HTML-Webseitencode mit der URL-Zeichenfolge von Dynamic Media Classic zu ändern, um eine Anforderung an Dynamic Media Image Servers zu senden. Mithilfe einer Commerce-Engine oder des dynamischen Webseiten-Codes wird das Vorlagenbild in der Größe und mit den Formatierungen eingefügt, die Sie in der für die Vorlage ausgewählten Bildvorgabe definiert haben.

>[!MORELIKETHIS]
>
>* [Einfügen dynamischer Bilder in Websites](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

