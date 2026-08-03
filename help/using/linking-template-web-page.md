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
autotag-review: '2026-05-13T19:52:27.080Z'
TQID: 'https://experienceleague.adobe.com/c1Un6UFrYZh-tqwPp98shMiTUEEMhkEn1vmxEl2rVq0'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: f55e82148ae9d11c54dda28351743b02c1fb58a4
workflow-type: tm+mt
source-wordcount: 330
ht-degree: 12%

---

# Verknüpfen einer Vorlage mit einer Web-Seite{#linking-a-template-to-a-web-page}

Ihre Websites und Programme greifen mithilfe von URL-Zeichenfolgen auf Dynamic Media Image Server-Inhalte zu. Nach dem Veröffentlichen einer Vorlage aktiviert Adobe Dynamic Media Classic eine URL-Zeichenfolge, die auf die Vorlage auf Dynamic Media-Bildservern verweist. Sie können diese URL zum Testen in einen Webbrowser einfügen.

Um URL-Zeichenfolgen in Ihren Web-Seiten und Anwendungen zu platzieren, kopieren Sie sie aus Adobe Dynamic Media Classic. Um eine mit einer Bildvorgabe generierte Vorlagen-URL-Zeichenfolge abzurufen, gehen Sie zum Bildschirm „Vorschau“ oder zum Durchsuchen-Panel (in der Detailansicht). Wählen Sie anschließend eine Bildvorgabe aus und klicken Sie auf „URL kopieren“.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Abrufen einer Vorlagen-URL {#obtaining-a-template-url}

Sie können die mit einer Bildvorgabe generierte Zeichenfolge einer Vorlagen-URL im Anzeigebereich „Vorschau für Vorlagen“ abrufen. Nachdem Sie die URL kopiert haben, wird sie in der Zwischenablage gespeichert, sodass Sie sie nach Bedarf einfügen können. Gehen Sie wie folgt vor, um eine Vorlagen-URL-Zeichenfolge abzurufen, die mit einer Bildvorgabe auf der Seite „Vorlagenvorschau“ generiert wurde:

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Vorschau]** der Vorlage oder gehen Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Vorschau]**.
1. Wählen Sie über die Menüs der Vorgabe die Bildvorgabe aus, mit der Sie die Vorlage bereitstellen möchten. Auf der Seite Vorschau wird die Vorlage so angezeigt, wie sie vom Server bereitgestellt wird.
1. Wählen Sie **[!UICONTROL URL kopieren]** aus, damit Sie die URL in die Zwischenablage kopieren können.

## Hinzufügen von Vorlagen-URLs zu einer Web-Seite {#adding-template-urls-to-your-web-page}

Um Ihrer Web-Seite eine Vorlage hinzuzufügen, wenden Sie sich an Ihr Web-Seiten-Entwicklungs-Team, um das `<IMG>`-Tag in Ihrem HTML-Web-Seiten-Code zu ändern. Verwenden Sie die Adobe Dynamic Media Classic-URL-Zeichenfolge, um eine Anfrage an Dynamic Media-Bildserver zu senden. Die Commerce-Engine oder der dynamische Web-Seiten-Code fügt das Vorlagenbild in der Größe und mit den Formatierungsspezifikationen ein, die von der Bildvorgabe definiert werden, die Sie für Ihre Vorlage ausgewählt haben.

>[!MORELIKETHIS]
>
>* [Hinzufügen dynamischer Bilder zu einer Web-Seite](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
