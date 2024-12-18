---
title: 'Schnellstart: Integrieren von Adobe Dynamic Media Classic und Adobe Analytics'
description: Eine Einführung und Kurzanleitung zur Integration von Adobe Dynamic Media Classic und Adobe Analytics.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 21%

---

# Schnellstart: Integrieren von Adobe Dynamic Media Classic und Adobe Analytics {#quick-start-integrating-dmc-analytics}

Mit dem branchenführenden Adobe Analytics können Marketingexperten von einer Stelle aus integrierte Daten beliebiger Online-Initiativen über mehrere Marketing-Kanäle hinweg erfassen, auswerten und optimieren.

Nach der Integration von Adobe Analytics mit Adobe Dynamic Media Classic können Sie Berichte zum Verhalten von Website-Besuchenden abrufen, die Adobe Dynamic Media Classic-Viewer auf Ihrer Website verwenden. Wenn beispielsweise ein Website-Besucher in einem Adobe Dynamic Media Classic Zoom-Viewer ein Zoom-Ziel auswählt, zeichnet Adobe Analytics diese Aktion auf. Adobe Analytics-Berichte können kumulative Informationen zu Benutzeraktivitäten in Adobe Dynamic Media Classic-Viewern erfassen.

Mit Adobe Analytics-Berichten können Sie sich einen detaillierten Überblick über die Aktivitäten von Kunden auf Ihrer Website verschaffen. Sie können bestimmen, welche Produktpräsentationen zu einer Konversion führen und welche kein Kundeninteresse wecken.

Siehe auch [Video in Adobe Analytics messen](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

>[!NOTE]
>
>Für die Integration von Analytics mit Adobe Dynamic Media Classic und die Erstellung von Analytics-Berichten ist ein gültiges Adobe Analytics-Konto erforderlich.

Dieser Schnellstart soll Ihnen den schnellen Einstieg in das Adobe Analytics Instrumentation Kit erleichtern.

## 1. Melden Sie sich über Adobe Dynamic Media Classic bei Adobe Analytics an und laden Sie die Adobe Analytics-Berichtsvariablen herunter

>[!NOTE]
>
>Stellen Sie sicher, dass Sie in Adobe Analytics als Mitglied der Zugriffsgruppe für Webdienste hinzugefügt wurden. Führen Sie diese Überprüfung durch, bevor Sie Adobe Analytics-Berichte konfigurieren. Und bevor Sie Adobe Analytics-Berichtsvariablen Adobe Dynamic Media Classic-Ereignissen zuordnen. Mitglieder dieser Gruppe können auf alle Berichte in den angegebenen Report Suites zugreifen. Sie können dazu die Web-Services-API der Experience Cloud verwenden, unabhängig von den in der Benutzeroberfläche festgelegten Berechtigungen. Um ein Mitglied zur Gruppe hinzuzufügen, gehen Sie in Adobe Analytics zu **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** > **[!UICONTROL Gruppen bearbeiten]**.

Nachdem Sie sich vergewissert haben, dass Sie Mitglied der Zugriffsgruppe für den Webdienst sind, navigieren Sie in Adobe Dynamic Media Classic zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Adobe Analytics]**. Wählen Sie auf der Seite &quot;Adobe Analytics-Konfiguration“ **[!UICONTROL Adobe Analytics-Anmeldung]** aus.

Siehe [Anmelden bei Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Geben Sie im Dialogfeld &quot;Adobe Analytics-Anmeldung“ Ihre Experience Cloud-Organisations-ID (optional) und Ihre vollständigen Anmeldeinformationen ein und wählen Sie dann **[!UICONTROL Anmeldung]** aus. Wählen Sie im Dropdown-Menü „Berichts-Suite“ den Namen der Berichts-Suite aus, die Sie verwenden möchten.

## 2. Zuweisen von Adobe Analytics-Berichtsvariablen zu Adobe Dynamic Media Classic-Viewer-Ereignissen und Adobe Dynamic Media Classic-Variablen

Geben Sie auf der Seite „Adobe Analytics-Konfiguration“ die Informationen an, die Sie in Adobe Analytics-Berichte aufnehmen möchten. Wählen Sie für jedes Adobe Dynamic Media Classic-Viewer-Ereignis, zu dem Sie Informationen benötigen, eine Adobe Analytics-Variable (aus Ihrer Report Suite) und eine Adobe Dynamic Media Classic-Variable aus.

* Viewer-Ereignisse beschreiben die Benutzeraktivität, die Sie in Berichten erfassen möchten.
* Adobe Dynamic Media Classic-Variablen beschreiben die Daten zu Benutzerereignissen, die die Berichte bereitstellen sollen.

Die Adobe Analytics-Konfiguration bietet zudem Werkzeuge, um Viewer-Ereignisse zu aktivieren, zu bearbeiten und zu löschen.

Nachdem Sie auf **[!UICONTROL Seite &quot;Adobe Analytics-]**&quot; die Option „Speichern“ ausgewählt haben, wird ein benutzerdefinierter Trackingcode zur Messung der Benutzeraktivität in die Adobe Dynamic Media Classic-Viewer eingefügt. Mit dieser Funktion können Sie Benutzeraktivitäten in Adobe Analytics-Berichten verfolgen. 

Siehe [Konfigurieren von Adobe Analytics-](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## 3. Publish - Ihre Adobe Dynamic Media Classic-Viewer

Publish unterstützt die Adobe Dynamic Media Classic-Viewer, sodass die Viewer (mit Code zum Tracking der Benutzeraktivität in Adobe Analytics-Berichten) auf Adobe Dynamic Media Classic-Servern geladen werden. Nach der Veröffentlichung werden diese Informationen in die Viewer aufgenommen. Verwenden Sie es für die Analyse durch Adobe Analytics.

Siehe [Publish-Konfigurationsinformationen](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. Platzieren von Adobe Dynamic Media Classic Viewers auf Ihrer Website

Platzieren Sie die Adobe Dynamic Media Classic-Viewer mit Adobe Analytics-Trackingcode auf Ihrer Website.

## 5. Testen der Adobe Analytics-Integration durch Anzeigen eines Adobe Analytics-Berichts

Rufen Sie die Adobe Analytics-Website auf, um Adobe Analytics-Berichte anzuzeigen. Auf der Berichterstellungsseite können Sie sowohl Daten anzeigen als auch Diagramme und Tabellen zur Auswertung von Benutzeraktivitäten mit verschiedenen Viewern generieren. 

Siehe [Testen der Adobe Analytics-Integration durch Anzeigen eines Adobe Analytics-](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
