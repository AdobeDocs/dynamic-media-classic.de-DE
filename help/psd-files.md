---
title: 'Arbeiten mit PSD-Dateien '
description: Erfahren Sie, wie Sie mit PSD-Dateien arbeiten.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '989'
ht-degree: 45%

---

# Arbeiten mit PSD-Dateien {#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

PSD (Photoshop Document Files) wird meist in Dynamic Media Classic zum Erstellen von Vorlagen verwendet. Wenn Sie eine PSD-Datei hochladen, können Sie automatisch eine Dynamic Media Classic-Vorlage aus der Datei erstellen (wählen Sie im Bildschirm &quot;Hochladen&quot;die Option Vorlage erstellen aus).

Dynamic Media Classic erstellt mehrere Bilder aus einer PSD-Datei mit Ebenen, wenn Sie die Datei zum Erstellen einer Vorlage verwenden. erstellt es für jede Ebene ein Bild.

## Optionen für das Hochladen von PSD-Dateien {#psd-upload-options}

Die Optionen zum Hochladen von PSD-Dateien finden Sie unter &quot;Photoshop-Optionen&quot;im Dialogfeld &quot;Upload-Auftragsoptionen&quot;. Sie können dabei eine Datei beschneiden, ein Farbprofil für sie auswählen, sie zum Erstellen einer Vorlage verwenden und einen Anker für sie auswählen.

Beim Hochladen von PSD-Dateien sind folgende Optionen verfügbar:

* **Optionen für das Zuschneiden** : Unter &quot;Optionen für  **[!UICONTROL Zuschneiden&quot;]**. Wählen Sie &quot;Zuschneiden&quot;, um den Leerraum automatisch von den Kanten einer PSD-Datei zu beschneiden. Klicken Sie auf **[!UICONTROL Manual]** , um Seiten der PSD-Datei zuzuschneiden:

   * **Zuschneiden**  - Wählen Sie das Menü &quot; **[!UICONTROL Zuschneiden weg&quot;aus]** und wählen Sie &quot; **** Farbe  **[!UICONTROL Transparenz]**&quot;.

      Bei Auswahl der Option „Farbe“ wählen Sie anschließend im Menü „Ecke“ die Ecke in der PSD-Datei aus, deren Farbe mit der Farbe der weißen Flächen, die Sie entfernen möchten, am besten übereinstimmt.

      Ziehen Sie den Regler, um eine Toleranz von 0 bis 1 anzugeben. Wenn Sie beim Beschneiden basierend auf Farbe den Wert 0 einstellen, werden Pixel nur abgeschnitten, wenn sie exakt der Farbe entsprechen, die Sie in der Ecke der PSD-Datei ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu. Um das Beschneiden auf der Grundlage der Transparenz vorzunehmen, geben Sie 0 an, damit Pixel nur dann abgeschnitten werden, wenn sie transparent sind. Werte, die näher an 1 liegen, erlauben mehr Transparenz.

   * **Manuell**  - Geben Sie die Anzahl der Pixel ein, die von einer beliebigen Seite oder jeder Seite des Bildes abgeschnitten werden sollen. Wie viel vom Bild abgeschnitten wird, hängt von der ppi-Einstellung (Pixel pro Zoll) in der Bilddatei ab. Wenn das Bild beispielsweise eine Auflösung von 150 ppi hat und Sie in den Textfeldern „Oben“, „Rechts“, „Unten“ und „Links“ jeweils den Wert 75 eingeben, wird an jeder Kante des Bilds ein halber Zoll (ca. 1,75 cm) abgeschnitten.

* **Farbprofiloptionen**  - Befindet sich unter  **[!UICONTROL Farbprofiloptionen]**.

   * **Beibehalten der Standardfarbe**

   * **Originalfarbraum beibehalten** : Behält den ursprünglichen Farbraum des Bildes bei.

   * **Benutzerdefiniert von > in**  - Öffnet Menüs, damit Sie einen Farbraum vom Typ &quot;Konvertieren von&quot;und &quot;Konvertieren in&quot;auswählen können. Sie können einen standardmäßigen Photoshop-Farbraum oder einen Farbraum auswählen, den Sie in Dynamic Media Classic hochgeladen haben. Siehe [ICC-Profile](/help/icc-profiles.md).

* **Photoshop-Optionen**

   * **Ebenen beibehalten**  - Rippt die Ebenen in der PSD, falls vorhanden, in einzelne Assets. Die Asset-Ebenen bleiben mit der PSD-Datei verknüpft. Zeigen Sie sie an, indem Sie die PSD-Datei in der Detailansicht öffnen und das Ebenenbedienfeld auswählen. Siehe Anzeigen und Bearbeiten von Ebenen in einer PSD-Datei.

   * **Vorlage erstellen**  - Erstellt eine Vorlage aus den Ebenen in der PSD-Datei.

   * **Text extrahieren**  - Extrahiert den Text, damit Benutzer in einem Viewer nach Text suchen können.

   * **Ebenen auf Hintergrundgröße ausdehnen**  - Erweitert die Größe der gerippten Bildebenen auf die Größe der Hintergrundebene.

   * **Ebenenbenennung**  - Ebenen in der PSD-Datei werden als separate Bilder hochgeladen. Um diese Bilder in Dynamic Media Classic zu benennen, wählen Sie eine der folgenden Optionen:

      * **Ebenenname**  - Benennt die Bilder nach ihren Ebenennamen in der PSD-Datei. Wenn eine Ebene der PSD-Originaldatei beispielsweise „Preisschild“ heißt, wird auch das zugehörige Bild „Preisschild“ genannt. Wenn es sich bei den Namen der Ebenen in der PSD-Datei jedoch um standardmäßige Photoshop-Ebenennamen handelt („Hintergrund“, „Ebene 1“, Ebene 2“ usw.), werden die Bilder nicht nach den Standardebenennamen, sondern nach den Nummern der Ebenen in der PSD-Datei benannt.

      * **Photoshop und Ebenennummer** : Benennt die Bilder nach den zugehörigen Ebenennummern in der PSD-Datei, wobei die ursprünglichen Ebenennamen ignoriert werden. Die Bilder werden mit dem Photoshop-Dateinamen und einer angefügten Nummer der Ebene benannt. Die zweite Ebene einer Datei mit dem Namen `Spring Ad.psd` trägt beispielsweise den Namen `Spring Ad_2`, selbst wenn sie in Photoshop einen nicht standardmäßigen Namen hatte.

      * **Photoshop und Ebenenname**  - Benennt die Bilder nach der PSD-Datei, gefolgt vom Ebenennamen oder der Ebenennummer. Die Nummern der Ebenen werden verwendet, wenn es sich bei den Namen der Ebenen in der PSD-Datei um standardmäßige Photoshop-Ebenennamen handelt. Beispiel: Eine Ebene mit dem Namen `Price Tag` in einer PSD-Datei mit dem Namen `SpringAd` trägt den Namen `Spring Ad_Price Tag`. Eine Ebene mit dem Standardnamen Ebene 2 wird `Spring Ad_2` genannt.
   * **Anker**  - Geben Sie an, wie Bilder in Vorlagen verankert werden, die aus der aus der PSD-Datei erstellten mehrschichtigen Komposition generiert werden. Standardmäßig wird der Anker zentriert. Bei einem zentrierten Anker können Ersatzbilder unabhängig von ihrem Seitenverhältnis denselben Raum am besten ausfüllen. Bilder mit einem anderen Seitenverhältnis, die dieses Bild ersetzen, nehmen effektiv denselben Raum ein, wenn auf die Vorlage verwiesen und der Parametersatz verwendet wird. Wählen Sie eine andere Einstellung, wenn es für Ihre Anwendung erforderlich ist, dass die Ersatzbilder den zugewiesenen Raum in der Vorlage ausfüllen.


## Anzeigen und Bearbeiten von Ebenen in einer PSD-Datei {#viewing-and-editing-layers-in-a-psd-file}

Wenn Sie beim Hochladen der PSD die Option Ebenen beibehalten ausgewählt haben, hat Dynamic Media Classic die einzelnen Ebenen in Assets gerippt. Sie können die zu einer PSD-Datei gehörenden Asset-Ebenen anzeigen und bearbeiten, indem Sie die Datei in der Detailansicht des Durchsuchenbedienfelds öffnen.

1. Doppelklicken Sie im Durchsuchenbedienfeld auf die vollständige PSD-Datei. Die Datei wird in der Detailansicht geöffnet.

   >[!NOTE]
   >
   >Stellen Sie sicher, dass Sie das komplette Asset öffnen und nicht nur eine der PSD-Ebenen.

1. Klicken Sie auf **[!UICONTROL Ebenen]**. Alle Ebenen werden als separate Bilder im Bedienfeld „Ebenen“ angezeigt.
1. Doppelklicken Sie auf eine Ebene und führen Sie einen der folgenden Schritte aus:

   * Um eine Imagemap auf der Ebene zu erstellen, klicken Sie auf das Symbol **[!UICONTROL Imagemap]** . (Siehe [Erstellen von Imagemaps](creating-image-maps.md#creating_image_maps).)
   * Um Zoomziele auf der Ebene zu erstellen, klicken Sie auf das Symbol **[!UICONTROL Zoomziele]** . (Siehe [Erstellen von Zoomzielen für geführtes Zoomen](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Um die Ebene zu beschneiden, klicken Sie auf das Symbol **[!UICONTROL Zuschneiden]** . (Siehe [Beschneiden von Bildern](cropping-image.md#cropping_an_image).)
   * Um die Ebene scharfzuzeichnen, klicken Sie auf **[!UICONTROL Scharfzeichnen]**. (Siehe [Scharfzeichnen von Bildern](sharpening-image.md#sharpening_an_image).)
   * Um die Ebene anzupassen, klicken Sie auf **[!UICONTROL Anpassen]**. (Siehe [Anpassen von Bildern](adjusting-image.md#adjusting_an_image).)

1. Klicken Sie auf **[!UICONTROL Speichern]** oder **[!UICONTROL Speicher unter]**.
1. Um eine andere Ebene anzuzeigen oder zu bearbeiten, klicken Sie auf einen Pfeil am unteren Rand der Ebenenvorschau.
1. Um die Detailansicht der Ebene zu verlassen, klicken Sie auf das Symbol **[!UICONTROL Rasteransicht]**.
