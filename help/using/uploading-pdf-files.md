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

In der Regel sind Adobe PDF-Dateien die Quelle für einen eCatalog. Diese Dateien enthalten alle Bildinformationen, Schriftarten und Vektorgrafiken. Sie können einen E-Katalog jedoch auch auf Grundlage von Bildern erstellen. Nachdem Sie Ihre PDF-Dateien für das Hochladen vorbereitet haben, wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Hochladen]** aus, um mit dem Hochladen der PDF zu beginnen.

Wenn Sie eine PDF für die Seitenextraktion hochladen, erzwingt Adobe die folgende Einschränkung:

| PDF-Limit-Typ | Erzwungene Beschränkung | Änderung der Beschränkung am 31. Dezember 2022 |
| --- | --- | --- |
| Maximale Seitenzahl für eine PDF, die für die Extraktion berücksichtigt werden soll | 5000 (für neue Uploads) | 100 (für alle PDF) |

Siehe auch [Dynamic Media-Einschränkungen](/help/using/limitations.md).

## Vorbereiten der PDF-Dateien

Bereiten Sie Ihre PDF-Dateien vor dem Hochladen auf Adobe Dynamic Media Classic vor:

* Um das Hochladen der Dateien zu vereinfachen, platzieren Sie alle Dateien im selben Ordner auf Ihrem Computer oder Netzwerk.
* Benennen Sie die Dateien in alphanumerischer Reihenfolge gemäß der gewünschten Seitenabfolge. Eine Vorabsortierung der Seiten erleichtert nach dem Hochladen die Anordnung der Dateien in der richtigen Reihenfolge.
* Um zu sehen, ob PDF-Seiten Zuschnittmarkierungen, Registrierungsziele oder Farbbalken enthalten, überprüfen Sie die Seiten. Diese Markierungen kennzeichnen die Stellen, an denen das Papier beim Druck abgeschnitten werden soll. Sie müssen vor der Veröffentlichung des E-Katalogs im Internet entfernt werden. Adobe Dynamic Media Classic bietet beim Hochladen von PDF-Dateien Optionen für Zuschnittmarkierungen.
* Wenn Sie möchten, dass Betrachter Ihren E-Katalog nach Keywords durchsuchen, überprüfen Sie, ob Ihre PDF-Dateien &quot;reduziert&quot;sind. Aus reduzierten PDF-Dateien können keine Suchbegriffe extrahiert werden. Um herauszufinden, ob eine PDF reduziert ist, wählen Sie den darin enthaltenen Text aus. Wenn Sie keinen Text auswählen können, wird die PDF reduziert und Viewer können in Ihrem eCatalog nicht nach Keywords suchen.
* Da PDF-Dateien speziell zum Drucken vorgesehen sind, enthalten sie normalerweise CMYK-Bilder. Standardmäßig kann Adobe Dynamic Media Classic diese CMYK-Bilder intelligent erkennen und mithilfe eines internen CMYK-Farbprofils konvertieren. Sie können zum Konvertieren der CMYK-Bilder auch ein benutzerdefiniertes Farbprofil verwenden. 

  Siehe [ICC-Profile (International Color Consortium)](icc-profiles.md#icc_profiles).

## Bewährte Optionen zum Hochladen von PDF-Dateien {#best-practice-pdf-upload-options}

Ausführliche Informationen zu den verschiedenen Methoden zum Hochladen finden Sie unter [Hochladen der Dateien](uploading-files.md#uploading_your_files).

Wählen Sie die Dateien aus, die Sie hochladen möchten, und wählen Sie dann die folgenden *Best Practice*-PDF-Optionen aus:

* **Zuschnitt-Optionen**: Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL Zuschnitt-Optionen]**. Wenn die PDF-Seiten Zuschnittmarkierungen, Registrierungsmarkierungen oder andere Markierungen enthalten, wählen Sie in der Dropdownliste **[!UICONTROL Zuschneiden]** die Option **[!UICONTROL Manuell]**. Geben Sie die Anzahl der Pixel ein, die oben, rechts, unten und links von den Seiten beschnitten werden sollen. Zuschnittmarkierungen sind oft auf einen halben Zoll-Rand eingestellt. Angenommen, Sie wählen **[!UICONTROL 150]** (empfohlen) als Pixelpro-Zoll-Auflösung. Geben Sie dann die Textfelder 75, 75, 75, 75 in die Textfelder oben, rechts, unten und links ein. In einem solchen Fall schneidet er einen halben Zoll von den Rändern ab (bei 150 ppi, die Hälfte von 1 entspricht 75 Pixel).

* **Verarbeitung**: Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL PDF-Optionen]** aus. Wählen Sie in der Dropdownliste **[!UICONTROL Verarbeitung]** die Option **[!UICONTROL Rastern]**. Die PDF-Datei muss gerastert werden, damit alle Seiten und Bilder im E-Katalog angezeigt werden können.

* **Suchbegriffe extrahieren (optional)**: Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL PDF-Optionen]** aus. Wählen Sie in der Dropdown-Liste &quot;Extract&quot;die Option **[!UICONTROL Suchbegriffe]** aus, wenn Sie möchten, dass Ihre Viewer in Ihrem E-Katalog nach Suchbegriffen suchen können.

* **E-Katalog aus mehreren Seiten automatisch generieren (optional)**: Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL PDF-Optionen]** aus. Klicken Sie auf **[!UICONTROL E-Katalog von mehreren Seiten automatisch generieren]** , damit Sie beim Hochladen automatisch einen E-Katalog erstellen können. Sie können dann sofort den Anzeigebereich „E-Katalog“ aufrufen und daran arbeiten, ohne zuerst PDF-Dateien auswählen und den Befehl „Erstellen“ aktivieren zu müssen. Der E-Katalog erhält in diesem Fall denselben Namen wie die PDF-Datei.

* **Auflösung**: Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL PDF-Optionen]** aus. Geben Sie im Textfeld **[!UICONTROL Auflösung]** einen Wert ein. Adobe Dynamic Media Classic empfiehlt 150 Pixel pro Zoll.

* **Farbraum**: Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL PDF-Optionen]** aus. Wählen Sie in der Dropdown-Liste Farbraum die Option **[!UICONTROL Automatisch erkennen]**. Normalerweise enthalten PDF-Dateien, die zum Drucken vorgesehen sind, CMYK-Bilder, während PDF-Dateien, die nur zum Anzeigen vorgesehen sind, RGB-Bilder enthalten. Wenn in einer PDF-Datei beide Farbräume verwendet wurden, können Sie einen bestimmten Farbraum auswählen, indem Sie „Immer RGB“ oder „Immer CMYK“ wählen. Zur Verwendung beider Farbräume innerhalb einer PDF-Datei kommt es, wenn Seitengrafiken im CMYK-Farbraum und Bilder im RGB-Farbraum verwendet werden. Wenn Sie ein ICC-Profil hochgeladen haben, wird dessen Name zur Auswahl im Menü „Farbraum“ angezeigt. 

  Siehe [ICC-Profile (International Color Consortium)](/help/using/icc-profiles.md).

* **Farbprofiloptionen**: Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL Farbprofiloptionen]** und wählen Sie dann eine Farbprofiloption:

   * **Ursprünglichen Farbraum beibehalten**: Behält den ursprünglichen Farbraum bei.

   * **Benutzerdefiniert von > bis**: Öffnet Untermenüs, damit Sie einen Farbraum **[!UICONTROL Konvertieren von]** und **[!UICONTROL Konvertieren in]** auswählen können. Sie können einen standardmäßigen Photoshop-Farbraum oder einen Farbraum auswählen, den Sie in Adobe Dynamic Media Classic hochgeladen haben.

<!-- * **Convert To SRGB**: Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on Web pages. -->

Siehe [ICC-Profile (International Color Consortium)](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Details zu allen PDF-Optionen finden Sie unter [Optionen für das Hochladen von PDF-Dateien](pdfs.md#pdf_upload_options).
