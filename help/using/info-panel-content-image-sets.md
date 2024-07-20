---
title: Verwalten des Infofeldinhalts in Bildsets
description: Erfahren Sie, wie Sie den Inhalt des Infofelds in Bildsets in Adobe Dynamic Media Classic verwalten.
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

# Verwalten des Infofeldinhalts in Bildsets{#managing-info-panel-content-in-image-sets}

Sie können nicht nur Imagemap-Text für Ihre Rollover in Bildsets verwenden, sondern auch ein Info-Bedienfeld, um größere Mengen von Rollover-Text, einschließlich Links, hinzuzufügen. Sie können das InfoPanel auch verwalten, indem Sie die Zeitzwischenspeicherung verwenden und Inhaltsaktualisierungen planen.

Sie können die Einrichtung und die Daten des InfoPanel mit den folgenden Funktionen in Adobe Dynamic Media Classic verwalten:

* Im Bereich &quot;Infobereich-Einrichtung&quot;können Sie die Vorlage für die Anzeige des Infofeldtexts, eine Standardantwort für Fehler und die Anzahl der Stunden angeben, in denen die Informationen zwischengespeichert werden. Zusätzlich können Sie festlegen, ob der Bildsatz automatisch veröffentlicht werden soll.
* Im Bereich Daten-Feed für das Infofeld können Sie eine CSV-Datei mit dem Text angeben, der im Rollover-Text des Infofelds angezeigt werden soll, und Zeitpläne für die Aktualisierung der Informationen festlegen.
* Im Dialogfeld Metadaten importieren können Sie eine tabulatorgetrennte TXT-Datei importieren, die die Rollover-Textinformationen enthält. Sie können diese TXT-Option oder das InfoPanel-Daten-Feed-Bedienfeld mit der CSV-Dateioption für Ihren Rollover-Text verwenden.

## Einrichten einer Antwortvorlage für Bildsets {#set-up-a-response-template-for-image-sets}

Sie können eine von drei vorgegebenen Antwortvorlagen für die Anzeige von Text in einem Infofeld auswählen. Diese vorgegebenen Antwortvorlagen bestimmen, wie Ihre Informationen im Infofeld dargestellt werden: Anzahl der Spalten und Zeilen, Schriftbild, Größe, Schriftart usw. Sie können eine vorgegebene Antwortvorlage auswählen oder eine eigene erstellen.

**So richten Sie eine Antwortvorlage für Bildsets ein:**

1. Doppelklicken Sie auf das Bildset, damit es in der Detailansicht geöffnet wird.
1. Wählen Sie **[!UICONTROL InfoPanel-Einrichtung]** aus.
1. Führen Sie in der Dropdown-Liste „Antwortvorlage“ einen der folgenden Schritte aus:

   * Um die Standardantwort zu verwenden, wählen Sie **[!UICONTROL Standard]** aus. Im Textfeld „Benutzervorlage“ wird, abgeblendet, der XML-Code für den Vorlagenentwurf angezeigt.
   * Um eine eigene Antwortvorlage zu erstellen, wählen Sie **[!UICONTROL Benutzerdefiniert]** aus. Geben Sie in das Textfeld „Benutzervorlage“ die XML-Definition der Vorlage ein. Sie können die Standardvorlage verwenden, die im Textfeld als Basis für Ihre eigene Antwort bereits definiert ist.

1. (Optional) Geben Sie im Feld &quot;Standardantwort&quot;den Text ein, der angezeigt werden soll, wenn bei Adobe Dynamic Media Classic beim Abrufen von Informationen für eine Imagemap ein Fehler auftritt. Wenn das System beispielsweise einen Firmennamen und einen Bildsatznamen, jedoch keinen Rollover-Bezeichner empfängt, wird dem Benutzer diese Meldung angezeigt.
1. Geben Sie in das Textfeld „Antwort-TTL“ die Anzahl der Stunden bis zum Zwischenspeichern der Daten ein.

   * Geben Sie eine niedrigere Zahl ein, wenn die Daten im Verlauf des Tages häufig aktualisiert werden.
   * Geben Sie eine höhere Zahl ein, falls die Daten relativ stabil sind und nicht so häufig aktualisiert werden müssen. Der Standardwert lautet zehn Stunden.

1. Wählen Sie **[!UICONTROL Hochladen]** aus, um den Inhalt des Infofelds basierend auf dem Wert rollover_key in s7info hochzuladen.
1. Navigieren Sie im Dialogfeld &quot;S7Info Upload&quot;zu der Datei, die Sie verwenden möchten, und wählen Sie dann **[!UICONTROL Upload]** aus.

   Unterstützte Dateiformate sind TAB-getrennte Dateien mit UTF-16-Kodierung und CSV-Dateien mit ASCII-Kodierung. Bei CSV-Dateien müssen Nicht-ASCII-Zeichen HTML-kodiert sein.

1. Wählen Sie im Bereich &quot;InfoPanel Setup&quot;die Option **[!UICONTROL Publish]**.

## Importieren des Quellinhalts für das Info-Bedienfeld in Bildsets {#import-source-content-for-the-info-panel-in-image-sets}

Sie können eine CSV-Datei (kommagetrennter Wert) mit ASCII-Kodierung (Nicht-ASCII-Zeichen müssen HTML-kodiert sein) oder eine tabulatorgetrennte Datei für den Quelltext eines Informationssystems für ein Bildset verwenden. Tabulatorgetrennte Dateien müssen die UTF-16-Kodierung (Unicode) verwenden. Sie können die verschiedenen Dateitypen mit verschiedenen Methoden importieren.

Beachten Sie beim Formatieren von Quellinhalt die folgenden Richtlinien:

* Die tabulatorgetrennten und kommagetrennten Daten können so viele Spalten enthalten, wie für die Rollover-Vorlage erforderlich sind.
* Das erste Element bzw. die erste Datenspalte ist die Rollover-ID (verknüpft mit dem Wert rollover_key aus den Imagemap-URLs).
* Stellen Sie sicher, dass jedes tabulatorgetrennte oder kommagetrennte Element nach der Kennung das Element ist, das in der Antwortvorlage ersetzt werden soll. Die erste Spalte wird also in $1$, die zweite in $2$ usw. ersetzt.

### Importieren von CSV-Inhalten in Bildsets von einem extern gehosteten Speicherort {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Doppelklicken Sie auf das Bildset, damit es in der Detailansicht geöffnet wird.
1. Wählen Sie **[!UICONTROL InfoPanel-Daten-Feed]** aus.
1. Geben Sie in das Textfeld der extern gehosteten CSV-Datei (HTTP) die URL der CSV-Datei ein.
1. (Optional) Geben Sie im Feld &quot;Planung aktualisieren&quot;einen Zeitpunkt für die Aktualisierung des Inhalts an und wählen Sie dann **[!UICONTROL Hinzufügen]** aus.

   Sie können mehrere Zeitpunkte für die Aktualisierung auswählen. Jede Aktualisierungszeit wird im Textfeld „Zeiten aktualisieren“ angegeben. Um eine geplante Zeit zu entfernen, wählen Sie sie aus und klicken Sie dann auf **[!UICONTROL Löschen]**.

1. (Optional) Wählen Sie **[!UICONTROL Aktualisierung ausführen]** aus, damit Sie den Inhalt sofort aktualisieren können.
