---
title: Anmelden bei Adobe Analytics
description: Hier erfahren Sie, wie Sie sich bei Adobe Analytics anmelden.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
translation-type: tm+mt
source-git-commit: 2f7366a77c0fa5f3953721cdd5328123d9c2a052
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 35%

---


# Anmelden bei Adobe Analytics{#log-in-to-adobe-analytics}

Bevor Sie sich anmelden, um Adobe Analytics-Berichte zu konfigurieren und Adobe Analytics-Berichtsvariablen Dynamic Media Classic-Ereignissen zuzuordnen, überprüfen Sie, ob Sie als Mitglied der Web Service Access-Gruppe in Adobe Analytics hinzugefügt wurden. Mitglieder dieser Gruppe können unabhängig von den in der Schnittstelle eingerichteten Berechtigungen auf alle Berichte in den angegebenen Bericht-Suites über die Marketing Cloud Web-Services-API zugreifen. Um ein Mitglied der Gruppe zu werden, klicken Sie in Adobe Analytics auf **Admin Tools** > **Benutzerverwaltung** > **Gruppen bearbeiten**.

Wenn Sie sich anmelden, haben Sie die Möglichkeit, Ihre Marketing Cloud-Organisations-ID einzugeben, um die neueste Videoanalyseimplementierung zu verwenden. Wenn Sie Ihre ID nicht eingeben, funktioniert Video Berichte weiterhin. Es kann jedoch dazu führen, dass die Daten nicht richtig in andere Daten für diesen Client von außerhalb von Dynamic Media Classic integriert werden.

>[!NOTE]
>
>Wenn Ihr Adobe Analytics-Konto zur Anmeldung in die Adobe IMS-basierte Authentifizierung (Identity Management System) migriert wurde, funktioniert die Eingabe direkter Anmeldeinformationen nicht.

**So melden Sie sich bei Adobe Analytics an**

1. Tippen Sie in der rechten oberen Ecke der Seite &quot;Dynamic Media Classic&quot;auf **[!UICONTROL Einstellungen > Anwendungseinstellungen]**.
1. Tippen Sie im linken Bereich unter **[!UICONTROL Anwendungseinstellungen]** auf **[!UICONTROL Adobe Analytics]**.
1. Tippen Sie auf der Seite &quot;Adobe Analytics-Konfiguration&quot;auf **[!UICONTROL Adobe Analytics-Anmeldung]**.
1. Geben Sie im Textfeld **[!UICONTROL Adobe Analytics Login]** Ihren Firmen-, Marketing Cloud-Organisations-ID (optional)-, Benutzernamen- und den *Shared-Secret*-Schlüssel in das Textfeld **[!UICONTROL Kennwort]** ein.

   Sie können den Schlüssel *shared secret* aus der Analytics Admin-Konsole abrufen. Siehe [API-Anmeldeinformationen für Benutzerkonten abrufen](https://github.com/AdobeDocs/analytics-2.0-apis/blob/master/create-oauth-client.md).

1. Klicken Sie auf **[!UICONTROL Anmelden]**.
1. Wählen Sie im Dropdownmenü **[!UICONTROL Report Suite]** eine Report Suite und klicken Sie dann auf **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >Bei der ersten Anmeldung bei Adobe Analytics ist die Dropdown-Liste „Berichts-Suite“ leer. Bei der ersten Anmeldung wählen Sie keine Report Suite aus. Wenn Sie sich zum ersten Mal angemeldet haben, melden Sie sich wieder ab und rufen Sie dann den Adobe Analytics-Anzeigebereich erneut auf. Melden Sie sich wieder an, damit Sie eine Berichts-Suite auswählen können.

>[!MORELIKETHIS]
>
>* [Konfigurieren von Adobe Analytics-Berichten](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

