---
title: Einrichten von Bildvorgaben
description: Erfahren Sie, wie Sie Bildvorgaben in Adobe Dynamic Media Classic einrichten.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
topic: Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 37%

---

# Einrichten von Bildvorgaben{#setting-up-image-presets}

Eine Bildvorgabe ähnelt einem Makro – es handelt sich um eine vordefinierte, mit gemeinsamem Namen gespeicherte Sammlung von Befehlen zur Größeneinstellung und Formatierung. Um zu verstehen, wie Bildvorgaben funktionieren, nehmen wir an, dass auf Ihrer Website jedes Produktbild in zwei verschiedenen Größen angezeigt werden muss: 500 × 500 Pixel und 150 × 150 Pixel. Sie erstellen zwei Bildvorgaben, eine mit der Bezeichnung &quot;Vergrößern&quot;, um Bilder mit einer Auflösung von 500 x 500 Pixel anzuzeigen, und eine mit der Bezeichnung &quot;Miniatur&quot;, um Bilder mit einer Größe von 150 × 150 Pixel anzuzeigen. Um Bilder in den Größen &quot;Vergrößern&quot;und &quot;Miniaturansicht&quot;bereitzustellen, sucht ein Dynamic Media-Bildserver nach der Definition von &quot;Bildvorgabe vergrößern&quot;und &quot;Bildvorgabe für Miniaturansichten&quot;. Dann erstellt der Server dynamisch je ein Bild in der Größe und mit den Formatierungsangaben, die in den beiden Bildvorgaben gespeichert sind.

Adobe Dynamic Media Classic enthält mehrere &quot;Best Practice&quot;-Bildvorgaben, die Sie bereits zur Verwendung eingerichtet haben. Administratoren können auch Bildvorgaben erstellen. Sie können eine Bildvorgabe komplett neu erstellen oder eine vorhandene Bildvorgabe abwandeln und unter neuem Namen speichern.

Bei Bildern, deren Größe bei der dynamischen Bereitstellung von einem Server verringert wird, kann es zu einem Verlust an Schärfe und Detail kommen. Aus diesem Grund enthält jede Bildvorgabe Elemente zur Formatierungssteuerung, mit denen ein Bild bei Bereitstellung in einer bestimmten Größe optimiert wird. Ihre Bilder werden dadurch scharf und klar für die Website bzw. Anwendung bereitgestellt.

## Erstellen einer Bildvorgabe {#creating-an-image-preset}

Als Unternehmensadministrator haben Sie die Möglichkeit, eigene Bildvorgaben zu erstellen. Sie können Bildvorgaben erstellen oder mit einer von Adobe Dynamic Media Classic bereitgestellten standardmäßigen Bildvorgabe beginnen, sie bearbeiten und mit einem neuen Namen speichern.

**So erstellen Sie eine Bildvorgabe:**

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Bildvorgaben]**.

   Hier können Sie den Namen einer Bildvorgabe auswählen, um die Vorschau einer vorhandenen Bildvorgabe einzublenden. Sobald Sie den Namen einer Bildvorgabe auswählen, ändern sich Größe und Aussehen des Beispielbilds im Vorschaufenster.

1. Führen Sie einen der folgenden Schritte aus:

   * **Erstellen einer Bildvorgabe** - Auswählen **[!UICONTROL Hinzufügen]**.
   * **Bearbeiten einer Bildvorgabe** - Navigieren Sie zu der Bildvorgabe, die der gewünschten am ähnlichsten ist, und wählen Sie dann **[!UICONTROL Bearbeiten]**.

1. Geben Sie einen Namen für die Bildvorgabe ein.
1. Geben Sie die Breite und Höhe in Pixeln ein. Diese Werte bestimmen die Größe, in der Bilder bereitgestellt werden.
1. Füllen Sie die Felder im Anzeigebereich „Vorgabe hinzufügen“ bzw. „Vorgabe bearbeiten“ aus. Einzelheiten dazu finden Sie im Abschnitt [Optionen für Bildvorgaben](application-setup.md#image_preset_options).

   Adobe Dynamic Media Classic empfiehlt die folgenden Best Practice-Optionen, um zu beginnen:

   * **[!UICONTROL Format]** - Wählen Sie JPEG oder ein anderes Format, das Ihren Anforderungen entspricht. Alle Webbrowser unterstützen das JPEG-Bildformat. Es bietet einen guten Ausgleich zwischen kleinen Dateigrößen und Bildqualität. JPEG-Bilder verwenden jedoch ein verlustbehaftetes Komprimierungsschema, das unerwünschte Bildartefakte hervorrufen kann, wenn die Komprimierungseinstellung zu niedrig ist. Aus diesem Grund empfiehlt Adobe Dynamic Media Classic, die Komprimierungsqualität (auf dem Regler) auf 75 festzulegen. Mit dieser Einstellung erreichen Sie eine angemessene Bildqualität bei ausreichend kleiner Dateigröße.

   * **[!UICONTROL Scharfzeichnen]** - Scharfzeichnen nicht auswählen (dieser Scharfzeichnungsfilter bietet weniger Kontrolle als **[!UICONTROL Unschärfemaske]** -Einstellungen).

   * **[!UICONTROL Beispielmodus]** - Auswählen **[!UICONTROL Bikubisch]**.

   * **[!UICONTROL Unschärfemaske]** (USM) - Geben Sie die folgenden Einstellungen ein:

   | Vorgabetyp | Größe | Unschärfem.: Betrag | Unschärfem.: Radius | Unschärfem.: Schwelle |
   | --- | --- | --- | --- | --- |
   | Cross-Selling (besonders kleine Miniaturansicht) | 75 × 75 | 1,5 | 0,8 | 5 |
   | Miniaturansicht | 150 × 150 | 1,1 | 1 | 5 |
   | Hauptansicht | 350 × 350 | 1 | 1 | 6 |
   | Vergrößerung | 500 × 500 | 1,2 | 1,2 | 5 |

1. Auswählen **[!UICONTROL Speichern]**.

Die hier aufgeführten Adobe Dynamic Media Classic-Best Practice-Optionen zum Erstellen von Bildvorgaben sind allgemeine Empfehlungen. Die Scharfzeichnung ist äußerst subjektiv. Diese &quot;Best Practice&quot;-Einstellungen basieren auf einem Primärbild von 2000 × 2000. Die Einstellungen für größere oder kleinere Primärdateien können unterschiedlich sein. Wenn Sie die Einstellungen für die Unschärfemaske anpassen möchten, empfiehlt Adobe Dynamic Media Classic die folgenden Bereiche:

* **[!UICONTROL Betrag]** - zwischen 0,8 und 1,5.

* **[!UICONTROL Radius]** - zwischen 0,6 und 2.

* **[!UICONTROL Schwellenwert]** - von 1 bis 6.

Um eine Bildvorgabe zu löschen, wählen Sie sie auf dem Bildschirm &quot;Bildvorgaben&quot;aus und wählen Sie dann **[!UICONTROL Löschen]**.

>[!MORELIKETHIS]
>
>* [Erstellen und Bearbeiten von Bildvorgaben](application-setup.md#creating_and_editing_image_presets)
>* [Optionen für Bildvorgaben](application-setup.md#image_preset_options)
>* [Vorschau eines Bild-Assets basierend auf seiner Bildvorgabe](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)
