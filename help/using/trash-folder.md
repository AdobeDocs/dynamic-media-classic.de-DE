---
title: Ordner "Papierkorb"verwalten
description: Erfahren Sie, wie Sie den Ordner "Papierkorb"verwalten.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 28%

---

# Ordner &quot;Papierkorb&quot;verwalten{#managing-the-trash-folder}

Elemente, die Sie aus Adobe Dynamic Media Classic löschen, werden in den Ordner &quot;Papierkorb&quot;verschoben. Diese gelöschten Elemente bleiben sieben Tage in diesem Ordner, bis sie wiederhergestellt oder dauerhaft gelöscht werden. Sie können gelöschte Elemente untersuchen, indem Sie unten in der Asset-Bibliothek das Symbol &quot;**[!UICONTROL Papierkorb]**&quot;auswählen und Elemente auf der Ordnerseite &quot;Papierkorb&quot;anzeigen.

Alle Benutzer können Elemente aus dem Ordner „Papierkorb“ wiederherstellen, sie also wieder in die Ordner übertragen, aus denen sie gelöscht wurden. Alle Benutzer haben außerdem die Möglichkeit, den Ordner „Papierkorb“ zu leeren, also den gesamten Inhalt daraus zu löschen.

Beim Löschen von Elementen aus dem Ordner &quot;Papierkorb&quot;werden Elemente dauerhaft aus Adobe Dynamic Media Classic gelöscht. Aus dem Ordner &quot;Papierkorb&quot;gelöschte Elemente können nicht mehr wiederhergestellt werden. Informationen zum Einstellen von Benachrichtigungen für Unternehmensadministratoren bei bevorstehendem automatischem Löschen von Assets aus dem Papierkorb finden Sie im Abschnitt [Allgemeine Programmeinstellungen](application-setup.md#general_settings).

>[!NOTE]
>
>Assets, die in den Ordner Papierkorb verschoben wurden, sind weiterhin in Adobe Dynamic Media Classic registriert. Angenommen, Sie versuchen, eine Datei hochzuladen, die denselben Namen wie eine gelöschte Datei im Ordner &quot;Papierkorb&quot;hat. Adobe Dynamic Media Classic behandelt das Asset, das Sie hochladen möchten, als doppeltes Asset. In diesem Fall wird eine Zahl an den Namen angehängt.

## Ordner „Papierkorb“ {#about-the-trash-folder}

Wenn Sie ein Element aus einem Ordner löschen, wird es im Ordner „Papierkorb“ abgelegt. Das Löschen eines Elements mit nachfolgendem Verschieben in den Ordner „Papierkorb“ ist mit folgenden Gegebenheiten bzw. Abläufen verbunden:

* Obwohl das Element aus Ihrem Adobe Dynamic Media Classic-Ordner entfernt wird, kann seine ID keinem anderen Asset zugewiesen werden, solange es sich noch im Ordner &quot;Papierkorb&quot;befindet. Wenn Sie versuchen, ein Asset mit demselben Namen wie eine Datei im Ordner &quot;Papierkorb&quot;hochzuladen, hängt Adobe Dynamic Media Classic eine Ziffer an den Namen des Assets an.
* Das Element kann nicht veröffentlicht werden. Selbst wenn das Element zur Veröffentlichung markiert war, als sie es gelöscht haben, wird es nicht veröffentlicht.
* Das Element verbleibt im Ordner &quot;Papierkorb&quot;, bis es wiederhergestellt wird, sieben Tage vergangen ist oder jemand den Befehl &quot;**[!UICONTROL Den Papierkorb leeren]**&quot; auswählt. Nach Ablauf von sieben Tagen wird das Element durch einen automatischen Datenbereinigungsvorgang endgültig gelöscht.

## Wiederherstellen von Assets aus dem Ordner Papierkorb {#restoring-assets-from-the-trash-folder}

Es ist nicht erforderlich, dass die Person, die ein Asset gelöscht hat, es wiederherstellt. Jeder kann Assets aus dem Ordner &quot;Papierkorb&quot;wiederherstellen. Wiederhergestellte Assets werden in den Ordnern platziert, aus denen sie zuvor gelöscht wurden. Wenn diese Ordner nicht mehr vorhanden sind, erstellt Adobe Dynamic Media Classic sie neu und die wiederhergestellten Assets werden in den neu erstellten Ordnern abgelegt.

Gehen Sie wie folgt vor, um Assets aus dem Ordner &quot;Papierkorb&quot;in den Ordnern wiederherzustellen, aus denen sie gelöscht wurden:

1. Wählen Sie unten im Bedienfeld &quot;Asset-Bibliothek&quot;das Symbol **[!UICONTROL Papierkorb]** aus, um den Ordner &quot;Papierkorb&quot;zu öffnen.
1. Wählen Sie die Assets aus, die Sie wiederherstellen möchten.
1. Wechseln Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Aus Papierkorb wiederherstellen]**.

## Endgültiges Löschen der Assets im Ordner „Papierkorb“ {#permanently-deleting-assets-in-the-trash-folder}

Wenn Sie Assets aus dem Ordner „Papierkorb“ löschen, werden sie endgültig aus dem System entfernt. Nach Ablauf von sieben Tagen werden Assets automatisch aus dem Ordner „Papierkorb“ gelöscht.

Sie können Assets dauerhaft aus dem Ordner &quot;Papierkorb&quot;löschen, indem Sie auf das Symbol **[!UICONTROL Papierkorb]** klicken. Führen Sie auf der Ordnerseite Papierkorb einen der folgenden Schritte aus:

* **Löschen einzelner Assets**: Sie können Assets dauerhaft löschen. Wählen Sie die gewünschten Assets aus und klicken Sie dann auf **[!UICONTROL Datei]** > **[!UICONTROL Leer aus Papierkorb]**.

* **Löschen aller Assets**: Wechseln Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Leerer Papierkorb]**.

>[!MORELIKETHIS]
>
>* [Löschen von Assets](moving-renaming-deleting-assets.md#delete_assets)
