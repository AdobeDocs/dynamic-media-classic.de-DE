---
title: Verwalten des Ordners „Papierkorb“
description: Erfahren Sie, wie Sie den Ordner "Papierkorb"verwalten.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 60%

---


# Verwalten des Ordners „Papierkorb“{#managing-the-trash-folder}

Elemente, die Sie aus Dynamic Media Classic löschen, werden in den Ordner &quot;Papierkorb&quot;verschoben. Sie bleiben sieben Tage lang in diesem Ordner; während dieser Zeit ist eine Wiederherstellung möglich. Nach Ablauf der sieben Tage werden die Elemente im Papierkorb endgültig gelöscht. Sie können gelöschte Elemente im Ordner „Papierkorb“ anzeigen, indem Sie unten in der Asset-Bibliothek auf das Symbol „Papierkorb“  klicken.

Alle Benutzer können Elemente aus dem Ordner „Papierkorb“ wiederherstellen, sie also wieder in die Ordner übertragen, aus denen sie gelöscht wurden. Alle Benutzer haben außerdem die Möglichkeit, den Ordner „Papierkorb“ zu leeren, also den gesamten Inhalt daraus zu löschen.

Beim Löschen von Elementen aus dem Ordner &quot;Papierkorb&quot;werden Elemente aus Dynamic Media Classic endgültig gelöscht. Elemente, die aus dem Ordner &quot;Papierkorb&quot;gelöscht wurden, können nicht mehr wiederhergestellt werden. Informationen zum Einstellen von Benachrichtigungen für Unternehmensadministratoren bei bevorstehendem automatischem Löschen von Assets aus dem Papierkorb finden Sie im Abschnitt [Allgemeine Programmeinstellungen](application-setup.md#general_settings).

>[!NOTE]
>
>Assets, die in den Ordner &quot;Papierkorb&quot;verschoben wurden, werden weiterhin in Dynamic Media Classic registriert. Wenn Sie versuchen, eine Datei hochzuladen, die denselben Namen wie eine gelöschte Datei im Ordner &quot;Papierkorb&quot;hat, behandelt Dynamic Media Classic das hochzuladende Asset als Duplikat-Asset. Deshalb wird dem Asset-Namen eine Zahl angehängt.

## Ordner „Papierkorb“{#about-the-trash-folder}

Wenn Sie ein Element aus einem Ordner löschen, wird es im Ordner „Papierkorb“ abgelegt. Das Löschen eines Elements mit nachfolgendem Verschieben in den Ordner „Papierkorb“ ist mit folgenden Gegebenheiten bzw. Abläufen verbunden:

* Obwohl das Element aus Ihren Dynamic Media Classic-Ordnern entfernt wurde, kann seine ID keinem anderen Asset zugewiesen werden, solange es sich im Ordner &quot;Papierkorb&quot;befindet. Wenn Sie versuchen, ein Asset mit demselben Namen wie eine Datei im Ordner &quot;Papierkorb&quot;hochzuladen, hängt Dynamic Media Classic eine Ziffer an den Namen des Assets an.
* Das Element kann nicht veröffentlicht werden. Selbst wenn das Element zur Veröffentlichung markiert war, als sie es gelöscht haben, wird es nicht veröffentlicht.
* Das Element bleibt im Ordner „Papierkorb“, bis es wiederhergestellt wird, bis der Befehl „Papierkorb leeren“ gewählt wird oder bis sieben Tage vergangen sind. Nach Ablauf von sieben Tagen wird das Element durch einen automatischen Datenbereinigungsvorgang endgültig gelöscht.

## Wiederherstellen von Assets aus dem Ordner „Papierkorb“  {#restoring-assets-from-the-trash-folder}

Ein Asset lässt sich nicht nur durch die Person wiederherstellen, die das Asset gelöscht hat; jeder Benutzer kann Assets aus dem Ordner „Papierkorb“ wiederherstellen. Wiederhergestellte Assets werden in den Ordnern platziert, aus denen sie zuvor gelöscht wurden. Wenn diese Ordner nicht mehr vorhanden sind, erstellt Dynamic Media Classic sie neu und die wiederhergestellten Assets werden in den neu erstellten Ordnern abgelegt.

Führen Sie zum Wiederherstellen von Assets aus dem Ordner „Papierkorb“ in die Ursprungsordner die folgenden Schritte aus:

1. Klicken Sie auf das Papierkorbsymbol, um den Ordner &quot;Papierkorb&quot;zu öffnen.
1. Wählen Sie die wiederherzustellenden Assets aus.
1. Wählen Sie „Datei“ > „Wiederherstellen“.

## Endgültiges Löschen der Assets im Ordner „Papierkorb“  {#permanently-deleting-assets-in-the-trash-folder}

Wenn Sie Assets aus dem Ordner „Papierkorb“ löschen, werden sie endgültig aus dem System entfernt. Nach Ablauf von sieben Tagen werden Assets automatisch aus dem Ordner „Papierkorb“ gelöscht.

Wenn Sie Assets endgültig aus dem Papierkorb löschen möchten, klicken Sie auf das Papierkorbsymbol , um den Ordner „Papierkorb“ zu öffnen. Dann können Sie einzelne Assets oder alle Assets in diesem Ordner löschen:

* **Löschen einzelner** AssetsWählen Sie die Assets, die Sie endgültig löschen möchten, und klicken Sie auf  **[!UICONTROL &quot;Datei&quot;> &quot;Aus Papierkorb]** löschen&quot;.

* **Löschen aller** AssetsKlicken Sie auf  **[!UICONTROL Datei > Papierkorb]** leeren.

>[!MORELIKETHIS]
>
>* [Löschen von Assets](moving-renaming-deleting-assets.md#delete_assets)

