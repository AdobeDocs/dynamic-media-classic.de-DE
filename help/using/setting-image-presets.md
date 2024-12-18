---
title: Einrichten von Bildvorgaben
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic Bildvorgaben einrichten.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 32%

---

# Einrichten von Bildvorgaben{#setting-up-image-presets}

Eine Bildvorgabe ähnelt einem Makro – es handelt sich um eine vordefinierte, mit gemeinsamem Namen gespeicherte Sammlung von Befehlen zur Größeneinstellung und Formatierung. Nehmen wir an, dass für Ihre Website jedes Produktbild in zwei verschiedenen Größen angezeigt werden muss, um zu verstehen, wie Bildvorgaben funktionieren: 500 × 500 Pixel und 150 × 150 Pixel. Sie erstellen zwei Bildvorgaben, eine mit dem Namen „Vergrößern“ zur Anzeige von Bildern mit einer Auflösung von 500 x 500 Pixel und die andere mit dem Namen „Miniaturansicht“ zur Anzeige von Bildern mit einer Auflösung von 150 × 150 Pixel. Zum Übermitteln von Bildern mit den Größen „Vergrößern“ und „Miniaturansicht“ sucht ein Dynamic Media-Bildserver nach der Definition der Bildvorgabe „Vergrößern“ und „Miniaturansicht“. Dann erstellt der Server dynamisch je ein Bild in der Größe und mit den Formatierungsangaben, die in den beiden Bildvorgaben gespeichert sind.

Adobe Dynamic Media Classic verfügt über mehrere „Best Practice“-Bildvorgaben, die bereits für die Verwendung durch Sie eingerichtet sind. Admins können auch Bildvorgaben erstellen. Sie können eine Bildvorgabe komplett neu erstellen oder eine vorhandene Bildvorgabe abwandeln und unter neuem Namen speichern.

Bei Bildern, deren Größe bei der dynamischen Bereitstellung von einem Server verringert wird, kann es zu einem Verlust an Schärfe und Detail kommen. Aus diesem Grund enthält jede Bildvorgabe Elemente zur Formatierungssteuerung, mit denen ein Bild bei Bereitstellung in einer bestimmten Größe optimiert wird. Mit diesen Steuerelementen wird sichergestellt, dass Ihre Bilder beim Versand an Ihre Website oder Anwendung scharf und klar sind.

## Erstellen einer Bildvorgabe {#creating-an-image-preset}

Wenn Sie ein Unternehmensadministrator sind, können Sie Ihre eigenen Bildvorgaben erstellen. Sie können Bildvorgaben erstellen oder mit einer von Adobe Dynamic Media Classic bereitgestellten Standardbildvorgabe beginnen, sie bearbeiten und unter einem neuen Namen speichern.

**So erstellen Sie eine Bildvorgabe:**

1. Navigieren Sie **[!UICONTROL Setup]** > **[!UICONTROL Bildvorgaben]**.

   Hier können Sie den Namen einer Bildvorgabe auswählen, um die Vorschau einer vorhandenen Bildvorgabe einzublenden. Sobald Sie den Namen einer Bildvorgabe auswählen, ändern sich Größe und Aussehen des Beispielbilds im Vorschaufenster.

1. Führen Sie einen der folgenden Schritte aus:

   * **Erstellen einer Bildvorgabe**: Wählen Sie **[!UICONTROL Hinzufügen]**.
   * **Bearbeiten einer Bildvorgabe**: Navigieren Sie zu der Bildvorgabe, die der am meisten ähnelt, die Sie erstellen möchten, und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

1. Geben Sie einen Namen für die Bildvorgabe ein.
1. Geben Sie die Breite und Höhe in Pixeln ein. Diese Werte bestimmen die Größe, in der Bilder bereitgestellt werden.
1. Füllen Sie die Felder im Anzeigebereich „Vorgabe hinzufügen“ bzw. „Vorgabe bearbeiten“ aus. Einzelheiten dazu finden Sie im Abschnitt [Optionen für Bildvorgaben](application-setup.md#image_preset_options).

   Adobe Dynamic Media Classic empfiehlt zu Beginn die folgenden „Best Practice“-Optionen:

   * **[!UICONTROL Format]**: Wählen Sie JPEG oder ein anderes Format, das Ihren Anforderungen entspricht. Alle Webbrowser unterstützen das JPEG-Bildformat. Es bietet eine gute Balance zwischen kleinen Dateigrößen und Bildqualität. JPEG-Bilder verwenden jedoch ein verlustbehaftetes Komprimierungsschema, das bei zu niedriger Komprimierungseinstellung unerwünschte Bildartefakte verursachen kann. Aus diesem Grund empfiehlt Adobe Dynamic Media Classic, die Komprimierungsqualität (auf dem Schieberegler) auf 75 festzulegen. Mit dieser Einstellung erreichen Sie eine angemessene Bildqualität bei ausreichend kleiner Dateigröße.

   * **[!UICONTROL Scharfzeichnen]**: Wählen Sie kein Scharfzeichnen aus (dieser Scharfzeichnungsfilter bietet weniger Kontrolle als **[!UICONTROL Unschärfemasken]**-Einstellungen).

   * **[!UICONTROL Resample Mode]**: Wählen Sie **[!UICONTROL Bi-Cubic]**.

   * **[!UICONTROL Unschärfemaske]** (USM): Geben Sie die folgenden Einstellungen ein:

   | Vorgabetyp | Größe | Unschärfem.: Betrag | Unschärfem.: Radius | Unschärfem.: Schwelle |
   | --- | --- | --- | --- | --- |
   | Cross-Selling (besonders kleine Miniaturansicht) | 75 × 75 | 1,5 | 0,8 | 5 |
   | Miniaturansicht | 150 × 150 | 1,1 | 1 | 5 |
   | Hauptansicht | 350 × 350 | 1 | 1 | 6 |
   | Vergrößerung | 500 × 500 | 1,2 | 1,2 | 5 |

1. Wählen Sie **[!UICONTROL Speichern]** aus.

Die hier aufgeführten „Best Practice“-Optionen für Adobe Dynamic Media Classic zum Erstellen von Bildvorgaben sind allgemeine Empfehlungen. Das Scharfzeichnen ist sehr subjektiv. Diese „Best Practice“-Einstellungen basierten auf einem Primärbild von 2000 × 2000. Die Einstellungen für größere oder kleinere Primärdateien können unterschiedlich sein. Wenn Sie die Einstellungen für die Unschärfemaske anpassen möchten, empfiehlt Adobe Dynamic Media Classic die folgenden Bereiche:

* **[!UICONTROL amount]**: zwischen `.8` und `1.5`.

* **[!UICONTROL Radius]**: Zwischen `.6` und `2`.

* **[!UICONTROL Schwellenwert]**: Von `1` bis `6`.

Um eine Bildvorgabe zu löschen, wählen Sie sie auf dem Bildschirm Bildvorgaben aus und klicken Sie dann auf **[!UICONTROL Löschen]**.

>[!MORELIKETHIS]
>
>* [Erstellen und Bearbeiten von Bildvorgaben](application-setup.md#creating_and_editing_image_presets)
>* [Optionen für Bildvorgaben](application-setup.md#image_preset_options)
>* [Vorschau eines Bild-Assets basierend auf seiner Bildvorgabe](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)
