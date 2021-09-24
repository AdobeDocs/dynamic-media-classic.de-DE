---
title: Anmelden bei Adobe Analytics
description: Erfahren Sie, wie Sie sich von Adobe Dynamic Media Classic aus bei Adobe Analytics anmelden.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: d18dbbf89a1bfe4df46cbe7d56cdf6f442595ddb
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 1%

---

# Anmelden bei Adobe Analytics{#log-in-to-adobe-analytics}

Bevor Sie sich anmelden, um Adobe Analytics-Berichte zu konfigurieren und Adobe Analytics-Berichtsvariablen mit Adobe Dynamic Media Classic-Ereignissen abzugleichen, stellen Sie sicher, dass Sie Mitglied der Zugriffsgruppe für Webdienste in Adobe Analytics sind. Mitglieder dieser Gruppe können über die Web-Services-API des Experience Cloud auf alle Berichte in den angegebenen Report Suites zugreifen, unabhängig von den in der Benutzeroberfläche festgelegten Berechtigungen. Um ein Mitglied zur Gruppe hinzuzufügen, gehen Sie in Adobe Analytics zu **[!UICONTROL Admin Tools]** > **[!UICONTROL Benutzerverwaltung]** > **[!UICONTROL Gruppen bearbeiten]**.

Bei der Anmeldung können Sie Ihre Experience Cloud-Organisations-ID eingeben, um die neueste Videoanalyseimplementierung zu verwenden. Wenn Sie sich gegen die Eingabe Ihrer ID entscheiden, funktioniert die Videoberichterstellung weiterhin. Dies kann jedoch dazu führen, dass die Daten nicht ordnungsgemäß mit anderen Daten für diesen Client von außerhalb von Adobe Dynamic Media Classic integriert werden.

>[!NOTE]
>
>Wenn Ihr Adobe Analytics-Konto zur Anmeldung zur Adobe IMS-basierten Authentifizierung (Identity Management System) migriert wurde, funktioniert die Eingabe direkter Anmeldeinformationen nicht.

**So melden Sie sich von Adobe Dynamic Media Classic aus bei Adobe Analytics an:**

Integrieren Sie zunächst Dynamic Media Classic in Adobe Analytics OAuth. Die OAuth-Integration von Adobe Analytics mit Dynamic Media Classic wird in der Regel nur einmal pro Benutzer durchgeführt.

1. Rufen Sie [Adobe Developer Console](https://developer.adobe.com/console) auf. Stellen Sie sicher, dass Ihr Konto über Administratorberechtigungen für die Organisation verfügt, für die die Integration erforderlich ist.
1. Wählen Sie in der rechten oberen Ecke der Startseite aus der Dropdown-Liste das entsprechende Unternehmen aus. (Der folgende Screenshot dient nur zu Informationszwecken. der tatsächlich gewählte Unternehmensname variieren kann.)

   ![Erstellen Sie ein neues Projekt](assets/analytics-oauth1.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie oben auf der Seite auf der Registerkarte **[!UICONTROL Home]** die Option **[!UICONTROL Neues Projekt erstellen]**.
   * Oben auf der Seite auf der Registerkarte **[!UICONTROL Projekte]** . Wählen Sie rechts auf der Seite **[!UICONTROL Neues Projekt erstellen]** aus.

1. Wählen Sie auf der Projektseite **[!UICONTROL API]** hinzufügen aus.
1. Wählen Sie auf der Seite **[!UICONTROL API]** hinzufügen **[!UICONTROL Adobe Analytics]** aus.
1. Wählen Sie in der rechten unteren Ecke der Seite **[!UICONTROL Weiter]** aus.

   ![API hinzufügen](assets/analytics-oauth2.png)

1. Wählen Sie auf der Seite **[!UICONTROL API]** konfigurieren **[!UICONTROL USER AUTHENTICATION OAuth]** aus.
1. Wählen Sie in der rechten unteren Ecke der Seite **[!UICONTROL Weiter]** aus.
1. Wählen Sie auf der Seite **[!UICONTROL API]** konfigurieren **[!UICONTROL OAUTH 2.0 Web]** aus.
1. Geben Sie im Textfeld **[!UICONTROL Standard-Umleitungs-URI]** den folgenden Pfad genau wie folgt ein:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. Geben Sie im Textfeld **[!UICONTROL Umleitungs-URI-Muster]** den folgenden Pfad genau wie folgt ein:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. Wählen Sie in der rechten unteren Ecke der Seite **[!UICONTROL Konfigurierte API speichern]** aus.
1. Wählen Sie im Navigationsfenster auf der linken Seite der Adobe Analytics-Seite unter **[!UICONTROL Credentials]** die Option **[!UICONTROL OAuth Web]**.
1. Gehen Sie unter **[!UICONTROL Berechtigungsdetails]** wie folgt vor:
   * Wählen Sie unter **[!UICONTROL Client-ID]** **[!UICONTROL Kopieren]** aus, um den Wert zu kopieren. Sie benötigen diesen Wert für die nachfolgende Analytics-Konfiguration in der Dynamic Media Classic-Desktop-Applikation, die befolgt werden soll.
   * Wählen Sie unter **[!UICONTROL Client Secret]** **[!UICONTROL Retrieve client secret]** aus, um den zugehörigen Wert anzuzeigen. Wählen Sie **[!UICONTROL Copy]** aus, um den Wert zu kopieren. Sie benötigen diesen Wert für die nachfolgende Adobe Analytics-Konfiguration in der Dynamic Media Classic-Desktop-Applikation, die befolgt werden soll.

**Konfigurieren von Adobe Analytics in der Dynamic Media Classic-Desktop-Applikation**

>[!NOTE]
>
>Nach der ersten Konfiguration von Adobe Analytics in Dynamic Media Classic müssen Sie die Konfiguration nur in den folgenden Fällen wiederholen:
>
>* In Analytics wird ein neuer Bericht hinzugefügt, und der Benutzer möchte mit dem Senden von Daten an diesen neuen Bericht beginnen.
>* Der Tracking-Server wird in Adobe Analytics aktualisiert.
>* Eine neue Tracking-Variable wird in einen Bericht eingeführt und Sie möchten eine bestimmte Viewer-Variable in der Benutzeroberfläche von Dynamic Media Classic mit dieser neuen Analytics-Variablen verknüpfen.

>


1. Navigieren Sie in der rechten oberen Ecke des Adobe Dynamic Media Classic-Desktop-Programms zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]**.
1. Wählen Sie im linken Bereich unter **[!UICONTROL Anwendungseinstellungen]** **[!UICONTROL Adobe Analytics]** aus.
1. Wählen Sie auf der Seite **[!UICONTROL Adobe Analytics Configuration]** die Option **[!UICONTROL Adobe Analytics Login]**.
1. Fügen Sie im Dialogfeld **[!UICONTROL Adobe Analytics Login]** im Feld Client-ID und im Feld Client-Geheimnis die entsprechenden Werte ein, die Sie zuvor kopiert haben.
1. Führen Sie die IMS-Anmeldung durch.

   Wenn Sie erfolgreich angemeldet sind, wird die Dropdownliste **[!UICONTROL UNTERNEHMEN]**, die von den Ihnen zur Verfügung stehenden Unternehmen initiiert wurde, sichtbar.

1. Wählen Sie aus der Dropdownliste **[!UICONTROL UNTERNEHMEN]** ein Unternehmen aus.

   Nachdem Sie ein Unternehmen ausgewählt haben, wird die Dropdownliste **[!UICONTROL SUITES]** angezeigt, die von den Report Suites initiiert wurde, die für das ausgewählte Unternehmen verfügbar sind.

1. Wählen Sie aus der Dropdownliste **[!UICONTROL SUITES]** eine Report Suite aus.

   >[!NOTE]
   >
   >Standardmäßig muss der Benutzer wissen, dass sowohl die Dropdownlisten **[!UICONTROL UNTERNEHMEN]** als auch **[!UICONTROL SUITES]** leer sind. Daher muss der Benutzer einen Wert aus jeder Liste auswählen. —>

1. Wählen Sie **[!UICONTROL OK]** aus, damit Sie die Konfiguration speichern können.

>[!MORELIKETHIS]
>
>* [Konfigurieren von Adobe Analytics-Berichten](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

