---
title: Angebotssets an Adobe Target Standard/Premium senden
description: Erfahren Sie, wie Sie Angebotssets von Adobe Dynamic Media Classic an Adobe Target Standard/Premium pushen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Angebotssets an Adobe Target Standard/Premium senden {#pushing-offer-sets-to-target}

Nachdem Sie ein Angebotsset erstellt oder bearbeitet haben, pushen Sie es in Adobe Target Standard/Premium, indem Sie die folgenden Schritte ausführen:

1. Wählen Sie im Bildschirm &quot;Test&amp;Target-Angebotsset&quot;die Option **[!UICONTROL Push-Angebote]**.
1. Geben Sie Ihren Clientcode und Ihre Anmeldedaten ein.
1. Wählen Sie **[!UICONTROL Anmelden]** aus.

Bei der Übertragung auf Adobe Target Standard/Premium wird das Präfix `S7_` automatisch an den Anfang der Angebotsnamen angehängt. Dieses Präfix wird angehängt, um sicherzustellen, dass Sie Adobe Dynamic Media Classic-Angebote in der Test&amp;Target-Angebotsliste einfach finden können. Das Angebot wird beispielsweise als `S7_<name of offer set>_<offer name>` angezeigt.

Adobe Dynamic Media Classic pusht in Adobe Target Standard-/Premium-Widget-Angebote. Mit Widget-Angeboten können Sie Ihre eigenen bereitgestellten Inhalte in Adobe Target Standard/Premium hosten. Widget-Angebote ähneln einem Standardangebot, das von Adobe Target Standard/Premium gehostet wird. Sie ermöglichen es Adobe Target Standard/Premium, auf Ihrem Server gespeicherte Angebotsinhalte bereitzustellen, sodass eine komplexere und dynamischere Nutzung möglich ist. Widget-Angebote können Inhalte von einer URL abrufen, diese Inhalte etwa zwei Stunden lang zwischenspeichern und bereitstellen. Widget-Angebote bieten einige Funktionen zur dynamischen Inhaltserstellung, die andere Angebote außerhalb von Adobe Target Standard/Premium nicht bieten. Wenn die mbox, die das Angebot bereitstellt, mbox-Parameter wie `mboxProductID` und `mbox.offerId` enthält, werden die URL-Parameter `productId=[PRODUCT_ID]`und `offerID=[OFFERID]` an die angeforderte URL angehängt. Diese Parameter werden von einem Dienst verwendet, der unter der Widget-Angebots-URL verfügbar ist, um Inhalte außerhalb von Adobe Target Standard/Premium zurückzugeben, die Produkt- oder Bestellinformationen aus Ihren Mboxes verwenden. Das Widget-Angebot ist auch über die API verfügbar, sodass Sie Angebote außerhalb von Adobe Target Standard/Premium programmgesteuert erstellen können.
