---
title: Einrichten von Zoom-Viewer-Vorgaben
description: Erfahren Sie, wie Sie Zoom-Viewer-Vorgaben in Adobe Dynamic Media Classic einrichten.
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

# Einrichten von Zoom-Viewer-Vorgaben{#setting-up-zoom-viewer-presets}

Zoom-Viewer-Vorgaben bestimmen Stil, Verhalten und Aussehen Ihrer Zoom-Viewer. Adobe Dynamic Media Classic bietet viele Optionen zum Anpassen und Entschlüsseln von Viewern. Adobe Dynamic Media Classic verfügt über standardmäßige einfache (schnelle), Flyout- und benutzerdefinierte Zoom-Viewer-Vorgaben. Administratoren können Viewer-Vorgaben für Unternehmen erstellen oder eine Standardvorgabe bearbeiten und sie mit einem neuen Namen speichern.

Alle Zoom-Viewer enthalten Schaltflächen zum Heranzoomen, Herauszoomen, Schwenken und Zurücksetzen des Bildes in seinen ursprünglichen Zustand vor dem Zoomen. Wie diese Schaltflächen aussehen und wie das Fenster selbst angezeigt wird, hängt von Ihrer Auswahl an Zoom-Viewer-Vorgaben ab. Sie können eine Zoom-Viewer-Vorgabe mit unterschiedlichen Farben, Rahmen, Schriftarten und Bildeinstellungen konfigurieren. Bei der Konfiguration eines Zoom-Viewers mit Geführtem Zoom können Sie auch festlegen, wo die Zoomziele platziert werden sollen. Zoomziele sind Miniaturansichten, auf die ein Benutzer klicken kann, um den von Ihnen zugeordneten Bildausschnitt heranzuzoomen.

## Zoom-Viewer-Vorgaben {#about-zoom-viewer-presets}

Adobe Dynamic Media Classic bietet die folgenden Zoom-Viewer-Vorgaben:

* **Zoom-Viewer: Einfach**: Stellt einen einfachen Zoom des Originalbilds bereit.

* **Zoom-Viewer: Fly-out**: Zeigt ein zweites Bild des vergrößerten Bereichs neben dem Originalbild an. Der Benutzer hat keine Steuerelemente zur Verfügung. Er bewegt einfach die Auswahl über den Bereich, der angezeigt werden soll.

Bedenken Sie bei der Festlegung der gesamten Bandbreitennutzung für diesen Viewer, dass sowohl das Hauptbild als auch das Flyout-Bild im Viewer geladen werden müssen. Die Größe des Flyout-Bildes wird anhand der Größe des Hauptbilds (Anzeigebreite und -höhe) und des Zoomfaktors bestimmt. Setzen Sie diese beiden Werte gut in Relation, damit das Flyout-Bild eine kompakte Dateigröße erhält. Wenn beispielsweise die Hauptbilddatei sehr groß ist, verringern Sie den Wert für den Zoomfaktor. (Die Flyout-Breite und Flyout-Höhe bestimmen die Größe des Flyout-Fensters, aber nicht die Größe des Flyout-Bildes, das in den Viewer geladen wird.)

Wenn die Größe des Hauptbildes beispielsweise 350 x 350 Pixel bei einem Zoomfaktor von 3 beträgt, ist das Flyout-Bild 1050 x 1050 Pixel groß. Wenn die Größe des Hauptbildes 300 x 300 Pixel bei einem Zoomfaktor von 4 beträgt, ist das Flyout-Bild 1200 x 1200 Pixel groß. Über die Einstellung für die JPEG-Qualität (empfohlener Wert: zwischen 80 und 90) können Sie die Dateigröße deutlich reduzieren. Der empfohlene Wert für den Zoomfaktor liegt, je nach Größe des Hauptbildes, zwischen 2,5 und 4.

Adobe Dynamic Media Classic empfiehlt die folgenden Parameter für Flyout-Zoom-Viewer-Vorgaben:

* **Vergrößerte Bildgröße**: Ungefähr 1500 x 1500 Pixel, höchstens 2000 x 2000 Pixel.

* **Bildgröße**: 100 KB oder weniger, höchstens 150 KB (komprimieren Sie die Datei, um sie unter 150 KB zu halten).

* **Zoom-Viewer: Benutzerdefiniert**: Bietet einen geführten oder nicht verwendeten Zoom mit Bildern, Bildsets mit mehreren Ansichten oder Farbmuster-Sets.

## Erstellen und Bearbeiten von Zoom-Viewer-Vorgaben {#creating-and-editing-zoom-viewer-presets}

1. Wechseln Sie in der Symbolleiste für globale Navigation zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Viewer-Vorgaben]**.
1. Führen Sie einen der folgenden Schritte aus:

   * **Vorgabe erstellen**: Auswählen **[!UICONTROL Hinzufügen]**. Wählen Sie im Dialogfeld &quot;Viewer-Vorgabe hinzufügen&quot;eine Plattform, einen Zoom-Viewer und klicken Sie auf **[!UICONTROL Hinzufügen]**. Geben Sie im Feld &quot;Vorgabenname&quot;einen Namen für die Vorgabe ein.

   * **Vorgabe bearbeiten**: Wählen Sie eine Zoom-Viewer-Vorgabe und dann **[!UICONTROL Bearbeiten]**.

1. Wählen Sie die gewünschten Einstellungen aus.

   Um eine Beschreibung einer Option anzuzeigen, wählen Sie die **[!UICONTROL Info-Tipp]** neben der Option.

   Auf der Seite Vorschau wird der Viewer angezeigt, wenn Sie Einstellungen aktualisieren und ändern.

1. Auswählen **[!UICONTROL Speichern]** oder **[!UICONTROL Speichern unter]**.
1. Überprüfen Sie auf der Seite &quot;Viewer-Vorgaben&quot;die von Ihnen erstellte Zoom-Viewer-Vorgabe oder Geführte Zoom-Viewer-Vorgabe. Wenn es angepasst werden muss, wählen Sie **[!UICONTROL Bearbeiten]**, ändern Sie die Einstellungen für `Configure Viewer` und wählen Sie **[!UICONTROL Speichern]**.

Informationen zum Verwalten von Viewer-Vorgaben im Anzeigebereich „Viewer-Vorgaben“ finden Sie unter [Viewer-Vorgaben](application-setup.md#viewer_presets).

>[!MORELIKETHIS]
>
>* [Erstellen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding_and_editing_viewer_presets)
