---
title: Administrationseinstellungen
seo-title: Administrationseinstellungen
description: 'null'
seo-description: Erfahren Sie, wie Sie den Administrationsbereich von Dynamic Media Classic einrichten.
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
translation-type: tm+mt
source-git-commit: 1ee586fab6a4e10a946848fd079438ade38490d9
workflow-type: tm+mt
source-wordcount: '1945'
ht-degree: 64%

---


<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Administrationseinstellungen{#administration-setup}

Die Anzeigebereiche &quot;Administrationseinstellungen&quot;dienen der Verwaltung von Benutzern von Dynamic Media Classic. Verwenden Sie diese Bildschirme, um Benutzern die Arbeit in Dynamic Media Classic zu ermöglichen und per E-Mail mit Benutzern zu kommunizieren.

1. To access Administration Setup options, click **Setup** > **Personal Setup** > **Administration Setup**.

## Benutzerverwaltung {#user-administration}

Allen Benutzern von Dynamic Media Classic wird eine Rolle zugewiesen, die ihre Berechtigungen und Zugriffsrechte auf Funktionen in Dynamic Media Classic bestimmt. Administratoren legen die verschiedenen Rollen und Verantwortungsbereiche für die Unternehmen fest, denen sie zugewiesen sind.

In der Regel konfiguriert Dynamic Media Classic den ersten Satz von Firmen und weist einen Firmen-Administrator zu. Der Administrator der Firma richtet dann Benutzer von Dynamic Media Classic ein und verwaltet sie.

Dynamic Media Classic unterstützt mehrere Benutzerrollen. Diese Rollen können auf Firmen zugreifen, die für Dynamic Media Classic eingerichtet wurden:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic User** Kann auf Firmen zugreifen, denen sie zugewiesen wurden. dürfen keine Verwaltungsaufgaben ausführen.

**Adobe Dynamic Media Classic Firma Admin** Kann nur eigene Firmen Ansicht und Verwaltung durchführen. Ein Unternehmensadministrator kann außerdem alle Verwaltungsfunktionen ausführen, einschließlich des Hinzufügens von Administratoren und Benutzern. Ein Administrator einer Firma kann einen Benutzer zu den DMC-Firma-Administratorkonten hinzufügen. (Dies ist die Standard-Benutzerrolle.)

Nachdem Sie einen Benutzer hinzugefügt haben, sendet Dynamic Media Classic dem Benutzer eine Begrüßungs-E-Mail. Die Nachricht enthält ein Kennwort und die URL für die dynamische Medienklassifizierung.

### Hinzufügen eines Benutzers oder Administrators {#adding-a-user-or-administrator}

1. Klicken Sie auf „Einstellungen“ > „Anwendungseinstellungen“ > „Administrationseinstellungen“ > „Benutzerverwaltung“.
1. Klicken Sie auf „Hinzufügen“.
1. Geben Sie den Namen und die E-Mail-Adresse des Benutzers oder Administrators ein, den Sie hinzufügen möchten, und klicken Sie dann auf „Weiter“.

   >[!NOTE]
   >
   >In E-Mail-Adressen ist kein Apostroph (’) erlaubt.

1. Wählen Sie die Rolle aus, die Sie dem Benutzer zuordnen möchten. 

   Siehe [Benutzerrollen und -rechte](administration-setup.md#user_administration)von Dynamic Media Classic.

1. Wählen Sie einen Unternehmensnamen aus, um einem Unternehmen einen Benutzer hinzuzufügen.
1. Wenn Sie den Benutzer einer Gruppe hinzufügen möchten (falls Sie einen Media-Portal-Benutzer oder -Mitarbeiter hinzufügen), klicken Sie auf „Weiter“ und fügen Sie den Benutzer hinzu.
1. Klicken Sie auf „Speichern“, um die Benutzereinrichtung abzuschließen.

   Nach dem Speichern werden Sie gefragt, ob Sie einem anderen Unternehmen einen Benutzer hinzufügen möchten. Klicken Sie auf „Hinzufügen“, wenn Sie den Benutzer einem Unternehmen hinzufügen möchten.

   Alle neuen Benutzer erhalten ein zufällig generiertes Kennwort; Benutzer müssen Kennwörter bei der ersten Anmeldung bei Dynamic Media Classic ändern.

   Die von Ihnen hinzugefügten neuen Benutzer erhalten eine Begrüßungs-E-Mail. Die E-Mail enthält ein temporäres Kennwort sowie Anleitungen zur Anmeldung am Scene7 Publishing System.

   Wenn der Benutzer die Begrüßungs-E-Mail nicht erhält, bitten Sie ihn, die Anmeldeseite von Dynamic Media Classic (https://s7sps1.scene7.com) aufzurufen und auf &quot;Kennwort vergessen&quot;zu klicken. Das Kennwort wird zurückgesetzt und es wird eine neue E-Mail gesendet. Wenn der Benutzer auch diese E-Mail nicht erhält und sie nicht in seinem Spam-Ordner ist, wenden Sie sich an den technischen Support.

   Beim Hinzufügen von neuen Media-Portal-Benutzern können Sie auch „Einstellungen“ > „Anwendungseinstellungen“ > „Benutzerverwaltung“ aufrufen und dann auf „Benutzerliste hochladen“ klicken und eine CSV-Datei wählen, die nicht mehr als 500 Benutzer enthält.

### Löschen eines Benutzers {#deleting-a-user}

Sie können Benutzer aus Dynamic Media Classic löschen, indem Sie sie für ungültig erklären. Ungültige Benutzer werden aus dem System und sämtlichen Konten entfernt.

1. Klicken Sie auf **„Einstellungen“** > **„Anwendungseinstellungen“** > **„Administrationseinstellungen“** > **„Benutzerverwaltung“**.
1. Wählen Sie aus der Liste einen Benutzer aus und klicken Sie dann auf **„Bearbeiten“**.
1. Deaktivieren Sie „Gültig“.
1. Klicken Sie auf „**Speichern**“.

### Aktivieren oder Deaktivieren von Benutzern {#activating-or-deactivating-users}

Benutzer, die deaktiviert wurden, können nicht mehr auf das oben im Menü „Konto zum Zugreifen auswählen“ aufgelistete Konto zugreifen.

1. Klicken Sie auf **„Einstellungen“** > **„Anwendungseinstellungen“** > **„Administrationseinstellungen“** > **„Benutzerverwaltung“**.
1. Aktivieren bzw. deaktivieren Sie in der Benutzerliste das Kontrollkästchen „Aktiv“ neben dem Namen des Benutzers.

### Bearbeiten von Benutzerinformationen {#editing-user-information}

Welche Benutzerinformationen Sie bearbeiten können, hängt von Ihrer Rolle als Administrator und der zugewiesenen Rolle der Benutzer ab, deren Angaben Sie bearbeiten möchten. Abgeblendete Optionen (nicht verfügbar) sind nicht bearbeitbar.

1. Gehen Sie zu **„Einstellungen“** > **„Anwendungseinstellungen“** > **„Administrationseinstellungen“** > **„Benutzerverwaltung“**.
1. Wählen Sie den Benutzer aus und klicken Sie auf **„Bearbeiten“**.
1. Wählen Sie den Eintrag in der Tabelle aus, die das Unternehmen anzeigt, für das Sie die Berechtigungen oder den Zugriff ändern möchten, und klicken Sie dann auf den Link „Unternehmen verwalten“.
1. Wählen Sie die Benutzerrolle aus.
1. Wenn Sie die Gruppenmitgliedschaft des Benutzers ändern möchten (falls Sie Media-Portal-Benutzer oder -Mitarbeiter bearbeiten oder hinzufügen), klicken Sie auf „Weiter“ und bearbeiten Sie die Gruppenmitgliedschaft.
1. Klicken Sie auf „**Speichern**“.

### Filtern und Sortieren der Benutzerliste {#filtering-and-sorting-the-user-list}

Sie können die Benutzerliste sortieren und filtern, um Benutzer zu suchen. Alle Benutzer sämtlicher von Ihnen verwalteten Konten werden in der Benutzerliste aufgelistet, unabhängig von dem im Menü „Konto zum Zugreifen auswählen“ ausgewählten Konto.

Sie können die folgenden Techniken zum Filtern der Benutzerliste verwenden:

**Filtern nach Gruppe** Wählen Sie im Menü Nach Gruppe die Option und wählen Sie eine Option, um die Liste auf die Benutzer in einer Gruppe zu beschränken.

**Nach Benutzerrolle** filtern Wählen Sie das Menü Nach Benutzerrolle aus und wählen Sie eine Option, um die Liste auf Benutzer oder Administratoren verschiedener Typen einzuschränken.

**Filtern nach Feldnamen** Wählen Sie die Option &quot;Filter nach Feld aktivieren&quot;. Wählen Sie anschließend im Menü „Nach Feldname“ die Spalte, nach der Sie filtern möchten, und im Menü „Zeichen filtern“ den gewünschten Buchstaben aus. Anschließend wird die Liste in der ausgewählten Spalte nach dem angegebenen Buchstaben gefiltert. Um wieder die vollständige Liste anzuzeigen, deaktivieren Sie die Option „Filtern nach Feld aktivieren“.

**Ungültige Benutzer** herausfiltern Deaktivieren Sie die Option &quot;Ungültige einschließen&quot;. In den Suchergebnissen werden nur Benutzer aufgelistet, die im System vorhanden sind. Ungültige Benutzer wurden aus dem System und sämtlichen von Ihnen verwalteten Konten gelöscht.

**Sortieren nach Spaltenüberschrift** Klicken Sie auf eine Überschrift, um alle Benutzer nach ihrem Status, alphabetisch nach Vorname, Nachname oder E-Mail, nach Benutzerrolle oder nach gültigem/ungültigem Status zu sortieren.

Wenn Sie mit sehr vielen Benutzern arbeiten, können Sie im Menü „Max. Listengr.“ eine Zahl eingeben, um die Länge der Liste zu beschränken.

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to a Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to a Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Click **Manage Organizations**.
1. Click **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Click **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, click **Solutions** &gt; **Experience Manager**. Under the Dynamic Media Classic card, click **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Bandbreite und Speicher {#bandwidth-storage}

Administratoren von Dynamic Media Classic können Bandbreite, Datenspeicherung und andere Berichtstypen für die von ihnen verwalteten Firmen generieren. Diese Berichte sind im Anzeigebereich „Bandbreite und Speicher“ verfügbar.

Klicken Sie auf „Einstellungen“ > „Persönliche Einstellungen“, um diesen Anzeigebereich zu öffnen. Erweitern Sie die Administrationseinstellungen und klicken Sie dann auf „Bandbreite und Speicher“.

### Berichtstypen {#types-of-reports}

Die folgende Tabelle beschreibt Berichte, die Sie im Anzeigebereich „Bandbreite und Speicher“ generieren können:

| Bericht | Information | Verwendung |
|:--- |:--- |:--- |
| Bandbreite | Bandbreitennutzung nach Unternehmen | Verfolgen Sie die Bandbreitennutzung nach Unternehmen über bestimmte Zeitspannen, um Datenverkehrsmuster zu ermitteln. |
| Speicher | Speicherverwendung | Verfolgen Sie die hochgeladene Datenmenge nach Unternehmen. |
| Bildinhalt | Die Anzahl der Bildanfragen nach Typ | Verfolgen Sie die Anzahl der Anfragen nach und das Volumen für verschiedene Bildtypen. |
| Domäne | Die Anzahl der URL-Anfragen nach Domäne | Verfolgen Sie die Bildernutzung auf der Basis der Domäne der Bildanfragen eines bestimmten Unternehmens. (Dynamic Media Classic kann mehr als eine Domäne pro Konto bereitstellen. Weitere Informationen erhalten Sie vom technischen Support.) |
| Video-Streaming | Bandbreitennutzung für Streaming-Videos | Verfolgen Sie die Nutzung von Streaming-Videos nach Unternehmen über bestimmte Zeitspannen, um Datenverkehrsmuster zu ermitteln. |
| Videoinhalt | Wiedergabezeit verschiedener Videos | Ermitteln Sie, welche Videos am häufigsten und am wenigsten häufig abgerufen werden. |


Der Bericht „Bildinhalt“ enthält Informationen über Anforderungen nach den folgenden Bildtypen:

**Bildanforderungen** für Bilder.

**Anfragen** nach Miniaturansichten für Muster oder alternative Bilder in Viewern.

**Anforderungen** für Maskenanfragen an Bilder, die Graustufenmasken zurückgeben.

**Bildanforderungen** für Viewer-Kacheln, die von einem Viewer geladen werden.

**Image-Rendering-Anforderungen** für VNT-Objekte, die ein Bild mit bestimmten Objekten in den angeforderten Vignetten zurückgeben.

**Image Rendering-Anforderungen** für VNT-Info-Anfragen, die Informationen zu den angeforderten Vignetten zurückgeben.

>[!NOTE]
>
>Der Bericht zu Video-Streaming bezieht nur Streaming-Videos mit ein. Die Anzeige progressiver Videos wird nicht verfolgt.

### Generieren eines Berichts {#generating-a-report}

So generieren Sie einen Bericht zur Bandbreite, zum Speicher, zu Bildinhalt, zur Domäne, zum Video-Streaming oder zu Videoinhalt:

1. Wählen Sie „Einstellungen“ > „Persönliche Einstellungen“.
1. Erweitern Sie die Administrationseinstellungen und klicken Sie dann auf „Bandbreite und Speicher“.
1. Klicken Sie auf eine Registerkarte: Bandbreite, Speicher, Bildinhalt, Domäne, Video-Streaming oder Videoinhalt. 

   Siehe [Berichtstypen](administration-setup.md#types_of_reports).

### Unterschiedliche Anzeige von Daten {#viewing-data-in-different-ways}

Nachdem Sie einen Bericht auf der Seite „Bandbreite und Speicher“ generiert haben, können Sie Optionen zum Anzeigen der Informationen auswählen. Sie können festlegen, wie die Informationen dargestellt werden, die Informationen in einem Diagramm oder Datenraster anzeigen und einen Zeitraum für das Erfassen von Informationen bestimmen. In der Datenansicht können Sie die Informationen auch sortieren und in Spalten anordnen.

**Anzeigen von Daten in einem Diagramm oder Datenraster** Klicken Sie auf die Option &quot;DiagrammAnsicht&quot;, um Daten in einem Diagramm Ansicht; Klicken Sie auf die Option &quot;Ansicht der Daten&quot;, um Daten in einem Datenraster Ansicht.

**Wählen Sie im Menü &quot;Berichtstyp&quot;den Typ** &quot;Zusammenfassung&quot;, &quot;Täglich&quot;oder &quot;Monatlich&quot;, um die Daten in Form einer Zusammenfassung, nach Tag oder Monat zu organisieren. Diese Option steht nicht in allen Berichten zur Verfügung.

**Festlegen eines Zeitraums** Wählen Sie Optionen zur Definition eines Zeitraums für Ihren Bericht aus und klicken Sie nach der Definition des Zeitraums auf Aktualisieren:

**Vordefinierter Zeitraum** Wählen Sie im Menü Vordefinierter Bericht eine Option. Wählen Sie beispielsweise „Letzter Monat“, um die Daten des letzten Monats zu erfassen.

**Benutzerdefinierter Zeitraum** Wählen Sie im Menü Vordefinierter Bericht die Option Benutzerdefiniert. Wählen Sie anschließend ein Datum im Menü „Startmonat“ (bzw. „Startdatum“) und ein Datum im Menü „Anzahl Monate (bzw. „Anzahl Tage“). Für Berichte zur Domäne und zum Videoinhalt können Sie ein bestimmtes Start- und Enddatum für die Erfassung von Berichtsinformationen wählen.

**Sortieren von Daten (nur Ansicht)** Klicken Sie zum Sortieren von Informationen in einer Spalte auf die Spaltenüberschrift. Bei erneutem Klicken wird die Sortierreihenfolge umgekehrt (absteigend).

**Neuanordnen von Spalten (nur Datenspalte)** Um eine Ansicht an eine andere Position im Datenraster zu verschieben, ziehen Sie die Überschrift.

### Exportieren und Drucken von Berichten {#exporting-and-printing-reports}

Nachdem Sie einen Bericht generiert haben, können Sie die Daten für die Verwendung in Tabellen und anderen Anwendungen exportieren. Sie können die Berichte auch ausdrucken.

**Exportieren von Berichtsdaten** In der Ansicht &quot;Daten&quot;sortieren und ordnen Sie die Daten nach Bedarf an. Rufen Sie anschließend das Menü „Exportieren“ auf und wählen Sie ein Format: „Tabulatorgetrennt“, „Durch Komma getrennt“ oder „HTML-formatiert“. Die Daten werden in dem gewünschten Format in die Zwischenablage kopiert. Jetzt können Sie die Daten in eine Tabelle oder Anwendung einfügen.

**Drucken eines Berichts** Klicken Sie auf Drucken, wählen Sie im Dialogfeld Drucken die gewünschten Optionen und klicken Sie dann auf OK.

## Bildfehler {#image-errors}

Administratoren von Dynamic Media Classic können Bildfehlerberichte erstellen. Ein Bildfehlerbericht zeigt eine Liste der 20 häufigsten Bildfehler in den letzten 24 Stunden für das Unternehmen an, bei dem Sie derzeit angemeldet sind. Gehen Sie folgendermaßen vor, um einen Bildfehlerbericht zu generieren:

1. Klicken Sie auf „Einstellungen“ > „Persönliche Einstellungen“.
1. Erweitern Sie die Administrationseinstellungen und klicken Sie dann auf „Bildfehler“.
1. (Optional) Führen Sie dann einen der folgenden Schritte aus:

   * Klicken Sie auf eine Spaltenüberschrift, um die Fehler nach der jeweiligen Spaltenangabe zu sortieren. Standardmäßig sind die Fehler absteigend nach der Anzahl der Instanzen geordnet.
   * Bewegen Sie den Cursor über das Feld „Antwort“ eines Fehlers, um die jeweilige Fehlermeldung anzuzeigen.
   * Bewegen Sie den Cursor über das Feld „URL“ oder „Referrer“, um den Link zum Bild oder der Referrer-Website anzuzeigen.
   * Klicken Sie auf „URL kopieren“, um den Link zum tatsächlichen Bild zu kopieren. Sie können diesen Link in ein Browserfenster kopieren, um das Bild aufzurufen und den Fehler zu prüfen.
   * Klicken Sie auf die zum Feld „Referrer“ gehörige Schaltfläche „URL kopieren“, um den Link zur Referrer-Website zu kopieren.

Die angezeigten Fehler betreffen das Unternehmen, bei dem Sie aktuell angemeldet sind. Jeder Fehler enthält die folgenden Informationen:

**Bild-ID** für das betreffende Bild.

**Zeit** Der Zeitraum, in dem der Fehler zum ersten Mal gemeldet wurde, bis zum letzten Mal, in den letzten 24 Stunden, gemeldet wurde.

**Zählt** Die Anzahl der im Bild gemeldeten Fehler.

**Antwort** Die spezifische Fehlermeldung. Fehler haben IDs, die mit 4xx oder 5xx beginnen.

**Mit URLs** wird die URL zum Bild in Scene7 Liste.

**Werber** Gibt die URL der Website an, von der die ursprüngliche Anforderung stammt. Der Referrer kann jede Website sein, auf der ein Link zu dem Bild zu finden ist.

Für die Spalten „URL“ und „Referrer“ gibt es die Schaltfläche „URL kopieren“, um das Testen der URLs zu vereinfachen.
