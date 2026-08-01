---
title: ICC-Profile (International Color Consortium)
description: Erfahren Sie mehr über ICC-Profile in Adobe Dynamic Media Classic.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
topic: Administration, Content Management
level: Intermediate
autotag-review: '2026-05-13T19:59:42.608Z'
TQID: 'https://experienceleague.adobe.com/eGKamqA47mITzfyTuHoFYLfWEXOP0jAl5XWDpihGjZA'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 5cf4a3f436cd6dd46ee68daeb0ef798402ae311a
workflow-type: tm+mt
source-wordcount: 527
ht-degree: 29%

---

# ICC-Profile{#icc-profiles}

Ein ICC-Profil (International Color Consortium) ist eine Datei, die beschreibt, wie Sie Bilddateien korrekt von einem Farbraum in einen anderen konvertieren können. Mithilfe von ICC-Profilen werden die Bilder in korrekten Farben angezeigt. Um beispielsweise Bilder, die zum Drucken vorgesehen sind, korrekt auf einem Computerbildschirm anzuzeigen, können Sie ein ICC-Profil auswählen. Das Profil konvertiert die Bilder in einen anderen Farbraum und gewährleistet, dass die Farben auf dem Bildschirm korrekt angezeigt werden.

In Adobe Dynamic Media Classic können Sie ein ICC-Profil auswählen, um Bilder beim Hochladen in einen anderen Farbraum zu konvertieren. Alle standardmäßigen Adobe Photoshop ICC-Profile sind standardmäßig in Adobe Dynamic Media Classic verfügbar. Um die Namen von Farbprofilen im Anzeigebereich „Hochladen“ anzuzeigen, wählen Sie im Menü „Farbprofil“ Klicken Sie dann auf **Benutzerdefiniert** > **An** und wählen Sie einen ICC-Profilnamen in den Menüs **Konvertiert von** und **Konvertiert in** aus.

Siehe [Optionen zur Bildbearbeitung beim Hochladen](image-editing-options-upload.md#image-editing-options-at-upload).

Neben der Verwendung der standardmäßigen ICC-Profile können Sie weitere ICC-Profile in Adobe Dynamic Media Classic hochladen und für die Farbraumkonvertierung verfügbar machen. Um die Profilklasse, den Farbraumtyp und den PCS-Typ eines ICC-Profils zu untersuchen, wechseln Sie im Durchsuchen-Panel zur Detailansicht.

Zusammenfassend lässt sich sagen, dass die wichtigsten Punkte für ICC-Profile folgende sind:

* ICC-Profile ermöglichen eine korrekte Farbkonvertierung zwischen verschiedenen Farbräumen für Bilddateien.
* Adobe Dynamic Media Classic umfasst alle standardmäßigen Adobe Photoshop ICC-Profile für zuverlässige Bildkonvertierungen.
* Benutzerdefinierte ICC-Profile bieten mehr Flexibilität für erweiterte Farbraumkonvertierungsanforderungen.
* Die Anzeige von Details wie Profil-Klasse und PCS-Typ in der Detailansicht hilft Ihnen bei der Verwaltung von ICC-Einstellungen.
* Das Hochladen von ICC-Profilen ist einfach und stellt den Zugriff über Ordner in [!DNL Adobe Dynamic Media Classic] sicher.


## ICC-Profile hochladen {#uploading-icc-profiles}

Hochladen von ICC-Profilen mit denselben Methoden, die Sie zum Hochladen von Dateien verwenden. Sie können ICC-Profile in einem beliebigen Adobe Dynamic Media Classic-Ordner speichern.

Siehe [Hochladen von Dateien](uploading-files.md#uploading_your_files).

## Überprüfen eines ICC-Profils {#examining-an-icc-profile}

Um ein ICC-Profil zu untersuchen, wählen Sie es im Durchsuchen-Panel aus und zeigen Sie es in der Detailansicht an. Die Detailansicht enthält diese Informationen zu ICC-Profilen:

* **[!UICONTROL Profile Class]**: Die ICC definiert jede Klasse für einen Anwendungstyp. Eingabeprofile gelten beispielsweise für Geräte wie Digitalkameras und Scanner. Ausgabeprofile gelten für Drucker.

* **[!UICONTROL Farbraumtyp]**: Dieser Wert ist der „Eingabe“-Farbraum des Profils, wie vom ICC definiert. Die Art des Farbraums definiert die Anzahl an Komponenten des Farbraums und deren Interpretation. Der RGB-Farbraum enthält beispielsweise drei Komponenten: Rot, Grün und Blau. Die Art des Farbraums gibt jedoch nicht die besonderen Farbcharakteristika des Farbraums an (z. B. die Chromatizität der Primärfarben).

* **[!UICONTROL PCS-]**: Dieser PCS-Typ ist der „Ausgabe“-Farbraum des Profils - der Profilverbindungsraum. Beispielsweise kann ein Farbprofil RGB in PCS konvertieren, von dem es anschließend in CMYK konvertiert wird.

Für ein Eingabe-, Anzeige- oder Ausgabeprofil, das zum Tagging von Farben oder Bildern nützlich ist, ist der PCS-Typ entweder XYZ oder Lab. Dieses Profil ist als der entsprechend bestimmte Farbraum gemäß der Definition der ICC-Spezifikation zu interpretieren.
