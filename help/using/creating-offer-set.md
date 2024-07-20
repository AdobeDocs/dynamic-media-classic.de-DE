---
title: Erstellen eines Angebotssets
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic ein Angebotsset erstellen.
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

# Erstellen eines Angebotssets {#creating-an-offer-set}

Sie können einen der folgenden Arten von Angebotssets erstellen:

* Video
* Parametrisierte Vorlage
* Bild

Wählen Sie für Vorlagen **[!UICONTROL Hinzufügen und Vorschau]** und legen Sie dann die von Ihnen gewählten Parameter fest. Andere Angebotssatz-Typen enthalten keine Parameter, Sie können sie jedoch dennoch anpassen, indem Sie **[!UICONTROL Vorschau]** auswählen und die verfügbaren Vorgaben ändern.

Adobe Dynamic Media Classic bietet Tools zum Bearbeiten und Erstellen von Angebotssets.

>[!NOTE]
>
>Bevor Sie ein Angebotsset erstellen, stellen Sie sicher, dass Sie alle Assets veröffentlichen, die Sie für das Set in Adobe Dynamic Media Classic verwenden möchten. Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

## Arten von Angebotssets {#types-of-offer-sets}

Erstellen Sie ein Angebotsset aus den folgenden Arten von Angebotssets:

* **Bilder**: Sie können Bilder für ein Angebotsset zusammenstellen. Jedes Bild enthält ein anderes Angebot im Set.

* **Bildvorlage**: Sie können Bildvorlagen in Adobe Dynamic Media Classic mit dem Befehl **[!UICONTROL Build]** > Vorlagengrundlagen parametrisieren. Über Parameter können Komponenten der Vorlage, der Text in Textrahmen und die verschiedenen Bilder ausgetauscht und angepasst werden. Für Angebotssets können Sie Vorlagenparameter verwenden, um beispielsweise Varianten desselben Bildes in Ihrem Angebotsset zu erstellen. Informationen zum Erstellen und Parametrisieren von Bildvorlagen finden Sie unter [Vorlagenparameter erstellen](creating-template-parameters.md#creating_template_parameters).

Siehe auch Schulungsvideo zu [Vorlagengrundlagen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) .

* **Video**: Sie können Videos für ein Angebotsset zusammenstellen. Jedes Video besteht dabei aus einem anderen Angebot im Set.

## Erstellen eines Angebotssets mit einer parametrisierten Vorlage {#creating-an-offer-set-with-a-parameterized-template}

Wenn Sie ein Angebotsset erstellen, wirkt sich die Option **[!UICONTROL Publish nach dem Speichern]** wie folgt auf das Set und die Set-Mitglieder aus:

| **[!UICONTROL Publish nach einer Speicheroption]** ausgewählt, bevor sie gespeichert wird? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein Angebotsset mit einer parametrisierten Vorlage:**

1. Wählen Sie die Vorlage oder das Banner aus.
1. Navigieren Sie zu **[!UICONTROL Build]** > **[!UICONTROL Test&amp;Target-Angebotsset]**.

   Auf der Seite &quot;Test&amp;Target-Angebotsset&quot;werden die Angebote im Angebotsset aufgelistet. Das erste Element in der Liste ist das Objekt.

1. Wählen Sie das Objekt aus und wählen Sie **[!UICONTROL Hinzufügen und Vorschau hinzufügen]** aus.

   Links auf dieser Seite sind die Parameter in der Vorlage mit ihren Werten aufgelistet.

1. Ändern Sie die Parameterwerte, um das Angebot zu erstellen. Geben Sie beispielsweise einen anderen Text in ein Textfeld ein, ändern Sie die Größe einer Ebene, tauschen Sie ein Bild gegen ein anderes aus oder wählen Sie eine andere Viewer-Vorgabe aus.
1. Wählen Sie **[!UICONTROL Speichern]** oder **[!UICONTROL Speichern unter**]** aus, um das Angebot als Teil des Angebotssets zu speichern.

   Auf der Seite &quot;Test&amp;Target-Angebotsset&quot;werden die von Ihnen erstellten Angebote aufgelistet.

1. Wiederholen Sie die Schritte 3 bis 5, um weitere Angebote für das Set zu erstellen.
1. Stellen Sie beim Beenden sicher, dass rechts unten auf der Seite **[!UICONTROL Publish nach einem Speichern*]** ausgewählt ist (Standard).
1. Wählen Sie &quot;**[!UICONTROL Schließen]**&quot;, geben Sie einen Namen für das Angebotsset ein und wählen Sie dann &quot;**[!UICONTROL Speichern]**&quot;.

Bevor Sie die Seite &quot;Test&amp;Target-Angebotsset&quot;schließen, pushen Sie das Angebotsset auf Adobe Target Standard/Premium. Siehe [Push-Angebotssätze an Test&amp;Target senden](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Erstellen eines Angebotssets mit Bildern oder Videos {#creating-an-offer-set-with-images-or-videos}

Wenn Sie ein Angebotsset erstellen, wirkt sich die Option **[!UICONTROL Publish nach dem Speichern]** wie folgt auf das Set und die Set-Mitglieder aus:

| **[!UICONTROL Publish nach einer Speicheroption]** ausgewählt, bevor sie gespeichert wird? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie ein Angebotsset mit Bildern oder Videos:**

1. Stellen Sie Bilder oder Videos für das Angebotsset zusammen. Starten Sie im Bildschirm &quot;Test&amp;Target-Angebotsset&quot;oder in der Raster- oder Listenansicht und verwenden Sie eine der folgenden Methoden:

   * **Bildschirm &quot;Test&amp;Target-Angebotsset&quot;**: Wechseln Sie zu &quot;**[!UICONTROL Build]**&quot;> &quot;**[!UICONTROL Test&amp;Target-Angebotsset]**&quot;. Ziehen Sie die Bilder oder Videos in den Anzeigebereich. Wenn Sie verschiedene Video- oder Bildgrößen erstellen möchten, ziehen Sie mehrere Kopien des Bildes oder Videos in den Anzeigebereich und legen Sie jede Größe einzeln fest.

   * **Rasteransicht oder Listenansicht**: Wählen Sie die Bilder oder Videos aus und gehen Sie dann zu **[!UICONTROL Build]** > **[!UICONTROL Test&amp;Target-Angebotsset]**.

1. Wählen Sie optional ein Bild oder Video aus und wählen Sie **[!UICONTROL Vorschau]** aus. Auf der Seite &quot;Angebote in der Vorschau&quot;können Sie die Größe und das Aussehen des ausgewählten Bildes oder Videos ändern. Sie können auch alle Bilder oder Videos im Angebotsset ändern.

   * Wählen Sie eine Vorlage aus, um Ansicht und Größe des Bildes oder Videos zu verändern.
   * Um die Vorgabe, die Sie ausgewählt haben, auf alle Angebote im Angebotsset anzuwenden, aktivieren Sie das Kontrollkästchen **[!UICONTROL Vorgaben für alle auswählen]** .

   Wählen Sie **[!UICONTROL Speichern]** aus, um Ihre Änderungen am Bild- oder Videoangebot zu speichern. Wählen Sie dann **[!UICONTROL Schließen]** aus, um zur Seite Test&amp;Target-Angebotsset zurückzukehren.

1. Nachdem Sie die Erstellung von Angeboten für das Angebotsset abgeschlossen und Bildvorgaben für verschiedene Bilder ausgewählt haben, stellen Sie sicher, dass **[!UICONTROL Publish nach dem Speichern]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]** aus, geben Sie einen Namen für das Angebotsset ein und wählen Sie **[!UICONTROL Speichern]** aus.

Bevor Sie die Seite &quot;Test&amp;Target-Angebotsset&quot;schließen, pushen Sie das Angebotsset auf Adobe Target Standard/Premium. Siehe [Push-Angebotssätze an Test&amp;Target senden](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## Bearbeiten von Angebotssets {#editing-an-offer-set}

Unabhängig davon, ob Sie einen veröffentlichten oder einen nicht veröffentlichten Satz bearbeiten, wirkt sich die Option **[!UICONTROL Publish nach dem Speichern]** wie folgt auf das Set und die Setmitglieder aus:

| Set bereits veröffentlicht? | **[!UICONTROL Publish nach Auswahl einer Speicheroption]** vor dem Speichern der Bearbeitung? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren Veröffentlichungsstatus bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie ein Angebotsset:**

1. Um ein Angebotsset zu bearbeiten, zeigen Sie es in der Raster- oder Listenansicht an und wählen Sie dann die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** aus.
1. Führen Sie auf der Seite &quot;Test&amp;Target-Angebotsset&quot;einen der folgenden Schritte aus:

   * **Entfernen eines Angebots**: Wählen Sie das Angebot aus und klicken Sie dann auf **[!UICONTROL Löschen]** , um ein Angebot aus dem Satz zu entfernen.
   * **Hinzufügen eines Angebots**: Wie Sie ein Angebot hinzufügen, hängt vom Typ des Angebotssets ab, mit dem Sie arbeiten:
      * **Vorlagen**: Wählen Sie **[!UICONTROL Hinzufügen und Vorschau hinzufügen]** aus und erstellen Sie auf der Seite Hinzufügen und Vorschau von Angeboten ein weiteres Angebot.
      * **Bilder und Videos**: Ziehen Sie ein Bild oder Video auf die Seite Test&amp;Target-Angebotsset .

   >[!NOTE]
   >
   >Ein mit einer Kampagne verknüpftes Angebotsset kann nicht gelöscht werden. Um ein mit einer Kampagne verknüpftes Angebotsset zu löschen, melden Sie sich bei Adobe Target Standard/Premium an und entfernen Sie zuerst die Kampagnenzuordnungen. Selbst wenn Sie die Zuordnung zu einer Kampagne aufgehoben haben, kann das Asset nur aus Adobe Dynamic Media Classic gelöscht werden, wozu eine Anmeldung bei Adobe Target Standard/Premium erforderlich ist und nicht aus Adobe Target Standard/Premium.

1. Stellen Sie nach Abschluss der Bearbeitung in der Nähe der rechten unteren Ecke der Seite sicher, dass **[!UICONTROL Publish nach dem Speichern]** ausgewählt ist (Standard).
1. Wählen Sie &quot;**[!UICONTROL Speichern]**&quot;, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und wählen Sie dann &quot;**[!UICONTROL Speichern]**&quot;.

## Löschen von Angebotssets {#delet-an-offer-set}

Wenn Sie ein Angebotsset löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (oder &quot;untergeordneten Elemente&quot;) in diesem Satz sind jedoch nicht betroffen. Stattdessen behalten sie ihren vorhandenen Status veröffentlicht oder unveröffentlicht bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie ein Angebotsset:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht mindestens ein Angebotsset aus.
1. Wechseln Sie in der Leiste &quot;Globale Navigation&quot;zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **Löschen**.

>[!MORELIKETHIS]
>
>* [Erstellen von Vorlagenparametern](creating-template-parameters.md#creating_template_parameters)
