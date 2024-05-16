---
title: Verknüpfen eines eCatalog mit einer Webseite
description: Erfahren Sie, wie Sie einen eCatalog mit einer Webseite in Adobe Dynamic Media Classic verknüpfen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
topic: Integrations, Development
level: Experienced
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 23%

---

# Verknüpfen eines eCatalog mit einer Webseite{#linking-an-ecatalog-to-a-web-page}

Ihre Websites und Anwendungen greifen mithilfe von URL-Zeichenfolgen oder eingebettetem Code auf Dynamic Media Image Server-Inhalte, einschließlich E-Katalogen, zu. Diese URL-Zeichenfolgen werden während des Veröffentlichungsvorgangs aktiviert. Um die URL-Zeichenfolge oder den eingebetteten Code für Ihren eCatalog in Ihre Webseiten und Anwendungen einzufügen, kopieren Sie ihn aus Adobe Dynamic Media Classic.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Eine eCatalog-URL kopieren {#copying-an-ecatalog-url}

1. Wählen Sie im Bedienfeld Asset-Suche in der Dropdown-Liste Anzeigen die Option **[!UICONTROL Katalog]**.
1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zum Asset-Ordner, der den eCatalog enthält, dessen Einbettungscode Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Auswählen **[!UICONTROL Rasteransicht]**. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bereich URLs und Einbettungscode auf der rechten Seite die Option **[!UICONTROL URL kopieren]** rechts neben dem gewünschten Viewer.
   * Auswählen **[!UICONTROL Rasteransicht]**. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL URL kopieren]**.

   * Auswählen **[!UICONTROL Listenansicht]**. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL URL kopieren]**.

   * Auswählen **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Navigieren Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **URL kopieren**.

## Hinzufügen von eCatalog-URLs zur Webseite {#adding-ecatalog-urls-to-your-web-page}

Die gängigste Methode zur Bereitstellung eines E-Katalogs besteht darin, einen Link in Form einer E-Katalog-Titelseite für Miniaturansichten auf Ihrer Webseite zu platzieren. Vergewissern Sie sich, dass der E-Katalog im Browser in einem eigenen zentrierten Popup-Fenster angezeigt wird (wenden Sie sich ggf. an die IT-Abteilung Ihres Unternehmens). In dem Fenster darf keine Symbol- und Adressleiste angezeigt werden.

Weitere Informationen und Codebeispiele finden Sie unter [Einbetten des E-Katalog-Viewers von HTML 5 in das Adobe Viewer-Referenzhandbuch](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Kopieren des Einbettungscodes eines eCatalog-Viewers {#copying-the-embed-code-of-an-ecatalog-viewer}

Mithilfe der Einbettungscode-Funktion können Sie den Viewer-Code für den ausgewählten E-Katalog überprüfen. Sie können den Code auch in die Zwischenablage kopieren, damit Sie ihn zur Bereitstellung des Viewers auf Ihren Webseiten einfügen können. Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

**So kopieren Sie den Einbettungscode eines eCatalog-Viewers:**

1. Wählen Sie im Bedienfeld Asset-Suche in der Dropdown-Liste Anzeigen die Option **[!UICONTROL Katalog]**.
1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zum Asset-Ordner, der den eCatalog enthält, dessen Einbettungscode Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Auswählen **[!UICONTROL Rasteransicht]**. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bereich &quot;URLs&quot;auf der rechten Seite **[!UICONTROL Einbettungscode]**.
   * Auswählen **[!UICONTROL Rasteransicht]**. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL Einbettungscode]**.

   * Auswählen **[!UICONTROL Listenansicht]**. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL Einbettungscode]**.

   * Auswählen **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Navigieren Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;in der Spalte &quot;Aktionen&quot;der Tabelle die Option **[!UICONTROL Einbettungscode]**.

1. Wählen Sie im Dialogfeld Einbettungscode die Option **[!UICONTROL In Zwischenablage kopieren]**.

   Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

1. Auswählen **[!UICONTROL Schließen]**.
