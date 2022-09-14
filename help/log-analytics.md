---
title: Anmelden bei Adobe Analytics
description: Erfahren Sie, wie Sie sich von Adobe Dynamic Media Classic aus bei Adobe Analytics anmelden.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 1%

---

# Anmelden bei Adobe Analytics{#log-in-to-adobe-analytics}

Bevor Sie sich anmelden, um Adobe Analytics-Berichte zu konfigurieren und Adobe Analytics-Berichtsvariablen mit Adobe Dynamic Media Classic-Ereignissen abzugleichen, stellen Sie sicher, dass Sie Mitglied der Gruppe Zugriff auf Webdienste in Adobe Analytics sind. Mitglieder dieser Gruppe können über die Web-Services-API des Experience Cloud auf alle Berichte in den angegebenen Report Suites zugreifen, unabhängig von den in der Benutzeroberfläche festgelegten Berechtigungen. Um der Gruppe ein Mitglied hinzuzufügen, navigieren Sie in Adobe Analytics zu **[!UICONTROL Admin Tools]** > **[!UICONTROL Benutzerverwaltung]** > **[!UICONTROL Gruppen bearbeiten]**.

Bei der Anmeldung können Sie Ihre Experience Cloud-Organisations-ID eingeben, um die neueste Videoanalyseimplementierung zu verwenden. Wenn Sie sich gegen die Eingabe Ihrer ID entscheiden, funktioniert die Videoberichterstellung weiterhin. Dies kann jedoch dazu führen, dass die Daten nicht ordnungsgemäß mit anderen Daten für diesen Client von außerhalb von Adobe Dynamic Media Classic integriert werden.

>[!NOTE]
>
>Wenn Ihr Adobe Analytics-Konto zur Anmeldung zur Adobe IMS-basierten Authentifizierung (Identity Management System) migriert wurde, funktioniert die Eingabe direkter Anmeldeinformationen nicht.

## Bei Adobe Analytics über Adobe Dynamic Media Classic anmelden {#log-in-to-analytics-from-dmc}

Integrieren Sie zunächst Dynamic Media Classic in Adobe Analytics OAuth. Die OAuth-Integration von Adobe Analytics mit Dynamic Media Classic wird in der Regel nur einmal pro Benutzer durchgeführt.

1. Zugriff [Adobe Developer-Konsole](https://developer.adobe.com/console). Stellen Sie sicher, dass Ihr Konto über Administratorberechtigungen für die Organisation verfügt, für die die Integration erforderlich ist.
1. Wählen Sie in der rechten oberen Ecke der Startseite aus der Dropdown-Liste das entsprechende Unternehmen aus. (Der folgende Screenshot dient nur zu Informationszwecken. der tatsächlich ausgewählte Unternehmensname kann variieren.)

   ![Erstellen Sie ein neues Projekt](assets/analytics-oauth1.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Am oberen Seitenrand von der **[!UICONTROL Startseite]** Registerkarte, wählen Sie **[!UICONTROL Neues Projekt erstellen]**.
   * Am oberen Seitenrand von der **[!UICONTROL Projekte]** Registerkarte. Wählen Sie rechts auf der Seite die Option **[!UICONTROL Neues Projekt erstellen]**.

1. Wählen Sie auf der Projektseite **[!UICONTROL API hinzufügen]**.
1. Im **[!UICONTROL API hinzufügen]** Seite, wählen Sie **[!UICONTROL Adobe Analytics]**.
1. Wählen Sie rechts unten auf der Seite die Option **[!UICONTROL Nächste]**.

   ![API hinzufügen](assets/analytics-oauth2.png)

1. Im **[!UICONTROL API konfigurieren]** Seite, wählen Sie **[!UICONTROL BENUTZERAUTHENTIFIZIERUNG OAuth]**.
1. Wählen Sie rechts unten auf der Seite die Option **[!UICONTROL Nächste]**.
1. Im **[!UICONTROL API konfigurieren]** Seite, wählen Sie **[!UICONTROL OAUTH 2.0 Web]**.
1. Im **[!UICONTROL Standard-Umleitungs-URI]** Geben Sie den folgenden Pfad genau wie folgt ein:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. Im **[!UICONTROL Umleitungs-URI-Muster]** Geben Sie den folgenden Pfad genau wie folgt ein:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. Wählen Sie in der rechten unteren Ecke der Seite die Option **[!UICONTROL Konfigurierte API speichern]**.
1. Im Navigationsfenster auf der linken Seite der Adobe Analytics-Seite, unter **[!UICONTROL Anmeldeinformationen]** auswählen **[!UICONTROL OAuth Web]**.
1. under **[!UICONTROL Details zu Berechtigungen]** führen Sie folgende Schritte aus:
   * under **[!UICONTROL Client-ID]** auswählen **[!UICONTROL Kopieren]** , um den Wert zu kopieren. Sie benötigen diesen Wert für die nachfolgende Analytics-Konfiguration im Dynamic Media Classic-Desktop-Programm, die befolgt werden soll.
   * under **[!UICONTROL Client Secret]** auswählen **[!UICONTROL Client-Geheimnis abrufen]** , um den zugehörigen Wert anzuzeigen. Auswählen **[!UICONTROL Kopieren]** , um den Wert zu kopieren. Sie benötigen diesen Wert für die nachfolgende Adobe Analytics-Konfiguration im Dynamic Media Classic-Desktop-Programm, die befolgt werden soll.

## Konfigurieren von Adobe Analytics in Adobe Dynamic Media Classic {#configure-analytics-in-dmc}

>[!NOTE]
>
>Nach der ersten Konfiguration von Adobe Analytics in Dynamic Media Classic müssen Sie die Konfiguration nur in den folgenden Fällen wiederholen:
>
>* In Analytics wird ein neuer Bericht hinzugefügt, und der Benutzer möchte mit dem Senden von Daten an diesen neuen Bericht beginnen.
>* Der Tracking-Server wird in Adobe Analytics aktualisiert.
>* Eine neue Tracking-Variable wird in einen Bericht eingeführt und Sie möchten in der Dynamic Media Classic-Benutzeroberfläche eine bestimmte Viewer-Variable mit dieser neuen Analytics-Variablen verknüpfen.
>


1. Navigieren Sie in der rechten oberen Ecke des Adobe Dynamic Media Classic-Desktop-Programms zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]**.
1. Im linken Bereich unter **[!UICONTROL Anwendungseinstellungen]** auswählen **[!UICONTROL Adobe Analytics]**.
1. Im **[!UICONTROL Adobe Analytics-Konfiguration]** Seite, wählen Sie **[!UICONTROL Adobe Analytics-Anmeldung]**.
1. Im **[!UICONTROL Adobe Analytics-Anmeldung]** im Dialogfeld **[!UICONTROL CLIENT-ID]** und **[!UICONTROL CLIENT SECRET]** -Feld die entsprechenden Werte ein, die Sie zuvor kopiert haben.
1. Wählen Sie in der rechten unteren Ecke des Dialogfelds die Option **[!UICONTROL Anmelden]** und führen Sie Ihre Anmeldung bei Adobe IMS (Identity Management Services) durch.

   Bei erfolgreicher Anmeldung wird das Dialogfeld &quot;Adobe Analytics-Anmeldung&quot;zusammen mit dem **[!UICONTROL UNTERNEHMEN]** Dropdown-Liste, initiiert von den Unternehmen, die Ihnen zur Verfügung stehen.

1. Aus dem **[!UICONTROL UNTERNEHMEN]** aus, wählen Sie ein Unternehmen aus.

   Nachdem Sie ein Unternehmen ausgewählt haben, wird die **[!UICONTROL SUITES]** Dropdown-Liste, die von den Report Suites initiiert wird, die für das ausgewählte Unternehmen verfügbar sind, wird angezeigt.

1. Aus dem **[!UICONTROL SUITES]** eine Report Suite aus.

   >[!NOTE]
   >
   >Standardmäßig muss der Benutzer wissen, dass beide **[!UICONTROL UNTERNEHMEN]** und **[!UICONTROL SUITES]** Dropdown-Listen sind leer. Daher muss der Benutzer einen Wert aus jeder Liste auswählen.

1. Auswählen **[!UICONTROL OK]** sodass Sie die Konfiguration speichern können.

   >[!NOTE]
   >
   >Die **[!UICONTROL Adobe Analytics Server]** wird mit einem vorgeschlagenen Drittanbieter-Tracking-Server ausgefüllt, der Ihrem Analytics-Namespace entspricht, wenn Sie **[!UICONTROL OK]**. Wenn Sie einen anderen Tracking-Server verwenden, aktualisieren Sie ihn in diesem Feld, um Datenverlust zu vermeiden.

1. Wählen Sie links unten auf der Seite &quot;Adobe Analytics-Konfiguration&quot;die Option **[!UICONTROL Speichern]** , um sicherzustellen, dass Ihre Adobe Analytics-Kontokonfiguration aktualisiert wird.

>[!MORELIKETHIS]
>
>* [Konfigurieren von Adobe Analytics-Berichten](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

