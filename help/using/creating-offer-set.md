---
title: Angebotssatz erstellen
description: Erfahren Sie, wie Sie ein Angebotsset in Adobe Dynamic Media Classic erstellen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
topic: Integrations, Development
level: Experienced
source-git-commit: 910410706fbd9dd79a8dda402af454a50132cc41
workflow-type: tm+mt
source-wordcount: '1227'
ht-degree: 33%

---

# Angebotssatz erstellen {#creating-an-offer-set}

Sie können die folgenden Angebotsset-Typen erstellen:

* Video
* Parametrisierte Vorlage
* Bild

Wählen Sie für Vorlagen **[!UICONTROL Hinzufügen und Vorschau]** und legen Sie dann die von Ihnen gewählten Parameter fest. Andere Angebotssatztypen enthalten keine Parameter, können aber dennoch angepasst werden, indem Sie **[!UICONTROL Vorschau]** und die verfügbaren Vorgaben ändern.

Adobe Dynamic Media Classic bietet Tools zum Bearbeiten und Erstellen von Angebotssets.

>[!NOTE]
>
>Bevor Sie ein Angebotsset erstellen, stellen Sie sicher, dass Sie alle Assets veröffentlichen, die Sie für das Set verwenden möchten, und zwar in Adobe Dynamic Media Classic. Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

## Angebotsset-Typen {#types-of-offer-sets}

Erstellen Sie ein Angebotsset aus den folgenden Angebotsset-Typen:

* **Bilder** - Sie können Bilder für ein Angebotsset zusammenstellen. Jedes Bild enthält ein anderes Angebot im Set.

* **Bildvorlage** - Sie können Bildvorlagen in Adobe Dynamic Media Classic mit der **[!UICONTROL Build]** > Vorlagengrundlagen, Befehl. Mithilfe von Parametern können Komponenten der Vorlage (Text in Textrahmen, die verschiedenen Bilder) ausgetauscht und angepasst werden. Für ein Angebotsset können Sie beispielsweise mithilfe von Vorlagenparametern verschiedene Varianten desselben Bildes erstellen. Informationen zum Erstellen und Parametrisieren von Bildvorlagen finden Sie unter [Vorlagenparameter erstellen](creating-template-parameters.md#creating_template_parameters).

Siehe auch [Vorlagengrundlagen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) Schulungsvideo.

* **Video** - Sie können Videos für ein Angebotsset zusammenstellen. Jedes Video besteht dabei aus einem anderen Angebot im Set.

## Angebotssatz mit parametrierter Vorlage erstellen {#creating-an-offer-set-with-a-parameterized-template}

Wenn Sie ein Angebotsset erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| **[!UICONTROL Nach dem Speichern veröffentlichen]** vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein Angebotsset mit einer parametrisierten Vorlage:**

1. Wählen Sie die Vorlage oder das Banner aus.
1. Navigieren Sie zu **[!UICONTROL Build]** > **[!UICONTROL Test&amp;Target-Angebotsset]**.

   Auf der Seite &quot;Test&amp;Target-Angebotsset&quot;werden die Angebote im Angebotsset aufgelistet. Das erste Element in der Liste ist das Objekt.

1. Wählen Sie das Objekt aus und wählen Sie **[!UICONTROL Hinzufügen und Vorschau]**.

   Links auf dieser Seite sind die Parameter in der Vorlage mit ihren Werten aufgelistet.

1. Ändern Sie die Parameterwerte, um das Angebot zu erstellen. Geben Sie beispielsweise anderen Text in ein Textfeld ein, ändern Sie die Größe einer Ebene, tauschen Sie ein Bild durch ein anderes aus oder wählen Sie eine andere Viewer-Vorgabe.
1. Auswählen **[!UICONTROL Speichern]** oder **[!UICONTROL Speichern unter**]** , um das Angebot als Teil des Angebotssatzes zu speichern.

   Auf der Seite &quot;Test&amp;Target-Angebotsset&quot;werden die von Ihnen erstellten Angebote aufgelistet.

1. Wiederholen Sie die Schritte 3 bis 5, um weitere Angebote für das Set zu erstellen.
1. Stellen Sie beim Beenden in der rechten unteren Ecke der Seite sicher, dass **[!UICONTROL Nach dem Speichern veröffentlichen*]** ausgewählt ist (Standard).
1. Auswählen **[!UICONTROL Schließen]**, geben Sie einen Namen für das Angebotsset ein und wählen Sie **[!UICONTROL Speichern]**.

Bevor Sie die Seite &quot;Test&amp;Target-Angebotsset&quot;schließen, pushen Sie das Angebotsset auf Adobe Target Standard/Premium. Siehe [Angebotssets an Test&amp;Target pushen](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Angebotssatz mit Bildern oder Videos erstellen {#creating-an-offer-set-with-images-or-videos}

Wenn Sie ein Angebotsset erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| **[!UICONTROL Nach dem Speichern veröffentlichen]** vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein Angebotsset mit Bildern oder Videos:**

1. Stellen Sie Bilder oder Videos für das Angebotsset zusammen. Starten Sie im Bildschirm &quot;Test&amp;Target-Angebotsset&quot;oder in der Raster- oder Listenansicht und verwenden Sie eine der folgenden Methoden:

   * **Bildschirm &quot;Test&amp;Target-Angebotsset&quot;** - Gehen Sie zu **[!UICONTROL Build]** > **[!UICONTROL Test&amp;Target-Angebotsset]**. Ziehen Sie die Bilder oder Videos in den Anzeigebereich. Wenn Sie verschiedene Video- oder Bildgrößen erstellen möchten, ziehen Sie mehrere Kopien des Bildes oder Videos in den Anzeigebereich und legen Sie jede Größe einzeln fest.

   * **Rasteransicht oder Listenansicht** - Wählen Sie die Bilder oder Videos aus und gehen Sie dann zu **[!UICONTROL Build]** > **[!UICONTROL Test&amp;Target-Angebotsset]**.

1. Wählen Sie optional ein Bild oder Video aus und wählen Sie **[!UICONTROL Vorschau]**. Auf der Seite &quot;Angebote in der Vorschau&quot;können Sie die Größe und das Aussehen des ausgewählten Bildes oder Videos ändern. Sie können auch alle Bilder oder Videos im Angebotsset ändern.

   * Wählen Sie eine Vorlage aus, um Ansicht und Größe des Bildes oder Videos zu verändern.
   * Um die ausgewählte Vorgabe auf alle Angebote im Angebotsset anzuwenden, wählen Sie die **[!UICONTROL Voreinstellungen für alle auswählen]** aktivieren.

   Auswählen **[!UICONTROL Speichern]** , um Ihre Änderungen am Bild- oder Videoangebot zu speichern. Wählen Sie anschließend **[!UICONTROL Schließen]** , um zur Seite Test&amp;Target-Angebotsset zurückzukehren.

1. Nachdem Sie die Angebote für das Angebotsset erstellt und Bildvorgaben für verschiedene Bilder ausgewählt haben, stellen Sie sicher, dass **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Auswählen **[!UICONTROL Speichern]** und geben Sie einen Namen für das Angebotsset ein und wählen Sie **[!UICONTROL Speichern]**.

Bevor Sie die Seite &quot;Test&amp;Target-Angebotsset&quot;schließen, pushen Sie das Angebotsset auf Adobe Target Standard/Premium. Siehe [Angebotssets an Test&amp;Target pushen](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Bearbeiten eines Angebotssets {#editing-an-offer-set}

Unabhängig davon, ob Sie ein veröffentlichtes Set oder ein nicht veröffentlichtes Set bearbeiten, wird die **[!UICONTROL Nach dem Speichern veröffentlichen]** -Option wirkt sich auf die Set- und Set-Mitglieder wie folgt aus:

| Set bereits veröffentlicht? | **[!UICONTROL Nach dem Speichern veröffentlichen]** vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren Veröffentlichungsstatus bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie ein Angebotsset:**

1. Um ein Angebotsset zu bearbeiten, zeigen Sie es in der Raster- oder Listenansicht an und wählen Sie dann dessen **[!UICONTROL Bearbeiten]** Rollover-Schaltfläche.
1. Führen Sie auf der Seite &quot;Test&amp;Target-Angebotsset&quot;einen der folgenden Schritte aus:

   * **Entfernen eines Angebots** - Wählen Sie das Angebot aus und klicken Sie auf **[!UICONTROL Löschen]** , um ein Angebot aus dem Satz zu entfernen.
   * **Hinzufügen eines Angebots** - Wie Sie ein Angebot hinzufügen, hängt vom Typ des Angebots ab, mit dem Sie arbeiten:
      * **Vorlagen** - Auswählen **[!UICONTROL Hinzufügen und Vorschau]** und erstellen Sie auf der Seite Hinzufügen und Vorschau von Angeboten ein weiteres Angebot.
      * **Bilder und Videos** - Ziehen Sie ein Bild oder Video auf die Seite Test&amp;Target-Angebotsset .

   >[!NOTE]
   >
   >Angebotssets, die einer Kampagne zugeordnet sind, können nicht gelöscht werden. Um ein mit einer Kampagne verknüpftes Angebotsset zu löschen, melden Sie sich bei Adobe Target Standard/Premium an und entfernen Sie zuerst die Kampagnenzuordnungen. Selbst wenn Sie die Zuordnung zu einer Kampagne aufgehoben haben, kann das Asset nur aus Adobe Dynamic Media Classic gelöscht werden, wozu eine Anmeldung bei Adobe Target Standard/Premium erforderlich ist und nicht aus Adobe Target Standard/Premium.

1. Stellen Sie nach Abschluss der Bearbeitung in der Nähe der rechten unteren Ecke der Seite sicher, dass **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Auswählen **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und wählen Sie dann **[!UICONTROL Speichern]**.

## Angebotsset löschen {#delet-an-offer-set}

Wenn Sie ein Angebotsset löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (oder &quot;untergeordneten Elemente&quot;) in diesem Satz sind jedoch nicht betroffen. Stattdessen behalten sie ihren vorhandenen Status veröffentlicht oder unveröffentlicht bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie ein Angebotsset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht mindestens ein Angebotsset aus.
1. Wechseln Sie in der Leiste Globale Navigation zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **Löschen**.

>[!MORELIKETHIS]
>
>* [Erstellen von Vorlagenparametern](creating-template-parameters.md#creating_template_parameters)
