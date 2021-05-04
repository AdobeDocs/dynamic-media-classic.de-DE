---
title: Konfigurieren von Zoom-Viewer-Vorgaben
description: Erfahren Sie, wie Sie Zoom-Viewer-Vorgaben einrichten.
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
feature: Dynamic Media Classic, Viewer, Zoom
role: Business Practitioner
exl-id: ddaaff6c-5447-408e-9c92-bcdfd1a0e72e
translation-type: tm+mt
source-git-commit: 9d73e74ffc4a1e7e31c84720a9bae105b6afb1ae
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 52%

---

# Konfigurieren von Zoom-Viewer-Vorgaben{#setting-up-zoom-viewer-presets}

Mithilfe von Zoom-Viewer-Vorgaben wird der Stil, das Verhalten und das Aussehen von Zoom-Viewern festgelegt. Dynamic Media Classic bietet viele Optionen zum Anpassen und Skin von Viewern. Im Lieferumfang von Dynamic Media Classic sind standardmäßige einfache (schnelle), Flyout- und benutzerdefinierte Zoom-Viewer-Vorgaben enthalten. Als Administrator können Sie Zoom-Viewer-Vorgaben für Firmen erstellen oder eine Standardvorgabe bearbeiten und unter einem neuen Namen speichern.

Alle Zoom-Viewer enthalten Schaltflächen zum Heranzoomen, Herauszoomen, Schwenken und Zurücksetzen des Bildes in seinen ursprünglichen Zustand vor dem Zoomen. Wie diese Schaltflächen aussehen und wie das Fenster selbst angezeigt wird, hängt von Ihrer Wahl der Zoom-Viewer-Vorgaben ab. Sie können eine Zoom-Viewer-Vorgabe mit unterschiedlichen Farben, Rahmen, Schriftarten und Bildeinstellungen konfigurieren. Wenn Sie einen Zoom-Viewer für geführtes Zoomen konfigurieren, können Sie darüber hinaus auch die Positionierung der Zoomziele festlegen. Zoomziele sind Miniaturansichten, auf die ein Benutzer klicken kann, um den von Ihnen zugeordneten Bildausschnitt heranzuzoomen.

## Zoom-Viewer-Vorgaben {#about-zoom-viewer-presets}

Dynamic Media Classic-Angebote:

* **Zoom-Viewer: Einfach**  - Bietet einen einfachen Zoom auf das Originalbild.

* **Zoom-Viewer: Fly-out** : Zeigt ein zweites Bild des gezoomten Bereichs neben dem Originalbild an. Der Benutzer hat keine Steuerelemente zur Verfügung. Er bewegt einfach die Auswahl über den Bereich, der angezeigt werden soll.

Bedenken Sie bei der Festlegung der gesamten Bandbreitennutzung für diesen Viewer, dass sowohl das Hauptbild als auch das Flyout-Bild im Viewer geladen werden müssen. Die Größe des Flyout-Bildes berechnet sich aus der Größe des Hauptbildes (Anzeigebreite und -höhe) und dem Zoomfaktor. Setzen Sie diese beiden Werte gut in Relation, damit das Flyout-Bild eine kompakte Dateigröße erhält. Wenn beispielsweise die Hauptbilddatei sehr groß ist, verringern Sie den Wert für den Zoomfaktor. (Die Flyout-Breite und Flyout-Höhe bestimmen die Größe des Flyout-Fensters, aber nicht die Größe des Flyout-Bildes, das in den Viewer geladen wird.)

Wenn die Größe des Hauptbildes beispielsweise 350 x 350 Pixel bei einem Zoomfaktor von 3 beträgt, ist das Flyout-Bild 1050 x 1050 Pixel groß. Wenn die Größe des Hauptbildes 300 x 300 Pixel bei einem Zoomfaktor von 4 beträgt, ist das Flyout-Bild 1200 x 1200 Pixel groß. Über die Einstellung für die JPEG-Qualität (empfohlener Wert: zwischen 80 und 90) können Sie die Dateigröße deutlich reduzieren. Der empfohlene Wert für den Zoomfaktor liegt, je nach Größe des Hauptbildes, zwischen 2,5 und 4.

Dynamic Media Classic empfiehlt die folgenden Parameter für Flyout-Zoom-Viewer-Vorgaben:

* **Vergrößerte Bildgröße** : Ungefähr 1500 x 1500 Pixel, nicht größer als 2000 x 2000 Pixel.

* **Bildgröße** : 100 KB oder weniger, maximal 150 KB (komprimieren Sie die Datei, um sie unter 150 KB zu halten).

* **Zoom-Viewer: Benutzerdefiniert** : Bietet geführtes oder nicht gezähltes Zoomen mit Bildern, Bildsätzen mit mehreren Ansichten oder Farbfeldsätzen.

## Erstellen und Bearbeiten von Zoom-Viewer-Vorgaben {#creating-and-editing-zoom-viewer-presets}

1. Klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Setup]** > **[!UICONTROL Viewer-Vorgaben]**.
1. Führen Sie einen der folgenden Schritte aus:

   * **Erstellen einer Vorgabe**  - Klicken Sie auf  **[!UICONTROL Hinzufügen]**. Wählen Sie im Dialogfeld &quot;Hinzufügen-Viewer-Vorgabe&quot;eine Plattform, wählen Sie einen Zoom-Viewer und klicken Sie dann auf **[!UICONTROL Hinzufügen]**. Geben Sie im Feld &quot;Vorgabenname&quot;einen Namen für die Vorgabe ein.

   * **Bearbeiten einer Vorgabe** : Wählen Sie eine Zoom-Viewer-Vorgabe und klicken Sie dann auf  **[!UICONTROL Bearbeiten]**.

1. Wählen Sie die gewünschten Einstellungen aus.

   Um eine Beschreibung einer Option anzuzeigen, klicken Sie neben der Option auf das Symbol **[!UICONTROL Info Tipp]**.

   Auf der Seite &quot;Vorschau&quot;wird der Viewer angezeigt, während Sie die Einstellungen aktualisieren und ändern.

1. Klicken Sie auf **[!UICONTROL Speichern]** oder **[!UICONTROL Speicher unter]**.
1. Überprüfen Sie auf der Seite &quot;Viewer-Vorgaben&quot;die erstellte Zoom-Viewer-Vorgabe oder Zoom-Viewer-Vorgabe für geführtes Zoomen. Wenn Sie eine Anpassung vornehmen müssen, klicken Sie auf **[!UICONTROL Bearbeiten]**, ändern Sie die Einstellungen auf der Seite &quot;Viewer konfigurieren&quot;und klicken Sie auf ****[!UICONTROL Speichern]****.

Informationen zum Verwalten von Viewer-Vorgaben im Anzeigebereich „Viewer-Vorgaben“ finden Sie unter [Viewer-Vorgaben](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Erstellen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding_and_editing_viewer_presets)

