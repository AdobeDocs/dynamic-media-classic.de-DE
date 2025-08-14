---
title: Erstellen von Vorlagen
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic eine Vorlage erstellen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
topic: Content Management
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '3433'
ht-degree: 36%

---

# Erstellen von Vorlagen

Um eine Vorlage zu erstellen, gehen Sie zu **[!UICONTROL Erstellen]** > **[!UICONTROL Vorlagengrundlagen]**. Wählen Sie entweder „Designer“ oder „Entwickler“ aus. Auf dieser Seite können Sie Bild- und Textebenen hinzufügen. Darüber hinaus können Sie sowohl die Anordnung als auch die Größe und Position von Ebenen ändern sowie Schatten- und Schein-Effekte auf Bilder und Text anwenden.

Siehe auch [Vorlagengrundlagen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) Schulungsvideo.

>[!NOTE]
>
>Wenn Sie eine Vorlage bearbeiten, die mit einer früheren Version von Adobe Dynamic Media Classic erstellt wurde, werden Sie beim Speichern in einer Eingabeaufforderung gefragt: „Möchten Sie eine Arbeitsflächen-Ebene hinzufügen?“ Wählen Sie **[!UICONTROL Nein]**, um das Hinzufügen eines Basisebenen zu vermeiden. Wenn Sie versehentlich **[!UICONTROL Ja]** auswählen, löschen Sie die `&allowCanvasPrompt` und `&layer=0` Modifikatoren in der URL und drücken Sie **[!UICONTROL Eingabetaste]** oder **[!UICONTROL Zurück]**.

## Erstellen der ersten Vorlage {#creating-the-initial-template}

Wenn Sie einen Vorlagensatz erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** auf die Mitglieder des Sets und des Sets wie folgt aus:

| **[!UICONTROL Nach Speichern veröffentlichen]** vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

Sie können Vorlagen aus einer vorhandenen Vorlage erstellen. Öffnen Sie die Vorlage, wählen Sie **[!UICONTROL Speichern unter]** und geben Sie im Dialogfeld Speichern unter einen neuen Namen ein.

**So erstellen Sie die ursprüngliche Vorlage:**

1. Verwenden Sie eine der folgenden Methoden, um Ihre Ausgangsvorlage zu erstellen:

   * **Zuerst die PSD oder die Bilder auswählen**: Wählen Sie im Durchsuchen-Panel die PSD-Datei(en) aus, die Sie für Ihre Vorlage verwenden möchten, und navigieren Sie zu **[!UICONTROL Erstellen]** > **[!UICONTROL Vorlagengrundlagen]**.

   * **Vom Vorlagenbildschirm starten**: Gehen Sie zu **[!UICONTROL Erstellen]** > **[!UICONTROL Vorlagengrundlagen]**. Wählen Sie entweder „Designer“ oder „Entwickler“ aus. 

1. Geben Sie im Dialogfeld Arbeitsflächengröße eingeben die Breite und die Höhenmaße für Ihre Vorlage ein.
1. Wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die PSD-Datei bzw. die Bilder, die Sie für die Vorlage verwenden möchten, in den Anzeigebereich „Vorlage“.
1. Wenn Sie fertig sind, stellen Sie sicher, dass unten rechts auf der Seite **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]** aus.
1. Wählen Sie einen Ordner zum Speichern Ihrer Vorlage aus, geben Sie einen Namen für die Vorlage ein und wählen Sie **[!UICONTROL Senden]**.

   Adobe Dynamic Media Classic verkleinert Bilder, wenn nötig, um sie auf die Arbeitsfläche zu passen, den Bereich auf dem Vorlagenbildschirm, der zum Definieren Ihrer Vorlage verwendet wird.

## Bearbeiten von Vorlagensätzen {#editing-a-template-set}

Unabhängig davon, ob Sie ein veröffentlichtes Set oder ein unveröffentlichtes Vorlagensatz bearbeiten, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** auf die Mitglieder des Sets und des Sets wie folgt aus:

| Set bereits veröffentlicht? | **[!UICONTROL Nach dem Speichern veröffentlichen]** Option vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren veröffentlichten Status bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie einen Vorlagensatz:**

1. Navigieren Sie in der Rasteransicht zu einem Vorlagensatz und wählen Sie dann unter dem Bild **[!UICONTROL Bearbeiten]** aus.
1. Ändern Sie die Vorlage nach Bedarf.
1. Stellen Sie nach Abschluss der Bearbeitung in der unteren rechten Ecke der Seite sicher, dass **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **[!UICONTROL Speichern]**.

## Löschen einer Vorlage

Wenn Sie ein Vorlagensatz löschen, wird das Set selbst in den Papierkorb verschoben. Die Mitglieder (oder „untergeordneten Elemente„) in diesem Set sind jedoch nicht betroffen. Stattdessen behalten sie jeweils ihren vorhandenen Status „Veröffentlicht“ oder „Unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie eine Vorlage:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht eine oder mehrere Vorlagen aus.
1. Navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.

## Grundlegendes zum Vorlagenbildschirm {#understanding-the-template-screen}

Der Anzeigebereich „Vorlage“ enthält Werkzeuge zum Bearbeiten und Parametrisieren von Ebenen:

Verwenden Sie diese Tools auf dem Vorlagenbildschirm, um Vorlagen zu erstellen:

* **[!UICONTROL Schwenken]**: Hiermit können Sie Ebenen auswählen, auf der Arbeitsfläche verschieben, ihre Größe ändern oder drehen.

* **[!UICONTROL Text]**: Erstellt eine Textebene. Ziehen Sie das Werkzeug auf die Arbeitsfläche, um eine Textebene zu erstellen, und geben Sie dann den gewünschten Text in der Ebene ein. Siehe [Erstellen einer Textebene](#creating-a-text-layer).

* **[!UICONTROL Vorschau]**: Öffnet den Bildschirm Vorschau und zeigt die Vorlage in einem Zoom-Viewer an. Sie sehen, wie die Vorlage für Benutzer auf Ihrer Website oder in Ihrem Programm aussieht.

* **[!UICONTROL Parameterzusammenfassung]** Öffnet den Bildschirm Parameterzusammenfassung. Darin werden die Namen aller Ebenen in der Vorlage sowie für jede Ebene die Namen der aktivierten Parameter angezeigt.

* **[!UICONTROL Texteditor v4.3 und Texteditor v4.2]**: Verwenden Sie den neuesten und am besten ausgestatteten Texteditor. Sie können den Texteditor 4.3 oder den vorherigen Texteditor 4.2 verwenden. Beim Erstellen von Vorlagen ist Text-Editor v4.3 standardmäßig ausgewählt. Beim Bearbeiten älterer Vorlagen ist Texteditor Version 4.2 standardmäßig ausgewählt. Der Texteditor v4.3 unterstützt derzeit keinen Zeilenumbruch. Wenn Sie also ältere Vorlagen bearbeiten, die Zeilenumbrüche verwenden, verwenden Sie den Texteditor v4.2, um die Vorlagentreue vollständig zu erhalten. Wenn Ihre ältere Vorlage keinen Zeilenumbruch verwendet, können Sie Texteditor v4.3 verwenden, um die vielen neuen Funktionen zu nutzen, die es bietet. Erhöhen Sie beispielsweise die Ränder, verringern Sie die Ränder, legen Sie Text in Großbuchstaben fest und kopieren Sie den Text.

  >[!NOTE]
  >
  >Die Entfernung von Text Editor v4.2 ist als Option in Adobe Dynamic Media Classic geplant. Es wird empfohlen, nach Möglichkeit Text-Editor 4.3 zu verwenden. Die **[!UICONTROL Zeilenumbruch]**-Option wird in eine zukünftige Version des Texteditors integriert.

* **[!UICONTROL Designer und Entwickler]**: Wählen Sie die Option aus, die Ihre Rolle am besten beschreibt.

* **[!UICONTROL Arbeitsfläche]**: Definiert die gesamte verfügbare Fläche in Pixel, um Ihre Vorlage zu definieren. Die Standardgröße ist 300 × 300 Pixel. Ebenen werden auf der Arbeitsfläche platziert.

* **[!UICONTROL Ebenenliste]**: Listet die Namen der Ebenen in der Vorlage auf. Um eine Ebene auszuwählen, markieren Sie deren Namen in der Liste „Ebenen“. Die Liste „Ebenen“ enthält Werkzeuge, mit denen Ebenen mit Effekten versehen, gelöscht, umsortiert und parametrisiert werden können. Siehe [Arbeiten mit Ebenen](#working-with-layers).

* **[!UICONTROL Ebeneneigenschaftsbereich]**: Dieser Bereich bietet Tools zum Ändern der Hintergrundfarbe, Deckkraft, Größe und Position einer Ebene. Sie können auch die Hintergrundfarbe, Deckkraft und Größe der Arbeitsfläche ändern. Außerdem können Sie hier die Schatten- und Schein-Effekte anpassen. Siehe [Arbeiten mit Ebenen](#working-with-layers).

## Erstellen von Bildebenen {#creating-image-layers}

1. Ziehen Sie das Bild von der Asset-Bibliothek auf die Arbeitsfläche.

   Der ID-Name des Bilds wird in der Liste „Ebenen“ angezeigt.

   >[!NOTE]
   >
   >Bei Bedarf werden Bilder in Adobe Dynamic Media Classic verkleinert, damit sie auf die Arbeitsfläche passen, wenn Sie eine Bildebene erstellen.

## Erstellen einer Textebene {#creating-a-text-layer}

1. Wählen Sie das **[!UICONTROL Text]**-Tool aus.
1. Ziehen Sie, um ein Textfeld auf der Arbeitsfläche oder auf einem Bild zu erstellen.
1. Fügen Sie im sich öffnenden Bildschirm Text Text hinzu, indem Sie einen der folgenden Schritte auf der Registerkarte Vorschau ausführen:

   * Geben Sie Text in das Textfeld ein. Um den Text in das Textfeld einzupassen, wählen Sie „Text einpassen“.
   * Fügen Sie Text aus der Zwischenablage in das Textfeld ein.

1. Klicken Sie **[!UICONTROL Anwenden]** und schließen Sie dann den Bildschirm Text .

### Formatieren von Text {#format-text}

Gehen Sie wie folgt vor, um Text in einer Textebene zu formatieren:

1. Doppelklicken Sie in der Liste „Ebenen“ auf den Namen des Textfelds, dessen Inhalt Sie bearbeiten möchten. Der Texteditor wird geöffnet.
1. Wählen Sie im Textfeld des Texteditors den Text aus, den Sie formatieren möchten. Sie können den gesamten Text, Teile des Textes oder einzelne Zeichen auswählen.
1. Geben Sie eine der folgenden Formatierungsoptionen an und wählen Sie dann **[!UICONTROL Übernehmen]**.

   * **[!UICONTROL Schriftart]**: Wählen Sie im Menü Schriftart eine Schriftart aus. Wenn eine gewünschte Schriftart nicht im Menü angezeigt wird, können Sie sie in Adobe Dynamic Media Classic hochladen. Siehe Schriftarten.

   * **[!UICONTROL Schriftgröße]**: Wählen Sie eine Schriftgröße aus dem Menü aus, geben Sie eine bestimmte Größe in das Feld ein oder wählen Sie die Pfeile **[!UICONTROL Nach oben]** oder **[!UICONTROL Nach unten]** aus, um die Größe um zwei Punkte zu erhöhen oder zu verringern.

   * **[!UICONTROL Farbe]**: Wählen Sie diese Option, um eine Farbe für den Text auszuwählen.

   * **[!UICONTROL Fett]**, **[!UICONTROL Kursiv]** oder **[!UICONTROL Unterstreichen]**: Wählen Sie den Text aus und klicken Sie dann auf das Symbol für die Formatierung, die Sie auf den Text anwenden möchten.

   * **[!UICONTROL Großbuchstaben]**, **[!UICONTROL Hochgestellt]** oder **[!UICONTROL Tiefgestellt]**: Wählen Sie den Text aus und klicken Sie dann auf das Symbol für die Formatierung, die Sie auf den Text anwenden möchten.

   * **[!UICONTROL Ausrichtung]**: Wählen Sie eine Ausrichtungsschaltfläche aus, um Text in der Textebene linksbündig, zentriert oder rechtsbündig auszurichten.

   * **[!UICONTROL Tracking]**: Geben Sie einen numerischen Wert ein, um den der Abstand zwischen Wörtern angepasst werden soll, oder wählen Sie einen solchen aus.

   * **[!UICONTROL Kerning]**: Geben Sie einen numerischen Wert ein, um den der Abstand zwischen den Zeichen angepasst werden soll, oder wählen Sie ihn aus.

   * **[!UICONTROL Zeilenabstand]**: Geben Sie einen numerischen Wert ein, um den der Abstand zwischen Zeilen angepasst werden soll, oder wählen Sie einen solchen aus.

   * **[!UICONTROL Grundlinienverschiebung]**: Geben Sie einen numerischen Wert ein, um den ein ausgewähltes Zeichen relativ zur Grundlinie des umgebenden Textes nach oben oder unten verschoben werden soll, oder wählen Sie ihn aus. Diese Option ist besonders nützlich, wenn Sie Bruchteile per Hand einstellen oder die Position von Inline-Grafiken anpassen.

>[!NOTE]
>
>Wählen **[!UICONTROL Rückgängig]** aus, wenn Sie die letzte Aktion rückgängig machen möchten. Wählen Sie **[!UICONTROL Wiederholen]** aus, wenn Sie Ihre Meinung ändern und eine Aktion rückgängig machen möchten, nachdem Sie **[!UICONTROL Rückgängig]** ausgewählt haben.

### Formatieren von Absätzen {#format-paragraphs}

1. Doppelklicken Sie in der Liste „Ebenen“ auf den Namen des Textfelds, dessen Inhalt Sie bearbeiten möchten. Der Texteditor wird geöffnet.
1. Wählen Sie den Absatz aus, den Sie formatieren möchten.
1. Geben Sie eine der folgenden Formatierungsoptionen an und wählen Sie dann **[!UICONTROL Übernehmen]**.

   * **[!UICONTROL Ausrichtung]**: Geben Sie den Ausrichtungstyp an, indem Sie auf **[!UICONTROL Links ausrichten]**, **[!UICONTROL Zentriert]**, **[!UICONTROL Rechts ausrichten]** oder **[!UICONTROL Blocksatz]** klicken.

   * **[!UICONTROL Ende der Absatzausrichtung]**: Wählen Sie diese Option aus, um die Art der Ausrichtung für die letzte Zeile im Absatz anzugeben: Letzte Zeile wird links ausgerichtet, Letzte Zeile wird zentriert und Letzte Zeile wird rechts ausgerichtet.

   * **[!UICONTROL Zeilenabstand]**: Geben Sie einen numerischen Wert ein, um den der Abstand zwischen allen Zeilen im Absatz angepasst werden soll, oder wählen Sie einen solchen aus.

   * **[!UICONTROL Alle einrücken]**: Wählen Sie diese Option, um den Einzug des Textes zu erhöhen.

   * **[!UICONTROL Einzug entfernen]**: Wählen Sie diese Option, um den Einzug des Textes zu verringern.

   * **[!UICONTROL Erste Zeile einrücken]**: Geben Sie den Betrag an, um den Sie die erste Textzeile einrücken möchten.

   * **[!UICONTROL Leerzeichen vor Absatz]**: Geben Sie den Leerraum an, der über der ersten Textzeile des Absatzes angezeigt werden soll.

   * **[!UICONTROL Leerzeichen nach Absatz]**: Geben Sie den Leerraum an, der unter der letzten Textzeile des Absatzes angezeigt werden soll.

   * **[!UICONTROL Vertikale Ausrichtung]**: Wählen Sie aus, wo der Text vertikal im Textfeld angezeigt werden soll: Oben, Mitte, unten.

   * **[!UICONTROL Textrichtung]**: Wählen Sie die Richtung aus, in der der Text angezeigt werden soll: von rechts nach links oder von links nach rechts.

### Anpassen der Eigenschaften der Textebene {#adjust-text-layer-properties}

1. Wählen Sie im Anzeigebereich „Vorlagen aus Grundelementen“ das Textfeld aus, das Sie anpassen möchten.
1. Wählen Sie im Feld „Ebeneneigenschaften“ eine der folgenden Optionen:

   * **[!UICONTROL Text verkleinern (nur Texteditor v4.2)]**: Wählen Sie diese Option, um den Text so zu verkleinern, dass er in das Textfeld passt.

   * **[!UICONTROL Zeilenumbruch (nur Text-Editor v4.2)]**: Wählen Sie eine Option zum Umbrechen aus, um anzugeben, ob oder wie der Text umgebrochen wird:

   * **[!UICONTROL Umbrechen]**: Umschließt den Text, damit er in ein zu kleines horizontales Textfeld passt.

   * **[!UICONTROL Kein Umbruch]**: Der Text wird nicht umgebrochen, wenn das Textfeld horizontal zu klein ist. Stattdessen wird ein Textabschnitt abgeschnitten.

   * **[!UICONTROL Unterbrechungsfreier Umbruch]**: Schließt Text ein, damit er in ein Textfeld passt, und unterbricht Wörter nicht.

   * **[!UICONTROL Position]**: Gibt die Position des Textfelds auf der Arbeitsfläche an.

   * **[!UICONTROL Abstand]**: Fügt Ränder hinzu oder schneidet das Ebenenrechteck zu. Geben Sie die Anzahl der Pixel an, die Sie für „Links“, „Oben“, „Unten“ und „Rechts“ hinzufügen oder entfernen möchten. Geben Sie positive Zahlen ein, wenn Sie dem Zuschnitt einen Rand oder negative Zahlen hinzufügen möchten.

### Anzeigen und Bearbeiten des Text-Quell-Codes {#view-and-edit-text-source-code}

Die Informationen auf der Registerkarte Source des Texteditors dienen als Referenz. Bearbeiten Sie diesen Text nur, wenn Sie mit der Bearbeitung von Quell-Code vertraut sind.

1. Doppelklicken Sie in der Liste „Ebenen“ auf den Namen des Textfelds, dessen Inhalt Sie bearbeiten möchten. Der Texteditor wird geöffnet.
1. Um den Quell-Code für den Text im Texteditor anzuzeigen, wählen Sie die Registerkarte **[!UICONTROL Source]** im Texteditor.
1. Überprüfen oder bearbeiten Sie den Text nach Wunsch.

   Die Änderungen bleiben erhalten, auch wenn Sie zwischen der Vorschau- und der Quell-Ansicht wechseln.

1. Wählen Sie **[!UICONTROL Anwenden]** aus, um die Bearbeitungen zu rendern.

## Arbeiten mit Ebenen {#working-with-layers}

Sie können in der Liste „Ebenen“ und im Bereich „Ebeneneigenschaften“ mit Ebenen arbeiten. Sie können die Anordnung von Ebenen sowie ihre Größe und Position ändern, Ebenen drehen und Hintergrund- und Vordergrundfarbe, Deckkraft und Übergangsmodus einer Ebene festlegen.

Sie können außerdem die Größe der Arbeitsfläche ändern sowie deren Hintergrundfarbe und Deckkraft festlegen.

### Ebenen neu anordnen {#reordering-layers}

Eine Änderung der Ebenenreihenfolge kann sich auf das Erscheinungsbild auswirken, insbesondere wenn Transparenz oder Überdruck erforderlich sind. Zeigen Sie unbedingt eine Vorschau der Ergebnisse an, bevor Sie die Änderungen festschreiben.

1. Wählen Sie eine der folgenden Vorgehensweisen, um die Ebenen in einer Vorlage neu anzuordnen:

   * Markieren Sie eine Ebene in der Liste „Ebenen“. Wählen Sie dann **[!UICONTROL Nach]** oder **[!UICONTROL Nach unten]** so oft wie nötig aus, um sie an der richtigen Position in der Liste zu platzieren.
   * Ziehen Sie eine Ebene in der Liste „Ebenen“ nach oben oder unten.

### Ändern der Größe und Position von Ebenen und der Arbeitsfläche {#changing-the-size-and-position-of-layers-and-the-canvas}

Ebenen müssen klein genug sein, damit sie auf die Arbeitsfläche passen. Sie können die Größe einer Ebene oder der Arbeitsfläche manuell oder durch Eingabe der Abmessungen ändern. Sie können die Position einer Ebene manuell oder durch Eingabe der Abstandswerte ändern. Sie können eine Ebene auch drehen.

>[!NOTE]
>
>Adobe Dynamic Media Classic empfiehlt, eine Bildvorgabe zu erstellen, die der genauen Größe Ihrer Vorlage entspricht. Durch die übereinstimmende Größe zwischen Bildvorgabe und Vorlage wird erreicht, dass die endgültige Ausgabegröße und die Scharfzeichnungsoptionen für die Vorlage korrekt festgelegt sind. Nachdem Sie diese Bildvorgabe erstellt haben, können Sie sie im Menü Vorgabe anwenden auf dem Bildschirm Vorlagenvorschau auswählen. Im Anzeigebereich können Sie sehen, wie das Bild aussieht, wenn es vom Server gesendet wird. Siehe [Einrichten von ](setting-image-presets.md#setting_up_image_presets).

* **Ändern der Größe einer Ebene**: Um die Größe einer Ebene oder Arbeitsfläche zu ändern, wählen Sie die Ebene oder Arbeitsfläche in der Liste „Ebenen“ aus und verwenden Sie eine der folgenden Techniken:

* **Größe manuell ändern**: Wählen Sie eine Ecke der Ebene oder der Arbeitsfläche aus und ziehen Sie sie. Bei Textebenen können Sie auch eine Kante der Ebene ziehen. Halten Sie die Umschalttaste gedrückt, während Sie ziehen, um die Größe zu ändern, aber das Seitenverhältnis (die Form) beizubehalten.

* **Ebenengrößenmaße eingeben**: Geben Sie in die Textfelder „W“ (Breite) und „H“ (Höhe) im Bereich „Ebeneneigenschaften“ Pixelmaße ein.

Sie können nicht nur die Größe einer Ebene ändern, sondern auch deren Umrandung erweitern. Geben Sie dazu im Bereich „Ebeneneigenschaften“ in den Feldern „Links“, „Rechts“, „Oben“ und „Unten“ Werte für die erweiterte Umrandung ein. Durch eine erweiterte Umrandung wird der aktuellen Ebene ein Rand hinzugefügt, um den Abstand der Ebene zur Begrenzung ihrer Basisebene zu vergrößern. Eine erweiterte Umrandung ist sinnvoll, wenn Sie einen Schatten-Effekt oder den Effekt „Schein nach außen“ hinzufügen und diesen Effekt deutlicher sichtbar machen möchten. Durch eine erweiterte Umrandung nimmt die Größe der Ebene zu und ihre Hintergrundfarbe wird in dem erweiterten Bereich angezeigt. Die Position der Basisebene wird im Verhältnis zur neuen Größe der Ebene angepasst. Wenn die aktuelle Ebene beispielsweise zentriert in der Basisebene angeordnet ist, führt eine Erweiterung auf der linken Seite der Ebene dazu, dass sie in der Basisebene weiter nach rechts verschoben wird.

* **Position einer Ebene ändern**: Um die Position einer Ebene auf der Arbeitsfläche zu ändern, wählen Sie den zugehörigen Namen in der Liste „Ebenen“ aus und verwenden Sie eine der folgenden Techniken:

* **Position manuell ändern**: Bewegen Sie den Mauszeiger in die Nähe, aber nicht über eine Ebenengrenze, und wenn Sie den Cursor mit den vier Spitzen sehen, wählen Sie aus und ziehen Sie.

* **Positionsversatzmessungen eingeben**: Geben Sie die X- und Y-Versatzmessungen in die Textfelder X und Y ein. Diese Werte entsprechen dem X- bzw. Y-Abstand des Ankerpunkts in Pixel.

* **Ebene drehen**: Das Feld „Drehen“ zeigt den Winkel an, in den die Ebene gedreht wurde. Um eine Ebene zu drehen, wählen Sie deren Namen in der Liste „Ebenen“ aus und führen Sie eine der folgenden Vorgehensweisen aus:

* **Manuell drehen**: Bewegen Sie den Mauszeiger in die Nähe der Ebene, aber nicht über eine Ecke der Ebene. Wenn der Cursor für das Drehen angezeigt wird, ziehen Sie die Ecke der Ebene in die gewünschte Richtung. Halten Sie beim Ziehen die Umschalttaste gedrückt, um in Schritten von 15 Grad zu drehen.

* **Gradmessung eingeben**: Geben Sie die Anzahl der Grad ein, um die die Ebene gedreht werden soll. Die Drehung erfolgt bei positiven Werten im Uhrzeigersinn und bei negativen gegen den Uhrzeigersinn.

**Ebene oder Ebeneneffekt ausblenden:**

Sie können einen Layer- oder Ebeneneffekt ausblenden, indem Sie das Augensymbol neben einem Layernamen oder einem Effektnamen auswählen. Ausgeblendete Ebenen werden nicht in Vorschauen oder in der Ausgabe angezeigt. Die Ebeneninformationen werden jedoch nicht aus der URL gelöscht. Stattdessen wird `hide=1` zur URL hinzugefügt, um zu beachten, dass die Ebene nicht sichtbar ist. Beispiel:

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### Bestimmen von Hintergrundfarbe, Deckkraft und Übergangsmodus

Um die Hintergrundfarbe, Deckkraft und den Übergangsmodus für eine Ebene oder die Arbeitsfläche auszuwählen, markieren Sie die Ebene oder Arbeitsfläche und führen Sie eine der folgenden Vorgehensweisen aus:

* **Vordergrundfarbe**: Wählen Sie **[!UICONTROL Vordergrundfarbe]** und wählen Sie ein Farbfeld aus, um die Farbe des Schattens oder Glühens zu ändern. Sie können auch einen Farbwertparameter in diesem Feld eingeben. Die Hintergrundfarbe wird nur für Ebenen mit Transparenz angewendet. Sie wird beispielsweise auf die teilweise transparente Ebene eines Preisschilds oder den Hintergrund eines Textfelds angewendet. Ebenen, die aus einem PSD-, TIFF- oder PNG-Bild bestehen, in dem Transparenz aktiviert wurde, können einen transparenten Hintergrund haben.

* **Hintergrundfarbe**: Wählen Sie **[!UICONTROL Hintergrundfarbe]** und wählen Sie ein Farbfeld, um die Farbe der abgefüllten Bereiche zu ändern.

* **Deckkraft**: Ziehen Sie den Regler für Deckkraft, damit jede Ebene durchsichtig wird, sodass ein Teil des darunter liegenden Bildes angezeigt wird. Die 100-Prozent-Einstellung ist undurchsichtig, 0 ist transparent.

* **Mischmodus**: Wählen Sie eine Option aus, um einen der in Photoshop verfügbaren Mischmodi zu simulieren. Sie haben die Wahl zwischen „Normal“, „Auflösen“, „Aufhellen“, „Abdunkeln“, „Multiplizieren“ und „Negativ multiplizieren“. Diese Optionen können nur auf Ebenen, nicht jedoch auf die Arbeitsfläche angewendet werden.

## Schatten- und Glüheffekte auf Ebenen verwenden {#using-shadow-and-glow-effects-on-layers}

Sie können einen Schatten- oder Schein-Effekt auf eine Ebene anwenden. Der Schatten oder das Leuchten gilt für den Umfang der Ebene und erstreckt sich nach innen oder außen, je nach der gewählten Schatten- oder Leucht-Option. Wenn Ihre Vorlage von einer PSD-Datei mit Shadow- und Glow-Effekten stammt, können Sie diese Effekte in Adobe Dynamic Media Classic anpassen.

Nachdem Sie einen Schatten- oder Schein-Effekt angewendet haben, können Sie dessen Größe, Farbe, Deckkraft und Position im Bereich „Ebeneneigenschaften“ des Anzeigebereichs „Vorlage“ anpassen.

### Anwenden eines Schatten- oder Leuchteffekts auf eine Ebene {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Markieren Sie eine Ebene in der Liste „Ebenen“.
1. Wählen Sie das Menü **[!UICONTROL `Add Effect`]** und dann eine Option aus:

   * **[!UICONTROL Schlagschatten]**: Wendet einen Schatten auf die untere und rechte Seite der Ebene an.

   * **[!UICONTROL Innerer Schatten]**: Wendet einen Schatteneffekt an allen Kanten der Ebene an.

   * **[!UICONTROL Äußerer Glanz]**: Wendet einen Glüheffekt um alle Kanten der Ebene an.

   * **[!UICONTROL Innerer Glanz]**: Wendet einen Glüheffekt an allen Kanten der Ebene an.

Nach dem Anwenden eines Effekts wird dessen Name in der Liste „Ebene“ angezeigt. Um einen Effekt zu löschen, wählen Sie in der Ebenenliste den entsprechenden Namen und anschließend **[!UICONTROL Löschen]** aus.

>[!NOTE]
>
>Manchmal kann der Effekt eines Schlagschattens oder äußeren Glühens nicht angezeigt werden, wenn die darunter liegende Ebene nicht groß genug ist, um ihn anzuzeigen. Wenn Sie den Schatten oder das Leuchten nicht sehen können, sollten Sie der Ebene Abstandswerte hinzufügen oder die Ebene neu anordnen. Siehe [Ändern der Größe und Position von Ebenen und Arbeitsfläche](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) und [Neuanordnen von Ebenen](creating-template.md#reordering_layers).

### Anpassen eines Schatten- oder Glüheffekts {#adjusting-a-shadow-or-glow-effect}

Um einen Schatten- oder Schein-Effekt anzupassen, markieren Sie dessen Namen in der Liste „Ebenen“. Ändern Sie dann im Bereich „Ebeneneigenschaften“ des Anzeigebereichs „Vorlage“ die Einstellungen für den Effekt.

* **[!UICONTROL Farbe]**: Klicken Sie auf die Schaltfläche „Farbe“ und wählen Sie ein Farbfeld aus, um die Farbe des Schattens oder Glühens zu ändern. Sie können auch einen Farbwertparameter in diesem Feld eingeben.

* **[!UICONTROL Deckkraft]**: Ziehen Sie den Regler, um die Intensität des Effekts zu bestimmen. Je geringer die Deckkraftwerte, desto transparenter die Effekte.

* **[!UICONTROL Mischmodus]**: Wählen Sie eine Option aus, um einen der in Photoshop verfügbaren Mischmodi zu simulieren. Sie haben die Wahl zwischen „Normal“, „Auflösen“, „Aufhellen“, „Abdunkeln“, „Multiplizieren“ und „Negativ multiplizieren“.

* **[!UICONTROL Größe]**: Geben Sie die Werte in das Feld X und Y ein, um den Schatteneffekt zu vergrößern oder zu verkleinern. Die Größenoptionen sind nur für die Effekte „Schatten nach innen“ und „Schlagschatten“ verfügbar.

* **[!UICONTROL Vergrößern]**: Ziehen Sie den Schieberegler, um den Effekt nach innen oder außen zu erweitern.

* **[!UICONTROL Weichzeichnen]**: Ziehen Sie den Schieberegler, um die Weichzeichnung an den Rändern des Effekts zu steuern. Je größer der Weichzeichnungswert, desto weicher (undeutlicher) die Kante.

## Maskieren von Ebenen {#masking-layers}

Über die Schaltfläche „Maske“ in der Liste „Ebenen“ können Sie angeben, wie die Maske oder der Alpha-Kanal einer Ebene verwendet werden soll. Mithilfe der Schaltfläche „Maske“ können Sie den Effekt einer Hintergrundebene auf eine bestimmte Ebene oder die gesamte übergeordnete Ebene in der Vorlage anwenden. Wählen Sie in der Liste „Ebenen“ eine Ebene aus und wählen Sie **[!UICONTROL Maske]**, um die folgenden Status zu durchlaufen:

* Der Hintergrund der Ebene ist deckend.
* Der Inhalt der Ebene erscheint invertiert und der Hintergrund der Ebene ist schwarz gefüllt.
* Der Hintergrund der Ebenen ist Schwarz gefüllt.
