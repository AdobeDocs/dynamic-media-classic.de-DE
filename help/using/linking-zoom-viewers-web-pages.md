---
title: Verknüpfen von Zoom-Viewern mit Webseiten
description: Erfahren Sie, wie Sie Zoom-Viewer mit Ihren Webseiten in Adobe Dynamic Media Classic verknüpfen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
topic: Administration, Content Management, Development
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 27%

---

# Verknüpfen von Zoom-Viewern mit Webseiten{#linking-zoom-viewers-to-your-web-pages}

Ihre Websites und Anwendungen greifen mithilfe von URL-Zeichenfolgen oder eingebettetem Code auf den Dynamic Media Image Server-Inhalt zu, einschließlich Primärbildern und zugehörigen Zoom-Zielen sowie Zoom-Viewer-Vorgaben. Diese URL-Zeichenfolgen werden während des Veröffentlichungsvorgangs aktiviert. Um diese URL-Zeichenfolgen oder den eingebetteten Code in Ihre Webseiten und Anwendungen zu platzieren, kopieren Sie sie aus Adobe Dynamic Media Classic.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Kopieren einer Zoom-Viewer-URL {#copying-a-zoom-viewer-url}

1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der den Zoom-Viewer enthält, dessen URL Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Auswählen **[!UICONTROL Rasteransicht]** oder **[!UICONTROL Listenansicht]**. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bereich URLs und Einbettungscode auf der rechten Seite die Option **[!UICONTROL URL kopieren]** rechts neben dem gewünschten Viewer.
   * Auswählen **[!UICONTROL Rasteransicht]**. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL URL kopieren]**.

   * Auswählen **[!UICONTROL Listenansicht]**. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL URL kopieren]**.

   * Auswählen **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Navigieren Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL URL kopieren]**.

## Hinzufügen von Zoom-Viewer-URLs zu Ihrer Webseite {#adding-zoom-viewer-urls-to-your-web-page}

In der Regel zoomen Besucher Bilder auf einer Website, indem sie zunächst ein Zoom-Symbol auswählen (häufig zeigt das Symbol das Bild einer Lupe an). Durch Auswahl dieses Symbols wird eine dynamische Webseite (ASP oder JSP) gestartet, auf der das Bild in einem Popup-Fenster angezeigt wird. In diesem Popup-Fenster können die Website-Besucher das Bild dann tatsächlich heranzoomen.

Weitere Informationen und Codebeispiele finden Sie unter [Einbetten von HTML 5 Basic Zoom Viewer im Referenzhandbuch für Adobe-Viewer](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Kopieren der Einbettungskopie eines Zoom-Viewers {#copying-the-embed-copy-of-a-zoom-viewer}

Mithilfe der Einbettungscode-Funktion können Sie den Viewer-Code für den ausgewählten Zoom-Viewer überprüfen. Sie können den Code auch in die Zwischenablage kopieren, damit Sie ihn zur Bereitstellung des Viewers auf Ihren Webseiten einfügen können. Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

**So kopieren Sie den Einbettungscode eines Zoom-Viewers:**

1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der den Zoom-Viewer enthält, dessen Einbettungscode Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Auswählen **[!UICONTROL Rasteransicht]**. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bereich URLs und Einbettungscode auf der rechten Seite die Option **[!UICONTROL Einbettungscode]** rechts neben dem gewünschten Viewer.
   * Auswählen **[!UICONTROL Rasteransicht]**. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL Einbettungscode]**.

   * Auswählen **[!UICONTROL Listenansicht]**. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL Einbettungscode]**.

   * Auswählen **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Navigieren Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL Einbettungscode]**.

1. Wählen Sie im Dialogfeld Einbettungscode die Option **[!UICONTROL In Zwischenablage kopieren]**.

   Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

1. Auswählen **[!UICONTROL Schließen]**.
