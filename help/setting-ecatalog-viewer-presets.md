---
title: Konfigurieren von E-Katalog-Viewer-Vorgaben
description: Erfahren Sie, wie Sie E-Katalog-Viewer-Vorgaben einrichten.
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 66%

---


# Konfigurieren von E-Katalog-Viewer-Vorgaben{#setting-up-ecatalog-viewer-presets}

Mit E-Katalog-Viewer-Vorgaben werden Stil, Verhalten und Aussehen von E-Katalog-Viewern bestimmt. Dynamic Media Classic stellt E-Katalog-Viewer-Vorgaben bereit. Als Administrator können Sie auch eigene E-Katalog-Viewer-Vorgaben erstellen.

Um eine neue Vorgabe zu erstellen, können Sie mit einer von Dynamic Media Classic bereitgestellten E-Katalog-Viewer-Vorgabe einen Beginn von Grund auf oder Beginn erstellen und unter einem neuen Namen speichern. Sie können eigene E-Katalog-Viewer-Vorgaben erstellen, um Druckwerbematerial in den Farben Ihres Unternehmens zu präsentieren.

E-Katalog-Viewer-Vorgaben bieten zahlreiche Einstellungen für das Umblättern der Seiten, für Zoomfunktionen, Suchfunktionen und die Auswahl von Skins. Das Aussehen dieser Steuerelemente und des Viewers an sich hängt von den ausgewählten E-Katalog-Viewer-Vorgaben ab.

Führen Sie folgende Schritte aus, um eine E-Katalog-Viewer-Vorgabe zu erstellen (nur Administratoren):

1. Klicken Sie auf **Einstellungen** > **Viewer-Vorgaben**.
1. Um im Anzeigebereich „Viewer-Vorgaben“ eine E-Katalog-Viewer-Vorgabe zu erstellen, können Sie ganz neu beginnen oder eine vorhandene E-Katalog-Viewer-Vorgabe als Vorlage verwenden:

   * **Erstellen einer E-Katalog-Viewer-**
VorgabeKlicken Sie auf Hinzufügen. Wählen Sie im Dialogfeld &quot;Hinzufügen-Viewer-Vorgabe&quot;eine Plattform, wählen Sie &quot;E-Katalog-Viewer&quot;und klicken Sie dann auf 
**Hinzufügen**.

   * **Bearbeiten einer E-Katalog-Viewer-**
VorgabeWählen Sie eine E-Katalog-Viewer-Vorgabe und klicken Sie dann auf Bearbeiten. Klicken 
**Speichern Sie** Asbest, nachdem Sie die Vorgabe erstellt haben.

1. Geben Sie im Anzeigebereich „Viewer konfigurieren“ einen Namen für die E-Katalog-Viewer-Vorgabe ein.
1. Legen Sie im Anzeigebereich „Viewer konfigurieren“ die Optionen fest.

   Klicken Sie auf das Informationssymbol  neben der Option, um dessen Beschreibung anzuzeigen.

   Im Anzeigebereich „Vorschau“ werden jeweils die Auswirkungen der vorgenommenen Änderungen angezeigt.

1. (Optional) Unter „Infofeldeinstellungen“ kann die Option „URL des Infoservers“ folgende spezielle Platzhalter umfassen, die vom Viewer ersetzt werden:

   | Platzhalter | Ersetzt durch | Anmerkungen |
   |--- |--- |--- |
   | `$1$` | „rollover_key“-Wert | Die Element-ID aus dem Element `<area>` der Map. |
   | `$2$` | frame | Die Sequenznummer des momentan angezeigten Bildfelds im Bildsatz. |
   | `$3$` | imageroot | Das erste Pfadelement des ersten Elements, das im Bildbefehl angegeben wird (normalerweise die Katalog-ID des Katalogeintrags, der den Bildsatz bestimmt). |

1. (Optional) Geben Sie in den Infofeldeinstellungen im Feld &quot;Antwortvorlage&quot;den Text ein, der angezeigt werden soll, wenn Dynamic Media Classic beim Abrufen von Informationen für eine Imagemap auf einen Fehler stößt. Wenn das System beispielsweise einen Firmennamen und einen E-Katalog-Namen, jedoch keinen Rollover-Bezeichner empfängt, so wird dem Benutzer diese Meldung angezeigt.

>[!NOTE]
>
>Um anstelle der im E-Katalog definierten Vorlage diese Antwortvorlage zu verwenden, fügen Sie am Ende der Infoserver-URL die Zeichenfolge „fmt=1“ ein. Beispiel: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Klicken Sie auf „**Speichern**“.
1. Wenn die soeben erstellte E-Katalog-Viewer-Vorgabe standardmäßig zum Anzeigen von E-Katalogen auf Ihrer Website verwendet werden soll, klicken Sie auf „Standard“.

Um eine E-Katalog-Viewer-Vorgabe zu löschen, wählen Sie sie im Anzeigebereich &quot;Viewer-Vorgaben&quot;aus und klicken Sie auf **Löschen**.

>[!MORELIKETHIS]
>
>* [Viewer-Vorgaben](application-setup.md#viewer_presets)

