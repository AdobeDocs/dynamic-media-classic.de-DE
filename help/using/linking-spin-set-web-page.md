---
title: Verknüpfen eines Rotationssets mit einer Webseite
description: Erfahren Sie, wie Sie ein Rotationsset mit einer Webseite in Adobe Dynamic Media Classic verknüpfen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 23%

---

# Verknüpfen eines Rotationssets mit einer Webseite{#linking-a-spin-set-to-a-web-page}

Websites und Anwendungen greifen über URL-Zeichenfolgen oder eingebetteten Code auf Dynamic Media Image Server-Inhalte, einschließlich Rotationssets, zu. Diese URL-Zeichenfolgen werden während des Veröffentlichungsvorgangs aktiviert. Um die URL-Zeichenfolge oder den Einbettungscode für Ihr Rotationsset in Ihren Webseiten und Anwendungen zu platzieren, kopieren Sie ihn aus Adobe Dynamic Media Classic.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Kopieren einer Rotationsset-URL {#copying-a-spin-set-url}

1. Wählen Sie im Bedienfeld &quot;Asset-Suche&quot;in der Dropdown-Liste &quot;Anzeigen&quot;die Option **[!UICONTROL Rotationsset]**.
1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der das Rotationsset enthält, dessen Einbettungscode Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld URLs und Einbettungscode auf der rechten Seite **[!UICONTROL URL kopieren]** rechts neben dem gewünschten Viewer aus.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und gehen Sie dann unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL URL kopieren]** aus.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL URL kopieren]** aus.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]** aus. Wechseln Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL URL kopieren]** aus.

## Hinzufügen von Rotationsset-URLs zu Ihrer Webseite {#adding-spin-set-urls-to-your-web-page}

Rotationssets werden wie alle Zoom-Viewer über eine dynamische Seite (ASP oder JSP) implementiert, mit der das Rotationsset in einem Zoom-Fenster angezeigt wird. Der URL-Aufruf an die Adobe Dynamic Media Classic-Plattform folgt demselben Protokoll für den Zoom-Viewer. Der Name der Viewer-Vorgabe hängt jedoch von der Vorgabe ab, die der Administrator als standardmäßige Rotationsset-Viewer-Vorgabe definiert hat. Beispielsweise enthält das folgende Beispiel einer nicht Live-URL-Syntax einen Vorgabennamen mit dem Namen `viewer.jsp` und der SKU-Parameter ist jetzt der Name des Rotationssets:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

Beachten Sie in diesem URL-Syntaxbeispiel (der Link ist nicht live) eine SKU-Nummer ( `sku=backpack_spin`). Die Zeichenfolge nach `sku=` ist der Name des Rotationssets ( `backpack spin`).

## Kopieren des Einbettungscodes eines Rotationsset-Viewers {#copying-the-embed-code-of-a-spin-set-viewer}

Mithilfe der Einbettungscode-Funktion können Sie den Viewer-Code für das ausgewählte Rotationsset überprüfen. Sie können den Code auch in die Zwischenablage kopieren, damit Sie ihn zur Bereitstellung des Viewers auf Ihren Webseiten einfügen können. Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

**So kopieren Sie den Einbettungscode eines Rotationsset-Viewers:**

1. Wählen Sie im Bedienfeld &quot;Asset-Suche&quot;in der Dropdown-Liste &quot;Anzeigen&quot;die Option **[!UICONTROL Rotationsset]**.
1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der das Rotationsset enthält, dessen Einbettungscode Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld URLs und Einbettungscode auf der rechten Seite **[!UICONTROL Einbettungscode]** rechts neben dem gewünschten Viewer aus.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und gehen Sie dann unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL Einbettungscode]** aus.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL Einbettungscode]** aus.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]** aus. Wechseln Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL Einbettungscode]** aus.

1. Wählen Sie im Dialogfeld &quot;Einbettungscode&quot;die Option **[!UICONTROL In Zwischenablage kopieren]**.

   Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

1. Wählen Sie **[!UICONTROL Close]** aus.
