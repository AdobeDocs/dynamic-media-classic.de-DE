---
title: Verknüpfen von URLs mit einer Webanwendung
description: Erfahren Sie, wie Sie URLs über Adobe Dynamic Media Classic mit Ihrer Webanwendung verknüpfen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
topic: Administration, Content Management, Development
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 26%

---

# Verknüpfen von URLs mit einer Webanwendung{#linking-urls-to-your-web-application}

Ihre Websites und Anwendungen greifen über URL-Zeichenfolgen auf den Dynamic Media Image Server-Inhalt zu. Nachdem Sie ein Bild veröffentlicht haben, aktiviert Adobe Dynamic Media Classic eine URL-Zeichenfolge, die auf Dynamic Media-Bildservern auf die Bildvorgabe verweist. Sie können diese URLs zum Testen in einen Webbrowser einfügen.

Um diese URL-Zeichenfolgen in Ihre Webseiten und Anwendungen zu platzieren, kopieren Sie sie aus Adobe Dynamic Media Classic. Um eine mit einer Bildvorgabe generierte URL-Zeichenfolge abzurufen, gehen Sie zum Bildschirm &quot;Vorschau&quot;oder zum Bedienfeld &quot;Durchsuchen&quot;(in der Detailansicht).

## Abrufen einer Bildvorgabe-URL {#obtaining-an-image-preset-url}

Eine mit einer Bildvorgabe generierte URL-Zeichenfolge lässt sich im Anzeigebereich „Vorschau“ und in der Detailansicht abrufen. Sie können die URL in die Zwischenablage kopieren und dann nach Bedarf einfügen.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

### Abrufen einer Bildvorgabe-URL aus der Vorschau {#obtaining-an-image-preset-url-from-preview}

1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zum Ordner &quot;Asset&quot;, der das Bild-Asset enthält, das in der Vorschau angezeigt werden soll.
1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie über dem Assets-Fenster rechts in der Symbolleiste **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Fenster &quot;Asset&quot;ein einzelnes Bild-Asset aus und navigieren Sie unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Bildvorgabenliste]**.
   * Wählen Sie über dem Assets-Fenster rechts in der Symbolleiste **[!UICONTROL Listenansicht]** aus. Wählen Sie im Fenster &quot;Asset&quot;ein einzelnes Bild-Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Bildvorgabeliste]**.
   * Wählen Sie über dem Assets-Fenster rechts in der Symbolleiste **[!UICONTROL Detailansicht]** aus. Wechseln Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Bildvorgabenliste]**.

1. (Optional) Wählen Sie in der Liste &quot;Bildvorgabe&quot;in der Dropdown-Liste URL-Kodierung für URL-Kopiegenerierung die URL-Kodierung aus, die beim Kopieren auf die URL des Bild-Assets angewendet werden soll.
1. Wählen Sie im Fenster Bildvorgabeliste oben rechts im Vorschaufenster **[!UICONTROL URL kopieren]** für den ausgewählten Vorgabetyp aus.
1. Wählen Sie in der rechten unteren Ecke des Fensters Bildvorgabenliste die Option **[!UICONTROL Schließen]** aus, um zum Assets-Bildschirm zurückzukehren.

### Abrufen einer Bildvorgabe-URL aus dem Bedienfeld &quot;Durchsuchen&quot; {#obtaining-an-image-preset-url-from-the-browse-panel}

1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zum Ordner Asset , der das Bild-Asset enthält, das Sie in der Vorschau anzeigen möchten.
1. Wählen Sie über dem Assets-Fenster rechts in der Symbolleiste **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Fenster „Asset“ ein einzelnes Bild-Asset aus.
1. Wählen Sie über dem Assets-Fenster rechts in der Symbolleiste **[!UICONTROL Detailansicht]** aus.
1. Wählen Sie im Bereich rechts auf dem Bildschirm die Option **[!UICONTROL URLs]** aus, damit Sie die Liste der Bildvorgaben erweitern können.
1. Wählen Sie den Link **[!UICONTROL URL kopieren]** neben dem Namen der Bildvorgabe mit der URL, die Sie in die Zwischenablage kopieren möchten.

## URL-Zeichenfolgen zu Bildvorgaben {#about-image-preset-url-strings}

Ein URL-Aufruf für die Bildgröße an Dynamic Media-Bildserver hat die folgende grundlegende Syntax:

*Pfad*/*Name des Image-Servers*/*Kontoname*/*Bildname*?*Modifikator1*&amp;*Modifikator2*&amp;...

In einer Dynamic Media Image Server-URL werden nach dem Fragezeichen (?) Anweisungen für den Server zur Anzeige des Bildes angezeigt. Beispielsweise liefert dieser URL-Aufruf ein Bild mit dem Namen &quot;backpack&quot;mit einer Breite von 250 Pixel:

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

Bildvorgabennamen in URLs sind in Dollarzeichen ($) eingeschlossen. Wenn ein Dynamic Media-Bildserver auf den Bildvorgabenteil der URL trifft (in diesem Fall auf &quot;`Large`&quot;), wobei die Größen- und Formatierungsanweisungen verwendet werden, die in der Bildvorgabe &quot;Groß&quot;definiert sind.

## Dynamische Bilder zu Ihrer Webseite hinzufügen {#adding-dynamic-images-to-your-web-page}

Beim Hinzufügen dynamischer Bilder zu Ihrer Webseite wird das Tag `<IMG>` im HTML-Seiten-Code in der Regel mithilfe der Adobe Dynamic Media Classic-URL-Zeichenfolge geändert, um eine Anforderung an Dynamic Media-Image-Server zu senden. Mit der Zeichenfolge wird das Bild in der Größe und Formatierung gemäß Bildvorgabe dargestellt.

Der typische Aufruf zum Öffnen eines statischen Bildes wäre beispielsweise dies:

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

Sie verwenden jetzt das Tag `<IMG>`, um den Verweis auf ein statisches Bild durch einen Bildvorgabenaufruf für die Adobe Dynamic Media Classic-Plattform zu ersetzen. Hier ein Beispiel:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$"
```

In diesem Beispiel &quot;sucht&quot;ein Dynamic Media-Bildserver die Definition von `$thumbnail$` und generiert dynamisch das entsprechende Bild mit den Größenangaben und Formatierungsspezifikationen, die in der `thumbnail`Bildvorgabe definiert sind. In einer URL-Zeichenfolge sind alle Elemente mit Ausnahme des Produktbild-Dateinamens ( in diesem Fall `backpack_trns` ) für die Seitenvorlage in der Regel fest verdrahtet. Das einzige Element, das automatisch von Ihrem kommerziellen Server in die Seitenvorlage eingefügt wird, ist die IPS-ID bzw. der Name des Bildes.
