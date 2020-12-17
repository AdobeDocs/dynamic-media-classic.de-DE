---
title: Hochladen der PDF-Dateien
seo-title: Hochladen der PDF-Dateien
description: 'null'
seo-description: Erfahren Sie, wie Sie die mit einem E-Katalog verknüpften PDF-Dateien hochladen.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 71%

---


# Hochladen der PDF-Dateien{#uploading-the-pdf-files}

Normalerweise werden Adobe PDF-Dateien als Grundlage für einen E-Katalog verwendet, da sie sämtliche Bildinformationen sowie Schriftarten und Vektorgrafiken enthalten. Sie können einen E-Katalog jedoch auch auf Grundlage von Bildern erstellen. Nachdem Sie die PDF-Dateien zum Hochladen vorbereitet haben, klicken Sie in der Symbolleiste für globale Navigation auf „Hochladen“, um den Vorgang zu starten.

## Vorbereiten der PDF-Dateien  {#preparing-your-pdf-files}

Bereiten Sie die PDF-Dateien vor dem Hochladen in Dynamic Media Classic vor:

* Platzieren Sie alle Dateien in demselben Ordner auf dem Computer oder im Netzwerk, um das Hochladen zu vereinfachen.
* Benennen Sie die Dateien in alphanumerischer Reihenfolge gemäß der gewünschten Seitenabfolge. Eine Vorabsortierung der Seiten erleichtert nach dem Hochladen die Anordnung der Dateien in der richtigen Reihenfolge.
* Überprüfen Sie, ob die PDF-Seiten Schnittmarken, Passermarken oder Farbkontrollstreifen enthalten. Diese Markierungen kennzeichnen die Stellen, an denen das Papier beim Druck abgeschnitten werden soll. Sie müssen vor der Veröffentlichung des E-Katalogs im Internet entfernt werden. Dynamic Media Classic bietet Optionen für Schnittmarken, wenn Sie PDF-Dateien hochladen.
* Wenn Sie möchten, dass Betrachter der Website den E-Katalog nach Schlüsselwörtern durchsuchen können, stellen Sie fest, ob es sich um reduzierte PDF-Dateien handelt. Aus reduzierten PDF-Dateien können keine Suchbegriffe extrahiert werden. Um festzustellen, ob eine PDF-Datei reduziert ist, versuchen Sie, Text darin zu markieren. Wenn kein Text markiert werden kann, ist es eine reduzierte PDF-Datei und folglich können Betrachter der Website den E-Katalog nicht nach Schlüsselwörtern durchsuchen.
* Da PDF-Dateien speziell zum Drucken vorgesehen sind, enthalten sie normalerweise CMYK-Bilder. Standardmäßig kann Dynamic Media Classic diese CMYK-Bilder intelligent erkennen und mithilfe eines internen CMYK-Profils konvertieren. Sie können zum Konvertieren der CMYK-Bilder auch ein benutzerdefiniertes Farbprofil verwenden. 

   Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

## Bewährte Optionen zum Hochladen von PDF-Dateien  {#best-practice-pdf-upload-options}

Ausführliche Informationen zu den verschiedenen Methoden zum Hochladen finden Sie unter [Hochladen der Dateien](uploading-files.md#uploading_your_files).

Wählen Sie die hochzuladenden Dateien aus und beachten Sie die folgenden bewährten Optionen ** für PDF-Dateien:

* ****
Beschneiden Wählen Sie im Menü &quot;Beschneiden&quot;die Option &quot;Manuell&quot;, wenn die Seiten Schnittmarken, Passermarken oder andere Markierungen enthalten. Geben Sie die Anzahl der Pixel an, die an den Seitenkanten oben, rechts, unten und links abgeschnitten werden sollen. Schnittmarken werden normalerweise einen halben Zoll vom Rand gesetzt. Sofern Sie die empfohlene Auflösung von 150 ppi gewählt haben, bewirkt die Eingabe des Werts 75 in den Textfeldern „Oben“, „Rechts“, „Unten“ und „Links“, dass die Ränder jeweils um einen halben Zoll (ca. 1,75 cm) beschnitten werden (weil 75 Pixel bei 150 ppi einem halben Zoll entsprechen).

* ****
VerarbeitungWählen Sie im Menü &quot;Verarbeitung&quot;die Option &quot;Rastern&quot;. Die PDF-Datei muss gerastert werden, damit alle Seiten und Bilder im E-Katalog angezeigt werden können.

* **Suchbegriffe extrahieren (optional)**
Wählen Sie diese Option, wenn Ihre Viewer nach Suchbegriffen in Ihrem E-Katalog suchen können sollen.

* **E-Katalog aus mehrseitiger PDF automatisch erstellen (optional)**
Wählen Sie diese Option, um beim Hochladen automatisch einen E-Katalog zu erstellen. Sie können dann sofort den Anzeigebereich „E-Katalog“ aufrufen und daran arbeiten, ohne zuerst PDF-Dateien auswählen und den Befehl „Erstellen“ aktivieren zu müssen. Der E-Katalog erhält in diesem Fall denselben Namen wie die PDF-Datei.

* ****
ResolutionDynamic Media Classic empfiehlt 150 Pixel pro Zoll.

* **Es wird empfohlen,**
ColorspaceDynamic Media Classic die Option &quot;Automatisch erkennen&quot;zu wählen. Normalerweise enthalten PDF-Dateien, die zum Drucken vorgesehen sind, CMYK-Bilder, während PDF-Dateien, die nur zum Anzeigen vorgesehen sind, RGB-Bilder enthalten. Wenn in einer PDF-Datei beide Farbräume verwendet wurden, können Sie einen bestimmten Farbraum auswählen, indem Sie „Immer RGB“ oder „Immer CMYK“ wählen. Zur Verwendung beider Farbräume innerhalb einer PDF-Datei kommt es, wenn Seitengrafiken im CMYK-Farbraum und Bilder im RGB-Farbraum verwendet werden. Wenn Sie ein ICC-Profil hochgeladen haben, wird dessen Name zur Auswahl im Menü „Farbraum“ angezeigt. 

   Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

* **Farbprofil**
Wählen Sie eine Profil-Option:

* **Konvertieren in**
SRGBConverts in SRGB (Standard Red Green Blue). sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Websites.

* **&quot;Ursprünglicher Farbraum beibehalten&quot;**
Behält den ursprünglichen Farbraum bei.

* **Benutzerdefiniert von >**
Zu öffnet Menüs, damit Sie einen Farbraum &quot;Konvertieren von&quot;und &quot;Konvertieren in&quot;auswählen können. Sie können einen Photoshop-Standardfarbraum oder einen Farbraum auswählen, den Sie in Dynamic Media Classic hochgeladen haben.

Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Details zu allen PDF-Optionen finden Sie unter [Optionen für das Hochladen von PDF-Dateien](pdfs.md#pdf_upload_options).

