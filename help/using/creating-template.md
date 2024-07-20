---
title: Erstellen von Vorlagen
description: Erfahren Sie, wie Sie eine Vorlage in Adobe Dynamic Media Classic erstellen.
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

Um eine Vorlage zu erstellen, gehen Sie zu **[!UICONTROL Build]** > **[!UICONTROL Vorlagengrundlagen]**. Wählen Sie entweder „Designer“ oder „Entwickler“ aus. Auf dieser Seite können Sie Bild- und Textebenen hinzufügen. Darüber hinaus können Sie sowohl die Anordnung als auch die Größe und Position von Ebenen ändern sowie Schatten- und Schein-Effekte auf Bilder und Text anwenden.

Siehe auch Schulungsvideo zu [Vorlagengrundlagen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) .

>[!NOTE]
>
>Wenn Sie eine Vorlage bearbeiten, die in einer früheren Version von Adobe Dynamic Media Classic erstellt wurde, werden Sie aufgefordert, beim Speichern von &quot;Möchten Sie eine Arbeitsflächenebene hinzufügen?&quot; Wählen Sie **[!UICONTROL Nein]** aus, um das Hinzufügen einer Basisebene zu vermeiden. Wenn Sie versehentlich **[!UICONTROL Ja]** auswählen, löschen Sie die Modifikatoren `&allowCanvasPrompt` und `&layer=0` in der URL und drücken Sie **[!UICONTROL Enter]** oder **[!UICONTROL Return]**.

## Erstellen der ursprünglichen Vorlage {#creating-the-initial-template}

Wenn Sie einen Vorlagensatz erstellen, wirkt sich die Option **[!UICONTROL Publish nach dem Speichern]** wie folgt auf den Satz und die Setmitglieder aus:

| **[!UICONTROL Publish nach einer Speicheroption]** ausgewählt, bevor sie gespeichert wird? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

Sie können Vorlagen aus einer vorhandenen Vorlage erstellen. Öffnen Sie die Vorlage, wählen Sie **[!UICONTROL Speichern unter]** aus und geben Sie im Dialogfeld &quot;Speichern unter&quot;einen neuen Namen ein.

**Erstellen der ursprünglichen Vorlage:**

1. Verwenden Sie eine der folgenden Methoden, um Ihre Ausgangsvorlage zu erstellen:

   * **Wählen Sie zuerst die PSD oder die Bilder aus**: Wählen Sie im Durchsuchenbedienfeld die PSD-Datei oder die-Bilder aus, die/die Sie für Ihre Vorlage verwenden möchten, gehen Sie zu **[!UICONTROL Build]** > **[!UICONTROL Vorlagengrundlagen]**.

   * **Starten Sie im Vorlagenbildschirm**: Wechseln Sie zu **[!UICONTROL Build]** > **[!UICONTROL Vorlagengrundlagen]**. Wählen Sie entweder „Designer“ oder „Entwickler“ aus. 

1. Geben Sie im Dialogfeld &quot;Enter Canvas Size&quot;die Breite und Höhe der Vorlage ein.
1. Wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die PSD-Datei bzw. die Bilder, die Sie für die Vorlage verwenden möchten, in den Anzeigebereich „Vorlage“.
1. Wenn Sie fertig sind, stellen Sie sicher, dass rechts unten auf der Seite **[!UICONTROL Publish nach einem Speichern]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]** aus.
1. Wählen Sie einen Ordner zum Speichern der Vorlage aus, geben Sie einen Namen für die Vorlage ein und wählen Sie **[!UICONTROL Senden]** aus.

   Adobe Dynamic Media Classic verkleinert Bilder bei Bedarf, um sie auf die Arbeitsfläche anzupassen, also den Bereich auf dem Bildschirm &quot;Vorlage&quot;zur Definition Ihrer Vorlage.

## Vorlagensatz bearbeiten {#editing-a-template-set}

Unabhängig davon, ob Sie einen veröffentlichten oder einen nicht veröffentlichten Vorlagensatz bearbeiten, wirkt sich die Option **[!UICONTROL Publish nach dem Speichern]** wie folgt auf den Satz und die Setmitglieder aus:

| Set bereits veröffentlicht? | **[!UICONTROL Publish nach Auswahl einer Speicheroption]** vor dem Speichern der Bearbeitung? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren Veröffentlichungsstatus bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie einen Vorlagensatz:**

1. Navigieren Sie in der Rasteransicht zu einem Vorlagensatz und wählen Sie unter dem Bild **[!UICONTROL Bearbeiten]** aus.
1. Ändern Sie die Vorlage nach Bedarf.
1. Wenn Sie die Bearbeitung abgeschlossen haben, stellen Sie sicher, dass rechts unten auf der Seite **[!UICONTROL Publish nach dem Speichern]** ausgewählt ist (Standard).
1. Wählen Sie &quot;**[!UICONTROL Speichern]**&quot;, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und wählen Sie dann &quot;**[!UICONTROL Speichern]**&quot;.

## Eine Vorlage löschen

Wenn Sie einen Vorlagensatz löschen, wird der Satz selbst in den Papierkorb verschoben. Die Mitglieder (oder &quot;untergeordneten Elemente&quot;) in diesem Satz sind jedoch nicht betroffen. Stattdessen behalten sie ihren vorhandenen Status veröffentlicht oder unveröffentlicht bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie eine Vorlage:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht eine oder mehrere Vorlagen aus.
1. Wechseln Sie in der Leiste &quot;Globale Navigation&quot;zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.

## Bildschirm &quot;Vorlage&quot; {#understanding-the-template-screen}

Der Anzeigebereich „Vorlage“ enthält Werkzeuge zum Bearbeiten und Parametrisieren von Ebenen:

Verwenden Sie diese Tools auf dem Bildschirm &quot;Vorlage&quot;, um Vorlagen zu erstellen:

* **[!UICONTROL Schwenken]**: Hiermit können Sie Ebenen auswählen, sie um die Arbeitsfläche verschieben, ihre Größe ändern oder sie drehen.

* **[!UICONTROL Text]**: Erstellt eine Textebene. Ziehen Sie das Werkzeug auf die Arbeitsfläche, um eine Textebene zu erstellen, und geben Sie dann den gewünschten Text in der Ebene ein. Siehe [Erstellen einer Textebene](#creating-a-text-layer).

* **[!UICONTROL Vorschau]**: Öffnet den Vorschaubildschirm und zeigt die Vorlage in einem Zoom-Viewer an. Sie sehen, wie die Vorlage für Benutzer auf Ihrer Website oder in Ihrer Anwendung aussieht.

* **[!UICONTROL Parameterzusammenfassung]** Öffnet den Bildschirm &quot;Parameterzusammenfassung&quot;. Darin werden die Namen aller Ebenen in der Vorlage sowie für jede Ebene die Namen der aktivierten Parameter angezeigt.

* **[!UICONTROL Texteditor v4.3 und Texteditor v4.2]**: Verwenden Sie den neuesten und am häufigsten verwendeten Texteditor. Sie können den Texteditor v4.3 oder den vorherigen Texteditor, Text Editor v4.2, verwenden. Beim Erstellen von Vorlagen ist standardmäßig der Texteditor v4.3 ausgewählt. Beim Bearbeiten älterer Vorlagen ist Texteditor Version 4.2 standardmäßig ausgewählt. Texteditor Version 4.3 unterstützt derzeit keine Zeilenumbrüche. Verwenden Sie daher beim Bearbeiten älterer Vorlagen, die Umbrüche verwenden, den Texteditor Version 4.2, um die Wiedergabetreue vollständig beizubehalten. Wenn Ihre ältere Vorlage keine Wortumbrüche verwendet, können Sie den Texteditor v4.3 auswählen, um die zahlreichen neuen Funktionen zu nutzen. So können Sie beispielsweise Ränder erhöhen, Ränder reduzieren, Text in allen Kapiteln einstellen und Text an Textgröße kopieren.

  >[!NOTE]
  >
  >Die Version 4.2 des Texteditors ist für die Entfernung als Option in Adobe Dynamic Media Classic geplant. Es wird empfohlen, nach Möglichkeit den Texteditor 4.3 zu verwenden. Die Option **[!UICONTROL Wortumbruch]** wird in eine zukünftige Version des Texteditors eingefügt.

* **[!UICONTROL Designer und Entwickler]**: Wählen Sie die Option aus, die Ihre Rolle am besten beschreibt.

* **[!UICONTROL Arbeitsfläche]**: Definiert den gesamten verfügbaren Bereich in Pixel zum Definieren Ihrer Vorlage. Die Standardgröße beträgt 300 × 300 Pixel. Ebenen werden auf der Arbeitsfläche platziert.

* **[!UICONTROL Ebenenliste]**: Listet den Namen der Ebenen in der Vorlage auf. Um eine Ebene auszuwählen, markieren Sie deren Namen in der Liste „Ebenen“. Die Liste „Ebenen“ enthält Werkzeuge, mit denen Ebenen mit Effekten versehen, gelöscht, umsortiert und parametrisiert werden können. Siehe [Arbeiten mit Ebenen](#working-with-layers).

* **[!UICONTROL Bereich &quot;Ebeneneigenschaften&quot;]**: Dieser Bereich bietet Tools zum Ändern der Hintergrundfarbe, Deckkraft, Größe und Position einer Ebene. Sie können auch die Hintergrundfarbe, Deckkraft und Größe der Arbeitsfläche ändern. Außerdem können Sie hier die Schatten- und Schein-Effekte anpassen. Siehe [Arbeiten mit Ebenen](#working-with-layers).

## Erstellen von Bildebenen {#creating-image-layers}

1. Ziehen Sie das Bild von der Asset-Bibliothek auf die Arbeitsfläche.

   Der ID-Name des Bilds wird in der Liste „Ebenen“ angezeigt.

   >[!NOTE]
   >
   >Bei Bedarf verkleinert Adobe Dynamic Media Classic die Bilder, damit sie beim Erstellen einer Bildebene auf die Arbeitsfläche passen.

## Erstellen einer Textebene {#creating-a-text-layer}

1. Wählen Sie das Tool **[!UICONTROL Text]** aus.
1. Ziehen Sie, um ein Textfeld auf der Arbeitsfläche oder auf einem Bild zu erstellen.
1. Fügen Sie im sich öffnenden Bildschirm Text Text hinzu, indem Sie auf der Registerkarte Vorschau einen der folgenden Schritte ausführen:

   * Geben Sie Text in das Textfeld ein. Um den Text in das Textfeld einzupassen, wählen Sie „Text einpassen“.
   * Fügen Sie Text aus der Zwischenablage in das Textfeld ein.

1. Wählen Sie **[!UICONTROL Anwenden]** und schließen Sie dann den Bildschirm &quot;Text&quot;.

### Formatieren von Text {#format-text}

Gehen Sie wie folgt vor, um Text in einer Textebene zu formatieren:

1. Doppelklicken Sie in der Liste „Ebenen“ auf den Namen des Textfelds, dessen Inhalt Sie bearbeiten möchten. Der Texteditor wird geöffnet.
1. Wählen Sie im Textfeld des Texteditors den Text aus, den Sie formatieren möchten. Sie können den gesamten Text, Teile des Textes oder einzelne Zeichen auswählen.
1. Geben Sie eine der folgenden Formatierungsoptionen an und wählen Sie dann **[!UICONTROL Anwenden]** aus.

   * **[!UICONTROL Schriftart]**: Wählen Sie eine Schriftart im Menü &quot;Schriftart&quot;. Wenn eine gewünschte Schriftart nicht im Menü angezeigt wird, können Sie sie in die Adobe Dynamic Media Classic hochladen. Siehe Schriftarten.

   * **[!UICONTROL Schriftgröße]**: Wählen Sie eine Schriftgröße aus dem Menü aus, geben Sie eine bestimmte Größe in das Feld ein oder wählen Sie die Pfeile **[!UICONTROL Nach oben]** oder **[!UICONTROL Nach unten]** aus, um die Schriftgröße um zwei Punkte zu erhöhen oder zu verringern.

   * **[!UICONTROL Farbe]**: Wählen Sie diese Option, um eine Farbe für Text auszuwählen.

   * **[!UICONTROL Fett]**, **[!UICONTROL Kursiv]** oder **[!UICONTROL Unterstrichen]**: Wählen Sie den Text aus und wählen Sie dann das Symbol für den Formatierungstyp aus, den Sie auf den Text anwenden möchten.

   * **[!UICONTROL Alle Überschriften]**, **[!UICONTROL Hochgestellt]** oder **[!UICONTROL Tiefgestellt]**: Wählen Sie den Text aus und wählen Sie dann das Symbol für den Formatierungstyp aus, den Sie auf den Text anwenden möchten.

   * **[!UICONTROL Ausrichtung]**: Wählen Sie eine Ausrichtungsschaltfläche, um Text in der Textebene linksbündig, zentriert oder rechtsbündig auszurichten.

   * **[!UICONTROL Tracking]**: Geben Sie einen numerischen Wert ein oder wählen Sie ihn aus, um den Abstand zwischen den Wörtern anzupassen.

   * **[!UICONTROL Kerning]**: Geben Sie einen numerischen Wert ein oder wählen Sie ihn aus, um den Abstand zwischen Zeichen anzupassen.

   * **[!UICONTROL Zeilenabstand]**: Geben Sie einen numerischen Wert ein oder wählen Sie einen numerischen Wert aus, um den der Abstand zwischen Zeilen angepasst werden soll.

   * **[!UICONTROL Grundlinienversatz]**: Geben Sie einen numerischen Wert ein oder wählen Sie einen numerischen Wert aus, um den ein ausgewähltes Zeichen relativ zur Grundlinie des umliegenden Texts nach oben oder unten verschoben werden soll. Diese Option ist besonders nützlich, wenn Sie Bruchteile manuell festlegen oder die Position von Inline-Grafiken anpassen.

>[!NOTE]
>
>Wählen Sie **[!UICONTROL Rückgängig]** aus, wenn Sie Ihre letzte Aktion rückgängig machen möchten. Wählen Sie **[!UICONTROL Wiederholen]** aus, wenn Sie Ihre Meinung zum Umkehren einer Aktion ändern möchten, nachdem Sie **[!UICONTROL Rückgängig]** ausgewählt haben.

### Formatieren von Absätzen {#format-paragraphs}

1. Doppelklicken Sie in der Liste „Ebenen“ auf den Namen des Textfelds, dessen Inhalt Sie bearbeiten möchten. Der Texteditor wird geöffnet.
1. Wählen Sie den Absatz aus, den Sie formatieren möchten.
1. Geben Sie eine der folgenden Formatierungsoptionen an und wählen Sie dann **[!UICONTROL Anwenden]** aus.

   * **[!UICONTROL Ausrichtung]**: Geben Sie den Ausrichtungstyp an, indem Sie auf &quot;**[!UICONTROL Linksbündig ausrichten]**&quot;, &quot;**[!UICONTROL Zentrieren]**&quot;, &quot;**[!UICONTROL Rechtsbündig ausrichten]**&quot;oder &quot;**[!UICONTROL justify]**&quot;klicken.

   * **[!UICONTROL Absatzende-Ausrichtung]**: Wählen Sie diese Option aus, um die Art der Ausrichtung für die letzte Zeile im Absatz anzugeben: Die letzte Zeile wird links ausgerichtet, die letzte Zeile wird zentriert und die letzte Zeile wird rechts ausgerichtet.

   * **[!UICONTROL Zeilenabstand]**: Geben Sie einen numerischen Wert ein oder wählen Sie einen aus, um den der Abstand zwischen allen Zeilen im Absatz angepasst werden soll.

   * **[!UICONTROL Alle einrücken]**: Wählen Sie diese Option aus, um den Einzug des Textes zu erhöhen.

   * **[!UICONTROL Einzug entfernen]**: Wählen Sie diese Option, um den Einzug des Textes zu verringern.

   * **[!UICONTROL Erste Zeile einrücken]**: Geben Sie den Betrag an, um den Sie die erste Textzeile einrücken möchten.

   * **[!UICONTROL Abstand vor Absatz]**: Geben Sie den Abstand an, der über der ersten Textzeile im Absatz angezeigt werden soll.

   * **[!UICONTROL Abstand nach Absatz]**: Geben Sie den Abstand an, der unter der letzten Textzeile im Absatz angezeigt werden soll.

   * **[!UICONTROL Vertikale Ausrichtung]**: Wählen Sie aus, wo der Text vertikal im Textfeld angezeigt werden soll: Oben, Mitte, Unten.

   * **[!UICONTROL Textrichtung]**: Wählen Sie die Richtung aus, in der der Text angezeigt werden soll: von rechts nach links oder von links nach rechts.

### Anpassen der Eigenschaften der Textebene {#adjust-text-layer-properties}

1. Wählen Sie im Anzeigebereich „Vorlagen aus Grundelementen“ das Textfeld aus, das Sie anpassen möchten.
1. Wählen Sie im Feld „Ebeneneigenschaften“ eine der folgenden Optionen:

   * **[!UICONTROL Text verkleinern (nur Texteditor v4.2)]**: Wählen Sie diese Option, um den Text so zu verkleinern, dass er in das Textfeld passt.

   * **[!UICONTROL Wortumbruch (nur Texteditor v4.2)]**: Um festzulegen, ob oder wie der Text umgebrochen wird, wählen Sie eine Umbruchoption aus:

   * **[!UICONTROL Umbruch]**: Wrappt den Text in ein Textfeld ein, das horizontal zu klein ist.

   * **[!UICONTROL Kein Umbruch]**: Wrappt den Text nicht um, wenn das Textfeld horizontal zu klein ist, und schneidet stattdessen einen Teil des Textes ab.

   * **[!UICONTROL Ununterbrochene Umbruch]**: Umfasst Text, um in ein Textfeld zu passen, ohne Wörter zu umbrechen.

   * **[!UICONTROL Position]**: Gibt die Position des Textfelds auf der Arbeitsfläche an.

   * **[!UICONTROL Abstand]**: Fügt Ränder hinzu oder schneidet das Ebenenrechteck ab. Geben Sie die Anzahl der Pixel an, die Sie für Links, Oben, Unten und Rechts hinzufügen oder entfernen möchten. Geben Sie positive Zahlen ein, wenn Sie eine Marge oder negative Zahlen zum Zuschnitt hinzufügen möchten.

### Anzeigen und Bearbeiten des Text-Quell-Codes {#view-and-edit-text-source-code}

Die auf der Registerkarte &quot;Source&quot;des Texteditors bereitgestellten Informationen dienen Ihrer Referenz. Bearbeiten Sie diesen Text nur, wenn Sie mit der Bearbeitung von Quell-Code vertraut sind.

1. Doppelklicken Sie in der Liste „Ebenen“ auf den Namen des Textfelds, dessen Inhalt Sie bearbeiten möchten. Der Texteditor wird geöffnet.
1. Um im Texteditor den Quellcode für den Text anzuzeigen, wählen Sie im Texteditor die Registerkarte **[!UICONTROL Source]** aus.
1. Überprüfen oder bearbeiten Sie den Text nach Wunsch.

   Die Änderungen bleiben erhalten, auch wenn Sie zwischen der Vorschau- und der Quell-Ansicht wechseln.

1. Wählen Sie **[!UICONTROL Anwenden]** aus, um die Änderungen zu rendern.

## Arbeiten mit Ebenen {#working-with-layers}

Sie können in der Liste „Ebenen“ und im Bereich „Ebeneneigenschaften“ mit Ebenen arbeiten. Sie können die Anordnung von Ebenen sowie ihre Größe und Position ändern, Ebenen drehen und Hintergrund- und Vordergrundfarbe, Deckkraft und Übergangsmodus einer Ebene festlegen.

Sie können außerdem die Größe der Arbeitsfläche ändern sowie deren Hintergrundfarbe und Deckkraft festlegen.

### Ebenen neu anordnen {#reordering-layers}

Das Ändern der Ebenenreihenfolge kann sich auf das Erscheinungsbild auswirken, insbesondere wenn Transparenz oder Überdruck erforderlich sind. Zeigen Sie unbedingt eine Vorschau der Ergebnisse an, bevor Sie die Änderungen festschreiben.

1. Wählen Sie eine der folgenden Vorgehensweisen, um die Ebenen in einer Vorlage neu anzuordnen:

   * Markieren Sie eine Ebene in der Liste „Ebenen“. Wählen Sie dann **[!UICONTROL Nach oben]** oder **[!UICONTROL Nach unten]** so oft wie nötig aus, um ihn an die richtige Position in der Liste zu setzen.
   * Ziehen Sie eine Ebene in der Liste „Ebenen“ nach oben oder unten.

### Größe und Position von Ebenen und Arbeitsfläche ändern {#changing-the-size-and-position-of-layers-and-the-canvas}

Ebenen müssen klein genug sein, damit sie auf die Arbeitsfläche passen. Sie können die Größe einer Ebene oder der Arbeitsfläche manuell oder durch Eingabe der Abmessungen ändern. Sie können die Position einer Ebene manuell oder durch Eingabe der Abstandswerte ändern. Sie können eine Ebene auch drehen.

>[!NOTE]
>
>Adobe Dynamic Media Classic empfiehlt, eine Bildvorgabe zu erstellen, die der exakten Größe Ihrer Vorlage entspricht. Durch die übereinstimmende Größe zwischen Bildvorgabe und Vorlage wird erreicht, dass die endgültige Ausgabegröße und die Scharfzeichnungsoptionen für die Vorlage korrekt festgelegt sind. Nachdem Sie diese Bildvorgabe erstellt haben, können Sie sie im Menü &quot;Vorgabe anwenden&quot;auf dem Bildschirm &quot;Vorlagenvorschau&quot;auswählen. Im Anzeigebereich können Sie sehen, wie das Bild aussieht, wenn es vom Server gesendet wird. Siehe [Einrichten von Bildvorgaben](setting-image-presets.md#setting_up_image_presets).

* **Ändern der Größe einer Ebene**: Um die Größe einer Ebene oder der Arbeitsfläche zu ändern, wählen Sie die Ebene oder Arbeitsfläche in der Liste &quot;Ebenen&quot;aus und verwenden Sie eine der folgenden Methoden:

* **Manuelles Ändern der Größe**: Wählen Sie eine Ecke der Ebene oder Arbeitsfläche aus und ziehen Sie sie. Bei Textebenen können Sie auch eine Kante der Ebene ziehen. Halten Sie beim Ziehen die Umschalttaste gedrückt, um die Größe zu ändern, aber behalten Sie das Seitenverhältnis (die Form) bei.

* **Eingeben von Ebenengrößenmessungen**: Geben Sie in die Textfelder &quot;W&quot;(Breite) und &quot;H&quot;(Höhe) im Bereich &quot;Ebeneneigenschaften&quot;Pixelmessungen ein.

Sie können nicht nur die Größe einer Ebene ändern, sondern auch deren Umrandung erweitern. Geben Sie dazu im Bereich „Ebeneneigenschaften“ in den Feldern „Links“, „Rechts“, „Oben“ und „Unten“ Werte für die erweiterte Umrandung ein. Durch eine erweiterte Umrandung wird der aktuellen Ebene ein Rand hinzugefügt, um den Abstand der Ebene zur Begrenzung ihrer Basisebene zu vergrößern. Eine erweiterte Umrandung ist sinnvoll, wenn Sie einen Schatten-Effekt oder den Effekt „Schein nach außen“ hinzufügen und diesen Effekt deutlicher sichtbar machen möchten. Durch eine erweiterte Umrandung nimmt die Größe der Ebene zu und ihre Hintergrundfarbe wird in dem erweiterten Bereich angezeigt. Die Position der Basisebene wird im Verhältnis zur neuen Größe der Ebene angepasst. Wenn die aktuelle Ebene beispielsweise zentriert in der Basisebene angeordnet ist, führt eine Erweiterung auf der linken Seite der Ebene dazu, dass sie in der Basisebene weiter nach rechts verschoben wird.

* **Ändern der Position einer Ebene**: Um die Position einer Ebene auf der Arbeitsfläche zu ändern, wählen Sie deren Namen in der Liste Ebenen aus und verwenden Sie eine der folgenden Methoden:

* **Manuelles Ändern der Position**: Bewegen Sie den Mauszeiger nahe an eine Ebenengrenze, aber nicht über eine Ebenengrenze. Wenn Sie den Cursor mit vier Pfeilen sehen, wählen Sie ihn aus und beginnen Sie mit dem Ziehen.

* **Eingeben von Positionssatzmessungen**: Geben Sie die Versatzwerte X und Y in die Textfelder X und Y ein. Diese Werte entsprechen dem X- bzw. Y-Abstand des Ankerpunkts in Pixel.

* **Drehen einer Ebene**: Das Feld &quot;Drehen&quot;listet den Winkel auf, zu dem die Ebene gedreht wurde. Um eine Ebene zu drehen, wählen Sie deren Namen in der Liste „Ebenen“ aus und führen Sie eine der folgenden Vorgehensweisen aus:

* **Manuelles Drehen**: Bewegen Sie den Cursor nahe an eine Ecke der Ebene, jedoch nicht darüber. Wenn der Cursor für das Drehen angezeigt wird, ziehen Sie die Ecke der Ebene in die gewünschte Richtung. Halten Sie beim Ziehen die Umschalttaste gedrückt, um in Schritten von 15 Grad zu drehen.

* **Eingeben einer Gradmessung**: Geben Sie die Anzahl der Grad ein, um die Ebene zu drehen. Die Drehung erfolgt bei positiven Werten im Uhrzeigersinn und bei negativen gegen den Uhrzeigersinn.

**Blendet eine Ebene oder einen Ebeneneffekt aus:**

Sie können eine Ebene oder einen Ebeneneffekt ausblenden, indem Sie das Augensymbol neben einem Ebenennamen oder Effektnamen auswählen. Ausgeblendete Ebenen werden nicht in Vorschauen oder in der Ausgabe angezeigt. Die Ebeneninformationen werden jedoch nicht aus der URL gelöscht. Stattdessen wird der URL `hide=1` hinzugefügt, um zu beachten, dass die Ebene ausgeblendet ist. Beispiel:

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### Hintergrundfarbe, Deckkraft und Mischmodus bestimmen

Um die Hintergrundfarbe, Deckkraft und den Übergangsmodus für eine Ebene oder die Arbeitsfläche auszuwählen, markieren Sie die Ebene oder Arbeitsfläche und führen Sie eine der folgenden Vorgehensweisen aus:

* **Vordergrundfarbe**: Wählen Sie **[!UICONTROL Vordergrundfarbe]** und wählen Sie ein Farbmuster aus, um die Farbe des Schatten- oder Schattens zu ändern. Sie können auch einen Farbwertparameter in diesem Feld eingeben. Die Hintergrundfarbe wird nur für Ebenen mit Transparenz angewendet. Sie wird beispielsweise auf die teilweise transparente Ebene eines Preisschilds oder den Hintergrund eines Textfelds angewendet. Ebenen, die aus einem PSD-, TIFF- oder PNG-Bild bestehen, in dem Transparenz aktiviert wurde, können einen transparenten Hintergrund haben.

* **Hintergrundfarbe**: Wählen Sie **[!UICONTROL Hintergrundfarbe]** und wählen Sie ein Farbmuster aus, um die Farbe der aufgefüllten Bereiche zu ändern.

* **Deckkraft**: Ziehen Sie den Schieberegler Deckkraft , um jede Ebene durchsichtig zu machen, sodass ein Teil des zugrunde liegenden Bildes sichtbar ist. Die Einstellung von 100 % ist deckend, 0 ist transparent.

* **Füllmethode**: Wählen Sie eine Option, um einen der in Photoshop verfügbaren Mischmodi zu simulieren. Sie haben die Wahl zwischen „Normal“, „Auflösen“, „Aufhellen“, „Abdunkeln“, „Multiplizieren“ und „Negativ multiplizieren“. Diese Optionen können nur auf Ebenen, nicht jedoch auf die Arbeitsfläche angewendet werden.

## Schatten- und Schatteneffekte auf Ebenen verwenden {#using-shadow-and-glow-effects-on-layers}

Sie können einen Schatten- oder Schein-Effekt auf eine Ebene anwenden. Der Schatten oder das Leuchten wird auf den Umfang der Ebene angewendet und erstreckt sich nach innen oder nach außen, je nach Schatten- oder Leuchten-Option. Wenn Ihre Vorlage aus einer PSD-Datei mit Schatten- und Schein-Effekten stammt, können Sie diese Effekte in Adobe Dynamic Media Classic anpassen.

Nachdem Sie einen Schatten- oder Schein-Effekt angewendet haben, können Sie dessen Größe, Farbe, Deckkraft und Position im Bereich „Ebeneneigenschaften“ des Anzeigebereichs „Vorlage“ anpassen.

### Anwenden eines Schatten- oder Schein-Effekts auf eine Ebene {#applying-a-shadow-or-glow-effect-to-a-layer}

1. Markieren Sie eine Ebene in der Liste „Ebenen“.
1. Wählen Sie das Menü **[!UICONTROL `Add Effect`]** aus und wählen Sie eine Option:

   * **[!UICONTROL Schatten ablegen]**: Wendet einen Schatten auf die untere und rechte Seite der Ebene an.

   * **[!UICONTROL Schatten nach innen]**: Wendet einen Schatteneffekt innerhalb aller Kanten der Ebene an.

   * **[!UICONTROL Äußerer Glanz]**: Wendet einen Glüheffekt auf alle Kanten der Ebene an.

   * **[!UICONTROL Inneres Glühen]**: Wendet einen Glüheffekt innerhalb aller Kanten der Ebene an.

Nach dem Anwenden eines Effekts wird dessen Name in der Liste „Ebene“ angezeigt. Um einen Effekt zu löschen, wählen Sie seinen Namen in der Liste &quot;Ebenen&quot;aus und klicken Sie dann auf **[!UICONTROL Löschen]**.

>[!NOTE]
>
>Manchmal kann der Effekt eines Schlagschattens oder eines äußeren Glühens nicht angezeigt werden, wenn die zugrunde liegende Ebene nicht groß genug ist, um sie anzuzeigen. Wenn Sie den Schatten oder das Licht nicht sehen können, sollten Sie erwägen, der Ebene Werte für den Abstand hinzuzufügen oder die Ebene neu anzuordnen. Siehe [Ändern der Größe und Position von Ebenen und Arbeitsfläche](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) und [Neuanordnen von Ebenen](creating-template.md#reordering_layers).

### Anpassen eines Schatten- oder Schein-Effekts {#adjusting-a-shadow-or-glow-effect}

Um einen Schatten- oder Schein-Effekt anzupassen, markieren Sie dessen Namen in der Liste „Ebenen“. Ändern Sie dann im Bereich „Ebeneneigenschaften“ des Anzeigebereichs „Vorlage“ die Einstellungen für den Effekt.

* **[!UICONTROL Farbe]**: Wählen Sie die Schaltfläche &quot;Farbe&quot;und wählen Sie ein Farbmuster aus, um die Farbe des Schattens oder des Glühens zu ändern. Sie können auch einen Farbwertparameter in diesem Feld eingeben.

* **[!UICONTROL Deckkraft]**: Ziehen Sie den Regler, um zu bestimmen, wie intensiv der Effekt ist. Je geringer die Deckkraftwerte, desto transparenter die Effekte.

* **[!UICONTROL Füllmethode]**: Wählen Sie eine Option, um einen der in Photoshop verfügbaren Mischmodi zu simulieren. Sie haben die Wahl zwischen „Normal“, „Auflösen“, „Aufhellen“, „Abdunkeln“, „Multiplizieren“ und „Negativ multiplizieren“.

* **[!UICONTROL Größe]**: Geben Sie in das Feld &quot;X&quot;und &quot;Y&quot;Messungen ein, um den Schatteneffekt zu vergrößern oder zu verkleinern. Die Größenoptionen sind nur für die Effekte „Schatten nach innen“ und „Schlagschatten“ verfügbar.

* **[!UICONTROL Vergrößern]**: Ziehen Sie den Regler, um den Effekt nach innen oder außen zu erweitern.

* **[!UICONTROL Weichzeichnen]**: Ziehen Sie den Regler, um die weichen Kanten des Effekts zu steuern. Je größer der Weichzeichnungswert, desto weicher (undeutlicher) die Kante.

## Ebenen maskieren {#masking-layers}

Über die Schaltfläche „Maske“ in der Liste „Ebenen“ können Sie angeben, wie die Maske oder der Alpha-Kanal einer Ebene verwendet werden soll. Mithilfe der Schaltfläche „Maske“ können Sie den Effekt einer Hintergrundebene auf eine bestimmte Ebene oder die gesamte übergeordnete Ebene in der Vorlage anwenden. Wählen Sie eine Ebene in der Liste &quot;Ebenen&quot;aus und wählen Sie **[!UICONTROL Maske]** aus, um die folgenden Status zu durchlaufen:

* Der Hintergrund der Ebene ist deckend.
* Der Inhalt der Ebene erscheint invertiert und der Hintergrund der Ebene ist schwarz gefüllt.
* Der Hintergrund der Ebenen ist Schwarz gefüllt.
