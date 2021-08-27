---
title: Verknüpfen eines Rotationssets mit einer Webseite
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic ein Rotationsset mit einer Webseite verknüpfen.
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 40%

---

# Verknüpfen eines Rotationssets mit einer Webseite{#linking-a-spin-set-to-a-web-page}

Websites und Anwendungen greifen über URL-Zeichenfolgen oder eingebetteten Code auf Dynamic Media Image Server-Inhalte, einschließlich Rotationssets, zu. Diese URL-Zeichenfolgen werden während des Veröffentlichungsvorgangs aktiviert. Um die URL-Zeichenfolge oder den Einbettungscode für Ihr Rotationsset auf Ihren Webseiten und in Ihren Anwendungen zu platzieren, kopieren Sie ihn aus der Adobe Dynamic Media Classic.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Kopieren einer Rotationsset-URL {#copying-a-spin-set-url}

1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets in der Dropdown-Liste Anzeigen die Option **[!UICONTROL Rotationsset]** aus.
1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der das Rotationsset enthält, dessen Einbettungscode Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld URLs und Einbettungscode auf der rechten Seite **[!UICONTROL URL]** kopieren rechts neben dem gewünschten Viewer aus.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL URL kopieren]** aus.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL URL kopieren]** aus.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Navigieren Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL URL kopieren]** aus.

## Hinzufügen von Rotationsset-URLs zu Ihrer Web-Seite {#adding-spin-set-urls-to-your-web-page}

Rotationssets werden wie alle Zoom-Viewer über eine dynamische Seite (ASP oder JSP) implementiert, mit der das Rotationsset in einem Zoom-Fenster angezeigt wird. Der URL-Aufruf an die Adobe Dynamic Media Classic-Plattform folgt demselben Protokoll für den Zoom-Viewer. Der Name der Viewer-Vorgabe hängt jedoch von der Vorgabe ab, die der Administrator als standardmäßige Rotationsset-Viewer-Vorgabe definiert hat. In folgendem Syntaxbeispiel enthält die URL (inaktiv) den Vorgabennamen `viewer.jsp`, und der SKU-Parameter entspricht dem Rotationssetnamen:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

Achten Sie in diesem URL-Syntaxbeispiel (inaktiver Link) auf die SKU-Nummer ( `sku=backpack_spin`). Die Zeichenfolge nach `sku=` ist der Name des Rotationssets ( `backpack spin`).

## Kopieren des Einbettungscodes eines Rotationsset-Viewers {#copying-the-embed-code-of-a-spin-set-viewer}

Mithilfe der Einbettungscode-Funktion können Sie den Viewer-Code für das ausgewählte Rotationsset überprüfen. Sie können den Code auch in die Zwischenablage kopieren, damit Sie ihn in Webseiten für die Bereitstellung des Viewers einfügen können. Die Bearbeitung des Codes ist im Dialogfeld Einbettungscode nicht zulässig.

**So kopieren Sie den Einbettungscode eines Rotationsset-Viewers:**

1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets in der Dropdown-Liste Anzeigen die Option **[!UICONTROL Rotationsset]** aus.
1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der das Rotationsset enthält, dessen Einbettungscode Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld URLs und Einbettungscode auf der rechten Seite **[!UICONTROL Einbettungscode]** rechts neben dem gewünschten Viewer aus.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL Einbettungscode]** aus.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL Einbettungscode]** aus.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Navigieren Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL Einbettungscode]** aus.

1. Wählen Sie im Dialogfeld &quot;Einbettungscode&quot;die Option **[!UICONTROL In Zwischenablage kopieren]**.

   Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

1. Wählen Sie **[!UICONTROL Close]** aus.
