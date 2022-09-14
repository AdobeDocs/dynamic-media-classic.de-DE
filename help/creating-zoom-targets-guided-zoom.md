---
title: Zoomziele für geführten Zoom erstellen
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic Zoomziele für geführtes Zoomen erstellen.
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 41%

---

# Zoomziele für geführten Zoom erstellen{#creating-zoom-targets-for-guided-zoom}

Anhand von Zoomzielen wird die Aufmerksamkeit der Betrachter auf bestimmte Bildausschnitte gelenkt. Neben dem Freiformzoomen können Viewer eine Miniaturansicht des Zoomziels auswählen und auf den Teil des Bildes zoomen, auf den sie sich konzentrieren sollen. Zoomziele bieten Ihnen die Möglichkeit, besonders attraktive oder interessante Bildausschnitte hervorzuheben.

![Zoomziele für geführten Zoom erstellen](/help/assets/zo_guided_zoom.png)

## Zoomziele {#about-zoom-targets}

Der maximale Zoomprozentsatz für Zoomziele ist 100 %. Der minimale Zoomprozentsatz variiert in Abhängigkeit von einer Kombination aus Viewer-Größe und Bildgröße, wie in folgender Tabelle dargestellt:

| Bildgröße | Viewer-Größe | Zoomprozentsatz |
| --- | --- | --- |
| Groß | Kleiner | Kleinerer Minimalwert |
| Klein | Größer | Größerer Minimalwert |

Sie können die Größe des Zoom-Viewers an die auf der Website verwendete Größe anpassen. Um diese Einstellung dauerhaft zu ändern, können Sie im Anzeigebereich „Einstellungen“ die Viewer-Größe entsprechend ändern (sofern Sie ein Administrator sind). Siehe [Einrichten von Zoom-Viewer-Vorgaben](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## Zoomziele erstellen und bearbeiten {#creating-and-editing-zoom-targets}

Im Zoomziel-Editor erstellen und bearbeiten Sie Zoomziele. Um diesen Editor zu öffnen, wählen Sie ein Bild und führen Sie einen der folgenden Schritte aus:

* Rollover auswählen **[!UICONTROL Bearbeiten]** und wählen Sie &quot;Zoomziele&quot;.
* Zeigen Sie das Bild im Durchsuchenbedienfeld in **[!UICONTROL Detailansicht]**, wählen Sie **[!UICONTROL Zoomziele]**.

Wählen Sie im Bildschirm &quot;Zoomziel-Editor&quot;die Option **[!UICONTROL Ziel auswählen]** Schaltfläche (Pfeil), um ein Ziel auszuwählen, bevor es seine Größe oder Position ändert. Um ein Zoomziel für das Bild zu erstellen, wählen Sie **[!UICONTROL Zielgruppen hinzufügen]** (Rechteck). Auf der Seite &quot;Zoom-Ziel-Editor&quot;finden Sie außerdem Tools zum Löschen, Kopieren und Benennen von Zoomzielen.

### Zoomziel erstellen {#creating-a-zoom-target}

Um ein Zoomziel zu erstellen, öffnen Sie die Seite &quot;Zoomziel-Editor&quot;und führen Sie die folgenden Schritte aus:

1. Auswählen **[!UICONTROL Zielgruppen hinzufügen]** (Rechteck), bewegen Sie den Mauszeiger über das Bild und wählen Sie aus, wo das Zoomziel liegen soll.

   Ein Miniaturbild des Zoomziels wird im Bedienfeld im rechten Anzeigebereich angezeigt.

1. Auswahl **[!UICONTROL Ziel auswählen]** (Pfeil), wählen Sie dann das von Ihnen erstellte Zoomziel aus und passen Sie Größe und Position des Ziels an.

   * **Größe ändern** - Bewegen Sie den Mauszeiger über eine Ecke des Zoomziels und ziehen Sie, um das Ziel zu vergrößern oder zu verkleinern.

   * **Position** - Bewegen Sie den Mauszeiger über das Zoomziel und ziehen Sie es an eine andere Position.

1. Geben Sie im Feld „Name“ einen Namen für das Zoomziel ein.

   >[!NOTE]
   >
   >In das Feld „Name“ geben Sie mehr als nur einen Namen ein. Wenn Benutzer den Zeiger über das Zoomziel bewegen, sehen sie, was Sie in das Feld „Name“ eingegeben haben. Geben Sie eine kurze Beschreibung des Zoomziels in das Feld „Name“ ein, damit die Benutzer wissen, auf was sie zoomen können.

1. Optional können Sie im Feld „Benutzerdaten“ entsprechende Informationen eingeben. Dieses Feld dient Website-Designern dazu, dem Zoomziel Informationen hinzuzufügen.
1. Auswählen **[!UICONTROL Speichern]**.

   Die Koordinaten und Zoomstärke des Zoomziels werden gespeichert. Eine Miniaturansicht Ihres Zoomziels mit dem von Ihnen eingegebenen Namen wird rechts im Anzeigebereich eingeblendet.

>[!NOTE]
>
>Um zu sehen, wie die Zoomziele in einem Zoom-Viewer aussehen, wählen Sie die **[!UICONTROL Vorschau]** im Zoomziel-Editor und wählen Sie im Vorschaubildschirm einen Zoom-Viewer aus. Weitere Informationen zu diesem Bildschirm finden Sie unter [Vorschau von Bildern mit unterschiedlichen Zoom-Viewern](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### Zoomziele bearbeiten {#editing-zoom-targets}

Verwenden Sie zum Bearbeiten von Zoomzielen die folgenden Verfahren auf der Seite &quot;Zoomziel-Editor&quot;:

* **Reposition** - Wählen Sie mit der Schaltfläche Ziel auswählen (Pfeil) das Ziel aus. Ziehen Sie das Ziel dann an eine andere Position.

* **Größe ändern** - Wählen Sie mit der Schaltfläche Ziel auswählen (Pfeil) das Ziel aus. Um das Ziel zu vergrößern oder zu verkleinern, bewegen Sie den Mauszeiger über eine Ecke des Zoomziels und ziehen Sie.

* **Löschen** - Wählen Sie rechts im Bildschirm das Miniaturbild des Ziels aus. Wählen Sie anschließend **[!UICONTROL Ziel löschen]**.

* **Umbenennen** - Wählen Sie rechts im Bildschirm das Miniaturbild des Ziels aus. Geben Sie dann einen Namen in die **[!UICONTROL Name]** Textfeld und wählen Sie **[!UICONTROL Speichern]**.

### Zoomziele kopieren {#copying-zoom-targets}

Sie können Zoomziele von einem Bild zu einem anderen kopieren. Kopieren Sie Ziele, wenn zwei Bilder ähnlichen Inhalt haben und ihre Zoomziele zu den gleichen Orten gehören. Gehen Sie wie folgt vor, um Zoomziele in ein anderes Bild zu kopieren:

1. Öffnen Sie das Bild mit den Zoomzielen, die Sie kopieren möchten, im Zoomziel-Editor.
1. Auswählen **[!UICONTROL Zielgruppen kopieren nach]**.
1. Wählen Sie im Dialogfeld Bilder auswählen ein Bild aus und wählen Sie **[!UICONTROL Auswählen]**.
