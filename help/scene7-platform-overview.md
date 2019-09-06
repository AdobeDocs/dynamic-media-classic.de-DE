---
title: Übersicht über die Adobe Dynamic Media Classic-Plattform
seo-title: Übersicht über die Adobe Dynamic Media Classic-Plattform
description: 'null'
seo-description: Eine Übersicht über die Plattform und den Workflow für dynamische Medien.
uuid: e 7 d 3 bfb 3-1 cfe -43 ea-b 662-aae 3 b 3928 c 71
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/getting_ started
discoiquuid: 2 b 134 cfa -7 f 46-4 f 5 f -959 e-b 30 aae 610 bb 9
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Übersicht über die Adobe Dynamic Media Classic-Plattform{#adobe-scene-platform-overview}

Dynamic Media Classic ist eine integrierte Umgebung für Rich Media-Verwaltung, Veröffentlichung und Wartung. Rich-Media-Daten können für alle Marketing- und Vertriebskanäle verwendet werden, einschließlich Internet, Druckmaterial, E-Mail-Kampagnen, Web-Portale, Desktop-Computer und sonstige Geräte.

## Workflows {#workflow-process}

Die wichtigsten Schritte für dynamische Medien Classic sind:

**Hochladen und Verwalten Ihrer Assets** Laden Sie Ihre Medienassets in SPS hoch. In diesem System können Sie Assets organisieren und durchsuchen sowie nach bestimmten Assets suchen. Außerdem können Sie Metadaten auf Assets anwenden. Wenn Sie die Adobe Scene7 Publishing System-Desktop-Anwendung installieren, können Sie Dateien und Ordner von Ihrem Desktop in einen Zielordner ziehen und so in diesen Ordner hochladen.

**Rich-Media-Erstellung** Erstellen Sie unterschiedliche Konfigurationen Ihrer Assets wie E-Kataloge, Bildsätze, Rotationssets, Mustersets, gemischte Mediensets, einfache Vorlagen und FXG-Vorlagen. Weitere Informationen finden Sie unter Rich-Media-Daten.

**Veröffentlichen und verwalten** Sie Assets im dynamischen Media Classic Saas-Netzwerk und überwachen Sie den Status von Assets, wenn sie veröffentlicht werden, verwalten Sie Benutzerrechte und behalten Sie die Sicherheit bei.

**Bereitstellen** von Medien aus dem dynamischen Media Classic Classic-saas-Netzwerk auf Webseiten, Anwendungen und mobilen Geräten; die Medien leistungsoptimiert sind und mit CDN-Caching bereitgestellt werden. Dynamic Media Classic stellt Ihnen eine URL für jedes Asset bereit. Sobald Sie das Asset veröffentlichen, wird die URL aktiv.

![Der Arbeitsablauf für dynamische Medien Classic](/help/assets/gs_workflow.png)

## Einzelne Masterbilder und einzelne URL-Aufrufe {#single-master-images-and-single-url-calls}

Dynamic Media Classic unterscheidet sich grundsätzlich von anderen Systemen, da Sie dynamische Medien Classic verwenden können, um Medien dynamisch aus einzelnen Master-Assets und URL-Aufrufen bereitzustellen.

Die URL-Zeichenfolgen, die Sie mit Dynamic Media Classic generieren, enthalten Anweisungen, die dem Server mitteilen, wie das Asset angezeigt wird, wenn es bereitgestellt wird. Ein und dasselbe Masterbild kann beispielsweise mit unterschiedlichen Größen, Formaten, Stärken, Farben und Zoomansichten gesendet werden. Im Zuge der Erstellung und Veröffentlichung von Medien-Assets mit Dynamic Media Classic konfigurieren Sie die Effekte visuell. Auf diese Weise werden die URL-Aufrufe erstellt, mit denen dem Server korrekt mitgeteilt wird, wie das Master-Asset in Anwendungen präsentiert werden soll.

![Dynamic Media Classic kann dasselbe Masterbild für verschiedene Medien in unterschiedlichen Größen und Formaten bereitstellen.](/help/assets/gs_dynamic_publishing.png)

## Inhalts-Caching {#content-caching}

Die Bilder, die Dynamisches Media Classic dynamisch generiert, sind Cache-freundlich; In den meisten Fällen handelt es sich um JPEG-Bilder mit eindeutigen URL-Aufrufen, die sie identifizieren. Die Bilder werden über ein CDN-System (Content Delivery Network) gesendet, ein Netzwerk von Servern, die über das Internet miteinander verbunden sind und dazu dienen, Inhalte schneller zu übermitteln. Die Bilder werden zunächst von weltweit verbreiteten Servern verteilt und dann an einzelne Computer gesendet. Wenn Sie einen Caching-Mechanismus mit einem beliebigen CDN-Anbieter implementieren, ändern Sie einfach den Servernamen, um auf den CDN-aktivierten dynamischen Medienserver zu verweisen. Alle dynamischen Media Classic-Editionen enthalten CDN-Caching.
