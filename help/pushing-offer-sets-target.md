---
title: Pushing von Angebot-Sets auf Adobe Target Standard/Premium
seo-title: Pushing von Angebot-Sets auf Adobe Target Standard/Premium
description: 'null'
seo-description: Erfahren Sie, wie Sie Angebot-Sets auf Adobe Target Standard/Premium verschieben.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 5%

---


# Pushing von Angebot-Sets auf Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Nachdem Sie einen Angebot-Satz erstellt oder bearbeitet haben, führen Sie folgende Schritte aus, um ihn in Target Standard/Premium zu verschieben:

1. In the Test&amp;Target Offer Set screen, click **[!UICONTROL Push Offers]**.
1. Geben Sie Ihren Clientcode und Ihre Anmeldedaten ein.
1. Klicken Sie auf **[!UICONTROL Anmelden]**.

Während der Übertragung auf Target Standard/Premium wird das Präfix S7_ automatisch an den Beginn der Angebot-Namen angehängt. Dieses Präfix wird angehängt, um sicherzustellen, dass Sie die Angebot von Dynamic Media Classic in der Test&amp;Zielgruppe Angebot-Liste leicht finden können. Das Angebot wird beispielsweise als S7_&lt;Name des Angebotssets>_&lt;Name des Angebots> angezeigt.

Dynamische Medien-Classic-Push-Vorgänge in Target Standard/Premium-Widget-Angebot. Mit Widget-Angeboten können Sie Ihre eigenen Angebot-Inhalte außerhalb von Target Standard/Premium hosten. Widget-Angebot ähneln einem Standard-Angebot, das außerhalb von Target Standard/Premium gehostet wird. Sie ermöglichen es Target Standard/Premium, auf Ihrem Server gespeicherte Angebot-Inhalte bereitzustellen, sodass eine anspruchsvollere und dynamischere Nutzung möglich ist. Widget-Angebote rufen Inhalte von einer URL ab, speichern diese und beliefern sie rund zwei Stunden lang. Widget-Angebot bieten einige dynamische Inhaltsgenerierungsfunktionen, die andere Angebot außerhalb von Target Standard/Premium nicht bieten. If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. Diese Parameter können von einem Dienst verwendet werden, der unter der Widget-Angebot-URL verfügbar ist, um Inhalte außerhalb von Target Standard/Premium zurückzugeben, die Produkt- oder Bestellinformationen aus Ihren mboxes verwenden. Das Widget-Angebot ist auch über die API verfügbar, um programmgesteuert Angebot außerhalb von Target Standard/Premium zu erstellen.
