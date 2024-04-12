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
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 50%

---

# ICC-Profile{#icc-profiles}

In einem ICC-Profil (International Color Consortium) wird beschrieben, wie Bilddateien korrekt von einem Farbraum in einen anderen konvertiert werden. Mithilfe von ICC-Profilen werden die Bilder in korrekten Farben angezeigt. Um beispielsweise Bilder, die zum Drucken vorgesehen sind, korrekt auf einem Computerbildschirm anzuzeigen, können Sie ein ICC-Profil auswählen. Das Profil konvertiert die Bilder in einen anderen Farbraum und gewährleistet, dass die Farben auf dem Bildschirm korrekt angezeigt werden.

In Adobe Dynamic Media Classic können Sie beim Hochladen der Bilder ein ICC-Profil auswählen, um Bilder in einen anderen Farbraum zu konvertieren. Alle standardmäßigen Photoshop ICC-Profile sind standardmäßig in Adobe Dynamic Media Classic verfügbar. Um die Namen von Farbprofilen im Anzeigebereich „Hochladen“ anzuzeigen, wählen Sie im Menü „Farbprofil“ Wählen Sie dann Benutzerdefiniert von > In und wählen Sie einen ICC-Profilnamen in den Menüs Konvertiert von und Konvertiert in .

Siehe [Bildbearbeitungsoptionen beim Hochladen](image-editing-options-upload.md#image-editing-options-at-upload).

Sie können nicht nur die standardmäßigen ICC-Profile verwenden, sondern auch andere ICC-Profile in Adobe Dynamic Media Classic hochladen und für die Farbraumkonvertierung verfügbar machen. Wechseln Sie im Durchsuchenbedienfeld zur Detailansicht, um die Profilklasse, den Farbraumtyp und den PCS-Typ eines ICC-Profils zu untersuchen.

## ICC-Profile hochladen {#uploading-icc-profiles}

ICC-Profile werden genau so wie andere Dateien hochgeladen. Sie können ICC-Profile in einem beliebigen Adobe Dynamic Media Classic-Ordner speichern.

Siehe [Hochladen der Dateien](uploading-files.md#uploading_your_files).

## ICC-Profil prüfen {#examining-an-icc-profile}

Um ein ICC-Profil zu untersuchen, wählen Sie es im Durchsuchenbedienfeld aus und zeigen Sie es in der Detailansicht an. Die Detailansicht enthält diese Informationen zu ICC-Profilen:

* **[!UICONTROL Profilklasse]** - Das ICC (International Color Consortium) definiert jede Klasse, um eine Art von Anwendung abzudecken. Beispielsweise betreffen Eingabeprofile Geräte wie Digitalkameras und Scanner, während Ausgabeprofile Drucker betreffen.

* **[!UICONTROL Farbraumtyp]** - Diese Zahl ist der &quot;Eingabe&quot;-Farbraum des Profils, wie vom ICC definiert. Die Art des Farbraums definiert die Anzahl an Komponenten des Farbraums und deren Interpretation. Der RGB-Farbraum enthält beispielsweise drei Komponenten: Rot, Grün und Blau. Die Art des Farbraums gibt jedoch nicht die besonderen Farbcharakteristika des Farbraums an (z. B. die Chromatizität der Primärfarben).

* **[!UICONTROL PCS-Typ]** - Dieser PCS-Typ ist der &quot;Ausgabe&quot;-Farbraum des Profils - sein Profil-Verbindungsraum. Beispielsweise kann ein Farbprofil RGB in PCS konvertieren, von dem es anschließend in CMYK konvertiert wird.

Für Eingabe-, Anzeige- oder Ausgabeprofile, mit denen Farben oder Bilder mit Tags versehen werden können, ist der PCS-Typ entweder „XYZ“ oder „Lab“. Dieses Profil ist als der entsprechend bestimmte Farbraum gemäß der Definition der ICC-Spezifikation zu interpretieren.
