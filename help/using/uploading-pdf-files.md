---
title: PDF-Dateien hochladen
description: Erfahren Sie, wie Sie die mit einem E-Katalog verknüpften PDF-Dateien in Adobe Dynamic Media Classic hochladen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
topic: Integrations, Development
level: Experienced
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 30%

---

# PDF-Dateien hochladen{#uploading-the-pdf-files}

Normalerweise sind Adobe PDF-Dateien die Quelle für einen E-Katalog. Diese Dateien enthalten alle Bildinformationen, Schriftarten und Vektorgrafiken. Sie können einen E-Katalog jedoch auch auf Grundlage von Bildern erstellen. Nachdem Sie Ihre PDF-Dateien für das Hochladen vorbereitet haben, wählen Sie in der globalen Navigationsleiste die Option **[!UICONTROL Hochladen]** aus, um mit dem Hochladen der PDF-Dateien zu beginnen.

Wenn Sie eine PDF zur Seitenextraktion hochladen, setzt Adobe die folgende Beschränkung durch:

| PDF-Limittyp | Limit | Änderung des Grenzwerts am 31. Dezember 2022 |
| --- | --- | --- |
| Maximale Seitenzahl einer PDF, damit eine Extraktion durchgeführt werden kann | 5.000 (für neue Uploads) | 100 (für alle PDFs) |

Siehe auch [Grenzwerte für Dynamic Media](/help/using/limitations.md).

## Vorbereiten der PDF-Dateien

Bereiten Sie Ihre PDF-Dateien vor dem Hochladen in Adobe Dynamic Media Classic vor:

* Um das Hochladen der Dateien zu vereinfachen, platzieren Sie alle Dateien im selben Ordner auf Ihrem Computer oder Netzwerk.
* Benennen Sie die Dateien in alphanumerischer Reihenfolge gemäß der gewünschten Seitenabfolge. Eine Vorabsortierung der Seiten erleichtert nach dem Hochladen die Anordnung der Dateien in der richtigen Reihenfolge.
* Überprüfen Sie die Seiten, um festzustellen, ob PDF-Seiten Zuschnittmarken, Registrierungsziele oder Farbbalken enthalten. Diese Markierungen kennzeichnen die Stellen, an denen das Papier beim Druck abgeschnitten werden soll. Sie müssen vor der Veröffentlichung des E-Katalogs im Internet entfernt werden. Adobe Dynamic Media Classic bietet Optionen zum Zuschneiden von Markierungen beim Hochladen von PDF-Dateien.
* Wenn Sie möchten, dass Betrachter Ihren E-Katalog nach Keyword durchsuchen, finden Sie heraus, ob Ihre PDF-Dateien „reduziert“ sind. Aus reduzierten PDF-Dateien können keine Suchbegriffe extrahiert werden. Um herauszufinden, ob eine PDF reduziert ist, versuchen Sie, den darin enthaltenen Text auszuwählen. Wenn Sie keinen Text auswählen können, ist die PDF reduziert und Viewer können nicht nach Keyword in Ihrem E-Katalog suchen.
* Da PDF-Dateien speziell zum Drucken vorgesehen sind, enthalten sie normalerweise CMYK-Bilder. Standardmäßig kann Adobe Dynamic Media Classic diese CMYK-Bilder intelligent erkennen und mithilfe eines internen CMYK-Farbprofils konvertieren. Sie können zum Konvertieren der CMYK-Bilder auch ein benutzerdefiniertes Farbprofil verwenden. 

  Siehe [ICC (International Color Consortium)-Profile](icc-profiles.md#icc_profiles).

## Bewährte Optionen zum Hochladen von PDF-Dateien {#best-practice-pdf-upload-options}

Ausführliche Informationen zu den verschiedenen Methoden zum Hochladen finden Sie unter [Hochladen der Dateien](uploading-files.md#uploading_your_files).

Wählen Sie die Dateien aus, die Sie hochladen möchten, und wählen Sie dann diese *Best Practice* PDF-Optionen aus:

* **Zuschnittsoptionen**: Wählen Sie im Dialogfeld Upload-Auftragsoptionen die Option **[!UICONTROL Zuschnittsoptionen]** aus. Wenn die PDF-Seiten Schnittmarken, Registrierungsmarken oder andere Markierungen enthalten, wählen Sie in der Dropdown-Liste **[!UICONTROL Zuschneiden]** die Option **[!UICONTROL Manuell]**. Geben Sie die Anzahl der Pixel ein, die von der oberen, rechten, unteren und linken Seite der Seiten abgeschnitten werden sollen. Schnittmarken werden oft auf einen halben Zoll Rand gesetzt. Angenommen, Sie wählen **[!UICONTROL 150]** (empfohlen) als Pixel-pro-Zoll-Auflösung. Geben Sie 75, 75, 75, 75 in die Textfelder Oben, Rechts, Unten und Links ein. In einem solchen Fall schneidet es einen halben Zoll von den Rändern (bei 150 ppi, die Hälfte von 1 gleich 75 Pixel).

* **Verarbeitung**: Wählen Sie im Dialogfeld „Upload-Auftragsoptionen“ die Option **[!UICONTROL PDF-Optionen]**. Wählen Sie in **[!UICONTROL Dropdown]** Liste „Verarbeitung“ die Option **[!UICONTROL Rastern]**. Die PDF-Datei muss gerastert werden, damit alle Seiten und Bilder im E-Katalog angezeigt werden können.

* **Suchbegriffe extrahieren (optional)**: Wählen Sie im Dialogfeld Upload-Auftragsoptionen die Option **[!UICONTROL PDF-Optionen]**. Wählen Sie in der Dropdown-Liste Extrahieren die Option **[!UICONTROL Suchbegriffe]**, wenn Sie möchten, dass Ihre Betrachter in der Lage sein sollen, in Ihrem E-Katalog nach einem Schlüsselwort zu suchen.

* **E-Katalog automatisch aus mehrseitigem PDF generieren (optional)**: Wählen Sie im Dialogfeld „Upload-Auftragsoptionen“ die Option **[!UICONTROL PDF-Optionen]**. PDF Klicken Sie auf **[!UICONTROL E-Katalog von mehreren Seiten aus automatisch erstellen]** damit Sie beim Hochladen automatisch einen E-Katalog erstellen können. Sie können dann sofort den Anzeigebereich „E-Katalog“ aufrufen und daran arbeiten, ohne zuerst PDF-Dateien auswählen und den Befehl „Erstellen“ aktivieren zu müssen. Der E-Katalog erhält in diesem Fall denselben Namen wie die PDF-Datei.

* **Lösung**: Wählen Sie im Dialogfeld „Upload-Auftragsoptionen“ die Option **[!UICONTROL PDF-Optionen]**. Geben **[!UICONTROL im Textfeld]** Auflösung“ einen Wert ein. Adobe Dynamic Media Classic empfiehlt 150 Pixel pro Zoll.

* **Farbraum**: Wählen Sie im Dialogfeld „Upload-Auftragsoptionen“ die Option **[!UICONTROL PDF-Optionen]**. Wählen Sie in der Dropdown-Liste „Farbraum“ die Option **[!UICONTROL Automatisch erkennen]**. Normalerweise enthalten PDF-Dateien, die zum Drucken vorgesehen sind, CMYK-Bilder, während PDF-Dateien, die nur zum Anzeigen vorgesehen sind, RGB-Bilder enthalten. Wenn in einer PDF-Datei beide Farbräume verwendet wurden, können Sie einen bestimmten Farbraum auswählen, indem Sie „Immer RGB“ oder „Immer CMYK“ wählen. Zur Verwendung beider Farbräume innerhalb einer PDF-Datei kommt es, wenn Seitengrafiken im CMYK-Farbraum und Bilder im RGB-Farbraum verwendet werden. Wenn Sie ein ICC-Profil hochgeladen haben, wird dessen Name zur Auswahl im Menü „Farbraum“ angezeigt. 

  Siehe [ICC (International Color Consortium)-Profile](/help/using/icc-profiles.md).

* **Farbprofiloptionen**: Wählen Sie im Dialogfeld „Upload-Auftragsoptionen“ die Option **[!UICONTROL Farbprofiloptionen]** und wählen Sie dann eine Farbprofiloption aus:

   * **Ursprünglichen Farbraum beibehalten**: Behält den ursprünglichen Farbraum bei.

   * **Benutzerdefiniert von > An**: Öffnet Untermenüs, in denen Sie einen **[!UICONTROL Konvertieren von]** und **[!UICONTROL Konvertieren in]** auswählen können. Sie können einen standardmäßigen Photoshop-Farbraum oder einen Farbraum auswählen, den Sie in Adobe Dynamic Media Classic hochgeladen haben.

<!-- * **Convert To SRGB**: Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on Web pages. -->

Siehe [ICC (International Color Consortium)-Profile](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Details zu allen PDF-Optionen finden Sie unter [Optionen für das Hochladen von PDF-Dateien](pdfs.md#pdf_upload_options).
