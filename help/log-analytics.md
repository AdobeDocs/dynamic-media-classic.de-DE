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
source-git-commit: 8111895ac527b92b152382ea80b7b383659f00a9
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 1%

---

# Anmelden bei Adobe Analytics{#log-in-to-adobe-analytics}

Bevor Sie sich anmelden, um Adobe Analytics-Berichte zu konfigurieren und Adobe Analytics-Berichtsvariablen Adobe Dynamic Media Classic-Ereignissen zuzuordnen, überprüfen Sie, ob Sie in Adobe Analytics der Web Service Access-Gruppe angehören. Mitglieder dieser Gruppe können über die Web-Services-API des Experience Cloud auf alle Berichte in den angegebenen Report Suites zugreifen, unabhängig von den in der Benutzeroberfläche festgelegten Berechtigungen. Um ein Mitglied der Gruppe in Adobe Analytics hinzuzufügen, gehen Sie zu **[!UICONTROL Admin Tools]** > **[!UICONTROL Benutzerverwaltung]** > **[!UICONTROL Gruppen bearbeiten]**.

Wenn Sie sich anmelden, haben Sie die Möglichkeit, Ihre Experience Cloud-Org-ID einzugeben, um die neueste Videoanalyseimplementierung zu verwenden. Wenn Sie Ihre ID nicht eingeben, funktioniert der Video-Berichte weiterhin. Es kann jedoch dazu führen, dass die Daten nicht korrekt in andere Daten für diesen Client von außerhalb von Adobe Dynamic Media Classic integriert werden.

>[!NOTE]
>
>Wenn Ihr Adobe Analytics-Konto zur Anmeldung auf Adobe IMS-basierte Authentifizierung (Identity Management System) migriert wurde, funktioniert die Eingabe direkter Anmeldedaten nicht.

## Bei Adobe Analytics von Adobe Dynamic Media Classic anmelden {#log-in-to-analytics-from-dmc}

Beginnen Sie mit der Integration von Dynamic Media Classic in Adobe Analytics OAuth. Die OAuth-Integration von Adobe Analytics mit Dynamic Media Classic erfolgt in der Regel nur einmal pro Benutzer.

1. Zugriff [Adobe Developer Console](https://developer.adobe.com/console). Vergewissern Sie sich, dass Ihr Konto über Administratorberechtigungen für das Unternehmen verfügt, für das die Integration erforderlich ist.
1. Wählen Sie in der Dropdown-Liste rechts oben in der Startseite die entsprechende Firma aus. (Der folgende Screenshot dient nur zu Informationszwecken. der tatsächlich gewählte Name der Firma kann abweichen.)

   ![Erstellen Sie ein neues Projekt](assets/analytics-oauth1.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Am oberen Seitenrand, aus dem **[!UICONTROL Startseite]** Tabulator auswählen **[!UICONTROL Neues Projekt erstellen]**.
   * Am oberen Seitenrand, aus dem **[!UICONTROL Projekte]** Tabulator. Wählen Sie in der Nähe der rechten Ecke der Seite **[!UICONTROL Neues Projekt erstellen]**.

1. Wählen Sie auf der Projektseite **[!UICONTROL hinzufügen-API]**.
1. Auf **[!UICONTROL API Hinzufügen]** Seite, auswählen **[!UICONTROL Adobe Analytics]**.
1. Wählen Sie in der Nähe der rechten unteren Ecke der Seite **[!UICONTROL Weiter]**.

   ![API Hinzufügen](assets/analytics-oauth2.png)

1. Auf **[!UICONTROL API konfigurieren]** Seite, auswählen **[!UICONTROL BENUTZERAUTHENTIFIZIERUNG OAuth]**.
1. Wählen Sie in der Nähe der rechten unteren Ecke der Seite **[!UICONTROL Weiter]**.
1. Auf **[!UICONTROL API konfigurieren]** Seite, auswählen **[!UICONTROL OAUTH 2.0 Web]**.
1. In **[!UICONTROL Standard-Umleitungs-URI]** Textfeld geben Sie den folgenden Pfad genau wie folgt ein:

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. In **[!UICONTROL Umleitungs-URI-Muster]** Textfeld geben Sie den folgenden Pfad genau wie folgt ein:

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. Wählen Sie in der rechten unteren Ecke der Seite **[!UICONTROL Konfigurierte API speichern]**.
1. Im Navigationsfenster auf der linken Seite der Adobe Analytics-Seite, unter **[!UICONTROL Anmeldedaten]**, wählen **[!UICONTROL OAuth Web]**.
1. Unter **[!UICONTROL Anmeldeinformationen]**, führen Sie folgende Schritte aus:
   * Unter **[!UICONTROL Client-ID]**, wählen **[!UICONTROL Kopieren]** um den Wert zu kopieren. Sie benötigen diesen Wert für die anschließende Analytics-Konfiguration in der Dynamic Media Classic-Desktopanwendung, die befolgt werden soll.
   * Unter **[!UICONTROL Kundengeheimnis]**, wählen **[!UICONTROL Kundengeheimnis abrufen]** , um den zugeordneten Wert anzuzeigen. Auswählen **[!UICONTROL Kopieren]** um den Wert zu kopieren. Sie benötigen diesen Wert für die anschließende Adobe Analytics-Konfiguration in der Dynamic Media Classic-Desktopanwendung, die folgen soll.

## Adobe Analytics in Adobe Dynamic Media Classic konfigurieren {#configure-analytics-in-dmc}

>[!NOTE]
>
>Nach der ursprünglichen Konfiguration von Adobe Analytics in Dynamic Media Classic müssen Sie die Konfiguration nur in folgenden Fällen wiederholen:
>
>* Ein neuer Bericht wird in Analytics hinzugefügt und der Benutzer möchte Beginn beim Senden von Daten an diesen neuen Bericht haben.
>* Der Tracking-Server wird in Adobe Analytics aktualisiert.
>* Eine neue Verfolgungsvariable wird in einem Bericht eingeführt und Sie möchten eine bestimmte Viewer-Variable in der Dynamic Media Classic-Benutzeroberfläche mit dieser neuen Analytics-Variablen verknüpfen.

>


1. In der Nähe der oberen rechten Ecke der Adobe Dynamic Media Classic-Desktopanwendung, navigieren Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]**.
1. Im linken Feld, unter **[!UICONTROL Anwendungseinstellungen]**, wählen **[!UICONTROL Adobe Analytics]**.
1. Auf **[!UICONTROL Adobe Analytics-Konfiguration]** Seite, auswählen **[!UICONTROL Adobe Analytics-Anmeldung]**.
1. In **[!UICONTROL Adobe Analytics-Anmeldung]** im **[!UICONTROL CLIENT-ID]** und **[!UICONTROL CLIENT SECRET]** , fügen Sie die entsprechenden Werte ein, die Sie zuvor kopiert haben.
1. Wählen Sie in der rechten unteren Ecke des Dialogfelds Anmelden aus und führen Sie die Adobe IMS (Identity Management Services)-Anmeldung durch.

   Wenn Sie sich erfolgreich angemeldet haben, wird das Dialogfeld Adobe Analytics-Anmeldung zusammen mit dem **[!UICONTROL Firmen]** Dropdown-Liste, initiiert durch die Firmen, die Ihnen zur Verfügung stehen.

1. Von **[!UICONTROL Firmen]** Dropdown-Liste, wählen Sie eine Firma aus.

   Nach Auswahl einer Firma wird die **[!UICONTROL SUITES]** -Dropdown-Liste, die von den Report Suites initiiert wird, die für die ausgewählte Firma verfügbar sind, wird sichtbar.

1. Von **[!UICONTROL SUITES]** aus, wählen Sie eine Report Suite aus.

   >[!NOTE]
   >
   >Standardmäßig muss der Benutzer wissen, dass beide **[!UICONTROL Firmen]** und **[!UICONTROL SUITES]** Dropdown-Listen sind leer. Der Benutzer muss daher aus jeder Liste einen Wert auswählen.

1. Auswählen **[!UICONTROL OK]** damit Sie die Konfiguration speichern können.

   >[!NOTE]
   >
   >Die **[!UICONTROL Adobe Analytics Server]** Feld wird mit einem vorgeschlagenen Drittanbieter-Tracking-Server gefüllt, der Ihrem Analytics-Namensraum entspricht, wenn Sie **[!UICONTROL OK]**. Wenn Sie einen anderen Tracking-Server verwenden, aktualisieren Sie ihn in diesem Feld, um Datenverluste zu vermeiden.

1. Wählen Sie in der linken unteren Ecke der Seite Adobe Analytics Configuration (-Konfiguration) **[!UICONTROL Speichern]** um sicherzustellen, dass Ihre Adobe Analytics-Kontokonfiguration aktualisiert wird.

>[!MORELIKETHIS]
>
>* [Adobe Analytics-Berichte konfigurieren](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

