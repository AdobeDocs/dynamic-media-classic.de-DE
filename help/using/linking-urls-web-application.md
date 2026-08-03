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
autotag-review: '2026-05-13T20:03:48.579Z'
TQID: 'https://experienceleague.adobe.com/c8e722KVmasJVtoVl8k7-5vGjvs4Lm-GZavm-TF9fk0'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1960799e4144942d4d9443196e6db425f87c7686
workflow-type: tm+mt
source-wordcount: 821
ht-degree: 14%

---

# Verknüpfen von URLs mit einer Web-Anwendung{#linking-urls-to-your-web-application}

Ihre Websites und Programme greifen mithilfe von URL-Zeichenfolgen auf Dynamic Media Image Server-Inhalte zu. Nach dem Veröffentlichen eines Bildes aktiviert Adobe Dynamic Media Classic eine URL-Zeichenfolge, die auf die Bildvorgabe auf Dynamic Media-Bildservern verweist. Sie können diese URLs in einem Webbrowser zum Testen verwenden.

Um diese URL-Zeichenfolgen in Ihren Web-Seiten und Anwendungen zu platzieren, kopieren Sie sie aus Adobe Dynamic Media Classic. Um eine mit einer Bildvorgabe generierte URL-Zeichenfolge abzurufen, gehen Sie zum Bildschirm Vorschau oder zum Durchsuchen-Panel (in der Detailansicht).

## Abrufen einer Bildvorgaben-URL {#obtaining-an-image-preset-url}

Eine mit einer Bildvorgabe generierte URL-Zeichenfolge lässt sich im Anzeigebereich „Vorschau“ und in der Detailansicht abrufen. Nachdem Sie die URL kopiert haben, wird sie in der Zwischenablage gespeichert, sodass Sie sie nach Bedarf einfügen können.

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
1. Wählen Sie **[!UICONTROL URLs]** im rechten Bereich aus, um die Liste der Bildvorgaben anzuzeigen.
1. Klicken Sie auf **[!UICONTROL Link]** URL kopieren“ neben dem Namen der Bildvorgabe mit der URL, die Sie in die Zwischenablage kopieren möchten.

## Übersicht über die Zeichenfolgen der Bildvorgaben-URLs {#about-image-preset-url-strings}

Ein URL-Aufruf für die Bildgröße auf Dynamic Media-Bildservern weist die folgende grundlegende Syntax auf:

*path*/*name of Image Server*/*account name*/*image name*?*modifier1*&amp;*modifier2*&amp;…

In einer Dynamic Media-Bildserver-URL folgen Anweisungen an den Server für die Anzeige des Bildes dem Fragezeichen (?). Dieser URL-Aufruf liefert beispielsweise ein Bild mit dem Namen „Rucksack“ in einer Breite von 250 Pixel:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

Eine Bildvorgabe-URL enthält alle Modifikator-Anweisungen für die Darstellung des Bildes in der richtigen Größe und mit der richtigen Formatierung. Beachten Sie ohne Bildvorgabe alle Modifikatoranweisungen nach dem Fragezeichen (?) in dieser URL-Zeichenfolge:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

In einer URL-Zeichenfolge, die mit einer Bildvorgabe generiert wird, ersetzt der Name der Bildvorgabe die durch die Bildvorgabe definierten Anweisungen. Wenn Sie sich beispielsweise auf die lange URL oben beziehen, lautet die URL-Zeichenfolge:

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

Bildvorgabennamen in URLs verwenden Dollarzeichen ($). Wenn ein Dynamic Media-Bildserver den Teil der Bildvorgabe der URL verarbeitet (in diesem Fall den `Large`), verwendet er die durch die Bildvorgabe „Groß“ definierten Anweisungen zur Größe und Formatierung.

## Hinzufügen dynamischer Bilder zu einer Web-Seite {#adding-dynamic-images-to-your-web-page}

Beim Hinzufügen dynamischer Bilder zu Web-Seiten wird das `<IMG>`-Tag normalerweise mithilfe der Adobe Dynamic Media Classic-URL-Zeichenfolge geändert, um Bilder von Dynamic Media-Bildservern anzufordern. Mit der Zeichenfolge wird das Bild in der Größe und Formatierung gemäß Bildvorgabe dargestellt.

Der typische Aufruf zum Öffnen eines statischen Bildes wäre beispielsweise dies:

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

Sie verwenden jetzt das Tag `<IMG>` , um den Verweis auf ein statisches Bild durch einen Aufruf der Bildvorgabe an die Adobe Dynamic Media Classic-Plattform zu ersetzen. Hier ein Beispiel:

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$"
```

In diesem Beispiel ruft ein Dynamic Media-Bildserver die Definition von `$thumbnail$` ab und generiert dynamisch das entsprechende Bild mit den in der `thumbnail` Bildvorgabe definierten Größenangaben und Formatierungsspezifikationen. In einer URL-Zeichenfolge werden alle Elemente mit Ausnahme des Produktbilddateinamens (in diesem Fall `backpack_trns`) normalerweise für die Seitenvorlage konfiguriert. Das einzige Element, das automatisch von Ihrem kommerziellen Server in die Seitenvorlage eingefügt wird, ist die IPS-ID bzw. der Name des Bildes.
