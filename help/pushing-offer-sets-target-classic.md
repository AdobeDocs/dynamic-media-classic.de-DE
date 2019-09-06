---
title: Weiterleiten von Angebotssets an Adobe Target Classic
seo-title: Weiterleiten von Angebotssets an Adobe Target Classic
description: 'null'
seo-description: Erfahren Sie, wie Sie Angebotssets an Adobe Target Classic senden.
uuid: 8 c 895 a 7 c -21 b 4-4 d 85-8 b 0 b-a 3 d 2 a 420 bf 2 e
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/target_ classic_ integration
discoiquuid: 39 a 05654-4 f 66-4 f 1 e-aec 5-ebe 6 d 174353 f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Weiterleiten von Angebotssets an Adobe Target Classic{#pushing-offer-sets-to-adobe-target-classic}

Nachdem Sie ein Angebotsset erstellt oder bearbeitet haben, leiten Sie es an Target Classic weiter, indem Sie folgende Schritte ausführen:

1. Klicken Sie im Anzeigebereich "Angebotsset von Target Classic" auf die Schaltfläche" Angebote fördern" .
1. Geben Sie Ihre Anmeldedaten ein.
1. Klicken Sie auf die Anmeldeschaltfläche.

Während der Übertragung an Target Classic wird das Präfix S 7_ automatisch an den Anfang der Angebotsnamen angehängt. Dieses Präfix wird angehängt, um sicherzustellen, dass Sie dynamische Media Classic-Angebote in der Angebotsliste von Target Classic leicht finden können. Das Angebot wird beispielsweise als S7_&lt;Name des Angebotssets&gt;_&lt;Name des Angebots&gt; angezeigt.

SPS-Pushes werden in Target Classic-Widget angeboten. Mit Widget-Angeboten können Sie Ihre eigenen Angebotsinhalte außerhalb von Target Classic hosten. Widget-Angebote ähneln einem Standardangebot, das außerhalb von Target Classic gehostet wird. Sie ermöglichen es Target Classic, Angebotsinhalte bereitzustellen, die auf Ihrem Server gespeichert sind, was eine anspruchsvollere und dynamischere Nutzung ermöglicht. Mit Widget-Angeboten können Inhalte aus einer URL abgerufen werden, die ca. zwei Stunden lang zwischengespeichert und bereitgestellt werden. Widget bietet einige dynamische Inhaltserstellungsfunktionen, die andere Angebote außerhalb von Target Classic nicht bieten. If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. Diese Parameter können von einem unter der URL des Widget-Angebots verfügbaren Dienst verwendet werden, um Inhalte außerhalb von Target Classic zurückzugeben, die Produkt- oder Bestellinformationen aus Ihren mboxes verwenden. Das Widget-Angebot kann auch über die API aufgerufen werden, um Angebote außerhalb von Target Classic programmgesteuert zu erstellen.
