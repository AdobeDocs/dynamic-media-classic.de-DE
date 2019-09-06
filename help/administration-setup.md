---
title: Administrationseinstellungen
seo-title: Administrationseinstellungen
description: 'null'
seo-description: Erfahren Sie, wie Sie den Administrationsbereich von Dynamic Media Classic einrichten.
uuid: 16 ba 9 fed-b 5 c 6-4991-83 b 3-8 d 7 d 7129013 a
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 3 c 9 ee 4 ec-dd 37-498 d -98 d 6-1339 b 80177 ff
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Administrationseinstellungen{#administration-setup}

Die Bildschirme „Administrationseinstellungen“ dienen Scene7 Publishing System-Benutzern zur Verwaltung. In diesen Anzeigebereichen können Sie die Einstellungen für die Arbeit der Benutzer mit dem Scene7 Publishing System festlegen und per E-Mail mit den Benutzern kommunizieren.

1. To access Administration Setup options, click **Setup** &gt; **Personal Setup** &gt; **Administration Setup**.

## Benutzerverwaltung {#user-administration}

Allen Benutzern von Classic Media Classic wird eine Rolle zugewiesen, die ihre Berechtigungen und Zugriffsrechte für Funktionen im Scene 7 Publishing System bestimmt. Administratoren legen die verschiedenen Rollen und Verantwortungsbereiche für die Unternehmen fest, denen sie zugewiesen sind.

In der Regel konfiguriert Dynamic Media Classic die erste Gruppe von Unternehmen und weist einen Unternehmensadministrator zu. Der Unternehmensadministrator richtet die Scene7 Publishing System-Benutzer ein und verwaltet sie.

Das Scene7 Publishing System unterstützt drei Benutzerrollen. Alle drei Rollen können auf Unternehmen zugreifen, die für das Scene7 Publishing System eingerichtet sind:

**SPS-Administrator** kann alle Funktionen im Scene 7 Publishing System anzeigen und verwalten sowie Unternehmen einrichten und Administratoren und Benutzer hinzufügen.

**Unternehmensadministrator** kann nur eigene Unternehmen anzeigen und verwalten. Ein Unternehmensadministrator kann außerdem alle Verwaltungsfunktionen ausführen, einschließlich des Hinzufügens von Administratoren und Benutzern. Ein Unternehmensadministrator kann einen Benutzer zu den SPS-Unternehmensadministratorkonten hinzufügen. (Dies ist die Standard-Benutzerrolle.)

**SPS-Benutzer** können auf Unternehmen zugreifen, denen sie zugewiesen wurden. kann keine Verwaltungsaufgaben ausführen.

Nachdem ein Benutzer hinzugefügt wurde, erhält er vom Scene7 Publishing System eine Begrüßungs-E-Mail. Die Nachricht enthält ein Kennwort und die Scene7 Publishing System-URL.

### Hinzufügen eines Benutzers oder Administrators {#adding-a-user-or-administrator}

1. Klicken Sie auf „Einstellungen“ &gt; „Anwendungseinstellungen“ &gt; „Administrationseinstellungen“ &gt; „Benutzerverwaltung“.
1. Klicken Sie auf „Hinzufügen“.
1. Geben Sie den Namen und die E-Mail-Adresse des Benutzers oder Administrators ein, den Sie hinzufügen möchten, und klicken Sie dann auf „Weiter“.

   >[!NOTE]
   >
   >In E-Mail-Adressen ist kein Apostroph (’) erlaubt.

1. Wählen Sie die Rolle aus, die Sie dem Benutzer zuordnen möchten. 

   Siehe [Benutzerrollen und -rechte für dynamische Medien](administration-setup.md#user_administration).

1. Wählen Sie einen Unternehmensnamen aus, um einem Unternehmen einen Benutzer hinzuzufügen.
1. Wenn Sie den Benutzer einer Gruppe hinzufügen möchten (falls Sie einen Media-Portal-Benutzer oder -Mitarbeiter hinzufügen), klicken Sie auf „Weiter“ und fügen Sie den Benutzer hinzu.
1. Klicken Sie auf „Speichern“, um die Benutzereinrichtung abzuschließen.

   Nach dem Speichern werden Sie gefragt, ob Sie einem anderen Unternehmen einen Benutzer hinzufügen möchten. Klicken Sie auf „Hinzufügen“, wenn Sie den Benutzer einem Unternehmen hinzufügen möchten.

   Alle neuen Benutzer erhalten ein zufällig generiertes Kennwort, das geändert werden muss, sobald sie sich zum ersten Mal beim Scene7 Publishing System anmelden.

   Die von Ihnen hinzugefügten neuen Benutzer erhalten eine Begrüßungs-E-Mail. Die E-Mail enthält ein temporäres Kennwort sowie Anleitungen zur Anmeldung am Scene7 Publishing System.

   Wenn der Benutzer die Begrüßungs-E-Email nicht erhält, gehen Sie zur SPS-Anmeldeseite (https://s7sps1.scene7.com) und klicken Sie auf "Forgot My Password" (Forgot My Password (Vergessene ID). Das Kennwort wird zurückgesetzt und es wird eine neue E-Mail gesendet. Wenn der Benutzer auch diese E-Mail nicht erhält und sie nicht in seinem Spam-Ordner ist, wenden Sie sich an den technischen Support.

   Beim Hinzufügen von neuen Media-Portal-Benutzern können Sie auch „Einstellungen“ &gt; „Anwendungseinstellungen“ &gt; „Benutzerverwaltung“ aufrufen und dann auf „Benutzerliste hochladen“ klicken und eine CSV-Datei wählen, die nicht mehr als 500 Benutzer enthält.

### Löschen eines Benutzers {#deleting-a-user}

Sie können Benutzer aus dem Scene7 Publishing System löschen, indem Sie sie als ungültig markieren. Ungültige Benutzer werden aus dem System und sämtlichen Konten entfernt.

1. Klicken Sie auf **„Einstellungen“** &gt; **„Anwendungseinstellungen“** &gt; **„Administrationseinstellungen“** &gt; **„Benutzerverwaltung“**.
1. Wählen Sie aus der Liste einen Benutzer aus und klicken Sie dann auf **„Bearbeiten“**.
1. Deaktivieren Sie „Gültig“.
1. Klicken Sie auf „**Speichern**“.

### Aktivieren oder Deaktivieren von Benutzern {#activating-or-deactivating-users}

Benutzer, die deaktiviert wurden, können nicht mehr auf das oben im Menü „Konto zum Zugreifen auswählen“ aufgelistete Konto zugreifen.

1. Klicken Sie auf **„Einstellungen“** &gt; **„Anwendungseinstellungen“** &gt; **„Administrationseinstellungen“** &gt; **„Benutzerverwaltung“**.
1. Aktivieren bzw. deaktivieren Sie in der Benutzerliste das Kontrollkästchen „Aktiv“ neben dem Namen des Benutzers.

### Bearbeiten von Benutzerinformationen {#editing-user-information}

Welche Benutzerinformationen Sie bearbeiten können, hängt von Ihrer Rolle als Administrator und der zugewiesenen Rolle der Benutzer ab, deren Angaben Sie bearbeiten möchten. Abgeblendete Optionen (nicht verfügbar) sind nicht bearbeitbar.

1. Gehen Sie zu **„Einstellungen“** &gt; **„Anwendungseinstellungen“** &gt; **„Administrationseinstellungen“** &gt; **„Benutzerverwaltung“**.
1. Wählen Sie den Benutzer aus und klicken Sie auf **„Bearbeiten“**.
1. Wählen Sie den Eintrag in der Tabelle aus, die das Unternehmen anzeigt, für das Sie die Berechtigungen oder den Zugriff ändern möchten, und klicken Sie dann auf den Link „Unternehmen verwalten“.
1. Wählen Sie die Benutzerrolle aus.
1. Wenn Sie die Gruppenmitgliedschaft des Benutzers ändern möchten (falls Sie Media-Portal-Benutzer oder -Mitarbeiter bearbeiten oder hinzufügen), klicken Sie auf „Weiter“ und bearbeiten Sie die Gruppenmitgliedschaft.
1. Klicken Sie auf „**Speichern**“.

### Filtern und Sortieren der Benutzerliste {#filtering-and-sorting-the-user-list}

Sie können die Benutzerliste sortieren und filtern, um Benutzer zu suchen. Alle Benutzer sämtlicher von Ihnen verwalteten Konten werden in der Benutzerliste aufgelistet, unabhängig von dem im Menü „Konto zum Zugreifen auswählen“ ausgewählten Konto.

Sie können die folgenden Techniken zum Filtern der Benutzerliste verwenden:

**Filtern nach Gruppe** Wählen Sie das Menü Nach Gruppe aus und wählen Sie eine Option, um die Liste auf Benutzer in einer Gruppe einzugrenzen.

**Filtern nach Benutzerrolle** Wählen Sie das Menü "Nach Benutzerrolle" und wählen Sie eine Option, um die Liste auf Benutzer oder Administratoren verschiedener Typen einzuschränken.

**Filtern nach Feldname** Wählen Sie die Option Filter nach Feld aktivieren. Wählen Sie anschließend im Menü „Nach Feldname“ die Spalte, nach der Sie filtern möchten, und im Menü „Zeichen filtern“ den gewünschten Buchstaben aus. Anschließend wird die Liste in der ausgewählten Spalte nach dem angegebenen Buchstaben gefiltert. Um wieder die vollständige Liste anzuzeigen, deaktivieren Sie die Option „Filtern nach Feld aktivieren“.

**Ungültige Benutzer** herausfiltern deaktivieren Sie die Option "Ungültige einschließen" . In den Suchergebnissen werden nur Benutzer aufgelistet, die im System vorhanden sind. Ungültige Benutzer wurden aus dem System und sämtlichen von Ihnen verwalteten Konten gelöscht.

**Nach Spaltenüberschrift sortieren** Klicken Sie auf eine Überschrift, um alle Benutzer nach ihrem Status alphabetisch nach Vorname, Nachname, Nachname oder E-Email, nach Benutzerrolle oder nach gültigem Status zu sortieren.

Wenn Sie mit sehr vielen Benutzern arbeiten, können Sie im Menü „Max. Listengr.“ eine Zahl eingeben, um die Länge der Liste zu beschränken.

### Verknüpfen einer IMS-Benutzeridentität mit einem klassischen IPS-Benutzerkonto für ein dynamisches IPS {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

Sie können eine Adobe IMS-Benutzeridentität mit einem klassischen IPS-Benutzerkonto für dynamische Medien verknüpfen, damit Sie sich über SSO (Single Sign On) anmelden und Scene 7 Publishing System über die Adobe Marketing Cloud starten können.

1. Adobe sollte Ihr Konto bereits mit einer Adobe Marketing Cloud-Organisation einrichten und mit Ihrem Scene 7 Publishing System-Produktkontext verknüpfen. Wenn diese Einrichtung noch nicht erfolgt ist oder Sie sich nicht sicher sind, ob sie fertig ist, wenden Sie sich an den Adobe-Kundendienst.

   Nach Abschluss des Setups können Sie sich bei der Adobe Marketing Cloud anmelden und Ihre Adobe Marketing Cloud-Identität mit Ihrem Benutzerkonto für dynamische Medien verknüpfen, indem Sie folgende Schritte ausführen.

1. Navigieren Sie in der Adobe Marketing Cloud zu Ihren Kontoeinstellungen.
1. Klicken **Sie auf Unternehmen verwalten**.
1. Klicken **Sie auf Konto verknüpfen** oder **Zugriff sichern**.
1. Wählen Sie **Experience Manager** und geben Sie Ihre Anmeldedaten ein.

   Ihre Anmeldeinformationen umfassen Ihre IPS-Unternehmensregion, E-Email-Adresse und Ihr Kennwort.

1. Klicken **Sie auf Link**.
1. Wenn der Link festgelegt ist, können Sie das Scene 7 Publishing System über die Adobe Marketing Cloud starten oder direkt starten.

   Führen Sie einen der folgenden Schritte aus:

   * Um Dynamisches Media Classic aus der Adobe Marketing Cloud heraus zu starten, klicken Sie in der linken Leiste der Adobe Marketing Cloud auf **Lösungen** &gt; **Experience Manager**. Klicken Sie unter der Karte "Dynamic Media Classic" auf **Start**.
   * Um sich direkt mit Ihren IMS-Anmeldedaten beim Scene 7 Publishing System anzumelden, verwenden Sie die folgende Website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Ersetzen Sie "N" im obigen Pfad durch die Nummer für den IPS-Unternehmensbereich. Das heißt, N = 1 für Nordamerika; 3 für EMEA; oder 5 für JAPAC.

## Bandbreite und Speicher {#bandwidth-storage}

SPS-Administratoren können Berichte zu Bandbreite und Speicherplatz sowie Berichte anderer Typen für die von ihnen verwalteten Unternehmen erstellen. Diese Berichte sind im Anzeigebereich „Bandbreite und Speicher“ verfügbar.

Klicken Sie auf „Einstellungen“ &gt; „Persönliche Einstellungen“, um diesen Anzeigebereich zu öffnen. Erweitern Sie die Administrationseinstellungen und klicken Sie dann auf „Bandbreite und Speicher“.

### Berichtstypen {#types-of-reports}

Die folgende Tabelle beschreibt Berichte, die Sie im Anzeigebereich „Bandbreite und Speicher“ generieren können:

| Bericht | Information | Verwendung |
|:--- |:--- |:--- |
| Bandbreite | Bandbreitennutzung nach Unternehmen | Verfolgen Sie die Bandbreitennutzung nach Unternehmen über bestimmte Zeitspannen, um Datenverkehrsmuster zu ermitteln. |
| Speicher | Speicherverwendung | Verfolgen Sie die hochgeladene Datenmenge nach Unternehmen. |
| Bildinhalt | Die Anzahl der Bildanfragen nach Typ | Verfolgen Sie die Anzahl der Anfragen nach und das Volumen für verschiedene Bildtypen. |
| Domäne | Die Anzahl der URL-Anfragen nach Domäne | Verfolgen Sie die Bildernutzung auf der Basis der Domäne der Bildanfragen eines bestimmten Unternehmens. (Dynamisches Media Classic kann mehr als eine Domäne pro Konto bereitstellen. Weitere Informationen erhalten Sie vom technischen Support.) |
| Video-Streaming | Bandbreitennutzung für Streaming-Videos | Verfolgen Sie die Nutzung von Streaming-Videos nach Unternehmen über bestimmte Zeitspannen, um Datenverkehrsmuster zu ermitteln. |
| Videoinhalt | Wiedergabezeit verschiedener Videos | Ermitteln Sie, welche Videos am häufigsten und am wenigsten häufig abgerufen werden. |


Der Bericht „Bildinhalt“ enthält Informationen über Anforderungen nach den folgenden Bildtypen:

**Bildanforderungsanfragen** für Bilder.

**Miniaturanforderungsanforderungen** für Musterbilder oder alternative Bilder in Viewern.

**Maskieren** von Anforderungen an Bilder, die Graustufen-Masken zurückgeben.

**Viewer-Kachelanforderungen,** die von einem Viewer geladen werden.

**VNT-Objektanforderungsanforderungen** , die ein Bild mit bestimmten Objekten in den angefragten Vignetten zurückgeben.

**VNT-Infoanforderungen Image Image** Rendering, die Informationen zu den angefragten Vignetten zurückgeben.

>[!NOTE]
>
>Der Bericht zu Video-Streaming bezieht nur Streaming-Videos mit ein. Die Anzeige progressiver Videos wird nicht verfolgt.

### Generieren eines Berichts {#generating-a-report}

So generieren Sie einen Bericht zur Bandbreite, zum Speicher, zu Bildinhalt, zur Domäne, zum Video-Streaming oder zu Videoinhalt:

1. Wählen Sie „Einstellungen“ &gt; „Persönliche Einstellungen“.
1. Erweitern Sie die Administrationseinstellungen und klicken Sie dann auf „Bandbreite und Speicher“.
1. Klicken Sie auf eine Registerkarte: Bandbreite, Speicher, Bildinhalt, Domäne, Video-Streaming oder Videoinhalt. 

   Siehe [Berichtstypen](administration-setup.md#types_of_reports).

### Unterschiedliche Anzeige von Daten {#viewing-data-in-different-ways}

Nachdem Sie einen Bericht auf der Seite „Bandbreite und Speicher“ generiert haben, können Sie Optionen zum Anzeigen der Informationen auswählen. Sie können festlegen, wie die Informationen dargestellt werden, die Informationen in einem Diagramm oder Datenraster anzeigen und einen Zeitraum für das Erfassen von Informationen bestimmen. In der Datenansicht können Sie die Informationen auch sortieren und in Spalten anordnen.

**Ansicht von Daten in einem Diagramm oder Datenraster** Klicken Sie auf die Option Diagrammansicht, um die Daten in einem Diagramm anzuzeigen. Klicken Sie auf die Option Datenansicht, um Daten in einem Datenraster anzuzeigen.

**Wählen Sie im Menü Berichtstyp die Option** "Zusammenfassung" ," Täglich" oder "Monatlich" , um die Daten in Zusammenfassungsform, nach Tag oder nach Monat zu organisieren. Diese Option steht nicht in allen Berichten zur Verfügung.

**Festlegen eines Zeitraums** zum Festlegen eines Zeitraums für den Bericht und Klicken Sie dann auf "Aktualisieren" , nachdem Sie einen Zeitraum definiert haben:

**Vordefinierter Zeitraum** Im Menü "Vordefinierte Berichte" wählen Sie eine Option. Wählen Sie beispielsweise „Letzter Monat“, um die Daten des letzten Monats zu erfassen.

**Benutzerdefinierter Zeitraum** im Menü "Vordefinierte Berichte" wählen Sie" Benutzerdefiniert" . Wählen Sie anschließend ein Datum im Menü „Startmonat“ (bzw. „Startdatum“) und ein Datum im Menü „Anzahl Monate (bzw. „Anzahl Tage“). Für Berichte zur Domäne und zum Videoinhalt können Sie ein bestimmtes Start- und Enddatum für die Erfassung von Berichtsinformationen wählen.

**Sortieren von Daten (nur Datenansicht)** Klicken Sie auf die Spaltenüberschrift, um Informationen in einer Spalte zu sortieren. Bei erneutem Klicken wird die Sortierreihenfolge umgekehrt (absteigend).

**Spalten (nur Datenansicht) neu anordnen** , um eine Spalte an eine andere Position im Datenraster zu verschieben, ziehen Sie die Überschrift.

### Exportieren und Drucken von Berichten {#exporting-and-printing-reports}

Nachdem Sie einen Bericht generiert haben, können Sie die Daten für die Verwendung in Tabellen und anderen Anwendungen exportieren. Sie können die Berichte auch ausdrucken.

**Exportieren von Berichtsdaten** in der Datenansicht Sortieren und ordnen Sie die Daten nach Bedarf an. Rufen Sie anschließend das Menü „Exportieren“ auf und wählen Sie ein Format: „Tabulatorgetrennt“, „Durch Komma getrennt“ oder „HTML-formatiert“. Die Daten werden in dem gewünschten Format in die Zwischenablage kopiert. Jetzt können Sie die Daten in eine Tabelle oder Anwendung einfügen.

**Drucken eines Berichts** Klicken Sie auf "Drucken" , wählen Sie die gewünschten Optionen im Dialogfeld" Drucken" aus und klicken Sie dann auf "OK" .

## Bildfehler {#image-errors}

SPS-Administratoren können Bildfehlerberichte generieren. Ein Bildfehlerbericht zeigt eine Liste der 20 häufigsten Bildfehler in den letzten 24 Stunden für das Unternehmen an, bei dem Sie derzeit angemeldet sind. Gehen Sie folgendermaßen vor, um einen Bildfehlerbericht zu generieren:

1. Klicken Sie auf „Einstellungen“ &gt; „Persönliche Einstellungen“.
1. Erweitern Sie die Administrationseinstellungen und klicken Sie dann auf „Bildfehler“.
1. (Optional) Führen Sie dann einen der folgenden Schritte aus:

   * Klicken Sie auf eine Spaltenüberschrift, um die Fehler nach der jeweiligen Spaltenangabe zu sortieren. Standardmäßig sind die Fehler absteigend nach der Anzahl der Instanzen geordnet.
   * Bewegen Sie den Cursor über das Feld „Antwort“ eines Fehlers, um die jeweilige Fehlermeldung anzuzeigen.
   * Bewegen Sie den Cursor über das Feld „URL“ oder „Referrer“, um den Link zum Bild oder der Referrer-Website anzuzeigen.
   * Klicken Sie auf „URL kopieren“, um den Link zum tatsächlichen Bild zu kopieren. Sie können diesen Link in ein Browserfenster kopieren, um das Bild aufzurufen und den Fehler zu prüfen.
   * Klicken Sie auf die zum Feld „Referrer“ gehörige Schaltfläche „URL kopieren“, um den Link zur Referrer-Website zu kopieren.

Die angezeigten Fehler betreffen das Unternehmen, bei dem Sie aktuell angemeldet sind. Jeder Fehler enthält die folgenden Informationen:

**Bild-ID** -ID für das fehlerhafte Bild.

**Zeit** Der Zeitraum, in dem der Fehler zum letzten Mal gemeldet wurde, wenn der Fehler in den letzten 24 Stunden gemeldet wurde.

**Zählt** die Anzahl der auf dem Bild gemeldeten Fehler.

**Antwort** Die spezifische Fehlermeldung. Fehler haben IDs, die mit 4xx oder 5xx beginnen.

**Urls** führen die URL für das Bild in Scene 7 aus.

**Referrer** Gibt die URL für die Website an, von der die ursprüngliche Anforderung stammt. Der Referrer kann jede Website sein, auf der ein Link zu dem Bild zu finden ist.

Für die Spalten „URL“ und „Referrer“ gibt es die Schaltfläche „URL kopieren“, um das Testen der URLs zu vereinfachen.
