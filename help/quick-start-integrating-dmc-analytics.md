---
title: '"Schnellstart: Integrieren von Adobe Dynamic Media Classic und Adobe Analytics"'
description: Eine Einführung und ein Schnellstart zur Integration von Adobe Dynamic Media Classic und Adobe Analytics, damit Sie schnell arbeiten können.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
source-git-commit: 44045daa35052f01a26c67e0b2a0fb1405c53292
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 27%

---

# Schnellstart: Integrieren von Adobe Dynamic Media Classic und Adobe Analytics {#quick-start-integrating-dmc-analytics}

Mit dem branchenführenden Adobe Analytics können Marketingexperten von einer Stelle aus integrierte Daten beliebiger Online-Initiativen über mehrere Marketing-Kanäle hinweg erfassen, auswerten und optimieren.

Nach der Integration von Adobe Analytics mit Adobe Dynamic Media Classic können Sie Berichte über das Verhalten von Website-Besuchern abrufen, die Adobe Dynamic Media Classic-Viewer auf Ihrer Website verwenden. Wenn beispielsweise ein Website-Besucher in einem Dynamic Media Classic Zoom-Viewer auf ein Zoomziel klickt, zeichnet Adobe Analytics diese Aktion auf. Adobe Analytics-Berichte können kumulative Informationen über Benutzeraktivitäten in Adobe Dynamic Media Classic-Viewern erfassen.

Mit Adobe Analytics-Berichten können Sie sich einen detaillierten Überblick über die Aktivitäten von Kunden auf Ihrer Website verschaffen. Sie können bestimmen, welche Produktpräsentationen zu Konversion führen und die kein Kundeninteresse wecken.

Siehe auch [Videomessung in Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

>[!NOTE]
>
>Zum Integrieren von Analytics in Adobe Dynamic Media Classic und zum Generieren von Analytics-Berichten ist ein gültiges Adobe Analytics-Konto erforderlich.

Diese Kurzanleitung hilft Ihnen, sich schnell mit dem Adobe Analytics-Instrumentierungskit vertraut zu machen.

## 1. Melden Sie sich über Adobe Dynamic Media Classic bei Adobe Analytics an und laden Sie Adobe Analytics-Berichtsvariablen herunter

>[!NOTE]
>
>Bevor Sie Adobe Analytics-Berichte konfigurieren und Adobe Analytics-Berichtsvariablen mit Adobe Dynamic Media Classic-Ereignissen verknüpfen können, stellen Sie sicher, dass Sie als Mitglied der Zugriffsgruppe für Webdienste in Adobe Analytics hinzugefügt wurden. Mitglieder dieser Gruppe können über die Web-Services-API des Experience Cloud auf alle Berichte in den angegebenen Report Suites zugreifen, unabhängig von den in der Benutzeroberfläche festgelegten Berechtigungen. Um ein Mitglied zur Gruppe hinzuzufügen, gehen Sie in Adobe Analytics zu **[!UICONTROL Admin Tools]** > **[!UICONTROL Benutzerverwaltung]** > **[!UICONTROL Gruppen bearbeiten]**.

Nachdem Sie sich vergewissert haben, dass Sie Mitglied der Zugriffsgruppe für Webdienste sind, gehen Sie in Adobe Dynamic Media Classic zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Adobe Analytics]**. Wählen Sie auf der Seite &quot;Adobe Analytics Configuration&quot;die Option **[!UICONTROL Adobe Analytics Login]**.

Siehe [Anmelden bei Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Geben Sie im Dialogfeld &quot;Adobe Analytics Login&quot;Ihre Experience Cloud-Organisations-ID (optional) und Ihre vollständigen Anmeldeinformationen ein und wählen Sie **[!UICONTROL Login]** aus. Wählen Sie im Dropdown-Menü „Berichts-Suite“ den Namen der Berichts-Suite aus, die Sie verwenden möchten.

## 2. Weisen Sie Adobe Analytics-Berichtsvariablen Adobe Dynamic Media Classic-Viewer-Ereignissen und Adobe Dynamic Media Classic-Variablen zu

Geben Sie auf der Seite „Adobe Analytics-Konfiguration“ die Informationen an, die Sie in Adobe Analytics-Berichte aufnehmen möchten. Wählen Sie für jede Adobe Dynamic Media Classic Viewer-Ereignis, für die Sie Informationen benötigen, eine Adobe Analytics-Variable (aus Ihrer Report Suite) und eine Dynamic Media Classic-Variable der Adobe.

* Viewer-Ereignisse beschreiben die Benutzeraktivität, die Sie in Berichten erfassen möchten.
* Adobe Dynamic Media Classic -Variablen beschreiben die Daten zu Benutzerereignissen, die die Berichte bereitstellen sollen.

Die Adobe Analytics-Konfiguration bietet zudem Werkzeuge, um Viewer-Ereignisse zu aktivieren, zu bearbeiten und zu löschen.

Nachdem Sie auf der Adobe Analytics-Konfigurationsseite **[!UICONTROL Speichern]** ausgewählt haben, wird der benutzerdefinierte Trackingcode zur Messung der Benutzeraktivität in die Adobe Dynamic Media Classic-Viewer eingefügt. Mit dieser Funktion können Sie Benutzeraktivitäten in Adobe Analytics-Berichten verfolgen. 

Siehe [Konfigurieren von Adobe Analytics-Berichten](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## 3. Veröffentlichen Sie Ihre Adobe Dynamic Media Classic-Viewer

Veröffentlichen Sie Ihre Adobe Dynamic Media Classic-Viewer, damit die Viewer (mit Code zur Benutzeraktivität in Adobe Analytics-Berichten) auf Adobe Dynamic Media Classic-Servern geladen werden. Nach der Veröffentlichung sind diese Informationen in den Viewern enthalten und können für die Adobe Analytics-Analyse verwendet werden. 

Siehe [Veröffentlichungskonfigurationsinformationen](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. Platzieren Sie Adobe Dynamic Media Classic-Viewer auf Ihrer Website.

Platzieren Sie die Adobe Dynamic Media Classic-Viewer mit dem Adobe Analytics-Trackingcode auf Ihrer Website.

## 5. Testen Sie die Adobe Analytics-Integration, indem Sie einen Adobe Analytics-Bericht anzeigen.

Rufen Sie die Adobe Analytics-Website auf, um Adobe Analytics-Berichte anzuzeigen. Auf der Berichterstellungsseite können Sie sowohl Daten anzeigen als auch Diagramme und Tabellen zur Auswertung von Benutzeraktivitäten mit verschiedenen Viewern generieren. 

Siehe [Testen der Adobe Analytics-Integration durch Anzeigen eines Adobe Analytics-Berichts](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
