---
title: PDF-Dateien hochladen
description: Erfahren Sie, wie Sie die mit einem E-Katalog verknüpften PDF-Dateien in Adobe Dynamic Media Classic hochladen.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: ac9cba2c33fb1df65e64746dea2557632b7b2903
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 39%

---

# PDF-Dateien hochladen{#uploading-the-pdf-files}

In der Regel sind Adobe PDF-Dateien die Quelle für einen eCatalog. Diese Dateien enthalten alle Bildinformationen, Schriftarten und Vektorgrafiken. Sie können einen E-Katalog jedoch auch auf Grundlage von Bildern erstellen. Nachdem Sie Ihre PDF-Dateien für den Upload vorbereitet haben, wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Hochladen]** , um mit dem Hochladen der PDF zu beginnen.

>[!NOTE]
>
>Wenn Sie eine PDF für die Seitenextraktion hochladen, enthält die Adobe die folgende Best Practice-Richtlinie und die erzwungene Beschränkung.
>
>* Maximale Seitenzahl pro PDF, die für die Extraktion berücksichtigt wird
   >   * Best Practice: 100
   >   * Erzwungene Beschränkung: 1000 (für Aktualisierungs-Uploads)


## Vorbereiten der PDF-Dateien {#preparing-your-pdf-files}

Bereiten Sie Ihre PDF-Dateien vor dem Hochladen auf Adobe Dynamic Media Classic vor:

* Um das Hochladen der Dateien zu vereinfachen, platzieren Sie alle Dateien im selben Ordner auf Ihrem Computer oder Netzwerk.
* Benennen Sie die Dateien in alphanumerischer Reihenfolge gemäß der gewünschten Seitenabfolge. Eine Vorabsortierung der Seiten erleichtert nach dem Hochladen die Anordnung der Dateien in der richtigen Reihenfolge.
* Um zu sehen, ob PDF-Seiten Zuschnittmarkierungen, Registrierungsziele oder Farbbalken enthalten, überprüfen Sie die Seiten. Diese Markierungen kennzeichnen die Stellen, an denen das Papier beim Druck abgeschnitten werden soll. Sie müssen vor der Veröffentlichung des E-Katalogs im Internet entfernt werden. Adobe Dynamic Media Classic bietet beim Hochladen von PDF-Dateien Optionen für Zuschnittmarkierungen.
* Wenn Sie möchten, dass Betrachter der Website den E-Katalog nach Schlüsselwörtern durchsuchen können, stellen Sie fest, ob es sich um reduzierte PDF-Dateien handelt. Aus reduzierten PDF-Dateien können keine Suchbegriffe extrahiert werden. Um festzustellen, ob eine PDF-Datei reduziert ist, versuchen Sie, Text darin zu markieren. Wenn Sie keinen Text auswählen können, wird die PDF reduziert und Viewer können in Ihrem eCatalog nicht nach Keywords suchen.
* Da PDF-Dateien speziell zum Drucken vorgesehen sind, enthalten sie normalerweise CMYK-Bilder. Standardmäßig kann Adobe Dynamic Media Classic diese CMYK-Bilder intelligent erkennen und mithilfe eines internen CMYK-Farbprofils konvertieren. Sie können zum Konvertieren der CMYK-Bilder auch ein benutzerdefiniertes Farbprofil verwenden. 

   Siehe [ICC-Profile (International Color Consortium)](icc-profiles.md#icc_profiles).

## Bewährte Optionen zum Hochladen von PDF-Dateien {#best-practice-pdf-upload-options}

Ausführliche Informationen zu den verschiedenen Methoden zum Hochladen finden Sie unter [Hochladen der Dateien](uploading-files.md#uploading_your_files).

Wählen Sie die hochzuladenden Dateien aus und beachten Sie die folgenden bewährten Optionen ** für PDF-Dateien:

* **Optionen zum Zuschneiden** - Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL Optionen zum Zuschneiden]**. Wenn die PDF-Seiten Zuschnittmarkierungen, Registrierungszeichen oder andere Zeichen enthalten, wird die **[!UICONTROL Zuschneiden]** Dropdown-Liste auswählen **[!UICONTROL Manuell]**. Geben Sie die Anzahl der Pixel an, die an den Seitenkanten oben, rechts, unten und links abgeschnitten werden sollen. Zuschnittmarkierungen sind oft auf einen halben Zoll-Rand eingestellt. Angenommen, Sie wählen **[!UICONTROL 150]** (empfohlen) als Pixelpro-Zoll-Auflösung und geben Sie in die Textfelder &quot;Oben&quot;, &quot;Rechts&quot;, &quot;Unten&quot;und &quot;Links&quot;die Werte 75, 75, 75 und 75 ein. In diesem Fall schneidet er einen halben Zoll von den Rändern ab (bei 150 ppi, die Hälfte von 1 entspricht 75 Pixel).

* **Verarbeitung** - Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL PDF-Optionen]**. Im **[!UICONTROL Verarbeitung]** Dropdown-Liste auswählen **[!UICONTROL Rastern]**. Die PDF-Datei muss gerastert werden, damit alle Seiten und Bilder im E-Katalog angezeigt werden können.

* **Suchbegriffe extrahieren (optional)** - Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL PDF-Optionen]**. Wählen Sie in der Dropdown-Liste Extract die Option **[!UICONTROL Suchbegriffe]** , wenn Sie möchten, dass Ihre Viewer in Ihrem eCatalog nach Keywords suchen können.

* **E-Katalog von mehreren Seiten automatisch generieren (optional)** - Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL PDF-Optionen]**. Auswählen **[!UICONTROL eCatalog von mehrseitiger PDF automatisch generieren]** , um beim Hochladen automatisch einen E-Katalog zu erstellen. Sie können dann sofort den Anzeigebereich „E-Katalog“ aufrufen und daran arbeiten, ohne zuerst PDF-Dateien auswählen und den Befehl „Erstellen“ aktivieren zu müssen. Der E-Katalog erhält in diesem Fall denselben Namen wie die PDF-Datei.

* **Auflösung** - Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL PDF-Optionen]**. Im **[!UICONTROL Auflösung]** Textfeld einen Wert eingeben. Adobe Dynamic Media Classic empfiehlt 150 Pixel pro Zoll.

* **Farbraum** - Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL PDF-Optionen]**. Wählen Sie in der Dropdownliste Farbraum die Option **[!UICONTROL Automatisch erkennen]**. Normalerweise enthalten PDF-Dateien, die zum Drucken vorgesehen sind, CMYK-Bilder, während PDF-Dateien, die nur zum Anzeigen vorgesehen sind, RGB-Bilder enthalten. Wenn in einer PDF-Datei beide Farbräume verwendet wurden, können Sie einen bestimmten Farbraum auswählen, indem Sie „Immer RGB“ oder „Immer CMYK“ wählen. Zur Verwendung beider Farbräume innerhalb einer PDF-Datei kommt es, wenn Seitengrafiken im CMYK-Farbraum und Bilder im RGB-Farbraum verwendet werden. Wenn Sie ein ICC-Profil hochgeladen haben, wird dessen Name zur Auswahl im Menü „Farbraum“ angezeigt. 

   Siehe [ICC-Profile (International Color Consortium)](/help/icc-profiles.md).

* **Farbprofiloptionen** - Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL Farbprofiloptionen]** und wählen Sie dann eine Farbprofil -Option:

   * **Originalfarbraum beibehalten** - Behält den ursprünglichen Farbraum bei.

   * **Benutzerdefiniert von > zu** - Öffnet Untermenüs, damit Sie eine **[!UICONTROL Konvertieren von]** und **[!UICONTROL Konvertieren in]** Farbraum. Sie können einen standardmäßigen Photoshop-Farbraum oder einen Farbraum auswählen, den Sie in Adobe Dynamic Media Classic hochgeladen haben.

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

Siehe [ICC-Profile (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Details zu allen PDF-Optionen finden Sie unter [Optionen für das Hochladen von PDF-Dateien](pdfs.md#pdf_upload_options).
