---
title: Konfigurieren von Zoom-Viewer-Vorgaben
seo-title: Konfigurieren von Zoom-Viewer-Vorgaben
description: 'null'
seo-description: Hier erfahren Sie, wie Sie Zoom-Viewer-Vorgaben einrichten.
uuid: 202 d 80 cb -8282-45 d 4-89 e 8-942 c 8677 aa 93
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/zoom
discoiquuid: 5023 a 933-e 229-4 d 3 c -8 e 91-3 ac 5 e 9 f 4970 b
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Konfigurieren von Zoom-Viewer-Vorgaben{#setting-up-zoom-viewer-presets}

Mithilfe von Zoom-Viewer-Vorgaben wird der Stil, das Verhalten und das Aussehen von Zoom-Viewern festgelegt. Dynamic Media Classic bietet viele Optionen zum Anpassen und Gestalten von Viewern. Dynamic Media Classic verfügt über standardmäßige einfache (schnelle), Flyout- und benutzerdefinierte Zoom-Viewer-Vorgaben. Als Administrator können Sie neue unternehmensweite Zoom-Viewer-Vorgaben erstellen oder eine Standardvorgabe bearbeiten und sie unter einem neuen Namen speichern.

Alle Zoom-Viewer enthalten Schaltflächen zum Heranzoomen, Herauszoomen, Schwenken und Zurücksetzen des Bildes in seinen ursprünglichen Zustand vor dem Zoomen. Das Aussehen dieser Schaltflächen und des Fensters an sich hängt von den ausgewählten Zoom-Viewer-Vorgaben ab. Sie können eine Zoom-Viewer-Vorgabe mit unterschiedlichen Farben, Rahmen, Schriftarten und Bildeinstellungen konfigurieren. Wenn Sie einen Zoom-Viewer für geführtes Zoomen konfigurieren, können Sie darüber hinaus auch die Positionierung der Zoomziele festlegen. Zoomziele sind Miniaturansichten, auf die ein Benutzer klicken kann, um den von Ihnen zugeordneten Bildausschnitt heranzuzoomen.

## Zoom-Viewer-Vorgaben {#about-zoom-viewer-presets}

Dynamic Media Classic bietet diese Zoom-Viewer-Vorgaben:

**Zoom-Viewer: Einfach** Stellt einen einfachen Zoom für das Originalbild bereit.

**Zoom-Viewer: Flyout** Zeigt ein zweites Bild des gezoomten Bereichs neben dem Originalbild an. Der Benutzer hat keine Steuerelemente zur Verfügung. Er bewegt einfach die Auswahl über den Bereich, der angezeigt werden soll.

Bedenken Sie bei der Festlegung der gesamten Bandbreitennutzung für diesen Viewer, dass sowohl das Hauptbild als auch das Flyout-Bild im Viewer geladen werden müssen. Die Größe des Flyout-Bildes berechnet sich aus der Größe des Hauptbildes (Anzeigebreite und -höhe) und dem Zoomfaktor. Setzen Sie diese beiden Werte gut in Relation, damit das Flyout-Bild eine kompakte Dateigröße erhält. Wenn beispielsweise die Hauptbilddatei sehr groß ist, verringern Sie den Wert für den Zoomfaktor. (Die Flyout-Breite und Flyout-Höhe bestimmen die Größe des Flyout-Fensters, aber nicht die Größe des Flyout-Bildes, das in den Viewer geladen wird.)

Wenn die Größe des Hauptbildes beispielsweise 350 x 350 Pixel bei einem Zoomfaktor von 3 beträgt, ist das Flyout-Bild 1050 x 1050 Pixel groß. Wenn die Größe des Hauptbildes 300 x 300 Pixel bei einem Zoomfaktor von 4 beträgt, ist das Flyout-Bild 1200 x 1200 Pixel groß. Über die Einstellung für die JPEG-Qualität (empfohlener Wert: zwischen 80 und 90) können Sie die Dateigröße deutlich reduzieren. Der empfohlene Wert für den Zoomfaktor liegt, je nach Größe des Hauptbildes, zwischen 2,5 und 4.

Dynamic Media Classic empfiehlt diese Parameter für Flyout-Zoom-Viewer-Vorgaben:

**Vergrößerte Bildgröße** ca. 1500 x 1500 Pixel, nicht 2000 x 2000 Pixel.

**Bildgröße** 100 KB oder darunter, höchstens 150 KB (komprimieren Sie die Datei, um sie unter 150 KB zu halten).

**Zoom-Viewer: Benutzerdefiniert** bietet geführte oder nicht gezeigte Zoom-Gesten mit Bildern, Bildsätzen mit mehreren Ansichten oder Farbmustersets.

## Erstellen und Bearbeiten von Zoom-Viewer-Vorgaben {#creating-and-editing-zoom-viewer-presets}

Führen Sie zum Erstellen oder Bearbeiten einer Zoom-Viewer-Vorgabe folgende Schritte aus:

1. Klicken Sie auf **Einstellungen** &gt; **Viewer-Vorgaben**.
1. Führen Sie einen der folgenden Schritte aus:

   **Erstellen einer Vorgabe durch** Klicken auf "Hinzufügen" . Wählen Sie im Dialogfeld "Viewer-Vorgabe hinzufügen" eine Plattform aus, wählen Sie einen Zoom-Viewer aus und klicken Sie auf" Hinzufügen" . Geben Sie im Feld "Vorgabenname" einen Namen für die Vorgabe ein.

   **Bearbeiten einer Vorgabe** Wählen Sie eine Zoom-Viewer-Vorgabe aus und klicken Sie auf **Bearbeiten**.

1. Wählen Sie die gewünschten Einstellungen aus.

   Um eine Beschreibung einer Option anzuzeigen, klicken Sie neben der Option auf das Symbol „Tipp“ .

   Im Anzeigebereich „Vorschau“ werden jeweils die Auswirkungen der vorgenommenen Änderungen angezeigt.

1. Klicken Sie auf **Speichern** oder **Speicher unter**.
1. Überprüfen Sie im Anzeigebereich „Viewer-Vorgaben“ die neu erstellte Zoom-Viewer-Vorgabe bzw. Zoom-Viewer-Vorgabe für geführtes Zoomen. If it needs adjusting, click **Edit**, change settings on the Configure Viewer screen, and click **Save**.

Informationen zum Verwalten von Viewer-Vorgaben im Anzeigebereich „Viewer-Vorgaben“ finden Sie unter [Viewer-Vorgaben](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Erstellen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding_and_editing_viewer_presets)

