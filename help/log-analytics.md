---
title: Anmelden bei Adobe Analytics
seo-title: Anmelden bei Adobe Analytics
description: 'null'
seo-description: Hier erfahren Sie, wie Sie sich bei Adobe Analytics anmelden.
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
translation-type: tm+mt
source-git-commit: ff112497b41f71b77f4afa47d331a1a9bc1e2d07
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 37%

---


# Anmelden bei Adobe Analytics{#log-in-to-adobe-analytics}

Bevor Sie sich anmelden, um Adobe Analytics-Berichte zu konfigurieren und Adobe Analytics-Berichtsvariablen Dynamic Media Classic-Ereignissen zuzuordnen, überprüfen Sie, ob Sie als Mitglied der Web Service Access-Gruppe in Adobe Analytics hinzugefügt wurden. Mitglieder dieser Gruppe können unabhängig von den in der Schnittstelle eingerichteten Berechtigungen auf alle Berichte in den angegebenen Bericht-Suites über die Marketing Cloud Web-Services-API zugreifen. Um ein Mitglied der Gruppe zu werden, klicken Sie in Adobe Analytics auf **Admin Tools** > **Benutzerverwaltung** > **Gruppen bearbeiten**.

Wenn Sie sich anmelden, haben Sie die Möglichkeit, Ihre Marketing Cloud-Organisations-ID einzugeben, um die neueste Videoanalyseimplementierung zu verwenden. Wenn Sie Ihre ID nicht eingeben, funktioniert Video Berichte weiterhin. Es kann jedoch dazu führen, dass die Daten nicht richtig in andere Daten für diesen Client von außerhalb von Dynamic Media Classic integriert werden.

>[!NOTE]
>
>Wenn Ihr Adobe Analytics-Konto zur Anmeldung in die Adobe IMS-basierte Authentifizierung (Identity Management System) migriert wurde, funktioniert die Eingabe direkter Anmeldeinformationen nicht.

**So melden Sie sich bei Adobe Analytics an**

1. Tippen Sie oben rechts auf der Seite &quot;Dynamic Media Classic&quot;auf **[!UICONTROL Einstellungen > Anwendungseinstellungen]**.
1. In the left pane, under **[!UICONTROL Application Setup]**, tap **[!UICONTROL Adobe Analytics]**.
1. In the Adobe Analytics Configuration page, tap **[!UICONTROL Adobe Analytics Login]**.
1. Geben Sie im Dialogfeld &quot; **[!UICONTROL Adobe Analytics-Anmeldung]** &quot;Ihren Firmen-, Marketing Cloud-Organisations-ID (optional)- und Benutzernamen sowie den *gemeinsamen geheimen* Schlüssel in das Textfeld &quot; **[!UICONTROL Kennwort]** &quot;ein.

   Sie können den *gemeinsamen geheimen* Schlüssel aus der Analytics Admin-Konsole abrufen. Siehe [API-Anmeldeinformationen für Benutzerkonten](https://helpx.adobe.com/analytics/kb/how-to-get-api-credentials-for-user-accounts-.html)abrufen.

1. Klicken Sie auf **[!UICONTROL Anmelden]**.
1. Wählen Sie im Dropdownmenü **[!UICONTROL Report Suite]** eine Report Suite und klicken Sie dann auf **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >Bei der ersten Anmeldung bei Adobe Analytics ist die Dropdown-Liste „Berichts-Suite“ leer. Bei der ersten Anmeldung wählen Sie keine Report Suite aus. Wenn Sie sich zum ersten Mal angemeldet haben, melden Sie sich wieder ab und rufen Sie dann den Adobe Analytics-Anzeigebereich erneut auf. Melden Sie sich wieder an, damit Sie eine Berichts-Suite auswählen können.

>[!MORELIKETHIS]
>
>* [Konfigurieren von Adobe Analytics-Berichten](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

