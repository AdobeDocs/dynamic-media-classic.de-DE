---
title: Festlegen, welche Exportoptionen Media Portal-Benutzern zur Verfügung stehen
description: Erfahren Sie, wie Sie Exportoptionen angeben, die für Media Portal-Benutzer in Adobe Dynamic Media Classic verfügbar sind.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 42%

---

# Festlegen, welche Exportoptionen Media Portal-Benutzern zur Verfügung stehen {#specifying-export-options-available-to-media-portal-users}

Media Portal-Benutzer können Bilder in einem anderen Format exportieren, sofern der Administrator ihnen die erforderlichen Berechtigungen zugewiesen hat. Sie können beispielsweise die Größe, das Dateiformat und die Bildqualität ändern. Ein automatisches Neuformatieren von Bildern während des Exports spart Zeit, da die Bilder nicht separat neu formatiert werden müssen. Darüber hinaus können Administratoren eine Vorgabe erstellen, also eine voreingestellte Auswahl von Formatierungseinstellungen für Bilder. Sie können eine Vorgabe beim Exportieren von Bildern verwenden, um sie entsprechend den Spezifikationen des Unternehmens neu zu formatieren.

Die folgenden beiden Einschränkungen gelten, wenn Sie Bild-Assets über eine benutzerdefinierte Konvertierung exportieren oder wenn Sie Originalbilder exportieren:

* Die komprimierte Zip-Exportdatei kann für den Exportauftrag maximal 1 GB groß sein.
* Sie können maximal 500 Assets pro Exportauftrag haben.

Siehe auch [Exportieren von Assets aus Adobe Dynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**So legen Sie Exportoptionen fest, die für Media Portal-Benutzer verfügbar sind:**

1. Wechseln Sie in der globalen Navigationsleiste zu **[!UICONTROL Einstellungen]** > **[!UICONTROL Bildvorgaben]**.
1. Legen Sie im Fenster „Bildvorgaben“ die folgenden Optionen nach Bedarf fest:

   * **Benutzerdefinierte Konversion aktivieren**: Wenn diese Option aktiviert ist, können Benutzer aus der Dropdownliste **[!UICONTROL Größe]** im Fenster &quot;Ausgewählte Assets exportieren&quot;eine andere Option auswählen. Benutzer können dann eine Maßeinheit wie Pixel oder Zentimeter auswählen und dann die gewünschte Breite und Höhe angeben. Wenn sie diese Dateien exportieren oder herunterladen, werden die Bilddateien neu formatiert.

     Wenn **[!UICONTROL Pixel]** aus der Dropdownliste **[!UICONTROL Größe]** ausgewählt werden, darf die resultierende Bildbreite × Höhe 100 Millionen Pixel nicht überschreiten. Diese Größe entspricht 10.000 × 10.000 Pixel für ein quadratisches Bild oder etwa 8.000 × 12.000 Pixel für ein Seitenverhältnis von 2 x 3. Diese Größenbeschränkung gilt nicht, wenn Sie Originalbilder exportieren.

     Deaktivieren Sie diese Option, damit Benutzer Dateien herunterladen können, ohne sie beim Herunterladen neu zu formatieren.

   * **Original exportieren aktivieren**: Hiermit können Sie Original-Primärbilder exportieren. Im Bedienfeld **[!UICONTROL Ausgewählte Assets exportieren]** können Benutzer das Dropdown-Menü **[!UICONTROL Konversion]** öffnen und **[!UICONTROL Original exportieren]** auswählen, um Originaldateien zu exportieren. Wenn diese Option deaktiviert ist, müssen Benutzer beim Exportieren von Bildern eine Bildvorgabe auswählen oder Konvertierungsoptionen festlegen.

>[!MORELIKETHIS]
>
>* [Bildvorgaben](application-setup.md#image_presets)
>* [Wählen Sie die Bildvorgabe-Zugriffsberechtigungen für eine Gruppe aus](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)
