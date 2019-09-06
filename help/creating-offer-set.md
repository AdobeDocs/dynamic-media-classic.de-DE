---
title: Erstellen eines Angebotssets
seo-title: Erstellen eines Angebotssets
description: 'null'
seo-description: Erfahren Sie, wie Sie ein Angebotsset erstellen.
uuid: 6 d 6 a 4 af 9-70 c 0-4 cfa -9 a 8 f -855 d 6 adfcc 8 f
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/target_ classic_ integration
discoiquuid: 59 b 6437 d-c 21 e -4929-9291-3032 dbb 44565
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Erstellen eines Angebotssets{#creating-an-offer-set}

Sie können die folgenden Angebotsset-Typen erstellen:

* Video
* Parametrisierte Vorlage
* Bild

For templates, click **Add and Preview**, then set the parameters you choose. Die anderen Angebotsset-Typen enthalten keine Parameter, aber Sie können sie dennoch anpassen, indem Sie auf **Vorschau** klicken und die verfügbaren Vorgaben ändern.

Dynamic Media Classic bietet Werkzeuge zur Bearbeitung und Erstellung von Angebotssets.

>[!NOTE]
>
>Bevor Sie ein Angebotsset erstellen, stellen Sie sicher, dass Sie alle Assets veröffentlichen, die Sie für das Set auf das Scene 7 Publishing System verwenden möchten. Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

## Angebotsset-Typen {#types-of-offer-sets}

Erstellen Sie ein Angebotsset aus den folgenden Angebotsset-Typen:

**Bilder** Sie können Bilder für ein Angebotsset zusammenstellen. Jedes Bild enthält ein anderes Angebot im Set.

**Bildvorlage** Sie können Bildvorlagen in Dynamic Media Classic mit dem Befehl Erstellen &gt; Vorlagen aus Grundelementen parametrisieren. Mithilfe von Parametern können Komponenten der Vorlage (Text in Textrahmen, die verschiedenen Bilder) ausgetauscht und angepasst werden. Für ein Angebotsset können Sie beispielsweise mithilfe von Vorlagenparametern verschiedene Varianten desselben Bildes erstellen. Weitere Informationen zum Erstellen und Parametrisieren von Bildvorlagen finden Sie unter Erstellen von Vorlagenparametern.

**Video** Sie können Video für ein Angebotsset zusammenstellen. Jedes Video besteht dabei aus einem anderen Angebot im Set.

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

   Auf der Seite Angebotsset von Target Classic werden Angebote im Angebotsset aufgelistet. Das erste Element in der Liste ist das Objekt.

1. Wählen Sie das Objekt aus und klicken Sie auf **Hinzufügen und Vorschau**.

   Links auf dieser Seite sind die Parameter in der Vorlage mit ihren Werten aufgelistet.

1. Ändern Sie die Parameterwerte, um das Angebot zu erstellen. Geben Sie beispielsweise anderen Text in ein Textfeld ein, ändern Sie die Größe einer Ebene, tauschen Sie ein Bild durch ein anderes aus oder wählen Sie eine andere Viewer-Vorgabe.
1. Klicken Sie auf **Speichern** oder **Speichern unter**, um das Angebot als Teil des Angebotssets zu speichern.

   Auf der Seite "Angebotsset von Target Classic" werden die von Ihnen erstellten Angebote aufgelistet.

1. Wiederholen Sie die Schritte 3 bis 5, um weitere Angebote für das Set zu erstellen.
1. When you finish, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Close**, enter a name for the offer set, and then click **Save**.

Bevor Sie die Seite "Angebotsset von Target Classic" schließen, leiten Sie das Angebotsset an Target Classic weiter. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Creating an offer set with images or videos {#creating-an-offer-set-with-images-or-videos}

Wenn Sie ein Angebotsset erstellen, wirkt sich die Option **Nach dem Speichern veröffentlichen** wie folgt auf das Set und die Set-Mitglieder aus:

| Option „Nach dem Speichern veröffentlichen“ vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein Angebotsset mit Bildern oder Videos**

1. Stellen Sie Bilder oder Videos für das Angebotsset zusammen. Starten Sie im Anzeigebereich "Angebotsset von Target Classic" oder in der Raster- oder Listenansicht eine der folgenden Methoden:

   **Angebotsset für Target Classic Klicken Sie** auf Erstellen &gt; Angebotsset für Target Classic. Ziehen Sie die Bilder oder Videos in den Anzeigebereich. Wenn Sie verschiedene Video- oder Bildgrößen erstellen möchten, ziehen Sie mehrere Kopien des Bildes oder Videos in den Anzeigebereich und legen Sie jede Größe einzeln fest.

   **Raster- oder Listenansicht** Wählen Sie die Bilder oder Videos aus und klicken Sie dann auf "Erstellen" &gt;" Target Classic-Angebotsset" .

1. Optional können Sie ein Bild oder Video auswählen und auf **Vorschau** klicken. Auf der Seite "Angebotsvorschau" können Sie die Größe und das Aussehen des ausgewählten Bildes oder Videos ändern. Sie können auch alle Bilder oder Videos im Angebotsset ändern.

   * Wählen Sie eine Vorlage aus, um Ansicht und Größe des Bildes oder Videos zu verändern.
   * Aktivieren Sie das Kontrollkästchen „Vorgaben für alle auswählen“, um die gewünschte Vorgabe auf alle Angebote im Angebotsset anzuwenden.
   Klicken Sie auf **Speichern**, um Ihre Änderungen am Bild- oder Videoangebot zu speichern. Then click **Close** to return to the Target Classic Offer Set page.

1. After you finish creating offers for the offer set and choosing Image Presets for different images, ensure that **Publish after save** is selected (default).
1. Klicken Sie auf **Speichern**, geben Sie einen Namen für das Angebotsset ein und klicken Sie auf **Speichern**.

Bevor Sie die Angebotsset-Seite von Target Classic schließen, leiten Sie das Angebotsset an Target Classic weiter. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Bearbeiten eines Angebotssets {#editing-an-offer-set}

Je nachdem, ob Sie ein veröffentlichtes oder unveröffentlichtes Set bearbeiten, wirkt sich die Option **Nach dem Speichern veröffentlichen** wie folgt auf das Set und die Set-Mitglieder aus:

| Set bereits veröffentlicht? | Option „Nach dem Speichern veröffentlichen“ vor dem Speichern Ihrer Bearbeitungen ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |--- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren veröffentlichten Status bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten den Status "Veröffentlicht" oder" Unveröffentlicht" bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie ein Angebotsset**

1. To edit an offer set, display the offer set in Grid view or List view, and then click its **Edit** rollover button.
1. Führen Sie auf der Seite "Angebotsset von Target Classic" einen der folgenden Schritte aus:

   **Entfernen eines Angebots**

   Select the offer, and then click **Delete** to remove an offer from the set.

   **Hinzufügen eines Angebots**

   Wie Sie ein Angebot hinzufügen, hängt vom Typ des Angebotssets ab, mit dem Sie arbeiten:

   * Templates: Click **Add &amp; Preview**, and on the Add &amp; Preview Offers page, create another offer.
   * Bilder und Videos: Ziehen Sie ein Bild oder Video auf die Angebotsset-Seite von Target Classic.
   ***Hinweis**: Sie können ein Angebotsset, das einer Kampagne zugeordnet ist, nicht löschen. Um ein mit einer Kampagne verknüpftes Angebotsset zu löschen, melden Sie sich bei Target Classic an und entfernen Sie zuerst die Kampagnenzuordnungen. Even after un-associating from a campaign, the asset can only be deleted from Scene7 Publishing System, requiring a login to Target Classic, and not from within Target Classic.*

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

