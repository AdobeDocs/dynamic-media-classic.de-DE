---
title: '"Schnellstart: Integration von Adobe Target Standard/Premium"'
description: Eine Einführung in Adobe Target Standard/Premium und ein Schnellstart für den schnellen Einstieg in die Adobe Target Standard/Premium-Integrationstechniken.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 12%

---

# Schnellstart: Integration von Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium überlässt Marketing-Experten direkt die Kontrolle, um schnell und kontinuierlich mehrere A/B- und Multivarianztests durchzuführen, die Effektivität zu messen und die Relevanz von Online-Inhalten durch Segmentierung, Targeting und automatisierte Personalisierung zu steigern.

Mit Dynamic Media Classic können Sie Angebote und Angebotssets für Adobe Target Standard-/Premium-Kampagnen erstellen. Sie können beispielsweise ein Angebotsset mit drei Varianten desselben Rich-Media-Assets erstellen. Dann können Sie Adobe Target Standard/Premium festlegen, welches Asset eine bessere Konversionssteigerung bietet. Sie können Angebote und Angebotssets aus einer einfachen Vorlage oder aus einzelnen Bildern erstellen. Nachdem das Angebotsset in Adobe Target Standard/Premium gepusht oder gespeichert wurde, wo die Angebote Mboxes und Erlebnissen zugeordnet sind, kann Adobe Target Standard/Premium Kampagnen ausführen. Diese Kampagnen bestimmen, welche Variante einer Website bei Clickthroughs und Konversion wahrscheinlich die beste Leistung erzielt.

Verwenden Sie für eine bessere Anpassung von dynamischen Dynamic Media Classic-Inhalten Adobe Target Standard/Premium HTML-Angebote. Weitere Informationen finden Sie in der [Produktdokumentation zu Adobe Target Standard/Premium](https://experienceleague.adobe.com/docs/target.html).

>[!NOTE]
>
>Für die Verwendung von Adobe Target Standard/Premium mit Dynamic Media Classic ist ein gültiges Adobe Target Standard-/Premium-Konto erforderlich.

Diese Kurzanleitung soll Ihnen einen schnellen Einstieg in die Arbeit mit HTML-Angebotssets von Adobe Target Standard/Premium ermöglichen. Führen Sie die Schritte 1 bis 3 aus. Nach jedem Schritt wird auf ein Thema mit weiteren Informationen verwiesen.

## 1. Geben Sie Ihre Adobe Target Standard-/Premium-URL auf der Seite &quot;Allgemeine Programmeinstellungen&quot;ein.

Dynamic Media Classic benötigt Ihre Adobe Target Standard-/Premium-URL zur Integration in Adobe Target Standard/Premium. Kopieren Sie den Teil Ihrer Adobe Target Standard-/Premium-URL bis einschließlich `.com` und geben Sie ihn auf der Seite **[!UICONTROL Allgemeine Anwendungseinstellungen]** in der Gruppe **[!UICONTROL Server]** in **[!UICONTROL Test&amp;Target-Server-Name]** ein. Siehe [Integrieren von Dynamic Media Classic mit Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. Erstellen Sie das Angebotsset.

Verwenden Sie eine parametrisierte Vorlage oder Bilder, um ein Angebotsset zu erstellen. Sie erstellen HTML-Angebotssätze auf der Seite Test&amp;Target-Angebotsset . Um diese Seite zu öffnen, wählen Sie Ihre Vorlage oder Bilder aus und klicken Sie dann in der Symbolleiste für globale Navigation auf **[!UICONTROL Build]** > **[!UICONTROL Test&amp;Target-Angebotsset]**.

Um ein Angebot mit einer Vorlage zu erstellen, klicken Sie auf **[!UICONTROL Hinzufügen und Vorschau]**. Ändern Sie auf der Seite Hinzufügen und Vorschau die Parameterwerte.

Um ein Angebot mit Bildern zu erstellen, ziehen Sie Bilder auf die Seite Test&amp;Target-Angebotsset . Klicken Sie auf **[!UICONTROL Vorschau]** und wählen Sie eine Bildvorgabe für ein Bild oder alle Bilder im Angebotsset aus.

Speichern Sie das Angebotsset, nachdem Sie es erstellt haben. 

Siehe [Erstellen eines Angebotssets](creating-offer-set.md#creating_an_offer_set).

## 3. Angebotssatz auf Adobe Target Standard/Premium pushen

Klicken Sie auf der Seite &quot;Test&amp;Target-Angebotsset&quot;auf **[!UICONTROL Push-Angebote]** und geben Sie Ihre Anmeldedaten im Dialogfeld &quot;Test&amp;Target-Anmeldung&quot;ein. Siehe [Pushing von Angebotssets in Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
