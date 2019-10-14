---
title: Parametrisieren einer Vorlage in Dynamic Media Classic
seo-title: Parametrisieren einer Vorlage in Dynamic Media Classic
description: 'null'
seo-description: Erfahren Sie, wie Sie eine Vorlage in Dynamic Media Classic parametrisieren.
uuid: 27c8c8b4-47f3-4270-a6db-d304648ba357
contentOwner: admin
content-type: Verweis
products: SG_EXPERIENCEMANAGER/Dynamic Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: df1a9ff5-a5ba-4480-ba0d-a19bc665f907
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Parametrisieren einer Vorlage in Dynamic Media Classic{#parameterizing-a-template-in-scene}

Nach dem Hochladen einer Illustrator-Vorlage, die Sie als FXG für dynamische Medien in das Scene7 Publishing System gespeichert haben, können Sie die variablen Elemente definieren. Parametrisieren Sie dazu die variablen Elemente in den Anzeigebereichen „Erstellen“ und „Vorschau“ von Vorlagen für Veröffentlichungen. Dynamic Media Classic bietet Werkzeuge zum Definieren von Text- und Objektparametern auf Ebenen und deren Eigenschaften. Außerdem können Sie verschiedene Versionen einer Vorlage erstellen.

Durch Parametrisierung einer FXG-Vorlage lassen sich die Variabilität von Text, Bildern und Grafiken in der Vorlage anpassen. So können Sie z. B. eine Textzeile so parametrisieren, dass die Endbenutzer den Text in der gesamten Webbenutzeroberfläche ändern können. Sie können auch leere Textfelder als Variablen definieren, sodass die Endbenutzer diese Felder mit personalisiertem Text füllen können. Sie können die Attribute und Eigenschaften von Designelementen auch im Anzeigebereich "Erstellen von Dynamischen Medien-Classic-Vorlagen für Veröffentlichungen"parametrisieren.

>[!NOTE]
>
>Die Parametrisierung der Vorlage in Dynamic Media Classic ist nicht erforderlich, wenn Sie die DOM-Manipulation verwenden möchten.

## Definieren von Parametern in FXG-Vorlagen {#defining-parameters-in-fxg-templates}

Führen Sie die folgenden Schritte in Dynamic Media Classic aus, um Parameter für eine FXG-Vorlage zu definieren:

1. Wählen Sie im Fenster „Durchsuchen“ die FXG-Datei aus.
1. Click **Build** and choose **Template Publishing**, or click the file’s **Edit** button.

   Der Anzeigebereich „Vorlagen für Veröffentlichungen“ wird geöffnet. 

1. Wählen Sie LRCo\FXG\Welcome_Summit_10 (FXG-Datei) und klicken Sie auf **Erstellen** &gt; **Vorlagen für Veröffentlichungen**.</p>

   ![](assets/wp_fxg_edit.png)

1. Wählen Sie im Ebenenbedienfeld im Anzeigenbereich „Vorlagen für Veröffentlichungen“ die Ebene mit den Elementen aus, die parametrisiert werden sollen.

   >[!NOTE]
   >
   >Vergewissern Sie sich durch wiederholtes Klicken auf das Augensymbol, dass Sie das gewünschte Objekt ausgewählt haben.

1. Klicken Sie im Eigenschaftenbedienfeld in der Spalte „Name“ (wenn Sie Text parametrisieren möchten) oder in der Spalte „Parameter“ (wenn Sie Objekte parametrisieren möchten) auf einen Parameter.

   * **Text** Klicken Sie auf das Textfeld (blättern Sie zum Suchen nach dem Textfeld zum unteren Rand der Liste Eigenschaften). Das Dialogfeld „Parameter“ wird angezeigt. Select the text that you want to parameterize and click **Add**. Sie können aus ein und derselben Texteigenschaft mehrere Parameter erstellen, indem Sie unterschiedliche Abschnitte des Texts auswählen und für jeden Abschnitt Parameter hinzufügen. To change the name of the parameter, click it, enter a new name, and click **Close**.

   * **Objekte** Klicken Sie auf ein Feld in der Spalte Parameter. Das Dialogfeld „Parameter bearbeiten“ wird angezeigt. Enter a name and click **OK**.
   Sie haben die Möglichkeit, mehrere Attribute auf einmal mit demselben Wert anzupassen, indem Sie für jedes der gewünschten Attribute denselben Parameternamen verwenden. For example, if your template has a rectangle and a star, you can type `newcolor` as the Parameter name for the SolidColor color attribute of each. Whenever you change the `newcolor` value, both the rectangle and the star change to the new color.

1. Legen Sie im Feld „Wert“ oder „Daten“ einen Standardwert für das Attribut fest. Stellen Sie alle Eigenschaften des ausgewählten Objekts ein, um genau das gewünschte Erscheinungsbild zu erhalten.
1. (Optional) Wiederholen Sie die Schritte 3 bis 5 für alle Objekte oder Ebenen, die parametrisiert werden sollen.
1. Klicken Sie auf **Speichern** oder **Speicher unter**.
1. Click **Preview** to open the FXG Preview window and see the parameters you created with their default values.

## Ein- bzw. Ausblenden eines Objekts oder einer Ebene in der FXG-Vorlage {#show-or-hide-an-object-or-layer-in-the-fxg-template}

Ausgeblendete Objekte und Ebenen sind in der Vorschau und in der Ausgabe nicht sichtbar, sie werden jedoch nicht aus der Datei gelöscht. Das Wiedereinblenden ist nach Bedarf möglich. Sichtbarkeit ist ein Attribut, das Sie als Variable definieren können. Durch Klicken auf das Augensymbol zum Ein- bzw. Ausblenden legen Sie den Standardwert für die Sichtbarkeit eines Objekts oder einer Ebene fest.

1. Wenn Sie ein Objekt oder eine Ebene in der Datei ausblenden möchten, klicken Sie im Objektebedienfeld auf das Augensymbol neben dem Namen dieses Objekts bzw. dieser Ebene.
1. Durch erneutes Klicken wird das Objekt bzw. die Ebene wieder eingeblendet.

## Erstellen unterschiedlicher Versionen einer Vorlage {#create-different-versions-of-a-template}

Sie können Attribute bearbeiten, um für verschiedene Verwendungen verschiedene Versionen der Vorlage zu erstellen.

Wenn Sie die Datei als neue FXG-Vorlage speichern möchten, ohne die ursprüngliche FXG-Vorlage zu überschreiben, klicken Sie im Anzeigebereich „Vorlagen für Veröffentlichungen“ auf „Speichern als“.

## Verwenden von Text mit Kontur {#using-stroked-text}

Text mit Kontur ist ein Beispiel für die Parametrisierung von Attributen. Dynamic Media Classic unterstützt die folgenden Funktionen für Text mit Kontur:

* Breite der Kontur
* Gestricheltes Konturmuster
* Verschiedene Verbindungsstile
* Verschiedene Abschlussstile
* Überdrucken der Kontur
* Separate Farbhandhabung für Konturen einschließlich Unterstützung für Volltonfarbe

In dieser Tabelle sind die Attribute für Text mit Kontur aufgeführt.

| Attribut | Beschreibung |
|--- |--- |
| s7:fill `<Boolean>`(S7FXG Only) | Gibt an, ob die Textfüllung aktiviert ist. Der Standardwert ist „true“. |
| s7:stroke `<Boolean>` (S7FXG Only) | Gibt an, ob die Textkontur aktiviert ist. Der Standardwert ist „false“. |
| s7:weight `<number>` (S7FXG Only) | Gibt die Stärke der Textkontur in Punkt an. Die Standardstärke ist 1 Punkt. |
| s7:joints `<string>` (miter, round, bevel) (S7FXG Only) | Gibt den Verbindungstyp für die Kontur an. Der Standardwert ist round. |
| s7:caps `<string>` (none, round, square) (S7FXG Only) | Gibt den Abschlusstyp für die Kontur an. Der Standardwert ist round. |
| s7:miterLimit `<number>` (S7FXG Only) | Gibt die Gehrungsgrenze an, wenn der Verbindungstyp für die Kontur eine Gehrungsverbindung ist. Die Standardgrenze ist 4. |
| s7:strokeOverprint `<Boolean>` (S7FXG Only) | Gibt an, ob Überdrucken für die Kontur aktiviert ist. Der Standardwert ist „false“. |
| s7:strokeColorName (nur S7FXG) | Wie s7:colorName, außer dass der Name der Farbe für die Kontur definiert wird. |
| s7:strokeColorValue (nur S7FXG) | Wie s7:colorValue, außer dass der Wert der Farbe für die Kontur definiert wird. |
| s7:strokeColorspace (nur S7FXG) | Wie s7:colorspace, außer dass der Farbraum für die Kontur definiert wird. |
| flm:dashPattern `<array>` (S7FXG Only) | Standardmäßig sind keine Muster für die Striche und Lücken festgelegt. Dieses Attribut definiert das Strich-Lücke-Muster der Kontur. Der erste Wert ist der Strich der Kontur. Der zweite Wert ist die Lücke zwischen den Strichen. Sie können den Array auf dieselbe Weise auf mehr Werte erweitern; dabei stehen die Werte alternierend für Strich und Lücke. |

## Arbeiten mit verformtem Text {#using-warped-text}

Mit verformtem Text können Sie das Erscheinungsbild von Text durch Effekte wie Welle, Flag, Dehnung usw. ändern.

Verformter Text wird für RichText-Objekte unterstützt. Der Text kann horizontal oder vertikal angeordnet sein und kann ein Punkttext, Flächentext und Text auf einem Pfad sein. Wenn Text verformt werden soll, muss zunächst das gesamte Textobjekt ausgewählt werden.

Verformter Text kann in Adobe Illustrator erstellt werden.

Beim Verformen von Text können Sie folgende Attribute festlegen:

* Stil
* Richtung
* Biegung
* Horizontale Verzerrung
* Vertikale Verzerrung

Jedes Attribut enthält einen Wertesatz.

| Attribut | Werte | Standard |
|--- |--- |--- |
| Styles7:warpStyle | nonearcarcLowerarcUpperarchbulgeshellLowershellUpperflagwavefishrisefishEyeinflatesqueezetwist | keine |
| Directions7:warpDirection | horizontalvertical | horizontal |
| Bends7:warpBend | -1 bis 1 | 0,5 |
| Horizontale Verzerrungen7:warpHorizontalDistortion | -1 bis 1 | 0 |
| Vertikale Verzerrungen7:warpVerticalDistortion | -1 bis 1 | 0 |

>[!NOTE]
>
>For `inflate` and `fishEye`, changing the `s7:warpDirection` flag between horizontal and vertical does not have any effect on the output.

Weitere Informationen zum Erstellen und Verwenden von verformten Text finden Sie in der Adobe Illustrator-Dokumentation.

>[!MORELIKETHIS]
>
>* [Erstellen der Ausgangsvorlage in Illustrator](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator)
>* [Hochladen von Dateien für Vorlagen für Veröffentlichungen](upload-files-template-publishing.md#upload_files_for_template-publishing)

