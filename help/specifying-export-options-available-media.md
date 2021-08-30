---
title: Festlegen, welche Exportoptionen Media Portal-Benutzern zur Verfügung stehen
description: Erfahren Sie, wie Sie Exportoptionen angeben, die für Media Portal-Benutzer in Adobe Dynamic Media Classic verfügbar sind.
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 68%

---

# Festlegen, welche Exportoptionen Media Portal-Benutzern zur Verfügung stehen {#specifying-export-options-available-to-media-portal-users}

Media Portal-Benutzer können Bilder in einem anderen Format exportieren, sofern der Administrator ihnen die erforderlichen Berechtigungen zugewiesen hat. Sie können beispielsweise die Größe, das Dateiformat und die Bildqualität ändern. Ein automatisches Neuformatieren von Bildern während des Exports spart Zeit, da die Bilder nicht separat neu formatiert werden müssen. Darüber hinaus können Administratoren eine Vorgabe erstellen, also eine voreingestellte Auswahl von Formatierungseinstellungen für Bilder. Sie können eine Vorgabe beim Exportieren von Bildern verwenden, um sie entsprechend den Spezifikationen des Unternehmens neu zu formatieren.

Die folgenden beiden Einschränkungen gelten, wenn Sie Bild-Asset über eine benutzerdefinierte Konvertierung exportieren oder wenn Sie Original-Masterbilder exportieren:

* Die komprimierte Zip-Exportdatei kann für den Exportauftrag maximal 1 GB groß sein.
* Sie können maximal 500 Assets pro Exportauftrag haben.

Siehe auch [Exportieren von Assets aus Adobe Dynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**So legen Sie Exportoptionen fest, die für Media Portal-Benutzer verfügbar sind:**

1. Navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Setup]** > **[!UICONTROL Bildvorgaben]**.
1. Legen Sie im Fenster „Bildvorgaben“ die folgenden Optionen nach Bedarf fest:

   * **Benutzerdefinierte Konversion aktivieren**  - Wenn diese Option aktiviert ist, können Benutzer aus der Dropdown-Liste  **** Größe im Fenster Ausgewählte Assets exportieren andere Optionen auswählen. Benutzer können dann eine Maßeinheit wie Pixel oder Zentimeter wählen und die gewünschte Breite und Höhe festlegen. Wenn sie diese Dateien exportieren oder herunterladen, werden die Bilddateien neu formatiert.

      Wenn in der Dropdownliste **[!UICONTROL Größe]** der Wert **[!UICONTROL Pixel]** ausgewählt wird, kann die resultierende Bildhöhe x Bildbreite maximal 100 Millionen Pixel betragen. Diese Größe entspricht 10.000 x 10.000 Pixel bei einem quadratischen Bild bzw. etwa 8.000 x 12.000 Pixel bei einem Seitenverhältnis von 2:3. Diese Größenbeschränkung gilt nicht, wenn Sie Original-Masterbilder exportieren.

      Wenn diese Option deaktiviert ist, können Benutzer nur Dateien herunterladen, ohne sie dabei neu zu formatieren.

   * **Original exportieren**  aktivieren - Ermöglicht den Export Übergeordneter Originalbilder. Im Bedienfeld **[!UICONTROL Ausgewählte Assets exportieren]** können Benutzer das Dropdown-Menü **[!UICONTROL Konversion]** öffnen und **[!UICONTROL Original exportieren]** auswählen, um Originaldateien zu exportieren. Deaktivieren Sie diese Option, wenn Sie Benutzer zwingen möchten, eine Bildvorgabe auszuwählen oder beim Exportieren von Bildern Konvertierungsoptionen auszuwählen.

>[!MORELIKETHIS]
>
>* [Bildvorgaben](application-setup.md#image_presets)
>* [Auswählen der Bildvorgabezugriffsberechtigungen für eine Gruppe](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

