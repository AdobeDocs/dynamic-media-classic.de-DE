---
title: Bei Adobe Analytics anmelden
description: Erfahren Sie, wie Sie sich von Adobe Dynamic Media Classic aus bei Adobe Analytics anmelden.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
topic: Integrations, Development
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# Bei Adobe Analytics anmelden{#log-in-to-adobe-analytics}

Stellen Sie sicher, dass Sie Mitglied der Gruppe Web Service Access in Adobe Analytics sind. Führen Sie diese Schritte aus, bevor Sie sich anmelden, um Adobe Analytics-Berichte zu konfigurieren und Adobe Analytics-Berichtsvariablen Adobe Dynamic Media Classic-Ereignissen zuzuordnen. Mitglieder dieser Gruppe können auf alle Berichte in den angegebenen Report Suites zugreifen. Verwenden Sie dazu die Experience Cloud Web Services API, unabhängig von den in der Benutzeroberfläche festgelegten Berechtigungen. Um ein Mitglied zur Gruppe hinzuzufügen, gehen Sie in Adobe Analytics zu &quot;**[!UICONTROL Admin Tools]**&quot;> &quot;**[!UICONTROL Benutzerverwaltung]**&quot;> &quot;**[!UICONTROL Gruppen bearbeiten]**&quot;.

Wenn Sie sich anmelden, können Sie Ihre Experience Cloud-Organisations-ID eingeben, um die neueste Videoanalyseimplementierung zu verwenden. Wenn Sie sich gegen die Eingabe Ihrer ID entscheiden, funktioniert die Videoberichterstellung weiterhin. Dies kann jedoch dazu führen, dass die Daten nicht ordnungsgemäß mit anderen Daten für diesen Client von außerhalb von Adobe Dynamic Media Classic integriert werden.

>[!NOTE]
>
>Wenn Ihr Adobe Analytics-Konto zur Anmeldung zur Adobe IMS-basierten Authentifizierung (Identity Management System) migriert wurde, funktioniert die Eingabe direkter Anmeldeinformationen nicht.

## Bei Adobe Analytics über Adobe Dynamic Media Classic anmelden {#log-in-to-analytics-from-dmc}

Integrieren Sie zunächst Dynamic Media Classic in Adobe Analytics OAuth. Die OAuth-Integration von Adobe Analytics mit Dynamic Media Classic wird in der Regel nur einmal pro Benutzer durchgeführt.

1. Rufen Sie [Adobe Developer Console](https://developer.adobe.com/console) auf. Stellen Sie sicher, dass Ihr Konto über Administratorberechtigungen für die Organisation verfügt, für die die Integration erforderlich ist.
1. Wählen Sie in der rechten oberen Ecke der Startseite aus der Dropdownliste das entsprechende Unternehmen aus. (Der folgende Screenshot dient nur zu Informationszwecken. Der tatsächlich ausgewählte Firmenname kann variieren.)

   ![Neues Projekt erstellen](assets/analytics-oauth1.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie oben auf der Seite auf der Registerkarte **[!UICONTROL Startseite]** die Option **[!UICONTROL Neues Projekt erstellen]**.
   * Öffnen Sie oben auf der Seite die Registerkarte **[!UICONTROL Projekte]** . Wählen Sie rechts auf der Seite **[!UICONTROL Neues Projekt erstellen]** aus.

1. Wählen Sie auf der Seite des Projekts **[!UICONTROL API hinzufügen]** aus.
1. Wählen Sie auf der Seite **[!UICONTROL API hinzufügen]** die Option **[!UICONTROL Adobe Analytics]** aus.
1. Wählen Sie rechts unten auf der Seite **[!UICONTROL Weiter]** aus.

   ![API hinzufügen](assets/analytics-oauth2.png)

1. Wählen Sie auf der Seite **[!UICONTROL `Configure API`]** die Option **[!UICONTROL BENUTZERAUTHENTIFIZIERUNG OAuth]** aus.
1. Wählen Sie rechts unten auf der Seite **[!UICONTROL Weiter]** aus.
1. Wählen Sie auf der Seite **[!UICONTROL `Configure API`]** die Option **[!UICONTROL OAUTH 2.0 Web]**.
1. Geben Sie im Textfeld **[!UICONTROL Standard-Umleitungs-URI]** den folgenden Pfad genau wie folgt ein:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. Geben Sie im Textfeld **[!UICONTROL Umleitungs-URI-Muster]** den folgenden Pfad genau wie folgt ein:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. Wählen Sie rechts unten auf der Seite **[!UICONTROL Konfigurierte API speichern]** aus.
1. Wählen Sie im Navigationsfenster auf der linken Seite der Adobe Analytics-Seite unter **[!UICONTROL Anmeldedaten]** die Option **[!UICONTROL OAuth Web]**.
1. Führen Sie unter **[!UICONTROL Berechtigungsdetails]** folgende Schritte aus:
   * Wählen Sie unter **[!UICONTROL Client-ID]** die Option **[!UICONTROL Kopieren]** aus, um den Wert zu kopieren. Sie benötigen diesen Wert für die nachfolgende Analytics-Konfiguration im Dynamic Media Classic-Desktop-Programm, die befolgt werden soll.
   * Wählen Sie unter **[!UICONTROL Client-Geheimnis]** die Option **[!UICONTROL Client-Geheimnis abrufen]** aus, um den zugehörigen Wert anzuzeigen. Wählen Sie **[!UICONTROL Kopieren]** aus, um den Wert zu kopieren. Sie benötigen diesen Wert für die nachfolgende Adobe Analytics-Konfiguration im Dynamic Media Classic-Desktop-Programm, die befolgt werden soll.

## Konfigurieren von Adobe Analytics in Adobe Dynamic Media Classic {#configure-analytics-in-dmc}

>[!NOTE]
>
>Nach der ersten Konfiguration von Adobe Analytics in Dynamic Media Classic müssen Sie die Konfiguration nur in den folgenden Fällen wiederholen:
>
>* In Analytics wird ein neuer Bericht hinzugefügt, und der Benutzer möchte mit dem Senden von Daten an diesen neuen Bericht beginnen.
>* Der Tracking-Server wird in Adobe Analytics aktualisiert.
>* Eine neue Tracking-Variable wird in einen Bericht eingeführt und Sie möchten in der Dynamic Media Classic-Benutzeroberfläche eine bestimmte Viewer-Variable mit dieser neuen Analytics-Variablen verknüpfen.
>

1. Wechseln Sie in der rechten oberen Ecke des Adobe Dynamic Media Classic-Desktop-Programms zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]**.
1. Wählen Sie im linken Bereich unter **[!UICONTROL Anwendungseinstellungen]** die Option **[!UICONTROL Adobe Analytics]** aus.
1. Wählen Sie auf der Seite **[!UICONTROL Adobe Analytics-Konfiguration]** die Option **[!UICONTROL Adobe Analytics-Anmeldung]** aus.
1. Fügen Sie im Dialogfeld **[!UICONTROL Adobe Analytics Login]** im Feld **[!UICONTROL CLIENT-ID]** und im Feld **[!UICONTROL CLIENT SECRET]** die entsprechenden Werte ein, die Sie zuvor kopiert haben.
1. Wählen Sie in der rechten unteren Ecke des Dialogfelds **[!UICONTROL Anmelden]** aus und führen Sie die Anmeldung bei Adobe IMS (Identity Management Services) durch.

   Bei erfolgreicher Anmeldung wird das Dialogfeld &quot;Adobe Analytics-Anmeldung&quot;zusammen mit der Dropdownliste **[!UICONTROL UNTERNEHMEN]** erneut angezeigt, die von den Ihnen zur Verfügung stehenden Unternehmen initiiert wurde.

1. Wählen Sie aus der Dropdownliste **[!UICONTROL UNTERNEHMEN]** ein Unternehmen aus.

   Nachdem Sie ein Unternehmen ausgewählt haben, wird die Dropdownliste **[!UICONTROL SUITES]** angezeigt, die von den Report Suites initiiert wurde, die für das ausgewählte Unternehmen verfügbar sind.

1. Wählen Sie aus der Dropdownliste **[!UICONTROL SUITES]** eine Report Suite aus.

   >[!NOTE]
   >
   >Standardmäßig muss der Benutzer wissen, dass sowohl die Dropdownlisten **[!UICONTROL UNTERNEHMEN]** als auch die Dropdownlisten **[!UICONTROL SUITES]** leer sind. Daher muss der Benutzer einen Wert aus jeder Liste auswählen.

1. Wählen Sie **[!UICONTROL OK]** aus, damit Sie die Konfiguration speichern können.

   >[!NOTE]
   >
   >Das Feld **[!UICONTROL Adobe Analytics Server]** wird mit einem vorgeschlagenen Drittanbieter-Tracking-Server ausgefüllt, der Ihrem Analytics-Namespace entspricht, wenn Sie **[!UICONTROL OK]** auswählen. Wenn Sie einen anderen Tracking-Server verwenden, aktualisieren Sie ihn in diesem Feld, um Datenverlust zu vermeiden.

1. Wählen Sie links unten auf der Seite &quot;Adobe Analytics-Konfiguration&quot;die Option **[!UICONTROL Speichern]** aus, um sicherzustellen, dass Ihre Adobe Analytics-Kontokonfiguration aktualisiert wird.

>[!MORELIKETHIS]
>
>* [Konfigurieren von Adobe Analytics-Berichten](configuring-analytics-reports.md#configuring_adobe_analytics_reports)
