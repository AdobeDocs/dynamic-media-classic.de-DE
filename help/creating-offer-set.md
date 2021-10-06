---
title: Angebotssatz erstellen
description: Erfahren Sie, wie Sie ein Angebotsset in Adobe Dynamic Media Classic erstellen.
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
source-git-commit: 53551f938946bb78074127c05f984ae97e9ccca1
workflow-type: tm+mt
source-wordcount: '1293'
ht-degree: 35%

---

# Angebotssatz erstellen {#creating-an-offer-set}

Sie können die folgenden Angebotsset-Typen erstellen:

* Video
* Parametrisierte Vorlage
* Bild

Wählen Sie für Vorlagen **[!UICONTROL Hinzufügen und Vorschau]** und legen Sie dann die von Ihnen gewählten Parameter fest. Die anderen Angebotssatztypen enthalten keine Parameter. Sie können sie jedoch dennoch anpassen, indem Sie **[!UICONTROL Vorschau]** auswählen und die verfügbaren Vorgaben ändern.

Adobe Dynamic Media Classic bietet Tools zum Bearbeiten und Erstellen von Angebotssets.

>[!NOTE]
>
>Bevor Sie ein Angebotsset erstellen, stellen Sie sicher, dass Sie alle Assets veröffentlichen, die Sie für das Set verwenden möchten, und zwar in Adobe Dynamic Media Classic. Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

## Angebotsset-Typen {#types-of-offer-sets}

Erstellen Sie ein Angebotsset aus den folgenden Angebotsset-Typen:

* **Bilder**  - Sie können Bilder für ein Angebotsset zusammenstellen. Jedes Bild enthält ein anderes Angebot im Set.

* **Bildvorlage**  - Sie können Bildvorlagen in Adobe Dynamic Media Classic mit dem Befehl  **[!UICONTROL Erstellen]**  > Vorlagengrundlagen parametrisieren. Mithilfe von Parametern können Komponenten der Vorlage (Text in Textrahmen, die verschiedenen Bilder) ausgetauscht und angepasst werden. Für ein Angebotsset können Sie beispielsweise mithilfe von Vorlagenparametern verschiedene Varianten desselben Bildes erstellen. Informationen zum Erstellen und Parametrisieren von Bildvorlagen finden Sie unter [Vorlagenparameter erstellen](creating-template-parameters.md#creating_template_parameters).

Siehe auch Schulungsvideo zu [Vorlagengrundlagen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) .

* **Video**  - Sie können Videos für ein Angebotsset zusammenstellen. Jedes Video besteht dabei aus einem anderen Angebot im Set.

## Angebotssatz mit parametrierter Vorlage erstellen {#creating-an-offer-set-with-a-parameterized-template}

Wenn Sie ein Angebotsset erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| **[!UICONTROL Nach der]** Speicheroption Veröffentlichen vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein Angebotsset mit einer parametrisierten Vorlage:**

1. Wählen Sie die Vorlage oder das Banner aus.
1. Gehen Sie zu **[!UICONTROL Build]** > **[!UICONTROL Test&amp;Target-Angebotsset]**.

   Auf der Seite &quot;Test&amp;Target-Angebotsset&quot;werden die Angebote im Angebotsset aufgelistet. Das erste Element in der Liste ist das Objekt.

1. Wählen Sie das Objekt aus und wählen Sie **[!UICONTROL Hinzufügen und Vorschau]** aus.

   Links auf dieser Seite sind die Parameter in der Vorlage mit ihren Werten aufgelistet.

1. Ändern Sie die Parameterwerte, um das Angebot zu erstellen. Geben Sie beispielsweise anderen Text in ein Textfeld ein, ändern Sie die Größe einer Ebene, tauschen Sie ein Bild durch ein anderes aus oder wählen Sie eine andere Viewer-Vorgabe.
1. Wählen Sie **[!UICONTROL Speichern]** oder **[!UICONTROL Speichern unter**]** aus, um das Angebot als Teil des Angebotssatzes zu speichern.

   Auf der Seite &quot;Test&amp;Target-Angebotsset&quot;werden die von Ihnen erstellten Angebote aufgelistet.

1. Wiederholen Sie die Schritte 3 bis 5, um weitere Angebote für das Set zu erstellen.
1. Wenn Sie fertig sind, stellen Sie in der Nähe der rechten unteren Ecke der Seite sicher, dass **[!UICONTROL Nach dem Speichern veröffentlichen*]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Close]**, geben Sie einen Namen für das Angebotsset ein und wählen Sie **[!UICONTROL Save]**.

Bevor Sie die Seite &quot;Test&amp;Target-Angebotsset&quot;schließen, pushen Sie das Angebotsset auf Adobe Target Standard/Premium. Siehe [Angebotssets an Test&amp;Target pushen](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Angebotssatz mit Bildern oder Videos erstellen {#creating-an-offer-set-with-images-or-videos}

Wenn Sie ein Angebotsset erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| **[!UICONTROL Nach der]** Speicheroption Veröffentlichen vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein Angebotsset mit Bildern oder Videos:**

1. Stellen Sie Bilder oder Videos für das Angebotsset zusammen. Starten Sie im Bildschirm &quot;Test&amp;Target-Angebotsset&quot;oder in der Raster- oder Listenansicht und verwenden Sie eine der folgenden Methoden:

   * **Bildschirm**  &quot;Test&amp;Target-Angebotsset&quot;- Wechseln Sie zu  **[!UICONTROL Erstellen]**  >  **[!UICONTROL Test&amp;Target-Angebotsset]**. Ziehen Sie die Bilder oder Videos in den Anzeigebereich. Wenn Sie verschiedene Video- oder Bildgrößen erstellen möchten, ziehen Sie mehrere Kopien des Bildes oder Videos in den Anzeigebereich und legen Sie jede Größe einzeln fest.

   * **Rasteransicht oder Listenansicht**  - Wählen Sie die Bilder oder Videos aus und gehen Sie dann zu  **[!UICONTROL Erstellen]**  >  **[!UICONTROL Test&amp;Target-Angebotsset]**.

1. Wählen Sie optional ein Bild oder Video aus und klicken Sie auf **[!UICONTROL Vorschau]**. Auf der Seite &quot;Angebote in der Vorschau&quot;können Sie die Größe und das Aussehen des ausgewählten Bildes oder Videos ändern. Sie können auch alle Bilder oder Videos im Angebotsset ändern.

   * Wählen Sie eine Vorlage aus, um Ansicht und Größe des Bildes oder Videos zu verändern.
   * Um die ausgewählte Vorgabe auf alle Angebote im Angebotsset anzuwenden, aktivieren Sie das Kontrollkästchen **[!UICONTROL Alle Vorgaben auswählen]**.

   Wählen Sie **[!UICONTROL Speichern]** aus, um Ihre Änderungen am Bild- oder Videoangebot zu speichern. Wählen Sie dann **[!UICONTROL Close]** aus, um zur Seite Test&amp;Target-Angebotsset zurückzukehren.

1. Nachdem Sie die Erstellung der Angebote für das Angebotsset abgeschlossen und Bildvorgaben für verschiedene Bilder ausgewählt haben, stellen Sie sicher, dass **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Save]** aus, geben Sie einen Namen für das Angebotsset ein und wählen Sie **[!UICONTROL Save]**.

Bevor Sie die Seite &quot;Test&amp;Target-Angebotsset&quot;schließen, pushen Sie das Angebotsset auf Adobe Target Standard/Premium. Siehe [Angebotssets an Test&amp;Target pushen](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Bearbeiten eines Angebotssatzes {#editing-an-offer-set}

Unabhängig davon, ob Sie einen veröffentlichten oder einen nicht veröffentlichten Satz bearbeiten, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf den Satz und die Setmitglieder aus:

| Set bereits veröffentlicht? | **[!UICONTROL Nach der]** Speicheroption veröffentlichen vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten den Status „veröffentlicht“ bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie ein Angebotsset:**

1. Um ein Angebotsset zu bearbeiten, zeigen Sie das Angebotsset in der Raster- oder Listenansicht an und wählen Sie dann die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** aus.
1. Führen Sie auf der Seite &quot;Test&amp;Target-Angebotsset&quot;einen der folgenden Schritte aus:

   * **Entfernen eines Angebots**  - Wählen Sie das Angebot aus und klicken Sie auf  **** Löschen , um ein Angebot aus dem Satz zu entfernen.
   * **Hinzufügen eines Angebots**  - Wie Sie ein Angebot hinzufügen, hängt vom Typ des Angebots ab, mit dem Sie arbeiten:
      * **Vorlagen**  - Wählen Sie  **[!UICONTROL Hinzufügen und Vorschau]** aus und erstellen Sie auf der Seite Hinzufügen und Vorschau von Angeboten ein weiteres Angebot.
      * **Bilder und Videos**  - Ziehen Sie ein Bild oder Video auf die Seite &quot;Test&amp;Target-Angebotsset&quot;.

   >[!NOTE]
   >
   >Angebotssets, die einer Kampagne zugeordnet sind, können nicht gelöscht werden. Um ein mit einer Kampagne verknüpftes Angebotsset zu löschen, melden Sie sich bei Adobe Target Standard/Premium an und entfernen Sie zuerst die Kampagnenzuordnungen. Selbst wenn Sie die Zuordnung zu einer Kampagne aufgehoben haben, kann das Asset nur aus Adobe Dynamic Media Classic gelöscht werden, wozu eine Anmeldung bei Adobe Target Standard/Premium erforderlich ist und nicht aus Adobe Target Standard/Premium.

1. Wenn Sie die Bearbeitung abgeschlossen haben, stellen Sie in der rechten unteren Ecke der Seite sicher, dass **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Save]**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für den Satz ein und wählen Sie **[!UICONTROL Save]** aus.

## Angebotsset löschen {#deleting-an-offer-set}

Wenn Sie ein Angebotsset löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (bzw. die untergeordneten Elemente) innerhalb des Sets sind davon jedoch nicht betroffen; sie behalten ihren jeweiligen Status „veröffentlicht“ oder „unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie ein Angebotsset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht mindestens ein Angebotsset aus.
1. Wechseln Sie in der globalen Navigationsleiste zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **Löschen**.

>[!MORELIKETHIS]
>
>* [Erstellen von Vorlagenparametern](creating-template-parameters.md#creating_template_parameters)

