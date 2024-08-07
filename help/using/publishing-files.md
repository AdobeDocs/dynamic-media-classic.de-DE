---
title: Publish-Dateien
description: Erfahren Sie, wie Sie Ihre Assets auf Dynamic Media-Image-Servern veröffentlichen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1674'
ht-degree: 21%

---

# Publish-Dateien{#publishing-files}

Sie veröffentlichen Ihre Assets auf Dynamic Media-Image-Servern. Sie können Assets einmalig veröffentlichen oder dafür sorgen, dass Adobe Dynamic Media Classic Assets regelmäßig veröffentlicht. Sobald die Assets veröffentlicht wurden, sind sie für Sie zur Bereitstellung verfügbar. Sie können die URL-Aufrufe aus Adobe Dynamic Media Classic kopieren und zu Ihrer Website oder Anwendung hinzufügen.

Adobe Dynamic Media Classic unterstützt jetzt die Bereitstellung aller Bilder und Videos über HTTP/2. Das heißt, dass eine veröffentlichte URL oder ein Einbettungscode für das Bild oder Video verfügbar ist, um in jede Anwendung integriert zu werden, die ein gehostetes Asset akzeptiert. Dieses veröffentlichte Asset verwendet das HTTP/2-Protokoll, um es bereitzustellen. Diese Bereitstellungsmethode verbessert die Kommunikation von Browsern und Servern, sodass die Antwort- und Ladezeiten aller Adobe Dynamic Media Classic-Assets verbessert werden. Siehe [Häufig gestellte Fragen zur Bereitstellung von Inhalten über HTTP2](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/http2).

## Nach dem Hochladen veröffentlichen {#publish-after-uploading}

Assets befinden sich entweder in einem veröffentlichten oder unveröffentlichten Status. Standardmäßig werden alle Assets, die Sie in Adobe Dynamic Media Classic hochladen, automatisch zur Veröffentlichung markiert.

Weitere Informationen finden Sie unter [Sofortiger Publish-Hinweis-PDF](/help/using/assets/rendering-instant-publish-notification.pdf).

Verwenden Sie die folgenden Verfahren, um Assets zur Veröffentlichung zu markieren:

* **[!UICONTROL Publish nach dem Hochladen]**: Wählen Sie auf der Seite &quot;Hochladen&quot;unten **[!UICONTROL Publish nach dem Hochladen]** aus. Die Standardeinstellung ist „ausgewählt“.

* **[!UICONTROL Publish nach dem Hochladen]**: Wählen Sie im Dialogfeld &quot;Auftragsoptionen&quot;die Option **[!UICONTROL Publish nach dem Hochladen]** aus. Die Standardeinstellung ist „ausgewählt“.

Einige abgeleitete Assets werden automatisch zur Veröffentlichung markiert, wenn ihre Stammelemente zur Veröffentlichung markiert werden. In dieser Tabelle werden untergeordnete Assets aufgeführt, die automatisch zur Veröffentlichung markiert werden.

| Übergeordnetes Element (Gruppe) | Untergeordnete Elemente (Mitglieder) |
| --- | --- |
| Bildsätze | Die Bilder in einem Satz. |
| Mustersets | Die Farbfelder in einem Satz. |
| Rotationssets | Die Bilder in einem Satz. |
| Vorlagen | Vorlagendateien, Seiten und Bilder. |

Abgeleitete Bilder werden auch automatisch zur Veröffentlichung markiert, wenn ihre übergeordneten Bilder veröffentlicht werden. Abgeleitete Bilder sind beispielsweise Bilder, die Sie mit Bildbearbeitungsoptionen angepasst haben. Sie können diese abgeleiteten Bilder in der Detailansicht unter &quot;Built &amp; Derivatives&quot;anzeigen.

## Veröffentlichungsauftrag erstellen {#creating-a-publish-job}

Erstellen Sie einen Veröffentlichungsauftrag, um Assets zu veröffentlichen, die Sie auf Adobe Dynamic Media Classic-Server hochgeladen haben, aber noch nicht automatisch veröffentlicht werden sollen. Sie können einen einmaligen Veröffentlichungsauftrag ausführen oder Aufträge planen, die regelmäßig wiederholt werden. Adobe Dynamic Media Classic bietet erweiterte Veröffentlichungsoptionen für die Veröffentlichung auf bestimmten Servern und Optionen zum erneuten Veröffentlichen von Assets, die bereits veröffentlicht wurden.

**So erstellen Sie einen Veröffentlichungsauftrag:**

1. Wählen Sie in der globalen Navigationsleiste **[!UICONTROL Publish]** aus.
1. Wählen Sie im Dialogfeld &quot;Veröffentlichen&quot;aus, ob Sie einen einmaligen oder einen wiederkehrenden Veröffentlichungsauftrag erhalten möchten.

   Siehe [Erstellen eines einmaligen Veröffentlichungsauftrags](publishing-files.md#creating_a_one_time_publish_job) und [Erstellen eines wiederkehrenden Veröffentlichungsauftrags](publishing-files.md#creating_a_recurring_publish_job).

1. Geben Sie einen Auftragsnamen ein.
1. Blenden Sie optional die erweiterten Optionen ein und legen Sie die gewünschten Einstellungen fest. 

   Siehe [Erweiterte Veröffentlichungsoptionen](publishing-files.md#advanced_publish_options).

1. Wählen Sie **[!UICONTROL Publish übermitteln]** aus.

Adobe Dynamic Media Classic verfolgt Veröffentlichungsaufträge auf der Seite &quot;Aufträge&quot;nach. Sie können Veröffentlichungsaufträge auf dieser Seite überprüfen.

>[!NOTE]
>
>Assets, die Sie erneut veröffentlicht haben (Sie haben sie bereits veröffentlicht), werden aufgrund des Web-Caching-Mechanismus im Inhaltsbereitstellungsnetzwerk (Content Delivery Network, CDN) nicht sofort auf Ihrer Website angezeigt. Siehe [Erneut veröffentlichte Assets und CDN-Verzögerungen](publishing-files.md#republished_assets_and_cdn_delays).

### Erstellen eines einmaligen Veröffentlichungsauftrags {#creating-a-one-time-publish-job}

Erstellen Sie einen einmaligen Veröffentlichungsauftrag, indem Sie auf der Seite &quot;Veröffentlichung&quot;die Option **[!UICONTROL Einmalig]** auswählen.

Wenn der Veröffentlichungsauftrag später ausgeführt werden soll, wählen Sie auf der Seite &quot;Veröffentlichung&quot;die Option **[!UICONTROL Einmalig]** aus. Wählen Sie aus der Dropdownliste **[!UICONTROL Für später einplanen]** aus. Verwenden Sie den Kalender und den Zeitregler, um einen Tag und eine Uhrzeit für die Ausführung des Veröffentlichungsauftrags auszuwählen.

### Wiederkehrenden Veröffentlichungsauftrag erstellen {#creating-a-recurring-publish-job}

Erstellen Sie einen wiederkehrenden Veröffentlichungsauftrag, indem Sie auf der Seite &quot;Veröffentlichung&quot;die Option **[!UICONTROL Wiederkehrend]** auswählen.

Wählen Sie dann die Option &quot;Wiederholen&quot;aus: **[!UICONTROL Täglich]**, **[!UICONTROL Wöchentlich]**, **[!UICONTROL Monatlich]** oder **[!UICONTROL Benutzerdefiniert]** und geben Sie dann an, wann der Veröffentlichungsauftrag wiederholt werden soll. Adobe Dynamic Media Classic bietet Kalendertools zur Planung des wiederkehrenden Veröffentlichungsauftrags. Sie können die Option **[!UICONTROL Benutzerdefiniert]** auswählen und eine Regel in das Textfeld &quot;Regel&quot;eingeben, um ein benutzerdefiniertes Auftragsintervall zu beschreiben.

Siehe [Erstellen eines benutzerdefinierten Zeitintervalls für Upload- oder Veröffentlichungsaufträge](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>Wiederkehrende Veröffentlichungsaufträge (und Upload-Aufträge) werden auf der Seite „Aufträge“ aufgelistet. Wenn Sie einen geplanten Auftrag bearbeiten oder löschen möchten, wählen Sie auf der Seite „Aufträge“ die Registerkarte „Geplant“ aus.

### Erweiterte Veröffentlichungsoptionen {#advanced-publish-options}

Sie können die erweiterten Optionen auf der Seite &quot;Publishing&quot;anzeigen und die folgenden Optionen zum Verarbeiten eines Veröffentlichungsauftrags auswählen:

* **[!UICONTROL Publish bis]**: Wählen Sie einen Servertyp aus, um Assets nur auf einem bestimmten Server zu veröffentlichen.

* **[!UICONTROL Publish]**: Adobe Dynamic Media Classic veröffentlicht standardmäßig nur Assets, die neu sind und noch nicht veröffentlicht wurden (Option &quot;Neu seit letzter Publish&quot;). Sie können jedoch **[!UICONTROL Vollständige Publish]** auswählen, damit Sie auch Assets veröffentlichen können, die seit der letzten Veröffentlichung aktualisiert oder geändert wurden. Wählen Sie &quot;**[!UICONTROL Vollständig mit Suchdaten]**&quot;, wenn Sie einen E-Katalog veröffentlichen und möchten, dass Leser ihn nach Schlüsselwörtern durchsuchen können.

* **[!UICONTROL Auftrag ausführen als]**: Wählen Sie einen Benutzernamen aus der Liste aus. Auf der Seite „Aufträge“ können Aufträge nach Benutzername sortiert werden. Durch die Auswahl eines Namens verknüpfen Sie einen Veröffentlichungsauftrag mit einem Benutzer.

**[!UICONTROL HTTP-Benachrichtigung]**: Geben Sie eine URL für den Trigger nachfolgender Veröffentlichungsaufträge ein.

Siehe [Verwenden eines Upload- oder Veröffentlichungsauftrags als Trigger](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Veröffentlichungsauftrag abbrechen {#canceling-a-publish-job}

Sie können einen laufenden Veröffentlichungsauftrag abbrechen. Als Administrator können Sie einen in Verarbeitung befindlichen Veröffentlichungsauftrag auch über die Seite „Aufträge“ für das Unternehmen stornieren.

Um einen Veröffentlichungsauftrag abzubrechen, gehen Sie zur Seite &quot;Aufträge&quot;und wählen Sie **[!UICONTROL Abbrechen]** aus. Auf der Registerkarte &quot;Geplant&quot;der Seite &quot;Aufträge&quot;können Sie einen Auftrag anhalten oder fortsetzen, indem Sie in der Spalte &quot;Aktiv&quot;des Auftrags das Kontrollkästchen deaktivieren oder aktivieren.

>[!NOTE]
>
>Nachdem Sie einen Veröffentlichungsauftrag abgebrochen haben, erhält er den Status &quot;Anhalten&quot;, bis der Auftrag einen Punkt erreicht hat, an dem er sicher anhalten kann. Das Beenden eines Veröffentlichungsauftrags kann einige Zeit in Anspruch nehmen, wenn der Auftrag gerade Daten aus der Datenbank abruft.

## Publish-Assets manuell {#manually-publishing-assets}

Sie können einzelne Assets manuell veröffentlichen, anstatt einen Veröffentlichungsauftrag zu erstellen. Wenn Sie Sets veröffentlichen, z. B. ein Bildset oder ein adaptives Videoset, werden das Set (oder &quot;übergeordnetes Element&quot;) und alle Mitglieder (oder &quot;untergeordnete Elemente&quot;) innerhalb dieses Sets veröffentlicht.

Nicht veröffentlichte Assets werden in der Benutzeroberfläche durch ein graues, rundes Symbol mit einem Schrägstrich (Status &quot;Nicht veröffentlicht&quot;) links neben dem Asset-Namen angezeigt. Nach dem Veröffentlichen eines Assets ändert sich das Symbol in ein grünes Kreissymbol mit einem weißen Häkchen (Status „veröffentlicht“).

**So veröffentlichen Sie Assets manuell:**

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Assets aus.

     Wechseln Sie in der globalen Navigationsleiste zu **[!UICONTROL Datei]** > **[!UICONTROL Publish]**.

   * Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht das graue, runde Symbol mit einem Schrägstrich links neben dem Asset-Namen aus.

## Manuelles Rückgängigmachen der Veröffentlichung von Assets {#manually-unpublishing-assets}

Sie können die Veröffentlichung einzelner Assets manuell rückgängig machen. Wenn Sie die Veröffentlichung von Sets, z. B. eines Mustersets oder eines E-Katalogs, rückgängig machen, erhält das Set (oder &quot;übergeordnetes&quot;) selbst den Status &quot;unveröffentlicht&quot;. Die Mitglieder (oder &quot;untergeordneten Elemente&quot;) in diesem Satz sind jedoch nicht betroffen. Stattdessen behalten sie ihren vorhandenen Status veröffentlicht oder unveröffentlicht bei.

Veröffentlichte Assets werden in der Benutzeroberfläche durch ein rundes, grünes Symbol mit einem weißen Häkchen in der Mitte (Veröffentlichungsstatus) links neben dem Asset-Namen gekennzeichnet. Nachdem die Veröffentlichung eines Assets rückgängig gemacht wurde, wird das Symbol grau mit einem Schrägstrich (Status &quot;Nicht veröffentlicht&quot;) dargestellt.

**So machen Sie die Veröffentlichung von Assets manuell rückgängig:**

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere veröffentlichte Assets aus.

     Wechseln Sie in der globalen Navigationsleiste zu **[!UICONTROL Datei]** > **[!UICONTROL Veröffentlichung rückgängig machen]**.

   * Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht das runde grüne Häkchensymbol links neben dem Asset-Namen aus.

## Abrufen des Veröffentlichungsverlaufs eines Assets {#getting-an-asset-s-publish-history}

Das letzte Datum, an dem ein Asset veröffentlicht wurde, wird in der Detailansicht oben im Bedienfeld angezeigt. Weitere Informationen zum Veröffentlichungsverlauf erhalten Sie, indem Sie das Bedienfeld Verlauf und veröffentlichte Server in der Detailansicht öffnen. Dort wird angezeigt, wann und auf welchen Servern das Asset veröffentlicht wurde.

## Erneut veröffentlichte Assets und CDN-Verzögerungen {#republished-assets-and-cdn-delays}

Adobe Dynamic Media Classic-Assets werden im Content Delivery Network (CDN) verteilt. CDN ist ein System von vernetzten Computer-Servern, die auf transparente Weise zusammenarbeiten, um Inhalte – insbesondere umfangreiche Medieninhalte – für Endbenutzer bereitzustellen. Im CDN-System werden Webinhalte im Internet in Webcaches gespeichert (das so genannte Edge-Cache-Netzwerk). Web-Inhalte werden von den Web-Caches an Endbenutzer bereitgestellt, um schnellere Sendungen zu ermöglichen.

Wenn ein Benutzer eine Webseite zum ersten Mal herunterlädt, werden die Assets an einen CDN-Web-Cache-Server bereitgestellt. Dieser Server speichert sie so, dass beim nächsten Zugriff eines Benutzers im selben Bereich auf die Webseite derselbe zwischengespeicherte Inhalt schneller bereitgestellt wird. Die Inhaltsbereitstellung erfolgt schneller, weil der Inhalt näher beim Endbenutzer aufbewahrt wird. CDN ermöglicht eine schnellere Anzeige von Webseiten. Die Bandbreitenanforderungen an den zentralen Server werden verringert, da die Inhalte über das Edge-Cache-Netzwerk bereitgestellt werden, nicht jedes Mal von einem zentralen Server aus.

Neu veröffentlichte Adobe Dynamic Media Classic-Inhalte stehen dem Endbenutzer sofort zur Verfügung und füllen das Edge-Cache-Netzwerk schnell. Neu veröffentlichte Inhalte, d. h. Bilder mit demselben Namen wie zuvor auf einem Image-Server veröffentlichte Bilder, werden jedoch bis zu zehn Stunden lang nicht im CDN aktualisiert. Stattdessen sehen Endbenutzer, was sich in einem Web-Cache im CDN-Netzwerk befindet. Aus diesem Grund werden die erneut veröffentlichten Adobe Dynamic Media Classic-Assets den Endbenutzern zehn Stunden lang nicht angezeigt.

Wenn Sie möchten, dass Ihre neu veröffentlichten Bild-Assets schneller als mit zehnstündiger Verzögerung verfügbar sind, können Sie Web-Caches im CDN leeren. Wenn Sie diese Web-Caches leeren, werden alte Inhalte aus CDN-Web-Caches entfernt und durch die zuletzt veröffentlichten Assets ersetzt.

Um den Cache zu leeren, gehen Sie in der Leiste &quot;Globale Navigation&quot;zu **[!UICONTROL Datei]** > **[!UICONTROL Ungültiges CDN]**. Alle ausgewählten Dateien werden aus dem Cache entfernt. Wenn keine veröffentlichbare Assets vorhanden oder Sie kein Unternehmensadministrator sind, ist die CDN-Option „Entfernen“ nicht verfügbar.

>[!MORELIKETHIS]
>
>* [Überprüfen der Auftragsdateien](checking-job-files.md)
>* [Wiederholte Aufträge bearbeiten, löschen, anhalten und fortsetzen](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)
