---
title: '"Beginn: Integration von Target Standard/Premium"'
seo-title: '"Beginn: Integration von Target Standard/Premium"'
description: 'null'
seo-description: Eine Einführung und ein kurzer Beginn zu Adobe Target Standard/Premium, mit dem Sie sich schnell mit den Integrationstechniken von Target Standard/Premium vertraut machen können.
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 19%

---


# Quick Beginn: Integration mit Adobe Target Standard/Premium{#quick-start-target-integration}

Adobe Target Standard/Premium bietet Marketingexperten die Möglichkeit, schnell und kontinuierlich mehrere A/B- und Multivarianz-Tests durchzuführen, die Effektivität zu messen und die Relevanz von Online-Inhalten durch Segmentierung, Targeting und automatisierte Personalisierung zu erhöhen.

Mit Dynamic Media Classic können Sie Angebot und Angebot-Sets für Target Standard/Premium-Kampagnen erstellen. Sie können beispielsweise einen Angebot-Satz mit drei Varianten desselben Rich-Media-Assets erstellen. Anschließend können Sie Target Standard/Premium bestimmen lassen, welches Asset eine bessere Konvertierungssteigerung bietet. Sie können Angebote und Angebotssets aus einer einfachen Vorlage oder aus einzelnen Bildern erstellen. Nachdem der Angebot-Satz an Adobe Target Standard/Premium weitergeleitet oder gespeichert wurde, wo die Angebot mit Mboxes und Erlebnissen verknüpft sind, kann Target Standard/Premium Kampagnen ausführen, um festzustellen, welche Variante einer Website für Durchklicks und Konversionen am besten geeignet ist.

Verwenden Sie für eine bessere Anpassung dynamischer Inhalte aus dem Classic-Bereich Target Standard/Premium-HTML-Angebot. Weitere Informationen finden Sie in der Produktdokumentation zu Target Standard/Premium.

>[!NOTE]
>
>Für die Verwendung von Target Standard/Premium mit Dynamic Media Classic ist ein gültiges Adobe Target Standard/Premium-Konto erforderlich.

**Quick Beginn**

Dieser Quick Beginn hilft Ihnen, sich schnell mit HTML-Angebot-Sets von Target Standard/Premium vertraut zu machen. Führen Sie die Schritte 1 bis 3 aus. Nach jedem Schritt wird auf ein Thema mit weiteren Informationen verwiesen.

**1. Enter your Adobe Target Standard/Premium URL in the Application General Settings screen.**

Für die Integration in Target Standard/Premium benötigt Dynamic Media Classic Ihre Target Standard/Premium-URL. Copy the portion of your Target Standard/Premium URL up to and including *.com*, and enter it in the Dynamic Media Classic Application General Settings screen. Siehe [Integration von Dynamic Media Classic mit Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target).

**2. Erstellen Sie das Angebotsset.**

Verwenden Sie eine parametrisierte Vorlage oder Bilder, um ein Angebotsset zu erstellen. Sie erstellen HTML-Angebotssets im Anzeigebereich „Test&amp;Target-Angebotsset“. To open this screen, select your template or images, and click **Build** > **Test&amp;Target Offer Set**.

Um ein Angebot mit einer Vorlage zu erstellen, klicken Sie auf **Hinzufügen und Vorschau**. Ändern Sie im Bildschirm &quot;Hinzufügen und Vorschau&quot;die Parameterwerte.

Um ein Angebot mit Bildern zu erstellen, ziehen Sie Bilder in den Anzeigebereich „Test&amp;Target-Angebotsset“. Click **Preview** to choose an Image Preset for an image or all the images in the offer set.

Speichern Sie das Angebotsset, nachdem Sie es erstellt haben. 

Siehe [Erstellen eines Angebotssets](creating-offer-set.md#creating_an_offer_set).

**3. Angebot auf Adobe Target Standard/Premium verschieben**

In the Test&amp;Target Offer Set screen, click **Push Offers**, and enter your login credentials in the Test&amp;Target Login dialog box. Siehe [Pushing von Angebot-Sets zu Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
