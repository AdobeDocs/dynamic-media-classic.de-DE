---
title: Einstellen von Bildvorgaben
seo-title: Einstellen von Bildvorgaben
description: 'null'
seo-description: Hier erfahren Sie, wie Sie Bildvorgaben einrichten.
uuid: 90530948-dee 9-41 bd-b 39 e -684140446 abc
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/image_ sizing
discoiquuid: 1 ec 39 fe 5-7 b 2 a -4034-9570-6 b 5595 f 97052
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Einstellen von Bildvorgaben{#setting-up-image-presets}

Eine Bildvorgabe ähnelt einem Makro – es handelt sich um eine vordefinierte, mit gemeinsamem Namen gespeicherte Sammlung von Befehlen zur Größeneinstellung und Formatierung. Ein Beispiel zur Funktionsweise von Bildvorgaben: Angenommen, für Ihre Website wird jedes Produktbild in zwei unterschiedlichen Größen benötigt, einmal im Format 500 x 500 Pixel und einmal im Format 150 x 150 Pixel. Sie erstellen dann zwei Bildvorgaben, eine mit der Bezeichnung „Vergrößerung“ zum Anzeigen von Bildern mit 500 x 500 Pixeln, eine mit der Bezeichnung „Miniaturansicht“ zum Anzeigen von Bildern mit 150 x 150 Pixeln. Um Bilder in der Größe "Vergrößerung" und" Miniaturansicht" bereitzustellen, sucht ein dynamischer Medienserver nach der Definition der Vergrößerungsbildvorgabe und der Bildvorgabe für Miniaturansichten. Dann erstellt der Server dynamisch je ein Bild in der Größe und mit den Formatierungsangaben, die in den beiden Bildvorgaben gespeichert sind.

Dynamic Media Classic verfügt über eine Reihe von Bildvorgaben, die mit Best Practices erstellt wurden und bereits für Sie eingerichtet wurden. Administratoren können auch neue Bildvorgaben erstellen. Sie können eine Bildvorgabe komplett neu erstellen oder eine vorhandene Bildvorgabe abwandeln und unter neuem Namen speichern.

Bei Bildern, deren Größe bei der dynamischen Bereitstellung von einem Server verringert wird, kann es zu einem Verlust an Schärfe und Detail kommen. Aus diesem Grund enthält jede Bildvorgabe Elemente zur Formatierungssteuerung, mit denen ein Bild bei Bereitstellung in einer bestimmten Größe optimiert wird. Ihre Bilder werden dadurch scharf und klar für die Website bzw. Anwendung bereitgestellt.

## Erstellen einer Bildvorgabe {#creating-an-image-preset}

Als Unternehmensadministrator haben Sie die Möglichkeit, eigene Bildvorgaben zu erstellen. Sie können neue Bildvorgaben erstellen oder mit einer standardmäßigen Bildvorgabe beginnen, die von Dynamic Media Classic bereitgestellt, bearbeitet und unter einem neuen Namen gespeichert wird.

**So erstellen Sie ein Bildvorgabe**

1. Klicken Sie auf **„Einstellungen“** &gt; **„Bildvorgaben“**.

   Hier können Sie den Namen einer Bildvorgabe auswählen, um die Vorschau einer vorhandenen Bildvorgabe einzublenden. Sobald Sie den Namen einer Bildvorgabe auswählen, ändern sich Größe und Aussehen des Beispielbilds im Vorschaufenster.

1. Führen Sie einen der folgenden Schritte aus:

   **Erstellen einer
Bildvorgabe** klicken Sie auf "Hinzufügen" .

   **Bearbeiten einer Bildvorgabe** zur Bildvorgabe, die am häufigsten der zu erstellenden Bildvorgabe entspricht, und klicken Sie dann auf Bearbeiten.

1. Geben Sie einen Namen für die Bildvorgabe ein.
1. Geben Sie die Breite und Höhe in Pixeln ein. Diese Werte bestimmen die Größe, in der Bilder bereitgestellt werden.
1. Füllen Sie die Felder im Anzeigebereich „Vorgabe hinzufügen“ bzw. „Vorgabe bearbeiten“ aus. Einzelheiten dazu finden Sie im Abschnitt [Optionen für Bildvorgaben](application-setup.md#image_preset_options).

   Dynamic Media Classic empfiehlt diese bewährten Optionen für den Start:

   **Format** Wählen Sie JPEG oder ein anderes Format, das Ihren Anforderungen entspricht. Das Bildformat JPEG wird von allen Webbrowsern unterstützt; es bietet Ausgewogenheit in Bezug auf geringe Dateigröße einerseits und hohe Bildqualität andererseits. Das JPEG-Format ist allerdings mit einer verlustbehafteten Komprimierung verbunden; bei zu hoch eingestellter Komprimierung können unerwünschte Bildartefakte entstehen. Aus diesem Grund empfiehlt Dynamic Media Classic, die Komprimierungsqualität (im Schieberegler) auf 75 einzustellen. Mit dieser Einstellung erreichen Sie eine angemessene Bildqualität bei ausreichend kleiner Dateigröße.

   **Beim Scharfzeichnen** wird kein Scharfzeichnen ausgewählt (dieser Scharfzeichnungsfilter bietet weniger Kontrolle als die Unschärfemaske-Einstellungen).

   **Resamplingmodus** Wählen Sie "Bikubisch" .

   **Optionen für Unschärfemaske (USM)** Geben Sie die hier gezeigten Einstellungen ein:

   | Vorgabetyp | Größe | Unschärfem.: Betrag | Unschärfem.: Radius | Unschärfem.: Schwelle |
   |--- |--- |--- |--- |--- |
   | Cross-Selling (besonders kleine Miniaturansicht) | 75 x 75 | 1,5 | 0,8 | 5 |
   | Miniaturansicht | 150 x 150 | 1,1 | 1 | 5 |
   | Hauptansicht | 350 x 350 | 1 | 1 | 6 |
   | Vergrößerung | 500 x 500 | 1,2 | 1,2 | 5 |

1. Klicken Sie auf „**Speichern**“.

Die "Best Practice" -Optionen für dynamische Medien zum Erstellen von Bildvorgaben, die hier aufgelistet sind, sind allgemeine Empfehlungen. Scharfzeichnen ist sehr subjektiv. Die oben aufgeführten Einstellungen wurden für ein Masterbild der Größe 2000 x 2000 Pixel festgelegt; Einstellungen für größere oder kleinere Masterversionen können abweichen. Wenn Sie die Unschärfemaske-Einstellungen anpassen möchten, empfiehlt Dynamic Media Classic diese Bereiche:

**Betrag** zwischen 0,8 und 1,5.

**Radius** zwischen .6 und 2.

**Schwellenwert** von 1-6.

Wenn Sie eine Bildvorgabe löschen möchten, wählen Sie sie im Anzeigebereich „Bildvorgaben“ aus und klicken Sie dann auf die Schaltfläche „Löschen“.

>[!MORELIKETHIS]
>
>* [Erstellen und Bearbeiten von Bildvorgaben](application-setup.md#creating_and_editing_image_presets)
>* [Optionen für Bildvorgaben](application-setup.md#image_preset_options)
>* [Anzeigen einer Bild-Asset-Vorschau auf Grundlage seiner Bildvorgabe](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

