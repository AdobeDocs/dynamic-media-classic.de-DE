---
title: Einrichten von Bildvorgaben
description: Erfahren Sie, wie Sie Bildvorgaben in Adobe Dynamic Media Classic einrichten.
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 54%

---

# Einrichten von Bildvorgaben{#setting-up-image-presets}

Eine Bildvorgabe ähnelt einem Makro – es handelt sich um eine vordefinierte, mit gemeinsamem Namen gespeicherte Sammlung von Befehlen zur Größeneinstellung und Formatierung. Um zu verstehen, wie Bildvorgaben funktionieren, nehmen wir an, dass auf Ihrer Website jedes Produktbild in zwei verschiedenen Größen angezeigt werden muss: 500 x 500 Pixel und 150 x 150 Pixel. Sie erstellen dann zwei Bildvorgaben, eine mit der Bezeichnung „Vergrößerung“ zum Anzeigen von Bildern mit 500 x 500 Pixeln, eine mit der Bezeichnung „Miniaturansicht“ zum Anzeigen von Bildern mit 150 x 150 Pixeln. Um Bilder in den Größen &quot;Vergrößern&quot;und &quot;Miniaturansicht&quot;bereitzustellen, sucht ein Dynamic Media-Bildserver nach der Definition der Bildvorgabe &quot;Vergrößern&quot;und der Bildvorgabe &quot;Miniaturansicht&quot;. Dann erstellt der Server dynamisch je ein Bild in der Größe und mit den Formatierungsangaben, die in den beiden Bildvorgaben gespeichert sind.

Adobe Dynamic Media Classic enthält mehrere Bildvorgaben, die bereits für die Verwendung durch Sie eingerichtet sind. Administratoren können auch Bildvorgaben erstellen. Sie können eine Bildvorgabe komplett neu erstellen oder eine vorhandene Bildvorgabe abwandeln und unter neuem Namen speichern.

Bei Bildern, deren Größe bei der dynamischen Bereitstellung von einem Server verringert wird, kann es zu einem Verlust an Schärfe und Detail kommen. Aus diesem Grund enthält jede Bildvorgabe Elemente zur Formatierungssteuerung, mit denen ein Bild bei Bereitstellung in einer bestimmten Größe optimiert wird. Ihre Bilder werden dadurch scharf und klar für die Website bzw. Anwendung bereitgestellt.

## Erstellen einer Bildvorgabe {#creating-an-image-preset}

Als Unternehmensadministrator haben Sie die Möglichkeit, eigene Bildvorgaben zu erstellen. Sie können Bildvorgaben erstellen oder mit einer standardmäßigen Bildvorgabe beginnen, die von Adobe Dynamic Media Classic bereitgestellt wird, sie bearbeiten und mit einem neuen Namen speichern.

**So erstellen Sie ein Bildvorgabe:**

1. Gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Bildvorgaben]**.

   Hier können Sie den Namen einer Bildvorgabe auswählen, um die Vorschau einer vorhandenen Bildvorgabe einzublenden. Sobald Sie den Namen einer Bildvorgabe auswählen, ändern sich Größe und Aussehen des Beispielbilds im Vorschaufenster.

1. Führen Sie einen der folgenden Schritte aus:

   * **Bildvorgabe erstellen**  - Wählen Sie  **[!UICONTROL Hinzufügen]** aus.
   * **Bildvorgabe bearbeiten**  - Navigieren Sie zu der Bildvorgabe, die der Bildvorgabe am ehesten ähnelt, die Sie erstellen möchten, und wählen Sie dann  **[!UICONTROL Bearbeiten]** aus.

1. Geben Sie einen Namen für die Bildvorgabe ein.
1. Geben Sie die Breite und Höhe in Pixeln ein. Diese Werte bestimmen die Größe, in der Bilder bereitgestellt werden.
1. Füllen Sie die Felder im Anzeigebereich „Vorgabe hinzufügen“ bzw. „Vorgabe bearbeiten“ aus. Einzelheiten dazu finden Sie im Abschnitt [Optionen für Bildvorgaben](application-setup.md#image_preset_options).

   Adobe Dynamic Media Classic empfiehlt die folgenden Best Practice-Optionen, um zu beginnen:

   * **[!UICONTROL Format]**  - Wählen Sie JPEG oder ein anderes Format, das Ihren Anforderungen entspricht. Alle Webbrowser unterstützen das JPEG-Bildformat. Es bietet eine gute Balance zwischen kleinen Dateigrößen und Bildqualität. Bilder im JPEG-Format verwenden jedoch ein verlustbehaftetes Komprimierungsschema, das unerwünschte Bildartefakte hervorrufen kann, wenn die Komprimierungseinstellung zu niedrig festgelegt ist. Daher empfiehlt Adobe Dynamic Media Classic, die Komprimierungsqualität (auf dem Regler) auf 75 festzulegen. Diese Einstellung bietet eine gute Balance zwischen Bildqualität und kleiner Dateigröße.

   * **[!UICONTROL Scharfzeichnen]**  - Wählen Sie nicht Scharfzeichnen aus (dieser Scharfzeichnungsfilter bietet weniger Kontrolle als  **[!UICONTROL Unschärfemaske-]** Einstellungen).

   * **[!UICONTROL Resample Mode]**  - Wählen Sie  **[!UICONTROL Bikubisch]**.

   * **[!UICONTROL Unschärfemaske]**  (USM) - Geben Sie die folgenden Einstellungen ein:

   | Vorgabetyp | Größe | Unschärfem.: Betrag | Unschärfem.: Radius | Unschärfem.: Schwelle |
   | --- | --- | --- | --- | --- |
   | Cross-Selling (besonders kleine Miniaturansicht) | 75 x 75 | 1,5 | 0,8 | 5 |
   | Miniaturansicht | 150 x 150 | 1,1 | 1 | 5 |
   | Hauptansicht | 350 x 350 | 1 | 1 | 6 |
   | Vergrößerung | 500 x 500 | 1,2 | 1,2 | 5 |

1. Wählen Sie **[!UICONTROL Save]** aus.

Die hier aufgelisteten Adobe Dynamic Media Classic-Best Practice-Optionen zum Erstellen von Bildvorgaben sind allgemeine Empfehlungen. Scharfzeichnen ist sehr subjektiv. Die oben aufgeführten Einstellungen wurden für ein Masterbild der Größe 2000 x 2000 Pixel festgelegt; Einstellungen für größere oder kleinere Masterversionen können abweichen. Wenn Sie die Einstellungen für die Unschärfemaske anpassen möchten, empfiehlt Adobe Dynamic Media Classic die folgenden Bereiche:

* **[!UICONTROL Betrag]**  - zwischen 0,8 und 1,5.

* **[!UICONTROL Radius]**  - zwischen 0,6 und 2.

* **[!UICONTROL Schwellenwert]**  - von 1 bis 6.

Um eine Bildvorgabe zu löschen, wählen Sie sie auf dem Bildschirm &quot;Bildvorgaben&quot;aus und klicken Sie dann auf **[!UICONTROL Löschen]**.

>[!MORELIKETHIS]
>
>* [Erstellen und Bearbeiten von Bildvorgaben](application-setup.md#creating_and_editing_image_presets)
>* [Optionen für Bildvorgaben](application-setup.md#image_preset_options)
>* [Vorschau eines Bild-Assets basierend auf seiner Bildvorgabe](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

