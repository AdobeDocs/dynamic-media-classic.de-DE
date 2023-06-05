---
title: Adobe Dynamic Media Classic-Programmübersicht
description: Eine Übersicht über das Adobe Dynamic Media Classic-Programm und den gesamten Workflow-Prozess.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 17%

---

# Adobe Dynamic Media Classic-Programmübersicht{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic ist eine integrierte Rich-Media-Management-, Publishing- und Serving-Umgebung. Rich-Media-Daten können für alle Marketing- und Vertriebskanäle verwendet werden, einschließlich Internet, Druckmaterial, E-Mail-Kampagnen, Web-Portale, Desktop-Computer und sonstige Geräte.

Siehe auch [Plattformübersicht](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) Schulungsvideo.

## Workflows {#workflow-process}

Die wichtigsten Schritte des Adobe Dynamic Media Classic-Workflows sind:

* **Hochladen und Verwalten von Assets** - Laden Sie Ihre Medien-Assets in Adobe Dynamic Media Classic hoch. In diesem System können Sie Assets organisieren und durchsuchen sowie nach bestimmten Assets suchen. Außerdem können Sie Metadaten auf Assets anwenden.

* **Rich Media erstellen** - Erstellen Sie unterschiedliche Konfigurationen Ihrer Assets wie E-Kataloge, Bildsets, Rotationssets, Mustersets, gemischte Mediensets, einfache Vorlagen und FXG-Vorlagen.

* **Veröffentlichen und Verwalten** - Veröffentlichen Sie Assets im SaaS-Netzwerk von Adobe Dynamic Media Classic. Überwachen Sie den Status von Assets, wenn sie veröffentlicht werden. Verwalten Sie Benutzerrechte und verwalten Sie die Sicherheit.

* **Serve** - Bereitstellung von Medien vom Adobe Dynamic Media Classic SaaS-Netzwerk zu Webseiten, Anwendungen und Mobilgeräten; die Medien sind leistungsoptimiert und werden mit CDN-Zwischenspeicherung bereitgestellt. Adobe Dynamic Media Classic stellt Ihnen eine URL für jedes Asset bereit. Sobald Sie das Asset veröffentlichen, wird die URL aktiv.

![Der Adobe Dynamic Media Classic-Workflow-Prozess](/help/using/assets/gs_workflow.png)

## Einzelne Primärbilder und einzelne URL-Aufrufe {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic unterscheidet sich grundlegend von anderen Systemen, da Sie mit Adobe Dynamic Media Classic Medien dynamisch aus einzelnen primären Assets und URL-Aufrufen bereitstellen können.

Die URL-Zeichenfolgen, die Sie mit Adobe Dynamic Media Classic generieren, enthalten Anweisungen, die dem Server mitteilen, wie das Asset bei der Bereitstellung angezeigt werden soll. Beispielsweise kann dasselbe Primärbild in unterschiedlichen Größen, Formaten, Gewichtungen, Farben und Zoom-Ansichten bereitgestellt werden. Beim Erstellen und Veröffentlichen von Medien-Assets mit Adobe Dynamic Media Classic konfigurieren Sie die Effekte visuell. Erstellen Sie dabei die URL-Aufrufe, die dem Server korrekt mitteilen, wie das primäre Asset für Anwendungen bereitgestellt werden soll.

![Adobe Dynamic Media Classic kann dasselbe Primärbild für verschiedene Medien in unterschiedlichen Größen und Formaten bereitstellen.](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic stellt sicher, dass unabhängig von Größe und Bandbreite für jeden Bildschirm konsistente, qualitativ hochwertige Erlebnisse bereitgestellt werden.*

## Inhalts-Caching {#content-caching}

Die von Adobe Dynamic Media Classic dynamisch generierten Bilder sind Cache-günstig. Normalerweise sind es JPEG-Bilder mit eindeutigen URL-Aufrufen, die sie identifizieren. Die Bilder werden über ein CDN-System (Content Delivery Network) gesendet, ein Netzwerk von Servern, die über das Internet miteinander verbunden sind und dazu dienen, Inhalte schneller zu übermitteln. Die Bilder werden zunächst von weltweit verbreiteten Servern verteilt und dann an einzelne Computer gesendet. Wenn Sie einen Caching-Mechanismus mit einem beliebigen CDN-Anbieter implementieren, ändern Sie einfach den Servernamen so, dass er auf den CDN-fähigen Dynamic Media-Bildserver verweist. Alle Adobe Dynamic Media Classic-Editionen umfassen das gebündelte CDN-Caching.
