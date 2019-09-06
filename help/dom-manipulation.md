---
title: DOM-Manipulation
seo-title: DOM-Manipulation
description: 'null'
seo-description: Erfahren Sie mehr über die DOM-Manipulation.
uuid: 275 cd 49 d -2 a 55-41 f 9-80 b 0-e 147 d 0 cd 2907
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/template-publishing
discoiquuid: 890 ca 93 e -3146-4347-864 b-bd 5 e 94037038
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# DOM-Manipulation{#dom-manipulation}

Die DOM-Manipulation (Document Object Model) ist ein Verfahren, bei dem Designdateien durch direktes Manipulieren ihres XML-Codes bearbeitet werden. Die DOM-Manipulation ermöglicht eine bessere Steuerung der variablen Designelemente. So können Sie auf diese Weise z. B. den Inhalt und das Aussehen der Designelemente ändern und bei Bedarf sogar neue Elemente erstellen.

Mit Dynamic Media Classic können Sie das DOM einer klassischen FXG-Vorlage mit URL-Befehlen nach der Veröffentlichung der Vorlage manipulieren. Designelemente in der FXG-Vorlage werden manipuliert, indem die Befehle über die URL übergeben werden. Auf diese Weise können Sie Attribute dynamisch manipulieren und Grafiken hinzufügen.

Um die DOM-Manipulation zu verwenden, erstellen Sie s 7: Elementids in Ihrer Illustrator-Datei, bevor sie sie in eine dynamische FXG-Datei für die dynamische Mediendatei konvertieren und in das SPS hochladen.

>[!NOTE]
>
>Bei der Verwendung von DOM-Manipulationsbefehlen müssen alle weitergeleiteten Werte URL-kodiert sein.

>[!NOTE]
>
>Illustrator Plug-in for Web-to-Print (for converting Illustrator files) converts to FXG 2.0. For information about this specification, see [www.adobe.com/go/learn_s7_fxg2_en](https://www.adobe.com/go/learn_s7_fxg2_en).

## Erstellen von s7:elementIDs in Illustrator-Dateien {#creating-s-elementids-in-illustrator-files}

Wenn Sie ein in Illustrator erstelltes Design mithilfe von DOM-Manipulation bearbeiten möchten, erstellen Sie in Ihrem Illustrator-Design s7:elementIDs. Auf diese Weise können Designelemente nach der Veröffentlichung der Vorlage mit URL-Befehlen bearbeitet werden.

### Erstellen von s7:elementIDs für die DOM-Manipulation von Text {#creating-s-elementids-for-dom-manipulation-of-text}

Wenn Sie eine s7:elementID für die DOM-Manipulation eines Textobjekts erstellen möchten, öffnen Sie das Ebenenbedienfeld in Illustrator. Benennen Sie dann die Textebene, auf der sich der variable Text befindet, mit einer s7:elementID. To do so, enter the letters `id` (for identification), a colon ( `:`), and a name. Beispiele für mögliche s7:elementID-Textebenennamen:

`id:BirthdayBoyName`

`id:DateofBirth`

`id:EnterFirstNameHer`

### Erstellen von s7:elementIDs für die DOM-Manipulation von Objekten {#creating-s-elementids-for-dom-manipulation-of-objects}

Wenn die Endbenutzer die Attribute von Objekten ändern können sollen, erstellen Sie s7:elementIDs für Objekte. Objekte können aus ganzen Textrahmen, Grafiken und Bildern bestehen. Ein Beispiel für eine Objekt-Element-ID ist ein farbiger Hintergrund. Mit dem Wechsel der Jahreszeiten kann der Endbenutzer die Hintergrundfarbe eines Posters an die jeweilige Jahreszeit anpassen.

Bevor Sie in Illustrator eine s7:elementID für ein Objekt erstellen, erstellen Sie zunächst eine separate Ebene für das Objekt.

Führen Sie die folgenden Schritte aus, um in Illustrator eine s7:elementID für ein Objekt zu erstellen:

1. Wählen Sie das Objekt aus.
1. Klicken **Sie auf "Fenster** " &gt;" **Ebenen**«.
1. Benennen Sie die Objektebene im Ebenenbedienfeld mit einer s 7: Elementid. To do so, enter the letters `id` (for identification), a colon ( `:`), and description to identify the element. Beispiele für mögliche s7:elementID-Objektebenennamen:

   `id:BackgroundColor`

   `id:RotationPercentage`

   `id:JacketJPG`

## Veröffentlichen von FXG-Vorlagen {#publish-fxg-templates}

Durch das Veröffentlichen der FXG-Vorlage wird sie auf den Servern für dynamische Medien gespeichert, wo sie für Ihre Website und Anwendung verfügbar sind. Im Zuge der Veröffentlichung aktiviert das Scene7 Publishing System die URLs, die Sie für Ihre Website bzw. Anwendung benötigen.

>[!NOTE]
>
>Wenn Sie Ihre FXG-Vorlage verwenden möchten, veröffentlichen Sie den gesamten Inhalt, der bei der Erstellung der Vorlage verwendet wurde, einschließlich der Schriftarten und Bilder. Wenn Sie nicht alle erforderlichen Dateien berücksichtigen, wird beim Veröffentlichen eine Fehlermeldung angezeigt.

### Markieren von FXG-Vorlagen zur Veröffentlichung {#mark-fxg-templates-for-publish}

Vorlagen und alle zugehörigen Unterstützungsdateien müssen zur Veröffentlichung markiert werden, damit sie auf dynamischen Medienservern platziert werden können.

1. Wählen Sie im Durchsuchenbedienfeld die FXG-Vorlage sowie ggf. verwendete Grafiken, Bilder und Schriftarten aus.
1. Klicken Sie auf **Zur Veröffentlichung markieren**.

### Veröffentlichen der FXG-Vorlage {#publish-your-fxg-template}

1. Klicken Sie in der globalen Navigationsleiste auf **„Veröffentlichen“**.
1. Wählen Sie eine Option für „Wann“ und geben Sie optional einen Namen für den Veröffentlichungsauftrag ein.
1. Click **Start Publish**.

### Indikatoranzeige für Textüberlauf {#text-overflow-indicator-display}

Ein *Indikator für Textüberlauf* wird angezeigt, wenn Text in einem Textrahmen (oder bei verkettetem Text im letzten Textrahmen) den vorgesehenen Platz überschreitet. Der Indikator ist ein rotes Kästchen mit einem Pluszeichen. Textüberlaufindikatoren sind im SPS immer aktiviert.

Textüberlaufindikatoren werden über den Modifikator `markOverflowingTextFrame` gesteuert. Verwenden Sie den Modifikator wie folgt:

| Modifikator/Werte | Beschreibung |
|--- |--- |
| Markoverflowingtextframe = 0,1 | Mit dem Wert „1“ werden Textflussindikatoren angezeigt. Der Standardwert ist „0“. (Obwohl der Standardwert „0“ ist, sind Textüberlaufindikatoren im SPS immer aktiviert.) Beachten Sie beim Modifikator markOverflowingTextFrame die Groß-/Kleinschreibung. |

>[!MORELIKETHIS]
>
>* [Definieren der Variabilität: Parametrisierung oder DOM-Manipulation?](defining-variability-parameterization-versus-dom.md#defining_variability_parameterization_versus_dom_manipulation)
>* [Veröffentlichen](publishing-files.md#publishing_files)

