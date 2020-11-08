---
title: Einstellen von Bildvorgaben
seo-title: Einstellen von Bildvorgaben
description: 'null'
seo-description: Erfahren Sie, wie Sie Bildvorgaben einrichten.
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 65%

---


# Einstellen von Bildvorgaben{#setting-up-image-presets}

Eine Bildvorgabe ähnelt einem Makro – es handelt sich um eine vordefinierte, mit gemeinsamem Namen gespeicherte Sammlung von Befehlen zur Größeneinstellung und Formatierung. Ein Beispiel zur Funktionsweise von Bildvorgaben: Angenommen, für Ihre Website wird jedes Produktbild in zwei unterschiedlichen Größen benötigt, einmal im Format 500 x 500 Pixel und einmal im Format 150 x 150 Pixel. Sie erstellen dann zwei Bildvorgaben, eine mit der Bezeichnung „Vergrößerung“ zum Anzeigen von Bildern mit 500 x 500 Pixeln, eine mit der Bezeichnung „Miniaturansicht“ zum Anzeigen von Bildern mit 150 x 150 Pixeln. Um Bilder in den Größen &quot;Vergrößern&quot;und &quot;Miniaturansicht&quot;bereitzustellen, sucht ein Dynamic Media-Image-Server die Definition der Bildvorgabe &quot;Vergrößern&quot;und &quot;Miniaturansicht&quot;. Dann erstellt der Server dynamisch je ein Bild in der Größe und mit den Formatierungsangaben, die in den beiden Bildvorgaben gespeichert sind.

Im Lieferumfang von Dynamic Media Classic sind verschiedene bewährte Bildvorgaben enthalten, die bereits für die Verwendung eingerichtet wurden. Administratoren können auch neue Bildvorgaben erstellen. Sie können eine Bildvorgabe komplett neu erstellen oder eine vorhandene Bildvorgabe abwandeln und unter neuem Namen speichern.

Bei Bildern, deren Größe bei der dynamischen Bereitstellung von einem Server verringert wird, kann es zu einem Verlust an Schärfe und Detail kommen. Aus diesem Grund enthält jede Bildvorgabe Elemente zur Formatierungssteuerung, mit denen ein Bild bei Bereitstellung in einer bestimmten Größe optimiert wird. Ihre Bilder werden dadurch scharf und klar für die Website bzw. Anwendung bereitgestellt.

## Erstellen einer Bildvorgabe {#creating-an-image-preset}

Als Unternehmensadministrator haben Sie die Möglichkeit, eigene Bildvorgaben zu erstellen. Sie können neue Bildvorgaben oder Beginn mit einer standardmäßigen Bildvorgabe erstellen, die von Dynamic Media Classic bereitgestellt wird, bearbeiten und mit einem neuen Namen speichern.

**So erstellen Sie ein Bildvorgabe**

1. Klicken Sie auf **„Einstellungen“** > **„Bildvorgaben“**.

   Hier können Sie den Namen einer Bildvorgabe auswählen, um die Vorschau einer vorhandenen Bildvorgabe einzublenden. Sobald Sie den Namen einer Bildvorgabe auswählen, ändern sich Größe und Aussehen des Beispielbilds im Vorschaufenster.

1. Führen Sie einen der folgenden Schritte aus:

   * **Erstellen einer Bildvorgabe** Klicken Sie auf Hinzufügen.

   * **Beim Bearbeiten einer Bildvorgabe** navigieren Sie zu der Bildvorgabe, die am ehesten der zu erstellenden ähnelt, und klicken Sie dann auf &quot;Bearbeiten&quot;.

1. Geben Sie einen Namen für die Bildvorgabe ein.
1. Geben Sie die Breite und Höhe in Pixeln ein. Diese Werte bestimmen die Größe, in der Bilder bereitgestellt werden.
1. Füllen Sie die Felder im Anzeigebereich „Vorgabe hinzufügen“ bzw. „Vorgabe bearbeiten“ aus. Einzelheiten dazu finden Sie im Abschnitt [Optionen für Bildvorgaben](application-setup.md#image_preset_options).

   Dynamic Media Classic empfiehlt für den Beginn die folgenden &quot;Best Practice&quot;-Optionen:

   * **Format** Wählen Sie JPEG oder ein anderes Format, das Ihren Anforderungen entspricht. Alle Webbrowser unterstützen das JPEG-Bildformat. Es bietet eine gute Balance zwischen kleinen Dateigrößen und Bildqualität. Bilder im JPEG-Format verwenden jedoch ein verlustbehaftetes Komprimierungsschema, das unerwünschte Bildartefakte hervorrufen kann, wenn die Komprimierungseinstellung zu niedrig festgelegt ist. Daher empfiehlt Dynamic Media Classic, die Komprimierungsqualität (auf dem Schieberegler) auf 75 einzustellen. Diese Einstellung bietet eine gute Balance zwischen Bildqualität und kleiner Dateigröße.

   * **Scharfzeichnen** Wählen Sie &quot;Scharfzeichnen&quot;nicht aus (diese Scharfzeichnungsfilter-Angebot haben weniger Kontrolle als die Einstellungen für &quot;Unschärfemaske&quot;).

   * **Resamplingmodus** wählen Sie &quot;bikubisch&quot;.

   * **Optionen** fürUnschärfemaske (USM) Geben Sie die folgenden Einstellungen ein:
   | Vorgabetyp | Größe | Unschärfem.: Betrag | Unschärfem.: Radius | Unschärfem.: Schwelle |
   |--- |--- |--- |--- |--- |
   | Cross-Selling (besonders kleine Miniaturansicht) | 75 x 75 | 1,5 | 0,8 | 5 |
   | Miniaturansicht | 150 x 150 | 1,1 | 1 | 5 |
   | Hauptansicht | 350 x 350 | 1 | 1 | 6 |
   | Vergrößerung | 500 x 500 | 1,2 | 1,2 | 5 |

1. Klicken Sie auf „**Speichern**“.

Die im Folgenden aufgeführten &quot;Best Practice&quot;-Optionen für die Erstellung von Bildvorgaben für dynamische Medien Classic sind allgemeine Empfehlungen. Scharfzeichnen ist hochgradig subjektiv. Die oben aufgeführten Einstellungen wurden für ein Masterbild der Größe 2000 x 2000 Pixel festgelegt; Einstellungen für größere oder kleinere Masterversionen können abweichen. Wenn Sie die Einstellungen für die Unschärfemaske anpassen möchten, empfiehlt Dynamic Media Classic die folgenden Bereiche:

* **Betrag** zwischen 0,8 und 1,5.

* **Radius** zwischen 0,6 und 2.

* **Schwellenwert** von 1-6.

Wenn Sie eine Bildvorgabe löschen möchten, wählen Sie sie im Anzeigebereich „Bildvorgaben“ aus und klicken Sie dann auf die Schaltfläche „Löschen“.

>[!MORELIKETHIS]
>
>* [Erstellen und Bearbeiten von Bildvorgaben](application-setup.md#creating_and_editing_image_presets)
>* [Optionen für Bildvorgaben](application-setup.md#image_preset_options)
>* [Anzeigen einer Bild-Asset-Vorschau auf Grundlage seiner Bildvorgabe](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

