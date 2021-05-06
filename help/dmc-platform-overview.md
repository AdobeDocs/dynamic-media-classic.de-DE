---
title: Übersicht über Adobe Dynamic Media Classic Programm
description: Eine Übersicht über das Programm und den Workflow von Dynamic Media Classic.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
translation-type: tm+mt
source-git-commit: eb37440a2917094aae8f32e9337b4c187ec6c1c2
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 30%

---

# Übersicht über das Programm der Adobe Dynamic Media Classic{#adobe-scene-platform-overview}

Dynamic Media Classic ist eine integrierte Rich Media Management-, Publishing- und Serving-Umgebung. Rich-Media-Daten können für alle Marketing- und Vertriebskanäle verwendet werden, einschließlich Internet, Druckmaterial, E-Mail-Kampagnen, Web-Portale, Desktop-Computer und sonstige Geräte.

## Workflows  {#workflow-process}

Die wichtigsten Schritte des Dynamic Media Classic-Workflows sind:

* **Hochladen und Verwalten Ihrer Assets**  - Laden Sie Ihre Medienelemente in Dynamic Media Classic hoch. In diesem System können Sie Assets organisieren und durchsuchen sowie nach bestimmten Assets suchen. Außerdem können Sie Metadaten auf Assets anwenden.

* **Rich-Media** -Erstellung - Erstellen Sie verschiedene Konfigurationen Ihrer Assets, z. B. E-Kataloge, Bildsätze, Rotationssets, Mustersets, gemischte Mediensets, einfache Vorlagen und FXG-Vorlagen.

* **Veröffentlichen und Verwalten** : Veröffentlichen Sie Assets im Dynamic Media Classic SaaS-Netzwerk, überwachen Sie den Status der Assets, wenn sie veröffentlicht werden, verwalten Sie Benutzerrechte und verwalten Sie die Sicherheit.

* **Bereitstellung**  von Medien aus dem Dynamic Media Classic SaaS-Netzwerk für Webseiten, Anwendungen und Mobilgeräte; die Medien sind leistungsoptimiert und werden mit CDN-Caching bereitgestellt. Dynamic Media Classic stellt eine URL für jedes Asset bereit. Sobald Sie das Asset veröffentlichen, wird die URL aktiv.

![Der Arbeitsablaufprozess von Dynamic Media Classic](/help/assets/gs_workflow.png)

## Einzelne Masterbilder und einzelne URL-Aufrufe {#single-master-images-and-single-url-calls}

Dynamic Media Classic unterscheidet sich grundlegend von anderen Systemen, da Sie mit Dynamic Media Classic Mediendateien dynamisch aus einzelnen Übergeordnet-Assets und URL-Aufrufen bereitstellen können.

Die URL-Zeichenfolgen, die Sie mit Dynamic Media Classic generieren, enthalten Anweisungen, die dem Server mitteilen, wie das Asset angezeigt wird, wenn es bereitgestellt wird. Ein und dasselbe Masterbild kann beispielsweise mit unterschiedlichen Größen, Formaten, Stärken, Farben und Zoomansichten gesendet werden. Beim Erstellen und Veröffentlichen von Medienelementen mit Dynamic Media Classic konfigurieren Sie die Effekte visuell. Auf diese Weise werden die URL-Aufrufe erstellt, mit denen dem Server korrekt mitgeteilt wird, wie das Master-Asset in Anwendungen präsentiert werden soll.

![Dynamic Media Classic kann das gleiche Übergeordnet-Bild für verschiedene Medien in unterschiedlichen Größen und Formaten bereitstellen.](/help/assets/gs_dynamic_publishing.png)
*Dynamic Media Classic stellt sicher, dass konsistente, qualitativ hochwertige Erlebnisse unabhängig von Größe und Bandbreite für jeden Bildschirm bereitgestellt werden.*

## Inhalts-Caching {#content-caching}

Die dynamisch von Dynamic Media Classic erstellten Bilder sind Cache-freundlich. Normalerweise handelt es sich dabei um JPEG-Bilder mit eindeutigen URL-Aufrufen, die sie identifizieren. Die Bilder werden über ein CDN-System (Content Delivery Network) gesendet, ein Netzwerk von Servern, die über das Internet miteinander verbunden sind und dazu dienen, Inhalte schneller zu übermitteln. Die Bilder werden zunächst von weltweit verbreiteten Servern verteilt und dann an einzelne Computer gesendet. Bei der Implementierung eines Caching-Mechanismus mit einem beliebigen CDN-Anbieter ändern Sie einfach den Servernamen so, dass er auf den CDN-fähigen Dynamic Media Image Server verweist. Alle Dynamic Media Classic-Editionen enthalten CDN-Caching im Paket.
