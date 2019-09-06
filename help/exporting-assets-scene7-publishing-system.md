---
title: Exportieren von Assets aus dem Scene7 Publishing System
seo-title: Exportieren von Assets aus dem Scene7 Publishing System
description: 'null'
seo-description: Hier erfahren Sie, wie Sie Assets aus dem Scene 7 Publishing System exportieren.
uuid: d 42 b 7 a 73-80 c 0-4 a 9 a-a 04 e -7 ef 53 e 6 fcf 22
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/managing_ assets
discoiquuid: eb 850 ec 7-a 669-41 ea-b 2 b 0-4 c 9178 e 34 f 95
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Exportieren von Assets aus dem Scene7 Publishing System{#exporting-assets-from-scene-publishing-system}

Sie können die im Scene7 Publishing System bearbeiteten Assets auf einem lokalen Netzlaufwerk speichern. Exportierte Assets werden zum Herunterladen oder Senden per E-Mail in einer ZIP-Datei zusammengestellt.

Die komprimierte Zip-Datei kann für den Exportauftrag maximal 1 GB groß sein. Beachten Sie außerdem, dass ein Exportauftrag maximal 500 Assets enthalten kann.

Dynamic Media Classic speichert einen Datensatz über exportierte Aufträge im Anzeigebereich "Aufträge" .

**So exportieren Sie Assets aus dem Scene7 Publishing System**

1. Wählen Sie die zu exportierenden Assets aus und klicken Sie dann auf **„Datei“** &gt; **„Exportieren“**.
1. Klicken Sie im Fenster „Ausgewählte Assets exportieren“ auf **„Bildoptionen“** und legen Sie dann die folgenden Optionen fest (Administratoren bestimmen, welche Optionen ihren Benutzern zur Verfügung stehen):

   **Wählen Sie** optional eine Bildvorgabe aus, um das Asset beim Exportieren zu formatieren. Wenn Sie eine Bildvorgabe wählen, stehen die übrigen Formatierungsoptionen nicht zur Verfügung, da das Asset die in der Bildvorgabe festgelegten Formate übernimmt.

   **Konvertierung** Konvertieren Sie die Asset-Datei oder das Originalbild.

   **Größe** Sie können eine Standardgröße auswählen. Sie können auch in der Dropdown-Liste „Größe“ auf „Andere“ klicken, die gewünschte Maßeinheit wählen und dann die Breite und Höhe festlegen.

   Siehe auch [Festlegen, welche Exportoptionen Media Portal-Benutzern zur Verfügung stehen](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   **Format** Wählen Sie ein Bildformat.

   **Wählen** Sie "RGB" ," CMYK" oder "Grau" .

   **Auflösung** wählen Sie 72, 150 oder 300 ppi.

   **Auftragsname** Sie können dem Export einen Auftragsnamen zuweisen.

   **E-Mail an** optional senden, geben Sie eine E-Mail-Adresse ein, um die Assets per E-Mail zu senden. In der E-Mail-Nachricht wird die URL aufgeführt, über die der Empfänger die Assets herunterladen kann.

1. Klicken Sie auf „**Exportieren**“.

Drei grundlegende Exportaktionen werden unterstützt:

* Ausgangsdatei: Exportieren Sie die Ausgangsdatei des Assets.
* Mit Vorlage konvertieren: Verwenden Sie eine Bildvorlage zur Asset-Formatierung.
* Ohne Vorlage konvertieren: Geben Sie Bildmodifikatoren im Exportdialogfeld an.

Die nachfolgenden Asset-Typen können nicht exportiert werden. Für alle anderen Typen sollte ein Export generiert werden.

* Bildsätze
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

