---
title: Übersicht über die Adobe Dynamic Media Classic-Plattform
seo-title: Übersicht über die Adobe Dynamic Media Classic-Plattform
description: 'null'
seo-description: Eine Übersicht über die Plattform und den Workflow von Dynamic Media Classic.
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: Verweis
products: SG_EXPERIENCEMANAGER/Dynamic Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting-started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Übersicht über die Adobe Dynamic Media Classic-Plattform{#adobe-scene-platform-overview}

Dynamic Media Classic ist eine integrierte Umgebung für Rich-Media-Verwaltung, -Veröffentlichung und -Bereitstellung. Rich-Media-Daten können für alle Marketing- und Vertriebskanäle verwendet werden, einschließlich Internet, Druckmaterial, E-Mail-Kampagnen, Web-Portale, Desktop-Computer und sonstige Geräte.

## Workflows {#workflow-process}

Die wichtigsten Workflow-Schritte für Dynamic Media Classic sind:

* **Hochladen und Verwalten Ihrer Assets** Hochladen Ihrer Medienelemente in das SPS. In diesem System können Sie Assets organisieren und durchsuchen sowie nach bestimmten Assets suchen. Außerdem können Sie Metadaten auf Assets anwenden. Wenn Sie die Adobe Scene7 Publishing System-Desktop-Anwendung installieren, können Sie Dateien und Ordner von Ihrem Desktop in einen Zielordner ziehen und so in diesen Ordner hochladen.

* **Rich-Media-Daten** erstellen Erstellen Sie verschiedene Konfigurationen Ihrer Assets, z. B. E-Kataloge, Bildsätze, Rotationssets, Mustersets, gemischte Mediensets, einfache Vorlagen und FXG-Vorlagen. Weitere Informationen finden Sie unter Rich-Media-Daten.

* **Veröffentlichen und verwalten** Sie Assets im Dynamischen Media Classic Saas-Netzwerk, überwachen Sie den Status der Assets beim Veröffentlichen, verwalten Sie Benutzerrechte und verwalten Sie die Sicherheit.

* **Bereitstellung von** Medien aus dem SaaS-Netzwerk für dynamische Medien, Anwendungen und Mobilgeräte; die Medien sind leistungsoptimiert und werden mit CDN-Caching bereitgestellt. Mit Dynamic Media Classic erhalten Sie eine URL für jedes Asset. Sobald Sie das Asset veröffentlichen, wird die URL aktiv.

![Der Workflow für dynamische Medien - Classic](/help/assets/gs_workflow.png)

## Einzelne Masterbilder und einzelne URL-Aufrufe {#single-master-images-and-single-url-calls}

Dynamic Media Classic unterscheidet sich grundsätzlich von anderen Systemen, da Sie mit Dynamic Media Classic Medien dynamisch aus einzelnen Master-Assets und URL-Aufrufen bereitstellen können.

Die URL-Zeichenfolgen, die Sie mit Dynamic Media Classic generieren, enthalten Anweisungen, die dem Server mitteilen, wie das Asset angezeigt wird, wenn es bereitgestellt wird. Ein und dasselbe Masterbild kann beispielsweise mit unterschiedlichen Größen, Formaten, Stärken, Farben und Zoomansichten gesendet werden. Beim Erstellen und Veröffentlichen von Medienelementen mit Dynamic Media Classic konfigurieren Sie die Effekte visuell. Auf diese Weise werden die URL-Aufrufe erstellt, mit denen dem Server korrekt mitgeteilt wird, wie das Master-Asset in Anwendungen präsentiert werden soll.

![Mit Dynamic Media Classic können Sie dasselbe Masterbild für verschiedene Medien in unterschiedlichen Größen und Formaten bereitstellen.](/help/assets/gs_dynamic_publishing.png)

## Inhalts-Caching {#content-caching}

Die dynamisch von Dynamic Media Classic erstellten Bilder sind Cache-freundlich. In den meisten Fällen handelt es sich um JPEG-Bilder mit eindeutigen URL-Aufrufen, die diese identifizieren. Die Bilder werden über ein CDN-System (Content Delivery Network) gesendet, ein Netzwerk von Servern, die über das Internet miteinander verbunden sind und dazu dienen, Inhalte schneller zu übermitteln. Die Bilder werden zunächst von weltweit verbreiteten Servern verteilt und dann an einzelne Computer gesendet. Bei der Implementierung eines Caching-Mechanismus mit einem beliebigen CDN-Anbieter ändern Sie einfach den Servernamen so, dass er auf den CDN-fähigen Dynamic Media Image Server verweist. Zu allen Dynamic Media Classic-Editionen gehört die gebündelte CDN-Zwischenspeicherung.
