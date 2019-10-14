---
title: Erstellen von Zoomzielen für geführten Zoom
seo-title: Erstellen von Zoomzielen für geführten Zoom
description: 'null'
seo-description: Erfahren Sie, wie Sie Zoomziele für geführtes Zoomen erstellen.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: admin
content-type: Verweis
products: SG_EXPERIENCEMANAGER/Dynamic Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Erstellen von Zoomzielen für geführten Zoom{#creating-zoom-targets-for-guided-zoom}

Anhand von Zoomzielen wird die Aufmerksamkeit der Betrachter auf bestimmte Bildausschnitte gelenkt. Neben dem freien Zoomen können Betrachter auch auf die Miniaturansicht eines Zoomziels klicken und direkt den Bildausschnitt heranzoomen, den Sie hervorheben möchten. Zoomziele bieten Ihnen die Möglichkeit, besonders attraktive oder interessante Bildausschnitte hervorzuheben.

![Erstellen von Zoomzielen für geführten Zoom](/help/assets/zo_guided_zoom.png)

## Zoomziele {#about-zoom-targets}

Der maximale Zoomprozentsatz für Zoomziele ist 100 %. Der minimale Zoomprozentsatz variiert in Abhängigkeit von einer Kombination aus Viewer-Größe und Bildgröße, wie in folgender Tabelle dargestellt:

| Bildgröße | Viewer-Größe | Zoomprozentsatz |
|--- |--- |--- |
| Groß | Kleiner | Kleinerer Minimalwert |
| Klein | Größer | Größerer Minimalwert |

Sie können die Größe des Zoom-Viewers an die auf der Website verwendete Größe anpassen. Um diese Einstellung dauerhaft zu ändern, können Sie im Anzeigebereich „Einstellungen“ die Viewer-Größe entsprechend ändern (sofern Sie ein Administrator sind). Siehe [Konfigurieren von Zoom-Viewer-Vorgaben](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Erstellen und Bearbeiten von Zoomzielen {#creating-and-editing-zoom-targets}

Im Zoomziel-Editor erstellen und bearbeiten Sie Zoomziele. Um diesen Editor zu öffnen, wählen Sie ein Bild und führen Sie einen der folgenden Schritte aus:

* Click the rollover **[!UICONTROL Edit]** button and choose Zoom Targets.
* In the Browse Panel, display the image in **[!UICONTROL Detail View]**, then click **[!UICONTROL Zoom Targets]**.

On the Zoom Target Editor screen, click **[!UICONTROL Select Target]** button (arrow) to select a target before changing its size or position. Click **[!UICONTROL Add Targets]** (rectangle) to create a zoom target on the image. Der Zoomziel-Editor bietet außerdem Werkzeuge zum Löschen, Kopieren und Benennen von Zoomzielen.

### Erstellen eines Zoomziels {#creating-a-zoom-target}

Öffnen Sie den Zoomziel-Editor und führen Sie folgende Schritte aus, um ein Zoomziel zu erstellen:

1. Click **[!UICONTROL Add Targets]** (rectangle), move the pointer over the image, and click where you want to the zoom target to be.

   Ein Miniaturbild des Zoomziels wird im Bedienfeld im rechten Anzeigebereich angezeigt.

1. Click **[!UICONTROL Select Target]** (arrow), click to select the zoom target you created, and adjust the size and position of the target.

   * **Größenanpassung** Bewegen Sie den Zeiger über eine Ecke des Zoomziels und ziehen Sie, um das Ziel zu vergrößern oder zu verkleinern.

   * **Positionierung** Bewegen Sie den Zeiger über das Zoomziel und ziehen Sie es an eine andere Position.

1. Geben Sie im Feld „Name“ einen Namen für das Zoomziel ein.

   >[!NOTE]
   >
   >In das Feld „Name“ geben Sie mehr als nur einen Namen ein. Wenn Benutzer den Zeiger über das Zoomziel bewegen, sehen sie, was Sie in das Feld „Name“ eingegeben haben. Geben Sie eine kurze Beschreibung des Zoomziels in das Feld „Name“ ein, damit die Benutzer wissen, auf was sie zoomen können.

1. Optional können Sie im Feld „Benutzerdaten“ entsprechende Informationen eingeben. Dieses Feld dient Website-Designern dazu, dem Zoomziel Informationen hinzuzufügen.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Die Koordinaten und Zoomstärke des Zoomziels werden gespeichert. Eine Miniaturansicht Ihres Zoomziels mit dem von Ihnen eingegebenen Namen wird rechts im Anzeigebereich eingeblendet.

>[!NOTE]
>
>Um sich eine Vorschau Ihrer Zoomziele in einem Zoom-Viewer anzeigen zu lassen, klicken Sie im Zoomziel-Editor auf die Schaltfläche „Vorschau“ und wählen Sie im Anzeigebereich „Vorschau“ einen Zoom-Viewer aus. Informationen zu diesem Anzeigebereich finden Sie unter [Anzeigen einer Vorschau von Bildern mit verschiedenen Zoom-Viewern](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Bearbeiten von Zoomzielen {#editing-zoom-targets}

Mit den folgenden Techniken können Sie im Zoomziel-Editor Zoomziele bearbeiten:

* **Positionieren** Sie das Ziel mithilfe der Schaltfläche "Ziel auswählen"(Pfeil) neu, und klicken Sie auf das Ziel, um es auszuwählen. Ziehen Sie das Ziel dann an eine andere Position.

* **Wenn Sie die Größe** mit der Schaltfläche "Ziel auswählen"ändern möchten (Pfeil), klicken Sie auf das Ziel, um es auszuwählen. Bewegen Sie den Zeiger dann über eine Ecke des Zoomziels und ziehen Sie, um das Ziel zu vergrößern oder zu verkleinern.

* **Löschen** Klicken Sie auf das Miniaturbild des Ziels auf der rechten Seite des Bildschirms. Klicken Sie dann auf Ziel **[!UICONTROL löschen]**.

* **Umbenennen** Klicken Sie auf das Miniaturbild des Ziels auf der rechten Seite des Bildschirms. Then enter a name in the **[!UICONTROL Name]** text field and click **[!UICONTROL Save]**.

### Kopieren von Zoomzielen {#copying-zoom-targets}

Sie können Zoomziele von einem Bild zu einem anderen kopieren. Kopieren Sie Ziele, wenn zwei Bilder ähnlichen Inhalt haben und ihre Zoomziele zu den gleichen Orten gehören. Um Zoomziele in ein anderes Bild zu kopieren, führen Sie die folgenden Schritte aus:

1. Öffnen Sie das Bild mit den Zoomzielen, die Sie im Zoomziel-Editor kopieren möchten.
1. Klicken Sie auf Ziele **[!UICONTROL kopieren nach]**.
1. In the Select Images dialog box, select an image and click **[!UICONTROL Select]**.

