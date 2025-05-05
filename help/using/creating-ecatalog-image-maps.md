---
title: Erstellen von E-Katalog-Imagemaps
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic E-Katalog-Imagemaps erstellen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 26%

---

# Erstellen von E-Katalog-Imagemaps{#creating-ecatalog-image-maps}

Eine Imagemap ist ein Bereich auf einer E-Katalog-Seite, über den Sie mit der Maus bzw. mit der Maus einen Trigger erstellen können. Wenn Sie den Mauszeiger über eine Imagemap bewegen, wird beispielsweise eine Rollover-Textbeschreibung eines Elements angezeigt. Wenn Sie eine Imagemap auswählen, wird eine andere Aktion initiiert. Sie können beispielsweise eine Web-Seite öffnen, damit Betrachterinnen und Betrachter mehr über ein Element erfahren oder es kaufen können, oder Sie können ein Video starten, um ein in Gebrauch befindliches Element anzuzeigen.

## E-Katalog-Imagemaps zeichnen {#drawing-ecatalog-image-maps}

Imagemaps für E-Kataloge werden auf der Registerkarte „Imagemap-Seiten“ des Anzeigebereichs „E-Katalog“ gezeichnet. In diesem Anzeigebereich wird links der Bereich „Imagemap“ mit den E-Katalogseiten und rechts eine Liste mit Imagemaps angezeigt. Wenn Sie Imagemaps erstellen, werden deren Namen in die Liste der Imagemaps eingetragen.

1. Wählen Sie die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** des E-Katalogs aus.
1. Wählen Sie **[!UICONTROL Seiten zuordnen]** aus.
1. Wählen Sie links im Anzeigebereich „Imagemap-Seiten“ die gewünschte Seite aus.
1. Zeichnen Sie im Bereich „Imagemap“ eine rechteckige oder polygonale (vieleckige) Imagemap:

   * **Rechteckige Karte**: Wählen Sie das Rechteck-Imagemap-Werkzeug aus und ziehen Sie auf die Seite, um das Rechteck zu erstellen.

   * **Polygonzuordnung**: Wählen Sie das Werkzeug Polygon-Imagemap und wählen Sie dann so oft wie nötig um den Umfang des Bildes aus. Wenn Sie diese Option auswählen, zeichnet Adobe Dynamic Media Classic die Ränder der Imagemap.

     Nachdem Sie eine Imagemap gezeichnet haben, weist Adobe Dynamic Media Classic ihr einen Namen in der Liste „Imagemap“ zu. Um den Namen zu bilden, hängt Adobe Dynamic Media Classic eine sequenzielle Nummer an den Namen der E-Katalog-Seite an, auf der Sie arbeiten.

1. (Optional) In der Liste „Imagemap“ können [!UICONTROL &#x200B; in der Spalte &#x200B;] einen neuen Namen für die Imagemap eingeben. Der von Ihnen eingegebene Name darf keine Leerzeichen enthalten.
1. Viewer können eine neue Web-Seite öffnen, wenn sie auf die Imagemap klicken. Geben Sie im Listenfeld „Imagemap“ die URL der Web-Seite in die Spalte URL ein.

   Um das Eingeben von URLs (href-Vorlagen) zu vereinfachen, wählen Sie **[!UICONTROL Bearbeiten]** und geben Sie eine Vorlage ein.

Siehe [Verwenden einer Vorlage zum Eingeben von JavaScript und URLs](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. (Optional) Wählen Sie in der Dropdown-Liste Anzeigen die Option **[!UICONTROL Rollover-Text]** aus und geben Sie dann den Text ein, der Benutzern auf dem Bildschirm angezeigt werden soll, wenn sie mit dem Mauszeiger auf die Imagemap zeigen.
1. (Optional) Wählen Sie in der Dropdown-Liste Anzeigen die Option **[!UICONTROL Sonstige Aktionen]** und geben Sie ein Attribut für eine Trigger- oder Fokusaktion ein, wenn Benutzer ihre Zeiger über eine Imagemap bewegen.

   Siehe [Definieren anderer Aktionen für Imagemaps](creating-image-maps.md#defining_other_actions_for_image_maps).

1. Wählen Sie **[!UICONTROL Speichern]** aus.
1. (Optional) Klicken Sie auf **[!UICONTROL Vorschau]**, um den E-Katalog mit der standardmäßigen E-Katalog-Viewer-Vorgabe anzuzeigen.

Um eine Imagemap zu löschen, wählen Sie ihren Namen in der Liste Imagemap aus und klicken Sie auf **[!UICONTROL Löschen]**. Sie können eine Imagemap auf einer Seite vorübergehend deaktivieren, ohne die Imagemap zu löschen. Wählen Sie die Option Imagemaps auf im Listenfeld „Imagemap“ aus.

## Einbetten von Rich-Media in einen E-Katalog {#embedding-rich-media-in-an-ecatalog}

Mit der Rich-Media-Option von eCatalog können Sie Videos im MP4-Format oder Rotationssets zu Imagemaps hinzufügen, die Sie einem eCatalog hinzugefügt haben. Wenn ein(e) Benutzende(r) den Bereich „Imagemap“ im E-Katalog auswählt, wird das zugehörige Rotationsset oder Video angezeigt. Diese Funktion ist besonders hilfreich, wenn Sie möchten, dass die Kunden einen Artikel in Aktion oder einen Artikel aus unterschiedlichen Blickwinkeln und Perspektiven sehen können.

Optional können Sie auch QuickInfo-Text anzeigen, wenn Kundinnen und Kunden ihre Zeiger über Ihre Imagemap bewegen, damit sie wissen, welche Auswahl sie treffen.

**So betten Sie Rich-Media in einen E-Katalog ein:**

1. Zeichnen Sie eine E-Katalog-Imagemap. 

   Siehe [E-Katalog-Imagemaps zeichnen](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. Wählen Sie in der Dropdown-Liste Anzeigen die Option **[!UICONTROL Rich Media]** aus.
1. Navigieren Sie im Bedienfeld Assets hinzufügen auf der linken Seite zu einem Ordner, der das Rotationsset oder Video-Asset (MP4-Format) enthält, das Sie einbetten möchten.
1. Ziehen Sie das Asset auf die Imagemap.
1. (Optional) Geben Sie im Listenfeld „Imagemap“ unter der Spaltenüberschrift **[!UICONTROL QuickInfo]** den Text ein, den die Betrachter auf dem Bildschirm sehen sollen, wenn sie mit dem Mauszeiger auf die Imagemap zeigen.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

## Bearbeiten von Imagemaps in E-Katalogen {#editing-ecatalog-image-maps}

Führen Sie auf der Registerkarte „Imagemap-Seiten“ des Anzeigebereichs „E-Katalog“ die folgenden Schritte zum Bearbeiten von Imagemaps in E-Katalogen durch:

* **Position anpassen**: Wählen Sie das Tool Schwenken aus, und bewegen Sie den Mauszeiger in die Nähe der Karte, aber nicht über deren Rand. Wenn der Mauszeiger einen Pfeil mit vier Spitzen anzeigt, ziehen Sie die gesamte Imagemap an eine neue Position.

  Siehe [Anpassen von Position, Form und Größe von Imagemaps](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Form und Größe ändern**: Um die Größe einer rechteckigen Imagemap zu ändern, wählen Sie das Tool „Schwenken“ aus. Bewegen Sie dann den Mauszeiger über den Rand oder eine Ecke der Imagemap. Wenn der Mauszeiger als Doppelpfeil dargestellt wird, ziehen Sie ihn. Um die Größe einer polygonalen Imagemap zu ändern, ziehen Sie einen quadratischen Auswahlziehpunkt an die gewünschte Stelle. Um einen Auswahlpunkt zu erstellen, wählen Sie den Rahmen der Imagemap aus und ziehen Sie ihn.

  Siehe [Anpassen von Position, Form und Größe von Imagemaps](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **Löschen von Imagemaps**: Wählen Sie das Tool „Schwenken“, wählen Sie die Imagemap aus, um sie auszuwählen, und klicken Sie dann auf **[!UICONTROL Löschen]**.

  Um alle Imagemaps aus einem E-Katalog zu entfernen, wählen Sie die Registerkarte **[!UICONTROL Bestellen]** und dann **[!UICONTROL Karten löschen]** aus.

* **Überlappende Imagemaps handhaben**: Ziehen Sie, um die Reihenfolge der Imagemaps in der Imagemap-Liste zu ändern.

  Siehe [Überlappende Imagemaps ](creating-image-maps.md#handling_overlapping_image_maps).

* **Kopieren von Imagemaps auf andere Seiten**: Wählen Sie **[!UICONTROL Karten kopieren nach]** (stellen Sie sicher, dass Sie sich auf der Registerkarte Seiten zuordnen befinden). Wählen Sie auf dem Bildschirm „Bilder auswählen“ die Seite(n) aus, auf die Sie die Imagemaps kopieren möchten, und klicken Sie auf **[!UICONTROL Auswählen]**.

  Siehe [Kopieren von Imagemaps in andere ](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>Wenn Sie Imagemaps auf verschiedene Seiten in einem E-Katalog kopieren, können Sie alle Imagemaps in einem E-Katalog in einen anderen E-Katalog kopieren. Siehe [Kopieren von Imagemaps unter anderen E-Katalogen](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## Überprüfen und Importieren von Imagemap-Daten {#reviewing-and-importing-image-map-data}

Im Anzeigebereich mit der Imagemap-Zusammenfassung werden Metadaten zum E-Katalog angezeigt. Sie können in diesem Anzeigebereich auch einen Stapelimport von Imagemap-Daten für den E-Katalog starten. Ein solcher Import von Imagemap-Daten erleichtert die Eingabe von Imagemap-URLs und Rollover-Text.

Um den Bildschirm „Zuordnungszusammenfassung“ anzuzeigen, wählen Sie auf der Registerkarte „Zuordnungsseiten“ des Bildschirms „E-Katalog **[!UICONTROL die Option „Zusammenfassung]**.

### Überprüfen der Zusammenfassung von Imagemap-Daten {#review-image-map-data-summary}

1. Wählen Sie im Bildschirm Seiten zuordnen die Option **[!UICONTROL Zusammenfassung]** aus.

   Der Bildschirm Zuordnungszusammenfassung zeigt an, wie viele Imagemaps, URLs, Rollover-Textbeschreibungen und andere Aktionen in Ihrem E-Katalog sind.

1. Wenn Rollover-Schlüssel-Fehler auftreten, wählen Sie den Fehler in der Spalte **[!UICONTROL Rollover-Schlüssel-Fehler]** aus, um zu sehen, was sich in Ihrer Tabelle ändern muss, um den Fehler zu korrigieren. Sie können den Text dieser Meldung kopieren und direkt in Ihre Tabelle einfügen.
1. Wählen Sie **[!UICONTROL Vorschau]** aus, um eine Seite im E-Katalog-Viewer zu untersuchen. Wählen Sie das X aus, um den Bildschirm Zusammenfassung zu schließen und zum Bildschirm Seiten zuordnen zurückzukehren, oder wählen Sie **[!UICONTROL Schließen]** aus, um zum Durchsuchen zurückzukehren.

### Importieren von Imagemap-Daten {#import-image-map-data}

Anstatt auf jeder Seite Imagemap-Daten einzugeben, können Sie über den Anzeigebereich mit der Imagemap-Zusammenfassung auch die Daten für den gesamten E-Katalog importieren. Die Imagemap-Daten werden in Form einer tabulatorgetrennten oder XML DTD-Datei importiert. Die Felder in der Datei müssen dieselbe Reihenfolge haben, wie im Anzeigebereich mit der Imagemap-Zusammenfassung dargestellt: „Name“, „Inhaltsverz.“, „Imagemaps“, „URLs“, „Rollover-Text“, „Andere Aktionen“ und „Suchzeichenfolgen“. Durch den Import von Imagemap-Daten müssen Sie die Daten nicht erst in die Imagemap-Liste eingeben, wenn Sie jede Imagemap erstellen.

>[!NOTE]
>
>Bevor Sie Imagemap-Daten importieren können, müssen Sie die Imagemaps bereits erstellt haben.

Führen Sie im Anzeigebereich mit der Imagemap-Zusammenfassung die folgenden Schritte zum Importieren vom Imagemap-Daten für die bereits erstellten Imagemaps aus:

1. Wählen **[!UICONTROL Zuordnungsdaten importieren]**.
1. Wählen Sie im Dialogfeld Metadaten importieren die Option **[!UICONTROL Durchsuchen]** und wählen Sie dann die durch Tabulatoren getrennte oder XML-DTD-Datei aus.
1. Geben Sie im Feld „Auftragsname“ einen Namen für die Datei ein (achten Sie darauf, die Dateinamenerweiterung dabei nicht zu ändern).
1. Wählen Sie **[!UICONTROL Hochladen]** aus.

## Kopieren von Imagemaps unter anderen E-Katalogen {#copying-image-maps-between-ecatalogs}

Sie können alle Imagemaps in einem E-Katalog in einen anderen E-Katalog kopieren. Das Kopieren der Imagemaps auf diese Weise ist ein praktisches Verfahren, um Imagemaps zwischen fremdsprachigen Versionen des gleichen E-Katalogs zu kopieren. Damit das Kopieren erfolgreich ist, empfiehlt Adobe Dynamic Media Classic, zwischen E-Katalogen mit derselben Seitenanzahl und denselben Bildern zu kopieren.

>[!NOTE]
>
>Falls der E-Katalog, in den Sie Imagemaps kopieren, bereits Imagemaps enthält, werden diese beim Kopiervorgang gelöscht.

Gehen Sie wie folgt vor, um alle Imagemaps in einem E-Katalog in einen anderen E-Katalog zu kopieren:

1. Wählen Sie den E-Katalog mit den Imagemaps aus, die Sie kopieren möchten, und klicken Sie auf die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** des E-Katalogs.
1. Wählen Sie auf der Registerkarte Bestellseiten die Option **[!UICONTROL Karten kopieren]**.
1. Wählen Sie im Dialogfeld Asset auswählen den E-Katalog aus, in den Sie die Imagemaps kopieren möchten, und klicken Sie dann auf **[!UICONTROL Auswählen]**.

Adobe Dynamic Media Classic zeigt eine Warnmeldung an, wenn der Ziel-E-Katalog, aus dem Sie Imagemaps kopieren, eine andere Anzahl von Seiten oder Bildern aufweist, die eine andere Größe aufweisen. Wählen Sie **[!UICONTROL Weiter]** aus, um die Imagemaps trotz der Warnung zu kopieren.
