---
title: Überprüfen von Auftragsdateien
description: Erfahren Sie, wie Sie Auftragsdateien in Adobe Dynamic Media Classic überprüfen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
topic: Administration, Content Management
level: Intermediate
source-git-commit: bb229047c0c9b3855453ea15dcd1f9754bc65cef
workflow-type: tm+mt
source-wordcount: '1622'
ht-degree: 23%

---

# Überprüfen von Auftragsdateien{#checking-job-files}

Zur Überwachung von Datei-Uploads in Adobe Dynamic Media Classic und von Dateien, die Sie auf Adobe Dynamic Media Classic-Servern veröffentlichen, bietet Adobe Dynamic Media Classic die Seite &quot;Aufträge&quot;. Sie können Aufträge auf der Seite &quot;Aufträge&quot;überprüfen, hochladen und veröffentlichen, den Status von Aufträgen überprüfen und Veröffentlichungsaufträge von dieser Seite aus abbrechen. Sie können außerdem Termine für die Ausführung von Upload-Aufträgen und Veröffentlichungsaufträgen planen.

Wenn Sie Assets hochladen, wird neben dem Menü „Aufträge“ die Anzahl der verarbeiteten Dateien sowie ein rotierendes Symbol angezeigt, das darauf hinweist, dass derzeit ein Auftrag verarbeitet wird. Sie können das Symbol auswählen, um weitere Informationen zum aktiven Auftrag anzuzeigen.

>[!NOTE]
>
>Eine Liste der kürzlich veröffentlichten Aufträge steht auch auf der Seite „Jüngste Aktivitäten“ zur Verfügung. Wählen Sie **[!UICONTROL Zuletzt verwendet]** in der Symbolleiste für globale Navigation aus.

## Seite „Aufträge“ {#about-the-jobs-page}

Wählen Sie **[!UICONTROL Aufträge]** in der Leiste &quot;Globale Navigation&quot;aus, damit die Seite &quot;Aufträge&quot;geöffnet wird. Standardmäßig werden die neuesten Aufträge oben in der Liste angezeigt.

Auf der Registerkarte „Verlauf“ der Seite „Aufträge“ werden die Aufträge nach folgenden Kategorien angezeigt:

* **[!UICONTROL Auftragstyp]**: Ein Symbol zeigt den Auftragstyp an: Hochladen und Publish sind die häufigsten Auftragstypen.

* **[!UICONTROL Auftragsname]**: Der Name des Auftrags. Der Name enthält den vom Benutzer eingegebenen Teil des Namens sowie Datum und Uhrzeit.

* **[!UICONTROL Gestartet]**: Der Zeitpunkt, zu dem der Auftrag gestartet wurde.

* **[!UICONTROL Gesamt]**: Die Anzahl der übertragenen Dateien.

* **[!UICONTROL W (Warnungen)]**: Die Anzahl der Warnungen im Auftrag (falls vorhanden). Warnmeldungen weisen auf Probleme mit dem Auftrag hin, die eine Ausführung des Auftrags insgesamt nicht beeinträchtigen. Die Warnmeldungen können normalerweise ignoriert werden, da sie auf ausgeblendete Dateien hinweisen. Beispielsweise enthalten die Dateien &quot;`.DS_store`&quot;(Mac) und &quot;Thumbs.db&quot;(Windows®) Informationen darüber, wie Bilddateien für Benutzer angezeigt werden. Warneinträge zu diesen Dateien können jedoch ignoriert werden, da sie sich nicht darauf beziehen, wie diese Dateien in Adobe Dynamic Media Classic verwendet werden. Sie können auf einen Auftragsnamen doppelklicken, um detaillierte Informationen über Warnungen abzurufen.

* **[!UICONTROL E (errors)]**: Listet die Anzahl der Fehler im Auftrag auf (falls vorhanden). Sie können auf einen Auftragsnamen doppelklicken, um detaillierte Informationen über Fehler abzurufen.

* **[!UICONTROL Dauer]**: Wie lange es dauerte, den Auftrag abzuschließen.

* **[!UICONTROL Status]**: Zeigt den Status des Auftrags an.

* **[!UICONTROL Ziel]**: Bei Upload-Aufträgen ist das Ziel der Unternehmensname und der Ordner, in den die Dateien hochgeladen wurden. Diese Kategorie gilt nicht für Aufträge zur Veröffentlichung.

* **[!UICONTROL Gesendet von]**: Listen, die die Assets hochgeladen haben.

>[!NOTE]
>
>Sie können laufende Veröffentlichungs- und Upload-Aufträge abbrechen, indem Sie neben der Fortschrittsleiste die Schaltfläche **[!UICONTROL Abbrechen]** auswählen.

## Ansichten auf der Seite &quot;Aufträge&quot;ändern {#changing-views-on-the-jobs-page}

Mit den folgenden Verfahren können Sie Aufträge sortieren oder die Ansicht der Registerkarte „Verlauf“ auf der Seite „Aufträge“ ändern:

* **[!UICONTROL Sortierung]**: Wählen Sie einen Spaltennamen aus, um die Liste nach einer bestimmten Spalte zu sortieren. Durch Klicken auf den Schalter neben dem Spaltennamen können Sie zwischen auf- und absteigender Sortierfolge wechseln.

* **[!UICONTROL Datumsbereich]**: Wählen Sie das Menü **[!UICONTROL Datumsbereich]** aus und wählen Sie eine Option, um die Liste der Aufträge auf das aktuelle Datum, die vorherige Woche oder den vorherigen Monat einzuschränken. Wählen Sie **[!UICONTROL Benutzerdefinierter Datumsbereich]** aus und geben Sie dann einen bestimmten Datumsbereich ein.

* **[!UICONTROL Auftragstyp]**: Wählen Sie im Menü **[!UICONTROL Auftragstyp]** die Option **[!UICONTROL Publish]** oder **[!UICONTROL Upload]** aus, um die Liste auf Veröffentlichungsaufträge oder Upload-Aufträge zu beschränken. Wählen Sie **[!UICONTROL Alle]** aus, um beide Auftragstypen anzuzeigen.

* **[!UICONTROL Anzeigen]**: Wechseln Sie zu **[!UICONTROL Anzeigen]** > **[!UICONTROL Meine Aufträge]** oder **[!UICONTROL Anzeigen]** > **[!UICONTROL Alle Aufträge]** , um die Liste auf Aufträge zu beschränken, die Sie bestellt haben, oder auf Aufträge, die von Personen in Ihrem Unternehmen bestellt wurden.

## Anzeigen, Kopieren oder Drucken eines Berichts &quot;Auftragsdetails&quot; {#viewing-copying-or-printing-a-job-details-report}

Doppelklicken Sie auf der Seite &quot;Aufträge&quot;auf den Namen eines Berichts, damit die Seite &quot;Auftragsdetails&quot;geöffnet wird. Auf dieser Seite werden die im Auftrag enthaltenen Dateien aufgelistet. Wählen Sie **[!UICONTROL Detail anzeigen]** aus, damit Sie die Adobe Dynamic Media Classic-ID, den Zielpfad und Statusinformationen eines Eintrags sehen können. Wenn Sie eine PDF- oder PostScript-Datei hochgeladen haben, für die Schriftarten erforderlich sind, die in Adobe Dynamic Media Classic nicht verfügbar sind, werden im Bericht die fehlenden Schriftarten aufgelistet.

Sie können diese Informationen in die Zwischenablage kopieren.

1. Doppelklicken Sie auf der Seite &quot;Aufträge&quot;auf den Namen eines Berichts.
1. Wählen Sie auf der Seite &quot;Auftragsdetails&quot;die Option **[!UICONTROL Details anzeigen]** aus, um einen detaillierten Bericht über einen Eintrag zu erhalten.
1. Wählen Sie **[!UICONTROL In Zwischenablage kopieren]** aus.

## Verarbeiten wiederkehrender Upload- und Veröffentlichungsaufträge {#handling-recurring-upload-and-publish-jobs}

Wiederkehrende Upload- und Veröffentlichungsaufträge, die Sie auf den Seiten &quot;Hochladen&quot;und &quot;Publish&quot;erstellen, werden auf der Registerkarte &quot;Geplant&quot;der Seite &quot;Aufträge&quot;aufgeführt. Sie können wiederkehrende Aufträge auf der Registerkarte „Geplant“ bearbeiten und löschen.

Wählen Sie in der Symbolleiste für globale Navigation die Schaltfläche &quot;Aufträge&quot;und wählen Sie auf der Seite &quot;Aufträge&quot;die Registerkarte **[!UICONTROL Geplant]** aus, damit Sie wiederkehrende Aufträge bearbeiten und löschen können.

>[!NOTE]
>
>Sie können die Auftragsliste auf der Registerkarte **[!UICONTROL Geplant]** mit den Menüs **[!UICONTROL Auftragstyp]** und **[!UICONTROL Anzeigen]** filtern. Wählen Sie einen Auftragstyp aus, damit Sie die Liste auf Veröffentlichungsaufträge eines bestimmten Typs eingrenzen können. Wählen Sie die Option **[!UICONTROL Anzeigen]** aus, damit Sie von Ihnen erstellte Aufträge oder Aufträge, die von allen Benutzern in Ihrem Unternehmen erstellt wurden, anzeigen können.

### Bearbeiten, Löschen, Anhalten und Fortsetzen wiederkehrender Aufträge {#editing-deleting-pausing-and-resuming-recurring-jobs}

Wählen Sie auf der Seite &quot;Aufträge&quot;einen wiederkehrenden Auftrag aus und befolgen Sie die folgenden Anweisungen, wenn Sie ihn bearbeiten oder löschen möchten:

* **Einen wiederkehrenden Auftrag bearbeiten**: Wählen Sie die Schaltfläche **[!UICONTROL Bearbeiten]** aus und geben Sie im Dialogfeld &quot;Geplanten Auftrag bearbeiten&quot;Planungsinformationen ein. Wenn der Auftrag in einem Intervall Ihrer Wahl wiederholt werden soll, gehen Sie zu **[!UICONTROL Wiederholen]** > **[!UICONTROL Benutzerdefiniert]**.

Siehe [Erstellen eines benutzerdefinierten Zeitintervalls für Upload- oder Veröffentlichungsaufträge](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **Löschen eines wiederkehrenden Auftrags**: Wählen Sie die Schaltfläche **[!UICONTROL Löschen]** aus.

* **Anhalten (und Wiederaufnehmen) eines wiederkehrenden Auftrags**: Heben Sie in der Spalte Aktiv das Kontrollkästchen auf, um einen Auftrag anzuhalten. Aktivieren Sie ein Kontrollkästchen, um einen angehaltenen Auftrag wieder aufzunehmen.

### Benutzerdefiniertes Upload- oder Veröffentlichungsauftragszeitintervall erstellen {#creating-a-custom-upload-or-publish-job-time-interval}

Um ein benutzerdefiniertes Zeitintervall für einen Upload-Auftrag (über FTP) oder einen Veröffentlichungsauftrag zu erstellen, gehen Sie auf der Seite &quot;Hochladen&quot;oder &quot;Publish&quot;zu **[!UICONTROL Wiederholen]** > **[!UICONTROL Benutzerdefiniert]**. Geben Sie dann im Feld Regel Zahlen und Platzhalter ein, die ein Zeitintervall für die wiederkehrenden Upload- oder Veröffentlichungsaufträge beschreiben.

Dies ist die Syntax zum Beschreiben benutzerdefinierter Zeitintervalle für Upload-Aufträge bzw. Veröffentlichungsaufträge im Feld „Regel“:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Beispielsweise plant `0 15 10 * * ?` einen Auftrag jeden Tag um 10:15.00 Uhr.

In den folgenden Tabellen und in der Liste unten ist dargestellt, wie sich ein Zeitintervall in das Feld „Regel“ eingeben lässt.

Diese Tabelle enthält Informationen zu den Zeitabschnitten, den jeweils zulässigen Werten und den unterstützten Platzhaltern:

| Zeitabschnitte | Zulässige Werte | Kommentare | Unterstützte Platzhalter |
|--- |--- |--- |--- |
| Sekunden | 0-59 |  | `,: * /` |
| Minuten | 0-59 |  | `,: * /` |
| Stunden | 0-23 | Beachten Sie die Verwendung des 24-Stunden-Formats. | `,: * /` |
| Tag des Monats | 1-31 | Es ist nicht möglich, einen numerischen Wert sowohl für &quot;Tag des Monats&quot;als auch für &quot;Tag der Woche&quot;anzugeben. Eines dieser Felder muss ein Platzhalterzeichen `?` verwenden. | `,: * / ? L C` |
| Monat | 1 bis 12 oder Jan, Feb, Mär, Apr, Mai, Jun, Jul, Aug, Sep, Okt, Nov, Dez | Bei Werten wird zwischen Groß- und Kleinschreibung unterschieden. | `,: * /` |
| Wochentag | Mo, Di, Mi, Do, Fr, Sa, So | Bei Werten wird zwischen Groß- und Kleinschreibung unterschieden. Es ist nicht möglich, einen numerischen Wert sowohl für &quot;Tag des Monats&quot;als auch für &quot;Tag der Woche&quot;anzugeben. Eines dieser Felder muss ein Platzhalterzeichen `?` verwenden. | `,: * / ? L C #` |
| Jahr (optional) | Leer oder 1970-2099 |  | `,: * /` |


In dieser Tabelle sind die im Feld „Regel“ zulässigen Platzhalterzeichen mit Nutzungshinweisen aufgeführt:

| Platzhalterzeichen | Name | Beschreibung |
| --- | --- | --- |
| `*` | Sternchen | Alle Werte (beispielsweise &quot;jede Minute&quot;). |
| `?` | Fragezeichen | Kein bestimmter Wert (z. B. &quot;beliebige Minute innerhalb der angegebenen Stunde&quot;). |
| `,` | Komma | Andere Werte (beispielsweise &quot;Montag und Mittwoch&quot;). |
| `-` | Trennstrich | Wertebereich (beispielsweise &quot;Montag bis Freitag&quot;). |
| `/` | Schrägstrich | Erhöhungen (z. B. &quot;alle 15 Minuten&quot;). |
| `L` | Großes L | Letzter &quot;Tag des Monats&quot;oder &quot;Tag der Woche&quot;(nur für diese Felder verfügbar). Wenn der Monat beispielsweise der Januar ist, wird der Auftrag mit dem Wert L für das Feld &quot;Tag des Monats&quot;für den 31. Januar geplant. Für das Feld &quot;Wochentag&quot;können Sie dieses Zeichen allein eingeben, um den Auftrag am Samstag zu planen. Sie können ihn mit einer Zahl (z. B. `6L`) verwenden, um den letzten Freitag des Monats anzugeben. Geben Sie &quot;`L`&quot;nicht mit den Platzhaltern Komma oder Bindestrich an. |
| `#` | Zeichen für „Nr.“ | Nter Wochentag des Monats (nur für das Feld &quot;Wochentag&quot;verfügbar). Beispielsweise gibt `6#3` im Feld &quot;Wochentag&quot;den dritten Freitag des Monats an. Die `6` bedeutet &quot;Freitag&quot;(der sechste Tag der Woche) und die `3` geben das dritte Vorkommen im Monat an. |
| `C` | Großes K | Erster Kalender &quot;Tag des Monats&quot;oder &quot;Tag der Woche&quot;(nur für diese Felder verfügbar). Wenn Sie beispielsweise den Wert &quot;`1C`&quot;für &quot;Tag des Monats&quot;angeben, wird der erste Tag im Kalender geplant, der am oder nach dem fünften Tag eintritt. Für das Feld &quot;Wochentag&quot;wird durch Angabe von `1C` der erste Tag im Kalender geplant, der am oder nach Sonntag stattfindet. |

Diese Liste enthält Beispiele zur Beschreibung von Zeitintervallen im Feld „Regel“:

* `0 0 12 * * ?` : Nicht jeden Tag
* `0 15 10 ? * *` : 10:15 Uhr jeden Tages
* `0 0/5 14 * * ?`: Alle 5 Minuten zwischen 14:00 und 14:55 Uhr täglich
* `0 0/5 14,18 * * ?` : Jeden Tag alle 5 Minuten zwischen 14:00 und 14:55 Uhr und alle 5 Minuten zwischen 18:00 und 18:55 Uhr
* `0 10,44 14 ? 3` : Mi jeden Mittwoch im März um 14:10 Uhr und 14:44 Uhr
* `0 15 10 ? *` : Montag bis Freitag um 10:15 Uhr jeden Wochentag
* `0 15 10 20 * ?` : Um 10:15 Uhr am 20. Tag jedes Monats
* `0 15 10 L * ?` : Um 10:15 Uhr am letzten Tag jedes Monats
* `0 15 10 ? * 6L` : Um 10:15 Uhr am letzten Freitag jedes Monats
* `0 15 10 * * 6#3` : Um 10:15 Uhr am dritten Freitag jedes Monats

## Upload- oder Veröffentlichungsauftrag als Trigger verwenden {#using-an-upload-or-publish-job-as-a-trigger}

Wenn Sie Assets über FTP hochladen oder einen Veröffentlichungsauftrag ausführen, können Sie einen nachfolgenden Auftrag planen, der nach Abschluss des Uploads beginnt. (Wenn dann andere Aufträge geplant sind, wird der hier geplante Auftrag hinter ihnen in die Warteschlange gestellt.) Der neue Auftrag sendet eine Benachrichtigung an die von Ihnen angegebene Adresse, damit der Code an dieser Stelle ausgelöst werden kann. Der nachfolgende Upload-Auftrag erhält denselben Namen wie der aktuelle Upload-Auftrag, jedoch mit dem Präfix „_Pub“.

Um einen Upload- oder Veröffentlichungsauftrag-Trigger in einen anderen Auftrag zu versetzen, wählen Sie auf der Seite &quot;Hochladen&quot;oder &quot;Publish&quot;die Option **[!UICONTROL Erweitert]** aus. Geben Sie dann die URL in das Textfeld „HTTP-Benachrichtigung“ ein.
