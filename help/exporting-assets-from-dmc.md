---
title: Exportieren von Assets aus Dynamic Media Classic
description: Erfahren Sie, wie Sie Assets aus Dynamic Media Classic exportieren.
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 63%

---

# Exportieren von Assets aus Dynamic Media Classic{#exporting-assets-from-dmc}

Sie können die in Dynamic Media Classic bearbeiteten Assets auf einem lokalen Netzlaufwerk speichern. Exportierte Assets werden zum Herunterladen oder Senden per E-Mail in einer ZIP-Datei zusammengestellt.

Die komprimierte Zip-Datei kann für den Exportauftrag maximal 1 GB groß sein. Außerdem sind maximal 500 Assets pro Exportauftrag zulässig.

Dynamic Media Classic speichert einen Datensatz mit Exportvorgängen im Bildschirm &quot;Aufträge&quot;.

**So exportieren Sie Assets aus Dynamic Media Classic:**

1. Wählen Sie die zu exportierenden Assets aus und klicken Sie dann auf **[!UICONTROL „Datei“]** > **[!UICONTROL „Exportieren“]**.
1. Klicken Sie im Fenster „Ausgewählte Assets exportieren“ auf **„Bildoptionen“** und legen Sie dann die folgenden Optionen fest (Administratoren bestimmen, welche Optionen ihren Benutzern zur Verfügung stehen):

   * **Vorgaben**  - Wählen Sie optional eine Bildvorgabe aus, um das Asset beim Exportieren zu formatieren. Wenn Sie eine Bildvorgabe wählen, stehen die übrigen Formatierungsoptionen nicht zur Verfügung, da das Asset die in der Bildvorgabe festgelegten Formate übernimmt.

   * **Konversion**  - Konvertieren Sie die Asset-Datei oder das Originalbild.

   * **Größe**  - Sie können eine Standardgröße auswählen. Sie können auch in der Dropdown-Liste „Größe“ auf **[!UICONTROL „Andere“]** klicken, die gewünschte Maßeinheit wählen und dann die Breite und Höhe festlegen.****

      Siehe auch [Festlegen, welche Exportoptionen Media Portal-Benutzern zur Verfügung stehen](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **Format**  - Wählen Sie ein Bildformat.

   * **Farbe**  - Wählen Sie RGB, CMYK oder Grau.

   * **Lösung**  - Wählen Sie 72 ppi, 150 ppi oder 300 ppi.

   * **Auftragsname**  - Sie können dem Export einen Auftragsnamen zuweisen.

   * **E-Mail senden an**  - Geben Sie optional eine E-Mail-Adresse ein, an die die Assets per E-Mail gesendet werden sollen. In der E-Mail-Nachricht wird die URL aufgeführt, über die der Empfänger die Assets herunterladen kann.

1. Klicken Sie auf „**[!UICONTROL Exportieren]**“.

Drei grundlegende Exportaktionen werden unterstützt:

* Ausgangsdatei: Exportieren Sie die Ausgangsdatei des Assets.
* Mit Vorlage konvertieren: Verwenden Sie eine Bildvorlage zur Asset-Formatierung.
* Ohne Vorlage konvertieren: Geben Sie Bildmodifikatoren im Exportdialogfeld an.

Die nachfolgenden Asset-Typen können nicht exportiert werden. Alle anderen generieren einen Export.

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
* PDF (generiert konvertierte Seiten)
* PostScript®

Wird eine große Menge verschiedener Asset-Typen für den Export ausgewählt, ergibt sich folgendes Verhalten:

* Alle Asset-Typen, die nicht exportiert werden können, werden vor dem Übermitteln des Auftrags aus der Liste entfernt.
* Wurde eine Konvertierung angefordert, werden alle konvertierbaren Typen konvertiert und die übrigen Typen als Ausgangsdateien exportiert.
