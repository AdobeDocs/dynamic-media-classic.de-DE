---
title: Verknüpfen einer Vorlage mit einer Website
description: Erfahren Sie, wie Sie eine Vorlage mit einer Webseite in Adobe Dynamic Media Classic verknüpfen.
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
topic: Administration, Content Management, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 38%

---

# Verknüpfen einer Vorlage mit einer Website{#linking-a-template-to-a-web-page}

Ihre Websites und Anwendungen greifen über URL-Zeichenfolgen auf den Dynamic Media Image Server-Inhalt zu. Nachdem Sie eine Vorlage veröffentlicht haben, aktiviert Adobe Dynamic Media Classic eine URL-Zeichenfolge, die auf Dynamic Media-Image-Servern auf die Vorlage verweist. Sie können diese URL zum Testen in einem Webbrowser einfügen.

Um URL-Zeichenfolgen in Ihren Webseiten und Anwendungen zu platzieren, kopieren Sie sie aus Adobe Dynamic Media Classic. Um eine mit einer Bildvorgabe generierte Vorlagen-URL-Zeichenfolge zu erhalten, gehen Sie zum Bildschirm &quot;Vorschau&quot;oder zum Durchsuchenbedienfeld (in der Detailansicht). Wählen Sie anschließend eine Bildvorgabe aus und klicken Sie auf „URL kopieren“.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Abrufen einer Vorlagen-URL {#obtaining-a-template-url}

Sie können die mit einer Bildvorgabe generierte Zeichenfolge einer Vorlagen-URL im Anzeigebereich „Vorschau für Vorlagen“ abrufen. Sie können die URL in die Zwischenablage kopieren und dann nach Bedarf einfügen. Gehen Sie wie folgt vor, um eine mit einer Bildvorgabe generierte Vorlagen-URL-Zeichenfolge von der Seite &quot;Vorlagenvorschau&quot;abzurufen:

1. Rollover der Vorlage auswählen **[!UICONTROL Vorschau]** Schaltfläche oder gehen Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Vorschau]**.
1. Wählen Sie in den Menüs der Vorgabe die Bildvorgabe, mit der Sie das Vorlagenbild übertragen möchten. Auf der Seite Vorschau wird angezeigt, wie die Vorlage aussieht, wenn sie vom Server bereitgestellt wird.
1. Auswählen **[!UICONTROL URL kopieren]** sodass Sie die URL in die Zwischenablage kopieren können.

## Vorlagen-URLs zu Ihrer Webseite hinzufügen {#adding-template-urls-to-your-web-page}

Wenden Sie sich an Ihr Webseitenentwicklungsteam, um eine Vorlage zu Ihrer Webseite hinzuzufügen und die `<IMG>` -Tag in Ihrem HTML-Webseitencode. Verwenden Sie die Adobe Dynamic Media Classic-URL-Zeichenfolge, um eine Anforderung an Dynamic Media-Bildserver zu senden. Mithilfe einer Commerce-Engine oder des dynamischen Webseiten-Codes wird das Vorlagenbild in der Größe und mit den Formatierungen eingefügt, die Sie in der für die Vorlage ausgewählten Bildvorgabe definiert haben.

>[!MORELIKETHIS]
>
>* [Dynamische Bilder zu Ihrer Webseite hinzufügen](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
