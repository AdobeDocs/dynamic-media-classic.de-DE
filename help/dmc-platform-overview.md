---
title: Adobe Dynamic Media Classic - Programmübersicht
description: Eine Übersicht über das Dynamic Media Classic-Programm und den Workflow-Prozess.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: 47845c30311fb9afb3fffb8502b6e7c534e4bfdb
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 30%

---

# Adobe Dynamic Media Classic - Programmübersicht{#adobe-scene-platform-overview}

Dynamic Media Classic ist eine integrierte Rich-Media-Management-, Publishing- und Serving-Umgebung. Rich-Media-Daten können für alle Marketing- und Vertriebskanäle verwendet werden, einschließlich Internet, Druckmaterial, E-Mail-Kampagnen, Web-Portale, Desktop-Computer und sonstige Geräte.

## Workflows {#workflow-process}

Die wichtigsten Workflow-Schritte von Dynamic Media Classic sind:

* **Hochladen und Verwalten von Assets**  - Laden Sie Ihre Medien-Assets in Dynamic Media Classic hoch. In diesem System können Sie Assets organisieren und durchsuchen sowie nach bestimmten Assets suchen. Außerdem können Sie Metadaten auf Assets anwenden.

* **Rich Media erstellen**  - Erstellen Sie verschiedene Konfigurationen Ihrer Assets, z. B. E-Kataloge, Bildsets, Rotationssets, Mustersets, gemischte Mediensets, einfache Vorlagen und FXG-Vorlagen.

* **Veröffentlichen und verwalten**  - Veröffentlichen Sie Assets im SaaS-Netzwerk von Dynamic Media Classic und überwachen Sie den Status von Assets bei der Veröffentlichung, verwalten Sie Benutzerrechte und gewährleisten Sie Sicherheit.

* **Bereitstellung**  - Bereitstellen von Medien aus dem Dynamic Media Classic SaaS-Netzwerk für Webseiten, Anwendungen und Mobilgeräte; die Medien sind leistungsoptimiert und werden mit CDN-Zwischenspeicherung bereitgestellt. Dynamic Media Classic bietet für jedes Asset eine URL. Sobald Sie das Asset veröffentlichen, wird die URL aktiv.

![Der Workflow-Prozess von Dynamic Media Classic](/help/assets/gs_workflow.png)

## Einzelne Masterbilder und einzelne URL-Aufrufe {#single-master-images-and-single-url-calls}

Dynamic Media Classic unterscheidet sich grundlegend von anderen Systemen, da Sie mit Dynamic Media Classic Medien dynamisch aus einzelnen Übergeordneten Assets und URL-Aufrufen bereitstellen können.

Die URL-Zeichenfolgen, die Sie mit Dynamic Media Classic generieren, enthalten Anweisungen, die dem Server mitteilen, wie das Asset bei der Bereitstellung angezeigt werden soll. Ein und dasselbe Masterbild kann beispielsweise mit unterschiedlichen Größen, Formaten, Stärken, Farben und Zoomansichten gesendet werden. Beim Erstellen und Veröffentlichen von Medien-Assets mit Dynamic Media Classic konfigurieren Sie die Effekte visuell. Auf diese Weise werden die URL-Aufrufe erstellt, mit denen dem Server korrekt mitgeteilt wird, wie das Master-Asset in Anwendungen präsentiert werden soll.

![Dynamic Media Classic kann dasselbe Übergeordnete Bild für verschiedene Medien in unterschiedlichen Größen und Formaten bereitstellen.](/help/assets/gs_dynamic_publishing.png)
*Dynamic Media Classic stellt sicher, dass konsistente, hochwertige Erlebnisse unabhängig von Größe und Bandbreite für jeden Bildschirm bereitgestellt werden.*

## Inhalts-Caching {#content-caching}

Die von Dynamic Media Classic dynamisch generierten Bilder sind zwischenspeicherfreundlich. normalerweise sind es JPEG-Bilder mit eindeutigen URL-Aufrufen, die sie identifizieren. Die Bilder werden über ein CDN-System (Content Delivery Network) gesendet, ein Netzwerk von Servern, die über das Internet miteinander verbunden sind und dazu dienen, Inhalte schneller zu übermitteln. Die Bilder werden zunächst von weltweit verbreiteten Servern verteilt und dann an einzelne Computer gesendet. Wenn Sie einen Caching-Mechanismus mit einem beliebigen CDN-Anbieter implementieren, ändern Sie einfach den Servernamen so, dass er auf den CDN-fähigen Dynamic Media-Bildserver verweist. Alle Dynamic Media Classic-Editionen umfassen das gebündelte CDN-Caching.
