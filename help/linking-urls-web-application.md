---
title: Verknüpfen von URLs mit einer Web-Anwendung
description: Erfahren Sie, wie Sie URLs mit Ihrer Webanwendung verknüpfen.
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
translation-type: tm+mt
source-git-commit: 38d09bb78834c6b3614bf2b96fd6aee5661e0a5a
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 53%

---

# Verknüpfen von URLs mit einer Web-Anwendung{#linking-urls-to-your-web-application}

Ihre Websites und Anwendungen greifen über URL-Zeichenfolgen auf den Inhalt von Dynamic Media Image Server zu. Nachdem Sie ein Bild veröffentlicht haben, aktiviert Dynamic Media Classic eine URL-Zeichenfolge, die auf den Dynamic Media-Image-Servern auf die Bildvorgabe verweist. Sie können die URLs zum Test kopieren und in einen Webbrowser einfügen.

Um diese URL-Zeichenfolgen in Ihre Webseiten und Anwendungen einzufügen, kopieren Sie sie aus Dynamic Media Classic. Die zu einer Bildvorgabe generierte URL-Zeichenfolge ist im Anzeigebereich „Vorschau“ und im Durchsuchenbedienfeld (in der Detailansicht) abrufbar.

## Abrufen einer Bildvorgabe-URL  {#obtaining-an-image-preset-url}

Eine mit einer Bildvorgabe generierte URL-Zeichenfolge lässt sich im Anzeigebereich „Vorschau“ und in der Detailansicht abrufen. Sie können die URL in die Zwischenablage kopieren und dann nach Bedarf einfügen.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

### Abrufen einer Bildvorgabe-URL aus „Vorschau“  {#obtaining-an-image-preset-url-from-preview}

1. Navigieren Sie in der Asset-Bibliothek auf der linken Seite zu den Asset-Ordnern, die das Bild-Asset enthalten, das Sie in der Vorschau anzeigen möchten.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie über dem Assets-Fenster auf der rechten Seite der Symbolleiste auf **[!UICONTROL „Rasteransicht“]**. Wählen Sie im Fenster &quot;Asset&quot;ein einzelnes Bild-Asset aus und klicken Sie anschließend unter dem Miniaturbild auf **[!UICONTROL Vorschau]** > **[!UICONTROL Bildvorgabe-Liste]**.
   * Klicken Sie über dem Assets-Fenster auf der rechten Seite der Symbolleiste auf **[!UICONTROL „Listenansicht“]**. Wählen Sie im Fenster &quot;Asset&quot;ein einzelnes Bild-Asset aus und klicken Sie dann rechts neben dem Miniaturbild auf **[!UICONTROL Vorschau]** > **[!UICONTROL Bildvorgabe-Liste]**.
   * Klicken Sie über dem Assets-Fenster auf der rechten Seite der Symbolleiste auf **[!UICONTROL „Detailansicht“]**. Klicken Sie in derselben Symbolleiste auf **[!UICONTROL Vorschau]** > **[!UICONTROL Bildvorgabe-Liste]**.

1. (Optional) Wählen Sie in der Liste &quot;Bildvorgabe&quot;in der Dropdown-Liste &quot;URL-Kodierung für URL-kopieren-Generierung&quot;die URL-Kodierung aus, die Sie beim Kopieren der Bild-Asset-URL auf die URL anwenden möchten.
1. Klicken Sie im Fenster &quot;Bildvorgabe-Liste&quot;oben rechts im Bereich &quot;Vorschau&quot;für den ausgewählten Vorgabentyp auf **[!UICONTROL URL kopieren]**.
1. Klicken Sie in der rechten unteren Ecke des Fensters &quot;Bildvorgabe&quot;auf **[!UICONTROL Schließen]**, um zum Bildschirm &quot;Assets&quot;zurückzukehren.

### Abrufen einer Bildvorgabe-URL im Durchsuchenbedienfeld {#obtaining-an-image-preset-url-from-the-browse-panel}

1. Navigieren Sie in der Asset-Bibliothek auf der linken Seite zu den Asset-Ordnern, die das Bild-Asset enthalten, das Sie in der Vorschau anzeigen möchten.
1. Klicken Sie über dem Assets-Fenster auf der rechten Seite der Symbolleiste auf **[!UICONTROL „Rasteransicht“]**. Wählen Sie im Fenster „Asset“ ein einzelnes Bild-Asset aus.
1. Klicken Sie über dem Assets-Fenster auf der rechten Seite der Symbolleiste auf **[!UICONTROL „Detailansicht“]**. 
1. Klicken Sie im Bedienfeld auf der rechten Seite des Bildschirms auf **[!UICONTROL URLs]**, um die Liste der Bildvorgaben zu entfalten.
1. Klicken Sie auf den Link **[!UICONTROL URL kopieren]** neben dem Namen der Bildvorgabe mit der URL, die Sie in die Zwischenablage kopieren möchten.

## URL-Zeichenfolgen zu Bildvorgaben {#about-image-preset-url-strings}

Ein URL-Aufruf zur Bildgrößenänderung für Dynamic Media-Image-Server hat die folgende grundlegende Syntax:

*Pfad*/*Name des Image-Servers*/*Kontoname*/*Bildname*?*Modifikator1*&amp;*Modifikator2*&amp;...

In einer Dynamic Media Image Server-URL werden nach dem Fragezeichen (?) Anweisungen zum Anzeigen des Bildes an den Server gesendet. Beispielsweise wird mit dem folgenden URL-Aufruf ein Bild namens „backpack“ mit einer Breite von 250 Pixeln angezeigt:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

Eine Bildvorgabe-URL enthält alle Modifikator-Anweisungen für die Darstellung des Bildes in der richtigen Größe und mit der richtigen Formatierung. Ohne Bildvorgabe sind nach dem Fragezeichen (?) sämtliche Modifikator-Anweisungen in der URL-Zeichenfolge angegeben:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

Bei einer URL-Zeichenfolge, die mit einer Bildvorgabe generiert wurde, ist statt der Vorgabenanweisungen der Name der Bildvorgabe angegeben – hier das Beispiel analog zur langen URL oben:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

Bildvorgabennamen in URLs sind in Dollarzeichen ($) eingeschlossen. Wenn ein Dynamic Media-Image-Server auf den Bildvorgabenteil der URL stößt (in diesem Fall auf das `Large`), verwenden Sie die Größen- und Formatierungsanweisungen, die in der Bildvorgabe &quot;Groß&quot;definiert sind.

## Einfügen dynamischer Bilder in Websites {#adding-dynamic-images-to-your-web-page}

Um Ihrer Webseite dynamische Bilder hinzuzufügen, wird das `<IMG>`-Tag im HTML-Code Ihrer Website in der Regel mithilfe der URL-Zeichenfolge von Dynamic Media Classic geändert, um eine Anforderung an Dynamic Media Image Servers zu senden. Mit der Zeichenfolge wird das Bild in der Größe und Formatierung gemäß Bildvorgabe dargestellt.

Der typische Aufruf zum Öffnen eines statischen Bildes wäre beispielsweise dies:

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

Mit dem Tag `<IMG>`ersetzen Sie nun den Verweis auf ein statisches Bild durch einen Bildvorgabenaufruf für die Dynamic Media Classic-Plattform. Hier ein Beispiel:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

In diesem Beispiel sucht ein Dynamic Media-Image-Server die Definition von `$thumbnail$` und generiert dynamisch das entsprechende Bild mit den Größen- und Formatierungsspezifikationen, die in der `thumbnail`Bildvorgabe definiert sind. In einer URL-Zeichenfolge sind normalerweise alle Elemente für die Seitenvorlage unveränderlich, ausgenommen der Produktbild-Dateiname (in diesem Fall `backpack_trns`). Das einzige Element, das automatisch von Ihrem kommerziellen Server in die Seitenvorlage eingefügt wird, ist die IPS-ID bzw. der Name des Bildes.
