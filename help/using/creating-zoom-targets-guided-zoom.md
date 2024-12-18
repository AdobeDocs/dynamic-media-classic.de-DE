---
title: Erstellen von Zoom-Zielen für geführtes Zoomen
description: Erfahren Sie, wie Sie Zoom-Ziele für geführtes Zoomen in Adobe Dynamic Media Classic erstellen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 27%

---

# Erstellen von Zoom-Zielen für geführtes Zoomen{#creating-zoom-targets-for-guided-zoom}

Anhand von Zoomzielen wird die Aufmerksamkeit der Betrachter auf bestimmte Bildausschnitte gelenkt. Neben dem Freiform-Zoomen können Betrachterinnen und Betrachter ein Zoom-Ziel-Miniaturbild auswählen und auf den Teil des Bildes zoomen, auf den sie sich konzentrieren sollen. Zoomziele bieten Ihnen die Möglichkeit, besonders attraktive oder interessante Bildausschnitte hervorzuheben.

![Erstellen von Zoom-Zielen für geführtes Zoomen](/help/using/assets/zo_guided_zoom.png)

## Über Zoom-Ziele {#about-zoom-targets}

Der maximale Zoom-Prozentsatz von Zoom-Zielen beträgt 100 Prozent. Der minimale Zoomprozentsatz variiert in Abhängigkeit von einer Kombination aus Viewer-Größe und Bildgröße, wie in folgender Tabelle dargestellt:

| Bildgröße | Viewer-Größe | Zoomprozentsatz |
| --- | --- | --- |
| Groß | Kleiner | Kleinerer Minimalwert |
| Klein | Größer | Größerer Minimalwert |

Sie können die Größe des Zoom-Viewers an die auf Ihrer Web-Seite verwendete Größe anpassen. Sie können diese Einstellung dauerhaft ändern, indem Sie die Viewer-Größe auf dem Bildschirm „Einstellungen“ ändern (wenn Sie Administrator sind). Siehe [Einrichten von Viewer-Vorgaben für Zoom](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Erstellen und Bearbeiten von Zoom-Zielen {#creating-and-editing-zoom-targets}

Erstellen und bearbeiten Sie Zoom-Ziele im Bildschirm Zoom-Ziel-Editor . Um diesen Editor zu öffnen, wählen Sie ein Bild und führen Sie einen der folgenden Schritte aus:

* Klicken Sie auf die Schaltfläche **[!UICONTROL Bearbeiten]** und wählen Sie Zoom-Ziele aus.
* Zeigen Sie das Bild im Durchsuchen-Panel in der **[!UICONTROL Detailansicht]** an und wählen Sie dann **[!UICONTROL Zoom-Ziele]** aus.

Klicken Sie im Bildschirm Zoom-Ziel-Editor auf die Schaltfläche **[!UICONTROL Ziel auswählen]** (Pfeil), um ein Ziel auszuwählen, bevor Sie dessen Größe oder Position ändern. Um ein Zoom-Ziel auf dem Bild zu erstellen, wählen Sie **[!UICONTROL Ziele hinzufügen]** (Rechteck) aus. Die Seite Zoom-Ziel-Editor bietet auch Tools zum Löschen, Kopieren und Benennen von Zoom-Zielen.

### Erstellen eines Zoom-Ziels {#creating-a-zoom-target}

Um ein Zoom-Ziel zu erstellen, öffnen Sie die Seite Zoom-Ziel-Editor und gehen Sie wie folgt vor:

1. Wählen Sie **[!UICONTROL Ziele hinzufügen]** (Rechteck) aus, bewegen Sie den Mauszeiger über das Bild und wählen Sie aus, wo sich das Zoom-Ziel befinden soll.

   Ein Miniaturbild des Zoomziels wird im Bedienfeld im rechten Anzeigebereich angezeigt.

1. Wählen Sie **[!UICONTROL Ziel auswählen]** (Pfeil) aus, wählen Sie dann das erstellte Zoomziel aus und passen Sie die Größe und Position des Ziels an.

   * **Größe ändern**: Bewegen Sie den Mauszeiger über eine Ecke des Zoomziels und ziehen Sie, um das Ziel zu vergrößern oder zu verkleinern.

   * **Position**: Bewegen Sie den Mauszeiger über das Zoom-Ziel und ziehen Sie es an eine andere Position.

1. Geben Sie im Feld „Name“ einen Namen für das Zoomziel ein.

   >[!NOTE]
   >
   >In das Feld „Name“ geben Sie mehr als nur einen Namen ein. Wenn Benutzer den Zeiger über das Zoomziel bewegen, sehen sie, was Sie in das Feld „Name“ eingegeben haben. Geben Sie eine kurze Beschreibung des Zoomziels in das Feld „Name“ ein, damit die Benutzer wissen, auf was sie zoomen können.

1. Optional können Sie im Feld „Benutzerdaten“ entsprechende Informationen eingeben. In diesem Feld können Website-Designer dem Zoom-Ziel Informationen hinzufügen.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

   Die Koordinaten und Zoomstärke des Zoomziels werden gespeichert. Eine Miniaturansicht Ihres Zoomziels mit dem von Ihnen eingegebenen Namen wird rechts im Anzeigebereich eingeblendet.

>[!NOTE]
>
>Um zu sehen, wie Ihre Zoom-Ziele in einem Zoom-Viewer aussehen, wählen Sie die Schaltfläche **[!UICONTROL Vorschau]** im Bildschirm Zoom-Ziel-Editor aus. Wählen Sie dann im Bildschirm Vorschau einen Zoom-Viewer aus. Weitere Informationen zu diesem Bildschirm finden Sie unter [Vorschau von Bildern mit verschiedenen Zoom-Viewern](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Zoom-Ziele bearbeiten {#editing-zoom-targets}

Um Zoom-Ziele zu bearbeiten, verwenden Sie die folgenden Techniken auf der Seite Zoom-Ziel-Editor :

* **Neu positionieren**: Wählen Sie mit der Schaltfläche Ziel auswählen (Pfeil) das Ziel aus. Ziehen Sie das Ziel dann an eine andere Position.

* **Größe ändern**: Wählen Sie mit der Schaltfläche Ziel auswählen (Pfeil) das Ziel aus. Um das Ziel zu vergrößern oder zu verkleinern, bewegen Sie den Mauszeiger über eine Ecke des Zoom-Ziels und ziehen Sie es.

* **Löschen**: Wählen Sie das Miniaturbild des Ziels auf der rechten Bildschirmseite aus. Wählen Sie dann **[!UICONTROL Ziel löschen]** aus.

* **Umbenennen**: Wählen Sie das Miniaturbild des Ziels auf der rechten Bildschirmseite aus. Geben Sie dann einen Namen in das Textfeld **[!UICONTROL Name]** ein und wählen Sie **[!UICONTROL Speichern]**.

### Zoom-Ziele kopieren {#copying-zoom-targets}

Sie können Zoom-Ziele von einem Bild in ein anderes kopieren. Kopieren Sie Ziele, wenn zwei Bilder ähnliche Inhalte aufweisen und ihre Zoom-Ziele zu denselben Speicherorten gehören. Gehen Sie wie folgt vor, um Zoom-Ziele in ein anderes Bild zu kopieren:

1. Öffnen Sie das Bild mit Zoom-Zielen, die Sie in den Bildschirm des Zoom-Ziel-Editors kopieren möchten.
1. Wählen Sie **[!UICONTROL Ziele kopieren nach]**.
1. Wählen Sie im Dialogfeld Bilder auswählen ein Bild aus und klicken Sie auf **[!UICONTROL Auswählen]**.
