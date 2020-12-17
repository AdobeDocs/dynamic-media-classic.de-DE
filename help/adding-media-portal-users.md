---
title: Hinzufügen und Verwalten von Media Portal-Benutzern
seo-title: Hinzufügen und Verwalten von Media Portal-Benutzern
description: 'null'
seo-description: Erfahren Sie, wie Sie Media Portal-Benutzer hinzufügen und verwalten
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 84%

---


# Hinzufügen und Verwalten von Media Portal-Benutzern{#adding-and-managing-media-portal-users}

Als Administrator können Sie Benutzer hinzufügen und verwalten, entscheiden, ob Benutzer Kennwörter ändern dürfen, Benutzerinformationen bearbeiten und Benutzerlisten hochladen. Diese Aufgaben werden im Anzeigebereich „Benutzerverwaltung“ ausgeführt. Um diesen Bildschirm aufzurufen, klicken Sie auf **[!UICONTROL „Einstellungen“]** > **[!UICONTROL „Anwendungseinstellungen“]** > **[!UICONTROL „Administrationseinstellungen“]** > **[!UICONTROL „Benutzerverwaltung“]**.

>[!NOTE]
>
>Bevor Sie Benutzer hinzufügen können, müssen Sie Gruppen einrichten, um die Benutzer zu verwalten. In Media Portal können Benutzer nur hinzugefügt werden, wenn sie gleichzeitig einer oder mehreren Gruppen zugewiesen werden. Weitere Informationen finden Sie unter [Erstellen und Verwalten von Media Portal-Gruppen](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Handhabung von Media Portal-Kennwörtern  {#handling-media-portal-passwords}

Media Portal-Benutzer, -Mitarbeiter und -Mitarbeiter-Benutzer erhalten eine E-Mail mit einem Kennwort, wenn Sie sie anmelden. Administratoren können entscheiden, ob Media Portal-Benutzer dieses Kennwort ändern dürfen.

1. Klicken Sie auf **[!UICONTROL „Einstellungen“]** > **[!UICONTROL „Media Portal-Einrichtung“]** > **[!UICONTROL „Allgemeine Einstellungen“]**.
1. Auf der Seite „Allgemeine Einstellungen“ können Sie **[!UICONTROL „Kennwortänderung durch MediaPortal-Benutzer zulassen“]** aktivieren oder deaktivieren.
1. Klicken Sie auf „**[!UICONTROL Speichern]**“.

>[!NOTE]
>
>Media Portal-Benutzer, die Kennwörter ändern dürfen, klicken auf **[!UICONTROL „Einstellungen“]** > **[!UICONTROL „Persönliche Einstellungen“]** und ändern Kennwörter im Bildschirm „Persönliche Einstellungen“.

## Hinzufügen eines Media Portal-Benutzers  {#adding-a-media-portal-user}

1. Klicken Sie auf **[!UICONTROL „Einstellungen“]** > **[!UICONTROL „Anwendungseinstellungen“]** > **[!UICONTROL „Administrationseinstellungen“]** > **[!UICONTROL „Benutzerverwaltung“]**.
1. Klicken Sie auf der Seite „Benutzerverwaltung“ auf **„Hinzufügen“**.
1. Geben Sie im Dialogfeld „Benutzer hinzufügen“ im Bedienfeld „Benutzerinformationen“ den Vornamen, Nachnamen und die E-Mail-Adresse des Benutzers ein und klicken Sie dann auf **[!UICONTROL „Weiter“]**.
1. Wählen Sie im Bedienfeld „Unternehmen/Rolle“ aus der Dropdown-Liste „Unternehmen“ ein oder mehrere Unternehmen für den Benutzer aus.
1. Wählen Sie in der Liste „Rolle“ eine Media Portal-Rolle aus und klicken Sie dann auf **[!UICONTROL „Weiter“]**.

   Siehe [Media Portal-Benutzerrollen](media-portal-user-roles.md#media_portal_user_roles).

1. Wählen Sie im Bedienfeld „Auf Gruppen zugreifen“ mindestens eine Gruppe aus.

   Siehe [Erstellen und Verwalten von Media Portal-Gruppen](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Optional) Klicken Sie auf **[!UICONTROL „E-Mail-Einstellungen“]**, um von den Standardeinstellungen abweichende E-Mail-Einstellungen auszuwählen.

   Siehe [Einrichten der Begrüßungs-E-Mail für Media Portal-Benutzer](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Klicken Sie auf **[!UICONTROL „Benutzer hinzufügen“]**.

Nachdem ein Benutzer hinzugefügt wurde, erhält er von Media Portal eine Begrüßungs-E-Mail. Die Nachricht enthält ein temporäres Passwort und die Media Portal-URL.

## Hochladen einer Media Portal-Benutzerliste  {#uploading-a-media-portal-user-list}

Um viele Benutzer gleichzeitig hinzuzufügen, können Sie eine Benutzerliste hochladen. Die Benutzer werden automatisch dem derzeit ausgewählten Konto hinzugefügt.

Erstellen Sie die Benutzerliste mit den Benutzerdaten als CSV-Datei (kommagetrennte Werte). Nach dem Hochladen der Liste werden die Benutzer in der Liste dem Konto automatisch mit ihren angegebenen Gruppenzuweisungen hinzugefügt. Jeder Benutzer erhält eine Begrüßungs-E-Mail mit einer Verknüpfung zum Media Portal und einem temporären Kennwort.

### Erstellen der CSV-Datei  {#creating-the-csv-file}

Erstellen Sie eine CSV-Datei (dateiname.csv), die dem folgenden Format entspricht. In der ersten Zeile der Datei müssen die in dieser Tabelle aufgelisteten Spaltenüberschriften enthalten sein. Die Sortierung der Spalten ist unerheblich. Alle Spalten sind erforderlich.

| Spaltenname | Beschreibung |
|--- |--- |
| Vorname | Der Vorname. |
| Nachname | Der Nachname. |
| E-Mail an Freunde senden | Eine gültige E-Mail-Adresse. |
| Kennwort | Ein Kennwort (auf Groß-/Kleinschreibung achten). |
| Benutzerrolle | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorUser |
| Gruppen | Auflistung aller dem Benutzer zugewiesenen Gruppen (durch Kommas getrennt). Geben Sie die Gruppe an, indem Sie vor dem Kontonamen einen Schrägstrich (/) einfügen. Beispiel: PortalCo/IT. „PortalCo“ ist das Konto und „IT“ ist die Gruppe innerhalb des PortalCo-Kontos. |

Die folgende Beispieltabelle zeigt, wie eine CSV-Datei aussehen muss:

| Vorname | Nachname | E-Mail an Freunde senden | Kennwort | Benutzerrolle | Gruppen |
|--- |--- |--- |--- |--- |--- |
| Peter | Peterson | `petep@company.com` | willkommen | Media Portal-Administrator | PortalCo/IT,PortalCo/Admin |
| Kevin | Marks | `kevinm@myco.com` | willkommen | Media Portal-Benutzer | PortalCo/MktgGroup, PortalCo/test |


### Hochladen der CSV-Datei  {#uploading-the-csv-file}

1. Öffnen Sie unter „Einstellungen“ den Anzeigebereich „Benutzerverwaltung“.
1. Klicken Sie auf **[!UICONTROL „Benutzerliste hochladen“]**.
1. Wählen Sie im Dialogfeld „Datei zum Hochladen auswählen“ die CSV-Datei aus und klicken Sie dann auf **[!UICONTROL „Öffnen“]**.

Alle Benutzer in der Liste werden automatisch den angegebenen Gruppen hinzugefügt. Jeder Benutzer erhält eine Begrüßungs-E-Mail.

>[!NOTE]
>
>Wenn die CSV-Datei nicht ordnungsgemäß formatiert war, wird die folgende Fehlermeldung angezeigt: „Bei der Verarbeitung der hochgeladenen CSV-Datei ist ein Fehler aufgetreten. Überprüfen Sie den Inhalt der Datei auf gültige Daten.“ Wenn die CSV-Datei einen vorhandenen IP- oder IPS-Benutzer enthält, wird dieser nicht der Benutzerliste hinzugefügt.

## Generieren einer auswählbaren Media Portal-Benutzerliste  {#generating-a-selectable-list-of-media-portal-users}

Sie können die Namen und E-Mail-Adressen von Media Portal-Benutzern in einem Popup-Fenster anzeigen. Dies ist nützlich, wenn Sie Benutzernamen und Adressen kopieren und in eine Anwendung außerhalb von Media Portal einfügen möchten.

1. Klicken Sie auf **[!UICONTROL „Einstellungen“]** > **[!UICONTROL „Anwendungseinstellungen“]** > **[!UICONTROL „Administrationseinstellungen“]** > **[!UICONTROL „Benutzerverwaltung“]**.
1. Wählen Sie in der Dropdown-Liste **[!UICONTROL „Nach Benutzerrolle“]** eine Media Portal-Rolle aus und klicken Sie auf **[!UICONTROL „Aktualisieren“]**, um die Namen einer Klasse von Media Portal-Benutzern anzuzeigen.
1. Klicken Sie auf **[!UICONTROL „Popup-Liste“]**, um das Popup-Fenster zu öffnen. Sie können diese Liste kopieren und einfügen.

## Einrichten der Begrüßungs-E-Mail für Media Portal-Benutzer  {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Sie können eine Begrüßungs-E-Mail an neue Media Portal-Benutzer, -Mitarbeiter und -Mitarbeiter-Benutzer senden lassen, die Sie hinzufügen. Sie können diese E-Mail-Nachricht konfigurieren oder Dynamic Media Classic anweisen, sie nicht zu senden.

1. Wählen Sie **[!UICONTROL „Einstellungen“]** > **[!UICONTROL „Anwendungseinstellungen“]** > **[!UICONTROL „Administrationseinstellungen“]** > **[!UICONTROL „Benutzerverwaltung“]**.
1. Klicken Sie im Bildschirm &quot;Benutzerverwaltung&quot;auf **[!UICONTROL E-Mail-Einstellungen]**.
1. Nehmen Sie im Dialogfeld „E-Mail-Einstellungen“ folgende Einstellungen vor:

   **[!UICONTROL Senden Sie]** E-MailDeaktivieren Sie diese Option, wenn Sie neue Benutzer nicht per E-Mail darüber informieren möchten, dass Sie sie registriert haben.

   **[!UICONTROL Standardkennwort]** Geben Sie ein temporäres Kennwort für neue Benutzer ein oder lassen Sie das Feld leer, damit Dynamic Media Classic zufällige Kennwörter generiert. Benutzer werden bei der ersten Anmeldung gebeten, ihr Kennwort zu ändern.

   **[!UICONTROL Ersatz-]** URLEngeben Sie eine URL ein, die sich vom Standard unterscheidet, wenn Ihre Benutzer über eine andere URL auf Dynamic Media Classic zugreifen.

## Andere Aufgaben zur Benutzerverwaltung {#other-user-management-tasks}

Über den Anzeigebereich „Benutzerverwaltung“ können Sie außerdem folgende Aufgaben ausführen:

**[!UICONTROL Filtern und Sortieren der]** Benutzerliste Filtern Sie die Liste der Media Portal-Benutzer, um Benutzer zu suchen. Siehe Filtern und Sortieren der Benutzerliste.

**[!UICONTROL Löschen von]** BenutzernLöschen eines Benutzers aus der Liste Siehe Löschen von Benutzern.

**[!UICONTROL Aktivieren und Deaktivieren von]** BenutzernBenutzer am Zugriff auf Ordner hindern Siehe Aktivieren und Deaktivieren von Benutzern.

**[!UICONTROL Bearbeiten]** von BenutzerinformationenGeben Sie aktuelle Informationen zu einem Benutzer ein. Siehe Bearbeiten von Benutzerinformationen.

**[!UICONTROL Erstellen benutzerdefinierter]** FelderErstellen Sie benutzerdefinierte, benutzerdefinierte Metadatenfelder, um Assets in Dynamic Media Classic zu organisieren. Die Felder können bei Bedarf auch aktiviert oder deaktiviert werden.

Siehe [Benutzerdefinierte Felder](application-setup.md#user_defined_fields).
