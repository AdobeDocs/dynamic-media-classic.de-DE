---
title: Verknüpfen von Zoom-Viewern mit Web-Seiten
description: Erfahren Sie, wie Sie Zoom-Viewer mit Ihren Web-Seiten in Adobe Dynamic Media Classic verknüpfen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
topic: Administration, Content Management, Development
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 23%

---

# Verknüpfen von Zoom-Viewern mit Web-Seiten{#linking-zoom-viewers-to-your-web-pages}

Ihre Websites und Anwendungen greifen über URL-Zeichenfolgen oder eingebetteten Code auf Dynamic Media Image Server-Inhalte zu. Dieser Zugriff umfasst primäre Bilder und zugehörige Zoom-Ziele. Sie enthält auch Viewer-Vorgaben für Zoom. Diese URL-Zeichenfolgen werden während des Veröffentlichungsvorgangs aktiviert. Um diese URL-Zeichenfolgen oder den eingebetteten Code in Ihren Web-Seiten und Anwendungen zu platzieren, kopieren Sie sie aus Adobe Dynamic Media Classic.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Kopieren einer Zoom-Viewer-URL {#copying-a-zoom-viewer-url}

1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der den Zoom-Viewer enthält, dessen URL Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** oder **[!UICONTROL Listenansicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld „URLs und Einbettungs-Code“ auf der rechten Seite **[!UICONTROL URL kopieren]** rechts neben dem gewünschten Viewer aus.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Klicken Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle auf **[!UICONTROL URL kopieren]**.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und gehen Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Klicken Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle auf **[!UICONTROL URL kopieren]**.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Wechseln Sie in der Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Klicken Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle auf **[!UICONTROL URL kopieren]**.

## Hinzufügen von Zoom-Viewer-URLs zu einer Web-Seite {#adding-zoom-viewer-urls-to-your-web-page}

In der Regel zoomen Besucher Bilder auf einer Website, indem sie zunächst ein Zoom-Symbol auswählen (oft zeigt das Symbol das Bild einer Lupe). Wenn Sie dieses Symbol auswählen, wird eine dynamische Web-Seite (ASP oder JSP) gestartet, die das Bild in einem Popup-Fenster anzeigt. In diesem Popup-Fenster können die Website-Besucher das Bild dann tatsächlich heranzoomen.

Weitere Informationen und Codebeispiele finden Sie unter [Einbetten des HTML5 Basic Zoom Viewers im Adobe Viewers-Referenzhandbuch](https://experienceleague.adobe.com/de/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Kopieren der Einbettungskopie eines Zoom-Viewers {#copying-the-embed-copy-of-a-zoom-viewer}

Mithilfe der Einbettungscode-Funktion können Sie den Viewer-Code für den ausgewählten Zoom-Viewer überprüfen. Sie können den Code auch in die Zwischenablage kopieren, damit Sie ihn zur Bereitstellung des Viewers in Ihre Web-Seiten einfügen können. Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

**So kopieren Sie den Einbettungs-Code eines Zoom-Viewers:**

1. Navigieren Sie im Bedienfeld „Asset-Bibliothek“ auf der linken Seite zum Asset-Ordner, der den Zoom-Viewer enthält, dessen Einbettungs-Code Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld „URLs und Einbettungs-Code“ auf der rechten Seite **[!UICONTROL Einbettungs-Code]** rechts neben dem gewünschten Viewer aus.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle **[!UICONTROL Einbettungs-Code]** aus.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und gehen Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle **[!UICONTROL Einbettungs-Code]** aus.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Wechseln Sie in der Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle **[!UICONTROL Einbettungs-Code]** aus.

1. Wählen Sie im Dialogfeld „Einbettungs-Code“ die Option **[!UICONTROL In Zwischenablage kopieren]**.

   Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

1. Wählen Sie **[!UICONTROL Schließen]** aus.
