---
title: ICC-Profile
description: Erfahren Sie mehr über ICC-Profile.
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 71%

---

# ICC-Profile{#icc-profiles}

In einem ICC-Profil (International Color Consortium) wird beschrieben, wie Bilddateien korrekt von einem Farbraum in einen anderen konvertiert werden. Mithilfe von ICC-Profilen werden die Bilder in korrekten Farben angezeigt. Um beispielsweise Bilder, die zum Drucken vorgesehen sind, korrekt auf einem Computerbildschirm anzuzeigen, können Sie ein ICC-Profil auswählen. Das Profil konvertiert die Bilder in einen anderen Farbraum und gewährleistet, dass die Farben auf dem Bildschirm korrekt angezeigt werden.

In Dynamic Media Classic können Sie beim Hochladen der Bilder ein ICC-Profil auswählen, um Bilder in einen anderen Farbraum zu konvertieren. Alle standardmäßigen Photoshop ICC-Profile sind standardmäßig in Dynamic Media Classic verfügbar. Um die Namen von Farbprofilen im Anzeigebereich „Hochladen“ anzuzeigen, wählen Sie im Menü „Farbprofil“ die Option „Benutzerdefinierte Einstellung von > in“ und wählen Sie anschließend in den Menüs „Konvertieren von“ und „Konvertieren in“ die entsprechenden ICC-Profilnamen aus.

Siehe [Bildbearbeitungsoptionen beim Hochladen](image-editing-options-upload.md#image-editing-options-at-upload).

Sie können nicht nur die standardmäßigen ICC-Profile verwenden, sondern auch andere ICC-Profile in Dynamic Media Classic hochladen und für die Farbraumkonvertierung verfügbar machen. Rufen Sie die Detailansicht des Durchsuchenbedienfelds auf, um die Einstellungen für „Profil-Kategorie“, „Art des Farbraums“ und „PCS-Typ“ eines ICC-Profils zu ermitteln.

## Hochladen von ICC-Profilen {#uploading-icc-profiles}

ICC-Profile werden genau so wie andere Dateien hochgeladen. Sie können ICC-Profile in einem beliebigen Dynamic Media Classic-Ordner speichern.

Siehe [Hochladen der Dateien](uploading-files.md#uploading_your_files).

## Überprüfen von ICC-Profilen {#examining-an-icc-profile}

Um ein ICC-Profil zu überprüfen, zeigen Sie es in der Detailansicht des Durchsuchenbedienfelds an. Die Detailansicht enthält folgende Informationen zu ICC-Profilen:

* **Profilklasse**  - Das ICC (International Color Consortium) definiert jede Klasse, um einen Anwendungstyp abzudecken. Beispielsweise betreffen Eingabeprofile Geräte wie Digitalkameras und Scanner, während Ausgabeprofile Drucker betreffen.

* **Farbraumtyp**  - Diese Zahl ist der &quot;Eingabe&quot;-Farbraum des Profils, wie vom ICC definiert. Die Art des Farbraums definiert die Anzahl an Komponenten des Farbraums und deren Interpretation. Der RGB-Farbraum enthält beispielsweise drei Komponenten: Rot, Grün und Blau. Die Art des Farbraums gibt jedoch nicht die besonderen Farbcharakteristika des Farbraums an (z. B. die Chromatizität der Primärfarben).

* **PCS-Typ**  - Dieser PCS-Typ ist der &quot;Ausgabe&quot;-Farbraum des Profils - sein Profil-Verbindungsraum. Beispielsweise kann ein Farbprofil RGB in PCS konvertieren, von dem es anschließend in CMYK konvertiert wird.

Für Eingabe-, Anzeige- oder Ausgabeprofile, mit denen Farben oder Bilder mit Tags versehen werden können, ist der PCS-Typ entweder „XYZ“ oder „Lab“. Dieses Profil ist als der entsprechend bestimmte Farbraum gemäß der Definition der ICC-Spezifikation zu interpretieren.
