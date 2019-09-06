---
title: Veröffentlichen von Dateien
seo-title: Veröffentlichen von Dateien
description: 'null'
seo-description: Hier erfahren Sie, wie Sie Dateien veröffentlichen.
uuid: cdcf 519 b -4 c 1 e -430 b-b 43 a -2 f 20 f 75071 b 1
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/upload_ and_ publish_ assets
discoiquuid: 39099 bc 0-9228-46 f 0-9 bee -3542059 f 4695
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Veröffentlichen von Dateien{#publishing-files}

Sie veröffentlichen Ihre Assets auf dynamischen Medienservern. Sie können Assets einmalig veröffentlichen oder dynamische Medien Classic anordnen, um Assets regelmäßig zu veröffentlichen. Sobald die Assets veröffentlicht wurden, sind sie für Sie zur Bereitstellung verfügbar. Sie können die URL-Aufrufe aus dem Scene7 Publishing System kopieren und in Ihre Website bzw. Anwendung einfügen.

Scene 7 Publishing System unterstützt jetzt die Bereitstellung aller Bilder und Videos über HTTP/2. Das heißt, eine veröffentlichte URL oder ein Einbettungscode für das Bild oder Video ist zur Integration in eine Anwendung verfügbar, die ein gehostetes Asset akzeptiert. Dieses veröffentlichte Asset wird dann über das HTTP/2-Protokoll bereitgestellt. Diese Bereitstellungsmethode verbessert die Kommunikation zwischen Browsern und Servern und ermöglicht eine bessere Reaktion und Ladezeiten aller Assets Ihrer dynamischen Media Classic-Assets. Siehe [HTTP 2-Bereitstellung von Content FAQ](https://docs.adobe.com/content/docs/en/aem/6-2/administer/integration/marketing-cloud/scene7/http2faq.html).

## Nach dem Hochladen veröffentlichen {#publish-after-uploading}

Assets befinden sich entweder in einem veröffentlichten oder unveröffentlichten Status. Standardmäßig werden alle Assets, die Sie in Dynamic Media Classic hochladen, automatisch zur Veröffentlichung markiert.

Weitere Informationen finden Sie im [PDF-Dokument zur sofortigen Veröffentlichung](https://marketing.adobe.com/resources/help/en_US/s7/rendering-instant-publish-notification.pdf).

Sie haben zum Markieren von Assets zur Veröffentlichung die folgenden Möglichkeiten:

**Nach dem Hochladen** auf der Seite Hochladen unten wählen Sie Nach dem Hochladen veröffentlichen. Die Standardeinstellung ist „ausgewählt“.

**Nach dem Hochladen** im Dialogfeld "Auftragsoptionen" veröffentlichen wählen Sie" Nach dem Hochladen veröffentlichen" . Die Standardeinstellung ist „ausgewählt“.

Einige abgeleitete Assets werden automatisch zur Veröffentlichung markiert, wenn ihre Stammelemente zur Veröffentlichung markiert werden. In der folgenden Tabelle sind die Arten von abgeleiteten Assets aufgeführt, die automatisch zur Veröffentlichung markiert werden.

| Übergeordnetes Element (Gruppe) | Untergeordnete Elemente (Mitglieder) |
|--- |--- |
| Bildsätze | Die Bilder in einem Satz. |
| Mustersets | Die Farbfelder in einem Satz. |
| Rotationssets | Die Bilder in einem Satz. |
| Vorlagen | Vorlagendateien, Seiten und Bilder. |

Abgeleitete Bilder werden zur Veröffentlichung markiert, wenn die zugehörigen Stammbilder veröffentlicht werden. Abgeleitete Bilder sind beispielsweise Bilder, die Sie mit Bildbearbeitungsoptionen angepasst haben. In der Detailansicht werden diese abgeleiteten Bilder unter „Version und Ableitungen“ angezeigt.

## Erstellen eines Veröffentlichungsauftrags {#creating-a-publish-job}

Erstellen Sie einen Veröffentlichungsauftrag, um Assets zu veröffentlichen, die Sie auf dynamische Media Classic-Server hochgeladen haben, die aber noch nicht automatisch veröffentlicht werden. Sie können Veröffentlichungsaufträge entweder nur einmal ausführen oder eine regelmäßig wiederkehrende Ausführung einstellen. Dynamic Media Classic bietet erweiterte Veröffentlichungsoptionen für die Veröffentlichung auf bestimmten Servern und Optionen zum erneuten Veröffentlichen von Assets, die bereits veröffentlicht wurden.

**So erstellen Sie einen Veröffentlichungsauftrag**

1. Klicken Sie in der globalen Navigationsleiste auf **„Veröffentlichen“**.
1. Wählen Sie im Dialogfeld „Veröffentlichen“ aus, ob Sie einen einmaligen oder einen wiederkehrenden Auftrag veröffentlichen möchten.

   Siehe [Erstellen eines einmaligen Veröffentlichungsauftrags](publishing-files.md#creating_a_one_time_publish_job) und [Erstellen eines wiederkehrenden Veröffentlichungsauftrags](publishing-files.md#creating_a_recurring_publish_job).

1. Geben Sie einen Auftragsnamen ein.
1. Blenden Sie optional die erweiterten Optionen ein und legen Sie die gewünschten Einstellungen fest. 

   Siehe [Erweiterte Veröffentlichungsoptionen](publishing-files.md#advanced_publish_options).

1. Klicken Sie auf **Veröffentlichung**.

SPS erfasst Veröffentlichungsaufträge auf der Seite „Aufträge“. Sie können Veröffentlichungsaufträge auf dieser Seite überprüfen.

>[!NOTE]
>
>Assets, die Sie erneut publizieren (nachdem sie bereits veröffentlicht wurden), werden aufgrund des Web-Cache-Mechanismus im Netzwerk zur Inhaltsbereitstellung (Content Delivery Network, CDN) nicht sofort auf Ihrer Website angezeigt. Siehe [Erneut veröffentlichte Assets und CDN-Verzögerungen](publishing-files.md#republished_assets_and_cdn_delays).

### Erstellen eines einmaligen Veröffentlichungsauftrags {#creating-a-one-time-publish-job}

Sie erstellen einen einmaligen Veröffentlichungsauftrag, indem Sie auf der Seite „Veröffentlichen“ die Option „Einmalig“ auswählen.

Wenn der Veröffentlichungsauftrag zu einem späteren Zeitpunkt ausgeführt werden soll, wählen Sie im Menü „Wann“ die Option „Für späteren Termin einplanen“. Wählen Sie dann per Kalender und Uhrzeit-Regler einen Zeitpunkt für die Ausführung des Veröffentlichungsauftrags aus.

### Erstellen eines wiederkehrenden Veröffentlichungsauftrags {#creating-a-recurring-publish-job}

Sie erstellen einen wiederkehrenden Veröffentlichungsauftrag, indem Sie auf der Seite „Veröffentlichen“ die Option „Wiederkehrend“ aktivieren.

Bestimmen Sie dann durch Auswählen einer Option für „Wiederholen“ („Täglich“, „Wöchentlich“, „Monatlich“ oder „Benutzerdefiniert“) das Intervall für die Ausführung des Veröffentlichungsauftrags. Dynamic Media Classic enthält Kalenderwerkzeuge zum Planen des wiederkehrenden Veröffentlichungsauftrags. Sie können die Option „Benutzerdefiniert“ wählen und in das Feld „Regel“ eine Regel zur Beschreibung eines benutzerdefinierten Auftragsintervalls eingeben. 

Siehe [Festlegen eines individuellen Zeitintervalls für Upload-Aufträge bzw. Veröffentlichungsaufträge](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>Wiederkehrende Veröffentlichungsaufträge (und Upload-Aufträge) werden auf der Seite „Aufträge“ aufgelistet. Wenn Sie einen geplanten Auftrag bearbeiten oder löschen möchten, wählen Sie auf der Seite „Aufträge“ die Registerkarte „Geplant“ aus.

### Erweiterte Veröffentlichungsoptionen {#advanced-publish-options}

Sie können auf der Seite „Veröffentlichen“ erweiterte Optionen anzeigen und damit Einstellungen für einen Veröffentlichungsauftrag festlegen:

**Veröffentlichen, um** einen Servertyp auszuwählen, um Assets nur auf einem bestimmten Server zu veröffentlichen, nicht auf allen Servern.

**Standardmäßig veröffentlichen** , SPS veröffentlicht nur Assets, die neu sind und noch nicht veröffentlicht wurden (Option "Neu seit letzter Veröffentlichung" ). Sie können jedoch die Option „Vollständige Veröffentlichung“ wählen, um auch solche Assets zu veröffentlichen, die aktualisiert wurden oder seit der letzten Veröffentlichung verändert wurden. Wählen Sie „Vollständig mit Suchdaten“, wenn Sie einen E-Katalog veröffentlichen und den Lesern das Durchsuchen unter Verwendung von Suchbegriffen ermöglichen möchten.

**Auftrag ausführen als** Auswählen eines Benutzernamens in der Liste. Auf der Seite „Aufträge“ können Aufträge nach Benutzername sortiert werden. Durch Wählen eines Namens verbinden Sie einen Veröffentlichungsauftrag mit einem Benutzer.

**HTTP-Benachrichtigung** Geben Sie eine URL ein, um nachfolgende Veröffentlichungsaufträge auszulösen.

Siehe [Verwenden eines Upload-Auftrags oder Veröffentlichungsauftrags als Auslöser](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## Stornieren eines Veröffentlichungsauftrags {#canceling-a-publish-job}

Sie haben die Möglichkeit, einen in Verarbeitung befindlichen Veröffentlichungsauftrag zu stornieren. Als Administrator können Sie einen in Verarbeitung befindlichen Veröffentlichungsauftrag auch über die Seite „Aufträge“ für das Unternehmen stornieren.

Rufen Sie zum Stornieren eines Veröffentlichungsauftrags die Seite „Aufträge“ auf und klicken Sie auf „Abbrechen“. Auf der Registerkarte „Geplant“ der Seite „Aufträge“ können Sie einen Auftrag anhalten und wiederaufnehmen, indem Sie in der Spalte „Aktiv“ des Auftrags das Kontrollkästchen markieren bzw. dessen Markierung aufheben.

>[!NOTE]
>
>Wenn Sie einen Veröffentlichungsauftrag storniert haben, ändert sich dessen Status zu „Wird angehalten“, bis ein Punkt erreicht wird, an dem ein sicherer Abbruch möglich ist. Bis zum Anhalten eines Veröffentlichungsauftrags kann es einige Zeit dauern, wenn gerade Daten aus der Datenbank abgerufen werden.

## Manuelles Veröffentlichen von Assets {#manually-publishing-assets}

Sie können einzelne Assets manuell veröffentlichen, anstatt einen Veröffentlichungsauftrag zu erstellen. Beim Veröffentlichen eines Sets, z. B. eines Bildsatzes oder adaptiven Videosets, werden das Set (das übergeordnete Element) und alle Mitglieder (die untergeordneten Elemente) innerhalb des Sets veröffentlicht.

Unveröffentlichte Assets werden in der Benutzeroberfläche durch ein graues durchgestrichenes Kreissymbol gekennzeichnet (Status „unveröffentlicht“). Das Symbol wird links neben dem Namen des Assets angezeigt. Nach dem Veröffentlichen eines Assets ändert sich das Symbol in ein grünes Kreissymbol mit einem weißen Häkchen (Status „veröffentlicht“).

**So veröffentlichen Sie Assets manuell**

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere Assets aus.

      Klicken Sie in der globalen Navigationsleiste auf **Datei** &gt; **Veröffentlichen**.

   * Klicken Sie in der Rasteransicht, Listenansicht oder Detailansicht auf das graue durchgestrichene Kreissymbol, das links neben dem Namen des Assets angezeigt wird.

## Manuelles Rückgängigmachen der Veröffentlichung von Assets {#manually-unpublishing-assets}

Sie können die Veröffentlichung einzelner Assets manuell rückgängig machen. Beim Rückgängigmachen der Veröffentlichung eines Sets, z. B. eines Mustersets oder eines E-Katalogs, erhält das Set (das übergeordnete Element) den Status „unveröffentlicht“. Die Mitglieder (bzw. die untergeordneten Elemente) innerhalb des Sets sind davon jedoch nicht betroffen; sie behalten ihren jeweiligen Status „veröffentlicht“ oder „unveröffentlicht“ bei.

Veröffentlichte Elemente werden in der Benutzeroberfläche mit einem grünen Kreissymbol mit einem weißen Häkchen gekennzeichnet (Status „veröffentlicht“), das links neben dem Namen des Assets angezeigt wird. Nach dem Rückgängigmachen der Veröffentlichung eines Assets ändert sich das Symbol in ein graues durchgestrichenes Kreissymbol (Status „unveröffentlicht“).

**So machen Sie die Veröffentlichung eines Assets manuell rückgängig**

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht ein oder mehrere veröffentlichte Assets aus.

      Klicken Sie in der globalen Navigationsleiste auf **Datei** &gt; **Veröffentlichung rückgängigmachen**.

   * Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht auf das grüne Kreissymbol mit dem Häkchen, das links neben dem Namen des Assets angezeigt wird.

## Abrufen des Veröffentlichungsverlaufs für ein Asset {#getting-an-asset-s-publish-history}

In der Detailansicht wird oben im Bedienfeld das Datum angezeigt, an dem das Asset zuletzt veröffentlicht wurde. Sie können weitere Details zum Veröffentlichungsverlauf abrufen, indem Sie in der Detailansicht das Bedienfeld „Verlauf und Veröffentlichungsserver“ öffnen. Dort wird angezeigt, wann und auf welchen Servern das Asset veröffentlicht wurde.

## Erneut veröffentlichte Assets und CDN-Verzögerungen {#republished-assets-and-cdn-delays}

Dynamische Medien-Assets werden im Content Delivery Network (CDN) verteilt. CDN ist ein System von vernetzten Computer-Servern, die auf transparente Weise zusammenarbeiten, um Inhalte – insbesondere umfangreiche Medieninhalte – für Endbenutzer bereitzustellen. Im CDN-System werden Web-Inhalte in Web-Caches gespeichert, die über das Internet verteilt sind (das so genannte Edge-Cache-Netzwerk). Web-Inhalte werden von diesen Web-Caches an Endbenutzer ausgegeben, damit die Bereitstellung schneller erfolgt.

Wenn ein Benutzer eine Website zum ersten Mal herunterlädt, werden die Assets an einen CDN-Web-Cache-Server übertragen und auf diesem Server gespeichert. Beim nächsten Abruf der Website von einem Benutzer in derselben geografischen Region kann der im Cache gespeicherte Inhalt schneller bereitgestellt werden. Die Inhaltsbereitstellung erfolgt schneller, weil der Inhalt näher beim Endbenutzer aufbewahrt wird. CDN ermöglicht eine schnellere Anzeige von Websites. Die Bandbreitenanforderungen an den zentralen Server werden verringert, da die Inhalte über das Edge-Cache-Netzwerk bereitgestellt werden, nicht jedes Mal von einem zentralen Server aus.

Neu veröffentlichte Dynamic Media Classic-Inhalte stehen dem Endbenutzer sofort zur Verfügung und füllen schnell das Edge-Cache-Netzwerk. Neue erneut veröffentlichte Inhalte – etwa Bilder mit identischen Namen wie zuvor auf einem Image-Server veröffentlichte Bilder – werden im CDN jedoch bis zu zehn Stunden lang nicht aktualisiert. Endbenutzer sehen stattdessen die Daten im Web-Cache des CDN. Aus diesem Grund werden Ihre erneut veröffentlichten Assets von Dynamic Media Classic möglicherweise erst nach zehn Stunden für Endbenutzer angezeigt.

Wenn Sie möchten, dass neue erneut veröffentlichte Bild-Assets schneller zur Verfügung stehen als mit zehnstündiger Verzögerung, können Sie Web-Caches im CDN bereinigen. Bei der Bereinigung der Web-Caches werden alte Inhalte aus den CDN-Web-Caches entfernt und durch die zuletzt veröffentlichten Assets ersetzt.

Klicken Sie zum Bereinigen des Cache auf „Datei“ &gt; „Ungültiges CDN“. Alle ausgewählten Dateien werden aus dem Cache entfernt. Wenn keine veröffentlichbare Assets vorhanden oder Sie kein Unternehmensadministrator sind, ist die CDN-Option „Entfernen“ nicht verfügbar.

>[!MORELIKETHIS]
>
>* [Überprüfen von Auftragsdateien](checking-job-files.md)
>* [Bearbeiten, Löschen, Anhalten und Wiederaufnehmen wiederkehrender Aufträge](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)
