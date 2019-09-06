---
title: Testen von Assets vor dem Veröffentlichen
seo-title: Testen von Assets vor dem Veröffentlichen
description: 'null'
seo-description: Erfahren Sie, wie Sie Assets testen, bevor Sie sie veröffentlichen.
uuid: 5 e 8 f 3 bec -6 cf 1-408 e -8 ea 1-aebde 0012 a 70
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/upload_ and_ publish_ assets
discoiquuid: 52 fadf 99-7 d 11-46 f 7-8483-a 9 f 87 ffc 2 f 67
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Testen von Assets vor dem Veröffentlichen {#testing-assets-before-making-them-public}

Mit Secure Testing können Sie eine sichere Testumgebung definieren und eine robuste B2B-Lösung erstellen, die auf einem konfigurierbaren Satz aus IP-Adressen und -Bereichen basiert. Mit dieser Funktion können Sie Ihre Implementierungen für dynamische Medien mit der Architektur Ihrer Content-Management- und Commerce-Plattformen vergleichen.

Mit Secure Testing können Sie eine Vorabversion (Staging) der Website mit unveröffentlichtem Inhalt in der Vorschau anzeigen.

Möglicherweise bevorzugen Sie aus folgenden Gründen das Erstellen einer Staging-Umgebung, anstatt Assets öffentlich verfügbar zu machen:

* Vorschau der Websites vor der Veröffentlichung (Staging-Website).
* Bereitstellen von Assets, deren Zugriff eingeschränkt sein soll, wie E-Kataloge, die Preise in einer B2B-Web-Anwendung anzeigen.
* Verwenden von Assets hinter einer Firewall als Teil des Produktinformations-Managementsystems, der Kundenservice-Anwendung, Online-Kursen usw.

>[!NOTE]
>
>Secure Testing beeinträchtigt nicht den Zugriff auf das Scene7 Publishing System. Die SPS-Sicherheit bleibt erhalten und erfordert die üblichen Zugangsdaten für SPS und entsprechende Webdienste.

## Funktionsweise von Secure Testing {#how-secure-testing-works}

Die meisten Unternehmen haben eine Firewall für den Internetzugriff. Der Zugriff auf das Internet ist damit auf bestimmten Routen möglich und normalerweise auf bestimmte öffentliche IP-Adressen beschränkt.

Über Ihr Unternehmensnetzwerk können Sie Ihre öffentliche IP-Adresse mithilfe von Websites wie https://whatismyip.com herausfinden oder diese Informationen von Ihrer IT-Abteilung anfordern.

Mit Secure Testing erstellt Dynamic Media Classic einen dedizierten Image-Server für Staging-Umgebungen oder interne Anwendungen. Mit jeder Anforderung bei diesem Server wird die Original-IP-Adresse überprüft. Wenn die eingehende Anforderung nicht auf der genehmigten Liste der IP-Adressen steht, wird eine Fehlerantwort zurückgesendet. Der dynamische Media-Administrator von Dynamic Media konfiguriert die genehmigte Liste von IP-Adressen für die Secure Testing-Umgebung ihres Unternehmens.

Da der Speicherort der ursprünglichen Anforderung bestätigt werden muss, wird der Verkehr des Secure Testing-Dienstes nicht über ein Inhaltsverteilungs-Netzwerk wie den Traffic des öffentlichen dynamischen Medien-Servers weitergeleitet. Anforderungen an den Secure Testing-Dienst können eine etwas höhere Latenz im Vergleich zu den öffentlichen dynamischen Medienservern aufweisen.

Unveröffentlichte Assets sind sofort über den Secure Testing-Dienst verfügbar und müssen nicht erst veröffentlicht werden. Dies ermöglicht es Ihnen, eine Vorschau auszuführen, bevor Assets auf dem für die Öffentlichkeit zugänglichen Image-Server veröffentlicht werden.

***Hinweis**: Secure Testing-Dienste nutzen den Katalog-Server, der mit einem internen Veröffentlichungskontext konfiguriert ist. Wenn Ihr Unternehmen daher für die Veröffentlichung von Secure Testing konfiguriert wurde, müssen Sie beachten, dass sämtliche hochgeladenen Assets im Scene7 Publishing System sofort in den Secure Testing-Diensten verfügbar sind. Dies gilt unabhängig davon, ob die Assets für das Hochladen oder Veröffentlichen markiert wurden.*

Secure Testing-Dienste unterstützen derzeit die folgenden Asset-Typen und -funktionen:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Bilder.
* Vignetten (Render-Server-Anforderungen).
* Render-Server-Anforderungen (unterstützt, müssen jedoch explizit vom Kunden angefordert werden).
* Sätze, einschließlich Bildsätzen, E-Katalog, Rendersets und Mediensets.
* Standard Dynamic Media Classic Rich Media Viewer.
* Dynamic Media Classic ondemand JSP-Seiten.
* Statische Inhalte wie PDF-Dateien und progressiv bereitgestellte Videos.
* HTTP-Videostreaming.
* Progressives Videostreaming.

Die folgenden Asset-Typen und -Funktionen werden derzeit nicht unterstützt:

* RTMP-Videostreaming
* UGC-Dienste
* Web-to-Print
* Dynamic Media Classic Info oder E-Katalog-Suche

## Testen des Secure Testing-Dienstes {#testing-the-secure-testing-service}

Sie sollten den Secure Testing-Dienst testen, um sicherzustellen, dass er wie erwartet funktioniert.

**Vorbereiten des Kontos**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Wenden Sie sich an den technischen Support und fordern Sie die Aktivierung der sicheren Testumgebung für Ihr Konto an.
1. Klicken Sie im Scene7 Publishing System auf **„Einstellungen“** &gt; **„Veröffentlichungseinstellungen“** &gt; **„Image-Server“**.
1. Wählen Sie auf der Seite „Veröffentlichung zum Image-Server“ in der Dropdownliste „Veröffentlichungskontext“ die Option **Image-Server-Test**.
1. Für den Client-Adressfilter klicken Sie auf **„Hinzufügen“**.
1. Wählen Sie das Kontrollkästchen aus, um die Adresse zu aktivieren, und geben Sie dann eine IP-Adresse und eine Netzmaske in die entsprechenden Textfelder ein.
1. Wiederholen Sie diese beiden Schritte, um weitere IP-Adressen hinzuzufügen. Fahren Sie andernfalls mit dem nächsten Schritt fort.
1. Klicken Sie unten links auf der Seite „Veröffentlichung zum Image-Server“ auf **Speichern**.
1. Laden Sie die gewünschten Bilder zu Ihrem Scene7 Publishing System-Konto hoch.

   Siehe [Hochladen von Dateien](uploading-files.md#uploading_files).

1. Vergewissern Sie sich, dass einige der Bilder zur Veröffentlichung markiert und andere nicht markiert sind, und senden Sie dann den Veröffentlichungsauftrag ab.

   Siehe [Veröffentlichen](publishing-files.md#publishing_files).

1. Legen Sie den Namen des Secure Testing-Dienstes fest, indem Sie auf **„Einstellungen“** &gt; **„Anwendungseinstellungen“** &gt; **„Allgemeine Einstellungen“** klicken.
1. Suchen Sie auf der Seite „Allgemeine Programmeinstellungen“ in der Gruppe „Server“ den Namen rechts neben **Servername für den Testveröffentlichungskontext**.

Wenden Sie sich an den technischen Support, wenn der Servername fehlt oder die URLs zum Server nicht funktionieren.

**Vorbereiten von Website-Variationen**

Sie benötigen zwei Variationen einer Website, die Links zu veröffentlichten und unveröffentlichten Assets enthält:

* Öffentliche Version: Verknüpfen von Assets mit Ihrer traditionellen Dynamic Media Classic-URL
* Staging-Version: Verknüpfen Sie Assets mit der gleichen Syntax, jedoch mit dem Namen der Secure Testing Site

**Ausführen von Tests**

Führen Sie die folgenden Tests aus:

1. Überprüfen Sie, ob Assets in Ihrem Unternehmensnetzwerk angezeigt werden.

   Innerhalb des Unternehmensnetzwerks, das durch den zuvor definierten IP-Adressbereich identifiziert wird, sollte die Staging-Version der Website alle Bilder anzeigen, ob markiert oder unmarkiert. So können Sie Tests durchführen, ohne versehentlich Bilder vor der Genehmigung der Vorschau oder Produkteinführung verfügbar zu machen.

   Überprüfen Sie, ob die öffentliche Version Ihrer Site veröffentlichte Assets wie zuvor mit Dynamic Media Classic gezeigt hat.

1. Überprüfen Sie, ob außerhalb des Unternehmensnetzwerks die unveröffentlichten Assets (die nicht für die Veröffentlichung markiert wurden) vor dem Zugriff durch Dritte geschützt sind.

   Greifen Sie auf Ihr Netzwerk von außerhalb zu (z. B. von Ihrem Heimcomputer oder über eine 3G-Verbindung). Vergewissern Sie sich so, dass die öffentliche Version der Website alle veröffentlichten Assets, jedoch keine unveröffentlichten Inhalte anzeigt.

   Die Staging-Version darf kein Asset anzeigen, weil Sie mit einer nicht zugelassenen IP-Adresse auf den Secure Testing-Dienst zugreifen.

