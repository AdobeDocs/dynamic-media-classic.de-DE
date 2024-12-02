---
title: 'Schnellstart: Integration von Adobe Dynamic Media Classic und Adobe Analytics'
description: Eine Einführung und ein Schnellstart zur Integration von Adobe Dynamic Media Classic und Adobe Analytics.
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

# Schnellstart: Integration von Adobe Dynamic Media Classic und Adobe Analytics {#quick-start-integrating-dmc-analytics}

Mit dem branchenführenden Adobe Analytics können Marketingexperten von einer Stelle aus integrierte Daten beliebiger Online-Initiativen über mehrere Marketing-Kanäle hinweg erfassen, auswerten und optimieren.

Nach der Integration von Adobe Analytics mit Adobe Dynamic Media Classic können Sie Berichte über das Verhalten von Website-Besuchern mit Adobe Dynamic Media Classic-Viewern auf Ihrer Website abrufen. Wenn beispielsweise ein Website-Besucher in einem Adobe Dynamic Media Classic-Zoom-Viewer ein Zoomziel auswählt, wird diese Aktion von Adobe Analytics aufgezeichnet. Adobe Analytics-Berichte können kumulative Informationen über Benutzeraktivitäten in Adobe Dynamic Media Classic-Viewern erfassen.

Mit Adobe Analytics-Berichten können Sie sich einen detaillierten Überblick über die Aktivitäten von Kunden auf Ihrer Website verschaffen. Sie können bestimmen, welche Produktpräsentationen zu Konversion führen und die kein Kundeninteresse wecken.

Siehe auch [Videomessung in Adobe Analytics](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

>[!NOTE]
>
>Zur Integration von Analytics in Adobe Dynamic Media Classic und zur Generierung von Analytics-Berichten ist ein gültiges Adobe Analytics-Konto erforderlich.

Diese Kurzanleitung soll Ihnen den schnellen Einstieg in das Adobe Analytics Instrumentation Kit erleichtern.

## 1. Melden Sie sich über Adobe Dynamic Media Classic bei Adobe Analytics an und laden Sie die Adobe Analytics-Berichtsvariablen herunter

>[!NOTE]
>
>Stellen Sie sicher, dass Sie als Mitglied der Gruppe Web Service Access in Adobe Analytics hinzugefügt wurden. Führen Sie diese Überprüfung aus, bevor Sie Adobe Analytics-Berichte konfigurieren. Und bevor Sie Adobe Analytics-Berichtsvariablen mit Adobe Dynamic Media Classic-Ereignissen verknüpfen. Mitglieder dieser Gruppe können auf alle Berichte in den angegebenen Report Suites zugreifen. Sie können dies mit der Experience Cloud Web Services API tun, unabhängig von den in der Benutzeroberfläche festgelegten Berechtigungen. Um ein Mitglied zur Gruppe hinzuzufügen, gehen Sie in Adobe Analytics zu &quot;**[!UICONTROL Admin Tools]**&quot;> &quot;**[!UICONTROL Benutzerverwaltung]**&quot;> &quot;**[!UICONTROL Gruppen bearbeiten]**&quot;.

Nachdem Sie sich vergewissert haben, dass Sie Mitglied der Zugriffsgruppe für Webdienste sind, gehen Sie in Adobe Dynamic Media Classic zu &quot;**[!UICONTROL Setup]**&quot;> &quot;**[!UICONTROL Anwendungseinstellungen]**&quot;> &quot;**[!UICONTROL Adobe Analytics]**&quot;. Wählen Sie auf der Seite &quot;Adobe Analytics-Konfiguration&quot;die Option **[!UICONTROL Adobe Analytics-Anmeldung]**.

Siehe [Anmelden bei Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Geben Sie im Dialogfeld &quot;Adobe Analytics Login&quot;Ihre Experience Cloud-Organisations-ID (optional) und Ihre vollständigen Anmeldedaten ein und wählen Sie dann **[!UICONTROL Login]** aus. Wählen Sie im Dropdown-Menü „Berichts-Suite“ den Namen der Berichts-Suite aus, die Sie verwenden möchten.

## 2. Weisen Sie Adobe Analytics-Berichtsvariablen zu Adobe Dynamic Media Classic-Viewer- und Adobe Dynamic Media Classic-Variablen zu

Geben Sie auf der Seite „Adobe Analytics-Konfiguration“ die Informationen an, die Sie in Adobe Analytics-Berichte aufnehmen möchten. Wählen Sie für jedes Adobe Dynamic Media Classic-Viewer-Ereignis, für das Sie Informationen benötigen, eine Adobe Analytics-Variable (aus Ihrer Report Suite) und eine Adobe Dynamic Media Classic-Variable aus.

* Viewer-Ereignisse beschreiben die Benutzeraktivität, die Sie in Berichten erfassen möchten.
* Adobe Dynamic Media Classic-Variablen beschreiben die Daten zu Benutzerereignissen, die die Berichte bereitstellen sollen.

Die Adobe Analytics-Konfiguration bietet zudem Werkzeuge, um Viewer-Ereignisse zu aktivieren, zu bearbeiten und zu löschen.

Nachdem Sie auf der Seite &quot;Adobe Analytics-Konfiguration&quot;die Option **[!UICONTROL Speichern]** ausgewählt haben, wird ein benutzerdefinierter Trackingcode zur Messung der Benutzeraktivität in die Adobe Dynamic Media Classic-Viewer eingefügt. Mit dieser Funktion können Sie Benutzeraktivitäten in Adobe Analytics-Berichten verfolgen. 

Siehe [Konfigurieren von Adobe Analytics-Berichten](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## 3. Publish Ihrer Adobe Dynamic Media Classic-Viewer

Publish Sie Ihre Adobe Dynamic Media Classic-Viewer, damit die Viewer (mit Code zur Verfolgung der Benutzeraktivität in Adobe Analytics-Berichten) auf Adobe Dynamic Media Classic-Servern geladen werden. Nach der Veröffentlichung sind diese Informationen in Viewern enthalten. Verwenden Sie sie zur Analyse durch Adobe Analytics.

Siehe [Publish-Konfigurationsinformationen](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. Platzieren Sie Adobe Dynamic Media Classic-Viewer auf Ihrer Website.

Platzieren Sie die Adobe Dynamic Media Classic-Viewer mit dem Adobe Analytics-Trackingcode auf Ihrer Website.

## 5. Testen Sie die Adobe Analytics-Integration durch Anzeigen eines Adobe Analytics-Berichts.

Rufen Sie die Adobe Analytics-Website auf, um Adobe Analytics-Berichte anzuzeigen. Auf der Berichterstellungsseite können Sie sowohl Daten anzeigen als auch Diagramme und Tabellen zur Auswertung von Benutzeraktivitäten mit verschiedenen Viewern generieren. 

Siehe [Testen der Adobe Analytics-Integration durch Anzeigen eines Adobe Analytics-Berichts](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
