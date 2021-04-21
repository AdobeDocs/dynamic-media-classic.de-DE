---
title: Testen von Assets vor dem Veröffentlichen
description: Erfahren Sie, wie Sie Assets testen, bevor Sie sie veröffentlichen.
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic, Asset Management
role: Business Practitioner
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
translation-type: tm+mt
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '1100'
ht-degree: 55%

---

# Testen von Assets vor dem Veröffentlichen {#testing-assets-before-making-them-public}

Mit Secure Testing können Sie eine sichere Testumgebung definieren und eine robuste B2B-Lösung erstellen, die auf einem konfigurierbaren Satz aus IP-Adressen und -Bereichen basiert. Mit dieser Funktion können Sie Ihre Dynamic Media Classic-Bereitstellungen mit der Architektur Ihrer Content-Management- und Commerce-Plattform abgleichen.

Mit Secure Testing können Sie eine Vorabversion (Staging) der Website mit unveröffentlichtem Inhalt in der Vorschau anzeigen.

Möglicherweise bevorzugen Sie aus folgenden Gründen das Erstellen einer Staging-Umgebung, anstatt Assets öffentlich verfügbar zu machen:

* Vorschau der Websites vor der Veröffentlichung (Staging-Website).
* Bereitstellen von Assets, deren Zugriff eingeschränkt sein soll, wie E-Kataloge, die Preise in einer B2B-Web-Anwendung anzeigen.
* Verwenden von Assets hinter einer Firewall als Teil des Produktinformations-Managementsystems, der Kundenservice-Anwendung, Online-Kursen usw.

>[!NOTE]
>
>Secure Testing beeinträchtigt nicht den Zugriff auf Dynamic Media Classic. Die Sicherheit von Dynamic Media Classic bleibt einheitlich und erfordert die üblichen Anmeldeinformationen für den Zugriff auf Dynamic Media Classic und zugehörige Webdienste.

## Funktionsweise von Secure Testing {#how-secure-testing-works}

Die meisten Unternehmen haben eine Firewall für den Internetzugriff. Der Zugriff auf das Internet ist damit auf bestimmten Routen möglich und normalerweise auf bestimmte öffentliche IP-Adressen beschränkt.

In Ihrem Unternehmensnetzwerk können Sie Ihre öffentliche IP-Adresse mithilfe von Websites wie https://whatismyip.com herausfinden oder diese Informationen bei Ihrer IT-Abteilung anfordern.

Mit dem Secure Testing stellt Dynamic Media Classic einen eigenen Image-Server für Staging-Umgebung oder interne Anwendungen her. Mit jeder Anforderung bei diesem Server wird die Original-IP-Adresse überprüft. Wenn die eingehende Anforderung nicht auf der genehmigten Liste der IP-Adressen steht, wird eine Fehlerantwort zurückgesendet. Der Dynamic Media Classic Firma Administrator konfiguriert die genehmigte Liste von IP-Adressen für die Secure Testing-Umgebung der Firma.

Da der Speicherort der ursprünglichen Anforderung bestätigt werden muss, wird der Traffic des Secure Testing-Dienstes nicht über ein Inhaltsverteilungsnetzwerk wie den öffentlichen Dynamic Media Image Server-Traffic geleitet. Anforderungen an den Secure Testing-Dienst weisen möglicherweise eine etwas höhere Latenz auf als die öffentlichen Dynamic Media-Image-Server.

Unveröffentlichte Assets sind sofort über den Secure Testing-Dienst verfügbar und müssen nicht erst veröffentlicht werden. Dies ermöglicht es Ihnen, eine Vorschau auszuführen, bevor Assets auf dem für die Öffentlichkeit zugänglichen Image-Server veröffentlicht werden.

>[!NOTE]
>
>Secure Testing-Dienste erweitern den Katalogserver, der mit einem internen Veröffentlichungskontext konfiguriert ist. Wenn Ihre Firma für die Veröffentlichung auf Secure Testing konfiguriert ist, beachten Sie daher, dass hochgeladene Assets in Dynamic Media Classic sofort in Secure Testing-Diensten verfügbar sind. Dies gilt unabhängig davon, ob die Assets für das Hochladen oder Veröffentlichen markiert wurden.

Secure Testing-Dienste unterstützen derzeit die folgenden Asset-Typen und -Funktionen:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Bilder.
* Vignetten (Render-Server-Anforderungen).
* Render-Server-Anforderungen (unterstützt, aber explizit vom Kunden angefordert).
* Sätze, einschließlich Bildsätzen, E-Katalog, Rendersets und Mediensets.
* Standard-Rich-Media-Viewer von Dynamic Media Classic
* Dynamic Media Classic OnDemand JSP-Seiten.
* Statische Inhalte wie PDF-Dateien und progressiv bereitgestellte Videos.
* HTTP-Videostreaming.
* Progressives Videostreaming.

Die folgenden Asset-Typen und -Funktionen werden derzeit nicht unterstützt:

* RTMP-Videostreaming
* UGC-Dienste
* Web-to-Print
* Dynamic Media Classic Info- oder E-Katalogsuche

## Testen des Secure Testing-Dienstes {#testing-the-secure-testing-service}

Sie sollten den Secure Testing-Dienst testen, um sicherzustellen, dass er wie erwartet funktioniert.

Hinweis: Wenn Sie keine IPs unter &quot;Einstellungen&quot;> &quot;Veröffentlichungseinstellungen&quot;> &quot;Image-Server&quot;> &quot;Bilddienst testen&quot;erwähnen
Wenn Sie nur eine IP hinzufügen, kann diese IP die Assets aufrufen und keine andere IP darf die Aufrufe tätigen. Solange in diesem Abschnitt keine IP erwähnt wird, dürfen alle IPs die Assets abrufen und werden angezeigt.

**Vorbereiten des Kontos**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Wenden Sie sich an den technischen Support und fordern Sie die Aktivierung der sicheren Testumgebung für Ihr Konto an.
1. Klicken Sie in Dynamic Media Classic auf **Setup** > **Veröffentlichungseinstellungen** > **Image-Server**.
1. Wählen Sie auf der Seite „Veröffentlichung zum Image-Server“ in der Dropdownliste „Veröffentlichungskontext“ die Option **Image-Server-Test**.
1. Für den Client-Adressfilter klicken Sie auf **„Hinzufügen“**.
1. Wählen Sie das Kontrollkästchen aus, um die Adresse zu aktivieren, und geben Sie dann eine IP-Adresse und eine Netzmaske in die entsprechenden Textfelder ein.

   >[!NOTE]
   >
   >Wenn Sie eine einzelne IP-Adresse und eine Netzmaske hinzufügen, kann diese Adresse Asset-Aufrufe ausführen. Andere von Ihnen hinzugefügte IP-Adressen und Netzmasken dürfen jedoch keine Asset-Aufrufe durchführen. Daher sollten Sie das Kontrollkästchen im obigen Schritt deaktivieren (deaktivieren), um die Möglichkeit zur Angabe einer IP-Adresse und Netzmaske zu deaktivieren. Auf diese Weise können *alle*-IP-Adressen Asset-Aufrufe durchführen, und sie werden alle angezeigt.

1. Führen Sie einen der folgenden Schritte aus:
   * Wiederholen Sie diese beiden Schritte, um weitere IP-Adressen hinzuzufügen.
   * Fahren Sie mit dem nächsten Schritt fort.
1. Klicken Sie unten links auf der Seite „Veröffentlichung zum Image-Server“ auf **Speichern**.
1. Laden Sie die gewünschten Bilder in Ihr Dynamic Media Classic-Konto hoch.

   Siehe [Hochladen von Dateien](uploading-files.md#uploading_files).

1. Vergewissern Sie sich, dass einige der Bilder zur Veröffentlichung markiert und andere nicht markiert sind, und senden Sie dann den Veröffentlichungsauftrag ab.

   Siehe [Veröffentlichen](publishing-files.md#publishing_files).

1. Legen Sie den Namen des Secure Testing-Dienstes fest, indem Sie auf **„Einstellungen“** > **„Anwendungseinstellungen“** > **„Allgemeine Einstellungen“** klicken.
1. Suchen Sie auf der Seite „Allgemeine Programmeinstellungen“ in der Gruppe „Server“ den Namen rechts neben **Servername für den Testveröffentlichungskontext**.

Wenden Sie sich an den Adobe Care, wenn der Servername fehlt oder die URLs zum Server nicht funktionieren.

**Vorbereiten von Website-Variationen**

Sie benötigen zwei Variationen einer Website, die Links zu veröffentlichten und unveröffentlichten Assets enthält:

* Öffentliche Version - Verknüpfen Sie Assets mit Ihrer herkömmlichen Dynamic Media Classic-URL-Syntax.
* Staging-Version - Verknüpfen Sie Assets mit derselben Syntax, jedoch mit dem Namen der Secure Testing-Site.

**Ausführen von Tests**

Führen Sie die folgenden Tests aus:

1. Überprüfen Sie, ob Assets in Ihrem Unternehmensnetzwerk angezeigt werden.

   Innerhalb des Unternehmensnetzwerks, das durch den zuvor definierten IP-Adressbereich identifiziert wird, sollte die Staging-Version der Website alle Bilder anzeigen, ob markiert oder unmarkiert. So können Sie Tests durchführen, ohne versehentlich Bilder vor der Genehmigung der Vorschau oder Produkteinführung verfügbar zu machen.

   Vergewissern Sie sich, dass die öffentliche Version Ihrer Site veröffentlichte Assets wie zuvor mit Dynamic Media Classic anzeigt.

1. Überprüfen Sie, ob außerhalb des Unternehmensnetzwerks die unveröffentlichten Assets (die nicht für die Veröffentlichung markiert wurden) vor dem Zugriff durch Dritte geschützt sind.

   Greifen Sie auf Ihr Netzwerk von außerhalb zu (z. B. von Ihrem Heimcomputer oder über eine 3G-Verbindung). Vergewissern Sie sich so, dass die öffentliche Version der Website alle veröffentlichten Assets, jedoch keine unveröffentlichten Inhalte anzeigt.

   Die Staging-Version darf kein Asset anzeigen, weil Sie mit einer nicht zugelassenen IP-Adresse auf den Secure Testing-Dienst zugreifen.
