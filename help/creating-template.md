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
role: Geschäftspraktiker
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '3442'
ht-degree: 65%

---


# Erstellen einer Vorlage {#creating-a-template}

Um eine Vorlage zu erstellen, klicken Sie auf „Erstellen > Vorlagen aus Grundelementen“. Wählen Sie entweder „Designer“ oder „Entwickler“ aus. Auf dieser Seite können Sie Bild- und Textebenen hinzufügen. Darüber hinaus können Sie sowohl die Anordnung als auch die Größe und Position von Ebenen ändern sowie Schatten- und Schein-Effekte auf Bilder und Text anwenden.

>[!NOTE]
>
>Wenn Sie eine Vorlage bearbeiten, die in einer früheren Version von Dynamic Media Classic erstellt wurde, erhalten Sie beim Speichern die Aufforderung &quot;Möchten Sie eine Arbeitsflächenebene hinzufügen?&quot; Wählen Sie „Nein“, um zu verhindern, dass eine neue Grundebene erstellt wird. Falls Sie versehentlich „Ja“ wählen, löschen Sie die Modifikatoren “&amp;allowCanvasPrompt” und “&amp;layer=0” in der URL und drücken Sie die Eingabetaste bzw. den Zeilenschalter.

## Erstellen der Ausgangsvorlage  {#creating-the-initial-template}

Wenn Sie einen Vorlagensatz erstellen, wirkt sich die Option **Nach dem Speichern veröffentlichen** wie folgt auf das Set und die Set-Mitglieder aus:

| Option „Nach dem Speichern veröffentlichen“ vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

Sie können Vorlagen aus einer vorhandenen Vorlage erstellen. Öffnen Sie die vorhandene Vorlage, klicken Sie auf **Speichern unter** und geben Sie im Dialogfeld „Speichern unter“ einen neuen Namen ein.

**So erstellen Sie einen ersten Vorlagensatz**

1. Verwenden Sie zum Erstellen der Vorlage eine der folgenden Methoden:

   **Wählen Sie** zuerst die PSD-Datei oder die Bilder aus. Wählen Sie im Durchsuchenbedienfeld die PSD-Datei bzw. die Bilder aus, die Sie für die Vorlage verwenden möchten, und klicken Sie auf Erstellen > Vorlagen aus Grundelementen.

   **Beginn im** Anzeigebereich &quot;Vorlage&quot;Klicken Sie auf Erstellen > Vorlagen aus Grundelementen. Wählen Sie entweder „Designer“ oder „Entwickler“ aus. 

1. Geben Sie im Dialogfeld „Größe der Arbeitsfläche eingeben“ Werte für die Breite und Höhe der Vorlage ein.
1. Wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die PSD-Datei bzw. die Bilder, die Sie für die Vorlage verwenden möchten, in den Anzeigebereich „Vorlage“.
1. Wenn Sie fertig sind, stellen Sie sicher, dass rechts unten auf der Seite die Option **Nach dem Speichern veröffentlichen** ausgewählt ist (Standard).
1. Klicken Sie auf **Speichern**.
1. Wählen Sie einen Ordner zum Speichern der Vorlage aus, geben Sie einen Namen für die Vorlage ein und klicken Sie auf **Absenden**.

   Dynamic Media Classic schrumpft bei Bedarf die Bilder, um sie auf die Arbeitsfläche zu passen, die sich im Anzeigebereich &quot;Vorlage&quot;befindet, um die Vorlage zu definieren.

## Bearbeiten eines Vorlagensatzes {#editing-a-template-set}

Je nachdem, ob Sie eine veröffentlichte oder unveröffentlichte Vorlage bearbeiten, wirkt sich die Option **Nach dem Speichern veröffentlichen** wie folgt auf das Set und die Set-Mitglieder aus:

| Set bereits veröffentlicht? | Option „Nach dem Speichern veröffentlichen“ vor dem Speichern Ihrer Bearbeitungen ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |--- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren Status &quot;veröffentlicht&quot;bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status &quot;veröffentlicht&quot;oder &quot;unveröffentlicht&quot;bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sei einen Vorlagensatz**

1. Wählen Sie in der Rasteransicht den gewünschten Vorlagensatz und klicken Sie unterhalb des Bildes auf **Bearbeiten**.
1. Nehmen Sie die erforderlichen Änderungen an der Vorlage vor.
1. Wenn Sie die Bearbeitung abgeschlossen haben, stellen Sie sicher, dass  rechts unten auf der Seite die Option **Nach dem Speichern veröffentlichen** ausgewählt ist (Standard).
1. Klicken Sie auf **Speichern**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **Speichern**.

## Löschen einer Vorlage  {#deleting-a-template}

Wenn Sie einen Vorlagensatz löschen, wird der Satz in den Papierkorb verschoben. Die Mitglieder (bzw. die untergeordneten Elemente) innerhalb des Sets sind davon jedoch nicht betroffen; sie behalten ihren jeweiligen Status „veröffentlicht“ oder „unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie eine Vorlage**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht eine oder mehrere Vorlagen aus.
1. Klicken Sie in der globalen Navigationsleiste auf **Datei** > **Löschen** > **Löschen**.

## Erklärungen zum Bildschirm „Vorlage“ {#understanding-the-template-screen}

Der Anzeigebereich „Vorlage“ enthält Werkzeuge zum Bearbeiten und Parametrisieren von Ebenen:

Zum Erstellen von Vorlagen stehen Ihnen im Anzeigebereich „Vorlage“ die folgenden Werkzeuge zur Verfügung:

**Schwenken-** WerkzeugErmöglicht Ihnen das Auswählen von Ebenen, das Verschieben von Ebenen um die Arbeitsfläche, die Größenanpassung oder das Drehen der Ebenen.

**Textwerkzeug** Erstellt eine Textebene. Ziehen Sie das Werkzeug auf die Arbeitsfläche, um eine Textebene zu erstellen, und geben Sie dann den gewünschten Text in der Ebene ein. Siehe Erstellen einer Textebene.

**Schaltfläche &quot;Vorschau&quot;** Öffnet den Anzeigebereich &quot;Vorschau&quot;und zeigt die Vorlage in einem Zoom-Viewer an. Sie sehen dann, wie die Vorlage auf der Website bzw. in der Anwendung aussehen wird.

**Schaltfläche &quot;Parameterzusammenfassung&quot;** Öffnet den Anzeigebereich &quot;Parameterzusammenfassung&quot;. Darin werden die Namen aller Ebenen in der Vorlage sowie für jede Ebene die Namen der aktivierten Parameter angezeigt.

**Texteditor Version 4.3 und Texteditor Version 4.2** Sie können den neuesten und am häufigsten verwendeten Texteditor, Texteditor Version 4.3 oder den vorherigen Texteditor, Texteditor Version 4.2, verwenden. Beim Erstellen neuer Vorlagen ist Texteditor Version 4.3 standardmäßig ausgewählt. Beim Bearbeiten älterer Vorlagen ist Texteditor Version 4.2 standardmäßig ausgewählt. Texteditor Version 4.3 unterstützt derzeit keine Umbrüche. Verwenden Sie daher Texteditor Version 4.2, wenn Sie ältere Vorlagen bearbeiten, die Umbrüche verwenden, um die Funktionsfähigkeit der Vorlage beizubehalten. Wenn Ihre älteren Vorlagen keine Umbrüche verwenden, können Sie Texteditor Version 4.3 verwenden, um von den zahlreichen neuen Funktionen zu profitieren, z. B. „Ränder vergrößern“, „Ränder verkleinern“, „Text in Großbuchstaben formatieren“ und „Text einpassen“.

***Hinweis **: In Dynamic Media Classic wird möglicherweise Texteditor Version 4.2 entfernt. Daher wird empfohlen, nach Möglichkeit Texteditor Version 4.3 zu verwenden. Die Option „Wortumbruch“ wird in einer späteren Version von Texteditor enthalten sein.*

**Designer und** EntwicklerWählen Sie die Option, die Ihre Rolle am besten beschreibt.

**** ArbeitsflächeDefiniert den gesamten verfügbaren Bereich zum Definieren der Vorlage in Pixel. Die Standardgröße beträgt 300 x 300 Pixel. Ebenen werden auf der Arbeitsfläche platziert.

**Ebenenliste** Listet die Namen der Ebenen in der Vorlage auf. Um eine Ebene auszuwählen, markieren Sie deren Namen in der Liste „Ebenen“. Die Liste „Ebenen“ enthält Werkzeuge, mit denen Ebenen mit Effekten versehen, gelöscht, umsortiert und parametrisiert werden können. Siehe Arbeiten mit Ebenen.

**Bereich &quot;Ebeneneigenschaften&quot;** bietet Werkzeuge zum Ändern der Hintergrundfarbe, Deckkraft, Größe und Position einer Ebene sowie der Hintergrundfarbe, Deckkraft und Größe der Arbeitsfläche. Außerdem können Sie hier die Schatten- und Schein-Effekte anpassen. Siehe Arbeiten mit Ebenen.

## Erstellen von Bildebenen {#creating-image-layers}

1. Ziehen Sie das Bild von der Asset-Bibliothek auf die Arbeitsfläche.

   Der ID-Name des Bilds wird in der Liste „Ebenen“ angezeigt.

>[!NOTE]
>
>Bei Bedarf schrumpft Dynamic Media Classic die Bilder, damit sie beim Erstellen einer Bildebene in die Arbeitsfläche passen.

## Erstellen einer Textebene {#creating-a-text-layer}

1. Klicken Sie auf das Textwerkzeug.
1. Ziehen Sie, um ein Textfeld auf der Arbeitsfläche oder auf einem Bild zu erstellen.
1. Über den eingeblendeten Anzeigebereich „Text“ können Sie Text einfügen, indem Sie unter der Registerkarte „Vorgabe“ die folgenden Schritte ausführen:

   * Geben Sie Text in das Textfeld ein. Um den Text in das Textfeld einzupassen, wählen Sie „Text einpassen“.
   * Fügen Sie Text aus der Zwischenablage in das Textfeld ein.

1. Klicken Sie auf „Übernehmen“ und schließen Sie das Textfeld.

### Formatieren von Text  {#format-text}

Um Text in einer Textebene zu formatieren, führen Sie die folgenden Schritte aus:

1. Doppelklicken Sie in der Liste „Ebenen“ auf den Namen des Textfelds, dessen Inhalt Sie bearbeiten möchten. Der Texteditor wird geöffnet.
1. Wählen Sie im Textfeld den zu formatierenden Text aus. Sie können den gesamten Text, Teile davon oder auch nur einzelne Zeichen auswählen.
1. Geben Sie die gewünschten Formatierungsoptionen an und klicken Sie auf „Übernehmen“.

   **Wählen Sie im Menü &quot;Schrift&quot;eine** Schrift aus. Wenn eine gewünschte Schriftart nicht im Menü angezeigt wird, können Sie sie in Dynamic Media Classic hochladen. Siehe Schriftarten.

   **Schriftgröße** Wählen Sie eine Schriftgröße aus dem Menü aus, geben Sie eine bestimmte Größe in das Feld ein oder klicken Sie auf die Nach-oben- oder Nach-unten-Pfeile, um die Größe um zwei Punkte zu erhöhen oder zu verringern.

   **** ColorClick wählt eine Farbe für Text.

   **Fett, Kursiv oder** UnterstreichenWählen Sie den Text aus und klicken Sie dann auf das Symbol für die Formatierung, die Sie auf den Text anwenden möchten.

   **&quot;Großbuchstaben&quot;, &quot;Hochgestellt&quot;oder &quot;** Tiefgestellt&quot;Wählen Sie den Text aus und klicken Sie dann auf das Symbol für die Formatierung, die Sie auf den Text anwenden möchten.

   **Ausrichtung** Wählen Sie eine Ausrichtungsschaltfläche aus, um Text in der Textebene linksbündig, zentriert oder rechtsbündig auszurichten.

   **** TrackingType oder wählen Sie einen numerischen Wert aus, um den der Abstand zwischen Wörtern angepasst werden soll.

   **** KerningType oder wählen Sie einen numerischen Wert aus, um den der Abstand zwischen Zeichen angepasst werden soll.

   **Line** SpacingType oder wählen Sie einen numerischen Wert aus, um den der Abstand zwischen den Zeilen angepasst werden soll.

   **Baseline** ShiftType oder wählen Sie einen numerischen Wert aus, um den ein ausgewähltes Zeichen relativ zur Grundlinie des umgebenden Textes nach oben oder unten verschoben werden soll. Diese Option ist insbesondere hilfreich, wenn Sie Brüche von Hand eingeben oder die Position von eingebundenen Grafiken anpassen.

>[!NOTE]
>
>Klicken Sie auf „Rückgängig“, um die letzte Aktion rückgängig zu machen. Klicken Sie auf „Wiederholen“, wenn Sie es sich nach dem Klicken auf „Rückgängig“ zum Zurücknehmen einer Aktion anders überlegen.

### Formatieren von Absätzen  {#format-paragraphs}

1. Doppelklicken Sie in der Liste „Ebenen“ auf den Namen des Textfelds, dessen Inhalt Sie bearbeiten möchten. Der Texteditor wird geöffnet.
1. Wählen Sie den Absatz, den Sie formatieren möchten.
1. Geben Sie die gewünschten Formatierungsoptionen an und klicken Sie auf „Übernehmen“.

   **** AlignmentKlicken Sie, um den Ausrichtungstyp anzugeben: ausrichten, zentrieren, rechts ausrichten oder ausrichten.

   **Absatzende** AusrichtungKlicken Sie auf , um die Art der Ausrichtung für die letzte Zeile im Absatz festzulegen: letzte Zeile links ausrichten; letzte Zeile zentriert; und die letzte Zeile rechts ausgerichtet wird.

   **Zeilenabstand** oder wählen Sie einen numerischen Wert aus, um den der Abstand zwischen allen Zeilen im Absatz angepasst werden soll.

   **Einzug** AlleKlicken, um den Einzug des Textes zu erhöhen.

   **Entfernen Sie** IndentClick, um den Einzug des Textes zu verringern.

   **Einzug erste** ZeileGeben Sie den Einzug für die erste Textzeile an.

   **Abstand vor** AbsatzGeben Sie den Abstand an, der über der ersten Textzeile im Absatz angezeigt werden soll.

   **Abstand nach** AbsatzGeben Sie den Abstand an, der unter der letzten Textzeile im Absatz angezeigt werden soll.

   **Vertikale** AusrichtungWählen Sie aus, wo der Text vertikal im Textfeld angezeigt werden soll: Oben, Mitte, unten.

   **Textrichtung** Wählen Sie die Richtung aus, in der der Text angezeigt werden soll: von rechts nach links oder von links nach rechts.

### Anpassen der Eigenschaften der Textebene {#adjust-text-layer-properties}

1. Wählen Sie im Anzeigebereich „Vorlagen aus Grundelementen“ das Textfeld aus, das Sie anpassen möchten.
1. Wählen Sie im Feld „Ebeneneigenschaften“ eine der folgenden Optionen:

   **Text verkleinern (nur Texteditor Version 4.2)** Wählen Sie diese Option, um den Text an die Größe des Textfelds anzupassen.

   **Wortumbruch (nur Texteditor Version 4.2)** Wählen Sie eine Umbruchoption, um anzugeben, ob oder wie der Text umgebrochen wird:

   **Umfasst** den Text, damit er in ein Textfeld passt, das horizontal zu klein ist.

   **Kein** UmbruchDer Text wird nicht umgebrochen, wenn das Textfeld horizontal zu klein ist. Stattdessen wird ein Teil des Textes abgeschnitten.

   **NB Wrap**  (Geschützte Umbrüche) umschließt Text, damit er in ein Textfeld passt, ohne dass Wörter umbrochen werden.

   **** PositionGibt die Position des Textfelds auf der Arbeitsfläche an.

   **Mit** PaddingFügt Ränder hinzu oder beschneidet das Rechteck der Ebene. Geben Sie die Anzahl der Pixel für links, oben, unten und rechts an, die hinzugefügt bzw. entfernt werden sollen. Geben Sie positive Zahlen ein, um einen Rand hinzuzufügen, bzw. negative zum Beschneiden.

### Anzeigen und Bearbeiten des Text-Quell-Codes {#view-and-edit-text-source-code}

Die im Texteditor auf der Registerkarte „Quelle“ angegebenen Informationen dienen nur zur Referenz. Bearbeiten Sie diesen Text nur, wenn Sie mit der Bearbeitung von Quell-Code vertraut sind.

1. Doppelklicken Sie in der Liste „Ebenen“ auf den Namen des Textfelds, dessen Inhalt Sie bearbeiten möchten. Der Texteditor wird geöffnet.
1. Klicken Sie im Texteditor auf die Registerkarte „Quelle“, um den Quell-Code des Texts anzuzeigen.
1. Überprüfen oder bearbeiten Sie den Text nach Wunsch.

   Die Änderungen bleiben erhalten, auch wenn Sie zwischen der Vorschau- und der Quell-Ansicht wechseln.

1. Klicken Sie auf „Übernehmen“, um die vorgenommenen Änderungen zu rendern.

## Arbeiten mit Ebenen  {#working-with-layers}

Sie können in der Liste „Ebenen“ und im Bereich „Ebeneneigenschaften“ mit Ebenen arbeiten. Sie können die Anordnung von Ebenen sowie ihre Größe und Position ändern, Ebenen drehen und Hintergrund- und Vordergrundfarbe, Deckkraft und Übergangsmodus einer Ebene festlegen.

Sie können außerdem die Größe der Arbeitsfläche ändern sowie deren Hintergrundfarbe und Deckkraft festlegen.

### Neuanordnen von Ebenen  {#reordering-layers}

Eine Änderung der Ebenenreihenfolge kann sich auf ihr Aussehen auswirken, insbesondere wenn Transparenz oder Überdrucken involviert sind. Zeigen Sie unbedingt eine Vorschau der Ergebnisse an, bevor Sie die Änderungen festschreiben.

1. Wählen Sie eine der folgenden Vorgehensweisen, um die Ebenen in einer Vorlage neu anzuordnen:

   * Markieren Sie eine Ebene in der Liste „Ebenen“. Klicken Sie dann entsprechend oft auf die Nach-oben- bzw. Nach-unten-Schaltfläche, um die Ebene an die richtige Position in der Liste zu verschieben.
   * Ziehen Sie eine Ebene in der Liste „Ebenen“ nach oben oder unten.

### Ändern der Größe und Position von Ebenen und der Arbeitsfläche  {#changing-the-size-and-position-of-layers-and-the-canvas}

Ebenen müssen klein genug sein, damit sie auf die Arbeitsfläche passen. Sie können die Größe einer Ebene oder der Arbeitsfläche manuell oder durch Eingabe der Abmessungen ändern. Sie können die Position einer Ebene manuell oder durch Eingabe der Abstandswerte ändern. Sie können eine Ebene auch drehen.

>[!NOTE]
>
>Dynamic Media Classic empfiehlt, eine Bildvorgabe zu erstellen, deren Größe exakt der Größe der Vorlage entspricht. Durch die übereinstimmende Größe zwischen Bildvorgabe und Vorlage wird erreicht, dass die endgültige Ausgabegröße und die Scharfzeichnungsoptionen für die Vorlage korrekt festgelegt sind. Nachdem Sie diese Bildvorgabe erstellt haben, können Sie im Anzeigebereich „Vorschau für Vorlagen“ im Menü „Vorgabe anwenden“ die Bildvorgabe auswählen. Im Anzeigebereich können Sie sehen, wie das Bild aussieht, wenn es vom Server gesendet wird. Siehe [Einstellen von Bildvorgaben](setting-image-presets.md#setting_up_image_presets).

**Ändern der Größe einer Ebene**

Um die Größe einer Ebene oder der Arbeitsfläche zu ändern, markieren Sie die Ebene oder Arbeitsfläche in der Liste „Ebenen“ und führen Sie eines der folgenden Verfahren aus:

**Manuelles Ändern der** GrößeAuswählen und Ziehen einer Ecke der Ebene oder Arbeitsfläche Bei Textebenen können Sie auch eine Kante der Ebene ziehen. Halten Sie beim Ziehen die Umschalttaste gedrückt, um die Größe zu ändern, dabei jedoch das Seitenverhältnis (die Form) beizubehalten.

**Eingeben von** Abmessungen der EbenengrößeGeben Sie in den Textfeldern &quot;W&quot;(Breite) und &quot;H&quot;(Höhe) im Bereich &quot;Ebeneneigenschaften&quot;Pixelmessungen ein.

Sie können nicht nur die Größe einer Ebene ändern, sondern auch deren Umrandung erweitern. Geben Sie dazu im Bereich „Ebeneneigenschaften“ in den Feldern „Links“, „Rechts“, „Oben“ und „Unten“ Werte für die erweiterte Umrandung ein. Durch eine erweiterte Umrandung wird der aktuellen Ebene ein Rand hinzugefügt, um den Abstand der Ebene zur Begrenzung ihrer Basisebene zu vergrößern. Eine erweiterte Umrandung ist sinnvoll, wenn Sie einen Schatten-Effekt oder den Effekt „Schein nach außen“ hinzufügen und diesen Effekt deutlicher sichtbar machen möchten. Durch eine erweiterte Umrandung nimmt die Größe der Ebene zu und ihre Hintergrundfarbe wird in dem erweiterten Bereich angezeigt. Die Position der Basisebene wird im Verhältnis zur neuen Größe der Ebene angepasst. Wenn die aktuelle Ebene beispielsweise zentriert in der Basisebene angeordnet ist, führt eine Erweiterung auf der linken Seite der Ebene dazu, dass sie in der Basisebene weiter nach rechts verschoben wird.

**Ändern der Position einer Ebene**

Um die Position einer Ebene auf der Arbeitsfläche zu ändern, markieren Sie deren Namen in der Liste „Ebenen“ und führen Sie eines der folgenden Verfahren aus:

**Manuelles Ändern der** PositionBewegen Sie den Mauszeiger nahe an eine Ebenengrenze, jedoch nicht darüber. Wenn Sie den Mauszeiger mit vier Spitzen sehen, klicken Sie auf und ziehen Sie den Beginn.

**Eingeben von** Versatzwerten für die PositionGeben Sie in den Textfeldern &quot;X&quot;und &quot;Y&quot;die Versatzwerte für die X- und Y-Werte ein. Diese Werte entsprechen dem X- bzw. Y-Abstand des Ankerpunkts in Pixel.

**Drehen einer Ebene**

Im Feld „Drehen“ sind die Winkel aufgelistet, um die die Ebene gedreht werden kann. Um eine Ebene zu drehen, wählen Sie deren Namen in der Liste „Ebenen“ aus und führen Sie eine der folgenden Vorgehensweisen aus:

**Manuelles** DrehenBewegen des Cursors nahe an einer Ecke der Ebene, jedoch nicht darüber. Wenn der Cursor für das Drehen angezeigt wird, ziehen Sie die Ecke der Ebene in die gewünschte Richtung. Halten Sie beim Ziehen die Umschalttaste gedrückt, um in Schritten von 15 Grad zu drehen.

**Eingeben einer** GradmessungGeben Sie die Anzahl der Grad ein, um die die Ebene gedreht werden soll. Die Drehung erfolgt bei positiven Werten im Uhrzeigersinn und bei negativen gegen den Uhrzeigersinn.

**Ausblenden einer Ebene oder eines Ebeneneffekts**

Sie können eine Ebene oder einen Ebeneneffekt ausblenden, indem Sie auf das Augensymbol  neben dem Ebenennamen oder dem Effektnamen klicken. Ausgeblendete Ebenen werden nicht in Vorschauen oder in der Ausgabe angezeigt. Die Ebeneninformationen werden jedoch nicht aus der URL gelöscht. Stattdessen wird „hide=1“ zu der URL hinzugefügt, um darauf hinzuweisen, dass die Ebene gegenwärtig ausgeblendet ist. Beispiel:

layer=5&amp;src=is{PortalCo/title}&amp;pos=274,192&amp;effect=-1&amp;.effect=Drop Shadow&amp;blendmode

layer=5&amp;src=is{PortalCo/title}&amp;pos=274,192&amp;hide=1&amp;effect=-1&amp;.effect=Drop Shadow&amp;blendmode

### Bestimmen von Hintergrundfarbe, Deckkraft und Übergangsmodus  {#determining-the-background-color-opacity-and-blend-mode}

Um die Hintergrundfarbe, Deckkraft und den Übergangsmodus für eine Ebene oder die Arbeitsfläche auszuwählen, markieren Sie die Ebene oder Arbeitsfläche und führen Sie eine der folgenden Vorgehensweisen aus:

**Vordergrundfarbe** Klicken Sie auf die Schaltfläche &quot;Vordergrundfarbe&quot;und wählen Sie ein Farbfeld aus, um die Farbe des Schatten- oder Schein-Effekts zu ändern. Sie können auch einen Farbwertparameter in diesem Feld eingeben. Die Hintergrundfarbe wird nur für Ebenen mit Transparenz angewendet. Sie wird beispielsweise auf die teilweise transparente Ebene eines Preisschilds oder den Hintergrund eines Textfelds angewendet. Ebenen, die aus einem PSD-, TIFF- oder PNG-Bild bestehen, in dem Transparenz aktiviert wurde, können einen transparenten Hintergrund haben.

**Hintergrundfarbe** Klicken Sie auf die Schaltfläche &quot;Hintergrundfarbe&quot;und wählen Sie ein Farbfeld aus, um die Farbe der aufgefüllten Bereiche zu ändern.

**** DeckkraftZiehen Sie den Schieberegler &quot;Deckkraft&quot;, um eine Ebene durchsichtig zu machen, sodass ein Teil des darunter liegenden Bilds durchscheint. Bei einem Wert von 100 Prozent ist die Ebene vollkommen undurchsichtig. Bei einem Wert von 0 ist sie vollkommen transparent.

**Übergangsmodus** Wählen Sie eine Option, um einen der in Photoshop verfügbaren Übergangsmodi zu simulieren. Sie haben die Wahl zwischen „Normal“, „Auflösen“, „Aufhellen“, „Abdunkeln“, „Multiplizieren“ und „Negativ multiplizieren“. Diese Optionen können nur auf Ebenen, nicht jedoch auf die Arbeitsfläche angewendet werden.

## Verwenden von Schatten- und Schein-Effekten mit Ebenen  {#using-shadow-and-glow-effects-on-layers}

Sie können einen Schatten- oder Schein-Effekt auf eine Ebene anwenden. Der Schatten- oder Schein-Effekt wird auf den Umfang der Ebene angewendet und kann nach innen oder außen gerichtet sein, je nachdem, welche Schatten- oder Schein-Option Sie wählen. Wenn Ihre Vorlage aus einer PSD-Datei mit Schatten- und Schein-Effekten stammt, können Sie diese Effekte in Dynamic Media Classic anpassen.

Nachdem Sie einen Schatten- oder Schein-Effekt angewendet haben, können Sie dessen Größe, Farbe, Deckkraft und Position im Bereich „Ebeneneigenschaften“ des Anzeigebereichs „Vorlage“ anpassen.

### Anwenden eines Schatten- oder Schein-Effekts auf eine Ebene  {#applying-a-shadow-or-glow-effect-to-a-layer}

So wenden Sie einen Schatten- oder Schein-Effekt an

1. Markieren Sie eine Ebene in der Liste „Ebenen“.
1. Wählen Sie im Menü „Effekt hinzufügen“ eine der folgenden Optionen:

   **Schlagschatten** Wendet einen Schatten auf den unteren und rechten Rand der Ebene an.

   **Inner** ShadowWendet einen Schatteneffekt innerhalb aller Kanten der Ebene an.

   **Äußeres** ScheinWendet einen Schein-Effekt auf alle Kanten der Ebene an.

   **Inner** GlowWendet einen Schein-Effekt innerhalb aller Kanten der Ebene an.

Nach dem Anwenden eines Effekts wird dessen Name in der Liste „Ebene“ angezeigt. Um einen Effekt zu löschen, markieren Sie dessen Namen in der Liste „Ebenen“ und klicken Sie dann auf „Löschen“.

>[!NOTE]
>
>In manchen Fällen sind die Effekte „Schlagschatten“ oder „Schein nach außen“ nicht zu sehen, wenn die darunter liegende Ebene nicht groß genug ist, um die Effekte anzuzeigen. Wenn ein Schatten- oder Schein-Effekt nicht zu sehen ist, können Sie Werte für eine erweiterte Umrandung eingeben oder die Anordnung der Ebene ändern. Siehe [Ändern der Größe und Position von Ebenen und der Arbeitsfläche](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas) und [Neuanordnen von Ebenen](creating-template.md#reordering_layers).

### Anpassen eines Schatten- oder Schein-Effekts  {#adjusting-a-shadow-or-glow-effect}

Um einen Schatten- oder Schein-Effekt anzupassen, markieren Sie dessen Namen in der Liste „Ebenen“. Ändern Sie dann im Bereich „Ebeneneigenschaften“ des Anzeigebereichs „Vorlage“ die Einstellungen für den Effekt.

**** FarbeWählen Sie die Schaltfläche &quot;Farbe&quot;und wählen Sie ein Farbfeld aus, um die Farbe des Schatten- oder Schein-Effekts zu ändern. Sie können auch einen Farbwertparameter in diesem Feld eingeben.

**** DeckkraftZiehen Sie den Schieberegler, um die Intensität des Effekts festzulegen. Je geringer die Deckkraftwerte, desto transparenter die Effekte.

**ÜbergangsmodusWählen Sie eine** Option, um einen der in Photoshop verfügbaren Übergangsmodi zu simulieren. Sie haben die Wahl zwischen „Normal“, „Auflösen“, „Aufhellen“, „Abdunkeln“, „Multiplizieren“ und „Negativ multiplizieren“.

**** GrößeGeben Sie im Feld &quot;X&quot;und &quot;Y&quot;Messungen ein, um den Schatteneffekt zu vergrößern oder zu verkleinern. Die Größenoptionen sind nur für die Effekte „Schatten nach innen“ und „Schlagschatten“ verfügbar.

**Ziehen Sie** den Schieberegler, um den Effekt nach innen oder außen zu erweitern.

**Ziehen Sie** den Schieberegler, um die weiche Kante an den Kanten des Effekts zu steuern. Je größer der Weichzeichnungswert, desto weicher (undeutlicher) die Kante.

## Maskieren von Ebenen  {#masking-layers}

Über die Schaltfläche „Maske“ in der Liste „Ebenen“ können Sie angeben, wie die Maske oder der Alpha-Kanal einer Ebene verwendet werden soll. Mithilfe der Schaltfläche „Maske“ können Sie den Effekt einer Hintergrundebene auf eine bestimmte Ebene oder die gesamte übergeordnete Ebene in der Vorlage anwenden. Wählen Sie in der Liste „Ebenen“ eine Ebene aus und klicken Sie auf „Maske“ , um zwischen folgenden Status zu wechseln:

* Der Hintergrund der Ebene ist deckend.
* Der Inhalt der Ebene erscheint invertiert und der Hintergrund der Ebene ist schwarz gefüllt.
* Der Hintergrund der Ebenen ist Schwarz gefüllt.

