---
title: Hinzufügen und Verwalten von Media Portal-Benutzern
description: Erfahren Sie, wie Sie Media Portal-Benutzer in Adobe Dynamic Media Classic hinzufügen und verwalten.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
topic: Administration
level: Intermediate
source-git-commit: bb229047c0c9b3855453ea15dcd1f9754bc65cef
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 50%

---

# Hinzufügen und Verwalten von Media Portal-Benutzern{#adding-and-managing-media-portal-users}

Als Administrator können Sie Benutzer hinzufügen und verwalten, entscheiden, ob Benutzer Kennwörter ändern dürfen, Benutzerinformationen bearbeiten und Benutzerlisten hochladen. Diese Aufgaben werden im Anzeigebereich „Benutzerverwaltung“ ausgeführt. Um auf diesen Bildschirm zuzugreifen, navigieren Sie zu &quot;**[!UICONTROL Setup]**&quot;> &quot;**[!UICONTROL Anwendungseinstellungen]**&quot;> &quot;**[!UICONTROL Administrationseinstellungen]**&quot;> &quot;**[!UICONTROL Benutzerverwaltung]**&quot;.

>[!NOTE]
>
>Bevor Sie Benutzer hinzufügen können, müssen Sie Gruppen einrichten, um die Benutzer zu verwalten. Mit Media Portal können Sie einen Benutzer hinzufügen, indem Sie ihn einer oder mehreren Gruppen zuweisen. Weitere Informationen finden Sie unter [Erstellen und Verwalten von Media Portal-Gruppen](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Verwaltung von Media Portal-Passwörtern {#handling-media-portal-passwords}

Media Portal-Benutzer, -Mitarbeiter und -Mitarbeiter-Benutzer erhalten eine E-Mail mit einem Kennwort, wenn Sie sie anmelden. Administratoren können entscheiden, ob Media Portal-Benutzer dieses Kennwort ändern dürfen.

1. Navigieren Sie zu &quot;**[!UICONTROL Setup]**&quot;> &quot;**[!UICONTROL Media Portal-Einrichtung]**&quot;> &quot;**[!UICONTROL Allgemeine Einstellungen]**&quot;.
1. Auf der Seite „Allgemeine Einstellungen“ können Sie **[!UICONTROL „Kennwortänderung durch MediaPortal-Benutzer zulassen“]** aktivieren oder deaktivieren.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

>[!NOTE]
>
>Media Portal-Benutzer, die Kennwörter ändern dürfen, können dies tun, indem sie **[!UICONTROL Einstellungen]** > **[!UICONTROL Persönliche Einstellungen]** auswählen und Kennwörter auf dem Bildschirm &quot;Persönliche Einstellungen&quot;ändern.

## Hinzufügen eines Media Portal-Benutzers {#adding-a-media-portal-user}

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Administrationseinstellungen]** > **[!UICONTROL Benutzerverwaltung]**.
1. Wählen Sie auf der Seite &quot;Benutzerverwaltung&quot;die Option **Hinzufügen**.
1. Geben Sie im Dialogfeld **[!UICONTROL `Add User`]** im Bedienfeld &quot;Benutzerinformationen&quot;den Vornamen, Nachnamen und die E-Mail-Adresse des Benutzers ein und wählen Sie dann **[!UICONTROL Weiter]** aus.
1. Wählen Sie im Bedienfeld „Unternehmen/Rolle“ aus der Dropdown-Liste „Unternehmen“ ein oder mehrere Unternehmen für den Benutzer aus.
1. Wählen Sie in der Liste &quot;Rolle&quot;eine Media Portal-Rolle und dann **[!UICONTROL Weiter]** aus.

   Siehe [Media Portal-Benutzerrollen](media-portal-user-roles.md#media_portal_user_roles).

1. Wählen Sie im Bedienfeld „Auf Gruppen zugreifen“ mindestens eine Gruppe aus.

   Siehe [Erstellen und Verwalten von Media Portal-Gruppen](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Optional) Wählen Sie **[!UICONTROL E-Mail-Einstellungen]** aus, um E-Mail-Einstellungen auszuwählen, die sich von den Standardeinstellungen unterscheiden.

   Siehe [Einrichten der Begrüßungs-E-Mail für Media Portal-Benutzer](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Wählen Sie **[!UICONTROL Benutzer hinzufügen]** aus.

Nachdem ein Benutzer hinzugefügt wurde, erhält er von Media Portal eine Begrüßungs-E-Mail. Die Nachricht enthält ein temporäres Passwort und die Media Portal-URL.

## Hochladen einer Media Portal-Benutzerliste {#uploading-a-media-portal-user-list}

Um viele Benutzer gleichzeitig hinzuzufügen, können Sie eine Benutzerliste hochladen. Die Benutzer werden automatisch dem derzeit ausgewählten Konto hinzugefügt.

Erstellen Sie die Benutzerliste mit den Benutzerdaten als CSV-Datei (kommagetrennte Werte). Nach dem Hochladen der Liste werden die Benutzer in der Liste dem Konto automatisch mit ihren angegebenen Gruppenzuweisungen hinzugefügt. Jeder Benutzer erhält eine Begrüßungs-E-Mail mit einer Verknüpfung zum Media Portal und einem temporären Kennwort.

### Erstellen der CSV-Datei {#create-the-csv-file}

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
| Prairie | Kat | `prairiek@company.com` | willkommen | Media Portal-Administrator | PortalCo/IT, PortalCo/Admin |
| Rick | Brough | `rickb@myco.com` | willkommen | Media Portal-Benutzer | PortalCo/MktgGroup, PortalCo/test |

### Hochladen der CSV-Datei {#uploading-the-csv-file}

1. Öffnen Sie unter „Einstellungen“ den Anzeigebereich „Benutzerverwaltung“.
1. Wählen Sie **[!UICONTROL Benutzerliste hochladen]** aus.
1. Wählen Sie im Dialogfeld &quot;Select File to Upload&quot;die CSV-Datei aus und wählen Sie dann **[!UICONTROL Open]** aus.

Jeder Benutzer in der Liste wird automatisch zu den angegebenen Gruppen hinzugefügt. Jeder Benutzer erhält eine Begrüßungs-E-Mail.

>[!NOTE]
>
>Wenn die CSV-Datei nicht korrekt formatiert wurde, wird die folgende Fehlermeldung angezeigt: &quot;Bei der Verarbeitung der hochgeladenen CSV-Datei ist ein Fehler aufgetreten. Prüfen Sie den Dateiinhalt auf gültige Daten.&quot; Wenn die CSV-Datei einen vorhandenen IP- oder IPS-Benutzer enthält, wird der Benutzer nicht zur Benutzerliste hinzugefügt.

## Generieren einer auswählbaren Media Portal-Benutzerliste {#generating-a-selectable-list-of-media-portal-users}

Sie können die Namen und E-Mail-Adressen von Media Portal-Benutzern in einem Popup-Fenster anzeigen. Dies ist nützlich, wenn Sie Benutzernamen und Adressen kopieren und in eine Anwendung außerhalb von Media Portal einfügen möchten.

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Administrationseinstellungen]** > **[!UICONTROL Benutzerverwaltung]**.
1. Wählen Sie in der Dropdownliste **[!UICONTROL Nach Benutzerrolle]** den Namen einer Media Portal-Benutzerrolle aus und wählen Sie **[!UICONTROL Aktualisieren]** , um die Namen einer Klasse von Media Portal-Benutzern anzuzeigen.
1. Wählen Sie **[!UICONTROL Popup-Liste]** aus. Kopieren Sie diese Liste und fügen Sie sie ein.

## Einrichten der Begrüßungs-E-Mail für Media Portal-Benutzer {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Sie können eine Begrüßungs-E-Mail an neue Media Portal-Benutzer, -Mitarbeiter und -Mitarbeiter-Benutzer senden lassen, die Sie hinzufügen. Sie können diese E-Mail-Nachricht konfigurieren oder Adobe Dynamic Media Classic anweisen, sie nicht zu senden.

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Administrationseinstellungen]** > **[!UICONTROL Benutzerverwaltung]**.
1. Wählen Sie im Bildschirm &quot;Benutzerverwaltung einrichten&quot;die Option **[!UICONTROL E-Mail-Einstellungen]**.
1. Nehmen Sie im Dialogfeld „E-Mail-Einstellungen“ folgende Einstellungen vor:

   * **[!UICONTROL E-Mail senden]**: Deaktivieren Sie diese Option, um neue Benutzer per E-Mail darüber zu informieren, dass Sie sie angemeldet haben.

   * **[!UICONTROL Standardkennwort]**: Geben Sie ein temporäres Kennwort für neue Benutzer ein oder lassen Sie das Feld leer, damit Adobe Dynamic Media Classic zufällige Kennwörter generiert. Benutzer werden aufgefordert, bei der ersten Anmeldung Kennwörter zu ändern.

   * **[!UICONTROL Ersatz-URL]**: Geben Sie eine URL ein, die sich von der Standardeinstellung unterscheidet, wenn Ihre Benutzer über eine andere URL auf Adobe Dynamic Media Classic zugreifen.

## Andere Aufgaben zur Benutzerverwaltung {#other-user-management-tasks}

Über den Anzeigebereich „Benutzerverwaltung“ können Sie außerdem folgende Aufgaben ausführen:

* **[!UICONTROL Filtern und Sortieren der Benutzerliste]**: Filtern Sie die Liste der Media Portal-Benutzer, um Benutzer zu finden.

* **[!UICONTROL Benutzer löschen]**: Entfernt einen Benutzer aus der Liste.

* **[!UICONTROL Benutzer aktivieren und deaktivieren]**: Benutzer daran hindern, auf Ordner zuzugreifen.

* **[!UICONTROL Benutzerinformationen bearbeiten]**: Geben Sie aktuelle Informationen zu einem Benutzer ein.

* **[!UICONTROL Benutzerdefinierte Felder erstellen]**: Erstellen Sie benutzerdefinierte, benutzerdefinierte Metadatenfelder, damit sie Ihnen beim Organisieren von Assets in der Adobe Dynamic Media Classic helfen können. Die Felder können bei Bedarf auch aktiviert oder deaktiviert werden.

Siehe [Benutzerdefinierte Felder](application-setup.md#user_defined_fields).
