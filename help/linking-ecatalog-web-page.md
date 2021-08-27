---
title: E-Katalog mit einer Webseite verknüpfen
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic einen eCatalog mit einer Webseite verknüpfen.
uuid: 90098a90-180b-477a-8533-24a52a93200b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 140640f2-3ca4-4b6c-a240-5f01be87fa9c
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 38%

---

# E-Katalog mit einer Webseite verknüpfen{#linking-an-ecatalog-to-a-web-page}

Ihre Websites und Anwendungen greifen mithilfe von URL-Zeichenfolgen oder eingebettetem Code auf Dynamic Media Image Server-Inhalte, einschließlich E-Katalogen, zu. Diese URL-Zeichenfolgen werden während des Veröffentlichungsvorgangs aktiviert. Um die URL-Zeichenfolge oder den eingebetteten Code für Ihren E-Katalog in Ihre Webseiten und Anwendungen einzufügen, kopieren Sie ihn aus der Adobe Dynamic Media Classic.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Eine eCatalog-URL kopieren {#copying-an-ecatalog-url}

1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets in der Dropdown-Liste Anzeigen die Option **[!UICONTROL Katalog]** aus.
1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der den E-Katalog enthält, dessen Einbettungscode Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld URLs und Einbettungscode auf der rechten Seite **[!UICONTROL URL]** kopieren rechts neben dem gewünschten Viewer aus.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL URL kopieren]** aus.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL URL kopieren]** aus.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Navigieren Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **URL kopieren** aus.

## Hinzufügen von eCatalog-URLs zur Webseite {#adding-ecatalog-urls-to-your-web-page}

Die am häufigsten verwendete Möglichkeit zum Implementieren eines E-Katalogs ist, eine Verknüpfung in Form einer Miniaturansicht der E-Katalog-Titelseite auf einer Website zu platzieren. Vergewissern Sie sich, dass der E-Katalog im Browser in einem eigenen zentrierten Popup-Fenster angezeigt wird (wenden Sie sich ggf. an die IT-Abteilung Ihres Unternehmens). In dem Fenster darf keine Symbol- und Adressleiste angezeigt werden.

Weitere Informationen und Codebeispiele finden Sie unter [Einbetten des HTML5-E-Katalog-Viewers im Adobe Viewer-Referenzhandbuch](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## Kopieren des Einbettungscodes eines eCatalog-Viewers {#copying-the-embed-code-of-an-ecatalog-viewer}

Mithilfe der Einbettungscode-Funktion können Sie den Viewer-Code für den ausgewählten E-Katalog überprüfen. Sie können den Code auch in die Zwischenablage kopieren, damit Sie ihn in Webseiten für die Bereitstellung des Viewers einfügen können. Die Bearbeitung des Codes ist im Dialogfeld Einbettungscode nicht zulässig.

**So kopieren Sie Einbettungscode eines E-Katalog-Viewers:**

1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets in der Dropdown-Liste Anzeigen die Option **[!UICONTROL Katalog]** aus.
1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der den E-Katalog enthält, dessen Einbettungscode Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld URLs auf der rechten Seite **[!UICONTROL Einbettungscode]** aus.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL Einbettungscode]** aus.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL Einbettungscode]** aus.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Navigieren Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL Einbettungscode]** aus.

1. Wählen Sie im Dialogfeld &quot;Einbettungscode&quot;die Option **[!UICONTROL In Zwischenablage kopieren]**.

   Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

1. Wählen Sie **[!UICONTROL Close]** aus.
