---
title: Viewer-Vorgaben für Zoom einrichten
description: Erfahren Sie, wie Sie Viewer-Vorgaben für Zoom in Adobe Dynamic Media Classic einrichten.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ddaaff6c-5447-408e-9c92-bcdfd1a0e72e
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 40%

---

# Viewer-Vorgaben für Zoom einrichten{#setting-up-zoom-viewer-presets}

Zoom-Viewer-Vorgaben bestimmen den Stil, das Verhalten und das Erscheinungsbild Ihrer Zoom-Viewer. Adobe Dynamic Media Classic bietet viele Optionen zum Anpassen und Gestalten von Viewern. Adobe Dynamic Media Classic verfügt über die standardmäßigen Viewer-Vorgaben „Standard“ (schnell), „Fly-out“ und „Benutzerdefiniert“ für Zoom. Als Administrator können Sie Viewer-Vorgaben für den Unternehmenszoom erstellen oder eine Standardvorgabe bearbeiten und unter einem neuen Namen speichern.

Alle Zoom-Viewer enthalten Schaltflächen zum Heranzoomen, Herauszoomen, Schwenken und Zurücksetzen des Bildes in seinen ursprünglichen Zustand vor dem Zoomen. Wie diese Schaltflächen aussehen und wie das Fenster selbst angezeigt wird, hängt von der Auswahl der Viewer-Vorgaben für Zoom ab. Sie können eine Zoom-Viewer-Vorgabe mit unterschiedlichen Farben, Rahmen, Schriftarten und Bildeinstellungen konfigurieren. Bei der Konfiguration eines geführten Zoom-Viewers können Sie auch auswählen, wo die Zoom-Ziele platziert werden sollen. Zoomziele sind Miniaturansichten, auf die ein Benutzer klicken kann, um den von Ihnen zugeordneten Bildausschnitt heranzuzoomen.

## Zoom-Viewer-Vorgaben {#about-zoom-viewer-presets}

Adobe Dynamic Media Classic bietet die folgenden Zoom-Viewer-Vorgaben:

* **Zoom-Viewer:**: Bietet einen einfachen Zoom auf dem Originalbild.

* **Zoom-Viewer:**-Out: Zeigt ein zweites Bild des gezoomten Bereichs neben dem Originalbild an. Der Benutzer hat keine Steuerelemente zur Verfügung. Er bewegt einfach die Auswahl über den Bereich, der angezeigt werden soll.

Bedenken Sie bei der Festlegung der gesamten Bandbreitennutzung für diesen Viewer, dass sowohl das Hauptbild als auch das Flyout-Bild im Viewer geladen werden müssen. Die Größe des Flyout-Bildes wird anhand der Hauptbildgröße (Bühnenbreite und -höhe) und des Zoom-Faktors bestimmt. Setzen Sie diese beiden Werte gut in Relation, damit das Flyout-Bild eine kompakte Dateigröße erhält. Wenn beispielsweise die Hauptbilddatei sehr groß ist, verringern Sie den Wert für den Zoomfaktor. (Die Flyout-Breite und Flyout-Höhe bestimmen die Größe des Flyout-Fensters, aber nicht die Größe des Flyout-Bildes, das in den Viewer geladen wird.)

Wenn die Größe des Hauptbildes beispielsweise 350 x 350 Pixel bei einem Zoomfaktor von 3 beträgt, ist das Flyout-Bild 1050 x 1050 Pixel groß. Wenn die Größe des Hauptbildes 300 x 300 Pixel bei einem Zoomfaktor von 4 beträgt, ist das Flyout-Bild 1200 x 1200 Pixel groß. Über die Einstellung für die JPEG-Qualität (empfohlener Wert: zwischen 80 und 90) können Sie die Dateigröße deutlich reduzieren. Der empfohlene Wert für den Zoomfaktor liegt, je nach Größe des Hauptbildes, zwischen 2,5 und 4.

Adobe Dynamic Media Classic empfiehlt die folgenden Parameter für ausfliegende Zoom-Viewer-Vorgaben:

* **Vergrößerte Bildgröße**: Ca. 1500 x 1500 Pixel, darf 2000 x 2000 Pixel nicht überschreiten.

* **Bildgröße**: 100 KB oder weniger, maximal 150 KB (komprimieren Sie die Datei unter 150 KB).

* **Zoom-Viewer: Benutzerdefiniert**: Bietet geführtes oder nicht geführtes Zoomen mit Bildern, Bildsets mit mehreren Ansichten oder Farbmustergruppen.

## Erstellen und Bearbeiten von Zoom-Viewer-Vorgaben {#creating-and-editing-zoom-viewer-presets}

1. Wechseln Sie in der globalen Navigationsleiste zu **[!UICONTROL Einstellungen]** > **[!UICONTROL Viewer-Vorgaben]**.
1. Führen Sie einen der folgenden Schritte aus:

   * **Voreinstellung erstellen** Wählen Sie **[!UICONTROL Hinzufügen]** aus. Wählen Sie im Dialogfeld „Viewer-Vorgabe hinzufügen“ eine Plattform, einen Zoom-Viewer und anschließend **[!UICONTROL Hinzufügen]** aus. Geben Sie in das Feld „Vorgabenname“ einen Namen für die Vorgabe ein.

   * **Bearbeiten einer Vorgabe**: Wählen Sie eine Vorgabe für den Zoom-Viewer aus und klicken Sie dann auf **[!UICONTROL Bearbeiten]**.

1. Wählen Sie die gewünschten Einstellungen aus.

   Um eine Beschreibung einer Option anzuzeigen, klicken Sie auf das Symbol **[!UICONTROL Info-]**) neben der Option.

   Auf der Seite Vorschau wird der Viewer angezeigt, während Sie die Einstellungen aktualisieren und ändern.

1. Wählen Sie **[!UICONTROL Speichern]** oder **[!UICONTROL Speichern unter]**.
1. Überprüfen Sie auf der Seite „Viewer-Vorgaben“ die von Ihnen erstellte Viewer-Vorgabe für Zoom oder Geführter Zoom. Wenn Anpassungen erforderlich sind, wählen Sie **[!UICONTROL Bearbeiten]**, ändern Sie die Einstellungen auf der `Configure Viewer` Seite und klicken Sie dann auf **[!UICONTROL Speichern]**.

Informationen zum Verwalten von Viewer-Vorgaben im Anzeigebereich „Viewer-Vorgaben“ finden Sie unter [Viewer-Vorgaben](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Erstellen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding_and_editing_viewer_presets)
