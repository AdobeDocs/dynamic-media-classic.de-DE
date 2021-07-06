---
title: Hochladen der PDF-Dateien
description: Erfahren Sie, wie Sie die mit einem eCatalog verknüpften PDF-Dateien hochladen.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 44%

---

# Hochladen der PDF-Dateien{#uploading-the-pdf-files}

In der Regel sind Adobe PDF-Dateien die Quelle für einen eCatalog. Diese Dateien enthalten alle Bildinformationen, Schriftarten und Vektorgrafiken. Sie können einen E-Katalog jedoch auch auf Grundlage von Bildern erstellen. Nachdem Sie die PDF-Dateien zum Hochladen vorbereitet haben, klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Upload]** , um mit dem Hochladen der PDF-Dateien zu beginnen.

## Vorbereiten der PDF-Dateien {#preparing-your-pdf-files}

Bereiten Sie Ihre PDF-Dateien vor dem Hochladen in Dynamic Media Classic vor:

* Um das Hochladen der Dateien zu vereinfachen, platzieren Sie alle Dateien im selben Ordner auf Ihrem Computer oder Netzwerk.
* Benennen Sie die Dateien in alphanumerischer Reihenfolge gemäß der gewünschten Seitenabfolge. Eine Vorabsortierung der Seiten erleichtert nach dem Hochladen die Anordnung der Dateien in der richtigen Reihenfolge.
* Um zu sehen, ob PDF-Seiten Zuschnittmarkierungen, Registrierungsziele oder Farbbalken enthalten, überprüfen Sie die Seiten. Diese Markierungen kennzeichnen die Stellen, an denen das Papier beim Druck abgeschnitten werden soll. Sie müssen vor der Veröffentlichung des E-Katalogs im Internet entfernt werden. Dynamic Media Classic bietet Optionen für Zuschnittmarkierungen beim Hochladen von PDF-Dateien.
* Wenn Sie möchten, dass Betrachter der Website den E-Katalog nach Schlüsselwörtern durchsuchen können, stellen Sie fest, ob es sich um reduzierte PDF-Dateien handelt. Aus reduzierten PDF-Dateien können keine Suchbegriffe extrahiert werden. Um festzustellen, ob eine PDF-Datei reduziert ist, versuchen Sie, Text darin zu markieren. Wenn Sie keinen Text auswählen können, wird die PDF-Datei reduziert und Viewer können in Ihrem eCatalog nicht nach Keywords suchen.
* Da PDF-Dateien speziell zum Drucken vorgesehen sind, enthalten sie normalerweise CMYK-Bilder. Standardmäßig kann Dynamic Media Classic diese CMYK-Bilder intelligent erkennen und mithilfe eines internen CMYK-Farbprofils konvertieren. Sie können zum Konvertieren der CMYK-Bilder auch ein benutzerdefiniertes Farbprofil verwenden. 

   Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

## Bewährte Optionen zum Hochladen von PDF-Dateien {#best-practice-pdf-upload-options}

Ausführliche Informationen zu den verschiedenen Methoden zum Hochladen finden Sie unter [Hochladen der Dateien](uploading-files.md#uploading_your_files).

Wählen Sie die hochzuladenden Dateien aus und beachten Sie die folgenden bewährten Optionen ** für PDF-Dateien:

* **Zuschnittoptionen**  - Klicken Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;auf &quot; **[!UICONTROL Zuschnittoptionen]**&quot;. Wenn die PDF-Seiten Zuschnittmarkierungen, Registrierungsmarkierungen oder andere Markierungen enthalten, wählen Sie in der Dropdownliste **[!UICONTROL Zuschneiden]** die Option **[!UICONTROL Manuell]**. Geben Sie die Anzahl der Pixel an, die an den Seitenkanten oben, rechts, unten und links abgeschnitten werden sollen. Zuschnittmarkierungen sind oft auf einen halben Zoll-Rand eingestellt. Angenommen, Sie wählen **[!UICONTROL 150]** (empfohlen) als Pixel-pro-Zoll-Auflösung und geben in die Textfelder oben, rechts, unten und links die Felder 75, 75, 75 und 75 ein. In diesem Fall schneidet er einen halben Zoll von den Rändern ab (bei 150 ppi, die Hälfte von 1 entspricht 75 Pixel).

* **Verarbeitung**  - Klicken Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;auf  **[!UICONTROL PDF-Optionen]**. Wählen Sie in der Dropdownliste **[!UICONTROL Verarbeitung]** die Option **[!UICONTROL Rastern]**. Die PDF-Datei muss gerastert werden, damit alle Seiten und Bilder im E-Katalog angezeigt werden können.

* **Suchbegriffe extrahieren (optional)**  - Klicken Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;auf  **[!UICONTROL PDF-Optionen]**. Wählen Sie in der Dropdown-Liste Extract die Option **[!UICONTROL Suchbegriffe]** aus, wenn Ihre Viewer in der Lage sein sollen, in Ihrem eCatalog nach Suchbegriffen zu suchen.

* **E-Katalog aus mehrseitiger PDF automatisch generieren (optional)**  - Klicken Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;auf  **[!UICONTROL PDF-Optionen]**. Wählen Sie **[!UICONTROL E-Katalog aus mehrseitigem PDF-Dokument automatisch erstellen]** aus, um beim Hochladen automatisch einen E-Katalog zu erstellen. Sie können dann sofort den Anzeigebereich „E-Katalog“ aufrufen und daran arbeiten, ohne zuerst PDF-Dateien auswählen und den Befehl „Erstellen“ aktivieren zu müssen. Der E-Katalog erhält in diesem Fall denselben Namen wie die PDF-Datei.

* **Lösung**  - Klicken Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;auf  **[!UICONTROL PDF-Optionen]**. Geben Sie im Textfeld **[!UICONTROL Auflösung]** einen Wert ein. Dynamic Media Classic empfiehlt 150 Pixel pro Zoll.

* **Farbraum**  - Klicken Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;auf  **[!UICONTROL PDF-Optionen]**. Wählen Sie in der Dropdown-Liste Farbraum die Option **[!UICONTROL Automatisch erkennen]** aus. Normalerweise enthalten PDF-Dateien, die zum Drucken vorgesehen sind, CMYK-Bilder, während PDF-Dateien, die nur zum Anzeigen vorgesehen sind, RGB-Bilder enthalten. Wenn in einer PDF-Datei beide Farbräume verwendet wurden, können Sie einen bestimmten Farbraum auswählen, indem Sie „Immer RGB“ oder „Immer CMYK“ wählen. Zur Verwendung beider Farbräume innerhalb einer PDF-Datei kommt es, wenn Seitengrafiken im CMYK-Farbraum und Bilder im RGB-Farbraum verwendet werden. Wenn Sie ein ICC-Profil hochgeladen haben, wird dessen Name zur Auswahl im Menü „Farbraum“ angezeigt. 

   Siehe [ICC-Profile](/help/icc-profiles.md).

* **Farbprofiloptionen**  - Klicken Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;auf  **[!UICONTROL Farbprofiloptionen]** und wählen Sie dann eine Farbprofiloption:

   * **Originalfarbraum beibehalten**  - Behält den ursprünglichen Farbraum bei.

   * **Benutzerdefiniert von > in**  - Öffnet Untermenüs, damit Sie einen  **[!UICONTROL Konvertierungsraum]** und  **[!UICONTROL einen]** Tocolor-Bereich auswählen können. Sie können einen standardmäßigen Photoshop-Farbraum oder einen Farbraum auswählen, den Sie in Dynamic Media Classic hochgeladen haben.

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Details zu allen PDF-Optionen finden Sie unter [Optionen für das Hochladen von PDF-Dateien](pdfs.md#pdf_upload_options).
