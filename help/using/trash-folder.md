---
title: Papierkorb-Ordner verwalten
description: Erfahren Sie, wie Sie den Papierkorb-Ordner verwalten.
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

# Papierkorb-Ordner verwalten{#managing-the-trash-folder}

Elemente, die Sie aus Adobe Dynamic Media Classic löschen, werden in den Papierkorb-Ordner verschoben. Diese gelöschten Elemente bleiben sieben Tage lang in diesem Ordner, bis sie wiederhergestellt oder dauerhaft gelöscht werden. Sie können gelöschte Elemente untersuchen, indem Sie auf das **[!UICONTROL Papierkorb]**-Symbol unten in der Asset-Bibliothek klicken und Elemente auf der Papierkorb-Ordnerseite anzeigen.

Alle Benutzer können Elemente aus dem Ordner „Papierkorb“ wiederherstellen, sie also wieder in die Ordner übertragen, aus denen sie gelöscht wurden. Alle Benutzer haben außerdem die Möglichkeit, den Ordner „Papierkorb“ zu leeren, also den gesamten Inhalt daraus zu löschen.

Durch das Löschen von Elementen aus dem Papierkorb-Ordner werden Elemente dauerhaft aus Adobe Dynamic Media Classic gelöscht. Aus dem Papierkorb-Ordner gelöschte Elemente können nicht mehr wiederhergestellt werden. Informationen zum Einstellen von Benachrichtigungen für Unternehmensadministratoren bei bevorstehendem automatischem Löschen von Assets aus dem Papierkorb finden Sie im Abschnitt [Allgemeine Programmeinstellungen](application-setup.md#general_settings).

>[!NOTE]
>
>Assets, die in den Papierkorb-Ordner verschoben wurden, sind weiterhin in Adobe Dynamic Media Classic registriert. Angenommen, Sie versuchen, eine Datei mit demselben Namen wie eine gelöschte Datei im Papierkorb-Ordner hochzuladen. Adobe Dynamic Media Classic behandelt das Asset, das Sie hochladen möchten, als doppeltes Asset. In diesem Fall wird eine Nummer an den Namen angehängt.

## Ordner „Papierkorb“ {#about-the-trash-folder}

Wenn Sie ein Element aus einem Ordner löschen, wird es im Ordner „Papierkorb“ abgelegt. Das Löschen eines Elements mit nachfolgendem Verschieben in den Ordner „Papierkorb“ ist mit folgenden Gegebenheiten bzw. Abläufen verbunden:

* Obwohl das Element aus Ihrem Adobe Dynamic Media Classic-Ordner entfernt wurde, kann seine ID keinem anderen Asset zugewiesen werden, solange es im Papierkorb-Ordner verbleibt. Wenn Sie versuchen, ein Asset mit demselben Namen wie eine Datei im Papierkorb-Ordner hochzuladen, fügt Adobe Dynamic Media Classic eine Zahl an den Namen des Assets an.
* Das Element kann nicht veröffentlicht werden. Selbst wenn das Element zur Veröffentlichung markiert war, als sie es gelöscht haben, wird es nicht veröffentlicht.
* Das Element verbleibt im Papierkorb-Ordner, bis es wiederhergestellt wird, sieben Tage vergehen oder jemand den Befehl **[!UICONTROL Leeren des Papierkorbs]** auswählt. Nach Ablauf von sieben Tagen wird das Element durch einen automatischen Datenbereinigungsvorgang endgültig gelöscht.

## Wiederherstellen von Assets aus dem Papierkorb-Ordner {#restoring-assets-from-the-trash-folder}

Die Person, die ein Asset gelöscht hat, muss es nicht wiederherstellen. Jeder kann Assets aus dem Papierkorb-Ordner wiederherstellen. Wiederhergestellte Assets werden in den Ordnern platziert, aus denen sie zuvor gelöscht wurden. Wenn diese Ordner nicht mehr vorhanden sind, erstellt Adobe Dynamic Media Classic sie neu, und die wiederhergestellten Assets werden in den neu erstellten Ordnern platziert.

Gehen Sie wie folgt vor, um Assets aus dem Papierkorb-Ordner in den Ordnern wiederherzustellen, aus denen sie gelöscht wurden:

1. Klicken Sie unten im Bedienfeld „Asset-Bibliothek“ auf das Symbol **[!UICONTROL Papierkorb]**, um den Papierkorb-Ordner zu öffnen.
1. Wählen Sie das Asset bzw. die Assets aus, die Sie wiederherstellen möchten.
1. Navigieren Sie **[!UICONTROL Datei]** > **[!UICONTROL Aus Papierkorb wiederherstellen]**.

## Endgültiges Löschen der Assets im Ordner „Papierkorb“ {#permanently-deleting-assets-in-the-trash-folder}

Wenn Sie Assets aus dem Ordner „Papierkorb“ löschen, werden sie endgültig aus dem System entfernt. Nach Ablauf von sieben Tagen werden Assets automatisch aus dem Ordner „Papierkorb“ gelöscht.

Sie können Assets dauerhaft aus dem Papierkorb-Ordner löschen, indem Sie auf das Symbol **[!UICONTROL Papierkorb]** klicken. Führen Sie auf der Seite Papierkorb-Ordner einen der folgenden Schritte aus:

* **Löschen einzelner Assets**: Sie können Assets dauerhaft löschen. Wählen Sie die gewünschten Assets aus und klicken Sie dann auf **[!UICONTROL Datei]** > **[!UICONTROL Leer aus Papierkorb]**.

* **Alle Assets löschen**: Navigieren Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Leerer Papierkorb]**.

>[!MORELIKETHIS]
>
>* [Assets löschen](moving-renaming-deleting-assets.md#delete_assets)
