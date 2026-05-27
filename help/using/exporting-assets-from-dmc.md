---
title: Exportieren von Assets aus Adobe Dynamic Media Classic
description: Erfahren Sie, wie Sie Assets aus Adobe Dynamic Media Classic exportieren.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T19:47:10.191Z'
TQID: 'https://experienceleague.adobe.com/wE2C1kA1I2fYIkXCqMvw-hPWIV5GMcj1Y0-dgkALyyc'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 443
ht-degree: 38%

---

# Exportieren von Assets aus Adobe Dynamic Media Classic{#exporting-assets-from-dmc}

Sie können die in Adobe Dynamic Media Classic bearbeiteten Assets auf einem lokalen Netzlaufwerk speichern. Exportierte Assets werden zum Herunterladen oder Senden per E-Mail in einer ZIP-Datei zusammengestellt.

Die komprimierte Zip-Datei kann für den Exportauftrag maximal 1 GB groß sein. Außerdem sind maximal 500 Assets pro Exportvorgang zulässig.

Adobe Dynamic Media Classic zeichnet die Exportaufträge im Bildschirm „Aufträge“ auf.

**So exportieren Sie Assets aus Adobe Dynamic Media Classic:**

1. Wählen Sie die Assets aus, die Sie exportieren möchten, und gehen Sie dann zu **[!UICONTROL Datei]** > **[!UICONTROL Exportieren]**.
1. Klicken Sie im Fenster „Ausgewählte Assets exportieren“ auf **[!UICONTROL „Bildoptionen“]** und legen Sie dann die folgenden Optionen fest (Administratoren bestimmen, welche Optionen ihren Benutzern zur Verfügung stehen):

   * **[!UICONTROL Vorgaben]**: Wählen Sie optional eine Bildvorgabe aus, um das Asset beim Exportieren zu formatieren. Wenn Sie eine Bildvorgabe wählen, stehen die übrigen Formatierungsoptionen nicht zur Verfügung, da das Asset die in der Bildvorgabe festgelegten Formate übernimmt.

   * **[!UICONTROL Konversion]**: Konvertiert die Asset-Datei oder das Originalbild.

   * **[!UICONTROL Größe]**: Sie können eine Standardgröße auswählen. Sie können auch **[!UICONTROL Sonstige]** aus der Dropdown-Liste **[!UICONTROL Größe]** auswählen, die gewünschte Maßeinheit auswählen und dann die Breite und Höhe angeben.

     Siehe auch [Angeben der für Media Portal-Benutzer verfügbaren Exportoptionen](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **[!UICONTROL Format]**: Wählen Sie ein Bildformat aus.

   * **[!UICONTROL Farbe]**: Wählen Sie &quot;RGB&quot;, „CMYK“ oder „Grau“.

   * **[!UICONTROL Auflösung]**: Wählen Sie 72 ppi, 150 ppi oder 300 ppi.

   * **[!UICONTROL Auftragsname]**: Sie können dem Export einen Auftragsnamen zuweisen.

   * **[!UICONTROL E-Mail senden an]**: Optional. Geben Sie eine E-Mail-Adresse ein, wenn Sie die Assets per E-Mail versenden möchten. In der E-Mail-Nachricht wird die URL aufgeführt, über die der Empfänger die Assets herunterladen kann.

1. Wählen Sie **[!UICONTROL Exportieren]** aus.

Drei grundlegende Exportaktionen werden unterstützt:

* Ausgangsdatei: Exportieren Sie die Ausgangsdatei des Assets.
* Mit Vorgabe konvertieren (Verwenden einer Bildvorgabe zum Formatieren des Assets)
* Ohne Vorlage konvertieren: Geben Sie Bildmodifikatoren im Exportdialogfeld an.

Die nachfolgenden Asset-Typen können nicht exportiert werden. Alle anderen generieren einen Export.

* Bildsätze
* Rendersets
* Rotationssets
* Mediensets
* Multibitrate-Sets
* E-Kataloge

Außerdem können Vorlagen nicht als „Originaldatei“ exportiert werden.

Sie können die Konvertierungsoptionen beim Export folgender Asset-Typen verwenden:

* Bilder
* Vorlagen
* Angepasste Bilder
* PDF (generiert konvertierte Seiten)
* PostScript®

Wird eine große Menge verschiedener Asset-Typen für den Export ausgewählt, ergibt sich folgendes Verhalten:

* Alle Asset-Typen, die nicht exportiert werden können, werden vor der Übermittlung aus der Liste entfernt
* Wenn eine Konvertierung angefordert wird, werden alle Typen, die konvertiert werden können, konvertiert, und alle anderen werden als Original exportiert
