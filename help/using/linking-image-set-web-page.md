---
title: Verknüpfen von Bildsets mit Web-Seiten
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic ein Bildset mit einer Web-Seite verknüpfen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: df4e5218-2a66-413c-b247-b2a16d884041
topic: Content Management
level: Intermediate
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 16%

---

# Verknüpfen von Bildsets mit Web-Seiten{#linking-an-image-set-to-a-web-page}

Nachdem Sie ein Bildset veröffentlicht haben, können Sie die zugehörige URL oder den Einbettungs-Code kopieren, um sie auf Ihrer Website oder in Ihrem Programm zu verwenden. Anschließend können Sie die URL bereitstellen oder den eingebetteten Code nach Bedarf einfügen, damit Benutzer das Bildset auf Ihrer Website oder in Ihrem Programm anzeigen können.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Kopieren einer Bildset-URL {#copying-an-image-set-url}

1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets in der Dropdown-Liste Anzeigen die Option **[!UICONTROL Bildset]**.
1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der den Bildsatz enthält, dessen Einbettungscode Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld **[!UICONTROL URLs und Einbettungs]** Code rechts neben dem gewünschten Viewer **[!UICONTROL URL kopieren]** aus.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Klicken Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle auf **[!UICONTROL URL kopieren]**.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und gehen Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Klicken Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle auf **[!UICONTROL URL kopieren]**.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Wechseln Sie in der Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Klicken Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle auf **[!UICONTROL URL kopieren]**.

## Hinzufügen von Bildset-URLs zu einer Web-Seite {#adding-image-set-urls-to-your-web-page}

Die häufigste Methode zur Bereitstellung von Bildsets besteht darin, einen Link (über ein Navigationssymbol) auf Ihrer Web-Seite zu platzieren. Wenn dieser Link ausgewählt ist, wird eine dynamische Seite (JSP) gestartet, auf der das Bildset in einem Popup-Zoomfenster angezeigt wird. Mit dem Link Zoom wird ein Popup-Fenster geöffnet, das die tatsächliche Zoom-Funktion enthält.

Weitere Informationen und Codebeispiele finden Sie im [Embedded HTML5 Zoom Viewer](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2) im Adobe Viewer-Referenzhandbuch.

## Kopieren des eingebetteten Codes eines Bildset-Viewers {#copying-the-embed-code-of-an-image-set-viewer}

Mithilfe der Funktion für eingebetteten Code können Sie den Viewer-Code für das ausgewählte Bildset überprüfen. Sie können den Code auch in die Zwischenablage kopieren, damit Sie ihn zur Bereitstellung des Viewers in Ihre Web-Seiten einfügen können. Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

**So kopieren Sie den eingebetteten Code eines Bildset-Viewers:**

1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets in der Dropdown-Liste Anzeigen die Option **[!UICONTROL Bildset]**.
1. Navigieren Sie im Bedienfeld „Asset-Bibliothek“ auf der linken Seite zu dem Asset-Ordner, der das Bildset enthält, dessen eingebetteten Code Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld „URLs“ auf der rechten Seite **[!UICONTROL Einbettungs-Code]**.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle **[!UICONTROL Einbettungs-Code]** aus.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und gehen Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle **[!UICONTROL Einbettungs-Code]** aus.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **Listenansicht** oder **Detailansicht**. Wechseln Sie in der Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle **[!UICONTROL Einbettungs-Code]** aus.

1. Wählen Sie im **[!UICONTROL Einbettungs]** Code-Dialogfeld die Option **[!UICONTROL In Zwischenablage kopieren]** aus.

   Das Bearbeiten des Codes ist im Dialogfeld **[!UICONTROL Code einbetten]** nicht zulässig.

1. Wählen Sie **[!UICONTROL Schließen]** aus.

>[!MORELIKETHIS]
>
>* [Veröffentlichen](publishing-files.md#publishing_files)
