---
title: Job-Dateien überprüfen
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
source-wordcount: '1633'
ht-degree: 23%

---

# Job-Dateien überprüfen{#checking-job-files}

Zur Überwachung von Datei-Uploads auf Adobe Dynamic Media Classic und von Dateien, die Sie auf Adobe Dynamic Media Classic-Servern veröffentlichen, bietet Adobe Dynamic Media Classic die Seite Vorgänge an. Sie können Aufträge auf der Seite „Aufträge“ überprüfen, hochladen und veröffentlichen, den Status von Aufträgen überprüfen und Veröffentlichungsaufträge auf dieser Seite abbrechen. Sie können außerdem Termine für die Ausführung von Upload-Aufträgen und Veröffentlichungsaufträgen planen.

Wenn Sie Assets hochladen, wird neben dem Menü „Aufträge“ die Anzahl der verarbeiteten Dateien sowie ein rotierendes Symbol angezeigt, das darauf hinweist, dass derzeit ein Auftrag verarbeitet wird. Sie können auf das Symbol klicken, um weitere Informationen über den aktiven Auftrag anzuzeigen.

>[!NOTE]
>
>Eine Liste der kürzlich veröffentlichten Aufträge steht auch auf der Seite „Jüngste Aktivitäten“ zur Verfügung. Wählen **[!UICONTROL in]** globalen Navigationsleiste „Zuletzt verwendet“ aus.

## Seite „Aufträge“ {#about-the-jobs-page}

Wählen Sie **[!UICONTROL Aufträge]** in der Symbolleiste für globale Navigation aus, sodass die Seite „Aufträge“ geöffnet wird. Standardmäßig werden die neuesten Aufträge oben in der Liste angezeigt.

Auf der Registerkarte „Verlauf“ der Seite „Aufträge“ werden die Aufträge nach folgenden Kategorien angezeigt:

* **[!UICONTROL Auftragstyp]**: Ein Symbol gibt den Auftragstyp an: Hochladen und Veröffentlichen sind die häufigsten Auftragstypen.

* **[!UICONTROL Vorgangsname]**: Der Name des Vorgangs. Der Name enthält den vom Benutzer eingegebenen Teil des Namens sowie das Datum und die Uhrzeit.

* **[!UICONTROL Gestartet]**: Zeitpunkt des Auftragsstarts.

* **[!UICONTROL Total]**: Die Anzahl der übertragenen Dateien.

* **[!UICONTROL W (Warnungen)]**: Die Anzahl der Warnungen im Auftrag (falls vorhanden). Warnmeldungen weisen auf Probleme mit dem Auftrag hin, die eine Ausführung des Auftrags insgesamt nicht beeinträchtigen. Die Warnmeldungen können normalerweise ignoriert werden, da sie auf ausgeblendete Dateien hinweisen. Beispielsweise enthalten `.DS_store`-Dateien (Mac) und Thumbs.db-Dateien (Windows®) Informationen zum Anzeigen von Bilddateien für Benutzerinnen und Benutzer. Warneinträge zu diesen Dateien können jedoch ignoriert werden, da sie sich nicht darauf beziehen, wie diese Dateien in Adobe Dynamic Media Classic verwendet werden. Sie können auf einen Auftragsnamen doppelklicken, um detaillierte Informationen über Warnungen abzurufen.

* **[!UICONTROL E (Fehler)]**: Listet die Anzahl der Fehler im Auftrag auf (falls vorhanden). Sie können auf einen Auftragsnamen doppelklicken, um detaillierte Informationen über Fehler abzurufen.

* **[!UICONTROL Dauer]**: Wie lange es dauerte, den Auftrag abzuschließen.

* **[!UICONTROL Status]**: Zeigt den Status des Auftrags an.

* **[!UICONTROL Ziel]**: Bei Upload-Aufträgen ist das Ziel der Firmenname und der Ordner, in den die Dateien hochgeladen wurden. Diese Kategorie gilt nicht für Aufträge zur Veröffentlichung.

* **[!UICONTROL Gesendet von]**: Listet auf, wer die Assets hochgeladen hat.

>[!NOTE]
>
>Sie können laufende Veröffentlichungs- und Upload-Aufträge abbrechen, indem Sie auf die Schaltfläche **[!UICONTROL Abbrechen]** neben der Fortschrittsleiste klicken.

## Ansichten auf der Seite „Aufträge“ ändern {#changing-views-on-the-jobs-page}

Mit den folgenden Verfahren können Sie Aufträge sortieren oder die Ansicht der Registerkarte „Verlauf“ auf der Seite „Aufträge“ ändern:

* **[!UICONTROL Sortierung]**: Wählen Sie einen Spaltennamen aus, um die Liste nach einer bestimmten Spalte zu sortieren. Durch Klicken auf den Schalter neben dem Spaltennamen können Sie zwischen auf- und absteigender Sortierfolge wechseln.

* **[!UICONTROL Datumsbereich]**: Wählen Sie das Menü **[!UICONTROL Datumsbereich]** und wählen Sie eine Option aus, um die Liste der Aufträge auf das aktuelle Datum, die vorherige Woche oder den vorherigen Monat einzugrenzen. Wählen Sie **[!UICONTROL Benutzerdefinierter Datumsbereich]** aus und geben Sie dann einen bestimmten Datumsbereich ein.

* **[!UICONTROL Vorgangstyp]**: Wählen Sie das Menü **[!UICONTROL Vorgangstyp]** und wählen Sie **[!UICONTROL Veröffentlichen]** oder **[!UICONTROL Hochladen]**, um die Liste auf Veröffentlichungsaufträge oder Upload-Aufträge einzugrenzen. Wählen Sie **[!UICONTROL Alle]** aus, um beide Vorgangstypen anzuzeigen.

* **[!UICONTROL Anzeigen]**: Wechseln Sie zu **[!UICONTROL Anzeigen]** > **[!UICONTROL Meine Aufträge]** oder **[!UICONTROL Anzeigen]** > **[!UICONTROL Alle Aufträge]**, um die Liste auf von Ihnen bestellte Aufträge oder Aufträge einzugrenzen, die von Personen in Ihrem Unternehmen bestellt wurden.

## Anzeigen, Kopieren oder Drucken eines Berichts zu Auftragsdetails {#viewing-copying-or-printing-a-job-details-report}

Doppelklicken Sie auf der Seite „Aufträge“ auf den Namen eines Berichts, damit die Seite „Auftragsdetails“ geöffnet wird. Auf dieser Seite werden die im Auftrag enthaltenen Dateien aufgelistet. Wählen Sie **[!UICONTROL Detail anzeigen]**, um die Adobe Dynamic Media Classic-ID, den Zielpfad und Statusinformationen eines Eintrags anzuzeigen. Wenn Sie eine PDF- oder PostScript-Datei hochgeladen haben, für die Schriftarten erforderlich sind, die in Adobe Dynamic Media Classic nicht verfügbar sind, listet der Bericht die fehlenden Schriftarten auf.

Sie können diese Informationen in die Zwischenablage kopieren.

1. Doppelklicken Sie auf der Seite Vorgänge auf den Namen eines Berichts.
1. Wählen Sie auf der Seite „Auftragsdetails **[!UICONTROL die Option &quot;]** anzeigen“ aus, um einen detaillierten Bericht zu einem Eintrag zu erhalten.
1. Wählen Sie **[!UICONTROL In Zwischenablage kopieren]** aus.

## Verarbeiten wiederkehrender Upload- und Veröffentlichungsaufträge {#handling-recurring-upload-and-publish-jobs}

Wiederkehrende Upload- und Veröffentlichungsaufträge, die Sie auf den Seiten „Hochladen“ und „Veröffentlichen“ erstellen, werden auf der Seite „Aufträge“ auf der Registerkarte „Geplant“ aufgeführt. Sie können wiederkehrende Aufträge auf der Registerkarte „Geplant“ bearbeiten und löschen.

Wählen Sie in der globalen Navigationsleiste die Schaltfläche Aufträge und auf der Seite Aufträge die Registerkarte **[!UICONTROL Geplant]** aus, damit Sie wiederkehrende Aufträge bearbeiten und löschen können.

>[!NOTE]
>
>Sie können die Auftragsliste auf der Registerkarte **[!UICONTROL Geplant]** mit den **[!UICONTROL Auftragstyp]** und **[!UICONTROL Anzeigen]** filtern. Wählen Sie einen Vorgangstyp aus, um die Liste auf Veröffentlichungsaufträge eines bestimmten Typs einzugrenzen. Wählen Sie eine **[!UICONTROL Anzeigen]**-Option aus, damit Sie von Ihnen erstellte oder von allen in Ihrem Unternehmen erstellte Aufträge anzeigen können.

### Wiederkehrende Aufträge bearbeiten, löschen, anhalten und fortsetzen {#editing-deleting-pausing-and-resuming-recurring-jobs}

Wählen Sie auf der Seite Aufträge einen wiederkehrenden Auftrag aus und befolgen Sie die folgenden Anweisungen, um ihn zu bearbeiten oder zu löschen:

* **Wiederkehrenden Auftrag bearbeiten**: Klicken Sie auf die Schaltfläche **[!UICONTROL Bearbeiten]** und geben Sie im Dialogfeld „Geplanten Auftrag bearbeiten“ Zeitplaninformationen ein. Wenn der Auftrag in einem Intervall Ihrer Wahl wiederholt werden soll, navigieren Sie zu **[!UICONTROL Wiederholen]** > **[!UICONTROL Benutzerdefiniert]**.

Siehe [Erstellen eines benutzerdefinierten Zeitintervalls für Uploads oder Veröffentlichungsaufträge](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **Löschen eines wiederkehrenden Auftrags**: Klicken Sie auf die Schaltfläche **[!UICONTROL Löschen]**.

* **Anhalten (und Fortsetzen) eines wiederkehrenden Auftrags**: Deaktivieren Sie in der Spalte „Aktiv“ ein Kontrollkästchen, um einen Auftrag anzuhalten. Aktivieren Sie ein Kontrollkästchen, um einen angehaltenen Auftrag fortzusetzen.

### Erstellen eines benutzerdefinierten Zeitintervalls für Upload- oder Veröffentlichungsaufträge {#creating-a-custom-upload-or-publish-job-time-interval}

Um ein benutzerdefiniertes Zeitintervall für einen Upload (über FTP) oder einen Veröffentlichungsauftrag zu erstellen, gehen Sie auf der Seite „Hochladen“ oder „Veröffentlichen“ zu **[!UICONTROL Wiederholen]** > **[!UICONTROL Benutzerdefiniert]**. Geben Sie dann Zahlen und Platzhalter in das Feld Regel ein, um das Zeitintervall für das Wiederholen der Upload- oder Veröffentlichungsaufträge zu beschreiben.

Dies ist die Syntax zum Beschreiben benutzerdefinierter Zeitintervalle für Upload-Aufträge bzw. Veröffentlichungsaufträge im Feld „Regel“:

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

Beispielsweise plant `0 15 10 * * ?` einen Auftrag jeden Tag um 10:1500 Uhr.

In den folgenden Tabellen und in der Liste unten ist dargestellt, wie sich ein Zeitintervall in das Feld „Regel“ eingeben lässt.

Diese Tabelle enthält Informationen zu den Zeitabschnitten, den jeweils zulässigen Werten und den unterstützten Platzhaltern:

| Zeitabschnitte | Zulässige Werte | Kommentare | Unterstützte Platzhalter |
|--- |--- |--- |--- |
| Sekunden | 0-59 |  | `,: * /` |
| Minuten | 0-59 |  | `,: * /` |
| Stunden | 0-23 | Beachten Sie die Verwendung des 24-Stunden-Formats. | `,: * /` |
| Tag des Monats | 1-31 | Sie können keinen numerischen Wert für „Tag des Monats“ und „Tag der Woche“ angeben. Eines dieser Felder muss ein `?` Platzhalterzeichen verwenden. | `,: * / ? L C` |
| Monat | 1 bis 12 oder Jan, Feb, Mär, Apr, Mai, Jun, Jul, Aug, Sep, Okt, Nov, Dez | Bei Werten wird zwischen Groß- und Kleinschreibung unterschieden. | `,: * /` |
| Wochentag | Mo, Di, Mi, Do, Fr, Sa, So | Bei Werten wird zwischen Groß- und Kleinschreibung unterschieden. Sie können keinen numerischen Wert für „Tag des Monats“ und „Tag der Woche“ angeben. Eines dieser Felder muss ein `?` Platzhalterzeichen verwenden. | `,: * / ? L C #` |
| Jahr (optional) | Leer oder 1970-2099 |  | `,: * /` |


In dieser Tabelle sind die im Feld „Regel“ zulässigen Platzhalterzeichen mit Nutzungshinweisen aufgeführt:

| Platzhalterzeichen | Name | Beschreibung |
| --- | --- | --- |
| `*` | Sternchen | Alle Werte (z. B. „jede Minute„). |
| `?` | Fragezeichen | Kein bestimmter Wert (z. B. „eine Minute innerhalb der angegebenen Stunde„). |
| `,` | Komma | Andere Werte (z. B. „Montag und Mittwoch„). |
| `-` | Trennstrich | Wertebereich (z. B. „Montag bis Freitag„). |
| `/` | Schrägstrich | Inkrementiert (z. B. „alle 15 Minuten„). |
| `L` | Großes L | Letzter „Tag des Monats“ oder „Tag der Woche“ (nur für diese Felder verfügbar). Wenn der Monat beispielsweise Januar ist, wird der Auftrag mit einem L-Wert für das Feld „Tag des Monats“ für den 31. Januar geplant. Für das Feld „Wochentag“ können Sie dieses Zeichen allein eingeben, um den Auftrag für Samstag zu planen. Sie können ihn mit einer Zahl verwenden (z. B. `6L`), um den letzten Freitag des Monats anzugeben. Geben Sie keine `L` mit den Platzhaltern Komma oder Bindestrich an. |
| `#` | Zeichen für „Nr.“ | „N“ Wochentag des Monats (nur für das Feld „Wochentag“ verfügbar). Beispiel: `6#3` im Feld „Wochentag“ gibt den dritten Freitag des Monats an. Der `6` bezeichnet „Freitag“ (den sechsten Tag der Woche) und der `3` das dritte Vorkommen im Monat. |
| `C` | Großes K | Erster Kalender „Tag des Monats“ oder „Tag der Woche“ (nur für diese Felder verfügbar). Wenn Sie beispielsweise den Wert `1C` für „Tag des Monats“ angeben, wird der erste Tag im Kalender geplant, der am oder nach dem fünften Tag auftritt. Für das Feld „Wochentag“ wird durch Angabe von `1C` der erste Tag im Kalender geplant, der am oder nach dem Sonntag stattfindet. |

Diese Liste enthält Beispiele zur Beschreibung von Zeitintervallen im Feld „Regel“:

* `0 0 12 * * ?` : Mittag jeden Tag
* `0 15 10 ? * *` : :15 Uhr morgens
* `0 0/5 14 * * ?`: Alle 5 Minuten zwischen :00 und :55 Uhr jeden Tag
* `0 0/5 14,18 * * ?` : Alle 5 Minuten zwischen :00 und :55 Uhr jeden Tag und alle 5 Minuten zwischen :00 und :55 Uhr jeden Tag
* `0 10,44 14 ? 3` : Mittwoch im :10 um 14 :44 14 Uhr
* `0 15 10 ? *` : Mo-Fr um 10:15 Uhr jeden Wochentag
* `0 15 10 20 * ?` : :15 Uhr am 20. jedes Monats
* `0 15 10 L * ?` : :15 Uhr am letzten Tag jedes Monats
* `0 15 10 ? * 6L` : :15 Uhr am letzten Freitag jedes Monats
* `0 15 10 * * 6#3` : :15 Uhr am dritten Freitag jedes Monats

## Verwenden eines Upload- oder Veröffentlichungsauftrags als Trigger {#using-an-upload-or-publish-job-as-a-trigger}

Wenn Sie Assets per FTP hochladen oder einen Veröffentlichungsauftrag ausführen, können Sie einen weiteren Auftrag planen, der nach Abschluss des Uploads beginnt. (Wenn der Start anderer Aufträge für diesen Zeitpunkt geplant ist, wird der hier geplante Auftrag in die Warteschlange gestellt.) Der neue Auftrag sendet eine Benachrichtigung an die von Ihnen angegebene Adresse, damit der Code an diesem Speicherort ausgelöst werden kann. Der nachfolgende Upload-Auftrag erhält denselben Namen wie der aktuelle Upload-Auftrag, jedoch mit dem Präfix „_Pub“.

Um einen Upload- oder Veröffentlichungsauftrag zu einem anderen Trigger zu machen, wählen Sie **[!UICONTROL Erweitert]** auf der Seite „Hochladen“ oder „Veröffentlichen“ aus. Geben Sie dann die URL in das Textfeld „HTTP-Benachrichtigung“ ein.
