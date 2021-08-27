---
title: Angebotssets an Adobe Target Standard/Premium senden
description: Erfahren Sie, wie Sie Angebotssets an Adobe Target Standard/Premium senden.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---

# Angebotssets an Adobe Target Standard/Premium senden {#pushing-offer-sets-to-target}

Nachdem Sie ein Angebotsset erstellt oder bearbeitet haben, pushen Sie es in Adobe Target Standard/Premium, indem Sie die folgenden Schritte ausführen:

1. Klicken Sie im Bildschirm &quot;Test&amp;Target-Angebotsset&quot;auf **[!UICONTROL Push-Angebote]**.
1. Geben Sie Ihren Clientcode und Ihre Anmeldedaten ein.
1. Klicken Sie auf **[!UICONTROL Anmelden]**.

Bei der Übertragung auf Adobe Target Standard/Premium wird das Präfix `S7_` automatisch an den Anfang der Angebotsnamen angehängt. Dieses Präfix ist angehängt, um sicherzustellen, dass Sie Adobe Dynamic Media Classic-Angebote einfach in der Test&amp;Target-Angebotsliste finden können. Das Angebot wird beispielsweise als `S7_<name of offer set>_<offer name>` angezeigt.

Adobe Dynamic Media Classic sendet Inhalte in Adobe Target Standard-/Premium-Widget-Angebote. Sie können Widget-Angebote verwenden, um eigene Angebotsinhalte außerhalb von Adobe Target Standard/Premium zu hosten. Widget-Angebote ähneln einem Standardangebot, das außerhalb von Adobe Target Standard/Premium gehostet wird. Sie ermöglichen es Adobe Target Standard/Premium, auf Ihrem Server gespeicherte Angebotsinhalte bereitzustellen, sodass eine komplexere und dynamischere Nutzung möglich ist. Widget-Angebote rufen Inhalte von einer URL ab, speichern diese Inhalte und liefern sie etwa zwei Stunden lang. Widget-Angebote bieten einige Funktionen zur dynamischen Inhaltserstellung, die andere Angebote außerhalb von Adobe Target Standard/Premium nicht bieten. Wenn die mbox, die das Angebot bereitstellt, mbox-Parameter wie `mboxProductID` und `mbox.offerId` enthält, werden die URL-Parameter `productId=[PRODUCT_ID]`und `offerID=[OFFERID]` an die angeforderte URL angehängt. Diese Parameter können von einem Dienst verwendet werden, der unter der URL des Widget-Angebots verfügbar ist, um Inhalte außerhalb von Adobe Target Standard/Premium zurückzugeben, die Produkt- oder Bestellinformationen aus Ihren Mboxes verwenden. Auf das Widget-Angebot kann auch über die API zugegriffen werden, um Angebote außerhalb von Adobe Target Standard/Premium programmgesteuert zu erstellen.
