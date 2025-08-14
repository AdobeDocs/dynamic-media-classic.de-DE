---
title: 'Schnellstart: Adobe Target Standard/Premium-Integration'
description: Eine Einführung und eine Kurzanleitung zu Adobe Target Standard/Premium, damit Sie die Adobe Target Standard/Premium-Integrationstechniken in Adobe Dynamic Media Classic schnell einrichten und ausführen können.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Schnellstart: Adobe Target Standard/Premium-Integration{#quick-start-target-integration}

Adobe Target Standard/Premium überlässt die Kontrolle direkt dem Marketing-Experten. Auf diese Weise können Sie schnell und kontinuierlich mehrere A/B- und multivariate Tests durchführen und die Effektivität messen. Und sie kann die Relevanz von Online-Inhalten durch Segmentierung, Targeting und Automated Personalization erhöhen.

Mit Adobe Dynamic Media Classic können Sie Angebote und Angebotssätze für Adobe Target Standard/Premium-Kampagnen erstellen. Sie können beispielsweise ein Angebotsset mit drei Varianten desselben Rich-Media-Assets erstellen. Dann können Sie Adobe Target Standard oder Premium verwenden, um zu bestimmen, welches Asset eine bessere Konversionssteigerung bietet. Sie können Angebote und Angebotssätze aus einer Basisvorlage oder aus einzelnen Bildern erstellen. Nachdem der Angebotssatz an Adobe Target Standard/Premium gesendet oder dort gespeichert wurde, wo die Angebote mit Mboxes und Erlebnissen verknüpft sind, kann Adobe Target Standard/Premium Kampagnen ausführen. Diese Kampagnen bestimmen, welche Variante einer Website für Clickthroughs und Konvertierungen am besten geeignet ist.

Verwenden Sie Adobe Target Standard/Premium-HTML-Angebote, um dynamische Adobe Dynamic Media Classic-Inhalte besser anzupassen. Weitere Informationen finden Sie in der [Adobe Target Standard/Premium](https://experienceleague.adobe.com/en/docs/target)Produktdokumentation.

>[!NOTE]
>
>Für die Verwendung von Adobe Target Standard/Premium mit Adobe Dynamic Media Classic ist ein gültiges Adobe Target Standard/Premium-Konto erforderlich.

Diese Kurzanleitung wurde entwickelt, um Sie schnell mit den Adobe Target Standard/Premium HTML-Angebotssätzen vertraut zu machen. Führen Sie die Schritte 1 bis 3 aus. Nach jedem Schritt finden Sie einen Querverweis auf eine Themenüberschrift, unter der Sie weitere Informationen finden.

## &#x200B;1. Geben Sie auf der Seite „Allgemeine Programmeinstellungen“ die Adobe Target Standard/Premium-URL ein

Adobe Dynamic Media Classic benötigt Ihre Adobe Target Standard/Premium-URL für die Integration mit Adobe Target Standard/Premium. Kopieren Sie den Teil Ihrer Adobe Target Standard/Premium-URL bis einschließlich `.com` und geben Sie ihn auf der Seite „Allgemeine **[!UICONTROL -Einstellungen“]** Adobe Dynamic Media Classic in die Gruppe **[!UICONTROL Server]** im Textfeld **[!UICONTROL Test&amp;Target]** Servername ein. Siehe [Integrieren von Adobe Dynamic Media Classic mit Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## &#x200B;2. Erstellen des Angebotssatzes

Verwenden Sie eine parametrisierte Vorlage oder Bilder, um ein Angebotsset zu erstellen. Sie können HTML-Angebotssätze auf der Seite Test&amp;Target-Angebotssätze erstellen. Wählen Sie zum Öffnen dieser Seite Ihre Vorlage oder Ihre Bilder aus und navigieren Sie dann in der globalen Navigationsleiste zu **[!UICONTROL Erstellen]** > **[!UICONTROL Test&amp;Target-]**.

Um ein Angebot mit einer Vorlage zu erstellen, wählen Sie **[!UICONTROL Hinzufügen und Vorschau]** aus. Ändern Sie auf der Seite „Hinzufügen und Vorschau“ die Parameterwerte.

Um ein Angebot mit Bildern zu erstellen, ziehen Sie die Bilder in die Seite „Test&amp;Target-Angebotssatz“. Wählen Sie **[!UICONTROL Vorschau]** und wählen Sie eine Bildvorgabe für ein Bild oder alle Bilder im Angebotsset aus.

Speichern Sie das Angebotsset, nachdem Sie es erstellt haben.

Siehe [Erstellen eines Angebotssatzes](creating-offer-set.md#creating_an_offer_set).

## &#x200B;3. Das Angebot auf Adobe Target Standard/Premium verschieben

Wählen Sie auf der Seite „Test&amp;Target-Angebotssatz“ die Option **[!UICONTROL Push-Angebote]** aus und geben Sie im Dialogfeld „Test&amp;Target-Anmeldung“ Ihre Anmeldedaten ein. Siehe [Pushen von Angebotssätzen auf Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
