---
title: Erstellen von Imagemaps in E-Katalogen
seo-title: Erstellen von Imagemaps in E-Katalogen
description: 'null'
seo-description: Hier erfahren Sie, wie Sie Imagemaps erstellen.
uuid: 943 ad 3 f 7-a 885-4 bc 2-88 cb -77083384 bdf 8
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/ecatalogs
discoiquuid: 4 cf 63359-63 b 5-4 da 7-9498-335 d 91 b 4776 c
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# Erstellen von Imagemaps in E-Katalogen{#creating-ecatalog-image-maps}

Eine Imagemap ist ein Bereich auf einer E-Katalogseite, über den Sie den Mauszeiger bewegen oder auf den Sie klicken können, um verschiedene Aktionen auszulösen. Wenn Sie den Mauszeiger über eine Imagemap bewegen, sehen Sie beispielsweise einen Rollover-Text mit der Beschreibung eines Elements. Wenn Sie auf eine Imagemap klicken, wird eine andere Aktion ausgelöst. Beispielsweise können Sie eine Webseite öffnen, damit die Besucher der Website mehr über einen Artikel erfahren oder ihn kaufen können oder damit Sie ein Video starten können, um einen Artikel in Aktion zu sehen.

## Zeichnen von Imagemaps in E-Katalogen {#drawing-ecatalog-image-maps}

Imagemaps für E-Kataloge werden auf der Registerkarte „Imagemap-Seiten“ des Anzeigebereichs „E-Katalog“ gezeichnet. In diesem Anzeigebereich wird links der Bereich „Imagemap“ mit den E-Katalogseiten und rechts eine Liste mit Imagemaps angezeigt. Beim Erstellen von Imagemaps werden deren Namen in der Imagemap-Liste eingefügt.

1. Klicken Sie auf die Rollover-Schaltfläche „Bearbeiten“ des E-Katalogs.
1. Click **Map Pages**.
1. Wählen Sie links im Anzeigebereich „Imagemap-Seiten“ die gewünschte Seite aus.
1. Zeichnen Sie im Bereich „Imagemap“ eine rechteckige oder polygonale (vieleckige) Imagemap:

   **Rechteckige Karte** Wählen Sie das Rechteck-Imagemap-Werkzeug aus und ziehen Sie auf die Seite, um das Rechteck zu erstellen.

   **Polygonale Karte** Wählen Sie das Polygon-Imagemap-Werkzeug aus und klicken Sie so oft wie nötig auf den Umfang des Bilds. Während Sie klicken, zeichnet Dynamic Media Classic die Ränder der Imagemap.

   Nachdem Sie eine Imagemap gezeichnet haben, weist Dynamic Media Classic diesen Namen in der Imagemap-Liste zu. Um den Namen zu bilden, hängt Dynamisches Media Classic eine sequenzielle Nummer an den Namen der E-Katalog-Seite an, auf der Sie arbeiten.

1. (Optional) Geben Sie im Imagemap-Liste-Bedienfeld in der Spalte „Name“ einen neuen Namen für die Imagemap ein. Der von Ihnen eingegebene Name darf keine Leerzeichen enthalten.
1. Sie können festlegen, dass beim Klicken auf eine Imagemap in einem Viewer eine neue Webseite geöffnet wird. Geben Sie im Imagemap-Liste-Bedienfeld in der Spalte „URL“ die URL der Webseite ein.

   Klicken Sie auf „Bearbeiten“ und geben Sie eine Vorlage ein, um die Eingabe von URLs (Href-Vorlagen) zu vereinfachen. 

   Siehe [Verwenden von Vorlagen zur Eingabe von JavaScript-Code und URLs](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Optional) In the Show drop-down list, click **Rollover Text**, and then enter the text that you want users to see onscreen when they move their pointers over the Image Map.
1. (Optional) In the Show drop-down list, click **Other Actions**, and enter an attribute to trigger a blur or focus action when users move their pointers over an Image Map.

   Siehe [Definieren anderer Aktionen für Imagemaps](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Klicken Sie auf „**Speichern**“.
1. (Optional) Click **Preview** to view the eCatalog with the default eCatalog Viewer preset.

Um eine Imagemap zu löschen, wählen Sie deren Namen in der Imagemap-Liste aus und klicken Sie dann auf „Löschen“. Um eine Imagemap vorübergehend auf einer Seite zu deaktivieren, ohne sie jedoch zu löschen, deaktivieren Sie im Imagemap-Liste-Bedienfeld die Option „Ein“ der jeweiligen Imagemap.

## Einbetten von Rich-Media-Daten in einen E-Katalog {#embedding-rich-media-in-an-ecatalog}

Mit der Rich-Media-Option des E-Katalogs können Sie Videos im MP4-Format oder Rotationssets zu Imagemaps hinzufügen, die Sie in einen E-Katalog eingefügt haben. Wenn ein Benutzer auf den Imagemap-Bereich im E-Katalog klickt, wird das verknüpfte Video oder das Rotationsset angezeigt. Diese Funktion ist besonders hilfreich, wenn Sie möchten, dass die Kunden einen Artikel in Aktion oder einen Artikel aus unterschiedlichen Blickwinkeln und Perspektiven sehen können.

Sie können optional auch QuickInfo-Text anzeigen, wenn Kunden den Mauszeiger über die Imagemap bewegen, sodass sie wissen, worauf sie klicken.

**So betten Sie Rich-Media-Daten in einen E-Katalog ein**

1. Zeichnen Sie eine E-Katalog-Imagemap. 

   Siehe [Zeichnen von Imagemaps in E-Katalogen](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. Wählen Sie aus der Dropdown-Liste „Anzeigen“ die Option „Rich-Media-Daten“ aus.
1. Navigieren Sie im Bedienfeld „Assets hinzufügen“ links zu einem Ordner, der das Rotationsset oder Video-Asset (MP4-Format) enthält, das Sie einbetten möchten.
1. Ziehen Sie das Asset auf die Imagemap.
1. (Optional) Geben Sie im Imagemap-Liste-Bedienfeld unter der Spaltenüberschrift „QuickInfo“ den Text ein, der den Besuchern am Bildschirm angezeigt werden soll, wenn sie den Mauszeiger über die Imagemap bewegen.
1. Klicken Sie auf „Speichern“.

## Bearbeiten von Imagemaps in E-Katalogen {#editing-ecatalog-image-maps}

Führen Sie auf der Registerkarte „Imagemap-Seiten“ des Anzeigebereichs „E-Katalog“ die folgenden Schritte zum Bearbeiten von Imagemaps in E-Katalogen durch:

**Anpassen der Position** Wählen Sie das Schwenken-Werkzeug aus und bewegen Sie den Mauszeiger nahe an den Rand der Map. Wenn sich der Zeiger in einen vierköpfigen Pfeil ändert, ziehen Sie die gesamte Imagemap an eine neue Position. 

Siehe [Anpassen der Position, Form und Größe von Imagemaps](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

**Um die Größe und Größe** einer rechteckigen Imagemap zu ändern, wählen Sie das Schwenken-Werkzeug aus. Bewegen Sie dann den Mauszeiger über den Rand oder eine Ecke der Imagemap. Wenn der Mauszeiger als Doppelpfeil dargestellt wird, ziehen Sie ihn. Um die Größe einer polygonalen Imagemap zu ändern, ziehen Sie einen quadratischen Auswahlziehpunkt an die gewünschte Stelle. Um einen Auswahlziehpunkt zu erstellen, klicken Sie auf den Rand der Imagemap und beginnen Sie zu ziehen. 

Siehe [Anpassen der Position, Form und Größe von Imagemaps](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

**Imagemaps löschen** : Wählen Sie das Schwenken-Werkzeug aus, klicken Sie auf die Imagemap, um sie auszuwählen, und klicken Sie dann auf Löschen.

(Um sämtliche Imagemaps aus einem E-Katalog zu entfernen, rufen Sie die Registerkarte „Seiten ordnen“ auf und klicken dann auf „Maps löschen“.)

**Durch Ziehen mit überlappenden Imagemaps** wird die Reihenfolge der Imagemaps in der Imagemap-Liste geändert.

Siehe [Beheben von überlappenden Imagemaps](creating-image-maps.md#handling_overlapping_image_maps).

**Kopieren von Imagemaps auf andere Seiten** Klicken Sie auf die Schaltfläche "Maps kopieren nach" (stellen Sie sicher, dass Sie auf der Registerkarte" Imagemap-Seiten" sind). Wählen Sie im Anzeigebereich „Bilder auswählen“ die Seite oder Seiten aus, auf der oder denen Sie die Imagemaps kopieren möchten, und klicken Sie auf „Auswählen“. 

Siehe [Kopieren von Imagemaps in andere Bilder](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Sie können Imagemaps nicht nur auf andere Seiten in einem E-Katalog kopieren, sondern auch alle Imagemaps in einem E-Katalog in einen anderen E-Katalog kopieren. Siehe [Kopieren von Imagemaps zwischen E-Katalogen](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Überprüfen und Importieren von Imagemap-Daten {#reviewing-and-importing-image-map-data}

Im Anzeigebereich mit der Imagemap-Zusammenfassung werden Metadaten zum E-Katalog angezeigt. Sie können in diesem Anzeigebereich auch einen Stapelimport von Imagemap-Daten für den E-Katalog starten. Ein solcher Import von Imagemap-Daten erleichtert die Eingabe von Imagemap-URLs und Rollover-Text.

Um die Map-Übersicht anzuzeigen, klicken Sie auf der Registerkarte „Imagemap-Seiten“ des E-Katalog-Anzeigebereichs auf „Zusammenfassung“.

### Überprüfen der Zusammenfassung von Imagemap-Daten {#review-image-map-data-summary}

1. Klicken Sie im Anzeigebereich „Imagemap-Seiten“ auf „Zusammenfassung“.

   Im Anzeigebereich mit der Imagemap-Zusammenfassung wird die Anzahl der im E-Katalog enthaltenen Imagemaps, URLs, Rollover-Textbeschreibungen und anderen Aktionen angezeigt.

1. Wenn Rollover_Key-Fehler auftreten, klicken Sie in der Spalte „Rollover_Key-Fehler“ auf einen Fehler, um Hinweise zur Fehlerbehebung in der Tabelle anzuzeigen. Sie können den Text dieser Meldung kopieren und direkt in Ihre Tabelle einfügen.
1. Klicken Sie auf „Vorschau“, um die Seite im E-Katalog-Viewer zu überprüfen, klicken Sie auf das „X“, um den Anzeigebereich „Zusammenfassung“ zu schließen, oder klicken Sie auf „Schließen“, um zum Anzeigebereich „Durchsuchen“ zurückzukehren.

### Importieren von Imagemap-Daten {#import-image-map-data}

Anstatt auf jeder Seite Imagemap-Daten einzugeben, können Sie über den Anzeigebereich mit der Imagemap-Zusammenfassung auch die Daten für den gesamten E-Katalog importieren. Die Imagemap-Daten werden in Form einer tabulatorgetrennten oder XML DTD-Datei importiert. Die Felder in der Datei müssen dieselbe Reihenfolge haben, wie im Anzeigebereich mit der Imagemap-Zusammenfassung dargestellt: „Name“, „Inhaltsverz.“, „Imagemaps“, „URLs“, „Rollover-Text“, „Andere Aktionen“ und „Suchzeichenfolgen“. Indem Sie Imagemap-Daten importieren, können Sie sich die Arbeit beim Eingeben der Daten in der Imagemap-Liste zum Erstellen der einzelnen Imagemaps sparen.

>[!NOTE]
>
>Bevor Sie Imagemap-Daten importieren können, müssen Sie die Imagemaps bereits erstellt haben.

Führen Sie im Anzeigebereich mit der Imagemap-Zusammenfassung die folgenden Schritte zum Importieren vom Imagemap-Daten für die bereits erstellten Imagemaps aus:

1. Klicken Sie auf „Map-Daten importieren“. 
1. Klicken Sie im Dialogfeld „Metadaten importieren“ auf „Durchsuchen“ und wählen Sie dann die tabulatorgetrennte Datei bzw. XML-DTD-Datei aus.
1. Geben Sie im Feld „Auftragsname“ einen Namen für die Datei ein (achten Sie darauf, die Dateinamenerweiterung dabei nicht zu ändern).
1. Klicken Sie auf „Hochladen“.

## Kopieren von Imagemaps zwischen E-Katalogen {#copying-image-maps-between-ecatalogs}

Sie können alle Imagemaps in einem E-Katalog in einen anderen E-Katalog kopieren. Das Kopieren der Imagemaps auf diese Weise ist ein praktisches Verfahren, um Imagemaps zwischen fremdsprachigen Versionen des gleichen E-Katalogs zu kopieren. Damit das Kopieren erfolgreich ist, empfiehlt Dynamic Media Classic, zwischen E-Katalogen mit derselben Anzahl vonseiten und denselben Bildern zu kopieren.

>[!NOTE]
>
>Falls der E-Katalog, in den Sie Imagemaps kopieren, bereits Imagemaps enthält, werden diese beim Kopiervorgang gelöscht.

Gehen Sie folgendermaßen vor, um alle Imagemaps in einem E-Katalog in einen anderen E-Katalog zu kopieren:

1. Wählen Sie den E-Katalog mit den zu kopierenden Imagemaps aus und klicken Sie auf die Rollover-Schaltfläche „Bearbeiten“ des E-Katalogs.
1. Klicken Sie auf der Registerkarte „Seiten ordnen“ auf „Maps kopieren“.
1. Wählen Sie im Dialogfeld „Asset auswählen“ den E-Katalog aus, in den Sie die Imagemaps kopieren möchten, und klicken Sie dann auf „Auswählen“.

Dynamic Media Classic zeigt eine Warnmeldung an, wenn der Ziele-Katalog (der E-Katalog, in den Sie Imagemaps kopieren) eine andere Anzahl vonseiten oder Bildern hat, die eine andere Größe haben. Durch Klicken auf „Fortfahren“ werden die Imagemaps trotz der Warnung kopiert.
