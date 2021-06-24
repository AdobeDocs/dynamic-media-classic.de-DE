---
title: Erstellen von Imagemaps in E-Katalogen
description: Erfahren Sie, wie Sie eCatalog-Imagemaps erstellen.
uuid: 943ad3f7-a885-4bc2-88cb-77083384bdf8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 4cf63359-63b5-4da7-9498-335d91b4776c
feature: Dynamic Media Classic,Viewers,eCatalog
role: Business Practitioner
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
source-git-commit: bd0659c015f259e25d6d07b620f5b1e948cabcbf
workflow-type: tm+mt
source-wordcount: '1484'
ht-degree: 55%

---

# Erstellen von Imagemaps in E-Katalogen{#creating-ecatalog-image-maps}

Eine Imagemap ist ein Bereich auf einer E-Katalogseite, über den Sie den Mauszeiger bewegen oder auf den Sie klicken können, um verschiedene Aktionen auszulösen. Wenn Sie den Mauszeiger beispielsweise über eine Imagemap bewegen, wird eine Rollover-Textbeschreibung eines Elements angezeigt. Wenn Sie auf eine Imagemap klicken, wird eine andere Aktion ausgelöst. Beispielsweise können Sie eine Webseite öffnen, damit die Besucher der Website mehr über einen Artikel erfahren oder ihn kaufen können oder damit Sie ein Video starten können, um einen Artikel in Aktion zu sehen.

## Zeichnen von Imagemaps in E-Katalogen {#drawing-ecatalog-image-maps}

Imagemaps für E-Kataloge werden auf der Registerkarte „Imagemap-Seiten“ des Anzeigebereichs „E-Katalog“ gezeichnet. In diesem Anzeigebereich wird links der Bereich „Imagemap“ mit den E-Katalogseiten und rechts eine Liste mit Imagemaps angezeigt. Beim Erstellen von Imagemaps werden deren Namen in der Imagemap-Liste eingefügt.

1. Klicken Sie auf die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** des E-Katalogs.
1. Klicken Sie auf **[!UICONTROL Seiten zuordnen]**.
1. Wählen Sie links im Anzeigebereich „Imagemap-Seiten“ die gewünschte Seite aus.
1. Zeichnen Sie im Bereich „Imagemap“ eine rechteckige oder polygonale (vieleckige) Imagemap:

   * **Rechteckige Karte**  - Wählen Sie das Rechteck-Bildzuordnungstool aus und ziehen Sie auf die Seite, um das Rechteck zu erstellen.

   * **Polygonale Karte**  - Wählen Sie das Polygon-Imagemap-Tool aus und klicken Sie so oft wie nötig um den Bildbereich. Beim Klicken zeichnet Dynamic Media Classic die Ränder der Imagemap.

      Nachdem Sie eine Imagemap gezeichnet haben, weist Dynamic Media Classic ihr einen Namen in der Imagemap-Liste zu. Um den Namen zu bilden, hängt Dynamic Media Classic eine sequenzielle Nummer an den Namen der eCatalog-Seite an, auf der Sie arbeiten.

1. (Optional) Geben Sie im Imagemap-Liste-Bedienfeld in der Spalte „Name“ einen neuen Namen für die Imagemap ein. Der von Ihnen eingegebene Name darf keine Leerzeichen enthalten.
1. Sie können festlegen, dass beim Klicken auf eine Imagemap in einem Viewer eine neue Webseite geöffnet wird. Geben Sie im Imagemap-Liste-Bedienfeld in der Spalte „URL“ die URL der Webseite ein.

   Um die Eingabe von URLs (Href templates) zu vereinfachen, klicken Sie auf **[!UICONTROL Bearbeiten]** und geben Sie eine Vorlage ein.

Siehe [Verwenden einer Vorlage zur Eingabe von JavaScript™ und URLs](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Optional) Klicken Sie in der Dropdownliste Anzeigen auf **[!UICONTROL Rollover-Text]** und geben Sie dann den Text ein, den Benutzer auf dem Bildschirm sehen sollen, wenn sie ihre Zeiger über die Imagemap bewegen.
1. (Optional) Klicken Sie in der Dropdownliste Anzeigen auf **[!UICONTROL Andere Aktionen]** und geben Sie ein Attribut ein, um eine Weichzeichnung oder Fokusaktion Trigger, wenn Benutzer den Zeiger über eine Imagemap bewegen.

   Siehe [Definieren anderer Aktionen für Imagemaps](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Klicken Sie auf „**[!UICONTROL Speichern]**“.
1. (Optional) Klicken Sie auf **[!UICONTROL Vorschau]** , um den eCatalog mit der standardmäßigen eCatalog-Viewer-Vorgabe anzuzeigen.

Um eine Imagemap zu löschen, wählen Sie deren Namen in der Liste &quot;Imagemap&quot;aus und klicken Sie auf **[!UICONTROL Löschen]**. Um eine Imagemap vorübergehend auf einer Seite zu deaktivieren, ohne sie jedoch zu löschen, deaktivieren Sie im Imagemap-Liste-Bedienfeld die Option „Ein“ der jeweiligen Imagemap.

## Einbetten von Rich-Media-Daten in einen E-Katalog {#embedding-rich-media-in-an-ecatalog}

Mit der Rich-Media-Option des E-Katalogs können Sie Videos im MP4-Format oder Rotationssets zu Imagemaps hinzufügen, die Sie in einen E-Katalog eingefügt haben. Wenn ein Benutzer auf den Imagemap-Bereich im E-Katalog klickt, wird das verknüpfte Video oder das Rotationsset angezeigt. Diese Funktion ist besonders hilfreich, wenn Sie möchten, dass die Kunden einen Artikel in Aktion oder einen Artikel aus unterschiedlichen Blickwinkeln und Perspektiven sehen können.

Sie können optional auch QuickInfo-Text anzeigen, wenn Kunden ihre Zeiger über Ihre Imagemap bewegen, damit sie wissen, worauf sie klicken.

**So betten Sie Rich-Media-Daten in einen E-Katalog ein:**

1. Zeichnen Sie eine E-Katalog-Imagemap. 

   Siehe [Zeichnen von Imagemaps in E-Katalogen](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. Wählen Sie in der Dropdown-Liste Anzeigen die Option **[!UICONTROL Rich Media]** aus.
1. Navigieren Sie im Bedienfeld „Assets hinzufügen“ links zu einem Ordner, der das Rotationsset oder Video-Asset (MP4-Format) enthält, das Sie einbetten möchten.
1. Ziehen Sie das Asset auf die Imagemap.
1. (Optional) Geben Sie im Listenfeld &quot;Imagemap&quot;unter der Spaltenüberschrift **[!UICONTROL Tool-Tipp]** den Text ein, den die Viewer auf dem Bildschirm sehen sollen, wenn sie ihren Mauszeiger über die Imagemap bewegen.
1. Klicken Sie auf „**[!UICONTROL Speichern]**“.

## Bearbeiten von Imagemaps in E-Katalogen {#editing-ecatalog-image-maps}

Führen Sie auf der Registerkarte „Imagemap-Seiten“ des Anzeigebereichs „E-Katalog“ die folgenden Schritte zum Bearbeiten von Imagemaps in E-Katalogen durch:

* **Position anpassen**  - Wählen Sie das Schwenken-Tool aus und bewegen Sie den Zeiger in die Nähe, jedoch nicht über den Rahmen der Karte. Wenn sich der Zeiger in einen vierköpfigen Pfeil ändert, ziehen Sie die gesamte Imagemap an eine neue Position. 

   Siehe [Anpassen der Position, Form und Größe von Imagemaps](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Ändern der Form und Größe**  - Um die Größe einer rechteckigen Imagemap zu ändern, wählen Sie das Schwenken-Tool aus. Bewegen Sie dann den Mauszeiger über den Rand oder eine Ecke der Imagemap. Wenn der Mauszeiger als Doppelpfeil dargestellt wird, ziehen Sie ihn. Um die Größe einer polygonalen Imagemap zu ändern, ziehen Sie einen quadratischen Auswahlziehpunkt an die gewünschte Stelle. Um einen Auswahlziehpunkt zu erstellen, klicken Sie auf den Rand der Imagemap und beginnen Sie zu ziehen. 

   Siehe [Anpassen der Position, Form und Größe von Imagemaps](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Löschen von Imagemaps** : Wählen Sie das Schwenken-Tool aus, klicken Sie auf die Imagemap, um sie auszuwählen, und klicken Sie dann auf  **[!UICONTROL Löschen]**.

   Um alle Imagemaps aus einem E-Katalog zu entfernen, klicken Sie auf die Registerkarte **[!UICONTROL Seiten bestellen]** und dann auf **[!UICONTROL Maps löschen]**.

* **Handhabung überlappender Imagemaps** : Ziehen Sie, um die Reihenfolge der Imagemaps in der Imagemap-Liste zu ändern.

   Siehe [Beheben von überlappenden Imagemaps](creating-image-maps.md#handling_overlapping_image_maps).

* **Kopieren von Imagemaps auf anderen Seiten**  - Klicken Sie auf  **[!UICONTROL Zuordnungen kopieren nach]**  (stellen Sie sicher, dass Sie sich auf der Registerkarte Zuordnungsseiten befinden). Wählen Sie im Bildschirm &quot;Bilder auswählen&quot;die Seite(n) aus, auf die Sie die Imagemaps kopieren möchten, und klicken Sie auf **[!UICONTROL Auswählen]**.

   Siehe [Kopieren von Imagemaps in andere Bilder](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Sie können Imagemaps nicht nur auf verschiedene Seiten in einem E-Katalog kopieren, sondern auch alle Imagemaps in einem E-Katalog in einen anderen eCatalog kopieren. Siehe [Kopieren von Imagemaps zwischen E-Katalogen](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Überprüfen und Importieren von Imagemap-Daten {#reviewing-and-importing-image-map-data}

Im Anzeigebereich mit der Imagemap-Zusammenfassung werden Metadaten zum E-Katalog angezeigt. Sie können in diesem Anzeigebereich auch einen Stapelimport von Imagemap-Daten für den E-Katalog starten. Ein solcher Import von Imagemap-Daten erleichtert die Eingabe von Imagemap-URLs und Rollover-Text.

Um die Map-Übersicht anzuzeigen, klicken Sie auf der Registerkarte „Imagemap-Seiten“ des E-Katalog-Anzeigebereichs auf „Zusammenfassung“.

### Überprüfen der Zusammenfassung von Imagemap-Daten {#review-image-map-data-summary}

1. Klicken Sie im Bildschirm &quot;Landkartenseiten&quot;auf **[!UICONTROL Zusammenfassung]**.

   Im Anzeigebereich mit der Imagemap-Zusammenfassung wird die Anzahl der im E-Katalog enthaltenen Imagemaps, URLs, Rollover-Textbeschreibungen und anderen Aktionen angezeigt.

1. Wenn Rollover-Schlüssel-Fehler auftreten, klicken Sie in der Spalte **[!UICONTROL Rollover_Key Error]** auf den Fehler, um zu sehen, was in Ihrer Tabelle geändert werden muss, um den Fehler zu korrigieren. Sie können den Text dieser Meldung kopieren und direkt in Ihre Tabelle einfügen.
1. Klicken Sie auf **[!UICONTROL Vorschau]** , um eine Seite im E-Katalog-Viewer zu untersuchen, klicken Sie auf das X, um den Zusammenfassungsbildschirm zu schließen und zum Bildschirm &quot;Zuordnungsseiten&quot;zurückzukehren, oder klicken Sie auf **[!UICONTROL Schließen]**, um zu &quot;Durchsuchen&quot;zurückzukehren.

### Importieren von Imagemap-Daten {#import-image-map-data}

Anstatt auf jeder Seite Imagemap-Daten einzugeben, können Sie über den Anzeigebereich mit der Imagemap-Zusammenfassung auch die Daten für den gesamten E-Katalog importieren. Die Imagemap-Daten werden in Form einer tabulatorgetrennten oder XML DTD-Datei importiert. Die Felder in der Datei müssen dieselbe Reihenfolge haben, wie im Anzeigebereich mit der Imagemap-Zusammenfassung dargestellt: „Name“, „Inhaltsverz.“, „Imagemaps“, „URLs“, „Rollover-Text“, „Andere Aktionen“ und „Suchzeichenfolgen“. Indem Sie Imagemap-Daten importieren, können Sie sich die Arbeit beim Eingeben der Daten in der Imagemap-Liste zum Erstellen der einzelnen Imagemaps sparen.

>[!NOTE]
>
>Bevor Sie Imagemap-Daten importieren können, müssen Sie die Imagemaps bereits erstellt haben.

Führen Sie im Anzeigebereich mit der Imagemap-Zusammenfassung die folgenden Schritte zum Importieren vom Imagemap-Daten für die bereits erstellten Imagemaps aus:

1. Klicken Sie auf **[!UICONTROL Map Data]** importieren.
1. Klicken Sie im Dialogfeld &quot;Metadaten importieren&quot;auf **[!UICONTROL Durchsuchen]** und wählen Sie dann die tabulatorgetrennte oder XML-DTD-Datei aus.
1. Geben Sie im Feld „Auftragsname“ einen Namen für die Datei ein (achten Sie darauf, die Dateinamenerweiterung dabei nicht zu ändern).
1. Klicken Sie auf **[!UICONTROL Hochladen]**.

## Kopieren von Imagemaps zwischen E-Katalogen {#copying-image-maps-between-ecatalogs}

Sie können alle Imagemaps in einem E-Katalog in einen anderen E-Katalog kopieren. Das Kopieren der Imagemaps auf diese Weise ist ein praktisches Verfahren, um Imagemaps zwischen fremdsprachigen Versionen des gleichen E-Katalogs zu kopieren. Damit das Kopieren erfolgreich ist, empfiehlt Dynamic Media Classic das Kopieren zwischen E-Katalogen mit derselben Anzahl von Seiten und Bildern.

>[!NOTE]
>
>Falls der E-Katalog, in den Sie Imagemaps kopieren, bereits Imagemaps enthält, werden diese beim Kopiervorgang gelöscht.

Gehen Sie wie folgt vor, um alle Imagemaps in einem eCatalog in einen anderen eCatalog zu kopieren:

1. Wählen Sie den E-Katalog mit den zu kopierenden Imagemaps aus und klicken Sie auf den Rollover **[!UICONTROL Bearbeiten]** des E-Katalogs.
1. Klicken Sie auf der Registerkarte &quot;Seiten bestellen&quot;auf **[!UICONTROL Maps kopieren]**.
1. Wählen Sie im Dialogfeld &quot;Select Asset&quot;den E-Katalog aus, in den Sie die Imagemaps kopieren möchten, und klicken Sie dann auf **[!UICONTROL Select]**.

Dynamic Media Classic zeigt eine Warnmeldung an, wenn der Ziel-eCatalog (der E-Katalog, in den Sie Imagemaps kopieren) eine andere Anzahl von Seiten oder Bildern mit einer anderen Größe aufweist. Klicken Sie auf **[!UICONTROL Weiter]** , um die Imagemaps trotz der Warnung zu kopieren.
