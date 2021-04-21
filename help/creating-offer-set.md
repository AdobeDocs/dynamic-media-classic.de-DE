---
title: Erstellen eines Angebotssets
description: Erfahren Sie, wie Sie ein Angebot-Set erstellen.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
translation-type: tm+mt
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '1223'
ht-degree: 51%

---

# Erstellen eines Angebotssets{#creating-an-offer-set}

Sie können die folgenden Angebotsset-Typen erstellen:

* Video
* Parametrisierte Vorlage
* Bild

Klicken Sie für Vorlagen auf **[!UICONTROL Hinzufügen und Vorschau]** und legen Sie dann die gewünschten Parameter fest. Die anderen Angebotsset-Typen enthalten keine Parameter, aber Sie können sie dennoch anpassen, indem Sie auf **[!UICONTROL Vorschau]** klicken und die verfügbaren Vorgaben ändern.

Dynamic Media Classic-Angebote zum Bearbeiten und Erstellen von Angebot-Sets.

>[!NOTE]
>
>Bevor Sie ein Angebot-Set erstellen, vergewissern Sie sich, dass Sie alle Assets veröffentlichen, die Sie für das Set mit Dynamic Media Classic verwenden möchten. Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

## Angebotsset-Typen {#types-of-offer-sets}

Erstellen Sie ein Angebotsset aus den folgenden Angebotsset-Typen:

* **Bilder** : Sie können Bilder für ein Angebot zusammenstellen. Jedes Bild enthält ein anderes Angebot im Set.

* **Bildvorlage** : Sie können Bildvorlagen in Dynamic Media Classic mit dem Befehl &quot;Erstellen&quot;> &quot;Vorlagen aus Grundelementen&quot;parametrisieren. Mithilfe von Parametern können Komponenten der Vorlage (Text in Textrahmen, die verschiedenen Bilder) ausgetauscht und angepasst werden. Für ein Angebotsset können Sie beispielsweise mithilfe von Vorlagenparametern verschiedene Varianten desselben Bildes erstellen. Weitere Informationen zum Erstellen und Parametrisieren von Bildvorlagen finden Sie unter Erstellen von Vorlagenparametern.

* **Video** : Sie können Videos für ein Videoset zusammenstellen. Jedes Video besteht dabei aus einem anderen Angebot im Set.

## Erstellen eines Angebot-Sets mit einer parametrisierten Vorlage {#creating-an-offer-set-with-a-parameterized-template}

Wenn Sie ein Angebotsset erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| Option „Nach dem Speichern veröffentlichen“ vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie einen Angebot-Satz mit einer parametrisierten Vorlage:**

1. Wählen Sie die Vorlage oder das Banner aus.
1. Klicken Sie auf **[!UICONTROL Erstellen]** > **[!UICONTROL Test&amp;Target-Angebotsset]**.

   Auf der Seite &quot;Test&amp;Zielgruppe-Angebot-Set&quot;werden die Angebot im Angebot-Set Liste. Das erste Element in der Liste ist das Objekt.

1. Wählen Sie das Objekt aus und klicken Sie auf **[!UICONTROL Hinzufügen und Vorschau]**.

   Links auf dieser Seite sind die Parameter in der Vorlage mit ihren Werten aufgelistet.

1. Ändern Sie die Parameterwerte, um das Angebot zu erstellen. Geben Sie beispielsweise anderen Text in ein Textfeld ein, ändern Sie die Größe einer Ebene, tauschen Sie ein Bild durch ein anderes aus oder wählen Sie eine andere Viewer-Vorgabe.
1. Klicken Sie auf **[!UICONTROL **Speichern]** oder **[!UICONTROL Speichern unter**]**, um das Angebot als Teil des Angebot-Sets zu speichern.

   Auf der Seite &quot;Test&amp;Zielgruppe-Angebot-Set&quot;werden die von Ihnen erstellten Angebot Liste.

1. Wiederholen Sie die Schritte 3 bis 5, um weitere Angebote für das Set zu erstellen.
1. Wenn Sie fertig sind, stellen Sie sicher, dass rechts unten auf der Seite **[!UICONTROL Nach dem Speichern veröffentlichen*]** ausgewählt ist (Standard).
1. Klicken Sie auf **[!UICONTROL Schließen]**, geben Sie einen Namen für den Angebot-Satz ein und klicken Sie dann auf **[!UICONTROL Speichern]**.

Bevor Sie die Seite &quot;Test&amp;Zielgruppe-Angebot-Set&quot;schließen, schieben Sie das Angebot auf Adobe Target Standard/Premium. Siehe [Weiterleiten von Angebotssets an Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Erstellen eines Angebot-Sets mit Bildern oder Videos {#creating-an-offer-set-with-images-or-videos}

Wenn Sie ein Angebotsset erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| **[!UICONTROL Nach]** Auswahl der Option &quot;Nach dem Speichern veröffentlichen&quot;vor dem Speichern veröffentlichen? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein Angebotsset mit Bildern oder Videos:**

1. Stellen Sie Bilder oder Videos für das Angebot-Set zusammen. Beginn im Bildschirm &quot;Test&amp;Zielgruppe-Angebot-Set&quot;oder in der Ansicht &quot;Raster-Ansicht&quot;oder &quot;Liste&quot;und verwenden Sie eine der folgenden Methoden:

   * **Bildschirm**  &quot;Test&amp;Zielgruppe-Angebot-Set&quot; **[!UICONTROL - Klicken Sie auf]** Erstellen **[!UICONTROL >]** Test&amp;Zielgruppe-Angebot-Set. Ziehen Sie die Bilder oder Videos in den Anzeigebereich. Wenn Sie verschiedene Video- oder Bildgrößen erstellen möchten, ziehen Sie mehrere Kopien des Bildes oder Videos in den Anzeigebereich und legen Sie jede Größe einzeln fest.

   * **Raster-Ansicht oder Liste-Ansicht** : Wählen Sie die Bilder oder Videos aus und klicken Sie dann auf  **[!UICONTROL Erstellen]** >  **[!UICONTROL Test&amp;Zielgruppe-Angebot-Set]**.

1. Optional können Sie ein Bild oder Video auswählen und auf **[!UICONTROL Vorschau]** klicken. Auf der Seite &quot;Vorschau Angebote&quot;können Sie die Größe und das Aussehen des ausgewählten Bildes oder Videos ändern. Sie können auch alle Angebote oder Videos im Videoset ändern.

   * Wählen Sie eine Vorlage aus, um Ansicht und Größe des Bildes oder Videos zu verändern.
   * Um die ausgewählte Vorgabe auf alle Angebot im Angebot-Set anzuwenden, klicken Sie auf das Kontrollkästchen **[!UICONTROL Vorgaben für alle auswählen]**.

   Klicken Sie auf **[!UICONTROL Speichern]**, um Ihre Änderungen am Bild- oder Videoangebot zu speichern. Klicken Sie anschließend auf **[!UICONTROL Schließen]**, um zur Seite „Test&amp;Target-Angebotsset“ zurückzukehren.

1. Nachdem Sie die Angebote für den Bildsatz erstellt und Bildvorgaben für verschiedene Angebote ausgewählt haben, stellen Sie sicher, dass **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Klicken Sie auf **[!UICONTROL Speichern]**, geben Sie einen Namen für das Angebotsset ein und klicken Sie auf **[!UICONTROL Speichern]**.

Bevor Sie die Seite &quot;Test&amp;Zielgruppe-Angebot-Set&quot;schließen, schieben Sie das Angebot auf Adobe Target Standard/Premium. Siehe [Weiterleiten von Angebotssets an Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Bearbeiten eines Angebotssets  {#editing-an-offer-set}

Unabhängig davon, ob Sie einen veröffentlichten oder unveröffentlichten Satz bearbeiten, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| Set bereits veröffentlicht? | **[!UICONTROL Nach]** Auswahl der Option &quot;Nach dem Speichern veröffentlichen&quot;veröffentlichen, bevor Sie Ihre Bearbeitung speichern? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |--- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten den Status „veröffentlicht“ bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie ein Angebotsset:**

1. Um einen Angebot-Satz zu bearbeiten, zeigen Sie den Angebot-Satz in der Ansicht &quot;Raster&quot;oder &quot;Liste&quot;an und klicken Sie dann auf die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]**.
1. Führen Sie auf der Seite &quot;Test&amp;Zielgruppe-Angebot-Set&quot;einen der folgenden Schritte aus:

   * **Entfernen eines Angebots** : Wählen Sie das Angebot aus und klicken Sie dann auf  **** Löschen, um ein Angebot aus dem Satz zu entfernen.
   * **Hinzufügen eines Angebots**  - Wie Sie ein Angebot hinzufügen, hängt davon ab, mit welchem Angebot Sie arbeiten:
      * **Vorlagen** : Klicken Sie auf  **[!UICONTROL Hinzufügen und Vorschau]** und erstellen Sie auf der Seite &quot;Angebote für Hinzufügen und Vorschau&quot;ein weiteres Angebot.
      * **Bilder und Videos** : Ziehen Sie ein Angebot oder Video auf die Seite &quot;Test&amp;Zielgruppe-Set&quot;.

   >[!NOTE]
   >
   >Angebotssets, die einer Kampagne zugeordnet sind, können nicht gelöscht werden. Um einen mit einer Kampagne verknüpften Angebot-Satz zu löschen, melden Sie sich bei Adobe Target Standard/Premium an und entfernen Sie zuerst die Kampagne-Verknüpfungen. Auch wenn die Verknüpfung zu einer Kampagne aufgehoben wurde, kann das Asset nur aus Dynamic Media Classic gelöscht werden, wozu eine Anmeldung bei Adobe Target Standard/Premium erforderlich ist, nicht jedoch aus Adobe Target Standard/Premium.

1. Wenn Sie die Bearbeitung abgeschlossen haben, stellen Sie sicher, dass rechts unten auf der Seite **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Klicken Sie auf **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **[!UICONTROL Speichern]**.

## Löschen eines Angebotssets  {#deleting-an-offer-set}

Wenn Sie ein Angebotsset löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (bzw. die untergeordneten Elemente) innerhalb des Sets sind davon jedoch nicht betroffen; sie behalten ihren jeweiligen Status „veröffentlicht“ oder „unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie ein Angebotsset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Angebotssets aus.
1. Klicken Sie in der globalen Navigationsleiste auf **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **Löschen**.

>[!MORELIKETHIS]
>
>* [Erstellen von Vorlagenparametern](creating-template-parameters.md#creating_template_parameters)

