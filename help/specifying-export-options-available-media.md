---
title: Festlegen, welche Exportoptionen Media Portal-Benutzern zur Verfügung stehen
description: Hier erfahren Sie, wie Sie Exportoptionen festlegen, die Media Portal-Benutzern zur Verfügung stehen.
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
feature: Dynamic Media Classic, Zusammenarbeit, Asset Management
role: Administrator, Geschäftspraktiker
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 81%

---


# Festlegen, welche Exportoptionen Media Portal-Benutzern zur Verfügung stehen {#specifying-export-options-available-to-media-portal-users}

Media Portal-Benutzer können Bilder in einem anderen Format exportieren, sofern der Administrator ihnen die erforderlichen Berechtigungen zugewiesen hat. Sie können beispielsweise die Größe, das Dateiformat und die Bildqualität ändern. Ein automatisches Neuformatieren von Bildern während des Exports spart Zeit, da die Bilder nicht separat neu formatiert werden müssen. Darüber hinaus können Administratoren eine Vorgabe erstellen, also eine voreingestellte Auswahl von Formatierungseinstellungen für Bilder. Sie können eine Vorgabe beim Exportieren von Bildern verwenden, um sie entsprechend den Spezifikationen des Unternehmens neu zu formatieren.

Die folgenden beiden Einschränkungen gelten, wenn Sie Bild-Asset über eine benutzerdefinierte Konvertierung exportieren oder wenn Sie Original-Masterbilder exportieren:

* Die komprimierte Zip-Exportdatei kann für den Exportauftrag maximal 1 GB groß sein.
* Sie können maximal 500 Assets pro Exportauftrag haben.

Siehe auch [Exportieren von Assets aus Dynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**So legen Sie fest, welche Exportoptionen Media Portal-Benutzern zur Verfügung stehen**.

1. Klicken Sie auf **„Einstellungen“** > **„Bildvorgaben“**.
1. Legen Sie im Fenster „Bildvorgaben“ die folgenden Optionen nach Bedarf fest:

   * **Benutzerdefinierte**
Konversion aktivieren Wenn diese Option aktiviert ist, können Benutzer im Fenster &quot;Ausgewählte Assets exportieren&quot;aus der Dropdown-Liste &quot;Größe&quot;eine andere Option auswählen. Benutzer können dann eine Maßeinheit wie Pixel oder Zentimeter wählen und die gewünschte Breite und Höhe festlegen. Wenn sie diese Dateien exportieren oder herunterladen, werden die Bilddateien neu formatiert.

      Wenn in der Dropdownliste **Größe** der Wert **Pixel** ausgewählt wird, kann die resultierende Bildhöhe x Bildbreite maximal 100 Millionen Pixel betragen. Diese Größe entspricht 10.000 x 10.000 Pixel bei einem quadratischen Bild bzw. etwa 8.000 x 12.000 Pixel bei einem Seitenverhältnis von 2:3. Diese Größenbeschränkung gilt nicht, wenn Sie Original-Masterbilder exportieren.

      Wenn diese Option deaktiviert ist, können Benutzer nur Dateien herunterladen, ohne sie dabei neu zu formatieren.

   * **Aktivieren Sie &quot;**
Original exportieren&quot;Ermöglicht den Export von Übergeordnet-Originalbildern. Im Bedienfeld „Ausgewählte Assets exportieren“ können Benutzer das Dropdown-Menü Konvertierung öffnen und Original exportieren auswählen, um Originaldateien zu exportieren. Wenn diese Option deaktiviert ist, müssen Benutzer beim Exportieren von Bildern eine Bildvorgabe auswählen oder Konvertierungsoptionen festlegen.

>[!MORELIKETHIS]
>
>* [Bildvorgaben](application-setup.md#image_presets)
>* [Auswählen der Bildvorgabezugriffsberechtigungen für eine Gruppe](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

