---
title: Einrichten einer Viewer-Vorgabe für gemischte Mediensets
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic eine Viewer-Vorgabe für gemischte Mediensets einrichten.
uuid: d5bf1840-e453-445d-bebc-84889b29f3c8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 8029aad8-d696-4d7c-99e2-3b08edb68181
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: d41b30e7-994a-43f3-8698-7dbfc36305ae
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 44%

---

# Einrichten einer Viewer-Vorgabe für gemischte Mediensets{#setting-up-a-mixed-media-set-viewer-preset}

Viewer-Vorgaben für gemischte Mediensets bestimmen den Stil, das Verhalten und das Aussehen Ihres Hauptviewers. Sie geben beim Konfigurieren einer Vorgabe an, welche anderen Viewer innerhalb eines gemischten Medienset-Viewers angezeigt werden sollen. Wenn Ihr gemischtes Medienset z. B. einen Bildsatz enthält, geben Sie für den gemischten Medienset-Viewer eine Viewer-Vorgabe für Bildsätze an.

Sie können alle oder bestimmte Community-Funktionen zum gemischten Medienset-Viewer hinzufügen. Die Funktion „Einbetten“ fügt eine Verknüpfung zum Viewer hinzu, über die Benutzer den Code für die Anzeige des Viewers auf einer externen Seite (wie z. B. einem Blog, einer Website oder einer Social-Networking-Site) kopieren können. Mit der Funktion „Verknüpfen“ wird dem Viewer die URL zur Verfügung gestellt, mit der Benutzer eine Verknüpfung zum Viewer erstellen können. Mit der Funktion „Zur Website“ können Sie eine Verknüpfung zu einer bestimmten Website einfügen.

1. Navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Setup]** > **[!UICONTROL Viewer-Vorgaben]**.
1. Führen Sie auf der Seite &quot;Viewer-Vorgaben&quot;einen der folgenden Schritte aus:

   * Um eine Vorgabe zu erstellen, wählen Sie **[!UICONTROL Hinzufügen]** aus. Wählen Sie im Dialogfeld &quot;Viewer-Vorgabe hinzufügen&quot;eine Plattform, wählen Sie **[!UICONTROL Viewer für gemischte Mediensets]** und dann **[!UICONTROL Hinzufügen]**.
   * Um eine Viewer-Vorgabe für gemischte Mediensets zu bearbeiten, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Bearbeiten]**.

1. Geben Sie auf der Seite &quot;Konfigurations-Viewer&quot;im Feld &quot;Vorgabenname&quot;einen Namen für die Viewer-Vorgabe für gemischte Mediensets ein.
1. Geben Sie **[!UICONTROL Registerkarten]** oder **[!UICONTROL Keine Registerkarten]** an. Über Registerkarten können Sie Elemente nach Typ, wie z. B. Videos, Mustersets oder Rotationsets trennen. Wenn Sie keine Registerkarten angeben, werden alle Elemente in einer Zeile unter dem Vorschaufenster angezeigt.
1. Geben Sie in das Feld **[!UICONTROL Name]** einen Namen für den Viewer ein, den Sie hinzufügen möchten.

   Wenn Sie beispielsweise ein Musterset zu Ihrem gemischten Medienset hinzufügen, geben Sie `Swatch Set A` ein.

1. Wählen Sie im Menü „Viewer“ den Asset-Typ aus, den Sie anzeigen möchten (z. B. „Mustersets“).
1. Wählen Sie im Menü „Vorgabe“ eine Vorgabe für den gewählten Asset-Typ aus.

   Wenn Sie beispielsweise ein Musterset hinzufügen, wählen Sie **[!UICONTROL SwatchSet1-Colors]**.

1. Wählen Sie **[!UICONTROL Hinzufügen]**.

   Die neue Viewer-Vorgabe wird in der Liste angezeigt.

1. Wiederholen Sie die Schritte 6–9 für alle Viewer-Vorgaben, die Sie hinzufügen möchten.
1. Gehen Sie wie folgt vor, um die Vorgabenliste zu bearbeiten:

   * Um eine Vorgabe aus der Liste zu löschen, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Löschen]**.
   * Um Vorgaben in der Liste neu anzuordnen, wählen Sie eine Vorgabe aus und wählen Sie den blauen Pfeil **[!UICONTROL Nach oben]** oder **[!UICONTROL Nach unten]** aus.

1. Um Community-Funktionen zum Viewer hinzuzufügen (Einbetten, Verknüpfen oder Zur Website), wählen Sie die Optionen für die folgenden Punkte aus:

   * **E-Mail**  - Wählen Sie  **** Ont aus, um eine E-Mail-Schaltfläche im Viewer zu aktivieren. Wenn Benutzer beim Anzeigen des Sets die Schaltfläche E-Mail auswählen, wird eine E-Mail mit dem Link zum Set geöffnet.

   * **Einbetten**  - Wählen Sie  **[!UICONTROL Live]** aus. Geben Sie im Feld „Beschriftung für Einbetten-Schaltfläche“ den Namen an, der im Viewer auf der Schaltfläche „Einbetten“ angezeigt werden soll. Wählen Sie bei Bedarf **[!UICONTROL Durchsuchen]** aus, um eine benutzerdefinierte Haut für die Schaltfläche zu suchen und auszuwählen.

   * **Link**  - Wählen Sie  **[!UICONTROL Live]** aus. Geben Sie im Feld Link Button Label den Namen ein, der im Viewer für die Schaltfläche Link angezeigt werden soll. Wählen Sie bei Bedarf **[!UICONTROL Durchsuchen]** aus, um eine benutzerdefinierte Haut für die Schaltfläche zu suchen und auszuwählen.

   * **Besuch**  - Wählen Sie  **[!UICONTROL Live]** aus. Geben Sie im Feld &quot;Beschriftung für Besuchsschaltflächen&quot;den Namen ein, der im Viewer für die Schaltfläche &quot;Besuch&quot;angezeigt werden soll. Geben Sie im Feld „URL besuchen“ die URL der Webseite an, die durch Klicken auf die Verknüpfung geöffnet werden soll.

1. Wählen Sie die weiteren gewünschten Optionen aus. Um eine Beschreibung einer Option anzuzeigen, wählen Sie das Symbol &quot;Info-Tipp&quot;neben der Option aus.

   Auf der Seite Vorschau wird der Viewer angezeigt, wenn Sie Einstellungen aktualisieren und ändern.

1. Wählen Sie **[!UICONTROL Save]** aus.

>[!MORELIKETHIS]
>
>* [Erstellen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding_and_editing_viewer_presets)

