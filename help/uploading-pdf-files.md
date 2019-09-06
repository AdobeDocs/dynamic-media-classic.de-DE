---
title: Hochladen der PDF-Dateien
seo-title: Hochladen der PDF-Dateien
description: 'null'
seo-description: Erfahren Sie, wie Sie die mit einem E-Katalog verknüpften PDF-Dateien hochladen.
uuid: 9 e 178 bb 2-ac 09-427 a-b 61 a-aad 4 e 87 a 837
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 0097 cba 5-c 886-4115-bc 35-7 ae 7 a 500202 f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Hochladen der PDF-Dateien{#uploading-the-pdf-files}

Normalerweise werden Adobe PDF-Dateien als Grundlage für einen E-Katalog verwendet, da sie sämtliche Bildinformationen sowie Schriftarten und Vektorgrafiken enthalten. Sie können einen E-Katalog jedoch auch auf Grundlage von Bildern erstellen. Nachdem Sie die PDF-Dateien zum Hochladen vorbereitet haben, klicken Sie in der Symbolleiste für globale Navigation auf „Hochladen“, um den Vorgang zu starten.

## Vorbereiten der PDF-Dateien {#preparing-your-pdf-files}

Die PDF-Dateien müssen vor dem Hochladen in das Scene7 Publishing System vorbereitet werden.

* Platzieren Sie alle Dateien in demselben Ordner auf dem Computer oder im Netzwerk, um das Hochladen zu vereinfachen.
* Benennen Sie die Dateien in alphanumerischer Reihenfolge gemäß der gewünschten Seitenabfolge. Eine Vorabsortierung der Seiten erleichtert nach dem Hochladen die Anordnung der Dateien in der richtigen Reihenfolge.
* Überprüfen Sie, ob die PDF-Seiten Schnittmarken, Passermarken oder Farbkontrollstreifen enthalten. Diese Markierungen kennzeichnen die Stellen, an denen das Papier beim Druck abgeschnitten werden soll. Sie müssen vor der Veröffentlichung des E-Katalogs im Internet entfernt werden. Dynamic Media Classic bietet Optionen für Schnittmarken beim Hochladen von PDF-Dateien.
* Wenn Sie möchten, dass Betrachter der Website den E-Katalog nach Schlüsselwörtern durchsuchen können, stellen Sie fest, ob es sich um reduzierte PDF-Dateien handelt. Aus reduzierten PDF-Dateien können keine Suchbegriffe extrahiert werden. Um festzustellen, ob eine PDF-Datei reduziert ist, versuchen Sie, Text darin zu markieren. Wenn kein Text markiert werden kann, ist es eine reduzierte PDF-Datei und folglich können Betrachter der Website den E-Katalog nicht nach Schlüsselwörtern durchsuchen.
* Da PDF-Dateien speziell zum Drucken vorgesehen sind, enthalten sie normalerweise CMYK-Bilder. Standardmäßig kann SPS diese CMYK-Bilder automatisch erkennen und mithilfe eines integrierten CMYK-Farbprofils konvertieren. Sie können zum Konvertieren der CMYK-Bilder auch ein benutzerdefiniertes Farbprofil verwenden. 

   Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

## Bewährte Optionen zum Hochladen von PDF-Dateien {#best-practice-pdf-upload-options}

Ausführliche Informationen zu den verschiedenen Methoden zum Hochladen finden Sie unter [Hochladen der Dateien](uploading-files.md#uploading_your_files).

Wählen Sie die hochzuladenden Dateien aus und beachten Sie die folgenden bewährten Optionen ** für PDF-Dateien:

**Beschneiden** Sie das Menü "Beschneiden" und wählen Sie" Manuell" , wenn die Seiten Schnittmarken, Passermarken oder andere Marken enthalten. Geben Sie die Anzahl der Pixel an, die an den Seitenkanten oben, rechts, unten und links abgeschnitten werden sollen. Schnittmarken werden normalerweise einen halben Zoll vom Rand gesetzt. Sofern Sie die empfohlene Auflösung von 150 ppi gewählt haben, bewirkt die Eingabe des Werts 75 in den Textfeldern „Oben“, „Rechts“, „Unten“ und „Links“, dass die Ränder jeweils um einen halben Zoll (ca. 1,75 cm) beschnitten werden (weil 75 Pixel bei 150 ppi einem halben Zoll entsprechen).

**Verarbeitung** Wählen Sie im Menü "Verarbeitung" die Option" Rastern" . Die PDF-Datei muss gerastert werden, damit alle Seiten und Bilder im E-Katalog angezeigt werden können.

**Suchbegriffe extrahieren (optional)** Wählen Sie diese Option, wenn Sie möchten, dass Ihre Viewer nach Schlüsselwörtern im E-Katalog suchen können.

**E-Katalog aus mehrseitiger PDF-Datei automatisch erstellen (optional)** Wählen Sie diese Option, um automatisch einen E-Katalog beim Hochladen zu erstellen. Sie können dann sofort den Anzeigebereich „E-Katalog“ aufrufen und daran arbeiten, ohne zuerst PDF-Dateien auswählen und den Befehl „Erstellen“ aktivieren zu müssen. Der E-Katalog erhält in diesem Fall denselben Namen wie die PDF-Datei.

**Die Auflösung** von Dynamic Media Classic empfiehlt 150 Pixel pro Zoll.

**Colorspace** Dynamic Media Classic empfiehlt die automatische Auswahl der Option "Automatisch erkennen" . Normalerweise enthalten PDF-Dateien, die zum Drucken vorgesehen sind, CMYK-Bilder, während PDF-Dateien, die nur zum Anzeigen vorgesehen sind, RGB-Bilder enthalten. Wenn in einer PDF-Datei beide Farbräume verwendet wurden, können Sie einen bestimmten Farbraum auswählen, indem Sie „Immer RGB“ oder „Immer CMYK“ wählen. Zur Verwendung beider Farbräume innerhalb einer PDF-Datei kommt es, wenn Seitengrafiken im CMYK-Farbraum und Bilder im RGB-Farbraum verwendet werden. Wenn Sie ein ICC-Profil hochgeladen haben, wird dessen Name zur Auswahl im Menü „Farbraum“ angezeigt. 

Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

**Farbprofil** Wählen Sie eine Farbprofil aus:

**In SRGB** konvertieren Konvertiert in SRGB (Standard
Red Green Blue). sRGB ist der empfohlene Farbraum für die Anzeige von Bildern auf Websites.

**Ursprünglicher Farbraum** behält den ursprünglichen Farbraum bei.

**Benutzerdefiniert von &gt; Zum** Öffnen der Menüs "Konvertieren von" und" Konvertieren in" . Sie können einen Photoshop-Standardfarbraum auswählen oder einen Farbraum, den Sie in SPS hochgeladen haben. 

Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Details zu allen PDF-Optionen finden Sie unter [Optionen für das Hochladen von PDF-Dateien](pdfs.md#pdf_upload_options).

