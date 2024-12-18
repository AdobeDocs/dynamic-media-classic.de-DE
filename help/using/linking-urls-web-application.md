---
title: Verknüpfen von URLs mit einer Web-Anwendung
description: Erfahren Sie, wie Sie von Adobe Dynamic Media Classic aus URLs mit Ihrer Web-Anwendung verknüpfen.
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

# Verknüpfen von URLs mit einer Web-Anwendung{#linking-urls-to-your-web-application}

Ihre Websites und Programme greifen über URL-Zeichenfolgen auf Dynamic Media-Bildserver-Inhalte zu. Nach dem Veröffentlichen eines Bildes aktiviert Adobe Dynamic Media Classic eine URL-Zeichenfolge, die auf die Bildvorgabe auf Dynamic Media-Bildservern verweist. Sie können diese URLs zum Testen in einen Webbrowser einfügen.

Um diese URL-Zeichenfolgen in Ihren Web-Seiten und Anwendungen zu platzieren, kopieren Sie sie aus Adobe Dynamic Media Classic. Um eine mit einer Bildvorgabe generierte URL-Zeichenfolge abzurufen, gehen Sie zum Bildschirm Vorschau oder zum Durchsuchen-Panel (in der Detailansicht).

## Abrufen einer Bildvorgaben-URL {#obtaining-an-image-preset-url}

Eine mit einer Bildvorgabe generierte URL-Zeichenfolge lässt sich im Anzeigebereich „Vorschau“ und in der Detailansicht abrufen. Sie können die URL in die Zwischenablage kopieren und dann nach Bedarf einfügen.

>[!NOTE]
>
>Diese URL wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

### Abrufen einer Bildvorgaben-URL aus der Vorschau {#obtaining-an-image-preset-url-from-preview}

1. Navigieren Sie im Bedienfeld „Asset-Bibliothek“ auf der linken Seite zum Asset-Ordner, der das Bild-Asset enthält, das Sie in der Vorschau anzeigen möchten.
1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie über dem Assets-Fenster rechts in der Symbolleiste die Option **[!UICONTROL Rasteransicht]**. Wählen Sie im Fenster „Asset“ ein einzelnes Bild-Asset aus und navigieren Sie dann unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Bildvorgabenliste]**.
   * Wählen Sie über dem Assets-Fenster rechts in der Symbolleiste **[!UICONTROL Listenansicht]** aus. Wählen Sie im Fenster „Asset“ ein einzelnes Bild-Asset aus und gehen Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Bildvorgabenliste]**.
   * Wählen Sie über dem Assets-Fenster rechts in der Symbolleiste die Option **[!UICONTROL Detailansicht]**. Navigieren Sie in der Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Bildvorgabenliste]**.

1. (Optional) Wählen Sie in der Liste der Bildvorgaben in der Dropdown-Liste URL-Codierung für URL-Generierung kopieren die URL-Codierung aus, die beim Kopieren auf die URL des Bild-Assets angewendet werden soll.
1. Wählen Sie im Fenster Bildvorgabenliste oben rechts im Bereich Vorschau die Option **[!UICONTROL URL kopieren]** für den ausgewählten Vorgabetyp aus.
1. Wählen Sie in der rechten unteren Ecke des Fensters Bildvorgabenliste die Option **[!UICONTROL Schließen]** aus, um zum Assets-Bildschirm zurückzukehren.

### Abrufen einer Bildvorgaben-URL über das Durchsuchen-Panel {#obtaining-an-image-preset-url-from-the-browse-panel}

1. Navigieren Sie im Bedienfeld „Asset-Bibliothek“ auf der linken Seite zum Asset-Ordner, der das Bild-Asset enthält, das Sie in der Vorschau anzeigen möchten.
1. Wählen Sie über dem Assets-Fenster rechts in der Symbolleiste die Option **[!UICONTROL Rasteransicht]**. Wählen Sie im Fenster „Asset“ ein einzelnes Bild-Asset aus.
1. Wählen Sie über dem Assets-Fenster rechts in der Symbolleiste die Option **[!UICONTROL Detailansicht]**.
1. Wählen Sie **[!UICONTROL URLs]** im Bedienfeld auf der rechten Bildschirmseite aus, um die Liste der Bildvorgaben zu erweitern.
1. Klicken Sie **[!UICONTROL Link]** URL kopieren) neben dem Namen der Bildvorgabe mit der URL, die Sie in die Zwischenablage kopieren möchten.

## URL-Zeichenfolgen zu Bildvorgaben {#about-image-preset-url-strings}

Ein URL-Aufruf für die Bilddimensionierung an Dynamic Media-Bildserver weist die folgende Grundsyntax auf:

*Pfad*/*Name des Image-Servers*/*Kontoname*/*Bildname*?*Modifikator1*&amp;*Modifikator2*&amp;...

In einer Dynamic Media-Bildserver-URL werden hinter dem Fragezeichen (?) Anweisungen an den Server für die Anzeige des Bildes angezeigt. Dieser URL-Aufruf liefert beispielsweise ein Bild mit dem Namen „Rucksack“ in einer Breite von 250 Pixel:

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

Bildvorgabennamen in URLs sind in Dollarzeichen ($) eingeschlossen. Wenn ein Dynamic Media-Bildserver auf den Bildvorgabenabschnitt der URL (in diesem Fall die `Large`) trifft, verwenden Sie die in der Bildvorgabe „Groß“ definierten Größenanweisungen und Formatierungsanweisungen.

## Hinzufügen dynamischer Bilder zu einer Web-Seite {#adding-dynamic-images-to-your-web-page}

Wenn Sie Ihrer Web-Seite dynamische Bilder hinzufügen, wird das `<IMG>`-Tag im HTML-Seiten-Code normalerweise mithilfe der Adobe Dynamic Media Classic-URL-Zeichenfolge geändert, um eine Anfrage an die Dynamic Media-Bildserver zu senden. Mit der Zeichenfolge wird das Bild in der Größe und Formatierung gemäß Bildvorgabe dargestellt.

Der typische Aufruf zum Öffnen eines statischen Bildes wäre beispielsweise dies:

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

Sie verwenden jetzt das Tag `<IMG>` , um den Verweis auf ein statisches Bild durch einen Aufruf der Bildvorgabe an die Adobe Dynamic Media Classic-Plattform zu ersetzen. Hier ein Beispiel:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$"
```

In diesem Beispiel „sucht“ ein Dynamic Media-Bildserver nach der Definition von `$thumbnail$` und generiert dynamisch das entsprechende Bild mit den in der Bildvorgabe `thumbnail`Bildvorgabe“ definierten Größenangaben und Formatierungsspezifikationen. In einer URL-Zeichenfolge werden alle Elemente mit Ausnahme des Produktbilddateinamens (in diesem Fall `backpack_trns`) normalerweise für die Seitenvorlage fest verdrahtet. Das einzige Element, das automatisch von Ihrem kommerziellen Server in die Seitenvorlage eingefügt wird, ist die IPS-ID bzw. der Name des Bildes.
