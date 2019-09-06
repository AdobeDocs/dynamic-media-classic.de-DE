---
title: Festlegen von Exportoptionen für Media Portal-Benutzer
seo-title: Festlegen von Exportoptionen für Media Portal-Benutzer
description: 'null'
seo-description: Hier erfahren Sie, wie Sie für Media Portal-Benutzer verfügbare Exportoptionen festlegen.
uuid: 5258 b 8 a 4-0704-43 cd -97 d 1-c 9 af 2 e 4 e 298 b
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 9 bfd 95 da -3714-4 e 38-98 af -331 a 04 c 685 f 5
translation-type: tm+mt
source-git-commit: 0f6c8e6ac69e29aab7a48425aab76c10170d9ddf

---


# Festlegen, welche Exportoptionen Media Portal-Benutzern zur Verfügung stehen {#specifying-export-options-available-to-media-portal-users}

Media Portal-Benutzer können Bilder in einem anderen Format exportieren, sofern der Administrator ihnen die erforderlichen Berechtigungen zugewiesen hat. Sie können beispielsweise die Größe, das Dateiformat und die Bildqualität ändern. Ein automatisches Neuformatieren von Bildern während des Exports spart Zeit, da die Bilder nicht separat neu formatiert werden müssen. Darüber hinaus können Administratoren eine Vorgabe erstellen, also eine voreingestellte Auswahl von Formatierungseinstellungen für Bilder. Sie können eine Vorgabe beim Exportieren von Bildern verwenden, um sie entsprechend den Spezifikationen des Unternehmens neu zu formatieren.

Die folgenden beiden Einschränkungen gelten, wenn Sie Bild-Asset über eine benutzerdefinierte Konvertierung exportieren oder wenn Sie Original-Masterbilder exportieren:

* Die komprimierte Zip-Exportdatei kann für den Exportauftrag maximal 1 GB groß sein.
* Sie können maximal 500 Assets pro Exportauftrag haben.

Siehe auch [Exportieren von Assets aus Scene7 Publishing System](exporting-assets-scene7-publishing-system.md#exporting_assets_from_scene7_publishing_system)

**So legen Sie fest, welche Exportoptionen Media Portal-Benutzern zur Verfügung stehen**.

1. Klicken Sie auf **„Einstellungen“** &gt; **„Bildvorgaben“**.
1. Legen Sie im Fenster „Bildvorgaben“ die folgenden Optionen nach Bedarf fest:

   **Benutzerdefinierte Konvertierung aktivieren** Wenn diese Option aktiviert ist, können Benutzer im Fenster "Ausgewählte Assets exportieren" aus der Dropdownliste" Größe" andere auswählen. Benutzer können dann eine Maßeinheit wie Pixel oder Zentimeter wählen und die gewünschte Breite und Höhe festlegen. Wenn sie diese Dateien exportieren oder herunterladen, werden die Bilddateien neu formatiert.

   Wenn in der Dropdownliste **Größe** der Wert **Pixel** ausgewählt wird, kann die resultierende Bildhöhe x Bildbreite maximal 100 Millionen Pixel betragen. Diese Größe entspricht 10.000 x 10.000 Pixel bei einem quadratischen Bild bzw. etwa 8.000 x 12.000 Pixel bei einem Seitenverhältnis von 2:3. Diese Größenbeschränkung gilt nicht, wenn Sie Original-Masterbilder exportieren.

   Wenn diese Option deaktiviert ist, können Benutzer nur Dateien herunterladen, ohne sie dabei neu zu formatieren.

   **Export Original** aktivieren Sie exportieren Original-Masterbilder. Im Bedienfeld „Ausgewählte Assets exportieren“ können Benutzer das Dropdown-Menü Konvertierung öffnen und Original exportieren auswählen, um Originaldateien zu exportieren. Wenn diese Option deaktiviert ist, müssen Benutzer beim Exportieren von Bildern eine Bildvorgabe auswählen oder Konvertierungsoptionen festlegen.

>[!MORELIKETHIS]
>
>* [Bildvorgaben](application-setup.md#image_presets)
>* [Auswählen der Bildvorgabezugriffsberechtigungen für eine Gruppe](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)
