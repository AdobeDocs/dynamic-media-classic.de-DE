---
title: ICC-Profile
seo-title: ICC-Profile
description: 'null'
seo-description: Erfahren Sie mehr über ICC-Profile.
uuid: 708 ff 2 ad -9 a 47-4 e 3 e-b 643-5 b 19648 f 726 b
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/support_ files
discoiquuid: 44 f 1 b 4 c 4-6 d 7 f -4 e 0 f -84 ce -11 d 26745 e 0 f 0
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# ICC-Profile{#icc-profiles}

In einem ICC-Profil (International Color Consortium) wird beschrieben, wie Bilddateien korrekt von einem Farbraum in einen anderen konvertiert werden. Mithilfe von ICC-Profilen werden die Bilder in korrekten Farben angezeigt. Um beispielsweise Bilder, die zum Drucken vorgesehen sind, korrekt auf einem Computerbildschirm anzuzeigen, können Sie ein ICC-Profil auswählen. Das Profil konvertiert die Bilder in einen anderen Farbraum und gewährleistet, dass die Farben auf dem Bildschirm korrekt angezeigt werden.

Im Scene7 Publishing System können Sie beim Hochladen der Bilder ein ICC-Profil auswählen, mit dem die Bilder in einen anderen Farbraum konvertiert werden. Alle ICC-Standardprofile für Photoshop sind standardmäßig in SPS verfügbar. Um die Namen von Farbprofilen im Anzeigebereich „Hochladen“ anzuzeigen, wählen Sie im Menü „Farbprofil“ die Option „Benutzerdefinierte Einstellung von &gt; in“ und wählen Sie anschließend in den Menüs „Konvertieren von“ und „Konvertieren in“ die entsprechenden ICC-Profilnamen aus. Siehe [Bildbearbeitungsoptionen beim Hochladen](image-editing-options-upload.md#image-editing-options-at-upload).

Neben der Verwendung der ICC-Standardprofile können Sie auch andere ICC-Profile in SPS hochladen und für die Farbraumkonvertierung zur Verfügung stellen. Rufen Sie die Detailansicht des Durchsuchenbedienfelds auf, um die Einstellungen für „Profil-Kategorie“, „Art des Farbraums“ und „PCS-Typ“ eines ICC-Profils zu ermitteln.

## Hochladen von ICC-Profilen {#uploading-icc-profiles}

ICC-Profile werden genau so wie andere Dateien hochgeladen. Sie können ICC-Profile in einem beliebigen SPS-Ordner speichern. Siehe [Hochladen der Dateien](uploading-files.md#uploading_your_files).

## Überprüfen von ICC-Profilen {#examining-an-icc-profile}

Um ein ICC-Profil zu überprüfen, zeigen Sie es in der Detailansicht des Durchsuchenbedienfelds an. Die Detailansicht enthält folgende Informationen zu ICC-Profilen:

**Profil-Klasse** Das ICC (International Color Consortium) definiert jede Klasse, um einen Anwendungstyp zu behandeln. Beispielsweise betreffen Eingabeprofile Geräte wie Digitalkameras und Scanner, während Ausgabeprofile Drucker betreffen.

**Farbraum-Typ** Diese Zahl ist der "input" -Farbraum des Profils, der vom ICC definiert wird. Die Art des Farbraums definiert die Anzahl an Komponenten des Farbraums und deren Interpretation. Der RGB-Farbraum enthält beispielsweise drei Komponenten: Rot, Grün und Blau. Die Art des Farbraums gibt jedoch nicht die besonderen Farbcharakteristika des Farbraums an (z. B. die Chromatizität der Primärfarben).

**PCS-Typ** Dieser PCS-Typ ist der "Ausgabe" -Farbraum des Profils - der Verbindungsfarbraum. Beispielsweise kann ein Farbprofil RGB in PCS konvertieren, von dem es anschließend in CMYK konvertiert wird.

Für Eingabe-, Anzeige- oder Ausgabeprofile, mit denen Farben oder Bilder mit Tags versehen werden können, ist der PCS-Typ entweder „XYZ“ oder „Lab“. Dieses Profil ist als der entsprechend bestimmte Farbraum gemäß der Definition der ICC-Spezifikation zu interpretieren.
