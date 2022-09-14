---
title: Angebotssets an Adobe Target Standard/Premium senden
description: Erfahren Sie, wie Sie Angebotssets von Adobe Dynamic Media Classic an Adobe Target Standard/Premium pushen.
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Angebotssets an Adobe Target Standard/Premium senden {#pushing-offer-sets-to-target}

Nachdem Sie ein Angebotsset erstellt oder bearbeitet haben, pushen Sie es in Adobe Target Standard/Premium, indem Sie die folgenden Schritte ausführen:

1. Wählen Sie im Bildschirm &quot;Test&amp;Target-Angebotsset&quot;die Option **[!UICONTROL Push-Angebote]**.
1. Geben Sie Ihren Clientcode und Ihre Anmeldedaten ein.
1. Auswählen **[!UICONTROL Anmelden]**.

Während der Übertragung an Adobe Target Standard/Premium wird das Präfix `S7_` wird automatisch an den Anfang der Angebotsnamen angehängt. Dieses Präfix wird angehängt, um sicherzustellen, dass Sie Adobe Dynamic Media Classic-Angebote in der Test&amp;Target-Angebotsliste einfach finden können. Das Angebot wird beispielsweise als `S7_<name of offer set>_<offer name>`.

Adobe Dynamic Media Classic pusht in Adobe Target Standard-/Premium-Widget-Angebote. Sie können Widget-Angebote verwenden, um eigene Angebotsinhalte außerhalb von Adobe Target Standard/Premium zu hosten. Widget-Angebote ähneln einem Standardangebot, das außerhalb von Adobe Target Standard/Premium gehostet wird. Sie ermöglichen es Adobe Target Standard/Premium, auf Ihrem Server gespeicherte Angebotsinhalte bereitzustellen, sodass eine komplexere und dynamischere Nutzung möglich ist. Widget-Angebote können Inhalte von einer URL abrufen, diese Inhalte etwa zwei Stunden lang zwischenspeichern und bereitstellen. Widget-Angebote bieten einige Funktionen zur dynamischen Inhaltserstellung, die andere Angebote außerhalb von Adobe Target Standard/Premium nicht bieten. Wenn die mbox, die das Angebot bereitstellt, Mbox-Parameter wie `mboxProductID` und `mbox.offerId`, die `productId=[PRODUCT_ID]`und `offerID=[OFFERID]` URL-Parameter werden an die angeforderte URL angehängt. Diese Parameter können von einem Dienst verwendet werden, der unter der URL des Widget-Angebots verfügbar ist, um Inhalte außerhalb von Adobe Target Standard/Premium zurückzugeben, die Produkt- oder Bestellinformationen aus Ihren Mboxes verwenden. Auf das Widget-Angebot kann auch über die API zugegriffen werden, um Angebote außerhalb von Adobe Target Standard/Premium programmgesteuert zu erstellen.
