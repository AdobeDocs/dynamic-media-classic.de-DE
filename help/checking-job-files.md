---
title: Überprüfen von Auftragsdateien
seo-title: Überprüfen von Auftragsdateien
description: 'null'
seo-description: Erfahren Sie, wie Sie Auftragsdateien überprüfen.
uuid: 8241 a 894-3014-4 a 5 c -96 ef -71 f 3 aaa 3716 a
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/upload_ and_ publish_ assets
discoiquuid: d 53 ae 5 dd -8 daf -4 d 87-b 9 a 6-3039 negativ 30538
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Überprüfen von Auftragsdateien{#checking-job-files}

Zum Überwachen von Datei-Uploads in das Scene 7 Publishing System und von Dateien, die Sie auf dynamischen Media Classic-Servern veröffentlichen, bietet SPS die Seite "Aufträge" an. Sie haben auf der Seite „Aufträge“ die Möglichkeit, Upload-Aufträge und Veröffentlichungsaufträge zu überprüfen, den Status von Aufträgen zu ermitteln und Veröffentlichungsaufträge zu stornieren. Sie können außerdem Termine für die Ausführung von Upload-Aufträgen und Veröffentlichungsaufträgen planen.

Wenn Sie Assets hochladen, wird neben dem Menü „Aufträge“ die Anzahl der verarbeiteten Dateien sowie ein rotierendes Symbol angezeigt, das darauf hinweist, dass derzeit ein Auftrag verarbeitet wird. Sie können auf das Symbol klicken, um weitere Informationen zum aktiven Auftrag anzuzeigen.

>[!NOTE]
>
>Eine Liste der kürzlich veröffentlichten Aufträge steht auch auf der Seite „Jüngste Aktivitäten“ zur Verfügung. Klicken Sie in der Symbolleiste für globale Navigation auf „Kürzlich“, um diese Seite zu öffnen.

## Seite „Aufträge“ {#about-the-jobs-page}

Klicken Sie auf der Symbolleiste für globale Navigation auf die Schaltfläche „Aufträge“, um die Seite „Aufträge“ zu öffnen. Standardmäßig werden die neuesten Aufträge oben in der Liste angezeigt.

Auf der Registerkarte „Verlauf“ der Seite „Aufträge“ werden die Aufträge nach folgenden Kategorien angezeigt:

**Auftragstyp** Ein Symbol gibt den Auftragstyp an: Upload und Veröffentlichung sind die häufigsten Auftragstypen.

**Auftragsname** Der Name des Auftrags. Enthalten sind der vom Benutzer eingegebene Teil des Namens und der Datums-/Zeitstempel.

**Begann** , wenn der Auftrag gestartet wurde.

**Gesamtanzahl** der übertragenen Dateien.

**W (Warnungen)** Die Anzahl der Warnmeldungen im Auftrag (falls vorhanden). Warnmeldungen weisen auf Probleme mit dem Auftrag hin, die eine Ausführung des Auftrags insgesamt nicht beeinträchtigen. Die Warnmeldungen können normalerweise ignoriert werden, da sie auf ausgeblendete Dateien hinweisen. Beispiele sind etwa die Dateien „.DS_store“ (Macintosh) und „Thumbs.db“ (Windows), die Informationen über das Anzeigen von Bilddateien für Nutzer enthalten. Warneinträge zu diesen Dateien können ignoriert werden, da sie nicht daran interessiert sind, wie diese Dateien in Dynamic Media Classic verwendet werden. Sie können auf einen Auftragsnamen doppelklicken, um detaillierte Informationen über Warnungen abzurufen.

**E (Fehler)** Gibt die Anzahl der Fehler im Auftrag an (falls vorhanden). Sie können auf einen Auftragsnamen doppelklicken, um detaillierte Informationen über Fehler abzurufen.

**Dauer** der Fertigstellung des Auftrags.

**Status** zeigt den Status des Auftrags an.

**Ziel** für Upload-Aufträge: Der Unternehmensname und Ordner, in den die Dateien hochgeladen wurden. Bei Veröffentlichungsaufträgen kommt diese Kategorie nicht vor.

**Gesendet von** Listen, die die Assets hochgeladen haben.

***Hinweis**: Sie können in Verarbeitung befindliche Veröffentlichungs- und Upload-Aufträge abbrechen, indem Sie neben der Fortschrittsleiste auf die Schaltfläche "Abbrechen" klicken.*

## Ändern von Ansichten auf der Seite „Aufträge“{#changing-views-on-the-jobs-page}

Mit den folgenden Verfahren können Sie Aufträge sortieren oder die Ansicht der Registerkarte „Verlauf“ auf der Seite „Aufträge“ ändern:

**Sortieren** Sie einen Spaltennamen, um die Liste nach einer bestimmten Spalte zu sortieren. Durch Klicken auf den Schalter neben dem Spaltennamen können Sie zwischen auf- und absteigender Sortierfolge wechseln.

**Datumsbereich** Wählen Sie das Menü Datumsbereich und wählen Sie eine Option, um die Liste der Aufträge auf das aktuelle Datum, die vorherige Woche oder den vorherigen Monat einzugrenzen. Wählen Sie „Benutzerdefinierter Datumsbereich“, wenn Sie einen bestimmten Datumsbereich festlegen möchten.

**Auftragstyp** Wählen Sie das Menü "Auftragstyp" und wählen Sie Veröffentlichen oder Hochladen, um die Liste auf Veröffentlichungsaufträge oder Upload-Aufträge einzugrenzen. Wenn Sie „Alle“ wählen, werden beide Arten von Aufträgen angezeigt.

**Wählen Sie** "Anzeigen" &gt;" Meine Aufträge" oder "Anzeigen" &gt;" Alle Aufträge" , um die Liste auf Aufträge bzw. Aufträge zu beschränken, die Sie in Ihrem Unternehmen bestellt haben.

## Anzeigen, Kopieren oder Drucken eines Auftragsdetailberichts {#viewing-copying-or-printing-a-job-details-report}

Doppelklicken Sie auf der Seite „Aufträge“ auf den Namen eines Berichts, um die Seite „Auftragsdetails“ zu öffnen. Auf dieser Seite werden die im Auftrag enthaltenen Dateien aufgelistet. Klicken Sie auf „Detailansicht“, um die SPS-ID, den Zielpfad und Statusinformationen für einen Eintrag anzuzeigen. Wenn Sie eine PDF- oder PostScript-Datei hochgeladen haben, für die im SPS nicht verfügbare Schriftarten erforderlich sind, werden die fehlenden Schriftarten im Bericht aufgeführt.

Sie können diese Informationen in die Zwischenablage kopieren.

1. Doppelklicken Sie auf der Seite „Aufträge“ auf den Namen eines Berichts, um die Seite „Auftragsdetails“ zu öffnen. 
1. Klicken Sie auf „Detailansicht“, um einen detaillierten Bericht über einen Eintrag zu erhalten.
1. Klicken Sie auf „In Zwischenabl. kop.“.

## Umgang mit wiederkehrenden Upload-Aufträgen und Veröffentlichungsaufträgen {#handling-recurring-upload-and-publish-jobs}

Wiederkehrende Upload- und Veröffentlichungsaufträge, die Sie auf den Seiten „Hochladen“ und „Veröffentlichen“ erstellen, werden auf der Seite „Aufträge“ auf der Registerkarte „Geplant“ angezeigt. Sie können wiederkehrende Aufträge auf der Registerkarte „Geplant“ bearbeiten und löschen.

Klicken Sie auf der Symbolleiste für globale Navigation auf die Schaltfläche „Aufträge“. Wählen Sie auf der Seite „Aufträge“ die Registerkarte „Geplant“ aus, um wiederkehrende Aufträge bearbeiten und löschen zu können.

>[!NOTE]
>
>Sie können die Auftragsliste auf der Registerkarte „Geplant“ über die Menüs „Auftragstyp“ und „Anzeigen“ filtern. Wählen Sie einen Auftragstyp, um die Liste auf Veröffentlichungsaufträge einer bestimmten Art einzuschränken. Wählen Sie eine „Anzeigen“-Option, um entweder nur die von Ihnen erstellten Aufträge oder die Aufträge aller Mitarbeiter im Unternehmen anzuzeigen.

### Bearbeiten, Löschen, Anhalten und Wiederaufnehmen wiederkehrender Aufträge {#editing-deleting-pausing-and-resuming-recurring-jobs}

Sie können einen auf der Seite „Aufträge“ ausgewählten wiederkehrenden Auftrag mit den folgenden Verfahren bearbeiten bzw. löschen:

**Bearbeiten eines wiederkehrenden Auftrags** Klicken Sie auf "Bearbeiten" und geben Sie im Dialogfeld" Geplanten Auftrag bearbeiten" Planinformationen ein. Wenn Sie möchten, dass der Auftrag in einem Intervall Ihrer Wahl wiederholt ausgeführt wird, wählen Sie „Wiederholen“ &gt; „Benutzerdefiniert“. 

Siehe [Festlegen eines individuellen Zeitintervalls für Upload-Aufträge bzw. Veröffentlichungsaufträge](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

**Löschen eines wiederkehrenden Auftrags** Klicken Sie auf "Löschen" .

**Anhalten (und Wiederaufnehmen) eines wiederkehrenden Auftrags** In der Spalte Aktiv Deaktivieren Sie ein Kontrollkästchen, um einen Auftrag anzuhalten. Aktivieren Sie ein Kontrollkästchen, um einen angehaltenen Auftrag fortzusetzen.

### Festlegen eines individuellen Zeitintervalls für Upload-Aufträge bzw. Veröffentlichungsaufträge {#creating-a-custom-upload-or-publish-job-time-interval}

Wenn Sie ein benutzerdefiniertes Zeitintervall für einen Upload-Auftrag (per FTP) oder einen Veröffentlichungsauftrag festlegen möchten, wählen Sie auf der Seite „Hochladen“ bzw. „Veröffentlichen“ den Befehl „Wiederholen“ &gt; „Benutzerdefiniert“. Geben Sie dann Zahlen und Platzhalter in das Feld „Regel“ ein, um ein Zeitintervall für die wiederkehrenden Upload-Aufträge bzw. Veröffentlichungsaufträge festzulegen.

Dies ist die Syntax zum Beschreiben benutzerdefinierter Zeitintervalle für Upload-Aufträge bzw. Veröffentlichungsaufträge im Feld „Regel“:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

For example, `0 15 10 * * ?` schedules a job at 10:15.00 every day.

In den folgenden Tabellen und in der Liste unten ist dargestellt, wie sich ein Zeitintervall in das Feld „Regel“ eingeben lässt.

Diese Tabelle enthält Informationen zu den Zeitabschnitten, den jeweils zulässigen Werten und den unterstützten Platzhaltern:

| Zeitabschnitte | Zulässige Werte | Kommentare | Unterstützte Platzhalter |
|--- |--- |--- |--- |
| Sekunden | 0-59 |  | , - * / |
| Minuten | 0-59 |  | , - * / |
| Stunden | 0-23 | Beachten Sie die Verwendung des 24-Stunden-Formats. | , - * / |
| Tag des Monats | 1-31 | Es ist nicht möglich, sowohl für „Tag des Monats“ als auch für „Wochentag“ einen numerischen Wert festzulegen. Eines der beiden Felder muss ein Platzhalterzeichen ? enthalten. | , - * / ? L K |
| Monat | 1-12 oder Jan, Feb, Mar, Apr, May, Jun, Jul, Aug, Sep, Sep, Op, Nov, Dec | Bei den Werten wird zwischen Groß- und Kleinschreibung unterschieden. | , - * / |
| Wochentag | Mo, Di, Mi, Do, Fr, Sa, So | Bei den Werten wird zwischen Groß- und Kleinschreibung unterschieden. Es ist nicht möglich, sowohl für „Tag des Monats“ als auch für „Wochentag“ einen numerischen Wert festzulegen. Eines der beiden Felder muss ein Platzhalterzeichen ? enthalten. | , - * / ? L K # |
| Jahr (optional) | Leer oder 1970-2099 |  | , - * / |


In dieser Tabelle sind die im Feld „Regel“ zulässigen Platzhalterzeichen mit Nutzungshinweisen aufgeführt:

| Platzhalterzeichen | Name | Beschreibung |
|--- |--- |--- |
| * | Sternchen | Alle Werte (beispielsweise „jede Minute“). |
| ? | Fragezeichen | Kein bestimmter Wert (beispielsweise „jede Minute innerhalb der festgelegten Stunde“). |
| , | Komma | Zusätzliche Werte (beispielsweise „Montag und Mittwoch“). |
| - | Trennstrich | Wertebereich (beispielsweise „Montag bis Freitag“). |
| / | Schrägstrich | Abschnitte (z. B. „alle 15 Minuten“). |
| L | Großes L | Letzter „Tag des Monats“ bzw. „Wochentag“ (nur bei diesen Feldern verfügbar). Im Monat Januar würde der Wert „L“ für „Tag des Monats“ den Auftrag beispielsweise für den 31. Januar planen.Für das Feld „Wochentag“ kann das Zeichen allein eingegeben werden, um den Auftrag für Samstag zu planen. Sie können es mit einer Zahl (z. B. 6 L) verwenden, um den letzten Freitag des Monats anzugeben. Geben Sie L nicht mit dem Platzhalter für Komma oder Bindestrich an. |
| # | Zeichen für „Nr.“ | Der n-te Wochentag des Monats (nur beim Feld „Wochentag“ verfügbar).Beispielsweise würde mit 6#3 im Feld „Wochentag“ der dritte Freitag des Monats festgelegt werden. Die 6 steht für Freitag (sechster Tag der Woche), die 3 für das dritte Auftreten im Monat. |
| K | Großes K | Erster „Tag des Monats“ im Kalender bzw. erster „Wochentag“ im Kalender (nur bei diesen Feldern verfügbar). Wenn Sie z. B. einen Wert von 1 C für "Tag des Monats" festlegen, wird der erste Tag im Kalender am oder nach dem fünften eingeblendet. Für das Feld" Wochentag" wird der erste Tag im Kalender, der am Tag oder nach dem Sonntag eintritt, als "1 C" festgelegt. |

Diese Liste enthält Beispiele zur Beschreibung von Zeitintervallen im Feld „Regel“:

* 0 0 12 * * ?: Jeden Tag am Mittag
* 0 15 10 ? * *: 10:15 morgens an jedem Tag
* 0 0/5 14 * * ?: Alle 5 Minuten zwischen 14:00 und 14:55 Uhr an jedem Tag
* 0 0/5 14,18 * * ?: Alle 5 Minuten zwischen 14:00 und 14:55 Uhr an jedem Tag und alle 5 Minuten zwischen 18:00 und 18:55 Uhr an jedem Tag
* 0 10,44 14 ? 3: Mi um 14:10 Uhr sowie 14:44 Uhr jeden Mittwoch im März
* 0 15 10 ? *: Mo-Fr um 10:15 Uhr jeden Wochentag
* 0 15 10 20 * ?: Um 10:15 Uhr am 20. Tag jedes Monats
* 0 15 10 L * ?: Um 10:15 Uhr am letzten Tag jedes Monats
* 0 15 10 ? * 6L: Um 10:15 Uhr am letzten Freitag jedes Monats
* 0 15 10 * * 6#3: Um 10:15 Uhr am dritten Freitag jedes Monats

## Verwenden eines Upload-Auftrags oder Veröffentlichungsauftrags als Auslöser {#using-an-upload-or-publish-job-as-a-trigger}

Wenn Sie Assets per FTP hochladen oder einen Veröffentlichungsauftrag ausführen, können Sie einen Folgeauftrag unmittelbar nach Abschluss des Uploads beginnen lassen. (Wenn für diesen Zeitpunkt die Ausführung anderer Aufträge geplant ist, wird der hier terminierte Auftrag in der Warteschlange hinter diesen Aufträgen eingereiht.) Für den neuen Auftrag wird eine Benachrichtigung an die von Ihnen festgelegte Adresse geschickt, sodass Code am vorgesehenen Ort ausgelöst werden kann. Der nachfolgende Upload-Auftrag erhält denselben Namen wie der aktuelle Upload-Auftrag, jedoch mit dem Präfix „_Pub“.

Wenn ein Upload-Auftrag- oder Veröffentlichungsauftrag einen anderen Auftrag auslösen soll, wählen Sie auf der Seite „Hochladen“ oder „Veröffentlichen“ die Option „Erweitert“. Geben Sie dann die URL in das Textfeld „HTTP-Benachrichtigung“ ein.
