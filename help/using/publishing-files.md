---
title: Publish-Dateien
description: Erfahren Sie, wie Sie Ihre Assets auf Dynamic Media-Bildservern veröffentlichen.
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

Sie veröffentlichen Ihre Assets auf Dynamic Media-Bildservern. Sie können Assets einmalig veröffentlichen oder veranlassen, dass Adobe Dynamic Media Classic Assets wiederholt veröffentlicht. Sobald die Assets veröffentlicht wurden, sind sie für Sie zur Bereitstellung verfügbar. Sie können die URL-Aufrufe aus Adobe Dynamic Media Classic kopieren und zu Ihrer Website oder Anwendung hinzufügen.

Adobe Dynamic Media Classic unterstützt jetzt die Bereitstellung aller Bilder und Videos über HTTP/2. Das heißt, eine veröffentlichte URL oder ein Einbettungs-Code für das Bild oder Video kann in jede Anwendung integriert werden, die ein gehostetes Asset akzeptiert. Dieses veröffentlichte Asset verwendet das HTTP/2-Protokoll, um es bereitzustellen. Diese Bereitstellungsmethode verbessert die Kommunikation zwischen Browsern und Servern und ermöglicht schnellere Antwort- und Ladezeiten für alle Adobe Dynamic Media Classic-Assets. Siehe [Häufig gestellte Fragen zur Bereitstellung von Inhalten über HTTP/2](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/http2).

## Nach dem Hochladen veröffentlichen {#publish-after-uploading}

Assets befinden sich entweder in einem veröffentlichten oder unveröffentlichten Status. Standardmäßig werden alle Assets, die Sie in Adobe Dynamic Media Classic hochladen, automatisch zur Veröffentlichung markiert.

Weitere Informationen finden Sie auf der [Instant Publish Notification PDF](/help/using/assets/rendering-instant-publish-notification.pdf).

Verwenden Sie diese Verfahren, um Assets zur Veröffentlichung zu markieren:

* **[!UICONTROL Publish nach dem Hochladen]**: Wählen Sie auf der Seite „Hochladen“ unten **[!UICONTROL Publish nach dem Hochladen]** aus. Die Standardeinstellung ist „ausgewählt“.

* **[!UICONTROL Publish nach dem Hochladen]**: Wählen Sie im Dialogfeld „Auftragsoptionen“ die Option **[!UICONTROL Publish nach dem Hochladen]**. Die Standardeinstellung ist „ausgewählt“.

Einige abgeleitete Assets werden automatisch zur Veröffentlichung markiert, wenn ihre Stammelemente zur Veröffentlichung markiert werden. In dieser Tabelle werden untergeordnete Assets aufgelistet, die automatisch zur Veröffentlichung markiert sind.

| Übergeordnetes Element (Gruppe) | Untergeordnete Elemente (Mitglieder) |
| --- | --- |
| Bildsätze | Die Bilder in einem Satz. |
| Mustersets | Die Farbfelder in einem Satz. |
| Rotationssets | Die Bilder in einem Satz. |
| Vorlagen | Vorlagendateien, Seiten und Bilder. |

Abgeleitete Bilder werden ebenfalls automatisch zur Veröffentlichung markiert, wenn ihre übergeordneten Bilder veröffentlicht werden. Abgeleitete Bilder sind beispielsweise Bilder, die Sie mit Bildbearbeitungsoptionen angepasst haben. Sie können diese abgeleiteten Bilder in der Detailansicht unter „Built &amp; Derivatives“ anzeigen.

## Erstellen eines Veröffentlichungsauftrags {#creating-a-publish-job}

Erstellen Sie einen Veröffentlichungsauftrag, um Assets zu veröffentlichen, die Sie auf Adobe Dynamic Media Classic-Server hochgeladen haben, die aber noch nicht automatisch veröffentlicht werden sollen. Sie können einen einmaligen Veröffentlichungsauftrag ausführen oder Aufträge so planen, dass sie regelmäßig wiederholt werden. Adobe Dynamic Media Classic bietet erweiterte Veröffentlichungsoptionen für die Veröffentlichung auf bestimmten Servern sowie Optionen für die erneute Veröffentlichung von bereits veröffentlichten Assets.

**So erstellen Sie einen Veröffentlichungsauftrag:**

1. Wählen Sie in der globalen Navigationsleiste **[!UICONTROL Publish]**.
1. Wählen Sie im Dialogfeld „Veröffentlichen“ aus, ob Sie einen einmaligen oder einen wiederkehrenden Veröffentlichungsauftrag wünschen.

   Siehe [Erstellen eines einmaligen Veröffentlichungsauftrags](publishing-files.md#creating_a_one_time_publish_job) und [Erstellen eines wiederkehrenden Veröffentlichungsauftrags](publishing-files.md#creating_a_recurring_publish_job).

1. Geben Sie einen Auftragsnamen ein.
1. Blenden Sie optional die erweiterten Optionen ein und legen Sie die gewünschten Einstellungen fest. 

   Siehe [Erweiterte Veröffentlichungsoptionen](publishing-files.md#advanced_publish_options).

1. Wählen Sie **[!UICONTROL Publish senden]** aus.

Adobe Dynamic Media Classic verfolgt Veröffentlichungsaufträge auf der Seite „Aufträge“. Sie können Veröffentlichungsaufträge auf dieser Seite überprüfen.

>[!NOTE]
>
>Assets, die Sie erneut veröffentlicht haben (Sie haben sie bereits veröffentlicht), wird aufgrund des Web-Caching-Mechanismus im Content Delivery Network (CDN) nicht sofort auf Ihrer Website angezeigt. Siehe [Erneut veröffentlichte Assets und CDN-Verzögerungen](publishing-files.md#republished_assets_and_cdn_delays).

### Erstellen eines einmaligen Veröffentlichungsauftrags {#creating-a-one-time-publish-job}

Erstellen Sie einen einmaligen Veröffentlichungsauftrag, indem Sie die Option **[!UICONTROL Einmal]** auf der Seite „Veröffentlichen“ auswählen.

Wenn der Veröffentlichungsauftrag später ausgeführt werden soll, wählen Sie auf der Seite „Veröffentlichen“ die Option **[!UICONTROL Einmal]** aus. Wählen Sie aus der Dropdown-Liste **[!UICONTROL Für später planen]** aus. Wählen Sie mit dem Kalender und dem Zeitschieber einen Tag und eine Uhrzeit für die Ausführung des Veröffentlichungsauftrags aus.

### Erstellen wiederkehrender Veröffentlichungsaufträge {#creating-a-recurring-publish-job}

Erstellen Sie einen wiederkehrenden Veröffentlichungsauftrag, indem Sie **[!UICONTROL Wiederkehrend]** auf der Seite „Veröffentlichen“ auswählen.

Wählen Sie dann die Wiederholungsoption **[!UICONTROL Täglich]**, **[!UICONTROL Wöchentlich]**, **[!UICONTROL Monatlich]** oder **[!UICONTROL Benutzerdefiniert]** und geben Sie an, wann der Veröffentlichungsauftrag wiederholt werden soll. Adobe Dynamic Media Classic bietet Kalendertools für die Planung des wiederkehrenden Veröffentlichungsauftrags. Sie können die Option **[!UICONTROL Benutzerdefiniert]** auswählen und eine Regel in das Textfeld „Regel“ eingeben, um ein benutzerdefiniertes Auftragsintervall zu beschreiben.

Siehe [Erstellen eines benutzerdefinierten Zeitintervalls für Uploads oder Veröffentlichungsaufträge](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>Wiederkehrende Veröffentlichungsaufträge (und Upload-Aufträge) werden auf der Seite „Aufträge“ aufgelistet. Wenn Sie einen geplanten Auftrag bearbeiten oder löschen möchten, wählen Sie auf der Seite „Aufträge“ die Registerkarte „Geplant“ aus.

### Erweiterte Veröffentlichungsoptionen {#advanced-publish-options}

Sie können die erweiterten Optionen auf der Seite „Veröffentlichen“ anzeigen und die folgenden Optionen für die Verarbeitung eines Veröffentlichungsauftrags auswählen:

* **[!UICONTROL Publish an]**: Wählen Sie einen Servertyp aus, um Assets nur auf einem bestimmten Server zu veröffentlichen.

* **[!UICONTROL Publish]**: Standardmäßig veröffentlicht Adobe Dynamic Media Classic nur Assets, die neu sind und zuvor noch nicht veröffentlicht wurden (die Option Neu seit letzter Publish). Sie können jedoch **[!UICONTROL Vollständige Publish]** auswählen, damit Sie auch Assets veröffentlichen können, die seit der letzten Veröffentlichung aktualisiert oder geändert wurden. Wählen Sie **[!UICONTROL Vollständig mit Suchdaten]**, wenn Sie einen E-Katalog veröffentlichen und möchten, dass die Leser ihn nach Keyword durchsuchen können.

* **[!UICONTROL Auftrag ausführen als]**: Wählen Sie einen Benutzernamen aus der Liste aus. Auf der Seite „Aufträge“ können Aufträge nach Benutzername sortiert werden. Durch die Auswahl eines Namens verknüpfen Sie einen Veröffentlichungsauftrag mit einem Benutzer.

**[!UICONTROL HTTP-Benachrichtigung]**: Geben Sie eine URL ein, um nachfolgende Veröffentlichungsaufträge in den Trigger aufzunehmen.

Siehe [Verwenden eines Upload- oder Veröffentlichungsauftrags als Trigger ](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Abbrechen von Veröffentlichungsaufträgen {#canceling-a-publish-job}

Sie können einen laufenden Veröffentlichungsauftrag abbrechen. Als Administrator können Sie einen in Verarbeitung befindlichen Veröffentlichungsauftrag auch über die Seite „Aufträge“ für das Unternehmen stornieren.

Um einen Veröffentlichungsauftrag abzubrechen, gehen Sie zur Seite „Aufträge“ und klicken Sie auf **[!UICONTROL Abbrechen]**. Auf der Registerkarte Geplant auf der Seite Aufträge können Sie einen Auftrag anhalten oder fortsetzen, indem Sie das Kontrollkästchen in der Spalte Aktiv des Auftrags deaktivieren oder aktivieren.

>[!NOTE]
>
>Nachdem Sie einen Veröffentlichungsauftrag abgebrochen haben, ändert sich sein Status in „Wird gestoppt“, bis der Auftrag einen Punkt erreicht hat, an dem er sicher gestoppt werden kann. Das Anhalten eines Veröffentlichungsauftrags kann einige Zeit in Anspruch nehmen, wenn der Auftrag gerade Daten aus der Datenbank abruft.

## Publish-Assets manuell {#manually-publishing-assets}

Sie können einzelne Assets manuell veröffentlichen, anstatt einen Veröffentlichungsauftrag zu erstellen. Beim Veröffentlichen von Sets, z. B. eines Bildsets oder eines adaptiven Videosets, werden das Set (oder „übergeordnete“ Elemente) und alle Mitglieder (oder „untergeordneten“ Elemente„) innerhalb dieses Sets veröffentlicht.

Nicht veröffentlichte Assets werden in der Benutzeroberfläche durch ein graues, rundes Symbol mit einem Schrägstrich (unveröffentlichter Status) links neben dem Asset-Namen gekennzeichnet. Nach dem Veröffentlichen eines Assets ändert sich das Symbol in ein grünes Kreissymbol mit einem weißen Häkchen (Status „veröffentlicht“).

**So veröffentlichen Sie Assets manuell:**

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Assets aus.

     Wechseln Sie in der globalen Navigationsleiste zu **[!UICONTROL Datei]** > **[!UICONTROL Publish]**.

   * Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht das graue, runde Symbol mit einem Schrägstrich links neben dem Asset-Namen aus.

## Manuelles Rückgängigmachen der Veröffentlichung von Assets {#manually-unpublishing-assets}

Sie können die Veröffentlichung einzelner Assets manuell rückgängig machen. Wenn Sie die Veröffentlichung von Sets aufheben, z. B. eines Mustersets oder eines E-Katalogs, wechselt das Set (oder „übergeordnete„) selbst in einen unveröffentlichten Status. Die Mitglieder (oder „untergeordneten Elemente„) in diesem Set sind jedoch nicht betroffen. Stattdessen behalten sie jeweils ihren vorhandenen Status „Veröffentlicht“ oder „Unveröffentlicht“ bei.

Veröffentlichte Assets werden in der Benutzeroberfläche durch ein rundes, grünes Symbol mit einem weißen Häkchen in der Mitte (Veröffentlichungsstatus) links neben dem Asset-Namen gekennzeichnet. Nachdem die Veröffentlichung eines Assets rückgängig gemacht wurde, wird das Symbol grau mit einem Schrägstrich (unveröffentlichter Status).

**So heben Sie die Veröffentlichung von Assets manuell auf:**

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere veröffentlichte Assets aus.

     Navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Datei]** > **[!UICONTROL Veröffentlichung aufheben]**.

   * Klicken Sie in der Rasteransicht, Listenansicht oder Detailansicht links neben dem Asset-Namen auf das runde, grüne Häkchensymbol.

## Abrufen des Veröffentlichungsverlaufs eines Assets {#getting-an-asset-s-publish-history}

Das letzte Datum, an dem ein Asset veröffentlicht wurde, wird in der Detailansicht oben im Bedienfeld angezeigt. Weitere Informationen zum Veröffentlichungsverlauf finden Sie, indem Sie das Bedienfeld Verlauf und Veröffentlichungs-Server in der Detailansicht öffnen. Dort wird angezeigt, wann und auf welchen Servern das Asset veröffentlicht wurde.

## Erneut veröffentlichte Assets und CDN-Verzögerungen {#republished-assets-and-cdn-delays}

Adobe Dynamic Media Classic-Assets werden im Content Delivery Network (CDN) verteilt. CDN ist ein System von vernetzten Computer-Servern, die auf transparente Weise zusammenarbeiten, um Inhalte – insbesondere umfangreiche Medieninhalte – für Endbenutzer bereitzustellen. Im CDN-System werden Web-Inhalte in Web-Caches im Internet gespeichert (das so genannte Edge-Cache-Netzwerk). Web-Inhalte werden von den Web-Caches an die Endbenutzer bereitgestellt, um schnellere Sendungen zu ermöglichen.

Wenn jemand zum ersten Mal eine Web-Seite herunterlädt, werden die Assets an einen CDN-Web-Cache-Server bereitgestellt. Dieser Server speichert sie, sodass derselbe zwischengespeicherte Inhalt schneller bereitgestellt wird, wenn das nächste Mal eine Person in demselben Bereich auf die Web-Seite zugreift. Die Inhaltsbereitstellung erfolgt schneller, weil der Inhalt näher beim Endbenutzer aufbewahrt wird. CDN sorgt für eine schnellere Anzeige von Web-Seiten. Die Bandbreitenanforderungen an den zentralen Server werden verringert, da die Inhalte über das Edge-Cache-Netzwerk bereitgestellt werden, nicht jedes Mal von einem zentralen Server aus.

Neu veröffentlichte Adobe Dynamic Media Classic-Inhalte sind für den Endbenutzer sofort verfügbar und füllen das Edge-Cache-Netzwerk schnell auf. Neu veröffentlichte Inhalte, d. h. Bilder mit denselben Namen wie zuvor auf einem Bildserver veröffentlichte Bilder, werden jedoch bis zu zehn Stunden lang nicht im CDN aktualisiert. Stattdessen sehen Endbenutzer, was sich in einem Web-Cache im CDN-Netzwerk befindet. Aus diesem Grund werden Ihre erneut veröffentlichten Adobe Dynamic Media Classic-Assets Endbenutzern zehn Stunden lang nicht angezeigt.

Wenn Sie möchten, dass Ihre neu veröffentlichten Bild-Assets früher als nach der zehnstündigen Verzögerung verfügbar sind, können Sie Web-Caches im CDN leeren. Wenn diese Web-Caches bereinigt werden, werden alte Inhalte aus den CDN-Web-Caches entfernt und durch die zuletzt veröffentlichten Assets ersetzt.

Um den Cache zu leeren, gehen Sie in der globalen Navigationsleiste zu **[!UICONTROL Datei]** > **[!UICONTROL CDN-Invalidierung]**. Alle ausgewählten Dateien werden aus dem Cache entfernt. Wenn keine veröffentlichbare Assets vorhanden oder Sie kein Unternehmensadministrator sind, ist die CDN-Option „Entfernen“ nicht verfügbar.

>[!MORELIKETHIS]
>
>* [Überprüfen Sie die Auftragsdateien](checking-job-files.md)
>* [Wiederkehrende Aufträge bearbeiten, löschen, anhalten und fortsetzen](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)
