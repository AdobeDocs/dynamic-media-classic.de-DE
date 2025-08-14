---
title: 'Kurzanleitung: Bildsätze'
description: Eine Einführung in und eine Kurzanleitung zu Bildsets, die Ihnen den schnellen Einstieg in die Verwendung von Bildset-Techniken in Adobe Dynamic Media Classic erleichtern.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
topic: Content Management
level: Beginner
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 11%

---

# Kurzanleitung: Bildsätze{#quick-start-image-sets}

Adobe Dynamic Media Classic-Bildsets bieten Benutzenden ein integriertes Anzeigeerlebnis. Im Viewer für dynamische Bildsets können Benutzer unterschiedliche Ansichten eines Elements anzeigen, indem sie auf eine Miniatur klicken. Mit Bildsets können Sie alternative, hochauflösende Ansichten eines Elements darstellen.

Der Bildsatz-Viewer bietet auch Zoomfunktionen zur genauen Betrachtung der Bilder. Wenn Sie möchten, können Sie geführte Zoom-Ziele und Imagemaps zu einem Teil Ihres Bildsets machen. Durch Bildsätze wird das Betrachten der Bilder stimmiger und individueller.

Siehe [Bild- und Rotationssets: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/556_Image%20&%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) Schulungsvideo.

Beim Erstellen eines Bildsets empfiehlt Adobe die folgenden Best Practices und erzwingt die folgenden Einschränkungen:

| Art des Limits | Optimale Vorgehensweise | Limit |
| --- | --- | --- |
| Anzahl der doppelten Assets pro Set | Keine Duplikate | 20 ‡ |
| Maximale Anzahl von Bildern pro Set | 5-10 Bilder pro Set | 1000 |

‡ Best Practice ist es, keine doppelten Assets in einem Satz zu haben. Für ein einzelnes Asset sind maximal 20 Duplikate zulässig. Wenn Sie innerhalb dieses Sets ein weiteres Duplikat für dieses Asset hinzufügen, gibt die Anfrage entweder einen Fehler aus oder ignoriert das Duplikat.

Siehe auch [Grenzwerte für Dynamic Media](/help/using/limitations.md).

Die folgenden Schnellstarts zu Bildsets helfen Ihnen bei der schnellen Einrichtung und Ausführung von Bildset-Verfahren in Adobe Dynamic Media Classic.

## &#x200B;1. Laden Sie die primären Bilder für mehrere Ansichten und Farbfelder hoch

Laden Sie zuerst die Bilder für die Bildsätze hoch. Da Benutzer Bilder im Bildset-Viewer einzoomen können, sollten Sie diese Funktion bei der Auswahl von Bildern berücksichtigen. Achten Sie darauf, dass die längste Seite der Bilder mindestens 2.000 Pixel hat. Adobe Dynamic Media Classic unterstützt viele Bilddateiformate, empfohlen werden jedoch verlustfreie TIFF-, PNG- und EPS-Bilder.

Wählen Sie in der globalen Navigationsleiste **[!UICONTROL Hochladen]** aus, um Dateien von Ihrem Computer in einen Ordner in Adobe Dynamic Media Classic hochzuladen.

Siehe [Vorbereiten von Bildset-Assets auf den Upload](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) und [Hochladen von Dateien](uploading-files.md#uploading-your-files).

## &#x200B;2. Erstellen eines Bildsets

In Bildsets wählen Benutzerinnen und Benutzer Miniaturansichten im Bildset-Viewer aus, um ein Bild aus einer anderen Seite oder einem anderen Winkel anzuzeigen.

Wählen Sie zum Erstellen eines Bildsets in der globalen Navigationsleiste die Option **[!UICONTROL Erstellen]** und wählen Sie dann **[!UICONTROL Bildsets]**. Ziehen Sie im Fenster Bildset Ihre Bilder auf die Seite, um das Bildset zu erstellen. Organisieren und löschen Sie Bilder wie gewünscht und fügen Sie sie hinzu. 

Siehe [Erstellen eines Bildsets](creating-image-set.md#creating-an-image-set).

Siehe auch [Zoom-Ziele und Imagemaps in Bildsets einbeziehen](/help/using/including-zoom-targets-image-maps-image-sets.md)

## &#x200B;3. Bereiten Sie Viewer-Vorgaben für Bildsets nach Bedarf vor

Administratoren können Bildsatz-Viewer-Vorgaben erstellen oder ändern. Adobe Dynamic Media Classic verfügt über standardmäßige Viewer-Vorgaben für jeden Rich-Media-Typ. Verwenden Sie den Zoom-Viewer: **[!UICONTROL Benutzerdefiniert]** > **[!UICONTROL Bilder]** oder **[!UICONTROL Bildsets]**/**[!UICONTROL Mehrere Ansichten]**, um Ihre Bildsets anzuzeigen.

Sie können Viewer-Vorgaben über den Bildschirm „Anwendungseinstellungen“ hinzufügen oder bearbeiten.

Siehe [Erstellen und Bearbeiten von Viewer-](application-setup.md#adding-and-editing-viewer-presets).

## &#x200B;4. Vorschau eines Bildsets

Wählen Sie das Bildset im Durchsuchen-Bedienfeld aus und klicken Sie dann auf **[!UICONTROL Vorschau]**. Klicken Sie auf der Seite Vorschau auf die Miniaturansichtssymbole, um das Bildset im ausgewählten Viewer zu überprüfen. Sie können auch andere Vorgaben aus dem Menü „Vorgaben“ auswählen. 

Siehe [Vorschau eines Assets](previewing-asset.md#previewing-an-asset).

## &#x200B;5. Veröffentlichen eines Bildsets

Beim Veröffentlichen eines Bildsets wird es auf Adobe Dynamic Media Classic-Servern platziert und die URL-Zeichenfolge aktiviert.

>[!NOTE]
>
>Dieser Schritt ist nicht erforderlich, wenn Sie **[!UICONTROL Nach dem Speichern veröffentlichen]** (Standard) zum Zeitpunkt der Erstellung und Speicherung des Bildsets ausgewählt haben.

Wählen Sie **[!UICONTROL Symbol]** Zur Veröffentlichung markieren“ links neben seinem Namen im Durchsuchen-Bedienfeld aus. Wählen Sie dann **[!UICONTROL Veröffentlichen]** aus. Klicken Sie auf der Seite „Veröffentlichen“ auf **[!UICONTROL Veröffentlichung starten]**.

Siehe [Dateien veröffentlichen](publishing-files.md#publishing-files).

## &#x200B;6. Verknüpfen eines Bildsets mit einer Website

Adobe Dynamic Media Classic erstellt URL-Aufrufe für Bildsets und aktiviert diese nach deren Veröffentlichung. Sie können diese URLs im Anzeigebereich „Vorschau“ kopieren.

Wählen Sie das Bildset und dann **[!UICONTROL Vorschau]** aus. Wählen Sie jetzt eine Bildset-Viewer-Vorgabe aus und klicken Sie auf die Schaltfläche **[!UICONTROL URL kopieren]**.

Siehe [Verknüpfen des Bildsets mit einer Web-Seite](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
