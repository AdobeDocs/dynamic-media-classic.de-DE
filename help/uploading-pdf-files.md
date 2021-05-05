---
title: Hochladen der PDF-Dateien
description: Erfahren Sie, wie Sie die mit einem E-Katalog verknüpften PDF-Dateien hochladen.
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic, Viewer, E-Katalog
role: Business Practitioner
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
translation-type: tm+mt
source-git-commit: 06bd65c92c88595786b14213944a7cebd0d2590b
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 44%

---

# Hochladen der PDF-Dateien{#uploading-the-pdf-files}

Normalerweise werden Adobe PDF-Dateien als Quelle für einen E-Katalog verwendet. Diese Dateien enthalten alle Bildinformationen, Schriftarten und Vektorgrafiken. Sie können einen E-Katalog jedoch auch auf Grundlage von Bildern erstellen. Nachdem Sie die PDF-Dateien zum Hochladen vorbereitet haben, klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Hochladen]**, um mit dem Hochladen der PDF-Dateien zu beginnen.

## Vorbereiten der PDF-Dateien {#preparing-your-pdf-files}

Bereiten Sie die PDF-Dateien vor dem Hochladen in Dynamic Media Classic vor:

* Um das Hochladen der Dateien zu vereinfachen, legen Sie alle Dateien im selben Ordner auf Ihrem Computer oder im Netzwerk ab.
* Benennen Sie die Dateien in alphanumerischer Reihenfolge gemäß der gewünschten Seitenabfolge. Eine Vorabsortierung der Seiten erleichtert nach dem Hochladen die Anordnung der Dateien in der richtigen Reihenfolge.
* Um zu sehen, ob PDF-Zielgruppen Schnittmarken, Registrierungs- oder Farbleisten enthalten, überprüfen Sie die Seiten. Diese Markierungen kennzeichnen die Stellen, an denen das Papier beim Druck abgeschnitten werden soll. Sie müssen vor der Veröffentlichung des E-Katalogs im Internet entfernt werden. Dynamic Media Classic bietet Optionen für Schnittmarken, wenn Sie PDF-Dateien hochladen.
* Wenn Sie möchten, dass Betrachter der Website den E-Katalog nach Schlüsselwörtern durchsuchen können, stellen Sie fest, ob es sich um reduzierte PDF-Dateien handelt. Aus reduzierten PDF-Dateien können keine Suchbegriffe extrahiert werden. Um festzustellen, ob eine PDF-Datei reduziert ist, versuchen Sie, Text darin zu markieren. Wenn Sie keinen Text auswählen können, wird die PDF-Datei reduziert und die Viewer können nicht nach Schlüsselwörtern in Ihrem E-Katalog suchen.
* Da PDF-Dateien speziell zum Drucken vorgesehen sind, enthalten sie normalerweise CMYK-Bilder. Standardmäßig kann Dynamic Media Classic diese CMYK-Bilder intelligent erkennen und mithilfe eines internen CMYK-Profils konvertieren. Sie können zum Konvertieren der CMYK-Bilder auch ein benutzerdefiniertes Farbprofil verwenden. 

   Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

## Bewährte Optionen zum Hochladen von PDF-Dateien  {#best-practice-pdf-upload-options}

Ausführliche Informationen zu den verschiedenen Methoden zum Hochladen finden Sie unter [Hochladen der Dateien](uploading-files.md#uploading_your_files).

Wählen Sie die hochzuladenden Dateien aus und beachten Sie die folgenden bewährten Optionen ** für PDF-Dateien:

* **Beschneidungsoptionen** : Klicken Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;auf  **[!UICONTROL Beschneidungsoptionen]**. Wenn die PDF-Seiten Schnittmarken, Registrierungsmarken oder andere Zeichen enthalten, wählen Sie in der Dropdown-Liste **[!UICONTROL Zuschneiden]** **[!UICONTROL Manuell]**. Geben Sie die Anzahl der Pixel an, die an den Seitenkanten oben, rechts, unten und links abgeschnitten werden sollen. Schnittmarken werden oft auf einen halben Zoll-Rand eingestellt. Angenommen, Sie wählen **[!UICONTROL 150]** (empfohlen) als Auflösung von Pixel pro Zoll und geben in die Textfelder &quot;Oben&quot;, &quot;Rechts&quot;, &quot;Unten&quot;und &quot;Links&quot;die Werte 75, 75, 75 und 75 ein. In diesem Fall wird ein halber Zoll von den Rändern abgeschnitten (bei 150 ppi, die Hälfte von 1 gleich 75 Pixel).

* **Verarbeitung** : Klicken Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;auf  **[!UICONTROL PDF-Optionen]**. Wählen Sie in der Dropdown-Liste **[!UICONTROL Verarbeitung]** **[!UICONTROL Rastern]**. Die PDF-Datei muss gerastert werden, damit alle Seiten und Bilder im E-Katalog angezeigt werden können.

* **Suchbegriffe extrahieren (optional)**  - Klicken Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;auf  **[!UICONTROL PDF-Optionen]**. Wählen Sie in der Dropdown-Liste &quot;Extrahieren&quot;die Option **[!UICONTROL Suchbegriffe]**, wenn Ihre Viewer in der Lage sein sollen, nach Suchbegriffen in Ihrem E-Katalog zu suchen.

* **E-Katalog aus mehrseitiger PDF automatisch erstellen (optional)**  - Klicken Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;auf  **[!UICONTROL PDF-Optionen]**. Wählen Sie **[!UICONTROL E-Katalog aus mehrseitigem PDF]** automatisch erstellen, um beim Hochladen automatisch einen E-Katalog zu erstellen. Sie können dann sofort den Anzeigebereich „E-Katalog“ aufrufen und daran arbeiten, ohne zuerst PDF-Dateien auswählen und den Befehl „Erstellen“ aktivieren zu müssen. Der E-Katalog erhält in diesem Fall denselben Namen wie die PDF-Datei.

* **Lösung** : Klicken Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;auf  **[!UICONTROL PDF-Optionen]**. Geben Sie im Textfeld **[!UICONTROL Auflösung]** einen Wert ein. Dynamic Media Classic empfiehlt 150 Pixel pro Zoll.

* **Farbraum** : Klicken Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;auf  **[!UICONTROL PDF-Optionen]**. Wählen Sie in der Dropdown-Liste &quot;Farbraum&quot;die Option **[!UICONTROL Automatisch erkennen]**. Normalerweise enthalten PDF-Dateien, die zum Drucken vorgesehen sind, CMYK-Bilder, während PDF-Dateien, die nur zum Anzeigen vorgesehen sind, RGB-Bilder enthalten. Wenn in einer PDF-Datei beide Farbräume verwendet wurden, können Sie einen bestimmten Farbraum auswählen, indem Sie „Immer RGB“ oder „Immer CMYK“ wählen. Zur Verwendung beider Farbräume innerhalb einer PDF-Datei kommt es, wenn Seitengrafiken im CMYK-Farbraum und Bilder im RGB-Farbraum verwendet werden. Wenn Sie ein ICC-Profil hochgeladen haben, wird dessen Name zur Auswahl im Menü „Farbraum“ angezeigt. 

   Siehe [ICC-Profile](/help/icc-profiles.md).

* **Optionen**  für farbiges Profil: Klicken Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;auf  **[!UICONTROL Farboptionen]** und wählen Sie dann eine Profil-Farboption:

   * **Ursprünglichen Farbraum**  beibehalten: Behält den ursprünglichen Farbraum bei.

   * **Benutzerdefiniert von > in**  - Öffnet Untermenüs, in denen Sie einen  **[!UICONTROL Konvertierungsraum]** und einen  **[!UICONTROL Tocolor-]** Konvertierungsbereich auswählen können. Sie können einen Photoshop-Standardfarbraum oder einen Farbraum auswählen, den Sie in Dynamic Media Classic hochgeladen haben.

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

Siehe [ICC-Profile](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>Details zu allen PDF-Optionen finden Sie unter [Optionen für das Hochladen von PDF-Dateien](pdfs.md#pdf_upload_options).
