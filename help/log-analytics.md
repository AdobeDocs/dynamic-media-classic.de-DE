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
source-git-commit: e3c2dcaa245e486ada62edd554db5a39d495483e
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 20%

---

# Anmelden bei Adobe Analytics{#log-in-to-adobe-analytics}

Bevor Sie sich anmelden, um Adobe Analytics-Berichte zu konfigurieren und Adobe Analytics-Berichtsvariablen mit Adobe Dynamic Media Classic-Ereignissen abzugleichen, stellen Sie sicher, dass Sie Mitglied der Zugriffsgruppe für Webdienste in Adobe Analytics sind. Mitglieder dieser Gruppe können über die Web-Services-API des Experience Cloud auf alle Berichte in den angegebenen Report Suites zugreifen, unabhängig von den in der Benutzeroberfläche festgelegten Berechtigungen. Um ein Mitglied zur Gruppe hinzuzufügen, gehen Sie in Adobe Analytics zu **[!UICONTROL Admin Tools]** > **[!UICONTROL Benutzerverwaltung]** > **[!UICONTROL Gruppen bearbeiten]**.

Bei der Anmeldung können Sie Ihre Experience Cloud-Organisations-ID eingeben, um die neueste Videoanalyseimplementierung zu verwenden. Wenn Sie sich gegen die Eingabe Ihrer ID entscheiden, funktioniert die Videoberichterstellung weiterhin. Dies kann jedoch dazu führen, dass die Daten nicht ordnungsgemäß mit anderen Daten für diesen Client von außerhalb von Adobe Dynamic Media Classic integriert werden.

>[!NOTE]
>
>Wenn Ihr Adobe Analytics-Konto zur Anmeldung zur Adobe IMS-basierten Authentifizierung (Identity Management System) migriert wurde, funktioniert die Eingabe direkter Anmeldeinformationen nicht.

**So melden Sie sich bei Adobe Analytics an:**

1. Navigieren Sie oben rechts auf der Seite &quot;Adobe Dynamic Media Classic&quot;zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]**.
1. Tippen Sie im linken Bereich unter **[!UICONTROL Anwendungseinstellungen]** auf **[!UICONTROL Adobe Analytics]**.
1. Tippen Sie auf der Seite &quot;Adobe Analytics-Konfiguration&quot;auf **[!UICONTROL Adobe Analytics-Anmeldung]**.
1. Geben Sie im Dialogfeld **[!UICONTROL Adobe Analytics Login]** im Textfeld **[!UICONTROL Kennwort]** den Unternehmensnamen, die Experience Cloud-Organisations-ID (optional), den Benutzernamen und den Schlüssel *shared secret* ein.

   Sie können den Schlüssel *shared secret* aus der Analytics-Admin Console abrufen. Siehe [API-Anmeldeinformationen für Benutzerkonten abrufen](https://github.com/AdobeDocs/analytics-2.0-apis/blob/master/create-oauth-client.md).

1. Wählen Sie **[!UICONTROL Anmelden]** aus.
1. Wählen Sie im Dropdown-Menü **[!UICONTROL Report Suite]** eine Report Suite und dann **[!UICONTROL OK]** aus.

   >[!NOTE]
   >
   >Bei der ersten Anmeldung bei Adobe Analytics ist die Dropdown-Liste „Berichts-Suite“ leer. Bei der ersten Anmeldung wählen Sie keine Report Suite aus. Wenn Sie sich zum ersten Mal angemeldet haben, melden Sie sich wieder ab und rufen Sie dann den Adobe Analytics-Anzeigebereich erneut auf. Melden Sie sich wieder an, damit Sie eine Berichts-Suite auswählen können.

>[!MORELIKETHIS]
>
>* [Konfigurieren von Adobe Analytics-Berichten](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

