---
title: Einstellen von Bildvorgaben
description: Erfahren Sie, wie Sie Bildvorgaben einrichten.
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
feature: Dynamic Media Classic,Bildvorgaben
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 64%

---

# Einstellen von Bildvorgaben{#setting-up-image-presets}

Eine Bildvorgabe ähnelt einem Makro – es handelt sich um eine vordefinierte, mit gemeinsamem Namen gespeicherte Sammlung von Befehlen zur Größeneinstellung und Formatierung. Ein Beispiel zur Funktionsweise von Bildvorgaben: Angenommen, für Ihre Website wird jedes Produktbild in zwei unterschiedlichen Größen benötigt, einmal im Format 500 x 500 Pixel und einmal im Format 150 x 150 Pixel. Sie erstellen dann zwei Bildvorgaben, eine mit der Bezeichnung „Vergrößerung“ zum Anzeigen von Bildern mit 500 x 500 Pixeln, eine mit der Bezeichnung „Miniaturansicht“ zum Anzeigen von Bildern mit 150 x 150 Pixeln. Um Bilder in den Größen &quot;Vergrößern&quot;und &quot;Miniaturansicht&quot;bereitzustellen, sucht ein Dynamic Media-Bildserver nach der Definition der Bildvorgabe &quot;Vergrößern&quot;und der Bildvorgabe &quot;Miniaturansicht&quot;. Dann erstellt der Server dynamisch je ein Bild in der Größe und mit den Formatierungsangaben, die in den beiden Bildvorgaben gespeichert sind.

Dynamic Media Classic enthält mehrere Bildvorgaben, die bereits für die Verwendung durch Sie eingerichtet sind. Administratoren können auch neue Bildvorgaben erstellen. Sie können eine Bildvorgabe komplett neu erstellen oder eine vorhandene Bildvorgabe abwandeln und unter neuem Namen speichern.

Bei Bildern, deren Größe bei der dynamischen Bereitstellung von einem Server verringert wird, kann es zu einem Verlust an Schärfe und Detail kommen. Aus diesem Grund enthält jede Bildvorgabe Elemente zur Formatierungssteuerung, mit denen ein Bild bei Bereitstellung in einer bestimmten Größe optimiert wird. Ihre Bilder werden dadurch scharf und klar für die Website bzw. Anwendung bereitgestellt.

## Erstellen einer Bildvorgabe {#creating-an-image-preset}

Als Unternehmensadministrator haben Sie die Möglichkeit, eigene Bildvorgaben zu erstellen. Sie können neue Bildvorgaben erstellen oder mit einer standardmäßigen Bildvorgabe beginnen, die Dynamic Media Classic bereitstellt, sie bearbeiten und mit einem neuen Namen speichern.

**So erstellen Sie ein Bildvorgabe:**

1. Klicken Sie auf **„Einstellungen“** > **„Bildvorgaben“**.

   Hier können Sie den Namen einer Bildvorgabe auswählen, um die Vorschau einer vorhandenen Bildvorgabe einzublenden. Sobald Sie den Namen einer Bildvorgabe auswählen, ändern sich Größe und Aussehen des Beispielbilds im Vorschaufenster.

1. Führen Sie einen der folgenden Schritte aus:

   * **Erstellen einer Bildvorgabe**
Klicken Sie auf &quot;Hinzufügen&quot;.

   * **Bearbeiten einer Bildvorgabe**
Durchsuchen Sie die Bildvorgabe, die der Bildvorgabe am ehesten ähnelt, und klicken Sie auf Bearbeiten.

1. Geben Sie einen Namen für die Bildvorgabe ein.
1. Geben Sie die Breite und Höhe in Pixeln ein. Diese Werte bestimmen die Größe, in der Bilder bereitgestellt werden.
1. Füllen Sie die Felder im Anzeigebereich „Vorgabe hinzufügen“ bzw. „Vorgabe bearbeiten“ aus. Einzelheiten dazu finden Sie im Abschnitt [Optionen für Bildvorgaben](application-setup.md#image_preset_options).

   Dynamic Media Classic empfiehlt die folgenden Best Practice-Optionen, um zu beginnen:

   * ****
FormatChoose JPEG oder ein anderes Format, das Ihren Anforderungen entspricht. Alle Webbrowser unterstützen das JPEG-Bildformat. Es bietet eine gute Balance zwischen kleinen Dateigrößen und Bildqualität. Bilder im JPEG-Format verwenden jedoch ein verlustbehaftetes Komprimierungsschema, das unerwünschte Bildartefakte hervorrufen kann, wenn die Komprimierungseinstellung zu niedrig festgelegt ist. Daher empfiehlt Dynamic Media Classic, die Komprimierungsqualität (auf dem Regler) auf 75 festzulegen. Diese Einstellung bietet eine gute Balance zwischen Bildqualität und kleiner Dateigröße.

   * ****
ScharfzeichnenWählen Sie nicht Scharfzeichnen aus (dieser Scharfzeichnungsfilter bietet weniger Kontrolle als die Einstellungen für &quot;Unschärfemaske&quot;).

   * **Resample**
ModeChoose Bikubisch.

   * **Unschärfemaske (USM)-**
OptionenGeben Sie die folgenden Einstellungen ein:
   | Vorgabetyp | Größe | Unschärfem.: Betrag | Unschärfem.: Radius | Unschärfem.: Schwelle |
   |--- |--- |--- |--- |--- |
   | Cross-Selling (besonders kleine Miniaturansicht) | 75 x 75 | 1,5 | 0,8 | 5 |
   | Miniaturansicht | 150 x 150 | 1,1 | 1 | 5 |
   | Hauptansicht | 350 x 350 | 1 | 1 | 6 |
   | Vergrößerung | 500 x 500 | 1,2 | 1,2 | 5 |

1. Klicken Sie auf „**Speichern**“.

Die im Folgenden aufgeführten Dynamic Media Classic-Best Practice-Optionen zum Erstellen von Bildvorgaben sind allgemeine Empfehlungen. Scharfzeichnen ist sehr subjektiv. Die oben aufgeführten Einstellungen wurden für ein Masterbild der Größe 2000 x 2000 Pixel festgelegt; Einstellungen für größere oder kleinere Masterversionen können abweichen. Wenn Sie die Einstellungen für die Unschärfemaske anpassen möchten, empfiehlt Dynamic Media Classic die folgenden Bereiche:

* ****
AmountBetween .8 and 1.5.

* ****
RadiusZwischen .6 und 2.

* ****
Schwellenwert1-6.

Wenn Sie eine Bildvorgabe löschen möchten, wählen Sie sie im Anzeigebereich „Bildvorgaben“ aus und klicken Sie dann auf die Schaltfläche „Löschen“.

>[!MORELIKETHIS]
>
>* [Erstellen und Bearbeiten von Bildvorgaben](application-setup.md#creating_and_editing_image_presets)
* [Optionen für Bildvorgaben](application-setup.md#image_preset_options)
* [Anzeigen eines Bild-Asset auf Grundlage seiner Bildvorgabe](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

