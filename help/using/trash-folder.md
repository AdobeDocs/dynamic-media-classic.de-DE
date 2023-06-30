---
title: Ordner "Papierkorb"verwalten
description: Erfahren Sie, wie Sie den Ordner "Papierkorb"verwalten.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 31%

---

# Ordner &quot;Papierkorb&quot;verwalten{#managing-the-trash-folder}

Elemente, die Sie aus Adobe Dynamic Media Classic löschen, werden in den Ordner Papierkorb verschoben. Die gelöschten bleiben sieben Tage in diesem Ordner, bis sie wiederhergestellt oder dauerhaft gelöscht werden. Sie können gelöschte Elemente untersuchen, indem Sie auf **[!UICONTROL Papierkorb]** -Symbol unten in der Asset-Bibliothek und Anzeigen von Elementen auf der Ordnerseite &quot;Papierkorb&quot;.

Alle Benutzer können Elemente aus dem Ordner „Papierkorb“ wiederherstellen, sie also wieder in die Ordner übertragen, aus denen sie gelöscht wurden. Alle Benutzer haben außerdem die Möglichkeit, den Ordner „Papierkorb“ zu leeren, also den gesamten Inhalt daraus zu löschen.

Beim Löschen von Elementen aus dem Ordner &quot;Papierkorb&quot;werden Elemente dauerhaft aus Adobe Dynamic Media Classic gelöscht. Aus dem Ordner &quot;Papierkorb&quot;gelöschte Elemente können nicht mehr wiederhergestellt werden. Informationen zum Einstellen von Benachrichtigungen für Unternehmensadministratoren bei bevorstehendem automatischem Löschen von Assets aus dem Papierkorb finden Sie im Abschnitt [Allgemeine Programmeinstellungen](application-setup.md#general_settings).

>[!NOTE]
>
>Assets, die in den Ordner Papierkorb verschoben wurden, werden weiterhin in Adobe Dynamic Media Classic registriert. Wenn Sie versuchen, eine Datei hochzuladen, die denselben Namen wie eine gelöschte Datei im Ordner &quot;Papierkorb&quot;hat, behandelt Adobe Dynamic Media Classic das Asset, das Sie hochladen möchten, als doppeltes Asset. Deshalb wird dem Asset-Namen eine Zahl angehängt.

## Ordner „Papierkorb“ {#about-the-trash-folder}

Wenn Sie ein Element aus einem Ordner löschen, wird es im Ordner „Papierkorb“ abgelegt. Das Löschen eines Elements mit nachfolgendem Verschieben in den Ordner „Papierkorb“ ist mit folgenden Gegebenheiten bzw. Abläufen verbunden:

* Obwohl das Element aus Ihren Adobe Dynamic Media Classic-Ordnern entfernt wurde, kann seine ID keinem anderen Asset zugewiesen werden, während es im Ordner &quot;Papierkorb&quot;verbleibt. Wenn Sie versuchen, ein Asset mit demselben Namen wie eine Datei im Ordner &quot;Papierkorb&quot;hochzuladen, hängt Adobe Dynamic Media Classic eine Ziffer an den Namen des Assets an.
* Das Element kann nicht veröffentlicht werden. Selbst wenn das Element zur Veröffentlichung markiert war, als sie es gelöscht haben, wird es nicht veröffentlicht.
* Das Element verbleibt im Ordner &quot;Papierkorb&quot;, bis es wiederhergestellt wird, sieben Tage vergangen ist oder jemand die Option **[!UICONTROL Löschen des Papierkorbs]** Befehl. Nach Ablauf von sieben Tagen wird das Element durch einen automatischen Datenbereinigungsvorgang endgültig gelöscht.

## Wiederherstellen von Assets aus dem Ordner &quot;Papierkorb&quot; {#restoring-assets-from-the-trash-folder}

Es ist nicht erforderlich, dass die Person, die ein Asset gelöscht hat, es wiederherstellt. Jeder kann Assets aus dem Ordner &quot;Papierkorb&quot;wiederherstellen. Wiederhergestellte Assets werden in den Ordnern platziert, aus denen sie zuvor gelöscht wurden. Wenn diese Ordner nicht mehr vorhanden sind, erstellt Adobe Dynamic Media Classic sie neu und die wiederhergestellten Assets werden in den neu erstellten Ordnern abgelegt.

Gehen Sie wie folgt vor, um Assets aus dem Ordner &quot;Papierkorb&quot;in den Ordnern wiederherzustellen, aus denen sie gelöscht wurden:

1. Wählen Sie unten im Bedienfeld &quot;Asset-Bibliothek&quot;die **[!UICONTROL Papierkorb]** -Symbol, um den Ordner Papierkorb zu öffnen.
1. Wählen Sie die Assets aus, die Sie wiederherstellen möchten.
1. Navigieren Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Aus Müll wiederherstellen]**.

## Endgültiges Löschen der Assets im Ordner „Papierkorb“ {#permanently-deleting-assets-in-the-trash-folder}

Wenn Sie Assets aus dem Ordner „Papierkorb“ löschen, werden sie endgültig aus dem System entfernt. Nach Ablauf von sieben Tagen werden Assets automatisch aus dem Ordner „Papierkorb“ gelöscht.

Um Assets dauerhaft aus dem Ordner &quot;Papierkorb&quot;zu löschen, wählen Sie die **[!UICONTROL Papierkorb]** Symbol. Führen Sie auf der Ordnerseite Papierkorb einen der folgenden Schritte aus:

* **Löschen einzelner Assets** - Wählen Sie die Assets aus, die Sie dauerhaft löschen möchten, und navigieren Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Aus Müll löschen]**.

* **Löschen aller Assets** - Gehen Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Leerer Papierkorb]**.

>[!MORELIKETHIS]
>
>* [Löschen von Assets](moving-renaming-deleting-assets.md#delete_assets)
