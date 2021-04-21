---
title: 'Arbeiten mit PSD-Dateien '
description: Erfahren Sie, wie Sie mit PSD-Dateien arbeiten.
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic, Asset Management
role: Business Practitioner
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
translation-type: tm+mt
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 58%

---

# Arbeiten mit PSD-Dateien {#working-with-psd-files}

PSD (Photoshop-Dokument-Dateien) werden in Dynamic Media Classic am häufigsten zum Erstellen von Vorlagen verwendet. Wenn Sie eine PSD-Datei hochladen, können Sie aus der Datei automatisch eine Dynamic Media Classic-Vorlage erstellen (wählen Sie im Anzeigebereich &quot;Hochladen&quot;die Option &quot;Vorlage erstellen&quot;).

Dynamic Media Classic erstellt mehrere Bilder aus einer PSD-Datei mit Ebenen, wenn Sie die Datei zum Erstellen einer Vorlage verwenden. Es wird für jede Ebene ein Bild erstellt.

## Optionen für das Hochladen von PSD-Dateien {#psd-upload-options}

Die Optionen zum Hochladen von PSD-Dateien befinden sich unter „Upload-Auftragsoptionen“ > „Photoshop-Optionen“. Sie können dabei eine Datei beschneiden, ein Farbprofil für sie auswählen, sie zum Erstellen einer Vorlage verwenden und einen Anker für sie auswählen.

Beim Hochladen von PSD-Dateien sind folgende Optionen verfügbar:

**Beschneiden**  (befindet sich unter &quot;Beschneidungsoptionen&quot;.) Wählen Sie die Option „Beschneiden“, um die weißen Flächen an den Rändern einer PSD-Datei automatisch abzuschneiden, oder wählen Sie die Option „Manuell“, um die Kanten der PSD-Datei zu beschneiden:

**&quot;** Beschneiden&quot;Wählen Sie im Menü &quot;Beschneiden basierend auf&quot;die Option &quot;Farbe&quot;oder &quot;Transparenz&quot;aus.

Bei Auswahl der Option „Farbe“ wählen Sie anschließend im Menü „Ecke“ die Ecke in der PSD-Datei aus, deren Farbe mit der Farbe der weißen Flächen, die Sie entfernen möchten, am besten übereinstimmt.

Ziehen Sie den Schieberegler auf einen Toleranzwert zwischen 0 und 1.

Wenn Sie beim Beschneiden basierend auf Farbe den Wert 0 einstellen, werden Pixel nur abgeschnitten, wenn sie exakt der Farbe entsprechen, die Sie in der Ecke der PSD-Datei ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu.

Wenn das Beschneiden auf der Grundlage der Transparenz erfolgen soll, geben Sie 0 an, damit Pixel nur abgeschnitten werden, wenn sie transparent sind. Werte, die näher an 1 liegen, lassen eine größere Transparenz zu.

* **Manuell** : Geben Sie die Anzahl der Pixel ein, die von einer Seite oder jeder Kante des Bilds abgeschnitten werden sollen. Wie viel vom Bild abgeschnitten wird, hängt von der ppi-Einstellung (Pixel pro Zoll) in der Bilddatei ab. Wenn das Bild beispielsweise eine Auflösung von 150 ppi hat und Sie in den Textfeldern „Oben“, „Rechts“, „Unten“ und „Links“ jeweils den Wert 75 eingeben, wird an jeder Kante des Bilds ein halber Zoll (ca. 1,75 cm) abgeschnitten.

* **Color Profil**  - (Befindet sich unter &quot;Color Profil Options&quot;.) Wählen Sie eine der folgenden Optionen:

* **In sRGB konvertieren (Standard)**  - Konvertiert in sRGB (Standard Red Green Blue). sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Websites.

* **Ursprünglichen Farbraum**  beibehalten: Behält den ursprünglichen Farbraum des Bildes bei.

* **Benutzerdefiniert von > in**  - Öffnet die Menüs, in denen Sie den Farbraum &quot;Konvertieren von&quot;und &quot;Konvertieren in&quot;wählen können. Sie können einen Photoshop-Standardfarbraum oder einen Farbraum auswählen, den Sie in Dynamic Media Classic hochgeladen haben. Siehe ICC-Profile.

* **Ebenen**  beibehalten: Rippt die Ebenen in der PSD-Datei (sofern vorhanden) in einzelne Assets. Die Asset-Ebenen bleiben mit der PSD-Datei verknüpft. Zeigen Sie sie an, indem Sie die PSD-Datei in der Detailansicht öffnen und das Ebenenbedienfeld auswählen. Siehe Anzeigen und Bearbeiten von Ebenen in einer PSD-Datei.

* **Vorlage**  erstellen: Erstellt eine Vorlage aus den Ebenen in der PSD-Datei.

* **Text**  extrahieren: Extrahiert den Text, damit Benutzer in einem Viewer nach Text suchen können.

* **Ebenen auf Hintergrundgröße**  erweitern: Erweitert die Größe der gerippten Bildebenen auf die Größe der Hintergrundebene.

* **Ebenenname** : Ebenen in der PSD-Datei werden als separate Bilder hochgeladen. Um diese Bilder in Dynamic Media Classic zu benennen, wählen Sie eine der folgenden Optionen:

* **Name**  der Ebene: Benennt die Bilder nach ihren Ebenennamen in der PSD-Datei. Wenn eine Ebene der PSD-Originaldatei beispielsweise „Preisschild“ heißt, wird auch das zugehörige Bild „Preisschild“ genannt. Wenn es sich bei den Namen der Ebenen in der PSD-Datei jedoch um standardmäßige Photoshop-Ebenennamen handelt („Hintergrund“, „Ebene 1“, Ebene 2“ usw.), werden die Bilder nicht nach den Standardebenennamen, sondern nach den Nummern der Ebenen in der PSD-Datei benannt.

* **Photoshop und Nummer**  der Ebene: Benennt die Bilder nach den Nummern der Ebenen in der PSD-Datei, wobei die ursprünglichen Ebenennamen ignoriert werden. Die Bilder werden mit dem Photoshop-Dateinamen und einer angefügten Nummer der Ebene benannt. Beispielsweise erhält die zweite Ebene der Datei „Frühjahrsannonce.psd“ den Namen „Frühjahrsannonce_2“, auch wenn sie in Photoshop einen nicht standardmäßigen Namen hatte.

* **Photoshop und Name**  der Ebene: Benennt die Bilder nach der PSD-Datei, gefolgt vom Namen oder der Nummer der Ebene. Die Nummern der Ebenen werden verwendet, wenn es sich bei den Namen der Ebenen in der PSD-Datei um standardmäßige Photoshop-Ebenennamen handelt. Beispielsweise erhält die Ebene „Preisschild“ in der PSD-Datei „Frühjahrsannonce“ den Namen „Frühjahrsannonce_Preisschild“. Eine Ebene mit dem standardmäßigen Namen „Ebene 2“ erhält den Namen „Frühjahrsannonce_2“.

* **Verankerung** : Geben Sie an, wie Bilder in Vorlagen verankert werden, die aus der aus der PSD-Datei erzeugten Komposition mit Ebenen generiert werden. Standardmäßig wird der Anker zentriert. Bei einem zentrierten Anker können Ersatzbilder unabhängig von ihrem Seitenverhältnis denselben Raum am besten ausfüllen. Bilder mit einem anderen Seitenverhältnis, die dieses Bild ersetzen, nehmen effektiv denselben Raum ein, wenn auf die Vorlage verwiesen und der Parametersatz verwendet wird. Wählen Sie eine andere Einstellung, wenn es für Ihre Anwendung erforderlich ist, dass die Ersatzbilder den zugewiesenen Raum in der Vorlage ausfüllen.

## Anzeigen und Bearbeiten von Ebenen in einer PSD-Datei  {#viewing-and-editing-layers-in-a-psd-file}

Wenn Sie beim Hochladen der PSD-Datei die Option &quot;Ebenen beibehalten&quot;aktiviert haben, wurden die einzelnen Ebenen von Dynamic Media Classic in Assets gerippt. Sie können die zu einer PSD-Datei gehörenden Asset-Ebenen anzeigen und bearbeiten, indem Sie die Datei in der Detailansicht des Durchsuchenbedienfelds öffnen.

1. Doppelklicken Sie auf die vollständige PSD-Datei im Durchsuchenbedienfeld, um diese in der Detailansicht zu öffnen.

   >[!NOTE]
   >
   >Stellen Sie sicher, dass Sie das komplette Asset öffnen und nicht nur eine der PSD-Ebenen.

1. Klicken Sie auf **[!UICONTROL Ebenen]**. Alle Ebenen werden als separate Bilder im Bedienfeld „Ebenen“ angezeigt.
1. Doppelklicken Sie auf eine Ebene, um sie zu öffnen, und führen Sie einen der folgenden Schritte aus:

   * Um eine Imagemap auf der Ebene zu erstellen, klicken Sie auf das Symbol **[!UICONTROL Imagemap]**. (Siehe [Erstellen von Imagemaps](creating-image-maps.md#creating_image_maps).)
   * Klicken Sie zum Erstellen von Zoom-Zielgruppen auf das Symbol **[!UICONTROL Zoom-Zielgruppen]**. (Siehe [Erstellen von Zoomzielen für geführtes Zoomen](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * Um die Ebene zu beschneiden, klicken Sie auf das Symbol **[!UICONTROL Beschneiden]**. (Siehe [Beschneiden von Bildern](cropping-image.md#cropping_an_image).)
   * Um die Ebene scharfzuzeichnen, klicken Sie auf **[!UICONTROL Scharfzeichnen]**. (Siehe [Scharfzeichnen von Bildern](sharpening-image.md#sharpening_an_image).)
   * Um die Ebene anzupassen, klicken Sie auf **[!UICONTROL Anpassen]**. (Siehe [Anpassen von Bildern](adjusting-image.md#adjusting_an_image).)

1. Klicken Sie auf **[!UICONTROL Speichern]** oder **[!UICONTROL Speicher unter]**.
1. Um eine andere Ebene anzuzeigen oder zu bearbeiten, klicken Sie auf einen Pfeil am unteren Rand der Ebenenvorschau.
1. Wenn Sie die Ebenen-Detailansicht beenden möchten, klicken Sie auf das Symbol für die Rasteransicht.
