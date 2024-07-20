---
title: E-Katalog-Viewer-Vorgaben einrichten
description: Erfahren Sie, wie Sie eCatalog-Viewer-Vorgaben in Adobe Dynamic Media Classic einrichten.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
topic: Integrations, Development
level: Experienced
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 25%

---

# E-Katalog-Viewer-Vorgaben einrichten{#setting-up-ecatalog-viewer-presets}

Mit E-Katalog-Viewer-Vorgaben werden Stil, Verhalten und Aussehen von E-Katalog-Viewern bestimmt. Adobe Dynamic Media Classic stellt E-Katalog-Viewer-Vorgaben bereit. Wenn Sie Administrator sind, können Sie auch eigene E-Katalog-Viewer-Vorgaben erstellen.

Um eine Vorgabe zu erstellen, können Sie von Grund auf neu beginnen oder mit einer von Adobe Dynamic Media Classic bereitgestellten E-Katalog-Viewer-Vorgabe beginnen und sie unter einem neuen Namen speichern. Sie können eigene E-Katalog-Viewer-Vorgaben erstellen, um Druckwerbematerial in den Farben Ihres Unternehmens zu präsentieren.

eCatalog-Viewer-Vorgaben bieten viele Einstellungen zum Navigieren von Seite zu Seite, zum Zoomen, Suchen und Auswählen von &quot;Skins&quot;. Wie diese Steuerelemente aussehen und wie der Viewer angezeigt wird, hängt von Ihrer Wahl der E-Katalog-Viewer-Vorgaben ab.

Führen Sie die folgenden Schritte aus, damit Sie eine E-Katalog-Viewer-Vorgabe erstellen können (Sie müssen Administrator sein):

1. Wechseln Sie in der Leiste &quot;Globale Navigation&quot;zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Viewer-Vorgaben]**.
1. Um im Anzeigebereich „Viewer-Vorgaben“ eine E-Katalog-Viewer-Vorgabe zu erstellen, können Sie ganz neu beginnen oder eine vorhandene E-Katalog-Viewer-Vorgabe als Vorlage verwenden:

   * **Erstellen einer eCatalog-Viewer-Vorgabe**: Wählen Sie **[!UICONTROL Hinzufügen]** aus. Wählen Sie im Dialogfeld &quot;Viewer-Vorgabe hinzufügen&quot;eine Plattform, wählen Sie einen E-Katalog-Viewer und dann **[!UICONTROL Hinzufügen]**.

   * **Eine E-Katalog-Viewer-Vorgabe bearbeiten**: Wählen Sie eine E-Katalog-Viewer-Vorgabe aus und klicken Sie dann auf **[!UICONTROL Bearbeiten]**. Wählen Sie **[!UICONTROL Speichern unter]** aus, nachdem Sie die Vorgabe fertig erstellt haben.

1. Geben Sie auf der Seite &quot;`Configure Viewer`&quot;einen Namen für die E-Katalog-Viewer-Vorgabe ein.
1. Legen Sie auf der Seite `Configure Viewer` die gewünschten Optionen fest.

   Wählen Sie das Symbol **[!UICONTROL Info Tipp]** neben der Option aus, wenn Sie die Beschreibung lesen möchten.

   Auf der Seite Vorschau wird der Viewer angezeigt, wenn Sie Einstellungen aktualisieren und ändern.

1. (Optional) In den **[!UICONTROL Einstellungen des Infobereichs]** kann die Option **[!UICONTROL URL des Informationsservers]** die folgenden speziellen Token enthalten, die der Viewer ersetzt:

   | Platzhalter | Ersetzt durch | Anmerkungen |
   | --- | --- | --- |
   | `$1$` | „rollover_key“-Wert | Die Element-ID aus dem Element `<area>` der Zuordnung. |
   | `$2$` | frame | Die Sequenznummer des momentan angezeigten Bildfelds im Bildsatz. |
   | `$3$` | Bildstamm | Das erste Pfadelement des ersten Elements, das im Bildbefehl angegeben wird (normalerweise die Katalog-ID des Katalogeintrags, der den Bildsatz bestimmt). |

1. (Optional) Geben Sie in das Feld **[!UICONTROL Einstellungen des Infobereichs]** im Feld **[!UICONTROL Antwortvorlage]** den Text ein, der angezeigt werden soll, wenn bei Adobe Dynamic Media Classic beim Abrufen von Informationen für eine Imagemap ein Fehler auftritt. Wenn das System beispielsweise einen Firmennamen und einen E-Katalog-Namen, jedoch keinen Rollover-Bezeichner empfängt, so wird dem Benutzer diese Meldung angezeigt.

>[!NOTE]
>
>Um diese Antwortvorlage anstelle der im eCatalog selbst definierten Vorlage zu verwenden, fügen Sie am Ende der URL des Informationsservers `fmt=1` hinzu. Beispiel: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Wählen Sie **[!UICONTROL Speichern]** aus.
1. Wählen Sie **[!UICONTROL Standard]** aus, damit die von Ihnen erstellte E-Katalog-Viewer-Vorgabe die zum Anzeigen von E-Katalogen auf Ihrer Webseite verwendete ist.

Um eine E-Katalog-Viewer-Vorgabe zu löschen, wählen Sie sie im Bildschirm &quot;Viewer-Vorgaben&quot;aus und wählen Sie **[!UICONTROL Löschen]** aus.

>[!MORELIKETHIS]
>
>* [Viewer-Vorgaben](application-setup.md#viewer_presets)
