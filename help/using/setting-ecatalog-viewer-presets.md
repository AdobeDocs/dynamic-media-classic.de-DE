---
title: E-Katalog-Viewer-Vorgaben einrichten
description: Erfahren Sie, wie Sie eCatalog-Viewer-Vorgaben in Adobe Dynamic Media Classic einrichten.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
topic: Integrations, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 34%

---

# E-Katalog-Viewer-Vorgaben einrichten{#setting-up-ecatalog-viewer-presets}

Mit E-Katalog-Viewer-Vorgaben werden Stil, Verhalten und Aussehen von E-Katalog-Viewern bestimmt. Adobe Dynamic Media Classic stellt E-Katalog-Viewer-Vorgaben bereit. Wenn Sie Administrator sind, können Sie auch eigene E-Katalog-Viewer-Vorgaben erstellen.

Um eine Vorgabe zu erstellen, können Sie von Grund auf neu beginnen oder mit einer von Adobe Dynamic Media Classic bereitgestellten E-Katalog-Viewer-Vorgabe beginnen und sie unter einem neuen Namen speichern. Sie können eigene E-Katalog-Viewer-Vorgaben erstellen, um Druckwerbematerial in den Farben Ihres Unternehmens zu präsentieren.

E-Katalog-Viewer-Vorgaben bieten zahlreiche Einstellungen für das Umblättern der Seiten, für Zoomfunktionen, Suchfunktionen und die Auswahl von Skins. Wie diese Steuerelemente aussehen und wie der Viewer angezeigt wird, hängt von Ihrer Wahl der E-Katalog-Viewer-Vorgaben ab.

Führen Sie die folgenden Schritte aus, damit Sie eine E-Katalog-Viewer-Vorgabe erstellen können (Sie müssen Administrator sein):

1. Wechseln Sie in der Symbolleiste für globale Navigation zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Viewer-Vorgaben]**.
1. Um im Anzeigebereich „Viewer-Vorgaben“ eine E-Katalog-Viewer-Vorgabe zu erstellen, können Sie ganz neu beginnen oder eine vorhandene E-Katalog-Viewer-Vorgabe als Vorlage verwenden:

   * **Erstellen einer eCatalog-Viewer-Vorgabe** - Auswählen **[!UICONTROL Hinzufügen]**. Wählen Sie im Dialogfeld &quot;Viewer-Vorgabe hinzufügen&quot;eine Plattform, wählen Sie einen E-Katalog-Viewer und dann **[!UICONTROL Hinzufügen]**.

   * **Bearbeiten einer eCatalog-Viewer-Vorgabe** - Wählen Sie eine E-Katalog-Viewer-Vorgabe aus und wählen Sie **[!UICONTROL Bearbeiten]**. Auswählen **[!UICONTROL Speichern unter]** nach Abschluss der Erstellung der Vorgabe.

1. Geben Sie im Anzeigebereich „Viewer konfigurieren“ einen Namen für die E-Katalog-Viewer-Vorgabe ein.
1. Legen Sie im Anzeigebereich „Viewer konfigurieren“ die Optionen fest.

   wählen Sie die **[!UICONTROL Info-Tipp]** neben der Option, wenn Sie die Beschreibung lesen möchten.

   Auf der Seite Vorschau wird der Viewer angezeigt, wenn Sie Einstellungen aktualisieren und ändern.

1. (Optional) Im **[!UICONTROL Einstellungen des Infobereichs]**, die **[!UICONTROL URL des Informationsservers]** -Option können die folgenden speziellen Token enthalten, die der Viewer ersetzt:

   | Platzhalter | Ersetzt durch | Anmerkungen |
   | --- | --- | --- |
   | `$1$` | „rollover_key“-Wert | Die Element-ID aus der `<area>` -Element der Zuordnung. |
   | `$2$` | frame | Die Sequenznummer des momentan angezeigten Bildfelds im Bildsatz. |
   | `$3$` | Bildstamm | Das erste Pfadelement des ersten Elements, das im Bildbefehl angegeben wird (normalerweise die Katalog-ID des Katalogeintrags, der den Bildsatz bestimmt). |

1. (Optional) Im **[!UICONTROL Einstellungen des Infobereichs]** in der **[!UICONTROL Antwortvorlage]** Geben Sie den Text ein, der angezeigt werden soll, wenn Adobe Dynamic Media Classic beim Abrufen von Informationen für eine Imagemap auf einen Fehler stößt. Wenn das System beispielsweise einen Firmennamen und einen E-Katalog-Namen, jedoch keinen Rollover-Bezeichner empfängt, so wird dem Benutzer diese Meldung angezeigt.

>[!NOTE]
>
>Um diese Antwortvorlage anstelle der im eCatalog selbst definierten Vorlage zu verwenden, fügen Sie `fmt=1` an das Ende der URL des Informationsservers. Beispiel: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Auswählen **[!UICONTROL Speichern]**.
1. Auswählen **[!UICONTROL Standard]** Wenn Sie möchten, dass die von Ihnen erstellte E-Katalog-Viewer-Vorgabe die zum Anzeigen von E-Katalogen auf Ihrer Web-Seite verwendete ist.

Um eine E-Katalog-Viewer-Vorgabe zu löschen, wählen Sie sie im Bildschirm &quot;Viewer-Vorgaben&quot;aus und wählen Sie **[!UICONTROL Löschen]**.

>[!MORELIKETHIS]
>
>* [Viewer-Vorgaben](application-setup.md#viewer_presets)
