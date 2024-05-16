---
title: Verknüpfen eines Bildsets mit einer Webseite
description: Erfahren Sie, wie Sie ein Bildset mit einer Web-Seite in Adobe Dynamic Media Classic verknüpfen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: df4e5218-2a66-413c-b247-b2a16d884041
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 17%

---

# Verknüpfen eines Bildsets mit einer Webseite{#linking-an-image-set-to-a-web-page}

Nachdem Sie ein Bildset veröffentlicht haben, können Sie dessen zugehörige URL oder den zugehörigen Einbettungscode für die Verwendung auf Ihrer Website oder in Ihrer Anwendung kopieren. Anschließend können Sie die URL bereitstellen oder den Einbettungscode nach Bedarf einfügen, damit Benutzer das Bildset auf Ihrer Website oder in Ihrer Anwendung anzeigen können.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Kopieren einer Bildset-URL {#copying-an-image-set-url}

1. Wählen Sie im Bedienfeld Asset-Suche in der Dropdown-Liste Anzeigen die Option **[!UICONTROL Bildset]**.
1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zum Asset-Ordner, der das Bildset enthält, dessen Einbettungscode Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Auswählen **[!UICONTROL Rasteransicht]**. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bereich URLs und Einbettungscode auf der rechten Seite die Option **[!UICONTROL URL kopieren]** rechts neben dem gewünschten Viewer.
   * Auswählen **[!UICONTROL Rasteransicht]**. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL URL kopieren]**.

   * Auswählen **[!UICONTROL Listenansicht]**. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL URL kopieren]**.

   * Auswählen **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Navigieren Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL URL kopieren]**.

## Hinzufügen von Bildset-URLs zur Webseite {#adding-image-set-urls-to-your-web-page}

Die gängigste Methode zur Bereitstellung von Bildsets besteht darin, einen Link (über ein Navigationssymbol) auf Ihrer Webseite zu platzieren. Wenn diese Option aktiviert ist, wird eine dynamische Seite (JSP) gestartet, auf der das Bildset in einem Popup-Zoomfenster angezeigt wird. Der Zoom-Link öffnet ein Popup-Fenster, das die eigentliche Zoom-Funktion enthält.

Weitere Informationen und Codebeispiele finden Sie im Abschnitt [Einbetten von HTML5-Zoom-Viewer im Referenzhandbuch für Adobe-Viewer](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Kopieren des Einbettungscodes eines Bildset-Viewers {#copying-the-embed-code-of-an-image-set-viewer}

Mithilfe der Einbettungscode-Funktion können Sie den Viewer-Code für den ausgewählten Bildsatz überprüfen. Sie können den Code auch in die Zwischenablage kopieren, damit Sie ihn zur Bereitstellung des Viewers auf Ihren Webseiten einfügen können. Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

**So kopieren Sie den Einbettungscode eines Bildset-Viewers:**

1. Wählen Sie im Bedienfeld Asset-Suche in der Dropdown-Liste Anzeigen die Option **[!UICONTROL Bildset]**.
1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zum Asset-Ordner, der das Bildset enthält, dessen Einbettungscode Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Auswählen **[!UICONTROL Rasteransicht]**. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bereich &quot;URLs&quot;auf der rechten Seite **[!UICONTROL Einbettungscode]**.
   * Auswählen **[!UICONTROL Rasteransicht]**. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL Einbettungscode]**.

   * Auswählen **[!UICONTROL Listenansicht]**. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL Einbettungscode]**.

   * Auswählen **[!UICONTROL Rasteransicht]**, **Listenansicht** oder **Detailansicht**. Navigieren Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL Einbettungscode]**.

1. Wählen Sie im Dialogfeld Einbettungscode die Option **[!UICONTROL In Zwischenablage kopieren]**.

   Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

1. Auswählen **[!UICONTROL Schließen]**.

>[!MORELIKETHIS]
>
>* [Veröffentlichen](publishing-files.md#publishing_files)
