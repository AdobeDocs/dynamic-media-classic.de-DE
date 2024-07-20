---
title: Verknüpfen einer Vorlage mit einer Webseite
description: Erfahren Sie, wie Sie eine Vorlage mit einer Webseite in Adobe Dynamic Media Classic verknüpfen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
topic: Administration, Content Management, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 17%

---

# Verknüpfen einer Vorlage mit einer Webseite{#linking-a-template-to-a-web-page}

Ihre Websites und Anwendungen greifen über URL-Zeichenfolgen auf den Dynamic Media Image Server-Inhalt zu. Nachdem Sie eine Vorlage veröffentlicht haben, aktiviert Adobe Dynamic Media Classic eine URL-Zeichenfolge, die auf Dynamic Media-Image-Servern auf die Vorlage verweist. Sie können diese URL zum Testen in einen Webbrowser einfügen.

Um URL-Zeichenfolgen in Ihren Webseiten und Anwendungen zu platzieren, kopieren Sie sie aus Adobe Dynamic Media Classic. Um eine mit einer Bildvorgabe generierte Vorlagen-URL-Zeichenfolge zu erhalten, gehen Sie zum Bildschirm &quot;Vorschau&quot;oder zum Bedienfeld &quot;Durchsuchen&quot;(in der Detailansicht). Wählen Sie anschließend eine Bildvorgabe aus und klicken Sie auf „URL kopieren“.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Abrufen einer Vorlagen-URL {#obtaining-a-template-url}

Sie können die mit einer Bildvorgabe generierte Zeichenfolge einer Vorlagen-URL im Anzeigebereich „Vorschau für Vorlagen“ abrufen. Sie können die URL in die Zwischenablage kopieren und dann nach Bedarf einfügen. Gehen Sie wie folgt vor, um eine mit einer Bildvorgabe generierte Vorlagen-URL-Zeichenfolge von der Seite &quot;Vorlagenvorschau&quot;abzurufen:

1. Wählen Sie die Rollover-Schaltfläche **[!UICONTROL Vorschau]** der Vorlage aus oder gehen Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Vorschau]** .
1. Wählen Sie in den Menüs der Vorgabe die Bildvorgabe aus, mit der Sie das Vorlagenbild bereitstellen möchten. Auf der Seite Vorschau wird angezeigt, wie die Vorlage aussieht, wenn sie vom Server bereitgestellt wird.
1. Wählen Sie **[!UICONTROL URL kopieren]** aus, damit Sie die URL in die Zwischenablage kopieren können.

## Vorlagen-URLs zu Ihrer Webseite hinzufügen {#adding-template-urls-to-your-web-page}

Wenden Sie sich an Ihr Webseitenentwicklungsteam, um Ihrer Webseite eine Vorlage hinzuzufügen und das Tag `<IMG>` im HTML-Webseitencode zu ändern. Verwenden Sie die Adobe Dynamic Media Classic-URL-Zeichenfolge, um eine Anforderung an Dynamic Media-Bildserver zu senden. Die Commerce-Engine oder der dynamische Webseitencode fügt das Vorlagenbild in der Größe und mit der Formatierungsspezifikation ein, die durch die Bildvorgabe definiert ist, die Sie für Ihre Vorlage auswählen.

>[!MORELIKETHIS]
>
>* [Dynamische Bilder zu Ihrer Webseite hinzufügen](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
