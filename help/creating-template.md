---
title: Erstellen einer Vorlage
description: Erfahren Sie, wie Sie eine Vorlage in Dynamic Media Classic erstellen.
uuid: c762224b-7c6c-4434-bada-c26570079645
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 8f7093da-d215-4337-ac95-69f0a5bf8648
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
translation-type: tm+mt
source-git-commit: 223bbacab2f244b91763de2ea324a5c8d777feb9
workflow-type: tm+mt
source-wordcount: '3382'
ht-degree: 52%

---

# Erstellen einer Vorlage {#creating-a-template}

Um eine Vorlage zu erstellen, klicken Sie auf **[!UICONTROL Erstellen]** > **[!UICONTROL Vorlagen aus Grundelementen]**. Wählen Sie entweder „Designer“ oder „Entwickler“ aus. Auf dieser Seite können Sie Bild- und Textebenen hinzufügen. Darüber hinaus können Sie sowohl die Anordnung als auch die Größe und Position von Ebenen ändern sowie Schatten- und Schein-Effekte auf Bilder und Text anwenden.

>[!NOTE]
>
>Wenn Sie eine Vorlage bearbeiten, die in einer früheren Version von Dynamic Media Classic erstellt wurde, werden Sie beim Speichern gefragt: &quot;Möchten Sie eine Arbeitsflächenebene hinzufügen?&quot; Klicken Sie auf **[!UICONTROL Nein]**, um das Hinzufügen einer Basisebene zu vermeiden. Wenn Sie versehentlich auf **[!UICONTROL Ja]** klicken, löschen Sie die Modifikatoren `&allowCanvasPrompt` und `&layer=0` in der URL und drücken Sie die Eingabetaste **[!UICONTROL oder**[!UICONTROL  Return ]**.]**

## Erstellen der Ausgangsvorlage {#creating-the-initial-template}

Wenn Sie einen Vorlagensatz erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| **[!UICONTROL Nach]** Auswahl der Option &quot;Nach dem Speichern veröffentlichen&quot;vor dem Speichern veröffentlichen? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

Sie können Vorlagen aus einer vorhandenen Vorlage erstellen. Öffnen Sie die vorhandene Vorlage, klicken Sie auf **[!UICONTROL Speichern unter]** und geben Sie im Dialogfeld „Speichern unter“ einen neuen Namen ein.

**So erstellen Sie einen ersten Vorlagensatz:**

1. Verwenden Sie zum Erstellen der Ausgangsvorlage eine der folgenden Methoden:

   * **Wählen Sie zuerst**  die PSD-Datei oder die Bilder aus. Wählen Sie im Durchsuchenbedienfeld die PSD-Datei bzw. die Bilder aus, die Sie für die Vorlage verwenden möchten, und klicken Sie auf  **[!UICONTROL Erstellen]** > Grundlagen der  **[!UICONTROL Vorlage]**.

   * **Beginn im Anzeigebereich**  &quot;Vorlage&quot;- Klicken Sie auf  **[!UICONTROL &quot;Erstellen]** &quot;> &quot; **[!UICONTROL Vorlagen aus Grundelementen]**&quot;. Wählen Sie entweder „Designer“ oder „Entwickler“ aus. 

1. Geben Sie im Dialogfeld „Größe der Arbeitsfläche eingeben“ Werte für die Breite und Höhe der Vorlage ein.
1. Wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die PSD-Datei bzw. die Bilder, die Sie für die Vorlage verwenden möchten, in den Anzeigebereich „Vorlage“.
1. Wenn Sie fertig sind, stellen Sie sicher, dass rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Klicken Sie auf **[!UICONTROL Speichern]**.
1. Wählen Sie einen Ordner zum Speichern der Vorlage aus, geben Sie einen Namen für die Vorlage ein und klicken Sie auf **[!UICONTROL Absenden]**.

   Dynamic Media Classic schrumpft bei Bedarf die Bilder, um sie auf die Arbeitsfläche zu passen, die sich im Anzeigebereich &quot;Vorlage&quot;befindet, um die Vorlage zu definieren.

## Bearbeiten eines Vorlagensatzes {#editing-a-template-set}

Unabhängig davon, ob Sie einen veröffentlichten oder unveröffentlichten Vorlagensatz bearbeiten, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| Set bereits veröffentlicht? | **[!UICONTROL Nach]** Auswahl der Option &quot;Nach dem Speichern veröffentlichen&quot;veröffentlichen, bevor Sie Ihre Bearbeitung speichern? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |--- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten den Status „veröffentlicht“ bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sei einen Vorlagensatz:**

1. Navigieren Sie in der Ansicht &quot;Raster&quot;zu einem Vorlagensatz und klicken Sie anschließend unter dem Bild auf **[!UICONTROL Bearbeiten]**.
1. Ändern Sie die Vorlage nach Bedarf.
1. Wenn Sie die Bearbeitung abgeschlossen haben, stellen Sie sicher, dass  rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Klicken Sie auf **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **[!UICONTROL Speichern]**.

## Löschen einer Vorlage  {#deleting-a-template}

Wenn Sie einen Vorlagensatz löschen, wird der Satz in den Papierkorb verschoben. Die Mitglieder (bzw. die untergeordneten Elemente) innerhalb des Sets sind davon jedoch nicht betroffen; sie behalten ihren jeweiligen Status „veröffentlicht“ oder „unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie eine Vorlage:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht eine oder mehrere Vorlagen aus.
1. Klicken Sie in der globalen Navigationsleiste auf **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.

## Erklärungen zum Bildschirm „Vorlage“ {#understanding-the-template-screen}

Der Anzeigebereich „Vorlage“ enthält Werkzeuge zum Bearbeiten und Parametrisieren von Ebenen:

Zum Erstellen von Vorlagen stehen Ihnen im Anzeigebereich „Vorlage“ die folgenden Werkzeuge zur Verfügung:

* **Schwenken-Werkzeug** : Hiermit können Sie Ebenen auswählen, sie um die Arbeitsfläche verschieben, ihre Größe ändern oder sie drehen.

* **Textwerkzeug** : Erstellt eine Textebene. Ziehen Sie das Werkzeug auf die Arbeitsfläche, um eine Textebene zu erstellen, und geben Sie dann den gewünschten Text in der Ebene ein. Siehe [Erstellen einer Textebene](#creating-a-text-layer).

* **Schaltfläche**  &quot;Vorschau&quot;: Öffnet den Anzeigebereich &quot;Vorschau&quot;und zeigt die Vorlage in einem Zoom-Viewer an. Sie sehen dann, wie die Vorlage auf der Website bzw. in der Anwendung aussehen wird.

* **Schaltfläche &quot;Parameterzusammenfassung&quot;** Öffnet den Anzeigebereich &quot;Parameterzusammenfassung&quot;. Darin werden die Namen aller Ebenen in der Vorlage sowie für jede Ebene die Namen der aktivierten Parameter angezeigt.

* **Texteditor Version 4.3 und Texteditor Version 4.2** - Sie können den neuesten und am häufigsten verwendeten Texteditor, Texteditor Version 4.3 oder den vorherigen Texteditor, Texteditor Version 4.2, verwenden. Beim Erstellen von Vorlagen ist Texteditor Version 4.3 standardmäßig ausgewählt. Beim Bearbeiten älterer Vorlagen ist Texteditor Version 4.2 standardmäßig ausgewählt. Texteditor Version 4.3 unterstützt derzeit keine Umbrüche. Verwenden Sie daher Texteditor Version 4.2, wenn Sie ältere Vorlagen bearbeiten, die Umbrüche verwenden, um die Funktionsfähigkeit der Vorlage beizubehalten. Wenn Ihre ältere Vorlage keine Umbrüche verwendet, können Sie Texteditor Version 4.3 wählen, um die vielen neuen Funktionen zu nutzen, die sie Angebot. Sie können beispielsweise Ränder vergrößern, Ränder verkleinern, Text in allen Kapiteln einstellen und Text einpassen.

   >[!NOTE]
   >
   >In Dynamic Media Classic wird möglicherweise Texteditor Version 4.2 entfernt. Daher wird empfohlen, nach Möglichkeit Texteditor Version 4.3 zu verwenden. Die Option „Wortumbruch“ wird in einer späteren Version von Texteditor enthalten sein.

* **Designer und Entwickler**  - Wählen Sie die Option, die Ihre Rolle am besten beschreibt.

* **Arbeitsfläche** : Definiert den gesamten verfügbaren Bereich zum Definieren der Vorlage in Pixel. Die Standardgröße beträgt 300 x 300 Pixel. Ebenen werden auf der Arbeitsfläche platziert.

* **Liste**  der Ebenen: Liste der Namen der Ebenen in der Vorlage. Um eine Ebene auszuwählen, markieren Sie deren Namen in der Liste „Ebenen“. Die Liste „Ebenen“ enthält Werkzeuge, mit denen Ebenen mit Effekten versehen, gelöscht, umsortiert und parametrisiert werden können. Siehe [Arbeiten mit Ebenen](#working-with-layers).

* **Bereich**  &quot;Ebeneneigenschaften&quot;- Angebote zum Ändern der Hintergrundfarbe, Deckkraft, Größe und Position einer Ebene sowie der Hintergrundfarbe, Deckkraft und Größe der Arbeitsfläche. Außerdem können Sie hier die Schatten- und Schein-Effekte anpassen. Siehe [Arbeiten mit Ebenen](#working-with-layers).

## Erstellen von Bildebenen  {#creating-image-layers}

1. Ziehen Sie das Bild von der Asset-Bibliothek auf die Arbeitsfläche.

   Der ID-Name des Bilds wird in der Liste „Ebenen“ angezeigt.

   >[!NOTE]
   >
   >Bei Bedarf schrumpft Dynamic Media Classic die Bilder, damit sie beim Erstellen einer Bildebene in die Arbeitsfläche passen.

## Erstellen einer Textebene {#creating-a-text-layer}

1. Klicken Sie auf das Tool **[!UICONTROL Text]**.
1. Ziehen Sie, um ein Textfeld auf der Arbeitsfläche oder auf einem Bild zu erstellen.
1. Über den eingeblendeten Anzeigebereich „Text“ können Sie Text einfügen, indem Sie unter der Registerkarte „Vorgabe“ die folgenden Schritte ausführen:

   * Geben Sie Text in das Textfeld ein. Um den Text in das Textfeld einzupassen, wählen Sie „Text einpassen“.
   * Fügen Sie Text aus der Zwischenablage in das Textfeld ein.

1. Klicken Sie auf **[!UICONTROL Apply]** und schließen Sie dann den Anzeigebereich &quot;Text&quot;.

### Formatieren von Text {#format-text}

Gehen Sie wie folgt vor, um Text in einer Textebene zu formatieren:

1. Doppelklicken Sie in der Liste „Ebenen“ auf den Namen des Textfelds, dessen Inhalt Sie bearbeiten möchten. Der Texteditor wird geöffnet.
1. Wählen Sie im Textfeld den zu formatierenden Text aus. Sie können den gesamten Text, Teile des Textes oder einzelne Zeichen auswählen.
1. Legen Sie die gewünschten Formatierungsoptionen fest und klicken Sie dann auf **[!UICONTROL Apply]**.

   * **Schrift** : Wählen Sie im Menü &quot;Schrift&quot;eine Schrift aus. Wenn eine gewünschte Schriftart nicht im Menü angezeigt wird, können Sie sie in Dynamic Media Classic hochladen. Siehe Schriftarten.

   * **Schriftgröße** : Wählen Sie im Menü eine Schriftgröße aus, geben Sie eine bestimmte Größe in das Feld ein oder klicken Sie auf die  **** Nach-oben- **** Nach-unten-Taste, um die Schriftgröße um zwei Punkte zu vergrößern oder zu verkleinern.

   * **Farbe** : Klicken Sie auf , um eine Farbe für den Text auszuwählen.

   * **Fett, Kursiv oder Unterstrichen** : Wählen Sie den Text aus und klicken Sie dann auf das Symbol für die Formatierung, die Sie auf den Text anwenden möchten.

   * **&quot;Großbuchstaben&quot;, &quot;Hochgestellt&quot;oder &quot;Tiefgestellt** &quot;- Wählen Sie den Text aus und klicken Sie dann auf das Symbol für die Formatierung, die Sie auf den Text anwenden möchten.

   * **Ausrichtung** : Wählen Sie eine Ausrichtungsschaltfläche aus, um Text in der Textebene linksbündig, zentriert oder rechtsbündig auszurichten.

   * **Verfolgung** : Geben Sie einen numerischen Wert ein, um den der Abstand zwischen den Wörtern angepasst werden soll, oder wählen Sie diesen aus.

   * **Kerning** : Geben Sie einen numerischen Wert ein, um den der Abstand zwischen Zeichen angepasst werden soll, oder wählen Sie einen solchen aus.

   * **Zeilenabstand** : Geben Sie einen numerischen Wert ein, um den der Abstand zwischen den Zeilen angepasst werden soll, oder wählen Sie diesen aus.

   * **Grundlinienversatz** : Geben Sie einen numerischen Wert ein, um den ein ausgewähltes Zeichen relativ zur Grundlinie des umgebenden Textes nach oben oder unten verschoben werden soll, oder wählen Sie diesen aus. Diese Option ist insbesondere hilfreich, wenn Sie Brüche von Hand eingeben oder die Position von eingebundenen Grafiken anpassen.

>[!NOTE]
>
>Klicken Sie auf **[!UICONTROL Rückgängig]**, um Ihre letzte Aktion umzukehren. Klicken Sie auf **[!UICONTROL Wiederholen]**, wenn Sie Ihre Meinung zum Umkehren einer Aktion ändern möchten, nachdem Sie auf **[!UICONTROL Rückgängig]** geklickt haben.

### Formatieren von Absätzen {#format-paragraphs}

1. Doppelklicken Sie in der Liste „Ebenen“ auf den Namen des Textfelds, dessen Inhalt Sie bearbeiten möchten. Der Texteditor wird geöffnet.
1. Wählen Sie den Absatz, den Sie formatieren möchten.
1. Legen Sie die gewünschten Formatierungsoptionen fest und klicken Sie dann auf **[!UICONTROL Apply]**.

   * **Ausrichtung** : Klicken Sie auf , um den Ausrichtungstyp anzugeben: ausrichten, zentrieren, rechts ausrichten oder ausrichten.

   * **Absatzende-Ausrichtung** : Klicken Sie auf , um die Art der Ausrichtung für die letzte Zeile im Absatz anzugeben: letzte Zeile links ausrichten; letzte Zeile zentriert; und die letzte Zeile rechts ausgerichtet wird.

   * **Zeilenabstand** : Geben Sie einen numerischen Wert ein, um den der Abstand zwischen allen Zeilen im Absatz angepasst werden soll, oder wählen Sie diesen aus.

   * **Alle**  einrücken: Klicken Sie auf , um den Einzug des Textes zu erhöhen.

   * **Einzug**  entfernen: Klicken Sie auf , um den Einzug des Textes zu verringern.

   * **Erste Zeile**  einrücken: Geben Sie den Einzug für die erste Textzeile an.

   * **Abstand vor Absatz** : Geben Sie den Abstand an, der über der ersten Textzeile im Absatz angezeigt werden soll.

   * **Abstand nach Absatz** : Geben Sie den Abstand an, der unter der letzten Textzeile im Absatz angezeigt werden soll.

   * **Vertikale Ausrichtung** : Wählen Sie aus, wo der Text vertikal im Textfeld angezeigt werden soll: Oben, Mitte, unten.

   * **Textrichtung** : Wählen Sie die Richtung aus, in der der Text angezeigt werden soll: von rechts nach links oder von links nach rechts.

### Anpassen der Eigenschaften der Textebene {#adjust-text-layer-properties}

1. Wählen Sie im Anzeigebereich „Vorlagen aus Grundelementen“ das Textfeld aus, das Sie anpassen möchten.
1. Wählen Sie im Feld „Ebeneneigenschaften“ eine der folgenden Optionen:

   * **Text verkleinern (nur Texteditor Version 4.2)**  - Wenn Sie den Text verkleinern möchten, können Sie ihn in das Textfeld einpassen.

   * **Wortumbruch (nur Texteditor Version 4.2)** - Um anzugeben, ob oder wie der Text umgebrochen wird, wählen Sie eine Umbruchoption:

   * **Umschließen** : Umfasst den Text, um in ein Textfeld einzupassen, das horizontal zu klein ist.

   * **Kein Umbruch** : Wendet den Text nicht an, wenn das Textfeld horizontal zu klein ist, und schneidet stattdessen einen Teil des Textes ab.

   * **NB Wrap** - (kein Umbruch) Umfasst Text, um ihn in ein Textfeld einzupassen, ohne dass Wörter umbrochen werden.

   * **Position** : Gibt die Position des Textfelds auf der Arbeitsfläche an.

   * **Auffüllung** : Fügt Ränder hinzu oder beschneidet das Rechteck der Ebene. Geben Sie die Anzahl der Pixel für links, oben, unten und rechts an, die hinzugefügt bzw. entfernt werden sollen. Geben Sie positive Zahlen ein, um einen Rand oder negative Zahlen zum Beschneiden hinzuzufügen.

### Anzeigen und Bearbeiten des Text-Quell-Codes {#view-and-edit-text-source-code}

Die im Texteditor auf der Registerkarte „Quelle“ angegebenen Informationen dienen nur zur Referenz. Bearbeiten Sie diesen Text nur, wenn Sie mit der Bearbeitung von Quell-Code vertraut sind.

1. Doppelklicken Sie in der Liste „Ebenen“ auf den Namen des Textfelds, dessen Inhalt Sie bearbeiten möchten. Der Texteditor wird geöffnet.
1. Um den Quellcode für den Text anzuzeigen, klicken Sie im Texteditor auf die Registerkarte **[!UICONTROL Quelle]**.
1. Überprüfen oder bearbeiten Sie den Text nach Wunsch.

   Die Änderungen bleiben erhalten, auch wenn Sie zwischen der Vorschau- und der Quell-Ansicht wechseln.

1. Klicken Sie auf **[!UICONTROL Anwenden]**, um die Änderungen anzuzeigen.

## Arbeiten mit Ebenen {#working-with-layers}

Sie können in der Liste „Ebenen“ und im Bereich „Ebeneneigenschaften“ mit Ebenen arbeiten. Sie können die Anordnung von Ebenen sowie ihre Größe und Position ändern, Ebenen drehen und Hintergrund- und Vordergrundfarbe, Deckkraft und Übergangsmodus einer Ebene festlegen.

Sie können außerdem die Größe der Arbeitsfläche ändern sowie deren Hintergrundfarbe und Deckkraft festlegen.

### Neuanordnen von Ebenen  {#reordering-layers}

Eine Änderung der Ebenenreihenfolge kann sich auf das Aussehen auswirken, insbesondere wenn Transparenz oder Überdrucken betroffen sind. Zeigen Sie unbedingt eine Vorschau der Ergebnisse an, bevor Sie die Änderungen festschreiben.

1. Wählen Sie eine der folgenden Vorgehensweisen, um die Ebenen in einer Vorlage neu anzuordnen:

   * Markieren Sie eine Ebene in der Liste „Ebenen“. Klicken Sie dann so oft wie nötig auf **[!UICONTROL Nach oben oder**[!UICONTROL  Nach unten ]**, um die Liste an die richtige Position zu setzen.]**
   * Ziehen Sie eine Ebene in der Liste „Ebenen“ nach oben oder unten.

### Ändern der Größe und Position von Ebenen und der Arbeitsfläche  {#changing-the-size-and-position-of-layers-and-the-canvas}

Ebenen müssen klein genug sein, damit sie auf die Arbeitsfläche passen. Sie können die Größe einer Ebene oder der Arbeitsfläche manuell oder durch Eingabe der Abmessungen ändern. Sie können die Position einer Ebene manuell oder durch Eingabe der Abstandswerte ändern. Sie können eine Ebene auch drehen.

>[!NOTE]
>
>Dynamic Media Classic empfiehlt, eine Bildvorgabe zu erstellen, deren Größe exakt der Größe der Vorlage entspricht. Durch die übereinstimmende Größe zwischen Bildvorgabe und Vorlage wird erreicht, dass die endgültige Ausgabegröße und die Scharfzeichnungsoptionen für die Vorlage korrekt festgelegt sind. Nachdem Sie diese Bildvorgabe erstellt haben, können Sie im Anzeigebereich „Vorschau für Vorlagen“ im Menü „Vorgabe anwenden“ die Bildvorgabe auswählen. Im Anzeigebereich können Sie sehen, wie das Bild aussieht, wenn es vom Server gesendet wird. Siehe [Einstellen von Bildvorgaben](setting-image-presets.md#setting_up_image_presets).

* **Ändern der Größe einer Ebene**  - Um die Größe einer Ebene oder Arbeitsfläche zu ändern, wählen Sie die Ebene oder Arbeitsfläche auf der Liste &quot;Ebenen&quot;aus und führen Sie eine der folgenden Vorgehensweisen aus:

* **Manuelles Ändern der Größe** : Wählen Sie eine Ecke der Ebene oder Arbeitsfläche aus und ziehen Sie sie. Bei Textebenen können Sie auch eine Kante der Ebene ziehen. Halten Sie beim Ziehen die Umschalttaste gedrückt, um die Größe zu ändern, dabei jedoch das Seitenverhältnis (die Form) beizubehalten.

* **Eingeben von Abmessungen**  der Ebenengröße: Geben Sie in den Textfeldern &quot;W&quot;(Breite) und &quot;H&quot;(Höhe) im Bereich &quot;Ebeneneigenschaften&quot;die Pixelmaße ein.

Sie können nicht nur die Größe einer Ebene ändern, sondern auch deren Umrandung erweitern. Geben Sie dazu im Bereich „Ebeneneigenschaften“ in den Feldern „Links“, „Rechts“, „Oben“ und „Unten“ Werte für die erweiterte Umrandung ein. Durch eine erweiterte Umrandung wird der aktuellen Ebene ein Rand hinzugefügt, um den Abstand der Ebene zur Begrenzung ihrer Basisebene zu vergrößern. Eine erweiterte Umrandung ist sinnvoll, wenn Sie einen Schatten-Effekt oder den Effekt „Schein nach außen“ hinzufügen und diesen Effekt deutlicher sichtbar machen möchten. Durch eine erweiterte Umrandung nimmt die Größe der Ebene zu und ihre Hintergrundfarbe wird in dem erweiterten Bereich angezeigt. Die Position der Basisebene wird im Verhältnis zur neuen Größe der Ebene angepasst. Wenn die aktuelle Ebene beispielsweise zentriert in der Basisebene angeordnet ist, führt eine Erweiterung auf der linken Seite der Ebene dazu, dass sie in der Basisebene weiter nach rechts verschoben wird.

* **Ändern der Position einer Ebene**  - Um die Position einer Ebene auf der Arbeitsfläche zu ändern, wählen Sie deren Namen in der Liste &quot;Ebenen&quot;aus und führen Sie eine der folgenden Vorgehensweisen aus:

* **Manuelles Ändern der Position** : Bewegen Sie den Zeiger nahe an eine Ebenengrenze, aber nicht darüber. Wenn Sie den Mauszeiger mit vier Pfeilschaltflächen sehen, klicken Sie auf und ziehen Sie den Beginn.

* **Eingeben von Versatzwerten**  für die Position: Geben Sie in den Textfeldern X und Y die Versatzwerte für die X- und Y-Werte ein. Diese Werte entsprechen dem X- bzw. Y-Abstand des Ankerpunkts in Pixel.

* **Drehen einer Ebene** : Im Feld &quot;Drehen&quot;wird der Winkel Liste, um den die Ebene gedreht wurde. Um eine Ebene zu drehen, wählen Sie deren Namen in der Liste „Ebenen“ aus und führen Sie eine der folgenden Vorgehensweisen aus:

* **Manuelles Drehen** : Bewegen Sie den Cursor nahe an eine Ecke der Ebene, jedoch nicht darüber. Wenn der Cursor für das Drehen angezeigt wird, ziehen Sie die Ecke der Ebene in die gewünschte Richtung. Halten Sie beim Ziehen die Umschalttaste gedrückt, um in Schritten von 15 Grad zu drehen.

* **Eingeben einer Gradmessung**  - Geben Sie die Anzahl der Grad ein, um die die Ebene gedreht werden soll. Die Drehung erfolgt bei positiven Werten im Uhrzeigersinn und bei negativen gegen den Uhrzeigersinn.

**Ausblenden einer Ebene oder eines Ebeneneffekts:**

Sie können eine Ebene oder einen Ebeneneffekt ausblenden, indem Sie auf das Augensymbol  neben dem Ebenennamen oder dem Effektnamen klicken. Ausgeblendete Ebenen werden nicht in Vorschauen oder in der Ausgabe angezeigt. Die Ebeneninformationen werden jedoch nicht aus der URL gelöscht. Stattdessen wird `hide=1` der URL hinzugefügt, um zu beachten, dass die Ebene vor der Ansicht ausgeblendet ist. Beispiel:

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### Bestimmen von Hintergrundfarbe, Deckkraft und Übergangsmodus {#determining-the-background-color-opacity-and-blend-mode}

Um die Hintergrundfarbe, Deckkraft und den Übergangsmodus für eine Ebene oder die Arbeitsfläche auszuwählen, markieren Sie die Ebene oder Arbeitsfläche und führen Sie eine der folgenden Vorgehensweisen aus:

* **Vordergrundfarbe** : Klicken Sie auf  **[!UICONTROL Vordergrundfarbe]** und wählen Sie ein Farbfeld aus, um die Farbe des Schatten- oder Schein-Effekts zu ändern. Sie können auch einen Farbwertparameter in diesem Feld eingeben. Die Hintergrundfarbe wird nur für Ebenen mit Transparenz angewendet. Sie wird beispielsweise auf die teilweise transparente Ebene eines Preisschilds oder den Hintergrund eines Textfelds angewendet. Ebenen, die aus einem PSD-, TIFF- oder PNG-Bild bestehen, in dem Transparenz aktiviert wurde, können einen transparenten Hintergrund haben.

* **Hintergrundfarbe**  - Klicken Sie auf  **[!UICONTROL Hintergrundfarbe]** und wählen Sie ein Farbfeld aus, um die Farbe der aufgefüllten Bereiche zu ändern.

* **Deckkraft** : Ziehen Sie den Schieberegler &quot;Deckkraft&quot;, um eine Ebene durchsichtig zu machen, sodass ein Teil des darunter liegenden Bilds durchscheint. Die Einstellung von 100 % ist undurchsichtig. 0 ist transparent.

* **Übergangsmodus** : Wählen Sie eine Option, um einen der in Photoshop verfügbaren Übergangsmodi zu simulieren. Sie haben die Wahl zwischen „Normal“, „Auflösen“, „Aufhellen“, „Abdunkeln“, „Multiplizieren“ und „Negativ multiplizieren“. Diese Optionen können nur auf Ebenen, nicht jedoch auf die Arbeitsfläche angewendet werden.

## Verwenden von Schatten- und Schein-Effekten mit Ebenen  {#using-shadow-and-glow-effects-on-layers}

Sie können einen Schatten- oder Schein-Effekt auf eine Ebene anwenden. Der Schatten- oder Schein-Effekt wird auf den Umfang der Ebene angewendet und kann nach innen oder außen gerichtet sein, je nachdem, welche Schatten- oder Schein-Option Sie wählen. Wenn Ihre Vorlage aus einer PSD-Datei mit Schatten- und Schein-Effekten stammt, können Sie diese Effekte in Dynamic Media Classic anpassen.

Nachdem Sie einen Schatten- oder Schein-Effekt angewendet haben, können Sie dessen Größe, Farbe, Deckkraft und Position im Bereich „Ebeneneigenschaften“ des Anzeigebereichs „Vorlage“ anpassen.

### Anwenden eines Schatten- oder Schein-Effekts auf eine Ebene  {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Markieren Sie eine Ebene in der Liste „Ebenen“.
1. Wählen Sie im Menü „Effekt hinzufügen“ eine der folgenden Optionen:

   * **Schlagschatten** : Wendet einen Schatten auf den unteren und rechten Rand der Ebene an.

   * **Schatten nach innen** : Wendet einen Schatteneffekt innerhalb aller Kanten der Ebene an.

   * **Schein nach außen** : Wendet einen Schein-Effekt auf alle Kanten der Ebene an.

   * **Schein nach innen** : Wendet einen Schein-Effekt innerhalb aller Kanten der Ebene an.

Nach dem Anwenden eines Effekts wird dessen Name in der Liste „Ebene“ angezeigt. Um einen Effekt zu löschen, wählen Sie ihn in der Liste &quot;Ebenen&quot;aus und klicken Sie dann auf **[!UICONTROL Löschen]**.

>[!NOTE]
>
>Manchmal kann der Effekt eines Schlagschattens oder eines Schein nach außen nicht angezeigt werden, wenn die darunter liegende Ebene nicht groß genug ist, um sie anzuzeigen. Wenn Sie den Schatten- oder Schein-Effekt nicht sehen können, können Sie der Ebene Werte für die erweiterte Umrandung hinzufügen oder die Anordnung der Ebene ändern. Siehe [Ändern der Größe und Position von Ebenen und Arbeitsfläche](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) und [Neuanordnen von Ebenen](creating-template.md#reordering_layers).

### Anpassen eines Schatten- oder Schein-Effekts {#adjusting-a-shadow-or-glow-effect}

Um einen Schatten- oder Schein-Effekt anzupassen, markieren Sie dessen Namen in der Liste „Ebenen“. Ändern Sie dann im Bereich „Ebeneneigenschaften“ des Anzeigebereichs „Vorlage“ die Einstellungen für den Effekt.

* **Farbe** : Klicken Sie auf &quot;Farbe&quot;und wählen Sie ein Farbfeld aus, um die Farbe des Schatten- oder Schein-Effekts zu ändern. Sie können auch einen Farbwertparameter in diesem Feld eingeben.

* **Deckkraft** : Ziehen Sie den Schieberegler, um die Intensität des Effekts festzulegen. Je geringer die Deckkraftwerte, desto transparenter die Effekte.

* **Übergangsmodus** : Wählen Sie eine Option, um einen der in Photoshop verfügbaren Übergangsmodi zu simulieren. Sie haben die Wahl zwischen „Normal“, „Auflösen“, „Aufhellen“, „Abdunkeln“, „Multiplizieren“ und „Negativ multiplizieren“.

* **Größe** : Geben Sie im Feld &quot;X&quot;und &quot;Y&quot;Messungen ein, um den Schatteneffekt zu vergrößern oder zu verkleinern. Die Größenoptionen sind nur für die Effekte „Schatten nach innen“ und „Schlagschatten“ verfügbar.

* **Vergrößern** : Ziehen Sie den Schieberegler, um den Effekt nach innen oder außen zu erweitern.

* **Weichzeichnen** : Ziehen Sie den Schieberegler, um die weiche Kante an den Kanten des Effekts zu steuern. Je größer der Weichzeichnungswert, desto weicher (undeutlicher) die Kante.

## Maskieren von Ebenen  {#masking-layers}

Über die Schaltfläche „Maske“ in der Liste „Ebenen“ können Sie angeben, wie die Maske oder der Alpha-Kanal einer Ebene verwendet werden soll. Mithilfe der Schaltfläche „Maske“ können Sie den Effekt einer Hintergrundebene auf eine bestimmte Ebene oder die gesamte übergeordnete Ebene in der Vorlage anwenden. Wählen Sie in der Liste &quot;Ebenen&quot;eine Ebene aus und klicken Sie auf **[!UICONTROL Maske]**, um zwischen den folgenden Status zu wechseln:

* Der Hintergrund der Ebene ist deckend.
* Der Inhalt der Ebene erscheint invertiert und der Hintergrund der Ebene ist schwarz gefüllt.
* Der Hintergrund der Ebenen ist Schwarz gefüllt.
