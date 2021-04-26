---
title: Verknüpfen eines Rotationssets mit einer Website
description: Erfahren Sie, wie Sie ein Rotationsset mit einer Webseite verknüpfen.
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
feature: Dynamic Media Classic, Viewer, Rotationssets
role: Business Practitioner
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
translation-type: tm+mt
source-git-commit: 38d09bb78834c6b3614bf2b96fd6aee5661e0a5a
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 87%

---

# Verknüpfen eines Rotationssets mit einer Website{#linking-a-spin-set-to-a-web-page}

Websites und Anwendungen greifen mithilfe von URL-Zeichenfolgen oder eingebettetem Code auf Dynamic Media Image Server-Inhalte, einschließlich Rotationssets, zu. Diese URL-Zeichenfolgen werden während des Veröffentlichungsvorgangs aktiviert. Um die URL-Zeichenfolge oder den Einbettungscode für das Rotationsset auf Ihren Webseiten und in Ihren Anwendungen einzufügen, kopieren Sie diese bzw. ihn aus Dynamic Media Classic.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Kopieren der URL eines Rotationssets  {#copying-a-spin-set-url}

1. Klicken Sie im Bedienfeld zum Durchsuchen von Assets in der Dropdown-Liste „Anzeigen“ auf „**[!UICONTROL Rotationsset]**“.
1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der das Rotationsset enthält, dessen Einbettungscode Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Klicken Sie auf „**[!UICONTROL Rasteransicht]**“. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Klicken Sie im URLs- und Code-einbetten-Bedienfeld auf der rechten Seite rechts neben dem gewünschten Viewer auf „**[!UICONTROL URL kopieren]**“.
   * Klicken Sie auf „**[!UICONTROL Rasteransicht]**“. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und klicken Sie anschließend unterhalb des Miniaturbilds auf „**[!UICONTROL Vorschau]**“ > „**[!UICONTROL Viewer-Liste]**“.

      Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**[!UICONTROL URL kopieren]**“.

   * Klicken Sie auf „**[!UICONTROL Listenansicht]**“. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und klicken Sie dann rechts neben dem Miniaturbild auf „**[!UICONTROL Vorschau]**“ > „**[!UICONTROL Viewer-Liste]**“.

      Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**[!UICONTROL URL kopieren]**“.

   * Klicken Sie auf „**[!UICONTROL Rasteransicht]**“, „**[!UICONTROL Listenansicht]**“ oder „**[!UICONTROL Detailansicht]**“. Klicken Sie in der gleichen Symbolleiste auf „**[!UICONTROL Vorschau]**“ > „**[!UICONTROL Viewer-Liste]**“.

      Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**[!UICONTROL URL kopieren]**“.

## Hinzufügen von Rotationsset-URLs zur Website  {#adding-spin-set-urls-to-your-web-page}

Rotationssets werden wie alle Zoom-Viewer über eine dynamische Seite (ASP oder JSP) implementiert, mit der das Rotationsset in einem Zoom-Fenster angezeigt wird. Der URL-Aufruf an die Dynamic Media Classic-Plattform erfolgt nach demselben Protokoll im Zoom-Viewer. Der Name der Viewer-Vorgabe hängt jedoch von der Vorgabe ab, die der Administrator als standardmäßige Rotationsset-Viewer-Vorgabe definiert hat. In folgendem Syntaxbeispiel enthält die URL (inaktiv) den Vorgabennamen `viewer.jsp`, und der SKU-Parameter entspricht dem Rotationssetnamen:

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

Achten Sie in diesem URL-Syntaxbeispiel (inaktiver Link) auf die SKU-Nummer ( `sku=backpack_spin`). Die Zeichenfolge nach `sku=` ist der Name des Rotationssets ( `backpack spin`).

## Kopieren von Einbettungscode eines Rotationsset-Viewers {#copying-the-embed-code-of-a-spin-set-viewer}

Mithilfe der Einbettungscode-Funktion können Sie den Viewer-Code für das ausgewählte Rotationsset überprüfen. Sie können den Code auch in die Zwischenablage kopieren, damit Sie ihn in Webseiten für die Bereitstellung des Viewers einfügen können. Die Bearbeitung des Codes ist im Dialogfeld Einbettungscode nicht zulässig.

**So kopieren Sie den Einbettungscode eines Rotationsset-Viewers:**

1. Klicken Sie im Bedienfeld zum Durchsuchen von Assets in der Dropdown-Liste „Anzeigen“ auf „**[!UICONTROL Rotationsset]**“.
1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der das Rotationsset enthält, dessen Einbettungscode Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Klicken Sie auf „**[!UICONTROL Rasteransicht]**“. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf ein einzelnes Asset, um es in der Detailansicht zu öffnen. Klicken Sie im URLs- und Code-einbetten-Bedienfeld auf der rechten Seite rechts neben dem gewünschten Viewer auf „**[!UICONTROL Code einbetten]**“.
   * Klicken Sie auf „**[!UICONTROL Rasteransicht]**“. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und klicken Sie anschließend unterhalb des Miniaturbilds auf „**[!UICONTROL Vorschau]**“ > „**[!UICONTROL Viewer-Liste]**“.

      Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**[!UICONTROL Code einbetten]**“.

   * Klicken Sie auf „**[!UICONTROL Listenansicht]**“. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und klicken Sie dann rechts neben dem Miniaturbild auf „**[!UICONTROL Vorschau]**“ > „**[!UICONTROL Viewer-Liste]**“.

      Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**[!UICONTROL Code einbetten]**“.

   * Klicken Sie auf „**[!UICONTROL Rasteransicht]**“, „**[!UICONTROL Listenansicht]**“ oder „**[!UICONTROL Detailansicht]**“. Klicken Sie in der gleichen Symbolleiste auf „**[!UICONTROL Vorschau]**“ > „**[!UICONTROL Viewer-Liste]**“.

      Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**[!UICONTROL Code einbetten]**“.

1. Klicken Sie im Dialogfeld „Code einbetten“ auf „**[!UICONTROL In Zwischenablage kopieren]**“.

   Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

1. Klicken Sie auf **[!UICONTROL Schließen]**.
