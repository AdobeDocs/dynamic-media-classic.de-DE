---
title: Verwalten des Ordners „Papierkorb“
seo-title: Verwalten des Ordners „Papierkorb“
description: 'null'
seo-description: Erfahren Sie, wie Sie den Ordner "Papierkorb"verwalten.
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: Verweis
products: SG_EXPERIENCEMANAGER/Dynamic Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Verwalten des Ordners „Papierkorb“{#managing-the-trash-folder}

Elemente, die Sie aus dem Scene7 Publishing System löschen, werden in den Ordner „Papierkorb“ verschoben. Sie bleiben sieben Tage lang in diesem Ordner; während dieser Zeit ist eine Wiederherstellung möglich. Nach Ablauf der sieben Tage werden die Elemente im Papierkorb endgültig gelöscht. Sie können gelöschte Elemente im Ordner „Papierkorb“ anzeigen, indem Sie unten in der Asset-Bibliothek auf das Symbol „Papierkorb“  klicken.

Alle Benutzer können Elemente aus dem Ordner „Papierkorb“ wiederherstellen, sie also wieder in die Ordner übertragen, aus denen sie gelöscht wurden. Alle Benutzer haben außerdem die Möglichkeit, den Ordner „Papierkorb“ zu leeren, also den gesamten Inhalt daraus zu löschen.

Durch das Entfernen der Elemente aus dem Ordner „Papierkorb“ werden die Elemente endgültig aus dem Scene7 Publishing System gelöscht; eine Wiederherstellung der Elemente ist danach nicht mehr möglich. Informationen zum Einstellen von Benachrichtigungen für Unternehmensadministratoren bei bevorstehendem automatischem Löschen von Assets aus dem Papierkorb finden Sie im Abschnitt [Allgemeine Programmeinstellungen](application-setup.md#general_settings).

>[!NOTE]
>
>Assets, die in den Ordner „Papierkorb“ verschoben wurden, sind immer noch beim Scene7 Publishing System registriert. Wenn Sie versuchen, eine Datei hochzuladen, die denselben Namen wie eine gelöschte Datei im Ordner "Papierkorb"hat, behandelt Dynamic Media Classic das hochzuladende Asset als doppeltes Asset. Deshalb wird dem Asset-Namen eine Zahl angehängt.

## Ordner „Papierkorb“{#about-the-trash-folder}

Wenn Sie ein Element aus einem Ordner löschen, wird es im Ordner „Papierkorb“ abgelegt. Das Löschen eines Elements mit nachfolgendem Verschieben in den Ordner „Papierkorb“ ist mit folgenden Gegebenheiten bzw. Abläufen verbunden:

* Obwohl das Element aus Ihren Scene7 Publishing System-Ordnern entfernt wurde, kann seine ID keinem anderen Asset zugewiesen werden, solange sich das Element im Ordner „Papierkorb“ befindet. Wenn Sie versuchen, ein Asset mit demselben Namen wie eine Datei im Ordner "Papierkorb"hochzuladen, hängt Dynamic Media Classic eine Ziffer an den Namen des Assets an.
* Das Element kann nicht veröffentlicht werden. Selbst wenn das Element zur Veröffentlichung markiert war, als sie es gelöscht haben, wird es nicht veröffentlicht.
* Das Element bleibt im Ordner „Papierkorb“, bis es wiederhergestellt wird, bis der Befehl „Papierkorb leeren“ gewählt wird oder bis sieben Tage vergangen sind. Nach Ablauf von sieben Tagen wird das Element durch einen automatischen Datenbereinigungsvorgang endgültig gelöscht.

## Wiederherstellen von Assets aus dem Ordner „Papierkorb“ {#restoring-assets-from-the-trash-folder}

Ein Asset lässt sich nicht nur durch die Person wiederherstellen, die das Asset gelöscht hat; jeder Benutzer kann Assets aus dem Ordner „Papierkorb“ wiederherstellen. Wiederhergestellte Assets werden in den Ordnern platziert, aus denen sie zuvor gelöscht wurden. Sollten diese Ordner nicht mehr vorhanden sein, werden sie vom Scene7 Publishing System neu erstellt; danach werden die wiederhergestellten Assets in den erneut erstellten Ordnern abgelegt.

Führen Sie zum Wiederherstellen von Assets aus dem Ordner „Papierkorb“ in die Ursprungsordner die folgenden Schritte aus:

1. Klicken Sie auf das Papierkorbsymbol, um den Ordner "Papierkorb"zu öffnen.
1. Wählen Sie die wiederherzustellenden Assets aus.
1. Wählen Sie „Datei“ &gt; „Wiederherstellen“.

## Endgültiges Löschen der Assets im Ordner „Papierkorb“ {#permanently-deleting-assets-in-the-trash-folder}

Wenn Sie Assets aus dem Ordner „Papierkorb“ löschen, werden sie endgültig aus dem System entfernt. Nach Ablauf von sieben Tagen werden Assets automatisch aus dem Ordner „Papierkorb“ gelöscht.

Wenn Sie Assets endgültig aus dem Papierkorb löschen möchten, klicken Sie auf das Papierkorbsymbol , um den Ordner „Papierkorb“ zu öffnen. Dann können Sie einzelne Assets oder alle Assets in diesem Ordner löschen:

* **Löschen einzelner Assets** Wählen Sie die Assets, die Sie endgültig löschen möchten, und klicken Sie auf **[!UICONTROL "Datei"&gt; "Aus Papierkorb]** löschen".

* **Löschen aller Assets** Klicken Sie auf **[!UICONTROL Datei &gt; Papierkorb]** leeren.

>[!MORELIKETHIS]
>
>* [Löschen von Assets](moving-renaming-deleting-assets.md#delete_assets)

