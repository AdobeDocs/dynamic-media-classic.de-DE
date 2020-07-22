---
title: '"Beginn: Integration von Dynamic Media Classic und Adobe Analytics "'
seo-title: '"Beginn: Integration von Dynamic Media Classic und Adobe Analytics "'
description: 'null'
seo-description: Eine Einführung und ein kurzer Beginn zur Integration von Dynamic Media Classic und Adobe Analytics, mit dem Sie sich schnell vertraut machen können.
uuid: 3f9e2c91-15d4-4b53-8220-9b1ca57c0b1d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: abec9a85-013c-4030-b129-bf27a89cb464
translation-type: tm+mt
source-git-commit: 7c9b1976ced6ef5ad48b624b99aeeffed380168a
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 44%

---


# Quick Beginn: Integration von Dynamic Media Classic und Adobe Analytics {#quick-start-integrating-dmc-analytics}

Mit dem branchenführenden Adobe Analytics können Marketingexperten von einer Stelle aus integrierte Daten beliebiger Online-Initiativen über mehrere Marketing-Kanäle hinweg erfassen, auswerten und optimieren.

Nach der Integration von Adobe Analytics mit Dynamic Media Classic können Sie Berichte über das Verhalten von Website-Besuchern mit Dynamic Media Classic-Viewern auf Ihrer Website abrufen. Wenn ein Besucher einer Website beispielsweise in einem Dynamic Media Classic Zoom Viewer auf eine Zoom-Zielgruppe klickt, zeichnet Adobe Analytics diese Aktion auf. Adobe Analytics-Berichte können kumulative Informationen zur Aktivität von Benutzern in Dynamic Media Classic-Viewern erfassen.

Mit Adobe Analytics-Berichten können Sie sich einen detaillierten Überblick über die Aktivitäten von Kunden auf Ihrer Website verschaffen. Sie können ermitteln, welche Produktpräsentationen zu Geschäftsabschlüssen führen und welche die Kunden nicht ansprechen.

Siehe auch [Videomessung in Adobe Analytics](https://docs.adobe.com/content/help/en/media-analytics/using/media-overview.html).

>[!NOTE]
>
>Ein gültiges Adobe Analytics-Konto ist erforderlich, um Analytics mit Dynamic Media Classic zu integrieren und Analytics-Berichte zu erstellen.

**Quick Beginn**

Diese Kurzanleitung hilft Ihnen, sich schnell mit dem Adobe Analytics-Instrumentierungskit vertraut zu machen.

**1. Log in to Adobe Analytics by way of Dynamic Media Classic and download Adobe Analytics report variables**

>[!NOTE]
>
>Bevor Sie Adobe Analytics-Berichte konfigurieren und Adobe Analytics-Berichtsvariablen Dynamic Media Classic-Ereignissen zuordnen können, überprüfen Sie, ob Sie als Mitglied der Web Service Access-Gruppe in Adobe Analytics hinzugefügt wurden. Mitglieder dieser Gruppe können unabhängig von den in der Schnittstelle eingerichteten Berechtigungen auf alle Berichte in den angegebenen Bericht-Suites über die Marketing Cloud Web-Services-API zugreifen. Um ein Mitglied der Gruppe zu werden, klicken Sie in Adobe Analytics auf **Admin Tools** > **Benutzerverwaltung** > **Gruppen bearbeiten**.

After you have verified that you are a member of the Web Service Access group, in Dynamic Media Classic, click **Setup** > **Application Setup** > **Adobe Analytics**. Klicken Sie auf der Seite „Adobe Analytics-Konfiguration“ auf **Adobe Analytics-Anmeldung**.

Siehe [Anmelden bei Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Geben Sie im Dialogfeld &quot;Adobe Analytics-Anmeldung&quot;Ihre Marketing Cloud-Organisations-ID (optional) und Ihre vollständigen Anmeldeinformationen ein und klicken Sie dann auf **Anmelden**. Wählen Sie im Dropdown-Menü „Berichts-Suite“ den Namen der Berichts-Suite aus, die Sie verwenden möchten.

**2. Weisen Sie Adobe Analytics-Berichtsvariablen Dynamic Media Classic Viewer-Ereignissen und Dynamic Media Classic-Variablen zu**

Geben Sie auf der Seite „Adobe Analytics-Konfiguration“ die Informationen an, die Sie in Adobe Analytics-Berichte aufnehmen möchten. Wählen Sie für jedes Dynamic Media Classic Viewer-Ereignis, über das Sie Informationen erhalten möchten, eine Adobe Analytics-Variable (aus Ihrer Report Suite) und eine Dynamic Media Classic-Variable.

* Viewer-Ereignisse beschreiben die Benutzeraktivität, die Sie in Berichten erfassen möchten.
* Dynamic Media Classic-Variablen beschreiben die Daten zu Ereignissen von Benutzern, die von den Berichten bereitgestellt werden sollen.

Die Adobe Analytics-Konfiguration bietet zudem Werkzeuge, um Viewer-Ereignisse zu aktivieren, zu bearbeiten und zu löschen.

Nachdem Sie im Anzeigebereich &quot;Adobe Analytics-Konfiguration&quot;auf &quot;Speichern&quot;geklickt haben, wird angepasster Trackingcode zur Messung der Aktivität von Benutzern in Dynamic Media Classic-Viewern eingefügt. Mit dieser Funktion können Sie Benutzeraktivitäten in Adobe Analytics-Berichten verfolgen. 

Siehe [Konfigurieren von Adobe Analytics-Berichten](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

**3. Veröffentlichen von Dynamic Media Classic-Viewern**

Veröffentlichen Sie Ihre Dynamic Media Classic-Viewer, damit die Viewer (mit Code zur Verfolgung der Aktivität von Benutzern in Adobe Analytics-Berichten) auf Dynamic Media Classic-Servern geladen werden. Nach der Veröffentlichung sind diese Informationen in den Viewern enthalten und können für die Adobe Analytics-Analyse verwendet werden. 

Siehe [Veröffentlichen von Konfigurationsinformationen](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

**4. Platzieren Sie Dynamic Media Classic-Viewer auf Ihrer Website**

Platzieren Sie die Dynamic Media Classic-Viewer mit dem Adobe Analytics-Trackingcode auf Ihrer Website.

**5. Testen Sie die Adobe Analytics-Integration, indem Sie einen Adobe Analytics-Bericht anzeigen.**

Rufen Sie die Adobe Analytics-Website auf, um Adobe Analytics-Berichte anzuzeigen. Auf der Berichterstellungsseite können Sie sowohl Daten anzeigen als auch Diagramme und Tabellen zur Auswertung von Benutzeraktivitäten mit verschiedenen Viewern generieren. 

Siehe [Testen der Adobe Analytics-Integration durch Anzeigen eines Adobe Analytics-Berichts](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
