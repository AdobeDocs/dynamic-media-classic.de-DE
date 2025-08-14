---
title: Erstellen von Angebotssets
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic einen Angebotssatz erstellen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
topic: Integrations, Development
level: Experienced
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 21%

---

# Erstellen von Angebotssets {#creating-an-offer-set}

Sie können jeden der folgenden Typen von Angebotssätzen erstellen:

* Video
* Parametrisierte Vorlage
* Bild

Klicken Sie bei Vorlagen auf **[!UICONTROL Hinzufügen und Vorschau]** und legen Sie dann die ausgewählten Parameter fest. Andere Angebotssatztypen enthalten keine Parameter, Sie können sie jedoch anpassen, indem Sie **[!UICONTROL Vorschau]** auswählen und die verfügbaren Voreinstellungen ändern.

Adobe Dynamic Media Classic bietet Tools zum Bearbeiten und Erstellen von Angebotssätzen.

>[!NOTE]
>
>Bevor Sie ein Angebotsset erstellen, stellen Sie sicher, dass Sie alle Assets, die Sie für das Set verwenden möchten, in Adobe Dynamic Media Classic veröffentlichen. Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

## Typen von Angebots-Sets {#types-of-offer-sets}

Erstellen Sie ein Angebotsset aus den folgenden Arten von Angebotssets:

* **Bilder**: Sie können Bilder für ein Angebotsset zusammenstellen. Jedes Bild enthält ein anderes Angebot im Set.

* **Bildvorlage**: Sie können Bildvorlagen in Adobe Dynamic Media Classic mit dem Befehl **[!UICONTROL Erstellen]** > Vorlagengrundlagen parametrisieren. Durch Parameter können Komponenten der Vorlage, der Text in Textrahmen und die verschiedenen Bilder ausgetauscht und angepasst werden. Für ein Angebotsset können Sie beispielsweise mithilfe von Vorlagenparametern Varianten desselben Bildes in Ihrem Angebotsset erstellen. Informationen zum Erstellen und Parametrisieren von Bildvorlagen finden Sie unter [Erstellen von Vorlagenparametern](creating-template-parameters.md#creating_template_parameters).

Siehe auch [Vorlagengrundlagen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) Schulungsvideo.

* **Video**: Sie können Videos für ein Angebotsset zusammenstellen. Jedes Video besteht dabei aus einem anderen Angebot im Set.

## Erstellen eines Angebotssets mit einer parametrisierten Vorlage {#creating-an-offer-set-with-a-parameterized-template}

Wenn Sie ein Angebotsset erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** auf das Set und die Set-Mitglieder wie folgt aus:

| **[!UICONTROL Nach Speichern veröffentlichen]** vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein Angebotsset mit einer parametrisierten Vorlage:**

1. Wählen Sie die Vorlage oder das Banner aus.
1. Navigieren Sie **[!UICONTROL Erstellen]** > **[!UICONTROL Test&amp;Target-]**.

   Auf der Seite „Test&amp;Target-Angebotssatz“ werden Angebote im Angebotssatz aufgelistet. Das erste Element in der Liste ist das Objekt.

1. Wählen Sie das -Objekt aus und wählen **[!UICONTROL Hinzufügen und Vorschau]**.

   Links auf dieser Seite sind die Parameter in der Vorlage mit ihren Werten aufgelistet.

1. Ändern Sie die Parameterwerte, um das Angebot zu erstellen. Geben Sie beispielsweise einen anderen Text in ein Textfeld ein, ändern Sie die Größe einer Ebene, tauschen Sie ein Bild durch ein anderes aus oder wählen Sie eine andere Viewer-Vorgabe aus.
1. Wählen Sie **[!UICONTROL Speichern]** oder **[!UICONTROL Speichern unter**]**, um das Angebot als Teil des Angebotssatzes zu speichern.

   Auf der Seite „Test&amp;Target-Angebotsset“ werden die von Ihnen erstellten Angebote aufgelistet.

1. Wiederholen Sie die Schritte 3 bis 5, um weitere Angebote für das Set zu erstellen.
1. Stellen Sie nach Abschluss des Vorgangs in der unteren rechten Ecke der Seite sicher, dass **[!UICONTROL Veröffentlichen nach dem Speichern*]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Schließen]**, geben Sie einen Namen für das Angebotsset ein und klicken Sie auf **[!UICONTROL Speichern]**.

Bevor Sie die Seite „Test&amp;Target-Angebotssatz“ schließen, übertragen Sie das Angebotssatz auf Adobe Target Standard/Premium. Siehe [Pushen von Angebotssätzen an Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Erstellen eines Angebotssets mit Bildern oder Videos {#creating-an-offer-set-with-images-or-videos}

Wenn Sie ein Angebotsset erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** auf das Set und die Set-Mitglieder wie folgt aus:

| **[!UICONTROL Nach Speichern veröffentlichen]** vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein Angebotsset mit Bildern oder Videos:**

1. Stellen Sie Bilder oder Videos für das Angebotssatz zusammen. Beginnen Sie im Bildschirm Test&amp;Target-Angebotsset oder in der Rasteransicht oder Listenansicht und verwenden Sie eine der folgenden Methoden:

   * **Bildschirm „Test&amp;Target-**&quot;: Wechseln Sie zu **[!UICONTROL Erstellen]** > **[!UICONTROL Test&amp;Target-]**. Ziehen Sie die Bilder oder Videos in den Anzeigebereich. Wenn Sie verschiedene Video- oder Bildgrößen erstellen möchten, ziehen Sie mehrere Kopien des Bildes oder Videos in den Anzeigebereich und legen Sie jede Größe einzeln fest.

   * **Rasteransicht oder Listenansicht**: Wählen Sie die Bilder oder Videos aus und gehen Sie dann zu **[!UICONTROL Erstellen]** > **[!UICONTROL Test&amp;Target-]**.

1. Wählen Sie optional ein Bild oder Video aus und klicken Sie auf **[!UICONTROL Vorschau]**. Auf der Seite Angebotsvorschau können Sie die Größe und das Erscheinungsbild des ausgewählten Bildes oder Videos ändern. Sie können auch alle Bilder oder Videos im Angebotsset ändern.

   * Wählen Sie eine Vorlage aus, um Ansicht und Größe des Bildes oder Videos zu verändern.
   * Um die von Ihnen ausgewählte Voreinstellung auf alle Angebote im Angebotsset anzuwenden, aktivieren Sie das Kontrollkästchen **[!UICONTROL Voreinstellungen auf alle]** auswählen“.

   Klicken Sie **[!UICONTROL Speichern]**, um Ihre Änderungen am Bild- oder Videoangebot zu speichern. Wählen Sie anschließend **[!UICONTROL Schließen]**, um zur Seite „Test&amp;Target-Angebotssatz“ zurückzukehren.

1. Nachdem Sie die Erstellung der Angebote für das Angebotsset abgeschlossen und Bildvorgaben für verschiedene Bilder ausgewählt haben, stellen Sie sicher, dass **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]**, geben Sie einen Namen für das Angebotsset ein und klicken Sie auf **[!UICONTROL Speichern]**.

Pushen Sie vor dem Schließen der Seite „Test&amp;Target-Angebotssatz“ das Angebotssatz auf Adobe Target Standard/Premium. Siehe [Pushen von Angebotssätzen an Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Bearbeiten von Angebotssets {#editing-an-offer-set}

Unabhängig davon, ob Sie ein veröffentlichtes Set oder ein unveröffentlichtes Set bearbeiten, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** auf die Mitglieder des Sets und des Sets wie folgt aus:

| Set bereits veröffentlicht? | **[!UICONTROL Nach dem Speichern veröffentlichen]** Option vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren veröffentlichten Status bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie ein Angebotsset:**

1. Um ein Angebotsset zu bearbeiten, zeigen Sie das Angebotsset in der Rasteransicht oder Listenansicht an und klicken Sie auf die **[!UICONTROL „Bearbeiten]**.
1. Führen Sie auf der Seite „Test&amp;Target-Angebotssatz“ einen der folgenden Schritte aus:

   * **Entfernen eines Angebots**: Wählen Sie das Angebot aus und klicken Sie dann auf **[!UICONTROL Löschen]**, um ein Angebot aus dem Set zu entfernen.
   * **Hinzufügen eines Angebots**: Wie Sie ein Angebot hinzufügen, hängt vom Typ des Angebotssatzes ab, mit dem Sie arbeiten:
      * **Vorlagen**: Wählen Sie **[!UICONTROL Hinzufügen und Vorschau]** aus und erstellen Sie auf der Seite „Hinzufügen und Vorschau von Angeboten“ ein weiteres Angebot.
      * **Bilder und Videos**: Ziehen Sie ein Bild oder Video auf die Seite „Test&amp;Target-Angebotssatz“.

   >[!NOTE]
   >
   >Ein mit einer Kampagne verknüpftes Angebotsset kann nicht gelöscht werden. Um einen mit einer Kampagne verknüpften Angebotssatz zu löschen, melden Sie sich bei Adobe Target Standard/Premium an und entfernen Sie zuerst die Kampagnenverknüpfungen. Selbst nach dem Aufheben der Verknüpfung mit einer Kampagne kann das Asset nur aus Adobe Dynamic Media Classic gelöscht werden, wodurch eine Anmeldung bei Adobe Target Standard/Premium erforderlich ist, nicht jedoch aus Adobe Target Standard/Premium.

1. Stellen Sie nach Abschluss der Bearbeitung in der unteren rechten Ecke der Seite sicher, dass **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **[!UICONTROL Speichern]**.

## Löschen von Angebotssets {#delet-an-offer-set}

Wenn Sie ein Angebotsset löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (oder „untergeordneten Elemente„) in diesem Set sind jedoch nicht betroffen. Stattdessen behalten sie jeweils ihren vorhandenen Status „Veröffentlicht“ oder „Unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie ein Angebotsset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Angebotssets aus.
1. Navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **Löschen**.

>[!MORELIKETHIS]
>
>* [Erstellen von Vorlagenparametern](creating-template-parameters.md#creating_template_parameters)
