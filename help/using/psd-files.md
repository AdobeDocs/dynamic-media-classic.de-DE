---
title: Arbeiten mit PSD-Dateien
description: Erfahren Sie, wie Sie mit PSD-Dateien in Adobe Dynamic Media Classic arbeiten.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
topic: Integrations, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '1023'
ht-degree: 21%

---

# Arbeiten mit PSD-Dateien{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)**: Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on Web pages. -->

PSD (Photoshop Document Files) wird in Adobe Dynamic Media Classic meist zum Erstellen von Vorlagen verwendet. Wenn Sie eine PSD-Datei hochladen, können Sie aus der Datei automatisch eine Adobe Dynamic Media Classic-Vorlage erstellen (wählen Sie im Bildschirm &quot;Hochladen&quot;die Option Vorlage erstellen aus).

Adobe Dynamic Media Classic erstellt mehrere Bilder aus einer PSD-Datei mit Ebenen, wenn Sie die Datei zum Erstellen einer Vorlage verwenden. Es wird für jede Ebene ein Bild erstellt.

## Optionen für das Hochladen von PSD-Dateien {#psd-upload-options}

Die Optionen zum Hochladen von PSD-Dateien finden Sie unter &quot;Photoshop-Optionen&quot;im Dialogfeld &quot;Upload-Auftragsoptionen&quot;. Sie können dabei eine Datei beschneiden, ein Farbprofil für sie auswählen, sie zum Erstellen einer Vorlage verwenden und einen Anker für sie auswählen.

Beim Hochladen von PSD-Dateien sind folgende Optionen verfügbar:

* **Optionen für Beschneiden**: Befindet sich unter **[!UICONTROL Optionen für Beschneiden]**. Wählen Sie **[!UICONTROL Zuschneiden]** aus, damit Sie den Leerraum automatisch von den Kanten einer PSD-Datei abschneiden können. Wählen Sie **[!UICONTROL Manuell]** aus, um die Seiten der PSD-Datei zu beschneiden:

   * **[!UICONTROL Zuschneiden]**: Wählen Sie das Menü **[!UICONTROL Entfernen basierend auf]** aus und wählen Sie **[!UICONTROL Farbe]** oder **[!UICONTROL Transparenz]**.

  Wenn Sie die Option **[!UICONTROL Farbe]** auswählen, wählen Sie das Menü &quot;Ecke&quot;aus und wählen Sie die Ecke des PSD mit der Farbe aus, die der zu beschneidenden Leerraumfarbe am besten entspricht.

  Ziehen Sie den Regler, um eine Toleranz von 0 bis 1 anzugeben. Wenn Sie beim Beschneiden basierend auf Farbe den Wert 0 einstellen, werden Pixel nur abgeschnitten, wenn sie exakt der Farbe entsprechen, die Sie in der Ecke der PSD-Datei ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu. Wenn Sie das Zuschneiden auf der Grundlage der Transparenz durchführen möchten, geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie transparent sind. Werte, die näher bei 1 liegen, ermöglichen mehr Transparenz.

   * **[!UICONTROL Manuell]**: Geben Sie die Anzahl der Pixel ein, die von einer beliebigen Seite oder jeder Seite des Bildes abgeschnitten werden sollen. Wie viel vom Bild abgeschnitten wird, hängt von der ppi-Einstellung (Pixel pro Zoll) in der Bilddatei ab. Angenommen, das Bild zeigt 150 ppi. Geben Sie dann die Zahl 75 in die Textfelder oben, rechts, unten und links ein. Jede Bildseite ist zugeschnitten, 0,5 Zoll.

* **Farbprofiloptionen**: Befindet sich unter **[!UICONTROL Farbprofiloptionen]**.

   * **[!UICONTROL Beibehaltung der Standardfarbe]**

   * **[!UICONTROL Ursprünglichen Farbraum beibehalten]**: Behält den ursprünglichen Farbraum des Bildes bei.

   * **[!UICONTROL Benutzerdefiniert von]** > **[!UICONTROL bis]**: Öffnet Menüs, damit Sie einen Farbraum &quot;Konvertieren von&quot;und &quot;Konvertieren in&quot;auswählen können. Sie können einen standardmäßigen Photoshop-Farbraum oder einen Farbraum auswählen, den Sie in Adobe Dynamic Media Classic hochgeladen haben. Siehe [ICC-Profile](/help/using/icc-profiles.md).

* **Photoshop-Optionen**

   * **[!UICONTROL Ebenen beibehalten]**: Rippt die Ebenen im PSD (falls vorhanden) in einzelne Assets. Die Asset-Ebenen bleiben mit der PSD-Datei verknüpft. Sie können sie anzeigen, indem Sie die PSD-Datei in der Detailansicht öffnen und das Ebenenbedienfeld auswählen. Siehe Anzeigen und Bearbeiten von Ebenen in einer PSD-Datei .

   * **[!UICONTROL Vorlage erstellen]**: Erstellt eine Vorlage aus den Ebenen in der PSD-Datei.

   * **[!UICONTROL Text extrahieren]**: Extrahiert den Text, damit Benutzer in einem Viewer nach Text suchen können.

   * **[!UICONTROL Ebenen auf Hintergrundgröße erweitern]**: Erweitert die Größe der gerippten Bildebenen auf die Größe der Hintergrundebene.

   * **[!UICONTROL Ebenenbenennung]**: Ebenen in der PSD-Datei werden als separate Bilder hochgeladen. Um diese Bilder in Adobe Dynamic Media Classic zu benennen, wählen Sie eine der folgenden Optionen:

      * **[!UICONTROL Ebenenname]**: Benennt die Bilder nach ihren Ebenennamen in der PSD-Datei. Wenn eine Ebene der PSD-Originaldatei beispielsweise „Preisschild“ heißt, wird auch das zugehörige Bild „Preisschild“ genannt. Wenn es sich bei den Ebenennamen in der PSD-Datei jedoch um standardmäßige Photoshop-Ebenennamen handelt (Hintergrund, Ebene 1, Ebene 2 usw.), werden die Bilder nach ihren Ebenennummern in der PSD-Datei benannt. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop und Ebenennummer]**: Benennt die Bilder nach ihren Ebenennummern in der PSD-Datei, wobei die ursprünglichen Ebenennamen ignoriert werden. Die Bilder werden mit dem Photoshop-Dateinamen und einer angefügten Nummer der Ebene benannt. Beispielsweise erhält die zweite Ebene einer Datei mit dem Namen `Spring Ad.psd` den Namen `Spring Ad_2`, selbst wenn sie in Photoshop über einen nicht standardmäßigen Namen verfügt.

      * **[!UICONTROL Photoshop und Ebenenname]**: Benennt die Bilder nach der PSD-Datei, gefolgt vom Ebenennamen oder der Ebenennummer. Die Nummern der Ebenen werden verwendet, wenn es sich bei den Namen der Ebenen in der PSD-Datei um standardmäßige Photoshop-Ebenennamen handelt. Beispielsweise erhält eine Ebene mit dem Namen `Price Tag` in einer PSD-Datei mit dem Namen `SpringAd` den Namen `Spring Ad_Price Tag`. Eine Ebene mit dem Standardnamen Ebene 2 erhält den Namen `Spring Ad_2`.

   * **[!UICONTROL Anker]**: Geben Sie an, wie Bilder in Vorlagen verankert werden, die aus der aus der PSD-Datei erzeugten Komposition mit Ebenen generiert werden. Standardmäßig wird der Anker zentriert. Ein zentrierter Anker ermöglicht Ersatzbilder, die unabhängig vom Seitenverhältnis des Ersatzbilds denselben Raum am besten füllen können. Bilder mit einem anderen Seitenverhältnis, die dieses Bild ersetzen, nehmen effektiv denselben Raum ein, wenn auf die Vorlage verwiesen und der Parametersatz verwendet wird. Wählen Sie eine andere Einstellung, wenn es für Ihre Anwendung erforderlich ist, dass die Ersatzbilder den zugewiesenen Raum in der Vorlage ausfüllen.

## Anzeigen und Bearbeiten von Ebenen in einer PSD-Datei {#viewing-and-editing-layers-in-a-psd-file}

Wenn Sie beim Hochladen der PSD die Option **[!UICONTROL Ebenen beibehalten]** ausgewählt haben, hat Adobe Dynamic Media Classic die einzelnen Ebenen in Assets gerippt. Sie können die zu einer PSD-Datei gehörigen Asset-Ebenen anzeigen und bearbeiten, indem Sie sie im Bedienfeld &quot;Durchsuchen&quot;in der Detailansicht öffnen.

>[!NOTE]
>
>Adobe Dynamic Media Classic unterstützt bis zu fünf Ebenen in einer verschachtelten Ebenengruppe.

1. Doppelklicken Sie im Bedienfeld Durchsuchen auf die vollständige PSD-Datei. Die Datei wird in der Detailansicht geöffnet.

   >[!NOTE]
   >
   >Stellen Sie sicher, dass Sie das komplette Asset öffnen und nicht nur eine der PSD-Ebenen.

1. Wählen Sie **[!UICONTROL Ebenen]** aus. Alle Ebenen werden als separate Bilder im Bedienfeld „Ebenen“ angezeigt.
1. Doppelklicken Sie auf eine Ebene und führen Sie einen der folgenden Schritte aus:

   * Um eine Imagemap auf der Ebene zu erstellen, wählen Sie das Symbol **[!UICONTROL Imagemap]** aus. (Siehe [Erstellen von Imagemaps](creating-image-maps.md#creating_image_maps).)
   * Um Zoomziele auf der Ebene zu erstellen, wählen Sie das Symbol **[!UICONTROL Zoomziele]** aus. (Siehe [Erstellen von Zoomzielen für den Zoom mit Guided Zoom](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Um die Ebene zu beschneiden, wählen Sie das Symbol **[!UICONTROL Zuschneiden]** aus. (Siehe [Zuschneiden eines Bildes](cropping-image.md#cropping_an_image).)
   * Um die Ebene scharfzuzeichnen, wählen Sie **[!UICONTROL Scharfzeichnen]** aus. (Siehe [Scharfzeichnen eines Bildes](sharpening-image.md#sharpening_an_image).)
   * Um die Ebene anzupassen, wählen Sie **[!UICONTROL Anpassen]** aus. (Siehe [Bild anpassen](adjusting-image.md#adjusting_an_image).)

1. Wählen Sie **[!UICONTROL Speichern]** oder **[!UICONTROL Speichern unter]** aus.
1. Um eine andere Ebene anzuzeigen oder zu bearbeiten, wählen Sie einen Pfeil am unteren Rand der Ebenenvorschau aus.
1. Um die Detailansicht der Ebene zu verlassen, wählen Sie das Symbol **[!UICONTROL Rasteransicht]** aus.
