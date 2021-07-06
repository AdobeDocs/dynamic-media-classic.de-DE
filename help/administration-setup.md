---
title: Administrationseinstellungen
description: Erfahren Sie, wie Sie den Administrationsbereich von Dynamic Media Classic einrichten.
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1935'
ht-degree: 41%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Administrationseinstellungen{#administration-setup}

Die Bildschirme &quot;Administrationseinstellungen&quot;dienen der Verwaltung von Dynamic Media Classic-Benutzern. Verwenden Sie diese Bildschirme, um Benutzern die Arbeit in Dynamic Media Classic zu ermöglichen und per E-Mail mit Benutzern zu kommunizieren.

1. Um auf die Optionen für Administrationseinstellungen zuzugreifen, klicken Sie auf **Setup** > **Persönliche Einstellungen** > **Administrationseinstellungen**.

## Benutzerverwaltung {#user-administration}

Allen Benutzern von Dynamic Media Classic wird eine Rolle zugewiesen, die ihre Berechtigungen und Zugriffsrechte für Funktionen in Dynamic Media Classic bestimmt. Administratoren legen die verschiedenen Rollen und Verantwortungsbereiche für die Unternehmen fest, denen sie zugewiesen sind.

In der Regel konfiguriert Dynamic Media Classic den ersten Satz von Unternehmen und weist einen Unternehmensadministrator zu. Der Unternehmensadministrator richtet dann Dynamic Media Classic-Benutzer ein und verwaltet sie.

Dynamic Media Classic unterstützt mehrere Benutzerrollen. Diese Rollen können auf Unternehmen zugreifen, die für Dynamic Media Classic eingerichtet sind:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic** UserKann auf Unternehmen zugreifen, denen sie zugewiesen wurden; keine Verwaltungsaufgaben wahrnehmen können.

**Adobe Dynamic Media Classic Company** AdminKann nur eigene Unternehmen anzeigen und verwalten. Ein Unternehmensadministrator kann außerdem alle Verwaltungsfunktionen ausführen, einschließlich des Hinzufügens von Administratoren und Benutzern. Ein Unternehmensadministrator kann einen Benutzer zu den DMC-Unternehmensadministratorkonten hinzufügen. (Dies ist die Standard-Benutzerrolle.)

Nachdem Sie einen Benutzer hinzugefügt haben, sendet Dynamic Media Classic eine Begrüßungs-E-Mail an den Benutzer. Die Nachricht enthält ein Kennwort und die Dynamic Media Classic-URL.

### Hinzufügen eines Benutzers oder Administrators {#adding-a-user-or-administrator}

1. Klicken Sie auf **[!UICONTROL „Einstellungen“]** > **[!UICONTROL „Anwendungseinstellungen“]** > **[!UICONTROL „Administrationseinstellungen“]** > **[!UICONTROL „Benutzerverwaltung“]**.
1. Klicken Sie auf **[!UICONTROL „Hinzufügen“]**.
1. Geben Sie den Namen und die E-Mail-Adresse des Benutzers oder Administrators ein, den Sie hinzufügen möchten, und klicken Sie dann auf **[!UICONTROL Weiter]**.

   >[!NOTE]
   >
   >Das Apostroph-Zeichen (`‘`) ist in E-Mail-Adressen nicht zulässig.

1. Um dem Benutzer eine Rolle zuzuweisen, wählen Sie die Option Rolle aus.

   Siehe [Dynamic Media Classic-Benutzerrollen und -berechtigungen](administration-setup.md#user_administration).

1. Um einem Unternehmen einen Benutzer hinzuzufügen, wählen Sie einen Unternehmensnamen aus.
1. Wenn Sie den Benutzer einer Gruppe hinzufügen möchten (wenn Sie einen Media Portal-Benutzer oder -Mitarbeiter hinzufügen), klicken Sie auf **[!UICONTROL Weiter]** und fügen Sie den Benutzer hinzu.
1. Klicken Sie auf **[!UICONTROL Save]** , um die Benutzereinrichtung abzuschließen.

   Nach dem Speichern werden Sie gefragt, ob Sie einem anderen Unternehmen einen Benutzer hinzufügen möchten. Klicken Sie auf **[!UICONTROL Hinzufügen]** , wenn Sie den Benutzer zu einem Unternehmen hinzufügen möchten.

   Allen neuen Benutzern wird ein zufällig generiertes Kennwort zugewiesen. Benutzer müssen Kennwörter bei der ersten Anmeldung bei der Dynamic Media Classic-Desktop-Applikation ändern.

   Die von Ihnen hinzugefügten neuen Benutzer erhalten eine Begrüßungs-E-Mail. Die E-Mail enthält ein temporäres Kennwort und erläutert, wie Sie sich bei Dynamic Media Classic anmelden.

   Wenn der Benutzer die Begrüßungs-E-Mail nicht erhält, bitten Sie ihn, die Dynamic Media Classic-Anmeldeseite (https://s7sps1.scene7.com) aufzurufen und auf &quot;Kennwort vergessen&quot;zu klicken. Das Kennwort wird zurückgesetzt und es wird eine neue E-Mail gesendet. Wenn der Benutzer auch diese E-Mail nicht erhält und sie nicht in seinem Spam-Ordner ist, wenden Sie sich an den technischen Support.

   Wenn Sie neue Media Portal-Benutzer hinzufügen, können Sie auch zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Benutzerverwaltung]** navigieren, dann auf **[!UICONTROL Benutzerliste hochladen]** klicken und eine CSV-Datei mit maximal 500 Benutzern auswählen.

### Löschen eines Benutzers {#deleting-a-user}

Sie können Benutzer aus Dynamic Media Classic löschen, indem Sie sie ungültig machen. Ungültige Benutzer werden aus dem System und sämtlichen Konten entfernt.

1. Klicken Sie auf **[!UICONTROL „Einstellungen“]** > **[!UICONTROL „Anwendungseinstellungen“]** > **[!UICONTROL „Administrationseinstellungen“]** > **[!UICONTROL „Benutzerverwaltung“]**.
1. Wählen Sie aus der Liste einen Benutzer aus und klicken Sie dann auf **[!UICONTROL „Bearbeiten“]**.
1. Deaktivieren Sie „Gültig“.
1. Klicken Sie auf „**[!UICONTROL Speichern]**“.

### Aktivieren oder Deaktivieren von Benutzern {#activating-or-deactivating-users}

Benutzer, die deaktiviert wurden, können nicht mehr auf das oben im Menü „Konto zum Zugreifen auswählen“ aufgelistete Konto zugreifen.

1. Klicken Sie auf **[!UICONTROL „Einstellungen“]** > **[!UICONTROL „Anwendungseinstellungen“]** > **[!UICONTROL „Administrationseinstellungen“]** > **[!UICONTROL „Benutzerverwaltung“]**.
1. Aktivieren oder deaktivieren Sie in der Benutzerliste die Option **[!UICONTROL Aktiv]** neben dem Namen des Benutzers.

### Bearbeiten von Benutzerinformationen {#editing-user-information}

Welche Benutzerinformationen Sie bearbeiten können, hängt von Ihrer Rolle als Administrator und der zugewiesenen Rolle der Benutzer ab, deren Angaben Sie bearbeiten möchten. Abgeblendete Optionen (nicht verfügbar) sind nicht bearbeitbar.

1. Klicken Sie auf **[!UICONTROL „Einstellungen“]** > **[!UICONTROL „Anwendungseinstellungen“]** > **[!UICONTROL „Administrationseinstellungen“]** > **[!UICONTROL „Benutzerverwaltung“]**.
1. Wählen Sie den Benutzer aus und klicken Sie auf **[!UICONTROL „Bearbeiten“]**.
1. Wählen Sie den Eintrag in der Tabelle aus, der das Unternehmen anzeigt, für das Sie Berechtigungen oder Zugriff ändern möchten, und klicken Sie dann auf **[!UICONTROL Unternehmen verwalten]**.
1. Wählen Sie die Benutzerrolle aus.
1. Wenn Sie die Gruppenmitgliedschaft des Benutzers ändern möchten (wenn Sie einen Media Portal-Benutzer oder -Mitarbeiter bearbeiten oder hinzufügen), klicken Sie auf **[!UICONTROL Weiter]** und bearbeiten Sie die Gruppenmitgliedschaft.
1. Klicken Sie auf „**[!UICONTROL Speichern]**“.

### Filtern und Sortieren der Benutzerliste {#filtering-and-sorting-the-user-list}

Sie können die Benutzerliste sortieren und filtern, um Benutzer zu suchen. Alle Benutzer sämtlicher von Ihnen verwalteten Konten werden in der Benutzerliste aufgelistet, unabhängig von dem im Menü „Konto zum Zugreifen auswählen“ ausgewählten Konto.

Sie können die folgenden Techniken zum Filtern der Benutzerliste verwenden:

* **Nach Gruppe filtern**  - Wählen Sie das Menü  **[!UICONTROL Nach]** Gruppierung aus und wählen Sie eine Option, um die Liste auf Benutzer in einer Gruppe einzuschränken.

* **Nach Benutzerrolle filtern**  - Wählen Sie das Menü  **[!UICONTROL Nach Benutzerrollen]** aus und wählen Sie eine Option, um die Liste auf Benutzer oder Administratoren unterschiedlicher Typen zu beschränken.

* **Filtern nach Feldname**  - Wählen Sie  **[!UICONTROL Filtern nach Feld aktivieren]** aus. Wählen Sie dann das Menü **[!UICONTROL Nach Feldname]** aus, wählen Sie eine Spalte zum Filtern der Liste, wählen Sie das Menü &quot;Zeichen filtern&quot;und wählen Sie einen Brief aus. Anschließend wird die Liste in der ausgewählten Spalte nach dem angegebenen Buchstaben gefiltert. Um die vollständige Liste anzuzeigen, deaktivieren Sie die Option **[!UICONTROL Filter nach Feld aktivieren]** .

* **Ungültige Benutzer herausfiltern**  - Deaktivieren Sie  **[!UICONTROL Ungültige einschließen]**. In den Suchergebnissen werden nur Benutzer aufgelistet, die im System vorhanden sind. Ungültige Benutzer wurden aus dem System und sämtlichen von Ihnen verwalteten Konten gelöscht.

* **Sortieren nach Spaltenüberschrift**  - Klicken Sie auf eine Überschrift, um alle Benutzer nach Status, alphabetisch nach Vorname, Nachname, E-Mail-Adresse, Benutzerrolle oder nach gültigem/ungültigem Status zu sortieren.

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

    * To launch Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, click **Solutions** > **Experience Manager**. Under the Dynamic Media Classic card, click **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Bandbreite und Speicher {#bandwidth-storage}

Dynamic Media Classic-Administratoren können für die von ihnen verwalteten Unternehmen Bandbreite, Speicher und andere Berichtstypen generieren. Diese Berichte sind auf der Seite Bandbreite und Speicher verfügbar.

Um diese Seite zu öffnen, klicken Sie auf **[!UICONTROL Setup]** > **[!UICONTROL Persönliche Einstellungen]**. Erweitern Sie **[!UICONTROL Administrationseinstellungen]** und klicken Sie dann auf **[!UICONTROL Bandbreite und Speicher]**.

### Berichtstypen {#types-of-reports}

In der folgenden Tabelle werden die Berichte beschrieben, die Sie auf der Seite &quot;Bandbreite und Speicher&quot;generieren können:

| Bericht | Information | Verwendung |
|:--- |:--- |:--- |
| Bandbreite | Bandbreitennutzung nach Unternehmen | Verfolgen Sie die Bandbreitennutzung nach Unternehmen über bestimmte Zeitspannen, um Datenverkehrsmuster zu ermitteln. |
| Speicher | Speicherverwendung | Verfolgen Sie die hochgeladene Datenmenge nach Unternehmen. |
| Bildinhalt | Die Anzahl der Bildanfragen nach Typ | Verfolgen Sie die Anzahl der Anfragen nach und das Volumen für verschiedene Bildtypen. |
| Domäne | Die Anzahl der URL-Anfragen nach Domäne | Verfolgen Sie die Bildernutzung auf der Basis der Domäne der Bildanfragen eines bestimmten Unternehmens. (Dynamic Media Classic kann mehr als eine Domäne pro Konto bereitstellen. Weitere Informationen erhalten Sie vom technischen Support.) |
| Video-Streaming | Bandbreitennutzung für Streaming-Videos | Verfolgen Sie die Nutzung von Streaming-Videos nach Unternehmen über bestimmte Zeitspannen, um Datenverkehrsmuster zu ermitteln. |
| Videoinhalt | Wiedergabezeit verschiedener Videos | Ermitteln Sie, welche Videos am häufigsten und am wenigsten häufig abgerufen werden. |

Der Bericht „Bildinhalt“ enthält Informationen über Anforderungen nach den folgenden Bildtypen:

* **Bildanforderung**  - Anforderungen für Bilder.

* **Miniaturanfrage**  - Anforderungen für Muster oder alternative Bilder in Viewern.

* **Maskenanforderung**  - Anforderungen an Bilder, die Graustufen-Masken zurückgeben.

* **Viewer-Kachelanforderung** : Bildanforderungen, die von einem Viewer geladen werden.

* **Vnt Object Request**  - Bildwiedergabeanforderungen, die ein Bild mit bestimmten Objekten in den angeforderten Vignetten zurückgeben.

* **Vnt Info Request**  - Bildrendering-Anfragen, die Informationen zu den angeforderten Vignetten zurückgeben.

>[!NOTE]
>
>Der Bericht zu Video-Streaming bezieht nur Streaming-Videos mit ein. Die Anzeige progressiver Videos wird nicht verfolgt.

### Generieren eines Berichts {#generating-a-report}

So generieren Sie einen Bericht zur Bandbreite, zum Speicher, zu Bildinhalt, zur Domäne, zum Video-Streaming oder zu Videoinhalt:

1. Wählen Sie **[!UICONTROL Setup]** > **[!UICONTROL Persönliche Einstellungen]**.
1. Erweitern Sie die Administrationseinstellung und klicken Sie dann auf **[!UICONTROL Bandwidth &amp; Storage]**.
1. Klicken Sie auf eine Registerkarte: **[!UICONTROL Bandbreite]**, **[!UICONTROL Speicher]**, **[!UICONTROL Bildinhalt]**, **[!UICONTROL Domäne]**, **[!UICONTROL Video-Streaming]** oder **[!UICONTROL Videoinhalt]**.

   Siehe [Berichtstypen](administration-setup.md#types_of_reports).

### Unterschiedliche Anzeige von Daten {#viewing-data-in-different-ways}

Nachdem Sie einen Bericht auf der Seite „Bandbreite und Speicher“ generiert haben, können Sie Optionen zum Anzeigen der Informationen auswählen. Sie können festlegen, wie die Informationen dargestellt werden, die Informationen in einem Diagramm oder Datenraster anzeigen und einen Zeitraum für das Erfassen von Informationen bestimmen. In der Datenansicht können Sie die Informationen auch sortieren und in Spalten anordnen.

* **Anzeigen von Daten in einem Diagramm oder Datenraster**  - Klicken Sie auf  **[!UICONTROL Diagrammansicht]** , um Daten in einem Diagramm anzuzeigen. Klicken Sie auf  **[!UICONTROL Datenansicht]** , um Daten in einem Datenraster anzuzeigen.

* **Auswahl des Präsentationstyps**  eines Berichts: Klicken Sie im Menü &quot;Berichtstyp&quot;auf  **[!UICONTROL Zusammenfassung]**,  **[!UICONTROL Täglich]** oder  **** Monat, um die Daten in Form einer Zusammenfassung, eines Tages oder eines Monats zu ordnen. Diese Option steht nicht in allen Berichten zur Verfügung.

* **Festlegen eines Zeitraums**  - Wählen Sie Optionen zum Definieren eines Zeitraums für Ihren Bericht aus und klicken Sie nach der Definition eines Zeitraums auf  **** Aktualisieren :

* **Vordefinierter Zeitraum**  - Wählen Sie im Menü Vordefinierter Bericht eine Option aus. Wählen Sie beispielsweise „Letzter Monat“, um die Daten des letzten Monats zu erfassen.

* **Benutzerdefinierter Zeitraum**  - Klicken Sie im Menü Vordefinierter Bericht auf  **[!UICONTROL Benutzerdefiniert]**. Wählen Sie anschließend ein Datum im Menü **[!UICONTROL Startmonat]** (oder **[!UICONTROL Startdatum]**) und ein Datum im Menü Anzahl der Monate (oder # oder Tage) aus. Für Berichte zur Domäne und zum Videoinhalt können Sie ein bestimmtes Start- und Enddatum für die Erfassung von Berichtsinformationen wählen.

* **Sortieren von Daten (nur Datenansicht)**  - Klicken Sie auf die Überschrift der Spalte, um Informationen zu einer Spalte zu sortieren. Bei erneutem Klicken wird die Sortierreihenfolge umgekehrt (absteigend).

* **Neuanordnen von Spalten (nur Datenansicht)**  - Um eine Spalte an eine andere Position im Datenraster zu verschieben, ziehen Sie die Überschrift.

### Exportieren und Drucken von Berichten {#exporting-and-printing-reports}

Nachdem Sie einen Bericht generiert haben, können Sie die Daten für die Verwendung in Tabellen und anderen Anwendungen exportieren. Sie können die Berichte auch ausdrucken.

* **Exportieren von Berichtsdaten**  - Sortieren und ordnen Sie die Daten in der Datenansicht nach Bedarf an. Öffnen Sie dann das Menü **[!UICONTROL Export]** und wählen Sie ein Format: **[!UICONTROL Tabulatorgetrennte]**, **[!UICONTROL Kommagetrennte]** oder **[!UICONTROL HTML-formatierte]**. Die Daten werden in dem gewünschten Format in die Zwischenablage kopiert. Jetzt können Sie die Daten in eine Tabelle oder Anwendung einfügen.

* **Drucken eines Berichts**  - Klicken Sie auf  **[!UICONTROL Drucken]**, wählen Sie die gewünschten Optionen im Dialogfeld &quot;Drucken&quot;aus und klicken Sie auf  **[!UICONTROL OK]**.

## Bildfehler {#image-errors}

Dynamic Media Classic-Administratoren können Bildfehlerberichte generieren. Ein Bildfehlerbericht zeigt eine Liste der 20 häufigsten Bildfehler in den letzten 24 Stunden für das Unternehmen an, bei dem Sie derzeit angemeldet sind. Gehen Sie wie folgt vor, um einen Bildfehlerbericht zu generieren:

1. Klicken Sie auf **[!UICONTROL Setup]** > **[!UICONTROL Persönliche Einstellungen]**.
1. Erweitern Sie die Administrationseinstellungen und klicken Sie dann auf **[!UICONTROL Bildfehler]**.
1. (Optional) Führen Sie dann einen der folgenden Schritte aus:

   * Klicken Sie auf eine Überschrift, um die Fehler nach den Überschrifteninformationen zu sortieren. Standardmäßig sind die Fehler absteigend nach der Anzahl der Instanzen geordnet.
   * Bewegen Sie den Cursor über das Feld „Antwort“ eines Fehlers, um die jeweilige Fehlermeldung anzuzeigen.
   * Um den Link zum Bild oder zur Referrer-Webseite anzuzeigen, bewegen Sie den Cursor über das URL-Feld oder das Referrer-Feld.
   * Um den Link zum tatsächlichen Bild zu kopieren, klicken Sie auf **[!UICONTROL URL kopieren URL]**. Sie können diesen Link in ein Browserfenster kopieren, um das Bild aufzurufen und den Fehler zu prüfen.
   * Um den Link auf die Referrer-Webseite zu kopieren, klicken Sie auf **[!UICONTROL Referrer Copy URL]**.

Die angezeigten Fehler betreffen das Unternehmen, bei dem Sie aktuell angemeldet sind. Jeder Fehler enthält die folgenden Informationen:

* **Bild-ID**  - ID für das fehlerhafte Bild.

* **Zeit**  - Der Zeitraum, in dem der Fehler zum ersten Mal in den letzten 24 Stunden gemeldet wurde, als der Fehler zuletzt gemeldet wurde.

* **Anzahl**  - Die Anzahl der Fehler, die im Bild gemeldet werden.

* **Antwort**  - Die spezifische Fehlermeldung. Fehler haben IDs, die mit 4xx oder 5xx beginnen.

* **URLs**  - Listet die URL zum Bild in Dynamic Media Classic auf.

* **Referrer**  - Gibt die URL für die Website an, von der die erste Anforderung stammt. Der Referrer kann jede Website sein, auf der ein Link zu dem Bild zu finden ist.

Für die Spalten „URL“ und „Referrer“ gibt es die Schaltfläche „URL kopieren“, um das Testen der URLs zu vereinfachen.
