---
title: '" Kurzanleitung: Integration von Dynamic Media Classic und Adobe Analytics "'
seo-title: '" Kurzanleitung: Integration von Dynamic Media Classic und Adobe Analytics "'
description: 'null'
seo-description: Eine Einführung und Schnellstart zur Integration von Dynamic Media Classic und Adobe Analytic, damit Sie schnell losfahren können.
uuid: 3 f 9 e 2 c 91-15 d 4-4 b 53-8220-9 b 1 ca 57 c 0 b 1 d
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/adobe_ analytics_ instrumentation_ kit
discoiquuid: abec 9 a 85-013 c -4030-b 129-bf 27 a 89 cb 464
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Kurzanleitung: Integration von Dynamic Media Classic und Adobe Analytics {#quick-start-integrating-scene-and-adobe-analytics}

Mit dem branchenführenden Adobe Analytics können Marketingexperten von einer Stelle aus integrierte Daten beliebiger Online-Initiativen über mehrere Marketing-Kanäle hinweg erfassen, auswerten und optimieren.

Nach der Integration von Adobe Analytics in das Scene 7 Publishing System können Sie Berichte über das Verhalten von Besuchern von Websites in der Website Ihrer Website erhalten. Wenn ein Besucher der Website beispielsweise in einem dynamischen Media-Zoom-Viewer auf ein Zoomziel klickt, zeichnet Adobe Analytics diese Aktion auf. Adobe Analytics-Berichte können kumulative Informationen über Benutzeraktivitäten in dynamischen Media Classic-Viewern erfassen.

Mit Adobe Analytics-Berichten können Sie sich einen detaillierten Überblick über die Aktivitäten von Kunden auf Ihrer Website verschaffen. Sie können ermitteln, welche Produktpräsentationen zu Geschäftsabschlüssen führen und welche die Kunden nicht ansprechen.

Siehe auch [Videomessung in Adobe Analytics](https://marketing.adobe.com/resources/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Um Adobe Analytics in das Scene7 Publishing System integrieren und Analytics-Berichte erstellen zu können, ist ein gültiges Adobe Analytics-Konto erforderlich.

**Kurzanleitung**

Diese Kurzanleitung hilft Ihnen, sich schnell mit dem Adobe Analytics-Instrumentierungskit vertraut zu machen.

**1. Log in to Adobe Analytics by way of Dynamic Media Classic and download Adobe Analytics report variables**

>[!NOTE]
>
>Bevor Sie Adobe Analytics-Berichte konfigurieren und Adobe Analytics-Berichtsvariablen zu dynamischen Media Classic-Ereignissen zuordnen können, vergewissern Sie sich, dass Sie in Adobe Analytics als Mitglied der Web Service Access-Gruppe hinzugefügt wurden. Mitglieder dieser Gruppe können unabhängig von den in der Schnittstelle eingerichteten Berechtigungen auf alle Berichte in den angegebenen Bericht-Suites über die Marketing Cloud Web-Services-API zugreifen. Um ein Mitglied der Gruppe zu werden, klicken Sie in Adobe Analytics auf **Admin Tools** &gt; **Benutzerverwaltung** &gt; **Gruppen bearbeiten**.

After you have verified that you are a member of the Web Service Access group, in Dynamic Media Classic, click **Setup** &gt; **Application Setup** &gt; **Adobe Analytics**. Klicken Sie auf der Seite „Adobe Analytics-Konfiguration“ auf **Adobe Analytics-Anmeldung**.

Siehe [Anmelden bei Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Geben Sie im Dialogfeld "Adobe Analytics-Anmeldung" Ihre Marketing Cloud-Organisations-ID (optional) ein und klicken Sie dann auf **Anmelden**. Wählen Sie im Dropdown-Menü „Berichts-Suite“ den Namen der Berichts-Suite aus, die Sie verwenden möchten.

**2. Weisen Sie Adobe Analytics-Berichtsvariablen dynamischer Media Classic Classic-Viewer-Ereignisse und Dynamic Media Classic-Variablen zu.**

Geben Sie auf der Seite „Adobe Analytics-Konfiguration“ die Informationen an, die Sie in Adobe Analytics-Berichte aufnehmen möchten. Wählen Sie für jedes dynamische Media-Viewer-Ereignis, dessen Informationen Sie benötigen, eine Adobe Analytics-Variable (aus Ihrer Report Suite) und eine dynamische Media Classic-Variable aus.

* Viewer-Ereignisse beschreiben die Benutzeraktivität, die Sie in Berichten erfassen möchten.
* Dynamische Media Classic-Variablen beschreiben die Daten zu Benutzerereignissen, die die Berichte liefern sollen.

Die Adobe Analytics-Konfiguration bietet zudem Werkzeuge, um Viewer-Ereignisse zu aktivieren, zu bearbeiten und zu löschen.

Nachdem Sie im Anzeigebereich "Adobe Analytics-Konfiguration" auf" Speichern" geklickt haben, wird angepasster Code zum Erfassen von Benutzeraktivitäten in die Dynamic Media Classic-Viewer eingefügt. Mit dieser Funktion können Sie Benutzeraktivitäten in Adobe Analytics-Berichten verfolgen. 

Siehe [Konfigurieren von Adobe Analytics-Berichten](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

**3. Veröffentlichen von dynamischen Media Classic-Viewern**

Veröffentlichen Sie Ihre dynamischen Media Classic-Viewer, damit die Viewer (mit Code zum Verfolgen der Benutzeraktivität in Adobe Analytics-Berichten) auf dynamischen Media Classic-Servern geladen werden. Nach der Veröffentlichung sind diese Informationen in den Viewern enthalten und können für die Adobe Analytics-Analyse verwendet werden. 

Siehe [Veröffentlichen von Konfigurationsinformationen](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

**4. Platzieren Sie dynamische Media Classic-Viewer auf Ihrer Website.**

Platzieren Sie die Viewer für dynamische Medien mit dem Adobe Analytics-Trackingcode auf Ihrer Website.

**5. Testen Sie die Adobe Analytics-Integration, indem Sie einen Adobe Analytics-Bericht anzeigen.**

Rufen Sie die Adobe Analytics-Website auf, um Adobe Analytics-Berichte anzuzeigen. Auf der Berichterstellungsseite können Sie sowohl Daten anzeigen als auch Diagramme und Tabellen zur Auswertung von Benutzeraktivitäten mit verschiedenen Viewern generieren. 

Siehe [Testen der Adobe Analytics-Integration durch Anzeigen eines Adobe Analytics-Berichts](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
