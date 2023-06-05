---
title: "Schnellstart: Integration von Adobe Target Standard/Premium"
description: Eine Einführung in Adobe Target Standard/Premium und ein Schnellstart für den schnellen Einstieg in die Adobe Target Standard/Premium-Integrationstechniken in Adobe Dynamic Media Classic.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 7%

---

# Schnellstart: Integration von Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium überlässt Marketing-Experten direkt die Kontrolle, um schnell und kontinuierlich mehrere A/B- und Multivarianztests durchzuführen, die Effektivität zu messen und die Relevanz von Online-Inhalten durch Segmentierung, Targeting und Automated Personalization zu steigern.

Mit Adobe Dynamic Media Classic können Sie Angebote und Angebotssets für Adobe Target Standard-/Premium-Kampagnen erstellen. Sie können beispielsweise ein Angebotsset mit drei Varianten desselben Rich-Media-Assets erstellen. Dann können Sie Adobe Target Standard/Premium festlegen, welches Asset eine bessere Konversionssteigerung bietet. Sie können Angebote und Angebotssets aus einer einfachen Vorlage oder aus einzelnen Bildern erstellen. Nachdem das Angebotsset in Adobe Target Standard/Premium gepusht oder gespeichert wurde, wo die Angebote Mboxes und Erlebnissen zugeordnet sind, kann Adobe Target Standard/Premium Kampagnen ausführen. Diese Kampagnen bestimmen, welche Variante einer Website bei Clickthroughs und Konversion wahrscheinlich die beste Leistung erzielt.

Verwenden Sie Adobe Target Standard-/Premium-HTML-Angebote, um die Anpassung von dynamischen Adobe Dynamic Media Classic-Inhalten zu verbessern. Siehe [Produktdokumentation zu Adobe Target Standard/Premium](https://experienceleague.adobe.com/docs/target.html) für weitere Informationen.

>[!NOTE]
>
>Für die Verwendung von Adobe Target Standard/Premium mit Adobe Dynamic Media Classic ist ein gültiges Adobe Target Standard-/Premium-Konto erforderlich.

Diese Kurzanleitung soll Ihnen einen schnellen Einstieg in die Arbeit mit Adobe Target Standard-/Premium-HTML-Angeboten ermöglichen. Führen Sie die Schritte 1 bis 3 aus. Nach jedem Schritt gibt es einen Querverweis zu einer Themenüberschrift, in der Sie weitere Informationen finden können.

## 1. Geben Sie Ihre Adobe Target Standard-/Premium-URL auf der Seite &quot;Allgemeine Programmeinstellungen&quot;ein.

Adobe Dynamic Media Classic benötigt Ihre Adobe Target Standard-/Premium-URL zur Integration in Adobe Target Standard/Premium. Kopieren Sie den Teil Ihrer Adobe Target Standard-/Premium-URL bis einschließlich `.com`und geben Sie ihn in die Adobe Dynamic Media Classic ein **[!UICONTROL Allgemeine Programmeinstellungen]** in der **[!UICONTROL Server]** Gruppe, **[!UICONTROL Test&amp;Target-Server-Name]** Textfeld. Siehe [Integrieren von Adobe Dynamic Media Classic mit Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. Erstellen Sie das Angebotsset.

Verwenden Sie eine parametrisierte Vorlage oder Bilder, um ein Angebotsset zu erstellen. Sie erstellen HTML-Angebotssets auf der Seite &quot;Test&amp;Target-Angebotsset&quot;. Um diese Seite zu öffnen, wählen Sie die Vorlage oder die Bilder aus und navigieren Sie dann in der Symbolleiste für globale Navigation zu **[!UICONTROL Build]** > **[!UICONTROL Test&amp;Target-Angebotsset]**.

Um ein Angebot mit einer Vorlage zu erstellen, wählen Sie **[!UICONTROL Hinzufügen und Vorschau]**. Ändern Sie auf der Seite Hinzufügen und Vorschau die Parameterwerte.

Um ein Angebot mit Bildern zu erstellen, ziehen Sie Bilder auf die Seite Test&amp;Target-Angebotsset . Auswählen **[!UICONTROL Vorschau]** und wählen Sie eine Bildvorgabe für ein Bild oder alle Bilder im Angebotsset aus.

Speichern Sie das Angebotsset, nachdem Sie es erstellt haben. 

Siehe [Angebotssatz erstellen](creating-offer-set.md#creating_an_offer_set).

## 3. Angebotssatz auf Adobe Target Standard/Premium pushen

Wählen Sie auf der Seite Test&amp;Target-Angebotsset die Option **[!UICONTROL Push-Angebote]** und geben Sie Ihre Anmeldedaten im Dialogfeld &quot;Test&amp;Target-Anmeldung&quot;ein. Siehe [Angebotssets an Adobe Target Standard/Premium senden](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
