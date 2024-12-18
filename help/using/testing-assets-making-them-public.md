---
title: Testen von Assets vor der Veröffentlichung
description: Erfahren Sie, wie Sie Assets in Adobe Dynamic Media Classic testen können, bevor Sie sie veröffentlichen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
topic: Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 19%

---

# Testen von Assets vor der Veröffentlichung {#testing-assets-before-making-them-public}

Mit Secure Testing können Sie eine sichere Testumgebung definieren und eine robuste B2B-Lösung erstellen, die auf einem konfigurierbaren Satz von IP-Adressen und -Bereichen basiert. Mit dieser Funktion können Sie Ihre Adobe Dynamic Media Classic-Bereitstellungen mit der Architektur Ihres Content-Management- und Geschäftssystems abgleichen.

Mit Secure Testing können Sie eine Vorabversion (Staging) der Website mit unveröffentlichtem Inhalt in der Vorschau anzeigen.

Aus den folgenden Gründen sollten Sie bei Bedarf eine Staging-Umgebung erstellen, anstatt Assets öffentlich verfügbar zu machen:

* Vorschau der Websites vor der Veröffentlichung (Staging-Website).
* Bereitstellen von Assets, die eingeschränkten Zugriff erfordern, wie z. B. E-Kataloge, die Preise in einer B2B-Web-Anwendung anzeigen.
* Verwenden von Assets hinter einer Firewall als Teil eines Produktinformations-Management-Systems, einer Kundendienstanwendung, einer Schulungs-Website usw.

>[!NOTE]
>
>Secure Testing hat keine Auswirkungen auf den Zugriff auf Adobe Dynamic Media Classic. Die Adobe Dynamic Media Classic-Sicherheit bleibt konsistent und erfordert die üblichen Anmeldeinformationen für den Zugriff auf Adobe Dynamic Media Classic und zugehörige Web-Services.

## Funktionsweise von Secure Testing {#how-secure-testing-works}

Die meisten Unternehmen haben eine Firewall für den Internetzugriff. Der Zugriff auf das Internet ist damit auf bestimmten Routen möglich und normalerweise auf bestimmte öffentliche IP-Adressen beschränkt.

Über Ihr Unternehmensnetzwerk können Sie mithilfe von Websites wie [https://www.whatismyip.com](https://www.whatismyip.com/) Ihre öffentliche IP-Adresse ermitteln oder diese Informationen bei Ihrer IT-Organisation anfordern.

Mit Secure Testing richtet Adobe Dynamic Media Classic einen dedizierten Image-Server für Staging-Umgebungen oder interne Anwendungen ein. Mit jeder Anforderung bei diesem Server wird die Original-IP-Adresse überprüft. Wenn die eingehende Anfrage nicht in der Liste genehmigter IP-Adressen enthalten ist, wird eine Fehlerantwort zurückgegeben. Der Adobe Dynamic Media Classic-Unternehmensadministrator konfiguriert die Liste genehmigter IP-Adressen für die Secure Testing-Umgebung seines Unternehmens.

Da der Speicherort der ursprünglichen Anfrage bestätigt werden muss, wird der Traffic des Secure Testing-Services nicht über ein Inhaltsverteilungsnetzwerk geleitet, wie der öffentliche Traffic des Dynamic Media-Bildservers. Anfragen an den Secure Testing-Service weisen eine etwas höhere Latenz auf als die öffentlichen Dynamic Media-Bildserver.

Unveröffentlichte Assets sind sofort über den Secure Testing-Dienst verfügbar und müssen nicht erst veröffentlicht werden. Auf diese Weise können Sie eine Vorschau ausführen, bevor Assets auf ihrem öffentlichen Bild-Server veröffentlicht werden.

>[!NOTE]
>
>Secure Testing-Services verwenden den Katalog-Server, der mit einem internen Veröffentlichungskontext konfiguriert ist. Wenn Ihr Unternehmen für die Veröffentlichung in Secure Testing konfiguriert ist, sind daher hochgeladene Assets in Adobe Dynamic Media Classic sofort in den Secure Testing-Services verfügbar. Diese Funktionalität gilt unabhängig davon, ob die Assets beim Hochladen zur Veröffentlichung markiert sind.

Secure Testing-Services unterstützen derzeit die folgenden Asset-Typen und -Funktionen:

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved "Render Server requests" from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* Bilder.
* Vignetten (Render-Server-Anforderungen).
* Rendering-Server-Anfragen (werden unterstützt, müssen aber vom Kunden explizit angefordert werden).
* Sätze, einschließlich Bildsätzen, E-Katalog, Rendersets und Mediensets.
* Standard-Adobe Dynamic Media Classic-Rich-Media-Viewer.
* Adobe Dynamic Media Classic OnDemand JSP-Seiten.
* Statische Inhalte wie PDF-Dateien und progressiv bereitgestellte Videos.
* HTTP-Videostreaming.
* Progressives Videostreaming.

Die folgenden Asset-Typen und -Funktionen werden derzeit nicht unterstützt:

* Adobe Dynamic Media Classic-Info- oder E-Katalog-Suche
* RTMP-Videostreaming
* Web-to-Print
* UGC-Services (benutzergenerierte Inhalte)

>[!IMPORTANT]
>
>Die Unterstützung für neue oder vorhandene UGC-Vektorbild-Assets in Adobe Dynamic Media Classic endete am 30. September 2021.

## Testen des Secure Testing-Service {#testing-the-secure-testing-service}

Testen Sie den Secure Testing-Service, damit Sie sicherstellen können, dass er erwartungsgemäß funktioniert.

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]***: If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### Vorbereiten des Kontos

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under "Prepare your account" 9/10/2012</p>

 -->

1. Wenden Sie sich an die Kundenunterstützung von Adobe und bitten Sie sie, Secure Testing für Ihr Konto zu aktivieren.
1. Wechseln Sie in Adobe Dynamic Media Classic in der globalen Navigationsleiste zu **[!UICONTROL Setup]** > **[!UICONTROL Publish-Setup]** > **[!UICONTROL Image-Server]**.
1. Wählen Sie auf der Seite Image-Server-Publish in der Dropdown-Liste **[!UICONTROL `Publish Context`]** die Option **[!UICONTROL Image-Serving testen]** aus.
1. Wählen Sie für den Client-Adressfilter die Option **[!UICONTROL Hinzufügen]**.
1. Aktivieren Sie das Kontrollkästchen, sodass die Adresse aktiviert ist, und geben Sie dann eine IP-Adresse und eine Netzmaske in die entsprechenden Textfelder ein.

   >[!NOTE]
   >
   >Wenn Sie eine einzelne IP-Adresse und Netzmaske hinzufügen, kann diese Adresse Asset-Aufrufe durchführen. Andere IP-Adressen und Netzmasken, die Sie hinzufügen, dürfen jedoch keine Asset-Aufrufe ausführen. Deaktivieren Sie daher ggf. das Kontrollkästchen im obigen Schritt, um die Möglichkeit zur Angabe einer IP-Adresse und einer Netzmaske zu deaktivieren. Dadurch können *alle* IP-Adressen Asset-Aufrufe durchführen, und sie werden alle angezeigt.

1. Führen Sie einen der folgenden Schritte aus:
   * Wiederholen Sie die vorherigen beiden Schritte, wenn Sie weitere IP-Adressen hinzufügen müssen.
   * Fahren Sie mit dem nächsten Schritt fort.
1. Klicken Sie unten links auf der Seite „Image-Server-Publish&quot; auf **[!UICONTROL Speichern]**
1. Laden Sie die gewünschten Bilder in Ihr Adobe Dynamic Media Classic-Konto hoch.

   Siehe [Dateien hochladen](uploading-files.md#uploading_files).

1. Stellen Sie sicher, dass einige der Bilder zur Veröffentlichung markiert und andere nicht markiert sind, und senden Sie dann den Veröffentlichungsauftrag.

   Siehe [Publish-](publishing-files.md#publishing_files).

1. Bestimmen Sie den Namen Ihres Secure Testing-Services, indem Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Einstellungen]** wechseln.
1. Suchen Sie auf der Seite „Allgemeine Programmeinstellungen“ in der Gruppe „Server“ den Namen rechts neben **[!UICONTROL Servername für den Testveröffentlichungskontext]**.

Wenden Sie sich an den Adobe-Support, wenn der Servername fehlt oder die URLs zum Server nicht funktionieren.

### Vorbereiten von Website-Variationen

Sie benötigen zwei Variationen einer Website, die Links zu veröffentlichten und unveröffentlichten Assets enthält:

* Öffentliche Version: Verknüpfen Sie Assets mithilfe Ihrer herkömmlichen Adobe Dynamic Media Classic-URL-Syntax.
* Staging-Version: Verknüpfen Sie Assets mithilfe derselben Syntax, aber mit dem Namen der Secure Testing-Site.

### Ausführen von Tests

Führen Sie die folgenden Tests aus:

1. Überprüfen Sie, ob Assets in Ihrem Unternehmensnetzwerk angezeigt werden.

   Innerhalb des Unternehmensnetzwerks, das durch den zuvor definierten IP-Adressbereich identifiziert wird, zeigt die Staging-Version der Website alle Bilder an, unabhängig davon, ob sie zur Veröffentlichung markiert sind oder nicht. Daher können Sie Tests durchführen, ohne Bilder versehentlich vor der Genehmigung der Vorschau oder dem Produktstart verfügbar zu machen.

   Vergewissern Sie sich, dass die öffentliche Version Ihrer Site veröffentlichte Assets anzeigt, wie Sie es bereits von Adobe Dynamic Media Classic gewohnt sind.

1. Stellen Sie von außerhalb Ihres Unternehmensnetzwerks sicher, dass nicht veröffentlichte (d. h. nicht zur Veröffentlichung markierte) Assets vor dem Zugriff Dritter geschützt sind.

   Greifen Sie von außerhalb auf Ihr Netzwerk zu (z. B. von Ihrem privaten Computer oder über eine 3G-Verbindung) und überprüfen Sie, ob in der öffentlichen Version der Site alle veröffentlichten Assets, aber keine unveröffentlichten Inhalte angezeigt werden.

   Die Staging-Version darf kein Asset anzeigen, weil Sie mit einer nicht zugelassenen IP-Adresse auf den Secure Testing-Dienst zugreifen.
