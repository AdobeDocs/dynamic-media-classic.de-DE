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

PSD (Photoshop-Dokumentdateien) werden meistens in Adobe Dynamic Media Classic zum Erstellen von Vorlagen verwendet. Wenn Sie eine PSD-Datei hochladen, können Sie daraus automatisch eine Adobe Dynamic Media Classic-Vorlage erstellen (wählen Sie auf dem Upload-Bildschirm die Option Vorlage erstellen aus).

Adobe Dynamic Media Classic erstellt mehrere Bilder aus einer PSD-Datei mit Ebenen, wenn Sie die Datei zum Erstellen einer Vorlage verwenden. Für jede Ebene wird ein Bild erstellt.

## Optionen für das Hochladen von PSD-Dateien {#psd-upload-options}

Optionen zum Hochladen von PSD-Dateien befinden sich unter Photoshop-Optionen im Dialogfeld Upload-Auftragsoptionen . Sie können dabei eine Datei beschneiden, ein Farbprofil für sie auswählen, sie zum Erstellen einer Vorlage verwenden und einen Anker für sie auswählen.

Beim Hochladen von PSD-Dateien sind folgende Optionen verfügbar:

* **Beschneidungsoptionen**: unter **[!UICONTROL Beschneidungsoptionen]**. Wählen Sie **[!UICONTROL Zuschneiden]** aus, um automatisch Leerraum an den Rändern einer PSD-Datei zuzuschneiden. Wählen Sie **[!UICONTROL Manuell]** aus, um die Seiten der PSD-Datei zuzuschneiden:

   * **[!UICONTROL Zuschneiden]**: Wählen Sie das Menü **[!UICONTROL Beschneiden basierend auf]** und wählen Sie **[!UICONTROL Farbe]** oder **[!UICONTROL Transparenz]**.

  Wenn Sie die Option **[!UICONTROL Farbe]** auswählen, wählen Sie im Menü „Ecke“ die PSD-Ecke mit der Farbe aus, die am besten der Leerraumfarbe entspricht, die Sie beschneiden möchten.

  Ziehen Sie den Schieberegler, um eine Toleranz von 0 bis 1 festzulegen. Wenn Sie beim Beschneiden basierend auf Farbe den Wert 0 einstellen, werden Pixel nur abgeschnitten, wenn sie exakt der Farbe entsprechen, die Sie in der Ecke der PSD-Datei ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu. Um Pixel auf Grundlage der Transparenz zuzuschneiden, geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie transparent sind. Zahlen, die näher an 1 liegen, ermöglichen mehr Transparenz.

   * **[!UICONTROL Manuell]**: Geben Sie die Anzahl der Pixel ein, die von einer Seite oder jeder Seite des Bildes abgeschnitten werden sollen. Wie viel vom Bild abgeschnitten wird, hängt von der ppi-Einstellung (Pixel pro Zoll) in der Bilddatei ab. Angenommen, das Bild zeigt 150 ppi. Geben Sie 75 in die Textfelder Oben, Rechts, Unten und Links ein. Jede Seite des Bildes wird zugeschnitten, 0,5 Zoll.

* **Farbprofiloptionen**: unter **[!UICONTROL Farbprofiloptionen]**.

   * **[!UICONTROL Beibehaltung der Standardfarbe]**

   * **[!UICONTROL Ursprünglichen Farbraum beibehalten]**: Behält den ursprünglichen Farbraum des Bildes bei.

   * **[!UICONTROL Benutzerdefiniertes Formular]** > **[!UICONTROL An]**: Öffnet Menüs, in denen Sie „Konvertieren aus“ und „In Farbraum konvertieren“ auswählen können. Sie können einen standardmäßigen Photoshop-Farbraum oder einen Farbraum auswählen, den Sie in Adobe Dynamic Media Classic hochgeladen haben. Siehe [ICC-Profile](/help/using/icc-profiles.md).

* **Photoshop-Optionen**

   * **[!UICONTROL Ebenen beibehalten]**: Teilt die Ebenen im PSD (falls vorhanden) in einzelne Assets auf. Die Asset-Ebenen bleiben mit der PSD-Datei verknüpft. Sie können sie anzeigen, indem Sie die PSD-Datei in der Detailansicht öffnen und das Ebenenbedienfeld auswählen. Siehe Anzeigen und Bearbeiten von Ebenen in einer PSD-Datei.

   * **[!UICONTROL Vorlage erstellen]**: Erstellt eine Vorlage aus den Ebenen in der PSD-Datei.

   * **[!UICONTROL Text extrahieren]**: Extrahiert den Text, damit Benutzer in einem Viewer nach Text suchen können.

   * **[!UICONTROL Ebenen auf Hintergrundgröße ausdehnen]**: Erweitert die Größe der ausgelösten Bildebenen auf die Größe der Hintergrundebene.

   * **[!UICONTROL Ebenenbenennung]**: Ebenen in der PSD-Datei werden als separate Bilder hochgeladen. Um diese Bilder in Adobe Dynamic Media Classic zu benennen, wählen Sie aus den folgenden Optionen:

      * **[!UICONTROL Ebenenname]**: Benennt die Bilder nach ihren Ebenennamen in der PSD-Datei. Wenn eine Ebene der PSD-Originaldatei beispielsweise „Preisschild“ heißt, wird auch das zugehörige Bild „Preisschild“ genannt. Wenn es sich bei den Ebenennamen in der PSD-Datei jedoch um standardmäßige Photoshop-Ebenennamen handelt (Hintergrund, Ebene 1, Ebene 2 usw.), werden die Bilder nach den zugehörigen Ebenennummern in der PSD-Datei benannt. <!-- not their default layer names -->

      * **[!UICONTROL Photoshop und Ebenennummer]**: Benennt die Bilder nach den zugehörigen Ebenennummern in der PSD-Datei, wobei die ursprünglichen Ebenennamen ignoriert werden. Die Bilder werden mit dem Photoshop-Dateinamen und einer angefügten Nummer der Ebene benannt. Beispielsweise erhält die zweite Ebene der Datei `Spring Ad.psd` den Namen `Spring Ad_2`, selbst wenn sie in Photoshop einen nicht standardmäßigen Namen hatte.

      * **[!UICONTROL Photoshop und Ebenenname]**: Benennt die Bilder nach der PSD-Datei, gefolgt vom Ebenennamen oder der Ebenennummer. Die Nummern der Ebenen werden verwendet, wenn es sich bei den Namen der Ebenen in der PSD-Datei um standardmäßige Photoshop-Ebenennamen handelt. Beispielsweise erhält eine Ebene namens `Price Tag` in einer PSD-Datei mit dem Namen `SpringAd` den Namen `Spring Ad_Price Tag`. Eine Ebene mit dem Standardnamen „Ebene 2“ wird als &quot;`Spring Ad_2`&quot; bezeichnet.

   * **[!UICONTROL Anker]**: Geben Sie an, wie Bilder in Vorlagen verankert werden, die aus der aus der PSD-Datei erstellten Ebenenkomposition generiert werden. Standardmäßig wird der Anker zentriert. Ein zentraler Anker ermöglicht Ersatzbilder, die den gleichen Raum unabhängig vom Seitenverhältnis des Ersatzbilds am besten ausfüllen können. Bilder mit einem anderen Seitenverhältnis, die dieses Bild ersetzen, nehmen effektiv denselben Raum ein, wenn auf die Vorlage verwiesen und der Parametersatz verwendet wird. Wählen Sie eine andere Einstellung, wenn es für Ihre Anwendung erforderlich ist, dass die Ersatzbilder den zugewiesenen Raum in der Vorlage ausfüllen.

## Anzeigen und Bearbeiten von Ebenen in einer PSD-Datei {#viewing-and-editing-layers-in-a-psd-file}

Wenn Sie beim Hochladen Ihrer PSD die Option **[!UICONTROL Ebenen beibehalten]** ausgewählt haben, hat Adobe Dynamic Media Classic die einzelnen Ebenen in Assets aufgeteilt. Sie können die zu einer PSD-Datei gehörenden Asset-Ebenen anzeigen und bearbeiten, indem Sie die Datei im Durchsuchen-Bedienfeld in der Detailansicht öffnen.

>[!NOTE]
>
>Adobe Dynamic Media Classic unterstützt bis zu fünf Ebenen in einer verschachtelten Ebenengruppe.

1. Doppelklicken Sie im Durchsuchen-Panel auf die vollständige PSD-Datei. Die Datei wird in der Detailansicht geöffnet.

   >[!NOTE]
   >
   >Stellen Sie sicher, dass Sie das komplette Asset öffnen und nicht nur eine der PSD-Ebenen.

1. Wählen Sie **[!UICONTROL Ebenen]** aus. Alle Ebenen werden als separate Bilder im Bedienfeld „Ebenen“ angezeigt.
1. Doppelklicken Sie auf eine Ebene und führen Sie einen der folgenden Schritte aus:

   * Um eine Imagemap auf der Ebene zu erstellen, klicken Sie auf das Symbol **[!UICONTROL Imagemap]** . (Siehe [Erstellen von Imagemaps](creating-image-maps.md#creating_image_maps).)
   * Um Zoom-Ziele auf der Ebene zu erstellen, wählen Sie das Symbol **[!UICONTROL Zoom-Ziele]** aus. (Siehe [Erstellen von Zoom-Zielen für geführtes Zoomen](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Um die Ebene zuzuschneiden, wählen Sie das Symbol **[!UICONTROL Zuschneiden]** aus. (Siehe [Zuschneiden eines Bildes](cropping-image.md#cropping_an_image).)
   * Um die Ebene zu schärfen, wählen Sie **[!UICONTROL Scharfzeichnen]** aus. (Siehe [Scharfzeichnen eines Bildes](sharpening-image.md#sharpening_an_image).)
   * Um die Ebene anzupassen, klicken Sie auf **[!UICONTROL Anpassen]**. (Siehe [Bild anpassen](adjusting-image.md#adjusting_an_image).)

1. Wählen Sie **[!UICONTROL Speichern]** oder **[!UICONTROL Speichern unter]**.
1. Um eine andere Ebene anzuzeigen oder zu bearbeiten, wählen Sie unten in der Ebenenvorschau einen Pfeil aus.
1. Um die Ebenendetailansicht zu verlassen, klicken Sie auf **[!UICONTROL Symbol &quot;]**&quot;.
