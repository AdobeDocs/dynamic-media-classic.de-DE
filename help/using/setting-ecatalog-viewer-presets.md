---
title: Viewer-Vorgaben für E-Katalog einrichten
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic Viewer-Vorgaben für E-Kataloge einrichten.
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

# Viewer-Vorgaben für E-Katalog einrichten{#setting-up-ecatalog-viewer-presets}

Mit E-Katalog-Viewer-Vorgaben werden Stil, Verhalten und Aussehen von E-Katalog-Viewern bestimmt. Adobe Dynamic Media Classic bietet E-Katalog-Viewer-Vorgaben. Sie können auch eigene E-Katalog-Viewer-Vorgaben erstellen, wenn Sie Administrator sind.

Um eine Vorgabe zu erstellen, können Sie von Grund auf neu beginnen oder mit einer von Adobe Dynamic Media Classic bereitgestellten E-Katalog-Viewer-Vorgabe beginnen und sie unter einem neuen Namen speichern. Sie können eigene E-Katalog-Viewer-Vorgaben erstellen, um Druckwerbematerial in den Farben Ihres Unternehmens zu präsentieren.

E-Katalog-Viewer-Vorgaben bieten viele Einstellungen zum Wechseln von Seite zu Seite, Zoomen, Suchen und Auswählen von „Skins“. Wie diese Steuerelemente aussehen und wie der Viewer angezeigt wird, hängt von der Auswahl der E-Katalog-Viewer-Vorgaben ab.

Führen Sie die folgenden Schritte aus, um eine E-Katalog-Viewer-Vorgabe zu erstellen (Sie müssen Administrator sein):

1. Wechseln Sie in der globalen Navigationsleiste zu **[!UICONTROL Einstellungen]** > **[!UICONTROL Viewer-Vorgaben]**.
1. Um im Anzeigebereich „Viewer-Vorgaben“ eine E-Katalog-Viewer-Vorgabe zu erstellen, können Sie ganz neu beginnen oder eine vorhandene E-Katalog-Viewer-Vorgabe als Vorlage verwenden:

   * **Erstellen einer E-Katalog-Viewer** Vorgabe: Wählen Sie **[!UICONTROL Hinzufügen]**. Wählen Sie im Dialogfeld „Viewer-Vorgabe hinzufügen“ eine Plattform und anschließend „eCatalog-Viewer“ und anschließend **[!UICONTROL Hinzufügen]**.

   * **Bearbeiten einer E-Katalog-Viewer** Vorgabe: Wählen Sie eine E-Katalog-Viewer-Vorgabe aus und klicken Sie dann auf **[!UICONTROL Bearbeiten]**. Wählen **[!UICONTROL Speichern unter]** nachdem Sie die Voreinstellung fertig erstellt haben.

1. Geben Sie auf der Seite `Configure Viewer` einen Namen für Ihre E-Katalog-Viewer-Vorgabe ein.
1. Legen Sie auf der Seite `Configure Viewer` die gewünschten Optionen fest.

   Klicken Sie auf **[!UICONTROL Info-]**) neben der Option, um die Beschreibung zu lesen.

   Auf der Seite Vorschau wird der Viewer angezeigt, während Sie die Einstellungen aktualisieren und ändern.

1. (Optional) In den **[!UICONTROL Einstellungen des Bedienfelds]** kann die Option **[!UICONTROL Informationsserver-URL]** die folgenden speziellen Token enthalten, die der Viewer ersetzt:

   | Platzhalter | Ersetzt durch | Anmerkungen |
   | --- | --- | --- |
   | `$1$` | „rollover_key“-Wert | Die Elementkennung aus dem `<area>` der Zuordnung. |
   | `$2$` | frame | Die Sequenznummer des momentan angezeigten Bildfelds im Bildsatz. |
   | `$3$` | Bildstamm | Das erste Pfadelement des ersten Elements, das im Bildbefehl angegeben wird (normalerweise die Katalog-ID des Katalogeintrags, der den Bildsatz bestimmt). |

1. (Optional) Geben Sie in **[!UICONTROL Einstellungen des Bedienfelds]** in das Feld **[!UICONTROL Antwortvorlage]** den Text ein, der angezeigt werden soll, wenn in Adobe Dynamic Media Classic beim Abrufen von Informationen für eine Imagemap ein Fehler auftritt. Wenn das System beispielsweise einen Firmennamen und einen E-Katalog-Namen, jedoch keinen Rollover-Bezeichner empfängt, so wird dem Benutzer diese Meldung angezeigt.

>[!NOTE]
>
>Um diese Antwortvorlage anstelle der im E-Katalog selbst definierten Vorlage zu verwenden, fügen Sie am Ende der Informationsserver-URL `fmt=1` hinzu. Beispiel: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Wählen Sie **[!UICONTROL Speichern]** aus.
1. Wählen Sie **[!UICONTROL Standard]** aus, damit die von Ihnen erstellte Viewer-Vorgabe für E-Kataloge diejenige ist, die zum Anzeigen von E-Katalogen auf Ihrer Web-Seite verwendet wird.

Um eine E-Katalog-Viewer-Vorgabe zu löschen, wählen Sie sie auf dem Bildschirm „Viewer-Vorgaben“ aus und klicken Sie auf **[!UICONTROL Löschen]**.

>[!MORELIKETHIS]
>
>* [Viewer-Vorgaben](application-setup.md#viewer_presets)
