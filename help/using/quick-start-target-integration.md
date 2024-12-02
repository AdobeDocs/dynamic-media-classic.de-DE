---
title: 'Schnellstart: Integration von Adobe Target Standard/Premium'
description: Eine Einführung in Adobe Target Standard/Premium und ein Schnellstart für den schnellen Einstieg in die Adobe Target Standard/Premium-Integrationstechniken in Adobe Dynamic Media Classic.
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

# Schnellstart: Integration von Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium überlässt die Kontrolle direkt den Marketing-Experten. Dies kann dazu beitragen, schnell und kontinuierlich mehrere A/B- und Multivarianztests durchzuführen und die Effektivität zu messen. Außerdem kann es die Relevanz von Online-Inhalten durch Segmentierung, Targeting und Automated Personalization steigern.

Mit Adobe Dynamic Media Classic können Sie Angebote und Angebotssets für Adobe Target Standard-/Premium-Kampagnen erstellen. Sie können beispielsweise ein Angebotsset mit drei Varianten desselben Rich-Media-Assets erstellen. Dann können Sie über Adobe Target Standard oder Premium verfügen, um zu ermitteln, welches Asset eine bessere Konversionssteigerung bietet. Sie können Angebote und Angebotssets aus einer einfachen Vorlage oder aus einzelnen Bildern erstellen. Nachdem das Angebotsset in Adobe Target Standard/Premium gepusht oder gespeichert wurde, wo die Angebote Mboxes und Erlebnissen zugeordnet sind, kann Adobe Target Standard/Premium Kampagnen ausführen. Diese Kampagnen bestimmen, welche Variante einer Website bei Clickthroughs und Konversion wahrscheinlich die beste Leistung erzielt.

Verwenden Sie Adobe Target Standard-/Premium-HTML-Angebote, um die Anpassung von dynamischen Adobe Dynamic Media Classic-Inhalten zu verbessern. Weitere Informationen finden Sie in der Produktdokumentation zu [Adobe Target Standard/Premium](https://experienceleague.adobe.com/en/docs/target) .

>[!NOTE]
>
>Für die Verwendung von Adobe Target Standard/Premium mit Adobe Dynamic Media Classic ist ein gültiges Adobe Target Standard-/Premium-Konto erforderlich.

Diese Kurzanleitung soll Ihnen den schnellen Einstieg in die Verwendung von Adobe Target Standard-/Premium-HTML-Angebotssets erleichtern. Führen Sie die Schritte 1 bis 3 aus. Nach jedem Schritt gibt es einen Querverweis zu einer Themenüberschrift, in der Sie weitere Informationen finden können.

## 1. Geben Sie Ihre Adobe Target Standard-/Premium-URL auf der Seite &quot;Allgemeine Programmeinstellungen&quot;ein.

Adobe Dynamic Media Classic benötigt Ihre Adobe Target Standard-/Premium-URL zur Integration in Adobe Target Standard/Premium. Kopieren Sie den Teil Ihrer Adobe Target Standard-/Premium-URL bis einschließlich &quot;`.com`&quot;und geben Sie ihn auf der Seite &quot;Adobe Dynamic Media Classic **[!UICONTROL Allgemeine Programmeinstellungen]**&quot;in das Textfeld &quot;**[!UICONTROL Server]**&quot;, **[!UICONTROL Test&amp;Target-Servername]**&quot;ein. Siehe [Integrieren von Adobe Dynamic Media Classic mit Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. Erstellen Sie das Angebotsset

Verwenden Sie eine parametrisierte Vorlage oder Bilder, um ein Angebotsset zu erstellen. Sie können HTML-Angebotssets auf der Seite &quot;Test&amp;Target-Angebotsset&quot;erstellen. Um diese Seite zu öffnen, wählen Sie die Vorlage oder die Bilder aus und navigieren Sie dann in der Symbolleiste für globale Navigation zu **[!UICONTROL Build]** > **[!UICONTROL Test&amp;Target-Angebotsset]**.

Um ein Angebot mit einer Vorlage zu erstellen, wählen Sie **[!UICONTROL Hinzufügen und Vorschau]** aus. Ändern Sie auf der Seite Hinzufügen und Vorschau die Parameterwerte.

Um ein Angebot mit Bildern zu erstellen, ziehen Sie die Bilder auf die Seite Test&amp;Target-Angebotsset . Wählen Sie **[!UICONTROL Vorschau]** und wählen Sie eine Bildvorgabe für ein Bild oder alle Bilder im Angebotsset aus.

Speichern Sie das Angebotsset, nachdem Sie es erstellt haben.

Siehe [Erstellen eines Angebotssets](creating-offer-set.md#creating_an_offer_set).

## 3. Angebotssatz in Adobe Target Standard/Premium verschieben

Wählen Sie auf der Seite &quot;Test&amp;Target-Angebotsset&quot;die Option **[!UICONTROL Push-Angebote]** aus und geben Sie Ihre Anmeldedaten im Dialogfeld &quot;Test&amp;Target-Anmeldung&quot;ein. Siehe [Angebotssets an Adobe Target Standard/Premium pushen](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
