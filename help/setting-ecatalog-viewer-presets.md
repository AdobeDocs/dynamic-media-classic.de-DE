---
title: Konfigurieren von E-Katalog-Viewer-Vorgaben
description: Erfahren Sie, wie Sie E-Katalog-Viewer-Vorgaben einrichten.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic, Viewer, Viewer-Vorgaben, E-Katalog
role: Business Practitioner
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
translation-type: tm+mt
source-git-commit: 6f3801a71dd2a5f162acacf7d8199dbf8c3520f7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 42%

---

# Konfigurieren von E-Katalog-Viewer-Vorgaben{#setting-up-ecatalog-viewer-presets}

Mit E-Katalog-Viewer-Vorgaben werden Stil, Verhalten und Aussehen von E-Katalog-Viewern bestimmt. Dynamic Media Classic stellt E-Katalog-Viewer-Vorgaben bereit. Als Administrator können Sie auch eigene E-Katalog-Viewer-Vorgaben erstellen.

Um eine Vorgabe zu erstellen, können Sie mit einer von Dynamic Media Classic bereitgestellten E-Katalog-Viewer-Vorgabe einen Beginn von Grund auf oder Beginn erstellen und unter einem neuen Namen speichern. Sie können eigene E-Katalog-Viewer-Vorgaben erstellen, um Druckwerbematerial in den Farben Ihres Unternehmens zu präsentieren.

E-Katalog-Viewer-Vorgaben bieten zahlreiche Einstellungen für das Umblättern der Seiten, für Zoomfunktionen, Suchfunktionen und die Auswahl von Skins. Wie diese Steuerelemente aussehen und wie der Viewer angezeigt wird, hängt von Ihrer Auswahl an E-Katalog-Viewer-Vorgaben ab.

Führen Sie die folgenden Schritte aus, um eine E-Katalog-Viewer-Vorgabe erstellen zu können (Sie müssen Administrator sein):

1. Klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Setup]** > **[!UICONTROL Viewer-Vorgaben]**.
1. Um im Anzeigebereich „Viewer-Vorgaben“ eine E-Katalog-Viewer-Vorgabe zu erstellen, können Sie ganz neu beginnen oder eine vorhandene E-Katalog-Viewer-Vorgabe als Vorlage verwenden:

   * **Erstellen einer E-Katalog-Viewer-Vorgabe**  - Klicken Sie auf  **[!UICONTROL Hinzufügen]**. Wählen Sie im Dialogfeld &quot;Hinzufügen-Viewer-Vorgabe&quot;eine Plattform, wählen Sie &quot;E-Katalog-Viewer&quot;und klicken Sie dann auf **[!UICONTROL Hinzufügen]**.

   * **Bearbeiten einer E-Katalog-Viewer-Vorgabe** : Wählen Sie eine E-Katalog-Viewer-Vorgabe aus und klicken Sie auf Bearbeiten. Klicken Sie auf **[!UICONTROL Speichern unter]**, nachdem Sie die Vorgabe erstellt haben.

1. Geben Sie im Anzeigebereich „Viewer konfigurieren“ einen Namen für die E-Katalog-Viewer-Vorgabe ein.
1. Legen Sie im Anzeigebereich „Viewer konfigurieren“ die Optionen fest.

   Klicken Sie auf das Symbol **[!UICONTROL Info Tip]** neben der Option, wenn Sie die Beschreibung lesen möchten.

   Auf der Seite &quot;Vorschau&quot;wird der Viewer angezeigt, während Sie die Einstellungen aktualisieren und ändern.

1. (Optional) In den **[!UICONTROL Infofeldeinstellungen]** kann die Option **[!UICONTROL URL des Infoservers]** die folgenden speziellen Token enthalten, die vom Viewer ersetzt werden:

   | Platzhalter | Ersetzt durch | Anmerkungen |
   |--- |--- |--- |
   | `$1$` | „rollover_key“-Wert | Die Element-ID aus dem Element `<area>` der Map. |
   | `$2$` | frame | Die Sequenznummer des momentan angezeigten Bildfelds im Bildsatz. |
   | `$3$` | imageroot | Das erste Pfadelement des ersten Elements, das im Bildbefehl angegeben wird (normalerweise die Katalog-ID des Katalogeintrags, der den Bildsatz bestimmt). |

1. (Optional) Geben Sie im Feld **[!UICONTROL Infofeldeinstellungen]** im Feld **[!UICONTROL Antwortvorlage]** den Text ein, der angezeigt werden soll, wenn Dynamic Media Classic beim Abrufen von Informationen für eine Imagemap auf einen Fehler stößt. Wenn das System beispielsweise einen Firmennamen und einen E-Katalog-Namen, jedoch keinen Rollover-Bezeichner empfängt, so wird dem Benutzer diese Meldung angezeigt.

>[!NOTE]
>
>Um diese Antwortvorlage anstelle der im E-Katalog selbst definierten Vorlage zu verwenden, fügen Sie am Ende der Infoserver-URL `fmt=1` hinzu. Beispiel: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Klicken Sie auf „**Speichern**“.
1. Wenn die soeben erstellte E-Katalog-Viewer-Vorgabe standardmäßig zum Anzeigen von E-Katalogen auf Ihrer Website verwendet werden soll, klicken Sie auf „Standard“.

Um eine E-Katalog-Viewer-Vorgabe zu löschen, wählen Sie sie im Anzeigebereich &quot;Viewer-Vorgaben&quot;aus und klicken Sie auf **[!UICONTROL Löschen]**.

>[!MORELIKETHIS]
>
>* [Viewer-Vorgaben](application-setup.md#viewer_presets)

