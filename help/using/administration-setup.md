---
title: Administrationseinrichtung
description: Erfahren Sie, wie Sie den Verwaltungsbereich von Adobe Dynamic Media Classic einrichten.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
topic: Administration
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '1974'
ht-degree: 32%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# Administrationseinstellungen{#administration-setup}

Die Bildschirme &quot;Administrationseinstellungen&quot;dienen der Verwaltung von Adobe Dynamic Media Classic-Benutzern. Verwenden Sie diese Bildschirme, um Benutzern die Arbeit in Adobe Dynamic Media Classic zu ermöglichen und per E-Mail mit anderen Benutzern zu kommunizieren.

1. Um auf die Optionen für Administrationseinstellungen zuzugreifen, gehen Sie zu **Einrichtung** > **Persönliche Einstellungen** > **Administrationseinstellungen**.

## Benutzerverwaltung {#user-administration}

Allen Adobe Dynamic Media Classic-Benutzern wird eine Rolle zugewiesen, die ihre Berechtigungen und Zugriffsrechte für Funktionen in Adobe Dynamic Media Classic bestimmt. Administratoren legen die verschiedenen Rollen und Verantwortungsbereiche für die Unternehmen fest, denen sie zugewiesen sind.

In der Regel konfiguriert Adobe Dynamic Media Classic die erste Gruppe von Unternehmen und weist einen Unternehmensadministrator zu. Der Unternehmensadministrator richtet dann Adobe Dynamic Media Classic-Benutzer ein und verwaltet sie.

Adobe Dynamic Media Classic unterstützt mehrere Benutzerrollen. Diese Rollen können auf Unternehmen zugreifen, die für die Adobe Dynamic Media Classic eingerichtet sind:

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic-Benutzer** Kann auf Unternehmen zugreifen, denen er zugewiesen wurde. Er kann keine Administratoraufgaben ausführen.

**Adobe Dynamic Media Classic-Unternehmensadministrator** Kann nur eigene Unternehmen anzeigen und verwalten. Ein Unternehmensadministrator kann außerdem alle Verwaltungsfunktionen ausführen, einschließlich des Hinzufügens von Administratoren und Benutzern. Ein Unternehmensadministrator kann einen Benutzer zu den DMC-Unternehmensadministratorkonten hinzufügen. (Dies ist die Standard-Benutzerrolle.)

Nachdem Sie einen Benutzer hinzugefügt haben, sendet Adobe Dynamic Media Classic dem Benutzer eine Begrüßungs-E-Mail. Die Nachricht enthält ein Kennwort und die Adobe Dynamic Media Classic-URL.

### Hinzufügen eines Benutzers oder Administrators {#adding-a-user-or-administrator}

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Administrationseinstellungen]** > **[!UICONTROL Benutzerverwaltung]**.
1. Wählen Sie **[!UICONTROL Hinzufügen]** aus.
1. Geben Sie den Namen und die E-Mail-Adresse des Benutzers oder Administrators ein, den Sie hinzufügen möchten, und wählen Sie dann **[!UICONTROL Weiter]** aus.

   >[!NOTE]
   >
   >Das Apostroph-Zeichen (`'`) ist in E-Mail-Adressen nicht zulässig.

1. Um dem Benutzer eine Rolle zuzuweisen, wählen Sie die Option Rolle aus.

   Siehe [Benutzerrollen und -berechtigungen für Adobe Dynamic Media Classic](administration-setup.md#user_administration).

1. Um einem Unternehmen einen Benutzer hinzuzufügen, wählen Sie einen Unternehmensnamen aus.
1. Wenn Sie den Benutzer einer Gruppe hinzufügen möchten (wenn Sie einen Media Portal-Benutzer oder -Mitarbeiter hinzufügen), wählen Sie **[!UICONTROL Weiter]** aus und fügen Sie den Benutzer hinzu.
1. Wählen Sie **[!UICONTROL Speichern]** aus, um die Benutzereinrichtung abzuschließen.

   Nach dem Speichern werden Sie gefragt, ob Sie einem anderen Unternehmen einen Benutzer hinzufügen möchten. Wählen Sie **[!UICONTROL Hinzufügen]** aus, wenn Sie den Benutzer einem Unternehmen hinzufügen möchten.

   Allen neuen Benutzern wird ein zufällig generiertes Kennwort zugewiesen. Benutzer müssen Kennwörter bei der ersten Anmeldung bei der Adobe Dynamic Media Classic-Desktop-Applikation ändern.

   Die von Ihnen hinzugefügten neuen Benutzer erhalten eine Begrüßungs-E-Mail. Die E-Mail enthält ein temporäres Kennwort und erläutert, wie Sie sich bei Adobe Dynamic Media Classic anmelden.

   Wenn der Benutzer die Begrüßungs-E-Mail nicht erhält, bitten Sie ihn, die Adobe Dynamic Media Classic-Anmeldeseite (https://s7sps1.scene7.com) aufzurufen und **[!UICONTROL Mein Kennwort vergessen]** auszuwählen. Das Kennwort wird zurückgesetzt und es wird eine neue E-Mail gesendet. Wenn der Benutzer auch diese E-Mail nicht erhält und sie nicht in seinem Spam-Ordner ist, wenden Sie sich an den technischen Support.

   Wenn Sie neue Media Portal-Benutzer hinzufügen, können Sie auch &quot;**[!UICONTROL Setup]**&quot;> &quot;**[!UICONTROL Anwendungseinstellungen]**&quot;> &quot;**[!UICONTROL Benutzerverwaltung]**&quot;, dann &quot;**[!UICONTROL Benutzerliste hochladen]**&quot;und eine CSV-Datei mit höchstens 500 Benutzern auswählen.

### Löschen eines Benutzers {#delet-a-user}

Sie können Benutzer aus Adobe Dynamic Media Classic löschen, indem Sie sie ungültig machen. Ungültige Benutzer werden aus dem System und sämtlichen Konten entfernt.

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Administrationseinstellungen]** > **[!UICONTROL Benutzerverwaltung]**.
1. Wählen Sie einen Benutzer aus der Liste und dann **[!UICONTROL Bearbeiten]** aus.
1. Deaktivieren Sie „Gültig“.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

### Benutzer aktivieren oder deaktivieren {#activating-or-deactivating-users}

Benutzer, die deaktiviert wurden, können nicht mehr auf das oben im Menü „Konto zum Zugreifen auswählen“ aufgelistete Konto zugreifen.

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Administrationseinstellungen]** > **[!UICONTROL Benutzerverwaltung]**.
1. Aktivieren oder deaktivieren Sie in der Benutzerliste die Option **[!UICONTROL Aktiv]** neben dem Namen des Benutzers.

### Bearbeiten von Benutzerinformationen {#editing-user-information}

Welche Benutzerinformationen Sie bearbeiten können, hängt von Ihrer Rolle als Administrator und der zugewiesenen Rolle der Benutzer ab, deren Angaben Sie bearbeiten möchten. Abgeblendete Optionen (nicht verfügbar) sind nicht bearbeitbar.

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Administrationseinstellungen]** > **[!UICONTROL Benutzerverwaltung]**.
1. Wählen Sie einen Benutzer aus der Liste und dann **[!UICONTROL Bearbeiten]** aus.
1. Wählen Sie den Eintrag in der Tabelle aus, der das Unternehmen anzeigt, für das Sie Berechtigungen oder Zugriff ändern möchten, und wählen Sie dann **[!UICONTROL Unternehmen verwalten]** aus.
1. Wählen Sie die Benutzerrolle aus.
1. Wenn Sie die Gruppenmitgliedschaft des Benutzers ändern möchten (wenn Sie einen Media Portal-Benutzer oder -Mitarbeiter bearbeiten oder hinzufügen), wählen Sie **[!UICONTROL Weiter]** aus und bearbeiten Sie die Gruppenmitgliedschaft.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

### Filtern und Sortieren der Benutzerliste {#filtering-and-sorting-the-user-list}

Sie können die Benutzerliste sortieren und filtern, um Benutzer zu suchen. Alle Benutzer sämtlicher von Ihnen verwalteten Konten werden in der Benutzerliste aufgelistet, unabhängig von dem im Menü „Konto zum Zugreifen auswählen“ ausgewählten Konto.

Sie können die folgenden Methoden zum Filtern von Benutzerlisten verwenden:

* **Nach Gruppe filtern**: Wählen Sie das Menü **[!UICONTROL Nach Gruppe]** aus und wählen Sie eine Option, um die Liste auf Benutzer in einer Gruppe zu beschränken.

* **Nach Benutzerrolle filtern**: Wählen Sie das Menü **[!UICONTROL Nach Benutzerrolle]** aus und wählen Sie eine Option, um die Liste auf Benutzer oder Administratoren unterschiedlicher Typen zu beschränken.

* **Filtern nach Feldname**: Wählen Sie **[!UICONTROL Filtern nach Feld aktivieren]** aus. Wählen Sie dann das Menü **[!UICONTROL Nach Feldname]** aus, wählen Sie eine Spalte zum Filtern der Liste, wählen Sie das Menü &quot;Zeichen filtern&quot;und wählen Sie einen Brief aus. Die Liste wird anhand des ausgewählten Briefs nach einer der Spalten gefiltert. Um die vollständige Liste anzuzeigen, deaktivieren Sie die Option **[!UICONTROL Filter nach Feld aktivieren]** .

* **Ungültige Benutzer herausfiltern**: Deaktivieren Sie **[!UICONTROL Ungültige einschließen]**. In den Suchergebnissen werden nur Benutzer aufgelistet, die im System vorhanden sind. Ungültige Benutzer wurden aus dem System und den von Ihnen verwalteten Konten gelöscht.

* **Sortieren nach Spaltenüberschrift**: Wählen Sie eine Überschrift aus, um alle Benutzer nach ihrem Status, alphabetisch nach Vorname, Nachname oder E-Mail-Adresse zu sortieren. Oder sortieren Sie nach Benutzerrolle oder nach dem gültigen/ungültigen Status.

Wenn Sie mit sehr vielen Benutzern arbeiten, können Sie im Menü „Max. Listengr.“ eine Zahl eingeben, um die Länge der Liste zu beschränken.

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to an Adobe Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to an Adobe Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Adobe Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Select **Manage Organizations**.
1. Select **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Select **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Adobe Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, select **Solutions** > **Experience Manager**. Under the Adobe Dynamic Media Classic card, select **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace "N" in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## Bandbreite und Speicher {#bandwidth-storage}

Adobe Dynamic Media Classic-Administratoren können für die von ihnen verwalteten Unternehmen Bandbreite, Speicherplatz und andere Berichtstypen generieren. Diese Berichte sind auf der Seite &quot;Bandbreite und Speicher&quot;verfügbar.

Um diese Seite zu öffnen, gehen Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Persönliche Einstellungen]**. Erweitern Sie **[!UICONTROL Administrationseinstellungen]** und wählen Sie dann **[!UICONTROL Bandbreite und Speicher]** aus.

### Berichtstypen {#types-of-reports}

In der folgenden Tabelle werden die Berichte beschrieben, die Sie auf der Seite &quot;Bandbreite und Speicher&quot;generieren können:

| Bericht | Information | Verwendung |
|:--- |:--- |:--- |
| Bandbreite | Bandbreitennutzung nach Unternehmen | Verfolgen Sie die Bandbreitennutzung nach Unternehmen über bestimmte Zeitspannen, um Datenverkehrsmuster zu ermitteln. |
| Speicher | Speicherverwendung | Verfolgen Sie die Menge der vom Unternehmen hochgeladenen Daten. |
| Bildinhalt | Die Anzahl der Bildanfragen nach Typ | Verfolgen Sie die Anzahl der Anfragen nach und das Volumen für verschiedene Bildtypen. |
| Domäne | Die Anzahl der URL-Anfragen nach Domäne | Verfolgen Sie die Bildernutzung auf der Basis der Domäne der Bildanfragen eines bestimmten Unternehmens. (Adobe Dynamic Media Classic kann mehr als eine Domäne pro Konto bereitstellen. Weitere Informationen erhalten Sie vom technischen Support.) |
| Video-Streaming | Bandbreitennutzung für Streaming-Videos | Verfolgen Sie die Nutzung von Streaming-Videos nach Unternehmen über bestimmte Zeitspannen, um Datenverkehrsmuster zu ermitteln. |
| Videoinhalt | Wiedergabezeit verschiedener Videos | Ermitteln Sie, welche Videos am häufigsten und am wenigsten häufig abgerufen werden. |

Der Bericht „Bildinhalt“ enthält Informationen über Anforderungen nach den folgenden Bildtypen:

* **Bildanforderung**: Anforderungen für Bilder.

* **Miniaturanfrage**: Anforderungen für Muster oder alternative Bilder in Viewern.

* **Maskenanforderung**: Anforderungen an Bilder, die Graustufenmasken zurückgeben.

* **Anforderung der Viewer-Kachel**: Von einem Viewer geladene Bildanforderungen.

* **VNT Object Request**: Bildwiedergabeanforderungen, die ein Bild mit bestimmten Objekten in den angeforderten Vignetten zurückgeben.

* **VNT Info Request**: Image Rendering-Anfragen, die Informationen zu den angeforderten Vignetten zurückgeben.

>[!NOTE]
>
>Der Bericht zu Video-Streaming bezieht nur Streaming-Videos mit ein. Die Anzeige progressiver Videos wird nicht verfolgt.

### Bericht erstellen {#generating-a-report}

So generieren Sie einen Bericht zur Bandbreite, zum Speicher, zu Bildinhalt, zur Domäne, zum Video-Streaming oder zu Videoinhalt:

1. Navigieren Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Persönliche Einstellungen]**.
1. Erweitern Sie die Administrationseinstellung und wählen Sie dann **[!UICONTROL Bandwidth &amp; Storage]** aus.
1. Wählen Sie eine Registerkarte aus: **[!UICONTROL Bandwidth]**, **[!UICONTROL Storage]**, **[!UICONTROL Image Content]**, **[!UICONTROL Domain]**, **[!UICONTROL Video Streaming]** oder **[!UICONTROL Video Content]**.

   Siehe [Berichtstypen](administration-setup.md#types_of_reports).

### Daten auf unterschiedliche Weise anzeigen {#viewing-data-in-different-ways}

Nachdem Sie einen Bericht auf der Seite „Bandbreite und Speicher“ generiert haben, können Sie Optionen zum Anzeigen der Informationen auswählen. Sie können festlegen, wie die Informationen dargestellt werden, die Informationen in einem Diagramm oder Datenraster anzeigen und einen Zeitraum für das Erfassen von Informationen bestimmen. In der Datenansicht können Sie die Informationen auch sortieren und in Spalten anordnen.

* **Daten in einem Diagramm oder Datenraster anzeigen**: Wählen Sie **[!UICONTROL Diagrammansicht]** aus, um Daten in einem Diagramm anzuzeigen. Wählen Sie **[!UICONTROL Datenansicht]** aus, um Daten in einem Datenraster anzuzeigen.

* **Wählen Sie einen Präsentationstyp des Berichts aus**: Wählen Sie im Menü &quot;Berichtstyp&quot;die Option **[!UICONTROL Zusammenfassung]**, **[!UICONTROL Täglich]** oder **[!UICONTROL Monatlich]** aus, um die Daten in Form einer Zusammenfassung, nach Tag oder nach Monat zu organisieren. Diese Option steht nicht in allen Berichten zur Verfügung.

* **Legen Sie einen Zeitraum fest**: Wählen Sie Optionen aus, um einen Zeitraum für Ihren Bericht zu definieren, und wählen Sie dann **[!UICONTROL Aktualisieren]** aus, nachdem Sie einen Zeitraum definiert haben:

* **Vordefinierter Zeitraum**: Wählen Sie im Menü Vordefinierter Bericht eine Option aus. Wählen Sie beispielsweise „Letzter Monat“, um die Daten des letzten Monats zu erfassen.

* **Benutzerdefinierter Zeitraum**: Wählen Sie im Menü Vordefinierter Bericht die Option **[!UICONTROL Benutzerdefiniert]** aus. Wählen Sie dann im Menü **[!UICONTROL Startmonat]** (oder **[!UICONTROL Startdatum]**) ein Datum und im Menü Anzahl der Monate (oder Tage) ein Datum aus. Für Berichte zur Domäne und zum Videoinhalt können Sie ein bestimmtes Start- und Enddatum für die Erfassung von Berichtsinformationen wählen.

* **Sortieren von Daten (nur Datenansicht)**: Sortieren Sie Informationen in einer Spalte. Wählen Sie die Überschrift der Spalte aus. Wählen Sie erneut aus, um in absteigender Reihenfolge zu sortieren.

* **Spalten neu anordnen (nur Datenansicht)**: Um eine Spalte an eine andere Position im Datenraster zu verschieben, ziehen Sie die Überschrift.

### Exportieren und Drucken von Berichten {#exporting-and-printing-reports}

Nachdem Sie einen Bericht generiert haben, können Sie die Daten für die Verwendung in Tabellen und anderen Anwendungen exportieren. Sie können die Berichte auch ausdrucken.

* **Berichtdaten exportieren**: Sortieren und ordnen Sie die Daten in der Datenansicht nach Bedarf an. Öffnen Sie dann das Menü **[!UICONTROL Exportieren]** und wählen Sie ein Format: **[!UICONTROL Tabulatorgetrennt]**, **[!UICONTROL Kommagetrennt]** oder **[!UICONTROL HTML Formatiert]**. Die Daten werden in dem von Ihnen ausgewählten Format in die Zwischenablage kopiert. Jetzt können Sie die Daten in eine Tabelle oder Anwendung einfügen.

* **Einen Bericht drucken**: Wählen Sie **[!UICONTROL Drucken]**, wählen Sie die gewünschten Optionen im Dialogfeld &quot;Drucken&quot;aus und klicken Sie auf **[!UICONTROL OK]**.

## Bildfehler {#image-errors}

Adobe Dynamic Media Classic-Administratoren können Bildfehlerberichte generieren. Ein Bildfehlerbericht zeigt eine Liste der 20 häufigsten Bildfehler in den letzten 24 Stunden für das Unternehmen an, bei dem Sie derzeit angemeldet sind. Gehen Sie wie folgt vor, um einen Bildfehlerbericht zu generieren:

1. Navigieren Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Persönliche Einstellungen]**.
1. Erweitern Sie die Administrationseinstellungen und wählen Sie dann **[!UICONTROL Bildfehler]** aus.
1. (Optional) Führen Sie dann einen der folgenden Schritte aus:

   * Um Fehler anhand der Überschrifteninformationen zu sortieren, wählen Sie eine Überschrift aus. Standardmäßig sind die Fehler absteigend nach der Anzahl der Instanzen geordnet.
   * Bewegen Sie den Cursor über das Feld „Antwort“ eines Fehlers, um die jeweilige Fehlermeldung anzuzeigen.
   * Um den Link zum Bild oder zur Referrer-Webseite anzuzeigen, bewegen Sie den Cursor über das URL-Feld oder das Referrer-Feld.
   * Um den Link zum tatsächlichen Bild zu kopieren, wählen Sie **[!UICONTROL URL kopieren URL]** aus. Sie können diesen Link in ein Browserfenster kopieren, um das Bild aufzurufen und den Fehler zu prüfen.
   * Um den Link auf die Webseite des Referrers zu kopieren, wählen Sie **[!UICONTROL URL des Referrers kopieren]** aus.

Die angezeigten Fehler beziehen sich auf das Unternehmen, bei dem Sie derzeit angemeldet sind. Jeder Fehler enthält die folgenden Informationen:

* **Bild-ID**: ID für das fehlerhafte Bild.

* **Zeit**: Der Zeitraum, in dem der Fehler zum ersten Mal innerhalb der letzten 24 Stunden gemeldet wurde, als der Fehler zuletzt gemeldet wurde.

* **Zählung**: Die Anzahl der Fehler, die im Bild gemeldet werden.

* **Antwort**: Die spezifische Fehlermeldung. Fehler haben IDs, die mit 4xx oder 5xx beginnen.

* **URLs**: Listet die URL zum Bild in Adobe Dynamic Media Classic auf.

* **Referrer**: Gibt die URL für die Website an, von der die erste Anforderung stammt. Der Referrer kann jede Website sein, die über einen Link zum Bild verfügt.

Für die Spalten „URL“ und „Referrer“ gibt es die Schaltfläche „URL kopieren“, um das Testen der URLs zu vereinfachen.
