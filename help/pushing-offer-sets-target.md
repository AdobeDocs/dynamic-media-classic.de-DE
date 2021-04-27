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
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Pushing von Angebot-Sets auf Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

Nachdem Sie ein Angebot-Set erstellt oder bearbeitet haben, führen Sie folgende Schritte aus, um es in Adobe Target Standard/Premium zu verschieben:

1. Klicken Sie im Bildschirm &quot;Test&amp;Zielgruppe-Angebot-Set&quot;auf **[!UICONTROL Push-Angebot]**.
1. Geben Sie Ihren Clientcode und Ihre Anmeldedaten ein.
1. Klicken Sie auf **[!UICONTROL Anmelden]**.

Während der Übertragung auf Adobe Target Standard/Premium wird das Präfix `S7_` automatisch an den Beginn der Angebot-Namen angehängt. Dieses Präfix wird angehängt, um sicherzustellen, dass Sie Dynamic Media Classic-Angebot in der Angebot-Liste von Test&amp;Zielgruppe leicht finden können. Das Angebot wird beispielsweise als `S7_<name of offer set>_<offer name>` angezeigt.

Dynamic Media Classic schiebt in Adobe Target Standard/Premium Widget-Angebot. Mit Widget-Angeboten können Sie Ihre eigenen Angebot-Inhalte außerhalb von Adobe Target Standard/Premium hosten. Widget-Angebot ähneln einem Standard-Angebot, das außerhalb von Adobe Target Standard/Premium gehostet wird. Sie ermöglichen es Adobe Target Standard/Premium, auf Ihrem Server gespeicherte Angebot-Inhalte bereitzustellen, wodurch eine anspruchsvollere und dynamischere Nutzung ermöglicht wird. Widget-Angebote rufen Inhalte von einer URL ab, speichern diese und beliefern sie rund zwei Stunden lang. Widget-Angebot bieten einige dynamische Inhaltsgenerierungsfunktionen, die andere Angebot außerhalb von Adobe Target Standard/Premium nicht bieten. Wenn die mbox, die das Angebot bereitstellt, mbox-Parameter wie `mboxProductID` und `mbox.offerId` enthält, werden die URL-Parameter `productId=[PRODUCT_ID]`und `offerID=[OFFERID]` an die angeforderte URL angehängt. Diese Parameter können von einem Dienst verwendet werden, der unter der Widget-Angebot-URL verfügbar ist, um Inhalte außerhalb von Adobe Target Standard/Premium zurückzugeben, die Produkt- oder Bestellinformationen aus Ihren mboxes verwenden. Das Widget-Angebot ist auch über die API verfügbar, um Angebot außerhalb von Adobe Target Standard/Premium programmgesteuert zu erstellen.
