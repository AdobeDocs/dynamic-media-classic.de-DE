---
title: Verwalten des Infofeldinhalts in Bildsätzen
seo-title: Verwalten des Infofeldinhalts in Bildsätzen
description: 'null'
seo-description: Erfahren Sie, wie Sie Infofeldinhalte in Bildsätzen verwalten.
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 73%

---


# Verwalten des Infofeldinhalts in Bildsätzen{#managing-info-panel-content-in-image-sets}

Zusätzlich zur Verwendung von Imagemap-Text für Ihre Rollover in Bildsätzen können Sie zum Hinzufügen größerer Mengen von Rollover-Text, einschließlich Links, ein Infofeld verwenden. Sie können das Infofeld auch mithilfe von zeitlich begrenztem Caching und geplanten Inhaltsaktualisierungen verwalten.

Sie können Ihre Infofeld-Einrichtung und Ihre Daten mithilfe der folgenden Funktionen in Dynamic Media Classic verwalten:

* Im Bedienbereich „Infofeld-Einrichtung“ können Sie Folgendes angeben: die Vorlage, die für die Anzeige des Infofeldtexts verwendet werden soll, eine Standardantwort bei Fehlern sowie die Dauer (in Stunden), die diese Informationen zwischengespeichert werden sollen. Zusätzlich können Sie festlegen, ob der Bildsatz automatisch veröffentlicht werden soll.
* Im Bedienfeld „Infofeld-Daten-Feed“ können Sie Folgendes angeben: eine CSV-Datei, die den Text enthält, der im Rollover-Text des Infofelds angezeigt werden soll, sowie die geplanten Zeiten zum Aktualisieren der Informationen.
* Mit dem Dialogfeld „Metadaten importieren“ können Sie eine tabulatorgetrennte TXT-Datei importieren, die die Rollover-Textdaten enthält. Sie können für Ihren Rollover-Text diese TXT-Option oder das Bedienfeld „Infofeld-Daten-Feed“ mit der CSV-Dateioption verwenden.

## Einrichten einer Antwortvorlage für Bildsätze {#set-up-a-response-template-for-image-sets}

Sie können eine von drei vorgegebenen Antwortvorlagen für die Anzeige von Text in einem Infofeld auswählen. Diese vorgegebenen Antwortvorlagen bestimmen, wie Ihre Informationen im Infofeld dargestellt werden: Anzahl der Spalten und Zeilen, Schriftbild, Größe, Schriftart usw. Sie können eine vorgegebene Antwortvorlage auswählen oder eine eigene erstellen.

**So richten Sie eine Antwortvorlage ein**

1. Doppelklicken Sie auf Ihren Bildsatz, um ihn in der Detailansicht zu öffnen.
1. Click **InfoPanel Setup** to unfold the panel.
1. Führen Sie in der Dropdown-Liste „Antwortvorlage“ einen der folgenden Schritte aus:

   * Wählen Sie „Standard“, um die Standardantwort zu verwenden. Im Textfeld „Benutzervorlage“ wird, abgeblendet, der XML-Code für den Vorlagenentwurf angezeigt.
   * Wählen Sie „Benutzerdefiniert“, um eine eigene Antwortvorlage zu erstellen. Geben Sie in das Textfeld „Benutzervorlage“ die XML-Definition der Vorlage ein. Sie können die Standardvorlage verwenden, die im Textfeld als Basis für Ihre eigene Antwort bereits definiert ist.

1. (Optional) Geben Sie im Feld &quot;Standardantwort&quot;den Text ein, der angezeigt werden soll, wenn Dynamic Media Classic beim Abrufen von Informationen für eine Imagemap auf einen Fehler stößt. Wenn das System beispielsweise einen Firmennamen und einen Bildsatznamen, jedoch keinen Rollover-Bezeichner empfängt, wird dem Benutzer diese Meldung angezeigt.
1. Geben Sie in das Textfeld „Antwort-TTL“ die Anzahl der Stunden bis zum Zwischenspeichern der Daten ein.

   * Geben Sie eine niedrigere Zahl ein, wenn die Daten im Verlauf des Tages häufig aktualisiert werden.
   * Geben Sie eine höhere Zahl ein, falls die Daten relativ stabil sind und nicht so häufig aktualisiert werden müssen. Der Standardwert lautet zehn Stunden.

1. Click **Upload** to upload info panel content, based on the rollover_key values, to s7info.
1. In the S7Info Upload dialog box, browse to the file that you want to use, and then click **Upload**.

   Es werden tabulatorgetrennte Dateien mit UTF-16-Kodierung und CSV-Dateien mit ASCII-Kodierung unterstützt. Bei CSV-Dateien müssen Nicht-ASCII-Zeichen HTML-kodiert sein.

1. In the InfoPanel Setup panel, click **Publish**.

## Importieren von Quellinhalt für das Infofeld in Bildsätzen {#import-source-content-for-the-info-panel-in-image-sets}

Sie können für den Quelltext eines Infofelds für einen Bildsatz eine CSV-Datei (kommagetrennte Werte) mit ASCII-Kodierung (Nicht-ASCII-Zeichen müssen HTML-kodiert sein) oder eine tabulatorgetrennte Datei verwenden. Tabulatorgetrennte Dateien müssen die UTF-16-Kodierung (Unicode) verwenden. Verschiedene Dateitypen werden mithilfe unterschiedlicher Methoden importiert.

Beachten Sie beim Formatieren von Quellinhalt die folgenden Richtlinien:

* Die tabulator- und kommagetrennten Daten müssen alle notwendigen Spalten für die Rollover-Vorlage enthalten.
* Das erste Element oder die erste Datenspalte muss der Rollover-Bezeichner sein (verknüpft mit dem rollover_key-Wert aus den Imagemap-URLs).
* Stellen Sie sicher, dass jedes tabulator- oder kommagetrennte Element nach dem Bezeichner das Element ist, das in der Antwortvorlage ersetzt werden soll (sodass also für die erste Spalte $1$, für die zweite $2$ usw. eingesetzt wird).

### Importieren von CSV-Inhalten aus einem extern gehosteten Speicherort in Bildsätze {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Doppelklicken Sie auf den Bildsatz, um ihn in der Detailansicht zu öffnen.
1. Click **InfoPanel Datafeed** to unfold the panel.
1. Geben Sie in das Textfeld der extern gehosteten CSV-Datei (HTTP) die URL der CSV-Datei ein.
1. (Optional) In the Schedule Update fields, specify a time to update the content, and then click **Add**.

   Sie können mehrere Zeitpunkte für die Aktualisierung auswählen. Jede Aktualisierungszeit wird im Textfeld „Zeiten aktualisieren“ angegeben. To remove a scheduled time, select it, and then click **Delete**.

1. (Optional) Click **Run Update** to immediately update the content.

