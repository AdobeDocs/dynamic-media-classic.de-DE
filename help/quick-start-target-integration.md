---
title: '"Beginn: Integration von Adobe Target Standard/Premium"'
description: Eine Einführung und ein kurzer Beginn zu Adobe Target Standard/Premium, mit dem Sie sich schnell mit Adobe Target Standard/Premium-Integrationstechniken vertraut machen können.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
translation-type: tm+mt
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 12%

---

# Quick Beginn: Integration von Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium bietet Marketingexperten die Möglichkeit, schnell und kontinuierlich mehrere A/B- und Multivarianz-Tests durchzuführen, die Effektivität zu messen und die Relevanz von Online-Inhalten durch Segmentierung, Targeting und automatisierte Personalisierung zu erhöhen.

Mit Dynamic Media Classic können Sie Angebote und Angebot-Sets für Adobe Target Standard/Premium-Kampagnen erstellen. Sie können beispielsweise einen Angebot-Satz mit drei Varianten desselben Rich-Media-Assets erstellen. Dann können Sie Adobe Target Standard/Premium festlegen, welches Asset eine bessere Konvertierungssteigerung bietet. Sie können Angebote und Angebotssets aus einer einfachen Vorlage oder aus einzelnen Bildern erstellen. Nachdem das Angebot-Set auf Adobe Target Standard/Premium verschoben oder gespeichert wurde, wo die Angebot mit Mboxes und Erlebnissen verknüpft sind, kann Adobe Target Standard/Premium Kampagnen ausführen. Diese Kampagnen bestimmen, welche Variante einer Website für Durchklicks und Konversionen wahrscheinlich am besten geeignet ist.

Verwenden Sie für eine bessere Anpassung dynamischer Dynamic Media Classic-Inhalte Adobe Target Standard/Premium-HTML-Angebot. Weitere Informationen finden Sie in der Produktdokumentation zu [Adobe Target Standard/Premium](https://experienceleague.adobe.com/docs/target.html).

>[!NOTE]
>
>Für die Verwendung von Adobe Target Standard/Premium mit Dynamic Media Classic ist ein gültiges Adobe Target Standard/Premium-Konto erforderlich.

Dieser Quick Beginn hilft Ihnen, sich schnell mit Adobe Target Standard/Premium HTML-Angebot-Sets vertraut zu machen. Führen Sie die Schritte 1 bis 3 aus. Nach jedem Schritt wird auf ein Thema mit weiteren Informationen verwiesen.

## 1. Geben Sie Ihre Adobe Target Standard/Premium-URL auf der Seite &quot;Allgemeine Programmeinstellungen&quot;ein.

Für die Integration mit Adobe Target Standard/Premium benötigt Dynamic Media Classic Ihre Adobe Target Standard/Premium-URL. Kopieren Sie den Teil Ihrer Adobe Target Standard-/Premium-URL bis einschließlich `.com` und geben Sie ihn auf der Seite **[!UICONTROL Allgemeine Programmeinstellungen]** in die Gruppe **[!UICONTROL Server]** ein, **[!UICONTROL Test&amp;Zielgruppe-Servername]**. Siehe [Integration von Dynamic Media Classic mit Adobe Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. Erstellen Sie das Angebotsset.

Verwenden Sie eine parametrisierte Vorlage oder Bilder, um ein Angebotsset zu erstellen. Sie erstellen HTML-Angebot-Sets auf der Seite &quot;Test&amp;Zielgruppe-Angebot-Set&quot;. Um diese Seite zu öffnen, wählen Sie die Vorlage oder die Bilder aus und klicken Sie dann in der Symbolleiste für globale Navigation auf **[!UICONTROL Erstellen]** > **[!UICONTROL Test&amp;Zielgruppe-Angebot-Set]**.

Um ein Angebot mit einer Vorlage zu erstellen, klicken Sie auf **[!UICONTROL Hinzufügen &amp; Vorschau]**. Ändern Sie auf der Seite &quot;Hinzufügen und Vorschau&quot;die Parameterwerte.

Um ein Angebot mit Bildern zu erstellen, ziehen Sie die Bilder auf die Seite &quot;Test&amp;Zielgruppe-Angebot-Set&quot;. Klicken Sie auf **[!UICONTROL Vorschau]** und wählen Sie eine Bildvorgabe für ein Angebot oder alle Bilder im Bildsatz aus.

Speichern Sie das Angebotsset, nachdem Sie es erstellt haben. 

Siehe [Erstellen eines Angebotssets](creating-offer-set.md#creating_an_offer_set).

## 3. Angebot auf Adobe Target Standard/Premium verschieben

Klicken Sie auf der Seite &quot;Test&amp;Zielgruppe-Angebot-Set&quot;auf **[!UICONTROL Push-Angebot]** und geben Sie Ihre Anmeldedaten im Dialogfeld &quot;Test&amp;Zielgruppe-Anmeldung&quot;ein. Siehe [Pushing von Angebot-Sets auf Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
