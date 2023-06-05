---
title: Erstellen von eCatalog-Imagemaps
description: Erfahren Sie, wie Sie eCatalog-Imagemaps in Adobe Dynamic Media Classic erstellen.
uuid: 943ad3f7-a885-4bc2-88cb-77083384bdf8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 4cf63359-63b5-4da7-9498-335d91b4776c
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '1492'
ht-degree: 40%

---

# Erstellen von eCatalog-Imagemaps{#creating-ecatalog-image-maps}

Eine Imagemap ist ein Bereich auf einer eCatalog-Seite, den Sie mit der Maus verschieben oder auswählen können, um Trigger-Aktionen verschiedener Art durchzuführen. Wenn Sie den Mauszeiger beispielsweise über eine Imagemap bewegen, wird eine Rollover-Textbeschreibung eines Elements angezeigt. Wenn Sie eine Imagemap auswählen, wird eine weitere Aktion eingeleitet. Beispielsweise können Sie eine Webseite öffnen, damit die Besucher der Website mehr über einen Artikel erfahren oder ihn kaufen können oder damit Sie ein Video starten können, um einen Artikel in Aktion zu sehen.

## Zeichnen von eCatalog-Imagemaps {#drawing-ecatalog-image-maps}

Imagemaps für E-Kataloge werden auf der Registerkarte „Imagemap-Seiten“ des Anzeigebereichs „E-Katalog“ gezeichnet. In diesem Anzeigebereich wird links der Bereich „Imagemap“ mit den E-Katalogseiten und rechts eine Liste mit Imagemaps angezeigt. Beim Erstellen von Imagemaps werden deren Namen in der Imagemap-Liste eingefügt.

1. Rollover des E-Katalogs auswählen **[!UICONTROL Bearbeiten]** Schaltfläche.
1. Auswählen **[!UICONTROL Seiten zuordnen]**.
1. Wählen Sie links im Anzeigebereich „Imagemap-Seiten“ die gewünschte Seite aus.
1. Zeichnen Sie im Bereich „Imagemap“ eine rechteckige oder polygonale (vieleckige) Imagemap:

   * **Rechteckige Karte** - Wählen Sie das Rechteck-Bildzuordnungstool aus und ziehen Sie es auf die Seite, um das Rechteck zu erstellen.

   * **Polygonale Karte** - Wählen Sie das Tool Polygon Image Map aus und wählen Sie dann so oft wie nötig den Bildbereich aus. Wie Sie auswählen, zeichnet Adobe Dynamic Media Classic die Ränder der Imagemap.

      Nachdem Sie eine Imagemap gezeichnet haben, weist Adobe Dynamic Media Classic ihr einen Namen in der Imagemap-Liste zu. Um den Namen zu bilden, hängt Adobe Dynamic Media Classic eine sequenzielle Nummer an den Namen der eCatalog-Seite an, auf der Sie arbeiten.

1. (Optional) In der Liste &quot;Imagemap&quot;in der [!UICONTROL Name] können Sie einen neuen Namen für die Imagemap eingeben. Der von Ihnen eingegebene Name darf keine Leerzeichen enthalten.
1. Sie können Viewer eine neue Webseite öffnen lassen, wenn sie die Imagemap auswählen. Geben Sie im Imagemap-Liste-Bedienfeld in der Spalte „URL“ die URL der Webseite ein.

   Um die Eingabe von URLs (Href-Vorlagen) zu vereinfachen, wählen Sie **[!UICONTROL Bearbeiten]** und geben Sie eine Vorlage ein.

Siehe [Verwenden Sie eine Vorlage, um JavaScript und URLs einzugeben.](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Optional) Wählen Sie in der Dropdownliste Anzeigen die Option **[!UICONTROL Rollover-Text]** und geben Sie dann den Text ein, den Benutzern auf dem Bildschirm angezeigt werden sollen, wenn sie ihre Zeiger über die Imagemap bewegen.
1. (Optional) Wählen Sie in der Dropdownliste Anzeigen die Option **[!UICONTROL Andere Aktionen]** und geben Sie ein Attribut ein, um eine Weichzeichnung oder Fokusaktion Trigger, wenn Benutzer ihre Zeiger über eine Imagemap bewegen.

   Siehe [Andere Aktionen für Imagemaps definieren](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Auswählen **[!UICONTROL Speichern]**.
1. (Optional) Wählen Sie **[!UICONTROL Vorschau]** , um den eCatalog mit der standardmäßigen eCatalog-Viewer-Vorgabe anzuzeigen.

Um eine Imagemap zu löschen, wählen Sie deren Namen in der Liste &quot;Imagemap&quot;aus und klicken Sie auf **[!UICONTROL Löschen]**. Um eine Imagemap vorübergehend auf einer Seite zu deaktivieren, ohne sie jedoch zu löschen, deaktivieren Sie im Imagemap-Liste-Bedienfeld die Option „Ein“ der jeweiligen Imagemap.

## Rich Media in einen eCatalog einbetten {#embedding-rich-media-in-an-ecatalog}

Mit der Rich-Media-Option des E-Katalogs können Sie Videos im MP4-Format oder Rotationssets zu Imagemaps hinzufügen, die Sie in einen E-Katalog eingefügt haben. Wenn ein Benutzer den Bereich &quot;Imagemap&quot;im eCatalog auswählt, wird das zugehörige Rotationsset oder Video angezeigt. Diese Funktion ist besonders hilfreich, wenn Sie möchten, dass die Kunden einen Artikel in Aktion oder einen Artikel aus unterschiedlichen Blickwinkeln und Perspektiven sehen können.

Sie können optional auch QuickInfo-Text anzeigen, wenn Kunden ihre Zeiger über Ihre Imagemap bewegen, damit sie wissen, was sie auswählen.

**So betten Sie Rich-Media-Daten in einen E-Katalog ein:**

1. Zeichnen Sie eine E-Katalog-Imagemap. 

   Siehe [Zeichnen von eCatalog-Imagemaps](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. Wählen Sie in der Dropdown-Liste Anzeigen die Option **[!UICONTROL Rich Media]**.
1. Navigieren Sie im Bedienfeld „Assets hinzufügen“ links zu einem Ordner, der das Rotationsset oder Video-Asset (MP4-Format) enthält, das Sie einbetten möchten.
1. Ziehen Sie das Asset auf die Imagemap.
1. (Optional) Im Listenbereich &quot;Imagemap&quot;unter **[!UICONTROL QuickInfo]** Spaltenüberschrift den Text eingeben, den Betrachtern angezeigt werden sollen, wenn sie den Mauszeiger über die Imagemap bewegen.
1. Auswählen **[!UICONTROL Speichern]**.

## Bearbeiten von Imagemaps in E-Katalogen {#editing-ecatalog-image-maps}

Führen Sie auf der Registerkarte „Imagemap-Seiten“ des Anzeigebereichs „E-Katalog“ die folgenden Schritte zum Bearbeiten von Imagemaps in E-Katalogen durch:

* **Position anpassen** - Wählen Sie das Schwenken-Tool aus und bewegen Sie den Mauszeiger nahe, jedoch nicht über den Rahmen der Karte. Wenn sich der Zeiger in einen vierköpfigen Pfeil ändert, ziehen Sie die gesamte Imagemap an eine neue Position. 

   Siehe [Position, Form und Größe von Imagemaps anpassen](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Form und Größe ändern** - Um die Größe einer rechteckigen Imagemap zu ändern, wählen Sie das Schwenken-Tool aus. Bewegen Sie dann den Mauszeiger über den Rand oder eine Ecke der Imagemap. Wenn der Mauszeiger als Doppelpfeil dargestellt wird, ziehen Sie ihn. Um die Größe einer polygonalen Imagemap zu ändern, ziehen Sie einen quadratischen Auswahlziehpunkt an die gewünschte Stelle. Um einen Auswahlpunkt zu erstellen, wählen Sie den Rahmen der Imagemap aus und ziehen Sie.

   Siehe [Position, Form und Größe von Imagemaps anpassen](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Löschen von Imagemaps** - Wählen Sie das Schwenken-Tool aus, wählen Sie die Imagemap aus, um sie auszuwählen, und klicken Sie auf **[!UICONTROL Löschen]**.

   Um alle Imagemaps aus einem E-Katalog zu entfernen, wählen Sie die **[!UICONTROL Bestellseiten]** und wählen Sie **[!UICONTROL Clear Maps]**.

* **Umgang mit überlappenden Imagemaps** - Ziehen Sie, um die Reihenfolge der Imagemaps in der Liste Imagemap zu ändern.

   Siehe [Überlagerte Imagemaps verwalten](creating-image-maps.md#handling_overlapping_image_maps).

* **Kopieren von Imagemaps auf anderen Seiten** - Auswählen **[!UICONTROL Zuordnungen kopieren nach]** (Stellen Sie sicher, dass Sie sich auf der Registerkarte Seiten zuordnen befinden). Wählen Sie im Bildschirm &quot;Bilder auswählen&quot;die Seite(n) aus, auf die Sie die Imagemaps kopieren möchten, und wählen Sie **[!UICONTROL Auswählen]**.

   Siehe [Kopieren von Imagemaps in andere Bilder](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Sie können Imagemaps nicht nur auf verschiedene Seiten in einem E-Katalog kopieren, sondern auch alle Imagemaps in einem E-Katalog in einen anderen eCatalog kopieren. Siehe [Kopieren von Imagemaps zwischen E-Katalogen](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Überprüfen und Importieren von Imagemap-Daten {#reviewing-and-importing-image-map-data}

Im Anzeigebereich mit der Imagemap-Zusammenfassung werden Metadaten zum E-Katalog angezeigt. Sie können in diesem Anzeigebereich auch einen Stapelimport von Imagemap-Daten für den E-Katalog starten. Ein solcher Import von Imagemap-Daten erleichtert die Eingabe von Imagemap-URLs und Rollover-Text.

Um den Bildschirm &quot;Map Summary&quot;anzuzeigen, wählen Sie auf der Registerkarte Map Pages auf dem eCatalog-Bildschirm die Option **[!UICONTROL Zusammenfassung]**.

### Überprüfen der Zusammenfassung von Imagemap-Daten {#review-image-map-data-summary}

1. Wählen Sie auf dem Bildschirm Seiten zuordnen die Option **[!UICONTROL Zusammenfassung]**.

   Im Anzeigebereich mit der Imagemap-Zusammenfassung wird die Anzahl der im E-Katalog enthaltenen Imagemaps, URLs, Rollover-Textbeschreibungen und anderen Aktionen angezeigt.

1. Wenn Rollover-Schlüsselfehler auftreten, wählen Sie den Fehler im **[!UICONTROL Rollover_key-Fehler]** in der Spalte, um zu sehen, was sich im Arbeitsblatt ändern muss, um den Fehler zu korrigieren. Sie können den Text dieser Meldung kopieren und direkt in Ihre Tabelle einfügen.
1. Auswählen **[!UICONTROL Vorschau]** damit Sie eine Seite im E-Katalog-Viewer untersuchen können; Wählen Sie das X aus, um den Zusammenfassungsbildschirm zu schließen und zum Bildschirm &quot;Zuordnungsseiten&quot;zurückzukehren, oder wählen Sie **[!UICONTROL Schließen]** , um zu &quot;Durchsuchen&quot;zurückzukehren.

### Importieren von Imagemap-Daten {#import-image-map-data}

Anstatt auf jeder Seite Imagemap-Daten einzugeben, können Sie über den Anzeigebereich mit der Imagemap-Zusammenfassung auch die Daten für den gesamten E-Katalog importieren. Die Imagemap-Daten werden in Form einer tabulatorgetrennten oder XML DTD-Datei importiert. Die Felder in der Datei müssen dieselbe Reihenfolge haben, wie im Anzeigebereich mit der Imagemap-Zusammenfassung dargestellt: „Name“, „Inhaltsverz.“, „Imagemaps“, „URLs“, „Rollover-Text“, „Andere Aktionen“ und „Suchzeichenfolgen“. Indem Sie Imagemap-Daten importieren, können Sie sich die Arbeit beim Eingeben der Daten in der Imagemap-Liste zum Erstellen der einzelnen Imagemaps sparen.

>[!NOTE]
>
>Bevor Sie Imagemap-Daten importieren können, müssen Sie die Imagemaps bereits erstellt haben.

Führen Sie im Anzeigebereich mit der Imagemap-Zusammenfassung die folgenden Schritte zum Importieren vom Imagemap-Daten für die bereits erstellten Imagemaps aus:

1. Auswählen **[!UICONTROL Map-Daten importieren]**.
1. Wählen Sie im Dialogfeld Metadaten importieren die Option **[!UICONTROL Durchsuchen]** und wählen Sie dann die tabulatorgetrennte oder XML-DTD-Datei aus.
1. Geben Sie im Feld „Auftragsname“ einen Namen für die Datei ein (achten Sie darauf, die Dateinamenerweiterung dabei nicht zu ändern).
1. Auswählen **[!UICONTROL Hochladen]**.

## Kopieren von Imagemaps zwischen E-Katalogen {#copying-image-maps-between-ecatalogs}

Sie können alle Imagemaps in einem E-Katalog in einen anderen E-Katalog kopieren. Das Kopieren der Imagemaps auf diese Weise ist ein praktisches Verfahren, um Imagemaps zwischen fremdsprachigen Versionen des gleichen E-Katalogs zu kopieren. Damit das Kopieren erfolgreich ist, empfiehlt Adobe Dynamic Media Classic das Kopieren zwischen E-Katalogen mit derselben Anzahl von Seiten und Bildern.

>[!NOTE]
>
>Falls der E-Katalog, in den Sie Imagemaps kopieren, bereits Imagemaps enthält, werden diese beim Kopiervorgang gelöscht.

Gehen Sie wie folgt vor, um alle Imagemaps in einem eCatalog in einen anderen eCatalog zu kopieren:

1. Wählen Sie den E-Katalog mit den zu kopierenden Imagemaps aus und wählen Sie den Rollover des E-Katalogs aus **[!UICONTROL Bearbeiten]** Schaltfläche.
1. Wählen Sie auf der Registerkarte Seiten sortieren die Option **[!UICONTROL Maps kopieren]**.
1. Wählen Sie im Dialogfeld &quot;Select Asset&quot;den E-Katalog aus, in den Sie die Imagemaps kopieren möchten, und klicken Sie dann auf **[!UICONTROL Auswählen]**.

Adobe Dynamic Media Classic zeigt eine Warnmeldung an, wenn der Ziel-eCatalog (der E-Katalog, in den Sie Imagemaps kopieren) eine andere Anzahl von Seiten oder Bildern mit einer anderen Größe aufweist. Auswählen **[!UICONTROL Weiter]** , um die Imagemaps trotz der Warnung zu kopieren.
