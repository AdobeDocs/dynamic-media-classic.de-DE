---
title: Hinzufügen und Verwalten von Media Portal-Benutzern
description: Erfahren Sie, wie Sie Media Portal-Benutzer in Adobe Dynamic Media Classic hinzufügen und verwalten.
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
topic: Administration
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 58%

---

# Hinzufügen und Verwalten von Media Portal-Benutzern{#adding-and-managing-media-portal-users}

Als Administrator können Sie Benutzer hinzufügen und verwalten, entscheiden, ob Benutzer Kennwörter ändern dürfen, Benutzerinformationen bearbeiten und Benutzerlisten hochladen. Diese Aufgaben werden im Anzeigebereich „Benutzerverwaltung“ ausgeführt. Um auf diesen Bildschirm zuzugreifen, navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Administrationseinstellungen]** > **[!UICONTROL Benutzerverwaltung]**.

>[!NOTE]
>
>Bevor Sie Benutzer hinzufügen können, müssen Sie Gruppen einrichten, um die Benutzer zu verwalten. In Media Portal können Benutzer nur hinzugefügt werden, wenn sie gleichzeitig einer oder mehreren Gruppen zugewiesen werden. Weitere Informationen finden Sie unter [Erstellen und Verwalten von Media Portal-Gruppen](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## Verwaltung von Media Portal-Passwörtern {#handling-media-portal-passwords}

Media Portal-Benutzer, -Mitarbeiter und -Mitarbeiter-Benutzer erhalten eine E-Mail mit einem Kennwort, wenn Sie sie anmelden. Administratoren können entscheiden, ob Media Portal-Benutzer dieses Kennwort ändern dürfen.

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Media Portal-Einrichtung]** > **[!UICONTROL Allgemeine Einstellungen]**.
1. Auf der Seite „Allgemeine Einstellungen“ können Sie **[!UICONTROL „Kennwortänderung durch MediaPortal-Benutzer zulassen“]** aktivieren oder deaktivieren.
1. Auswählen **[!UICONTROL Speichern]**.

>[!NOTE]
>
>Benutzer von Media Portal, die Kennwörter ändern dürfen, können dies durch Auswahl von **[!UICONTROL Einrichtung]** > **[!UICONTROL Persönliche Einstellungen]** und das Ändern von Passwörtern auf dem Bildschirm &quot;Persönliche Einstellungen&quot;.

## Hinzufügen eines Media Portal-Benutzers {#adding-a-media-portal-user}

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Administrationseinstellungen]** > **[!UICONTROL Benutzerverwaltung]**.
1. Wählen Sie auf der Seite &quot;Benutzerverwaltung&quot;die Option **Hinzufügen**.
1. Geben Sie im Dialogfeld &quot;Benutzer hinzufügen&quot;im Bedienfeld &quot;Benutzerinformationen&quot;den Vornamen, Nachnamen und die E-Mail-Adresse des Benutzers ein und wählen Sie dann **[!UICONTROL Nächste]**.
1. Wählen Sie im Bedienfeld „Unternehmen/Rolle“ aus der Dropdown-Liste „Unternehmen“ ein oder mehrere Unternehmen für den Benutzer aus.
1. Wählen Sie in der Liste &quot;Rolle&quot;eine Media Portal-Rolle aus und klicken Sie auf **[!UICONTROL Nächste]**.

   Siehe [Media Portal-Benutzerrollen](media-portal-user-roles.md#media_portal_user_roles).

1. Wählen Sie im Bedienfeld „Auf Gruppen zugreifen“ mindestens eine Gruppe aus.

   Siehe [Erstellen und Verwalten von Media Portal-Gruppen](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. (Optional) Wählen Sie **[!UICONTROL E-Mail-Einstellungen]** , um andere E-Mail-Einstellungen als die Standardeinstellungen zu wählen.

   Siehe [Einrichten der Begrüßungs-E-Mail für Media Portal-Benutzer](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users).

1. Auswählen **[!UICONTROL Benutzer hinzufügen]**.

Nachdem ein Benutzer hinzugefügt wurde, erhält er von Media Portal eine Begrüßungs-E-Mail. Die Nachricht enthält ein temporäres Passwort und die Media Portal-URL.

## Hochladen einer Media Portal-Benutzerliste {#uploading-a-media-portal-user-list}

Um viele Benutzer gleichzeitig hinzuzufügen, können Sie eine Benutzerliste hochladen. Die Benutzer werden automatisch dem derzeit ausgewählten Konto hinzugefügt.

Erstellen Sie die Benutzerliste mit den Benutzerdaten als CSV-Datei (kommagetrennte Werte). Nach dem Hochladen der Liste werden die Benutzer in der Liste dem Konto automatisch mit ihren angegebenen Gruppenzuweisungen hinzugefügt. Jeder Benutzer erhält eine Begrüßungs-E-Mail mit einer Verknüpfung zum Media Portal und einem temporären Kennwort.

### Erstellen der CSV-Datei {#creating-the-csv-file}

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
| Prairie | Kat | `prairiek@company.com` | willkommen | Media Portal-Administrator | PortalCo/IT,PortalCo/Admin |
| Rick | Brough | `rickb@myco.com` | willkommen | Media Portal-Benutzer | PortalCo/MktgGroup, PortalCo/test |

### Hochladen der CSV-Datei {#uploading-the-csv-file}

1. Öffnen Sie unter „Einstellungen“ den Anzeigebereich „Benutzerverwaltung“.
1. Auswählen **[!UICONTROL Hochladen der Benutzerliste]**.
1. Wählen Sie im Dialogfeld &quot;Select File to Upload&quot;die CSV-Datei aus und wählen Sie dann **[!UICONTROL Öffnen]**.

Alle Benutzer in der Liste werden automatisch den angegebenen Gruppen hinzugefügt. Jeder Benutzer erhält eine Begrüßungs-E-Mail.

>[!NOTE]
>
>Wenn die CSV-Datei nicht ordnungsgemäß formatiert war, wird die folgende Fehlermeldung angezeigt: „Bei der Verarbeitung der hochgeladenen CSV-Datei ist ein Fehler aufgetreten. Überprüfen Sie den Inhalt der Datei auf gültige Daten.“ Wenn die CSV-Datei einen vorhandenen IP- oder IPS-Benutzer enthält, wird dieser nicht der Benutzerliste hinzugefügt.

## Generieren einer auswählbaren Media Portal-Benutzerliste {#generating-a-selectable-list-of-media-portal-users}

Sie können die Namen und E-Mail-Adressen von Media Portal-Benutzern in einem Popup-Fenster anzeigen. Dies ist nützlich, wenn Sie Benutzernamen und Adressen kopieren und in eine Anwendung außerhalb von Media Portal einfügen möchten.

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Administrationseinstellungen]** > **[!UICONTROL Benutzerverwaltung]**.
1. Im **[!UICONTROL Nach Benutzerrolle]** Dropdownliste den Namen einer Media Portal-Benutzerrolle auswählen und **[!UICONTROL Aktualisieren]** , um die Namen einer Klasse von Media Portal-Benutzern anzuzeigen.
1. Auswählen **[!UICONTROL Popup-Liste]**. Kopieren Sie diese Liste und fügen Sie sie ein.

## Einrichten der Begrüßungs-E-Mail für Media Portal-Benutzer {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

Sie können eine Begrüßungs-E-Mail an neue Media Portal-Benutzer, -Mitarbeiter und -Mitarbeiter-Benutzer senden lassen, die Sie hinzufügen. Sie können diese E-Mail-Nachricht konfigurieren oder Adobe Dynamic Media Classic anweisen, sie nicht zu senden.

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Administrationseinstellungen]** > **[!UICONTROL Benutzerverwaltung]**.
1. Wählen Sie im Bildschirm &quot;Benutzerverwaltungseinstellungen&quot;die Option **[!UICONTROL E-Mail-Einstellungen]**.
1. Nehmen Sie im Dialogfeld „E-Mail-Einstellungen“ folgende Einstellungen vor:

   * **[!UICONTROL E-Mail senden]** - Deaktivieren Sie diese Option, wenn Sie neue Benutzer nicht per E-Mail darüber informieren möchten, dass Sie sie angemeldet haben.

   * **[!UICONTROL Standardkennwort]** - Geben Sie ein temporäres Kennwort für neue Benutzer ein oder lassen Sie das Feld leer, damit Adobe Dynamic Media Classic zufällige Kennwörter generiert. Benutzer werden aufgefordert, bei der ersten Anmeldung Kennwörter zu ändern.

   * **[!UICONTROL Ersatz-URL]** - Geben Sie eine URL ein, die sich von der Standardeinstellung unterscheidet, wenn Ihre Benutzer über eine andere URL auf Adobe Dynamic Media Classic zugreifen.

## Andere Aufgaben zur Benutzerverwaltung {#other-user-management-tasks}

Über den Anzeigebereich „Benutzerverwaltung“ können Sie außerdem folgende Aufgaben ausführen:

* **[!UICONTROL Benutzerliste filtern und sortieren]** - Filtern Sie die Liste der Media Portal-Benutzer, um Benutzer zu finden.

* **[!UICONTROL Benutzer löschen]** - Entfernen Sie einen Benutzer aus der Liste.

* **[!UICONTROL Benutzer aktivieren und deaktivieren]** - Benutzer daran hindern, auf Ordner zuzugreifen.

* **[!UICONTROL Bearbeiten von Benutzerinformationen]** - Geben Sie aktuelle Informationen zu einem Benutzer ein.

* **[!UICONTROL Benutzerdefinierte Felder erstellen]** - Erstellen Sie benutzerdefinierte, benutzerdefinierte Metadatenfelder, damit Sie Assets in der Adobe Dynamic Media Classic organisieren können. Die Felder können bei Bedarf auch aktiviert oder deaktiviert werden.

Siehe [Benutzerdefinierte Felder](application-setup.md#user_defined_fields).
