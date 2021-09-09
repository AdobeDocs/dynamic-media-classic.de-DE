---
title: Testen Sie Assets, bevor Sie sie veröffentlichen
description: Erfahren Sie, wie Sie Assets in Adobe Dynamic Media Classic testen, bevor Sie sie veröffentlichen.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
source-git-commit: e8e2eeba81f93cd72bdf5e09d5441de9bd3bc776
workflow-type: tm+mt
source-wordcount: '1049'
ht-degree: 32%

---

# Testen Sie Assets, bevor Sie sie veröffentlichen {#testing-assets-before-making-them-public}

Mit Secure Testing können Sie eine sichere Testumgebung definieren und eine robuste B2B-Lösung erstellen, die auf einem konfigurierbaren Satz von IP-Adressen und -Bereichen basiert. Mit dieser Funktion können Sie Ihre Adobe Dynamic Media Classic-Implementierungen mit der Architektur Ihres Content-Management- und Business-Systems abgleichen.

Mit Secure Testing können Sie eine Vorabversion (Staging) der Website mit unveröffentlichtem Inhalt in der Vorschau anzeigen.

Erstellen Sie bei Bedarf eine Staging-Umgebung, anstatt Assets aus folgenden Gründen öffentlich verfügbar zu machen:

* Vorschau der Websites vor der Veröffentlichung (Staging-Website).
* Bereitstellen von Assets, deren Zugriff eingeschränkt sein soll, wie E-Kataloge, die Preise in einer B2B-Web-Anwendung anzeigen.
* Verwenden von Assets hinter einer Firewall als Teil des Produktinformations-Managementsystems, der Kundenservice-Anwendung, Online-Kursen usw.

>[!NOTE]
>
>Secure Testing hat keine Auswirkungen auf den Zugriff auf Adobe Dynamic Media Classic. Die Sicherheit von Adobe Dynamic Media Classic bleibt konsistent und erfordert die üblichen Anmeldeinformationen für den Zugriff auf Adobe Dynamic Media Classic und zugehörige Webdienste.

## Funktionsweise von Secure Testing {#how-secure-testing-works}

Die meisten Unternehmen haben eine Firewall für den Internetzugriff. Der Zugriff auf das Internet ist damit auf bestimmten Routen möglich und normalerweise auf bestimmte öffentliche IP-Adressen beschränkt.

Über Ihr Unternehmensnetzwerk können Sie Ihre öffentliche IP-Adresse mithilfe von Websites wie [https://www.whatismyip.com](https://www.whatismyip.com/) ermitteln oder diese Informationen von Ihrer IT-Organisation anfordern.

Mit dem Secure Testing richtet Adobe Dynamic Media Classic einen dedizierten Image-Server für Staging-Umgebungen oder interne Anwendungen ein. Mit jeder Anforderung bei diesem Server wird die Original-IP-Adresse überprüft. Wenn die eingehende Anforderung nicht auf der genehmigten Liste der IP-Adressen steht, wird eine Fehlerantwort zurückgesendet. Der Adobe Dynamic Media Classic-Unternehmensadministrator konfiguriert die Liste genehmigter IP-Adressen für die sichere Testumgebung seines Unternehmens.

Da der Speicherort der ursprünglichen Anforderung bestätigt werden muss, wird der Traffic des Secure Testing-Dienstes nicht über ein Inhaltsverteilungsnetzwerk wie den öffentlichen Dynamic Media Image Server-Traffic geleitet. Anforderungen an den Secure Testing-Dienst weisen im Vergleich zu den öffentlichen Dynamic Media-Bildservern eine etwas höhere Latenz auf.

Unveröffentlichte Assets sind sofort über den Secure Testing-Dienst verfügbar und müssen nicht erst veröffentlicht werden. Auf diese Weise können Sie eine Vorschau ausführen, bevor Assets auf ihrem öffentlichen Bildserver veröffentlicht werden.

>[!NOTE]
>
>Sichere Testdienste verwenden den Katalogserver, der mit einem internen Veröffentlichungskontext konfiguriert ist. Wenn Ihr Unternehmen daher für die Veröffentlichung auf Secure Testing konfiguriert ist, werden hochgeladene Assets in Adobe Dynamic Media Classic sofort in den Secure Testing Services verfügbar. Diese Funktion gilt unabhängig davon, ob die Assets beim Hochladen zur Veröffentlichung markiert sind.

Secure Testing Services unterstützen derzeit die folgenden Asset-Typen und -Funktionen:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Bilder.
* Vignetten (Render-Server-Anforderungen).
* Render Server-Anforderungen (unterstützt, aber explizit vom Kunden angefordert).
* Sätze, einschließlich Bildsätzen, E-Katalog, Rendersets und Mediensets.
* Standard-Adobe Dynamic Media Classic Rich-Media-Viewer.
* Adobe Dynamic Media Classic OnDemand JSP-Seiten.
* Statische Inhalte wie PDF-Dateien und progressiv bereitgestellte Videos.
* HTTP-Videostreaming.
* Progressives Videostreaming.

Die folgenden Asset-Typen und -Funktionen werden derzeit nicht unterstützt:

* RTMP-Videostreaming
* UGC-Dienste (benutzergenerierte Inhalte)
* Web-to-Print
* Adobe Dynamic Media Classic Info oder eCatalog-Suche

## Testen des Secure Testing-Dienstes {#testing-the-secure-testing-service}

Testen Sie den Secure Testing-Dienst, um sicherzustellen, dass er wie erwartet funktioniert.

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]*** - If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### Vorbereiten des Kontos

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Wenden Sie sich an die Kundenunterstützung von Adobe und fordern Sie sie auf, sichere Tests für Ihr Konto zu aktivieren.
1. Navigieren Sie in Adobe Dynamic Media Classic auf der Symbolleiste für globale Navigation zu **[!UICONTROL Setup]** > **[!UICONTROL Veröffentlichungseinrichtung]** > **[!UICONTROL Image-Server]**.
1. Wählen Sie auf der Seite Veröffentlichung zum Image-Server in der Dropdown-Liste **[!UICONTROL Veröffentlichungskontext]** die Option **[!UICONTROL Image-Serving testen]**.
1. Wählen Sie für den Client-Adressfilter **[!UICONTROL Hinzufügen]** aus.
1. Aktivieren Sie das Kontrollkästchen, damit die Adresse aktiviert ist, und geben Sie dann eine IP-Adresse und eine Netzmaske in die entsprechenden Textfelder ein.

   >[!NOTE]
   >
   >Wenn Sie eine einzelne IP-Adresse und Netzmaske hinzufügen, kann diese Adresse Asset-Aufrufe durchführen. Andere von Ihnen hinzugefügte IP-Adressen und Netzmasken dürfen jedoch keine Asset-Aufrufe durchführen. Deaktivieren Sie daher das Kontrollkästchen im obigen Schritt, um die Möglichkeit zu deaktivieren, eine IP-Adresse und eine Netzmaske anzugeben. Auf diese Weise können *alle* IP-Adressen Asset-Aufrufe durchführen, und alle werden angezeigt.

1. Führen Sie einen der folgenden Schritte aus:
   * Wiederholen Sie die beiden vorherigen Schritte, wenn Sie weitere IP-Adressen hinzufügen müssen.
   * Fahren Sie mit dem nächsten Schritt fort.
1. Wählen Sie links unten auf der Seite &quot;Veröffentlichung zum Image-Server&quot;die Option **[!UICONTROL Save]**
1. Laden Sie die gewünschten Bilder in Ihr Adobe Dynamic Media Classic-Konto hoch.

   Siehe [Hochladen von Dateien](uploading-files.md#uploading_files).

1. Vergewissern Sie sich, dass einige der Bilder zur Veröffentlichung markiert und andere nicht markiert sind, und senden Sie dann den Veröffentlichungsauftrag ab.

   Siehe [Veröffentlichen von Dateien](publishing-files.md#publishing_files).

1. Bestimmen Sie den Namen Ihres Secure Testing-Dienstes, indem Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Einstellungen]** navigieren.
1. Suchen Sie auf der Seite „Allgemeine Programmeinstellungen“ in der Gruppe „Server“ den Namen rechts neben **[!UICONTROL Servername für den Testveröffentlichungskontext]**.

Wenden Sie sich an die Adobe Care , wenn der Servername fehlt oder die URLs zum Server nicht funktionieren.

### Vorbereiten von Website-Variationen

Sie benötigen zwei Variationen einer Website, die Links zu veröffentlichten und unveröffentlichten Assets enthält:

* Öffentliche Version - Verknüpfen Sie Assets mit Ihrer herkömmlichen Adobe Dynamic Media Classic URL-Syntax.
* Staging-Version - Verknüpfen Sie Assets mit derselben Syntax wie mit dem Namen der Secure Testing-Site.

### Ausführen von Tests

Führen Sie die folgenden Tests aus:

1. Überprüfen Sie, ob Assets in Ihrem Unternehmensnetzwerk angezeigt werden.

   Innerhalb des Unternehmensnetzwerks, das durch den zuvor definierten IP-Adressbereich identifiziert wurde, zeigt die Staging-Version der Website alle Bilder an, unabhängig davon, ob sie zur Veröffentlichung markiert wurden oder nicht. Daher können Sie Tests durchführen, ohne Bilder versehentlich vor der Genehmigung der Vorschau oder dem Produktstart verfügbar zu machen.

   Vergewissern Sie sich, dass die öffentliche Version Ihrer Site veröffentlichte Assets anzeigt, wie sie zuvor mit Adobe Dynamic Media Classic aufgetreten sind.

1. Überprüfen Sie, ob außerhalb des Unternehmensnetzwerks die unveröffentlichten Assets (die nicht für die Veröffentlichung markiert wurden) vor dem Zugriff durch Dritte geschützt sind.

   Greifen Sie auf Ihr Netzwerk von außerhalb zu (z. B. von Ihrem Heimcomputer oder über eine 3G-Verbindung). Vergewissern Sie sich so, dass die öffentliche Version der Website alle veröffentlichten Assets, jedoch keine unveröffentlichten Inhalte anzeigt.

   Die Staging-Version darf kein Asset anzeigen, weil Sie mit einer nicht zugelassenen IP-Adresse auf den Secure Testing-Dienst zugreifen.
