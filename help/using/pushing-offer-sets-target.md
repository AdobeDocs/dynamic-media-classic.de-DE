---
title: Angebotssets auf Adobe Target Standard/Premium pushen
description: Erfahren Sie, wie Sie von Adobe Dynamic Media Classic aus Angebotssätze auf Adobe Target Standard/Premium übertragen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:55:22.850Z'
TQID: 'https://experienceleague.adobe.com/8j9sRn1zhAhgj-wMV6hYix1F9aARZjDUiFZofcVVcBw'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 289
ht-degree: 0%

---

# Angebotssets auf Adobe Target Standard/Premium pushen {#pushing-offer-sets-to-target}

Nachdem Sie ein Angebotsset erstellt oder bearbeitet haben, übertragen Sie es auf Adobe Target Standard/Premium, indem Sie die folgenden Schritte ausführen:

1. Wählen Sie im Bildschirm „Test&amp;Target-Angebotssatz“ die Option **[!UICONTROL Push-Angebote]**.
1. Geben Sie Ihren Clientcode und Ihre Anmeldedaten ein.
1. Wählen Sie **[!UICONTROL Anmelden]** aus.

Bei der Übertragung auf Adobe Target Standard/Premium wird das Präfix `S7_` automatisch an den Beginn der Angebotsnamen angehängt. Dieses Präfix ist beigefügt, damit Sie Adobe Dynamic Media Classic-Angebote in der Test&amp;Target-Angebotsliste leicht finden können. Das Angebot wird beispielsweise als `S7_<name of offer set>_<offer name>` angezeigt.

Adobe Dynamic Media Classic übernimmt Adobe Target Standard/Premium-Widget-Angebote. Sie können Widget-Angebote verwenden, um Ihre eigenen angebotenen Inhalte auf Adobe Target Standard/Premium zu hosten. Widget-Angebote ähneln einem Standardangebot, das von Adobe Target Standard/Premium gehostet wird. Sie ermöglichen es Adobe Target Standard/Premium, auf Ihrem Server gespeicherte Angebotsinhalte bereitzustellen, was eine komplexere und dynamischere Nutzung ermöglicht. Widget-Angebote können Inhalte von einer URL abrufen, diese Inhalte zwischenspeichern und für etwa zwei Stunden bereitstellen. Widget-Angebote bieten einige Funktionen zur dynamischen Inhaltserstellung, die andere Angebote außerhalb von Adobe Target Standard/Premium nicht bieten. Wenn die Mbox, die das Angebot bereitstellt, Mbox-Parameter wie `mboxProductID` und `mbox.offerId` enthält, werden die `productId=[PRODUCT_ID]`- und `offerID=[OFFERID]` URL-Parameter an die angeforderte URL angehängt. Diese Parameter werden von einem Service verwendet, der unter der Widget-Angebots-URL verfügbar ist, um Inhalte außerhalb von Adobe Target Standard/Premium zurückzugeben, die Produkt- oder Bestellinformationen aus Ihren Mboxes verwenden. Auf das Widget-Angebot kann auch über die API zugegriffen werden, sodass Sie programmgesteuert Angebote außerhalb von Adobe Target Standard/Premium erstellen können.
