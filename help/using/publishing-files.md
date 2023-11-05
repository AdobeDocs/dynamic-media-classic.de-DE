---
title: Veröffentlichen von Dateien
description: "Erfahren Sie, wie Sie Ihre Assets auf Dynamic Media-Image-Servern veröffentlichen. Sie können Assets einmalig veröffentlichen oder dafür sorgen, dass Adobe Dynamic Media Classic Assets regelmäßig veröffentlicht. Sobald die Assets veröffentlicht wurden, sind sie für Sie zur Bereitstellung verfügbar. Sie können die URL-Aufrufe aus Adobe Dynamic Media Classic kopieren und zu Ihrer Website oder Anwendung hinzufügen."
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
topic: Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '1732'
ht-degree: 37%

---

# Veröffentlichen von Dateien{#publishing-files}

Sie veröffentlichen Ihre Assets auf Dynamic Media-Image-Servern. Sie können Assets einmalig veröffentlichen oder dafür sorgen, dass Adobe Dynamic Media Classic Assets regelmäßig veröffentlicht. Sobald die Assets veröffentlicht wurden, sind sie für Sie zur Bereitstellung verfügbar. Sie können die URL-Aufrufe aus Adobe Dynamic Media Classic kopieren und zu Ihrer Website oder Anwendung hinzufügen.

Adobe Dynamic Media Classic unterstützt jetzt die Bereitstellung aller Bilder und Videos über HTTP/2. Das heißt, dass eine veröffentlichte URL oder ein Einbettungscode für das Bild oder Video verfügbar ist, um in jede Anwendung integriert zu werden, die ein gehostetes Asset akzeptiert. Das veröffentlichte Asset wird dann über das HTTP/2-Protokoll bereitgestellt. Diese Bereitstellungsmethode verbessert die Kommunikation von Browsern und Servern, sodass die Antwort- und Ladezeiten aller Adobe Dynamic Media Classic-Assets verbessert werden. Siehe [Häufig gestellte Fragen zur Bereitstellung von Inhalt über HTTP/2](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/http2.html#dynamic).

## Nach dem Hochladen veröffentlichen {#publish-after-uploading}

Assets befinden sich entweder in einem veröffentlichten oder unveröffentlichten Status. Standardmäßig werden alle Assets, die Sie in Adobe Dynamic Media Classic hochladen, automatisch zur Veröffentlichung markiert.

Weitere Informationen finden Sie unter [Sofortige PDF zur Veröffentlichung](/help/using/assets/rendering-instant-publish-notification.pdf).

Sie haben zum Markieren von Assets zur Veröffentlichung die folgenden Möglichkeiten:

* **[!UICONTROL Nach dem Hochladen veröffentlichen]** - Wählen Sie auf der Seite Hochladen unten die Option **[!UICONTROL Nach dem Hochladen veröffentlichen]**. Die Standardeinstellung ist „ausgewählt“.

* **[!UICONTROL Nach dem Hochladen veröffentlichen]** - Wählen Sie im Dialogfeld &quot;Auftragsoptionen&quot;die Option **[!UICONTROL Nach dem Hochladen veröffentlichen]**. Die Standardeinstellung ist „ausgewählt“.

Einige abgeleitete Assets werden automatisch zur Veröffentlichung markiert, wenn ihre Stammelemente zur Veröffentlichung markiert werden. In der folgenden Tabelle sind die Arten von abgeleiteten Assets aufgeführt, die automatisch zur Veröffentlichung markiert werden.

| Übergeordnetes Element (Gruppe) | Untergeordnete Elemente (Mitglieder) |
| --- | --- |
| Bildsätze | Die Bilder in einem Satz. |
| Mustersets | Die Farbfelder in einem Satz. |
| Rotationssets | Die Bilder in einem Satz. |
| Vorlagen | Vorlagendateien, Seiten und Bilder. |

Abgeleitete Bilder werden zur Veröffentlichung markiert, wenn die zugehörigen Stammbilder veröffentlicht werden. Abgeleitete Bilder sind beispielsweise Bilder, die Sie mit Bildbearbeitungsoptionen angepasst haben. Sie können diese abgeleiteten Bilder in der Detailansicht unter &quot;Built &amp; Derivatives&quot;anzeigen.

## Veröffentlichungsauftrag erstellen {#creating-a-publish-job}

Erstellen Sie einen Veröffentlichungsauftrag, um Assets zu veröffentlichen, die Sie auf Adobe Dynamic Media Classic-Server hochgeladen haben, aber noch nicht automatisch veröffentlichen möchten. Sie können einen einmaligen Veröffentlichungsauftrag ausführen oder Aufträge planen, die regelmäßig wiederholt werden. Adobe Dynamic Media Classic bietet erweiterte Veröffentlichungsoptionen für die Veröffentlichung auf bestimmten Servern und Optionen zum erneuten Veröffentlichen von Assets, die bereits veröffentlicht wurden.

**So erstellen Sie einen Veröffentlichungsauftrag:**

1. Wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Veröffentlichen]**.
1. Wählen Sie im Dialogfeld „Veröffentlichen“ aus, ob Sie einen einmaligen oder einen wiederkehrenden Auftrag veröffentlichen möchten.

   Siehe [Erstellen eines einmaligen Veröffentlichungsauftrags](publishing-files.md#creating_a_one_time_publish_job) und [Wiederkehrenden Veröffentlichungsauftrag erstellen](publishing-files.md#creating_a_recurring_publish_job).

1. Geben Sie einen Auftragsnamen ein.
1. Blenden Sie optional die erweiterten Optionen ein und legen Sie die gewünschten Einstellungen fest. 

   Siehe [Erweiterte Veröffentlichungsoptionen](publishing-files.md#advanced_publish_options).

1. Auswählen **[!UICONTROL Veröffentlichen senden]**.

Adobe Dynamic Media Classic verfolgt Veröffentlichungsaufträge auf der Seite &quot;Aufträge&quot;nach. Sie können Veröffentlichungsaufträge auf dieser Seite überprüfen.

>[!NOTE]
>
>Assets, die Sie erneut veröffentlichen (Sie haben sie bereits veröffentlicht), werden aufgrund des Web-Caching-Mechanismus im Inhaltsbereitstellungsnetzwerk (Content Delivery Network, CDN) nicht sofort auf Ihrer Website angezeigt. Siehe [Erneut veröffentlichte Assets und CDN-Verzögerungen](publishing-files.md#republished_assets_and_cdn_delays).

### Erstellen eines einmaligen Veröffentlichungsauftrags {#creating-a-one-time-publish-job}

Erstellen Sie einen einmaligen Veröffentlichungsauftrag, indem Sie die **[!UICONTROL Einmalig]** auf der Seite Veröffentlichen .

Wenn der Veröffentlichungsauftrag später ausgeführt werden soll, wählen Sie auf der Seite Veröffentlichen die Option **[!UICONTROL Einmalig]**, wählen Sie **[!UICONTROL Für später einplanen]** aus der Dropdown-Liste. Verwenden Sie den Kalender und den Zeitregler, um einen Tag und eine Uhrzeit für die Ausführung des Veröffentlichungsauftrags auszuwählen.

### Wiederkehrenden Veröffentlichungsauftrag erstellen {#creating-a-recurring-publish-job}

Erstellen eines wiederkehrenden Veröffentlichungsauftrags durch Auswahl von **[!UICONTROL Wiederkehrend]** auf der Seite &quot;Veröffentlichen&quot;.

Wählen Sie anschließend die Option Wiederholen aus. **[!UICONTROL Täglich]**, **[!UICONTROL Wöchentlich]**, **[!UICONTROL Monatlich]** oder **[!UICONTROL Benutzerdefiniert]** und geben Sie an, wann der Veröffentlichungsauftrag wiederholt werden soll. Adobe Dynamic Media Classic bietet Kalendertools zur Planung des wiederkehrenden Veröffentlichungsauftrags. Sie können **[!UICONTROL Benutzerdefiniert]** und geben Sie eine Regel in das Textfeld Regel ein, um ein benutzerdefiniertes Auftragsintervall zu beschreiben.

Siehe [Benutzerdefiniertes Upload- oder Veröffentlichungsauftragszeitintervall erstellen](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>Wiederkehrende Veröffentlichungsaufträge (und Upload-Aufträge) werden auf der Seite „Aufträge“ aufgelistet. Wenn Sie einen geplanten Auftrag bearbeiten oder löschen möchten, wählen Sie auf der Seite „Aufträge“ die Registerkarte „Geplant“ aus.

### Erweiterte Veröffentlichungsoptionen {#advanced-publish-options}

Sie können auf der Seite „Veröffentlichen“ erweiterte Optionen anzeigen und damit Einstellungen für einen Veröffentlichungsauftrag festlegen:

* **[!UICONTROL Veröffentlichen in]** - Wenn Sie Assets nur auf einem bestimmten Server veröffentlichen möchten, wählen Sie einen Servertyp aus.

* **[!UICONTROL Veröffentlichen]** - Standardmäßig veröffentlicht Adobe Dynamic Media Classic nur Assets, die neu sind und noch nicht veröffentlicht wurden (Option &quot;Neu seit letzter Veröffentlichung&quot;). Sie können jedoch **[!UICONTROL Vollständige Veröffentlichung]** , um auch Assets zu veröffentlichen, die seit der letzten Veröffentlichung aktualisiert oder geändert wurden. Auswählen **[!UICONTROL Vollständig mit Suchdaten]** Wenn Sie einen E-Katalog veröffentlichen und möchten, dass die Leser ihn mit einem Schlüsselwort durchsuchen können.

* **[!UICONTROL Auftrag ausführen als]** - Wählen Sie einen Benutzernamen aus der Liste aus. Auf der Seite „Aufträge“ können Aufträge nach Benutzername sortiert werden. Durch Wählen eines Namens verbinden Sie einen Veröffentlichungsauftrag mit einem Benutzer.

**[!UICONTROL HTTP-Benachrichtigung]** - Geben Sie eine URL zum Trigger nachfolgender Veröffentlichungsaufträge ein.

Siehe [Upload- oder Veröffentlichungsauftrag als Trigger verwenden](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).

## Veröffentlichungsauftrag abbrechen {#canceling-a-publish-job}

Sie können einen laufenden Veröffentlichungsauftrag abbrechen. Als Administrator können Sie einen in Verarbeitung befindlichen Veröffentlichungsauftrag auch über die Seite „Aufträge“ für das Unternehmen stornieren.

Um einen Veröffentlichungsauftrag abzubrechen, gehen Sie zur Seite &quot;Aufträge&quot;und wählen Sie **[!UICONTROL Abbrechen]**. Auf der Registerkarte &quot;Geplant&quot;der Seite &quot;Aufträge&quot;können Sie einen Auftrag anhalten oder fortsetzen, indem Sie in der Spalte &quot;Aktiv&quot;des Auftrags das Kontrollkästchen deaktivieren oder aktivieren.

>[!NOTE]
>
>Nachdem Sie einen Veröffentlichungsauftrag abgebrochen haben, erhält er den Status &quot;Anhalten&quot;, bis der Auftrag einen Punkt erreicht hat, an dem er sicher anhalten kann. Bis zum Anhalten eines Veröffentlichungsauftrags kann es einige Zeit dauern, wenn gerade Daten aus der Datenbank abgerufen werden.

## Assets manuell veröffentlichen {#manually-publishing-assets}

Sie können einzelne Assets manuell veröffentlichen, anstatt einen Veröffentlichungsauftrag zu erstellen. Wenn Sie Sets veröffentlichen, z. B. ein Bildset oder ein adaptives Videoset, werden das Set (oder &quot;übergeordnetes Element&quot;) und alle Mitglieder (oder &quot;untergeordnete Elemente&quot;) innerhalb dieses Sets veröffentlicht.

Nicht veröffentlichte Assets werden in der Benutzeroberfläche durch ein graues, rundes Symbol mit einem Schrägstrich (Status &quot;Nicht veröffentlicht&quot;) links neben dem Asset-Namen angezeigt. Nach dem Veröffentlichen eines Assets ändert sich das Symbol in ein grünes Kreissymbol mit einem weißen Häkchen (Status „veröffentlicht“).

**So veröffentlichen Sie Assets manuell:**

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Assets aus.

     Wechseln Sie in der Leiste Globale Navigation zu **[!UICONTROL Datei]** > **[!UICONTROL Veröffentlichen]**.

   * Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht das graue, runde Symbol mit einem Schrägstrich links neben dem Asset-Namen aus.

## Veröffentlichung von Assets manuell rückgängig machen {#manually-unpublishing-assets}

Sie können die Veröffentlichung einzelner Assets manuell rückgängig machen. Wenn Sie die Veröffentlichung von Sets, z. B. eines Mustersets oder eines E-Katalogs, rückgängig machen, erhält das Set (oder &quot;übergeordnetes&quot;) selbst den Status &quot;unveröffentlicht&quot;. Die Mitglieder (oder &quot;untergeordneten Elemente&quot;) in diesem Satz sind jedoch nicht betroffen. Stattdessen behalten sie ihren vorhandenen Status veröffentlicht oder unveröffentlicht bei.

Veröffentlichte Assets werden in der Benutzeroberfläche durch ein rundes, grünes Symbol mit einem weißen Häkchen in der Mitte (Veröffentlichungsstatus) links neben dem Asset-Namen gekennzeichnet. Nachdem die Veröffentlichung eines Assets rückgängig gemacht wurde, wird das Symbol grau mit einem Schrägstrich (Status &quot;Nicht veröffentlicht&quot;) dargestellt.

**So machen Sie die Veröffentlichung eines Assets manuell rückgängig:**

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere veröffentlichte Assets aus.

     Wechseln Sie in der Leiste Globale Navigation zu **[!UICONTROL Datei]** > **[!UICONTROL Veröffentlichung rückgängig machen]**.

   * Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht das runde grüne Häkchensymbol links neben dem Asset-Namen aus.

## Abrufen des Veröffentlichungsverlaufs eines Assets {#getting-an-asset-s-publish-history}

Das letzte Datum, an dem ein Asset veröffentlicht wurde, wird in der Detailansicht oben im Bedienfeld angezeigt. Weitere Informationen zum Veröffentlichungsverlauf erhalten Sie, indem Sie das Bedienfeld Verlauf und veröffentlichte Server in der Detailansicht öffnen. Dort wird angezeigt, wann und auf welchen Servern das Asset veröffentlicht wurde.

## Erneut veröffentlichte Assets und CDN-Verzögerungen {#republished-assets-and-cdn-delays}

Adobe Dynamic Media Classic-Assets werden im Content Delivery Network (CDN) verteilt. CDN ist ein System von vernetzten Computer-Servern, die auf transparente Weise zusammenarbeiten, um Inhalte – insbesondere umfangreiche Medieninhalte – für Endbenutzer bereitzustellen. Im CDN-System werden Web-Inhalte in Web-Caches gespeichert, die über das Internet verteilt sind (das so genannte Edge-Cache-Netzwerk). Web-Inhalte werden von den Web-Caches an Endbenutzer gesendet, um schnellere Sendungen zu ermöglichen.

Wenn ein Benutzer eine Website zum ersten Mal herunterlädt, werden die Assets an einen CDN-Web-Cache-Server übertragen und auf diesem Server gespeichert. Beim nächsten Abruf der Website von einem Benutzer in derselben geografischen Region kann der im Cache gespeicherte Inhalt schneller bereitgestellt werden. Die Inhaltsbereitstellung erfolgt schneller, weil der Inhalt näher beim Endbenutzer aufbewahrt wird. CDN ermöglicht eine schnellere Anzeige von Websites. Die Bandbreitenanforderungen an den zentralen Server werden verringert, da die Inhalte über das Edge-Cache-Netzwerk bereitgestellt werden, nicht jedes Mal von einem zentralen Server aus.

Neu veröffentlichte Adobe Dynamic Media Classic-Inhalte stehen dem Endbenutzer sofort zur Verfügung und füllen das Edge-Cache-Netzwerk schnell. Neue erneut veröffentlichte Inhalte – etwa Bilder mit identischen Namen wie zuvor auf einem Image-Server veröffentlichte Bilder – werden im CDN jedoch bis zu zehn Stunden lang nicht aktualisiert. Endbenutzer sehen stattdessen die Daten im Web-Cache des CDN. Aus diesem Grund werden die erneut veröffentlichten Adobe Dynamic Media Classic-Assets den Endbenutzern zehn Stunden lang nicht angezeigt.

Wenn Sie möchten, dass neue erneut veröffentlichte Bild-Assets schneller zur Verfügung stehen als mit zehnstündiger Verzögerung, können Sie Web-Caches im CDN bereinigen. Bei der Bereinigung der Web-Caches werden alte Inhalte aus den CDN-Web-Caches entfernt und durch die zuletzt veröffentlichten Assets ersetzt.

Um den Cache zu leeren, navigieren Sie in der Leiste Globale Navigation zu **[!UICONTROL Datei]** > **[!UICONTROL Ungültiges CDN]**. Alle ausgewählten Dateien werden aus dem Cache entfernt. Wenn keine veröffentlichbare Assets vorhanden oder Sie kein Unternehmensadministrator sind, ist die CDN-Option „Entfernen“ nicht verfügbar.

>[!MORELIKETHIS]
>
>* [Überprüfen von Auftragsdateien](checking-job-files.md)
>* [Bearbeiten, Löschen, Anhalten und Fortsetzen wiederkehrender Aufträge](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)
