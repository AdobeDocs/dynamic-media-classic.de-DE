---
title: Erstellen eines Angebotssets
seo-title: Erstellen eines Angebotssets
description: 'null'
seo-description: Erfahren Sie, wie Sie ein Angebotsset erstellen.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: Verweis
products: SG_EXPERIENCEMANAGER/Dynamic Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Erstellen eines Angebotssets{#creating-an-offer-set}

Sie können die folgenden Angebotsset-Typen erstellen:

* Video
* Parametrisierte Vorlage
* Bild

For templates, click **Add and Preview**, then set the parameters you choose. Die anderen Angebotsset-Typen enthalten keine Parameter, aber Sie können sie dennoch anpassen, indem Sie auf **Vorschau** klicken und die verfügbaren Vorgaben ändern.

Dynamic Media Classic bietet Werkzeuge zum Bearbeiten und Erstellen von Angebotssets.

>[!NOTE]
>
>Bevor Sie ein Angebotsset erstellen, müssen Sie alle Assets veröffentlichen, die Sie für das Set mit dem Scene7 Publishing System verwenden möchten. Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

## Angebotsset-Typen {#types-of-offer-sets}

Erstellen Sie ein Angebotsset aus den folgenden Angebotsset-Typen:

* **Bilder** Sie können Bilder für ein Angebotsset zusammenstellen. Jedes Bild enthält ein anderes Angebot im Set.

* **Bildvorlage** Sie können Bildvorlagen in Dynamic Media Classic mit dem Befehl "Erstellen"&gt; "Vorlagen aus Grundelementen"parametrisieren. Mithilfe von Parametern können Komponenten der Vorlage (Text in Textrahmen, die verschiedenen Bilder) ausgetauscht und angepasst werden. Für ein Angebotsset können Sie beispielsweise mithilfe von Vorlagenparametern verschiedene Varianten desselben Bildes erstellen. Weitere Informationen zum Erstellen und Parametrisieren von Bildvorlagen finden Sie unter Erstellen von Vorlagenparametern.

* **Video** Sie können Videos für ein Angebotsset zusammenstellen. Jedes Video besteht dabei aus einem anderen Angebot im Set.

## Erstellen eines Angebotssets mit einer parametrisierten Vorlage {#creating-an-offer-set-with-a-parameterized-template}

Wenn Sie ein Angebotsset erstellen, wirkt sich die Option **Nach dem Speichern veröffentlichen** wie folgt auf das Set und die Set-Mitglieder aus:

| Option „Nach dem Speichern veröffentlichen“ vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein Angebotsset mit einer parametrisierten Vorlage**

1. Wählen Sie die Vorlage oder das Banner aus.
1. Click **Build** &gt; **Target Classic Offer Set**.

   Auf der Seite "Angebotsset für Target Classic"werden die Angebote im Angebotsset aufgelistet. Das erste Element in der Liste ist das Objekt.

1. Wählen Sie das Objekt aus und klicken Sie auf **Hinzufügen und Vorschau**.

   Links auf dieser Seite sind die Parameter in der Vorlage mit ihren Werten aufgelistet.

1. Ändern Sie die Parameterwerte, um das Angebot zu erstellen. Geben Sie beispielsweise anderen Text in ein Textfeld ein, ändern Sie die Größe einer Ebene, tauschen Sie ein Bild durch ein anderes aus oder wählen Sie eine andere Viewer-Vorgabe.
1. Klicken Sie auf **Speichern** oder **Speichern unter**, um das Angebot als Teil des Angebotssets zu speichern.

   Auf der Seite "Angebotsset für Target Classic"werden die von Ihnen erstellten Angebote aufgelistet.

1. Wiederholen Sie die Schritte 3 bis 5, um weitere Angebote für das Set zu erstellen.
1. When you finish, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Close**, enter a name for the offer set, and then click **Save**.

Bevor Sie die Seite "Target Classic-Angebotsset"schließen, drücken Sie das Angebotsset auf Target Classic. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Creating an offer set with images or videos {#creating-an-offer-set-with-images-or-videos}

Wenn Sie ein Angebotsset erstellen, wirkt sich die Option **Nach dem Speichern veröffentlichen** wie folgt auf das Set und die Set-Mitglieder aus:

| Option „Nach dem Speichern veröffentlichen“ vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein Angebotsset mit Bildern oder Videos**

1. Stellen Sie Bilder oder Videos für das Angebotsset zusammen. Starten Sie im Anzeigebereich "Target Classic-Angebotsset"oder in der Raster- oder Listenansicht und verwenden Sie eine der folgenden Methoden:

   * **Wählen Sie im Bildschirm**"Target Classic-Angebotsset"Erstellen &gt; Target Classic-Angebotsset. Ziehen Sie die Bilder oder Videos in den Anzeigebereich. Wenn Sie verschiedene Video- oder Bildgrößen erstellen möchten, ziehen Sie mehrere Kopien des Bildes oder Videos in den Anzeigebereich und legen Sie jede Größe einzeln fest.

   * **Raster- oder Listenansicht** Wählen Sie die Bilder oder Videos aus und klicken Sie dann auf Erstellen &gt; Target Classic-Angebotsset.

1. Optional können Sie ein Bild oder Video auswählen und auf **Vorschau** klicken. Auf der Seite "Angebote in der Vorschau"können Sie Größe und Aussehen des ausgewählten Bildes oder Videos ändern. Sie können auch alle Bilder oder Videos im Angebotsset ändern.

   * Wählen Sie eine Vorlage aus, um Ansicht und Größe des Bildes oder Videos zu verändern.
   * Aktivieren Sie das Kontrollkästchen „Vorgaben für alle auswählen“, um die gewünschte Vorgabe auf alle Angebote im Angebotsset anzuwenden.
   Klicken Sie auf **Speichern**, um Ihre Änderungen am Bild- oder Videoangebot zu speichern. Then click **Close** to return to the Target Classic Offer Set page.

1. After you finish creating offers for the offer set and choosing Image Presets for different images, ensure that **Publish after save** is selected (default).
1. Klicken Sie auf **Speichern**, geben Sie einen Namen für das Angebotsset ein und klicken Sie auf **Speichern**.

Bevor Sie die Seite "Angebotsset"von Target Classic schließen, müssen Sie das Angebotsset auf Target Classic verschieben. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Bearbeiten eines Angebotssets {#editing-an-offer-set}

Je nachdem, ob Sie ein veröffentlichtes oder unveröffentlichtes Set bearbeiten, wirkt sich die Option **Nach dem Speichern veröffentlichen** wie folgt auf das Set und die Set-Mitglieder aus:

| Set bereits veröffentlicht? | Option „Nach dem Speichern veröffentlichen“ vor dem Speichern Ihrer Bearbeitungen ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |--- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren Status "veröffentlicht"bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status "veröffentlicht"oder "unveröffentlicht"bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie ein Angebotsset**

1. To edit an offer set, display the offer set in Grid view or List view, and then click its **Edit** rollover button.
1. Führen Sie auf der Seite "Target Classic-Angebotsset"einen der folgenden Schritte aus:

   * **Entfernen eines Angebots** Wählen Sie das Angebot aus und klicken Sie dann auf **Löschen** , um ein Angebot aus dem Set zu entfernen.
   * **Hinzufügen eines Angebots** Das Hinzufügen eines Angebots hängt davon ab, mit welchem Angebotsset Sie arbeiten:
   * **Vorlagen** Klicken Sie auf **Hinzufügen und Vorschau** und erstellen Sie auf der Seite Angebote hinzufügen und Vorschau anzeigen ein weiteres Angebot.
   * **Bilder und Videos** ziehen Sie ein Bild oder Video auf die Seite "Target Classic-Angebotsset".
   >[!NOTE]
   >
   >Angebotssets, die einer Kampagne zugeordnet sind, können nicht gelöscht werden. Um ein mit einer Kampagne verknüpftes Angebotsset zu löschen, melden Sie sich bei Target Classic an und entfernen Sie zunächst die Kampagnenzuordnungen. Selbst nach Aufhebung der Zuordnung zu einer Kampagne kann das Asset nur aus dem Scene7 Publishing System gelöscht werden, wobei eine Anmeldung bei Target Classic erforderlich ist, nicht aus Target Classic.

1. When you finish editing, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Klicken Sie auf **Speichern**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **Speichern**.

## Löschen eines Angebotssets {#deleting-an-offer-set}

Wenn Sie ein Angebotsset löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (bzw. die untergeordneten Elemente) innerhalb des Sets sind davon jedoch nicht betroffen; sie behalten ihren jeweiligen Status „veröffentlicht“ oder „unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie ein Angebotsset**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Angebotssets aus.
1. Klicken Sie in der globalen Navigationsleiste auf **Datei** &gt; **Löschen** &gt; **Löschen**.

>[!MORELIKETHIS]
>
>* [Erstellen von Vorlagenparametern](creating-template-parameters.md#creating_template_parameters)

