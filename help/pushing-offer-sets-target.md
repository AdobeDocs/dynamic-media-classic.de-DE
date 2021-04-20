---
title: Pushing von Angebot-Sets auf Adobe Target Standard/Premium
description: Erfahren Sie, wie Sie Angebot-Sets auf Adobe Target Standard/Premium verschieben.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 5%

---


# Pushing von Angebot-Sets auf Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Nachdem Sie einen Angebot-Satz erstellt oder bearbeitet haben, führen Sie folgende Schritte aus, um ihn in Target Standard/Premium zu verschieben:

1. Klicken Sie im Bildschirm &quot;Test&amp;Zielgruppe-Angebot-Set&quot;auf **[!UICONTROL Push-Angebot]**.
1. Geben Sie Ihren Clientcode und Ihre Anmeldedaten ein.
1. Klicken Sie auf **[!UICONTROL Anmelden]**.

Während der Übertragung auf Target Standard/Premium wird das Präfix S7_ automatisch an den Beginn der Angebot-Namen angehängt. Dieses Präfix wird angehängt, um sicherzustellen, dass Sie Dynamic Media Classic-Angebot in der Angebot-Liste von Test&amp;Zielgruppe leicht finden können. Das Angebot wird beispielsweise als S7_&lt;Name des Angebotssets>_&lt;Name des Angebots> angezeigt.

Dynamic Media Classic schiebt in Target Standard/Premium-Widget-Angebot. Mit Widget-Angeboten können Sie Ihre eigenen Angebot-Inhalte außerhalb von Target Standard/Premium hosten. Widget-Angebot ähneln einem Standard-Angebot, das außerhalb von Target Standard/Premium gehostet wird. Sie ermöglichen es Target Standard/Premium, auf Ihrem Server gespeicherte Angebot-Inhalte bereitzustellen, sodass eine anspruchsvollere und dynamischere Nutzung möglich ist. Widget-Angebote rufen Inhalte von einer URL ab, speichern diese und beliefern sie rund zwei Stunden lang. Widget-Angebot bieten einige dynamische Inhaltsgenerierungsfunktionen, die andere Angebot außerhalb von Target Standard/Premium nicht bieten. Wenn die mbox, die das Angebot bereitstellt, mbox-Parameter wie `mboxProductID` und `mbox.offerId` enthält, werden die URL-Parameter `productId=[PRODUCT_ID]`und `offerID=[OFFERID]` an die angeforderte URL angehängt. Diese Parameter können von einem Dienst verwendet werden, der unter der Widget-Angebot-URL verfügbar ist, um Inhalte außerhalb von Target Standard/Premium zurückzugeben, die Produkt- oder Bestellinformationen aus Ihren mboxes verwenden. Das Widget-Angebot ist auch über die API verfügbar, um programmgesteuert Angebot außerhalb von Target Standard/Premium zu erstellen.
