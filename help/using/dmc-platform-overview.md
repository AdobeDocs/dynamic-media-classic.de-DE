---
title: Übersicht über das Adobe Dynamic Media Classic-Programm
description: Ein Überblick über das Adobe Dynamic Media Classic-Programm und den gesamten Workflow-Prozess.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
topic: Administration
level: Beginner
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 12%

---

# Übersicht über das Adobe Dynamic Media Classic-Programm{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic ist eine integrierte Umgebung für Rich-Media-Management, Veröffentlichung und Bereitstellung. Rich-Media können an alle Marketing- und Verkaufskanäle gesendet werden. Zu diesen Kanälen gehören das Internet, Druckmaterialien, E-Mail-Kampagnen, Web-Portale, Desktops und Geräte.

Siehe auch [Platform - Übersicht](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) Schulungsvideo.

## Workflows {#workflow-process}

Die wichtigsten Adobe Dynamic Media Classic-Workflow-Schritte sind:

* **Assets hochladen und verwalten**: Laden Sie Ihre Medien-Assets in Adobe Dynamic Media Classic hoch. In diesem System können Sie Assets organisieren und durchsuchen sowie nach bestimmten Assets suchen. Sie können auch Metadaten auf Assets anwenden.

* **Rich-Media erstellen** Erstellen Sie verschiedene Konfigurationen Ihrer Assets, z. B. E-Kataloge, Bildsets, Rotationssets, Mustersets, Sets mit gemischten Medien, einfache Vorlagen und FXG-Vorlagen.

* **Publish und Verwalten**: Publish-Assets für das Adobe Dynamic Media Classic SaaS-Netzwerk. Überwachen des Status von Assets bei ihrer Veröffentlichung. Verwalten Sie Benutzerrechte und gewährleisten Sie die Sicherheit.

* **Serve**: Stellen Sie Medien aus dem Adobe Dynamic Media Classic SaaS-Netzwerk für Web-Seiten, Anwendungen und Mobilgeräte bereit. Die Medien sind leistungsoptimiert und werden mit CDN-Caching bereitgestellt. Adobe Dynamic Media Classic stellt für jedes Asset eine URL bereit. Sobald Sie das Asset veröffentlichen, wird die URL aktiv.

![Der Adobe Dynamic Media Classic-Workflow-Prozess](/help/using/assets/gs_workflow.png)

## Einzelne primäre Bilder und einzelne URL-Aufrufe {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic unterscheidet sich grundlegend von anderen Systemen, da Sie mit Adobe Dynamic Media Classic Medien dynamisch aus einzelnen primären Assets und URL-Aufrufen bereitstellen können.

Die mit Adobe Dynamic Media Classic generierten URL-Zeichenfolgen enthalten Anweisungen, die dem Server mitteilen, wie das Asset bei der Bereitstellung angezeigt werden soll. Beispielsweise kann dasselbe Primärbild in verschiedenen Größen, Formaten, Gewichtungen, Farben und Zoom-Ansichten bereitgestellt werden. Beim Erstellen und Veröffentlichen von Medien-Assets mit Adobe Dynamic Media Classic können Sie die Auswirkungen visuell konfigurieren. Dabei erstellen Sie die URL-Aufrufe, die dem Server korrekt mitteilen, wie das primäre Asset Anwendungen präsentiert wird.

![Adobe Dynamic Media Classic kann dasselbe Primärbild für verschiedene Medien in unterschiedlichen Größen und Formaten bereitstellen.](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic stellt sicher, dass unabhängig von Größe und Bandbreite auf jedem Bildschirm konsistente, hochwertige Erlebnisse bereitgestellt werden.*

## Inhalts-Caching {#content-caching}

Die Bilder, die Adobe Dynamic Media Classic dynamisch generiert, sind für den Cache geeignet. Normalerweise werden dabei Bilder mit eindeutigen URL-Aufrufen JPEG, die sie identifizieren. Die Bilder werden über ein CDN-System (Content Delivery Network) gesendet, ein Netzwerk von Servern, die über das Internet miteinander verbunden sind und dazu dienen, Inhalte schneller zu übermitteln. Die Bilder werden zunächst von weltweit verbreiteten Servern verteilt und dann an einzelne Computer gesendet. Wenn Sie einen Caching-Mechanismus mit einem CDN-Anbieter implementieren, ändern Sie einfach den Servernamen, sodass er auf den CDN-fähigen Dynamic Media-Bildserver verweist. Alle Adobe Dynamic Media Classic-Editionen enthalten gebündeltes CDN-Caching.
