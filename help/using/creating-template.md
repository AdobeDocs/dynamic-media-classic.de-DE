---
title: Erstellen von Vorlagen
description: Erfahren Sie, wie Sie eine Vorlage in Adobe Dynamic Media Classic erstellen.
uuid: c762224b-7c6c-4434-bada-c26570079645
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 8f7093da-d215-4337-ac95-69f0a5bf8648
feature: Dynamic Media Classic
role: User
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
topic: Content Management
level: Experienced
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '3420'
ht-degree: 41%

---

# Erstellen von Vorlagen {#creating-a-template}

Um eine Vorlage zu erstellen, navigieren Sie zu **[!UICONTROL Build]** > **[!UICONTROL Vorlagengrundlagen]**. Wählen Sie entweder „Designer“ oder „Entwickler“ aus. Auf dieser Seite können Sie Bild- und Textebenen hinzufügen. Darüber hinaus können Sie sowohl die Anordnung als auch die Größe und Position von Ebenen ändern sowie Schatten- und Schein-Effekte auf Bilder und Text anwenden.

Siehe auch [Vorlagengrundlagen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) Schulungsvideo.

>[!NOTE]
>
>Wenn Sie eine Vorlage bearbeiten, die in einer früheren Version von Adobe Dynamic Media Classic erstellt wurde, werden Sie aufgefordert, beim Speichern von &quot;Möchten Sie eine Arbeitsflächenebene hinzufügen?&quot;zu fragen. Auswählen **[!UICONTROL Nein]** um das Hinzufügen einer Basisebene zu vermeiden. Wenn Sie versehentlich **[!UICONTROL Ja]**, löschen Sie die `&allowCanvasPrompt` und `&layer=0` Modifikatoren in der URL und drücken Sie **[!UICONTROL Eingabe]** oder **[!UICONTROL Rückgabe]**.

## Erstellen der ursprünglichen Vorlage {#creating-the-initial-template}

Wenn Sie einen Vorlagensatz erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| **[!UICONTROL Nach dem Speichern veröffentlichen]** vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

Sie können Vorlagen aus einer vorhandenen Vorlage erstellen. Öffnen Sie die Vorlage und wählen Sie **[!UICONTROL Speichern unter]** und geben Sie im Dialogfeld &quot;Speichern unter&quot;einen neuen Namen ein.

**So erstellen Sie die Ausgangsvorlage:**

1. Verwenden Sie eine der folgenden Methoden, um Ihre Ausgangsvorlage zu erstellen:

   * **Wählen Sie zuerst die PSD oder die Bilder aus** - Wählen Sie im Durchsuchen-Bedienfeld die PSD-Datei(en) aus, die Sie für Ihre Vorlage verwenden möchten, und navigieren Sie zu **[!UICONTROL Build]** > **[!UICONTROL Vorlagengrundlagen]**.

   * **Vom Bildschirm &quot;Vorlage&quot;aus starten** - Gehen Sie zu **[!UICONTROL Build]** > **[!UICONTROL Vorlagengrundlagen]**. Wählen Sie entweder „Designer“ oder „Entwickler“ aus. 

1. Geben Sie im Dialogfeld &quot;Enter Canvas Size&quot;die Breite und Höhe der Vorlage ein.
1. Wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die PSD-Datei bzw. die Bilder, die Sie für die Vorlage verwenden möchten, in den Anzeigebereich „Vorlage“.
1. Wenn Sie fertig sind, stellen Sie sicher, dass rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Auswählen **[!UICONTROL Speichern]**.
1. Wählen Sie einen Ordner zum Speichern der Vorlage aus, geben Sie einen Namen für die Vorlage ein und wählen Sie **[!UICONTROL Einsenden]**.

   Adobe Dynamic Media Classic verkleinert Bilder bei Bedarf, um sie auf die Arbeitsfläche anzupassen, also den Bereich auf dem Bildschirm &quot;Vorlage&quot;zur Definition Ihrer Vorlage.

## Vorlagensatz bearbeiten {#editing-a-template-set}

Unabhängig davon, ob Sie einen veröffentlichten Satz oder einen nicht veröffentlichten Vorlagensatz bearbeiten, wird die **[!UICONTROL Nach dem Speichern veröffentlichen]** -Option wirkt sich auf die Set- und Set-Mitglieder wie folgt aus:

| Set bereits veröffentlicht? | **[!UICONTROL Nach dem Speichern veröffentlichen]** vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren Veröffentlichungsstatus bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie einen Vorlagensatz:**

1. Navigieren Sie in der Rasteransicht zu einem Vorlagensatz und wählen Sie unter dem Bild die Option **[!UICONTROL Bearbeiten]**.
1. Ändern Sie die Vorlage nach Bedarf.
1. Wenn Sie die Bearbeitung abgeschlossen haben, stellen Sie sicher, dass  rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Auswählen **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und wählen Sie dann **[!UICONTROL Speichern]**.

## Eine Vorlage löschen {#deleting-a-template}

Wenn Sie einen Vorlagensatz löschen, wird der Satz in den Papierkorb verschoben. Die Mitglieder (oder &quot;untergeordneten Elemente&quot;) in diesem Satz sind jedoch nicht betroffen. Stattdessen behalten sie ihren vorhandenen Status veröffentlicht oder unveröffentlicht bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie eine Vorlage:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht eine oder mehrere Vorlagen aus.
1. Wechseln Sie in der Leiste Globale Navigation zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.

## Bildschirm &quot;Vorlage&quot; {#understanding-the-template-screen}

Der Anzeigebereich „Vorlage“ enthält Werkzeuge zum Bearbeiten und Parametrisieren von Ebenen:

Verwenden Sie diese Tools auf dem Bildschirm &quot;Vorlage&quot;, um Vorlagen zu erstellen:

* **[!UICONTROL Schwenken]** - Hiermit können Sie Ebenen auswählen, sie um die Arbeitsfläche verschieben, ihre Größe ändern oder sie drehen.

* **[!UICONTROL Text]** - Erstellt eine Textebene. Ziehen Sie das Werkzeug auf die Arbeitsfläche, um eine Textebene zu erstellen, und geben Sie dann den gewünschten Text in der Ebene ein. Siehe [Erstellen einer Textebene](#creating-a-text-layer).

* **[!UICONTROL Vorschau]** - Öffnet den Vorschaubildschirm und zeigt die Vorlage in einem Zoom-Viewer an. Sie sehen dann, wie die Vorlage auf der Website bzw. in der Anwendung aussehen wird.

* **[!UICONTROL Parameterzusammenfassung]** Öffnet den Bildschirm &quot;Parameterzusammenfassung&quot;. Darin werden die Namen aller Ebenen in der Vorlage sowie für jede Ebene die Namen der aktivierten Parameter angezeigt.

* **[!UICONTROL Texteditor v4.3 und Texteditor v4.2]** - Sie können den neuesten Texteditor mit den meisten Funktionen, den Texteditor v4.3 oder den vorherigen Texteditor, Text Editor v4.2, verwenden. Beim Erstellen von Vorlagen ist standardmäßig der Texteditor v4.3 ausgewählt. Beim Bearbeiten älterer Vorlagen ist Texteditor Version 4.2 standardmäßig ausgewählt. Texteditor Version 4.3 unterstützt derzeit keine Zeilenumbrüche. Verwenden Sie daher beim Bearbeiten älterer Vorlagen, die Umbrüche verwenden, den Texteditor Version 4.2, um die Wiedergabetreue vollständig beizubehalten. Wenn Ihre ältere Vorlage keine Wortumbrüche verwendet, können Sie den Texteditor v4.3 auswählen, um die zahlreichen neuen Funktionen zu nutzen. So können Sie beispielsweise Ränder erhöhen, Ränder reduzieren, Text in allen Kapiteln einstellen und Text an Textgröße kopieren.

  >[!NOTE]
  >
  >Der Texteditor v4.2 ist für die Entfernung als Option in Adobe Dynamic Media Classic geplant. Daher wird empfohlen, nach Möglichkeit den Texteditor 4.3 zu verwenden. Die **[!UICONTROL Wortumbruch]** wird in eine künftige Version des Texteditors aufgenommen.

* **[!UICONTROL Designer und Entwickler]** - Wählen Sie die Option aus, die Ihre Rolle am besten beschreibt.

* **[!UICONTROL Arbeitsfläche]** - Definiert den gesamten verfügbaren Bereich in Pixel zur Definition Ihrer Vorlage. Die Standardgröße beträgt 300 × 300 Pixel. Ebenen werden auf der Arbeitsfläche platziert.

* **[!UICONTROL Ebenenliste]** - Listet den Namen der Ebenen in der Vorlage auf. Um eine Ebene auszuwählen, markieren Sie deren Namen in der Liste „Ebenen“. Die Liste „Ebenen“ enthält Werkzeuge, mit denen Ebenen mit Effekten versehen, gelöscht, umsortiert und parametrisiert werden können. Siehe [Arbeiten mit Ebenen](#working-with-layers).

* **[!UICONTROL Bereich &quot;Ebeneneigenschaften&quot;]** - Bietet Tools zum Ändern der Hintergrundfarbe, Deckkraft, Größe und Position einer Ebene sowie der Hintergrundfarbe, Deckkraft und Größe der Arbeitsfläche. Außerdem können Sie hier die Schatten- und Schein-Effekte anpassen. Siehe [Arbeiten mit Ebenen](#working-with-layers).

## Erstellen von Bildebenen {#creating-image-layers}

1. Ziehen Sie das Bild von der Asset-Bibliothek auf die Arbeitsfläche.

   Der ID-Name des Bilds wird in der Liste „Ebenen“ angezeigt.

   >[!NOTE]
   >
   >Bei Bedarf verkleinert Adobe Dynamic Media Classic die Bilder, damit sie beim Erstellen einer Bildebene auf die Arbeitsfläche passen.

## Erstellen einer Textebene {#creating-a-text-layer}

1. Wählen Sie die **[!UICONTROL Text]** -Tool.
1. Ziehen Sie, um ein Textfeld auf der Arbeitsfläche oder auf einem Bild zu erstellen.
1. Über den eingeblendeten Anzeigebereich „Text“ können Sie Text einfügen, indem Sie unter der Registerkarte „Vorgabe“ die folgenden Schritte ausführen:

   * Geben Sie Text in das Textfeld ein. Um den Text in das Textfeld einzupassen, wählen Sie „Text einpassen“.
   * Fügen Sie Text aus der Zwischenablage in das Textfeld ein.

1. Auswählen **[!UICONTROL Anwenden]** und schließen Sie dann den Bildschirm Text .

### Formatieren von Text {#format-text}

Gehen Sie wie folgt vor, um Text in einer Textebene zu formatieren:

1. Doppelklicken Sie in der Liste „Ebenen“ auf den Namen des Textfelds, dessen Inhalt Sie bearbeiten möchten. Der Texteditor wird geöffnet.
1. Wählen Sie im Textfeld des Texteditors den Text aus, den Sie formatieren möchten. Sie können den gesamten Text, Teile des Textes oder einzelne Zeichen auswählen.
1. Geben Sie eine der folgenden Formatierungsoptionen an und wählen Sie dann **[!UICONTROL Anwenden]**.

   * **[!UICONTROL Schriftart]** - Wählen Sie im Menü Schriftart eine Schriftart aus. Wenn eine gewünschte Schriftart nicht im Menü angezeigt wird, können Sie sie in die Adobe Dynamic Media Classic hochladen. Siehe Schriftarten.

   * **[!UICONTROL Schriftgröße]** - Wählen Sie im Menü eine Schriftgröße aus, geben Sie eine bestimmte Größe in das Feld ein oder wählen Sie die **[!UICONTROL up]** oder **[!UICONTROL Nach]** Pfeile zum Vergrößern oder Verkleinern der Größe um zwei Punkte.

   * **[!UICONTROL Farbe]** - Wählen Sie diese Option, um eine Farbe für Text auszuwählen.

   * **[!UICONTROL Fett]**, **[!UICONTROL Kursiv]** oder **[!UICONTROL Unterstreichen]** - Wählen Sie den Text aus und wählen Sie dann das Symbol für den Formatierungstyp aus, den Sie auf den Text anwenden möchten.

   * **[!UICONTROL Alle Karten]**, **[!UICONTROL Hochgestellt]** oder **[!UICONTROL Tiefgestellt]** - Wählen Sie den Text aus und wählen Sie dann das Symbol für den Formatierungstyp aus, den Sie auf den Text anwenden möchten.

   * **[!UICONTROL Ausrichtung]** - Wählen Sie eine Ausrichtungsschaltfläche , um Text in der Textebene linksbündig, zentriert oder rechtsbündig auszurichten.

   * **[!UICONTROL Tracking]** - Geben Sie einen numerischen Wert ein oder wählen Sie ihn aus, um den Abstand zwischen den Wörtern anzupassen.

   * **[!UICONTROL Kerning]** - Geben Sie einen numerischen Wert ein oder wählen Sie einen aus, um den der Abstand zwischen Zeichen angepasst werden soll.

   * **[!UICONTROL Zeilenabstand]** - Geben Sie einen numerischen Wert ein oder wählen Sie einen aus, um den der Abstand zwischen Zeilen angepasst werden soll.

   * **[!UICONTROL Grundlinienversatz]** - Geben Sie einen numerischen Wert ein oder wählen Sie einen numerischen Wert aus, um den ein ausgewähltes Zeichen relativ zur Grundlinie des umgebenden Textes nach oben oder unten verschoben werden soll. Diese Option ist besonders nützlich, wenn Sie Bruchteile manuell festlegen oder die Position von Inline-Grafiken anpassen.

>[!NOTE]
>
>Auswählen **[!UICONTROL Rückgängig]** , wenn Sie Ihre letzte Aktion rückgängig machen möchten. Auswählen **[!UICONTROL Wiederholen]** wenn Sie sich bei der Zurücksetzung einer Aktion anders entscheiden, nachdem Sie **[!UICONTROL Rückgängig]**.

### Formatieren von Absätzen {#format-paragraphs}

1. Doppelklicken Sie in der Liste „Ebenen“ auf den Namen des Textfelds, dessen Inhalt Sie bearbeiten möchten. Der Texteditor wird geöffnet.
1. Wählen Sie den Absatz aus, den Sie formatieren möchten.
1. Geben Sie eine der folgenden Formatierungsoptionen an und wählen Sie dann **[!UICONTROL Anwenden]**.

   * **[!UICONTROL Ausrichtung]** - Wählen Sie diese Option aus, um den Ausrichtungstyp anzugeben: links ausrichten, zentriert ausrichten, rechts ausrichten oder ausrichten.

   * **[!UICONTROL Absatzende-Ausrichtung]** - Wählen Sie diese Option aus, um die Art der Ausrichtung für die letzte Zeile im Absatz festzulegen: Letzte Zeile wird linksbündig, letzte Zeile zentriert und letzte Zeile rechts ausgerichtet.

   * **[!UICONTROL Zeilenabstand]** - Geben Sie einen numerischen Wert ein oder wählen Sie ihn aus, um den Abstand zwischen allen Zeilen im Absatz anzupassen.

   * **[!UICONTROL Alle einziehen]** - Wählen Sie diese Option aus, um den Einzug des Textes zu erhöhen.

   * **[!UICONTROL Einzug entfernen]** - Wählen Sie diese Option aus, um den Einzug des Textes zu verringern.

   * **[!UICONTROL Einzug Erste Zeile]** - Geben Sie den Betrag an, um den die erste Textzeile eingerückt werden soll.

   * **[!UICONTROL Leerzeichen vor Absatz]** - Geben Sie den Abstand an, der über der ersten Textzeile im Absatz angezeigt werden soll.

   * **[!UICONTROL Leerzeichen nach Absatz]** - Geben Sie den Abstand an, der unter der letzten Textzeile im Absatz angezeigt werden soll.

   * **[!UICONTROL Vertikale Ausrichtung]** - Wählen Sie aus, wo der Text vertikal im Textfeld angezeigt werden soll: Oben, Mitte, Unten.

   * **[!UICONTROL Textrichtung]** - Wählen Sie die Richtung aus, in der der Text angezeigt werden soll: von rechts nach links oder von links nach rechts.

### Anpassen der Eigenschaften der Textebene {#adjust-text-layer-properties}

1. Wählen Sie im Anzeigebereich „Vorlagen aus Grundelementen“ das Textfeld aus, das Sie anpassen möchten.
1. Wählen Sie im Feld „Ebeneneigenschaften“ eine der folgenden Optionen:

   * **[!UICONTROL Text verkleinern (nur Texteditor v4.2)]** - Um in das Textfeld zu passen, wählen Sie aus, um den Text zu verkleinern.

   * **[!UICONTROL Wortumbruch (nur Texteditor v4.2)]** - Um anzugeben, ob oder wie der Text umgebrochen wird, wählen Sie eine Umbruchoption aus:

   * **[!UICONTROL Umbruch]** - Wrappt den Text in ein Textfeld ein, das horizontal zu klein ist.

   * **[!UICONTROL Keine Umbruch]** - Richtet den Text nicht um, wenn das Textfeld horizontal zu klein ist, und schneidet stattdessen einen Teil des Textes ab.

   * **[!UICONTROL Breit geflossen]** - Umfasst Text, um in ein Textfeld zu passen, ohne Wörter zu umbrechen.

   * **[!UICONTROL Position]** - Gibt die Position des Textfelds auf der Arbeitsfläche an.

   * **[!UICONTROL Auffüllung]** - Fügt Ränder hinzu oder schneidet das Ebenenrechteck zu. Geben Sie die Anzahl der Pixel an, die Sie für Links, Oben, Unten und Rechts hinzufügen oder entfernen möchten. Geben Sie positive Zahlen ein, wenn Sie einen Rand oder negative Zahlen zum Zuschneiden hinzufügen möchten.

### Anzeigen und Bearbeiten des Text-Quell-Codes {#view-and-edit-text-source-code}

Die im Texteditor auf der Registerkarte „Quelle“ angegebenen Informationen dienen nur zur Referenz. Bearbeiten Sie diesen Text nur, wenn Sie mit der Bearbeitung von Quell-Code vertraut sind.

1. Doppelklicken Sie in der Liste „Ebenen“ auf den Namen des Textfelds, dessen Inhalt Sie bearbeiten möchten. Der Texteditor wird geöffnet.
1. Um im Texteditor den Quellcode für den Text anzuzeigen, wählen Sie die **[!UICONTROL Quelle]** im Texteditor.
1. Überprüfen oder bearbeiten Sie den Text nach Wunsch.

   Die Änderungen bleiben erhalten, auch wenn Sie zwischen der Vorschau- und der Quell-Ansicht wechseln.

1. Auswählen **[!UICONTROL Anwenden]** , um die Änderungen zu rendern.

## Arbeiten mit Ebenen {#working-with-layers}

Sie können in der Liste „Ebenen“ und im Bereich „Ebeneneigenschaften“ mit Ebenen arbeiten. Sie können die Anordnung von Ebenen sowie ihre Größe und Position ändern, Ebenen drehen und Hintergrund- und Vordergrundfarbe, Deckkraft und Übergangsmodus einer Ebene festlegen.

Sie können außerdem die Größe der Arbeitsfläche ändern sowie deren Hintergrundfarbe und Deckkraft festlegen.

### Ebenen neu anordnen {#reordering-layers}

Das Ändern der Ebenenreihenfolge kann sich auf das Erscheinungsbild auswirken, insbesondere wenn Transparenz oder Überdruck erforderlich sind. Zeigen Sie unbedingt eine Vorschau der Ergebnisse an, bevor Sie die Änderungen festschreiben.

1. Wählen Sie eine der folgenden Vorgehensweisen, um die Ebenen in einer Vorlage neu anzuordnen:

   * Markieren Sie eine Ebene in der Liste „Ebenen“. Wählen Sie anschließend **[!UICONTROL up]** oder **[!UICONTROL Nach]** so oft wie nötig, um ihn an der richtigen Position in der Liste zu platzieren.
   * Ziehen Sie eine Ebene in der Liste „Ebenen“ nach oben oder unten.

### Größe und Position von Ebenen und Arbeitsfläche ändern {#changing-the-size-and-position-of-layers-and-the-canvas}

Ebenen müssen klein genug sein, damit sie auf die Arbeitsfläche passen. Sie können die Größe einer Ebene oder der Arbeitsfläche manuell oder durch Eingabe der Abmessungen ändern. Sie können die Position einer Ebene manuell oder durch Eingabe der Abstandswerte ändern. Sie können eine Ebene auch drehen.

>[!NOTE]
>
>Adobe Dynamic Media Classic empfiehlt, eine Bildvorgabe zu erstellen, die der exakten Größe Ihrer Vorlage entspricht. Durch die übereinstimmende Größe zwischen Bildvorgabe und Vorlage wird erreicht, dass die endgültige Ausgabegröße und die Scharfzeichnungsoptionen für die Vorlage korrekt festgelegt sind. Nachdem Sie diese Bildvorgabe erstellt haben, können Sie sie im Menü &quot;Vorgabe anwenden&quot;auf dem Bildschirm &quot;Vorlagenvorschau&quot;auswählen. Im Anzeigebereich können Sie sehen, wie das Bild aussieht, wenn es vom Server gesendet wird. Siehe [Einrichten von Bildvorgaben](setting-image-presets.md#setting_up_image_presets).

* **Ändern der Größe einer Ebene** - Um die Größe einer Ebene oder der Arbeitsfläche zu ändern, wählen Sie die Ebene oder die Arbeitsfläche in der Liste Ebenen aus und verwenden Sie eine der folgenden Methoden:

* **Manuelles Ändern der Größe** - Wählen Sie eine Ecke der Ebene oder Arbeitsfläche aus und ziehen Sie sie. Bei Textebenen können Sie auch eine Kante der Ebene ziehen. Halten Sie beim Ziehen die Umschalttaste gedrückt, um die Größe zu ändern, dabei jedoch das Seitenverhältnis (die Form) beizubehalten.

* **Eingeben von Ebenengrößenmessungen** - Geben Sie die Pixelmessungen in die Textfelder W (Breite) und H (Höhe) im Bereich Ebeneneigenschaften ein.

Sie können nicht nur die Größe einer Ebene ändern, sondern auch deren Umrandung erweitern. Geben Sie dazu im Bereich „Ebeneneigenschaften“ in den Feldern „Links“, „Rechts“, „Oben“ und „Unten“ Werte für die erweiterte Umrandung ein. Durch eine erweiterte Umrandung wird der aktuellen Ebene ein Rand hinzugefügt, um den Abstand der Ebene zur Begrenzung ihrer Basisebene zu vergrößern. Eine erweiterte Umrandung ist sinnvoll, wenn Sie einen Schatten-Effekt oder den Effekt „Schein nach außen“ hinzufügen und diesen Effekt deutlicher sichtbar machen möchten. Durch eine erweiterte Umrandung nimmt die Größe der Ebene zu und ihre Hintergrundfarbe wird in dem erweiterten Bereich angezeigt. Die Position der Basisebene wird im Verhältnis zur neuen Größe der Ebene angepasst. Wenn die aktuelle Ebene beispielsweise zentriert in der Basisebene angeordnet ist, führt eine Erweiterung auf der linken Seite der Ebene dazu, dass sie in der Basisebene weiter nach rechts verschoben wird.

* **Ändern der Position einer Ebene** - Um die Position einer Ebene auf der Arbeitsfläche zu ändern, wählen Sie deren Namen in der Liste Ebenen aus und verwenden Sie eine der folgenden Methoden:

* **Manuelles Ändern der Position** - Bewegen Sie den Mauszeiger nahe, aber nicht über eine Ebenengrenze. Wenn Sie den vierköpfigen Pfeilzeiger sehen, wählen Sie aus und beginnen Sie mit dem Ziehen.

* **Eingeben der Positionssversatzmessungen** - Geben Sie die X- und Y-Versatzmessungen in die X- und Y-Textfelder ein. Diese Werte entsprechen dem X- bzw. Y-Abstand des Ankerpunkts in Pixel.

* **Drehen einer Ebene** - Das Feld Drehen zeigt den Winkel an, um den die Ebene gedreht wurde. Um eine Ebene zu drehen, wählen Sie deren Namen in der Liste „Ebenen“ aus und führen Sie eine der folgenden Vorgehensweisen aus:

* **Manuelles Drehen** - Bewegen Sie den Cursor nahe an eine Ecke der Ebene, jedoch nicht darüber. Wenn der Cursor für das Drehen angezeigt wird, ziehen Sie die Ecke der Ebene in die gewünschte Richtung. Halten Sie beim Ziehen die Umschalttaste gedrückt, um in Schritten von 15 Grad zu drehen.

* **Eingeben einer Gradmessung** - Geben Sie die Anzahl der Grad ein, um die die Ebene gedreht werden soll. Die Drehung erfolgt bei positiven Werten im Uhrzeigersinn und bei negativen gegen den Uhrzeigersinn.

**Ausblenden einer Ebene oder eines Ebeneneffekts:**

Sie können eine Ebene oder einen Ebeneneffekt ausblenden, indem Sie das Augensymbol neben einem Ebenennamen oder Effektnamen auswählen. Ausgeblendete Ebenen werden nicht in Vorschauen oder in der Ausgabe angezeigt. Die Ebeneninformationen werden jedoch nicht aus der URL gelöscht. stattdessen `hide=1` wird der URL hinzugefügt, um zu beachten, dass die Ebene ausgeblendet ist. Beispiel:

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### Hintergrundfarbe, Deckkraft und Mischmodus bestimmen {#determining-the-background-color-opacity-and-blend-mode}

Um die Hintergrundfarbe, Deckkraft und den Übergangsmodus für eine Ebene oder die Arbeitsfläche auszuwählen, markieren Sie die Ebene oder Arbeitsfläche und führen Sie eine der folgenden Vorgehensweisen aus:

* **Vordergrundfarbe** - Auswählen **[!UICONTROL Vordergrundfarbe]** und wählen Sie ein Farbmuster aus, um die Farbe des Schattens oder des Glühens zu ändern. Sie können auch einen Farbwertparameter in diesem Feld eingeben. Die Hintergrundfarbe wird nur für Ebenen mit Transparenz angewendet. Sie wird beispielsweise auf die teilweise transparente Ebene eines Preisschilds oder den Hintergrund eines Textfelds angewendet. Ebenen, die aus einem PSD-, TIFF- oder PNG-Bild bestehen, in dem Transparenz aktiviert wurde, können einen transparenten Hintergrund haben.

* **Hintergrundfarbe** - Auswählen **[!UICONTROL Hintergrundfarbe]** und wählen Sie ein Farbmuster aus, um die Farbe der aufgefüllten Bereiche zu ändern.

* **Deckkraft** - Ziehen Sie den Schieberegler Deckkraft , um jede Ebene durchsichtig zu machen, sodass ein Teil des zugrunde liegenden Bildes sichtbar wird. Die Einstellung von 100 % ist deckend, 0 ist transparent.

* **Füllmethode** - Wählen Sie eine Option, um einen der in Photoshop verfügbaren Mischmodi zu simulieren. Sie haben die Wahl zwischen „Normal“, „Auflösen“, „Aufhellen“, „Abdunkeln“, „Multiplizieren“ und „Negativ multiplizieren“. Diese Optionen können nur auf Ebenen, nicht jedoch auf die Arbeitsfläche angewendet werden.

## Schatten- und Schatteneffekte auf Ebenen verwenden {#using-shadow-and-glow-effects-on-layers}

Sie können einen Schatten- oder Schein-Effekt auf eine Ebene anwenden. Der Schatten- oder Schein-Effekt wird auf den Umfang der Ebene angewendet und kann nach innen oder außen gerichtet sein, je nachdem, welche Schatten- oder Schein-Option Sie wählen. Wenn Ihre Vorlage aus einer PSD-Datei mit Schatten- und Schein-Effekten stammt, können Sie diese Effekte in Adobe Dynamic Media Classic anpassen.

Nachdem Sie einen Schatten- oder Schein-Effekt angewendet haben, können Sie dessen Größe, Farbe, Deckkraft und Position im Bereich „Ebeneneigenschaften“ des Anzeigebereichs „Vorlage“ anpassen.

### Anwenden eines Schatten- oder Schein-Effekts auf eine Ebene {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Markieren Sie eine Ebene in der Liste „Ebenen“.
1. Wählen Sie im Menü „Effekt hinzufügen“ eine der folgenden Optionen:

   * **[!UICONTROL Schlagschatten]** - Wendet einen Schatten auf die untere und rechte Seite der Ebene an.

   * **[!UICONTROL Schatten nach innen]** - Wendet einen Schatteneffekt innerhalb aller Kanten der Ebene an.

   * **[!UICONTROL Äußere Leuchte]** - Wendet einen Glüheffekt auf alle Kanten der Ebene an.

   * **[!UICONTROL Glühen nach innen]** - Wendet einen Glüheffekt innerhalb aller Kanten der Ebene an.

Nach dem Anwenden eines Effekts wird dessen Name in der Liste „Ebene“ angezeigt. Um einen Effekt zu löschen, wählen Sie ihn in der Liste &quot;Ebenen&quot;aus und klicken Sie auf **[!UICONTROL Löschen]**.

>[!NOTE]
>
>Manchmal kann der Effekt eines Schlagschattens oder eines äußeren Glühens nicht angezeigt werden, wenn die zugrunde liegende Ebene nicht groß genug ist, um sie anzuzeigen. Wenn Sie den Schatten oder das Licht nicht sehen können, sollten Sie erwägen, der Ebene Werte für den Abstand hinzuzufügen oder die Ebene neu anzuordnen. Siehe [Ändern der Größe und Position von Ebenen und Arbeitsfläche](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) und [Neuanordnen von Ebenen](creating-template.md#reordering_layers).

### Anpassen eines Schatten- oder Schein-Effekts {#adjusting-a-shadow-or-glow-effect}

Um einen Schatten- oder Schein-Effekt anzupassen, markieren Sie dessen Namen in der Liste „Ebenen“. Ändern Sie dann im Bereich „Ebeneneigenschaften“ des Anzeigebereichs „Vorlage“ die Einstellungen für den Effekt.

* **[!UICONTROL Farbe]** - Wählen Sie die Schaltfläche Farbe und wählen Sie ein Farbmuster aus, um die Farbe des Schattens oder Glühens zu ändern. Sie können auch einen Farbwertparameter in diesem Feld eingeben.

* **[!UICONTROL Deckkraft]** - Ziehen Sie den Regler, um zu bestimmen, wie intensiv der Effekt ist. Je geringer die Deckkraftwerte, desto transparenter die Effekte.

* **[!UICONTROL Füllmethode]** - Wählen Sie eine Option, um einen der in Photoshop verfügbaren Mischmodi zu simulieren. Sie haben die Wahl zwischen „Normal“, „Auflösen“, „Aufhellen“, „Abdunkeln“, „Multiplizieren“ und „Negativ multiplizieren“.

* **[!UICONTROL Größe]** - Geben Sie im Feld &quot;X&quot;und &quot;Y&quot;Messungen ein, um den Schatteneffekt zu vergrößern oder zu verkleinern. Die Größenoptionen sind nur für die Effekte „Schatten nach innen“ und „Schlagschatten“ verfügbar.

* **[!UICONTROL Wachstum]** - Ziehen Sie den Schieberegler, um den Effekt nach innen oder außen zu erweitern.

* **[!UICONTROL Weichzeichnen]** - Ziehen Sie den Schieberegler, um die Federung an den Kanten des Effekts zu steuern. Je größer der Weichzeichnungswert, desto weicher (undeutlicher) die Kante.

## Ebenen maskieren {#masking-layers}

Über die Schaltfläche „Maske“ in der Liste „Ebenen“ können Sie angeben, wie die Maske oder der Alpha-Kanal einer Ebene verwendet werden soll. Mithilfe der Schaltfläche „Maske“ können Sie den Effekt einer Hintergrundebene auf eine bestimmte Ebene oder die gesamte übergeordnete Ebene in der Vorlage anwenden. Wählen Sie in der Liste &quot;Ebenen&quot;eine Ebene aus und klicken Sie auf **[!UICONTROL Maskieren]** um diese Status zu durchlaufen:

* Der Hintergrund der Ebene ist deckend.
* Der Inhalt der Ebene erscheint invertiert und der Hintergrund der Ebene ist schwarz gefüllt.
* Der Hintergrund der Ebenen ist Schwarz gefüllt.
