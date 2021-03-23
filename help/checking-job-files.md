---
title: Überprüfen von Auftragsdateien
description: Erfahren Sie, wie Auftragsdateien überprüft werden.
uuid: 8241a894-3014-4a5c-96ef-71f3aaa3716a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: d53ae5dd-8daf-4d87-b9a6-3039bad30538
feature: Dynamic Media Classic, Asset Management
role: Geschäftspraktiker
translation-type: tm+mt
source-git-commit: 3def4a02eda8dc36f2811b3d4f0e870fff1994e4
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 60%

---


# Überprüfen von Auftragsdateien{#checking-job-files}

Zur Überwachung von Datei-Uploads in Dynamic Media Classic und von Dateien, die Sie auf Dynamic Media Classic-Servern veröffentlichen, wird die Seite &quot;Aufträge&quot;von Dynamic Media Classic-Angeboten angezeigt. Sie haben auf der Seite „Aufträge“ die Möglichkeit, Upload-Aufträge und Veröffentlichungsaufträge zu überprüfen, den Status von Aufträgen zu ermitteln und Veröffentlichungsaufträge zu stornieren. Sie können außerdem Termine für die Ausführung von Upload-Aufträgen und Veröffentlichungsaufträgen planen.

Wenn Sie Assets hochladen, wird neben dem Menü „Aufträge“ die Anzahl der verarbeiteten Dateien sowie ein rotierendes Symbol angezeigt, das darauf hinweist, dass derzeit ein Auftrag verarbeitet wird. Sie können auf das Symbol klicken, um weitere Informationen zum aktiven Auftrag anzuzeigen.

>[!NOTE]
>
>Eine Liste der kürzlich veröffentlichten Aufträge steht auch auf der Seite „Jüngste Aktivitäten“ zur Verfügung. Klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Zuletzt verwendet, um diese Seite zu öffnen.]**

## Seite „Aufträge“{#about-the-jobs-page}

Wählen Sie in der Symbolleiste für globale Navigation **[!UICONTROL Aufträge]** aus, um die Seite &quot;Aufträge&quot;zu öffnen. Standardmäßig werden die neuesten Aufträge oben in der Liste angezeigt.

Auf der Registerkarte „Verlauf“ der Seite „Aufträge“ werden die Aufträge nach folgenden Kategorien angezeigt:

**AuftragstypEin Symbol** zeigt den Auftragstyp an: Hochladen und Veröffentlichen sind die häufigsten Auftragstypen.

**Auftragsname** Der Name des Auftrags. Der Name enthält den vom Benutzer eingegebenen Teil des Namens sowie das Datum und die Uhrzeit.

**** StartetBeim Starten des Auftrags.

**** GesamtsummeDie Anzahl der übertragenen Dateien.

**W (Warnungen)**  Die Anzahl der Warnungen im Auftrag (falls vorhanden). Warnmeldungen weisen auf Probleme mit dem Auftrag hin, die eine Ausführung des Auftrags insgesamt nicht beeinträchtigen. Die Warnmeldungen können normalerweise ignoriert werden, da sie auf ausgeblendete Dateien hinweisen. Beispielsweise enthalten die Dateien `.DS_store` (Macintosh) und Thumbs.db (Windows®) Informationen darüber, wie Bilddateien für Benutzer angezeigt werden. Warneinträge zu diesen Dateien können jedoch ignoriert werden, da sie sich nicht darauf beziehen, wie diese Dateien in Dynamic Media Classic verwendet werden. Sie können auf einen Auftragsnamen doppelklicken, um detaillierte Informationen über Warnungen abzurufen.

**E (Fehler)** Liste der Anzahl der Fehler im Auftrag (falls vorhanden). Sie können auf einen Auftragsnamen doppelklicken, um detaillierte Informationen über Fehler abzurufen.

**** DauerDauer des Auftrags.

**Status** Zeigt den Status des Auftrags an.

**** ZielBei Upload-Aufträgen: Name der Firma und , in die die Dateien hochgeladen wurden. Bei Veröffentlichungsaufträgen kommt diese Kategorie nicht vor.

**Gesendet** vonListen, die die Assets hochgeladen haben.

***Hinweis **: Sie können in Verarbeitung befindliche Veröffentlichungs- und Upload-Aufträge stornieren, indem Sie auf die Schaltfläche &quot;Abbrechen&quot;neben der Fortschrittsleiste klicken.*

## Ändern von Ansichten auf der Seite „Aufträge“{#changing-views-on-the-jobs-page}

Mit den folgenden Verfahren können Sie Aufträge sortieren oder die Ansicht der Registerkarte „Verlauf“ auf der Seite „Aufträge“ ändern:

**** SortierenWählen Sie einen Spaltennamen aus, um die Liste nach einer bestimmten Spalte zu sortieren. Durch Klicken auf den Schalter neben dem Spaltennamen können Sie zwischen auf- und absteigender Sortierfolge wechseln.

**Datumsbereich** Wählen Sie im Menü &quot;Datumsbereich&quot;eine Option aus, um die Liste von Aufträgen auf das aktuelle Datum, die vorherige Woche oder den vorherigen Monat einzuschränken. Wählen Sie &quot;Benutzerdefinierter Datumsbereich&quot;und geben Sie dann einen bestimmten Datumsbereich ein.

**AuftragstypWählen Sie** im Menü &quot;Auftragstyp&quot;die Option &quot;Veröffentlichen&quot;oder &quot;Hochladen&quot;, um die Liste auf Veröffentlichungsaufträge oder Upload-Aufträge zu beschränken. Wenn Sie „Alle“ wählen, werden beide Arten von Aufträgen angezeigt.

**Wählen Sie &quot;** Anzeigen&quot;> &quot;Meine Aufträge&quot;oder &quot;Anzeigen&quot;> &quot;Alle Aufträge&quot;, um die Liste auf die von Ihnen bestellten Aufträge oder Aufträge zu beschränken, die von den Mitarbeitern in Ihrer Firma bestellt wurden.

## Anzeigen, Kopieren oder Drucken eines Berichts mit Auftragsdetails {#viewing-copying-or-printing-a-job-details-report}

Doppelklicken Sie auf der Seite „Aufträge“ auf den Namen eines Berichts, um die Seite „Auftragsdetails“ zu öffnen. Auf dieser Seite werden die im Auftrag enthaltenen Dateien aufgelistet. Klicken Sie auf &quot;Ansichten-Details&quot;, um die Dynamic Media Classic-ID, den Zielpfad und Statusinformationen eines Eintrags anzuzeigen. Wenn Sie eine PDF- oder PostScript-Datei hochgeladen haben, für die Schriftarten erforderlich sind, die in Dynamic Media Classic nicht verfügbar sind, werden die fehlenden Schriftarten im Bericht Liste.

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

### Bearbeiten, Löschen, Anhalten und Wiederaufnehmen wiederkehrender Aufträge  {#editing-deleting-pausing-and-resuming-recurring-jobs}

Sie können einen auf der Seite „Aufträge“ ausgewählten wiederkehrenden Auftrag mit den folgenden Verfahren bearbeiten bzw. löschen:

**Bearbeiten eines wiederkehrenden** AuftragsKlicken Sie auf &quot;Bearbeiten&quot;und geben Sie im Dialogfeld &quot;Geplanten Auftrag bearbeiten&quot;Planungsinformationen ein. Wenn Sie möchten, dass der Auftrag in einem Intervall Ihrer Wahl wiederholt ausgeführt wird, wählen Sie „Wiederholen“ > „Benutzerdefiniert“. 

Siehe [Festlegen eines individuellen Zeitintervalls für Upload-Aufträge bzw. Veröffentlichungsaufträge](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

**Löschen eines wiederkehrenden** AuftragsKlicken Sie auf &quot;Löschen&quot;.

**Anhalten (und Wiederaufnehmen) eines wiederkehrenden** AuftragsDeaktivieren Sie in der Spalte Aktiv das Kontrollkästchen, um einen Auftrag anzuhalten. Aktivieren Sie ein Kontrollkästchen, um einen angehaltenen Auftrag wiederaufzunehmen.

### Festlegen eines individuellen Zeitintervalls für Upload-Aufträge bzw. Veröffentlichungsaufträge {#creating-a-custom-upload-or-publish-job-time-interval}

Wenn Sie ein benutzerdefiniertes Zeitintervall für einen Upload-Auftrag (per FTP) oder einen Veröffentlichungsauftrag festlegen möchten, wählen Sie auf der Seite „Hochladen“ bzw. „Veröffentlichen“ den Befehl „Wiederholen“ > „Benutzerdefiniert“. Geben Sie dann Zahlen und Platzhalter in das Feld „Regel“ ein, um ein Zeitintervall für die wiederkehrenden Upload-Aufträge bzw. Veröffentlichungsaufträge festzulegen.

Dies ist die Syntax zum Beschreiben benutzerdefinierter Zeitintervalle für Upload-Aufträge bzw. Veröffentlichungsaufträge im Feld „Regel“:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Beispiel: `0 15 10 * * ?` plant jeden Tag einen Auftrag um 10:15.00 Uhr.

In den folgenden Tabellen und in der Liste unten ist dargestellt, wie sich ein Zeitintervall in das Feld „Regel“ eingeben lässt.

Diese Tabelle enthält Informationen zu den Zeitabschnitten, den jeweils zulässigen Werten und den unterstützten Platzhaltern:

| Zeitabschnitte | Zulässige Werte | Kommentare | Unterstützte Platzhalter |
|--- |--- |--- |--- |
| Sekunden | 0-59 |  | `, - * /` |
| Minuten | 0-59 |  | `, - * /` |
| Stunden | 0-23 | Beachten Sie die Verwendung des 24-Stunden-Formats. | `, - * /` |
| Tag des Monats | 1-31 | Es ist nicht möglich, sowohl für „Tag des Monats“ als auch für „Wochentag“ einen numerischen Wert festzulegen. Eines dieser Felder muss ein Platzhalterzeichen `?` verwenden. | `, - * / ? L C` |
| Monat | 1-12 oder Jan, Feb, Mar, Apr, May, Jun, Jul, Aug, Sep, Sep, Okt, Nov, Dec | Bei den Werten wird zwischen Groß- und Kleinschreibung unterschieden. | `, - * /` |
| Wochentag | Mo, Di, Mi, Do, Fr, Sa, So | Bei den Werten wird zwischen Groß- und Kleinschreibung unterschieden. Es ist nicht möglich, sowohl für „Tag des Monats“ als auch für „Wochentag“ einen numerischen Wert festzulegen. Eines der beiden Felder muss ein Platzhalterzeichen ? enthalten. | `, - * / ? L C #` |
| Jahr (optional) | Leer oder 1970-2099 |  | `, - * /` |


In dieser Tabelle sind die im Feld „Regel“ zulässigen Platzhalterzeichen mit Nutzungshinweisen aufgeführt:

| Platzhalterzeichen | Name | Beschreibung |
|--- |--- |--- |
| `*` | Sternchen | Alle Werte (beispielsweise „jede Minute“). |
| `?` | Fragezeichen | Kein bestimmter Wert (beispielsweise „jede Minute innerhalb der festgelegten Stunde“). |
| `,` | Komma | Andere Werte (z. B. &quot;Montag und Mittwoch&quot;). |
| `-` | Trennstrich | Wertebereich (beispielsweise „Montag bis Freitag“). |
| `/` | Schrägstrich | Abschnitte (z. B. „alle 15 Minuten“). |
| `L` | Großes L | Letzter „Tag des Monats“ bzw. „Wochentag“ (nur bei diesen Feldern verfügbar). Im Monat Januar würde der Wert „L“ für „Tag des Monats“ den Auftrag beispielsweise für den 31. Januar planen. Für das Feld „Wochentag“ kann das Zeichen allein eingegeben werden, um den Auftrag für Samstag zu planen. Sie können ihn mit einer Zahl (z. B. `6L`) verwenden, um den letzten Freitag des Monats anzugeben. Geben Sie `L` nicht mit den Platzhaltern Komma oder Bindestrich an. |
| `#` | Zeichen für „Nr.“ | Der n-te Wochentag des Monats (nur beim Feld „Wochentag“ verfügbar). Beispiel: `6#3` im Feld &quot;Wochentag&quot;gibt den dritten Freitag des Monats an. Das `6` gibt &quot;Friday&quot;(sechster Tag der Woche) und das `3` das dritte Vorkommen im Monat an. |
| `C` | Großes K | Erster „Tag des Monats“ im Kalender bzw. erster „Wochentag“ im Kalender (nur bei diesen Feldern verfügbar). Wenn Sie beispielsweise den Wert `1C` für &quot;Tag des Monats&quot;angeben, wird der erste Tag im Kalender eingeplant, der am oder nach dem fünften Tag eintritt. Beim Festlegen von `1C` wird für das Feld &quot;Wochentag&quot;der erste Tag im Kalender am oder nach dem Sonntag eingeplant |

Diese Liste enthält Beispiele zur Beschreibung von Zeitintervallen im Feld „Regel“:

* 0 0 12 * * ?: Jeden Tag am Mittag
* 0 15 10 ? * *: 10:15 morgens an jedem Tag
* 0 0/5 14 * * ?: Alle 5 Minuten zwischen 14:00 und 14:55 Uhr an jedem Tag
* 0 0/5 14,18 * * ?: Alle 5 Minuten zwischen 14:00 und 14:55 Uhr an jedem Tag und alle 5 Minuten zwischen 18:00 und 18:55 Uhr an jedem Tag
* 0 10,44 14 ? 3: Mi um 14:10 Uhr sowie 14:44 Uhr jeden Mittwoch im März
* 0 15 10 ? *: Montag bis Freitag um 10:15 Uhr
* 0 15 10 20 * ?: Um 10:15 Uhr am 20. Tag jedes Monats
* 0 15 10 L * ?: Um 10:15 Uhr am letzten Tag jedes Monats
* 0 15 10 ? * 6L: Um 10:15 Uhr am letzten Freitag jedes Monats
* 0 15 10 * * 6#3: Um 10:15 Uhr am dritten Freitag jedes Monats

## Verwenden eines Upload-Auftrags oder Veröffentlichungsauftrags als Auslöser  {#using-an-upload-or-publish-job-as-a-trigger}

Wenn Sie Assets per FTP hochladen oder einen Veröffentlichungsauftrag ausführen, können Sie einen Folgeauftrag planen, der nach Abschluss des Uploads beginnt. (Wenn dann andere Aufträge beginnen sollen, wird der hier geplante Auftrag in der Warteschlange hinter ihnen liegen.) Für den neuen Auftrag wird eine Benachrichtigung an die von Ihnen festgelegte Adresse geschickt, sodass Code am vorgesehenen Ort ausgelöst werden kann. Der nachfolgende Upload-Auftrag erhält denselben Namen wie der aktuelle Upload-Auftrag, jedoch mit dem Präfix „_Pub“.

Wenn ein Upload-Auftrag- oder Veröffentlichungsauftrag einen anderen Auftrag auslösen soll, wählen Sie auf der Seite „Hochladen“ oder „Veröffentlichen“ die Option „Erweitert“. Geben Sie dann die URL in das Textfeld „HTTP-Benachrichtigung“ ein.
