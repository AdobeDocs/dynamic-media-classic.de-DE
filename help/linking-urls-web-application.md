---
title: Verknüpfen von URLs mit einer Web-Anwendung
seo-title: Verknüpfen von URLs mit einer Web-Anwendung
description: 'null'
seo-description: Erfahren Sie, wie Sie URLs mit Ihrer Webanwendung verknüpfen.
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 72%

---


# Verknüpfen von URLs mit einer Web-Anwendung{#linking-urls-to-your-web-application}

Ihre Websites und Anwendungen greifen mithilfe von URL-Zeichenfolgen auf Dynamic Media-Image-Server-Inhalte zu. Nachdem Sie ein Bild veröffentlicht haben, aktiviert Dynamic Media Classic eine URL-Zeichenfolge, die auf den Image-Servern von Dynamic Media auf die Bildvorgabe verweist. Sie können die URLs zum Test kopieren und in einen Webbrowser einfügen.

Um diese URL-Zeichenfolgen in Ihre Webseiten und Anwendungen einzufügen, kopieren Sie sie aus Dynamic Media Classic. Die zu einer Bildvorgabe generierte URL-Zeichenfolge ist im Anzeigebereich „Vorschau“ und im Durchsuchenbedienfeld (in der Detailansicht) abrufbar.

## Abrufen einer Bildvorgabe-URL {#obtaining-an-image-preset-url}

Eine mit einer Bildvorgabe generierte URL-Zeichenfolge lässt sich im Anzeigebereich „Vorschau“ und in der Detailansicht abrufen. Sie können die URL in die Zwischenablage kopieren und dann nach Bedarf einfügen.

***Hinweis **: Die URL ist erst aktiv, wenn Sie das Asset veröffentlichen.*

### Abrufen einer Bildvorgabe-URL aus „Vorschau“{#obtaining-an-image-preset-url-from-preview}

1. Navigieren Sie in der Asset-Bibliothek auf der linken Seite zu den Asset-Ordnern, die das Bild-Asset enthalten, das Sie in der Vorschau anzeigen möchten.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie über dem Assets-Fenster auf der rechten Seite der Symbolleiste auf „Rasteransicht“. Wählen Sie im Fenster „Asset“ ein einzelnes Bild-Asset und klicken Sie anschließend unterhalb des Miniaturbilds auf „Vorschau“ > „Bildvorgabeliste“.
   * Klicken Sie über dem Assets-Fenster auf der rechten Seite der Symbolleiste auf „Listenansicht“. Wählen Sie im Fenster „Asset“ ein einzelnes Bild-Asset und klicken Sie anschließend rechts neben dem Miniaturbild auf „Vorschau“ > „Bildvorgabeliste“.
   * Klicken Sie über dem Assets-Fenster auf der rechten Seite der Symbolleiste auf „Detailansicht“. Klicken Sie in der gleichen Symbolleiste auf „Vorschau“ > „Bildvorgabeliste“.

1. (Optional) Wählen Sie unten im Fenster „Bildvorgabeliste“ in der Dropdown-Liste „URL-Kodierung für URL-kopieren-Generierung“ die URL-Kodierung aus, die beim Kopieren der Bild-Asset-URL für die URL verwendet werden soll.
1. Klicken Sie im Fester „Bildvorgabeliste“ im rechten oberen Bereich des Vorschaubereichs auf „URL kopieren“ für den ausgewählten Vorgabetyp.
1. Klicken Sie in der rechten unteren Ecke des Fensters „Bildvorgabeliste“ auf „Schließen“, um zum Assets-Fenster zurückzukehren.

### Abrufen einer Bildvorgabe-URL im Durchsuchenbedienfeld {#obtaining-an-image-preset-url-from-the-browse-panel}

1. Navigieren Sie in der Asset-Bibliothek auf der linken Seite zu den Asset-Ordnern, die das Bild-Asset enthalten, das Sie in der Vorschau anzeigen möchten.
1. Klicken Sie über dem Assets-Fenster auf der rechten Seite der Symbolleiste auf „Rasteransicht“. Wählen Sie im Fenster „Asset“ ein einzelnes Bild-Asset aus.
1. Klicken Sie über dem Assets-Fenster auf der rechten Seite der Symbolleiste auf „Detailansicht“.
1. Klicken Sie im Bereich auf der rechten Seite auf „URLs“, um die Liste der Bildvorgaben einzublenden.
1. Klicken Sie neben dem Namen der Bildvorgabe mit der URL, die Sie in die Zwischenablage kopieren möchten, auf „URL kopieren“.

## URL-Zeichenfolgen zu Bildvorgaben {#about-image-preset-url-strings}

Ein URL-Aufruf zur Bildgrößenänderung für Dynamic Media-Image-Server hat die folgende grundlegende Syntax:

*Pfad*/*Name des Image-Servers*/*Kontoname*/*Bildname*?*Modifikator1*&amp;*Modifikator2*&amp;...

In einer Dynamic Media Image Server-URL werden nach dem Fragezeichen (?) Serveranweisungen zum Anzeigen des  angezeigt. Beispielsweise wird mit dem folgenden URL-Aufruf ein Bild namens „backpack“ mit einer Breite von 250 Pixeln angezeigt:

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

Bildvorgabennamen in URLs sind in Dollarzeichen ($) eingeschlossen. When a Dynamic Media Image Server encounters the Image Preset portion of the URL (the `Large` in this case), using the size and formatting instructions defined by the “Large” Image Preset.

## Einfügen dynamischer Bilder in Websites {#adding-dynamic-images-to-your-web-page}

To add dynamic images to your web page, the `<IMG>` tag in your HTML web page code typically is modified using the Dynamic Media Classic URL string to make a request to Dynamic Media Image Servers. Mit der Zeichenfolge wird das Bild in der Größe und Formatierung gemäß Bildvorgabe dargestellt.

Der typische Aufruf zum Öffnen eines statischen Bildes wäre beispielsweise dies:

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

you now use the `<IMG>`tag to replace the reference to a static image with an Image Preset call to the Dynamic Media Classic platform. Hier ein Beispiel:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

In this example, a Dynamic Media Image Server “looks up” the definition of `$thumbnail$` and dynamically generates the appropriate image with the sizing and formatting specifications defined by the `thumbnail`Image Preset. In einer URL-Zeichenfolge sind normalerweise alle Elemente für die Seitenvorlage unveränderlich, ausgenommen der Produktbild-Dateiname (in diesem Fall `backpack_trns`). Das einzige Element, das automatisch von Ihrem kommerziellen Server in die Seitenvorlage eingefügt wird, ist die IPS-ID bzw. der Name des Bildes.
