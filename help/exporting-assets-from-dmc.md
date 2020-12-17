---
title: Exportieren von Assets aus Dynamic Media Classic
seo-title: Exportieren von Assets aus Dynamic Media Classic
description: 'null'
seo-description: Erfahren Sie, wie Sie Assets aus Dynamic Media Classic exportieren.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 69%

---


# Exportieren von Assets aus Dynamic Media Classic{#exporting-assets-from-dmc}

Sie können Assets, die Sie in Dynamic Media Classic bearbeitet haben, auf einem lokalen Netzlaufwerk speichern. Exportierte Assets werden zum Herunterladen oder Senden per E-Mail in einer ZIP-Datei zusammengestellt.

Die komprimierte Zip-Datei kann für den Exportauftrag maximal 1 GB groß sein. Beachten Sie außerdem, dass ein Exportauftrag maximal 500 Assets enthalten kann.

Dynamic Media Classic speichert im Anzeigebereich &quot;Aufträge&quot;einen Datensatz zu Exportaufträgen.

**So exportieren Sie Assets aus Dynamic Media Classic**

1. Wählen Sie die zu exportierenden Assets aus und klicken Sie dann auf **„Datei“** > **„Exportieren“**.
1. Klicken Sie im Fenster „Ausgewählte Assets exportieren“ auf **„Bildoptionen“** und legen Sie dann die folgenden Optionen fest (Administratoren bestimmen, welche Optionen ihren Benutzern zur Verfügung stehen):

   * **Optional können Sie**
eine Bildvorgabe auswählen, um das Asset beim Exportieren zu formatieren. Wenn Sie eine Bildvorgabe wählen, stehen die übrigen Formatierungsoptionen nicht zur Verfügung, da das Asset die in der Bildvorgabe festgelegten Formate übernimmt.

   * ****
ConversionKonvertieren Sie die Asset-Datei oder das Originalbild.

   * ****
GrößeSie können eine Standardgröße auswählen. Sie können auch in der Dropdown-Liste „Größe“ auf „Andere“ klicken, die gewünschte Maßeinheit wählen und dann die Breite und Höhe festlegen.

      Siehe auch [Festlegen, welche Exportoptionen Media Portal-Benutzern zur Verfügung stehen](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **Format**
Wählen Sie ein Bildformat.

   * **Wählen Sie**
RGB, CMYK oder Grau.

   * ****
AuflösungWählen Sie 72, 150 oder 300 ppi.

   * **AuftragsnameSie können**
dem Export einen Auftragsnamen zuweisen.

   * **Senden**
von E-Mail an optional eine E-Mail-Adresse, um die Assets per E-Mail zu senden. In der E-Mail-Nachricht wird die URL aufgeführt, über die der Empfänger die Assets herunterladen kann.

1. Klicken Sie auf „**Exportieren**“.

Drei grundlegende Exportaktionen werden unterstützt:

* Ausgangsdatei: Exportieren Sie die Ausgangsdatei des Assets.
* Mit Vorlage konvertieren: Verwenden Sie eine Bildvorlage zur Asset-Formatierung.
* Ohne Vorlage konvertieren: Geben Sie Bildmodifikatoren im Exportdialogfeld an.

Die nachfolgenden Asset-Typen können nicht exportiert werden. Für alle anderen Typen sollte ein Export generiert werden.

* Bildsets
* Rendersets
* Rotationssets
* Mediensets
* Sets mit mehreren Bitraten
* E-Kataloge

Vorlagen können außerdem nicht als Ausgangsdatei exportiert werden.

Sie können die Konvertierungsoptionen beim Export folgender Asset-Typen verwenden:

* Bilder
* Vorlagen
* Angepasste Bilder
* PDF (erzeugt konvertierte Seiten)
* PostScript

Wird eine große Menge verschiedener Asset-Typen für den Export ausgewählt, ergibt sich folgendes Verhalten:

* Alle Asset-Typen, die nicht exportiert werden können, werden vor dem Übermitteln des Auftrags aus der Liste entfernt.
* Wurde eine Konvertierung angefordert, werden alle konvertierbaren Typen konvertiert und die übrigen Typen als Ausgangsdateien exportiert.

