---
title: Verknüpfen einer Vorlage mit einer Web-Seite
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic eine Vorlage mit einer Web-Seite verknüpfen.
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

# Verknüpfen einer Vorlage mit einer Web-Seite{#linking-a-template-to-a-web-page}

Ihre Websites und Programme greifen über URL-Zeichenfolgen auf Dynamic Media-Bildserver-Inhalte zu. Nachdem Sie eine Vorlage veröffentlicht haben, aktiviert Adobe Dynamic Media Classic eine URL-Zeichenfolge, die auf die Vorlage auf Dynamic Media-Bildservern verweist. Sie können diese URL zum Testen in einen Webbrowser einfügen.

Um URL-Zeichenfolgen in Ihren Web-Seiten und Anwendungen zu platzieren, kopieren Sie sie aus Adobe Dynamic Media Classic. Um eine mit einer Bildvorgabe generierte Vorlagen-URL-Zeichenfolge abzurufen, gehen Sie zum Bildschirm „Vorschau“ oder zum Durchsuchen-Panel (in der Detailansicht). Wählen Sie anschließend eine Bildvorgabe aus und klicken Sie auf „URL kopieren“.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Abrufen einer Vorlagen-URL {#obtaining-a-template-url}

Sie können die mit einer Bildvorgabe generierte Zeichenfolge einer Vorlagen-URL im Anzeigebereich „Vorschau für Vorlagen“ abrufen. Sie können die URL in die Zwischenablage kopieren und dann nach Bedarf einfügen. Gehen Sie wie folgt vor, um eine Vorlagen-URL-Zeichenfolge abzurufen, die mit einer Bildvorgabe auf der Seite „Vorlagenvorschau“ generiert wurde:

1. Wählen Sie die Rollover-Schaltfläche **[!UICONTROL Vorschau]** der Vorlage aus oder gehen Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Vorschau]**.
1. Wählen Sie über die Menüs der Vorgabe die Bildvorgabe aus, mit der Sie das Vorlagenbild bereitstellen möchten. Auf der Vorschauseite sehen Sie, wie die Vorlage aussieht, wenn sie vom Server bereitgestellt wird.
1. Wählen Sie **[!UICONTROL URL kopieren]** aus, damit Sie die URL in die Zwischenablage kopieren können.

## Hinzufügen von Vorlagen-URLs zu einer Web-Seite {#adding-template-urls-to-your-web-page}

Um Ihrer Web-Seite eine Vorlage hinzuzufügen, wenden Sie sich an Ihr Web-Seiten-Entwicklungs-Team, um das `<IMG>`-Tag in Ihrem HTML-Web-Seiten-Code zu ändern. Verwenden Sie die Adobe Dynamic Media Classic-URL-Zeichenfolge, um eine Anfrage an Dynamic Media-Bildserver zu senden. Die Commerce-Engine oder der dynamische Web-Seiten-Code fügt das Vorlagenbild in der Größe und mit der Formatierungsspezifikation ein, die in der Bildvorgabe definiert sind, die Sie für Ihre Vorlage auswählen.

>[!MORELIKETHIS]
>
>* [Hinzufügen dynamischer Bilder zu einer Web-Seite](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
