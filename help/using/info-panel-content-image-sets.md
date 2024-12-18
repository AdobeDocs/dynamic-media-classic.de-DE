---
title: Verwalten von Inhalten des Infobereichs in Bildsets
description: Erfahren Sie, wie Sie den Inhalt des Infobereichs in Bildsets in Adobe Dynamic Media Classic verwalten.
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
topic: Content Management
level: Intermediate
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 34%

---

# Verwalten von Inhalten des Infobereichs in Bildsets{#managing-info-panel-content-in-image-sets}

Zusätzlich zur Verwendung von Imagemap-Text für Ihre Rollover in Bildsets können Sie ein Infobedienfeld verwenden, um größere Mengen an Rollover-Text hinzuzufügen, einschließlich Links. Sie können das InfoPanel auch verwalten, indem Sie die Zeit zwischenspeichern und Inhaltsaktualisierungen planen.

Sie können Ihre InfoPanel-Einrichtung und -Daten mithilfe der folgenden Funktionen in Adobe Dynamic Media Classic verwalten:

* Im Bedienfeld „Info-Bedienfeld-Setup“ können Sie die Vorlage für die Anzeige des Textes im Info-Bedienfeld, eine Standardantwort bei Fehlern und die Anzahl der Stunden, in denen die Informationen zwischengespeichert werden, angeben. Zusätzlich können Sie festlegen, ob der Bildsatz automatisch veröffentlicht werden soll.
* Im Bedienfeld „Info-Bedienfeld“ für den Daten-Feed können Sie eine CSV-Datei mit dem Text angeben, der im Rollover-Text des Info-Bedienfelds angezeigt werden soll, und Zeiten für die Aktualisierung der Informationen planen.
* Im Dialogfeld „Metadaten importieren“ können Sie eine durch Tabulatoren getrennte TXT-Datei importieren, die die Informationen zum Rollover-Text enthält. Sie können diese TXT-Option oder das InfoPanel-Datenfeed-Bedienfeld mit der CSV-Dateioption für Ihren Rollover-Text verwenden.

## Einrichten einer Antwortvorlage für Bildsets {#set-up-a-response-template-for-image-sets}

Sie können eine von drei vorgegebenen Antwortvorlagen für die Anzeige von Text in einem Infofeld auswählen. Diese vorgegebenen Antwortvorlagen bestimmen, wie Ihre Informationen im Infofeld dargestellt werden: Anzahl der Spalten und Zeilen, Schriftbild, Größe, Schriftart usw. Sie können eine vorgegebene Antwortvorlage auswählen oder eine eigene erstellen.

**So richten Sie eine Antwortvorlage für Bildsets ein:**

1. Doppelklicken Sie auf das Bildset, um es in der Detailansicht zu öffnen.
1. Wählen Sie **[!UICONTROL InfoPanel-Einrichtung]** aus.
1. Führen Sie in der Dropdown-Liste „Antwortvorlage“ einen der folgenden Schritte aus:

   * Um die Standardantwort zu verwenden, wählen Sie **[!UICONTROL Standard]** aus. Im Textfeld „Benutzervorlage“ wird, abgeblendet, der XML-Code für den Vorlagenentwurf angezeigt.
   * Um Ihre eigene Antwortvorlage zu erstellen, wählen Sie **[!UICONTROL Benutzerdefiniert]** aus. Geben Sie in das Textfeld „Benutzervorlage“ die XML-Definition der Vorlage ein. Sie können die Standardvorlage verwenden, die im Textfeld als Basis für Ihre eigene Antwort bereits definiert ist.

1. (Optional) Geben Sie in das Feld „Standardantwort“ den Text ein, der angezeigt werden soll, wenn Adobe Dynamic Media Classic beim Abrufen von Informationen für eine Imagemap auf einen Fehler stößt. Wenn das System beispielsweise einen Firmennamen und einen Bildsatznamen, jedoch keinen Rollover-Bezeichner empfängt, wird dem Benutzer diese Meldung angezeigt.
1. Geben Sie in das Textfeld „Antwort-TTL“ die Anzahl der Stunden bis zum Zwischenspeichern der Daten ein.

   * Geben Sie eine niedrigere Zahl ein, wenn die Daten im Verlauf des Tages häufig aktualisiert werden.
   * Geben Sie eine höhere Zahl ein, falls die Daten relativ stabil sind und nicht so häufig aktualisiert werden müssen. Der Standardwert lautet zehn Stunden.

1. Wählen Sie **[!UICONTROL Hochladen]** aus, um Inhalte des Informationsbereichs basierend auf dem Wert „rollover_key“ in s7info hochzuladen.
1. Suchen Sie im Dialogfeld „S7Info-Upload“ nach der gewünschten Datei und wählen Sie &quot;**[!UICONTROL &quot;]**.

   Unterstützte Dateiformate sind TAB-getrennte Dateien mit UTF-16-Kodierung und CSV-Dateien mit ASCII-Kodierung. Bei CSV-Dateien müssen Nicht-ASCII-Zeichen HTML-kodiert sein.

1. Wählen Sie im Bedienfeld „InfoPanel-Setup“ **[!UICONTROL Publish]**.

## Importieren von Quellinhalten für das Infobedienfeld in Bildsets {#import-source-content-for-the-info-panel-in-image-sets}

Sie können eine CSV-Datei (kommagetrennte Wertedatei) mit ASCII-Codierung (Nicht-ASCII-Zeichen müssen HTML-codiert sein) oder eine durch Tabulatoren getrennte Datei für den Quelltext eines Info-Bedienfelds für ein Bildset verwenden. Tabulatorgetrennte Dateien müssen die UTF-16-Kodierung (Unicode) verwenden. Sie können die verschiedenen Dateitypen mit verschiedenen Methoden importieren.

Beachten Sie beim Formatieren von Quellinhalt die folgenden Richtlinien:

* Die tabulator- und kommagetrennten Daten können so viele Spalten enthalten, wie für die Rollover-Vorlage erforderlich sind.
* Das erste Datenelement oder die erste Datenspalte ist die Rollover-Kennung (die mit dem Wert rollover_key aus den Imagemap-URLs verknüpft ist).
* Stellen Sie sicher, dass jedes durch Tabulatoren oder Kommas getrennte Element nach der Kennung das Element ist, das Sie in die Antwortvorlage ersetzen möchten. Die erste Spalte wird also durch $1$ ersetzt, die zweite Spalte durch $2$ usw.).

### Importieren von CSV-Inhalten in Bildsets von einem extern gehosteten Speicherort {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Doppelklicken Sie auf das Bildset, damit es in der Detailansicht geöffnet wird.
1. Wählen Sie **[!UICONTROL InfoPanel-Daten-Feed]**.
1. Geben Sie in das Textfeld der extern gehosteten CSV-Datei (HTTP) die URL der CSV-Datei ein.
1. (Optional) Geben Sie im Feld Zeitplanaktualisierung einen Zeitpunkt für die Aktualisierung des Inhalts ein und wählen Sie dann **[!UICONTROL Hinzufügen]**.

   Sie können mehrere Zeitpunkte für die Aktualisierung auswählen. Jede Aktualisierungszeit wird im Textfeld „Zeiten aktualisieren“ angegeben. Um eine geplante Zeit zu entfernen, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Löschen]**.

1. (Optional) Wählen Sie **[!UICONTROL Aktualisierung ausführen]** aus, damit Sie den Inhalt sofort aktualisieren können.
