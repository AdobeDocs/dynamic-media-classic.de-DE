---
title: Verwalten des Infofeldinhalts in Bildsätzen
description: Erfahren Sie, wie Sie Infofeldinhalte in Bildsätzen verwalten.
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
feature: Dynamic Media Classic, Viewer, Bildsätze
role: Business Practitioner
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
translation-type: tm+mt
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '763'
ht-degree: 54%

---

# Verwalten des Infofeldinhalts in Bildsätzen{#managing-info-panel-content-in-image-sets}

Zusätzlich zur Verwendung von Imagemap-Text für Ihre Rollover in Bildsätzen können Sie zum Hinzufügen größerer Mengen von Rollover-Text, einschließlich Links, ein Infofeld verwenden. Sie können das Infofeld auch mithilfe von zeitlich begrenztem Caching und geplanten Inhaltsaktualisierungen verwalten.

Sie können Ihre Infofeld-Einrichtung und Ihre Daten mithilfe der folgenden Funktionen in Dynamic Media Classic verwalten:

* Im Bedienbereich „Infofeld-Einrichtung“ können Sie Folgendes angeben: die Vorlage, die für die Anzeige des Infofeldtexts verwendet werden soll, eine Standardantwort bei Fehlern sowie die Dauer (in Stunden), die diese Informationen zwischengespeichert werden sollen. Zusätzlich können Sie festlegen, ob der Bildsatz automatisch veröffentlicht werden soll.
* Im Bedienfeld &quot;Infofeld-Daten-Feed&quot;können Sie eine CSV-Datei angeben, die den Text enthält, der im Rollover-Text des Infofelds angezeigt werden soll, sowie die Zeitpläne für die Aktualisierung der Informationen.
* Mit dem Dialogfeld „Metadaten importieren“ können Sie eine tabulatorgetrennte TXT-Datei importieren, die die Rollover-Textdaten enthält. Sie können diese TXT-Option oder das Infofeld-Datenfeed-Bedienfeld mit der CSV-Dateioption für Ihren Rollover-Text verwenden.

## Einrichten einer Antwortvorlage für Bildsätze {#set-up-a-response-template-for-image-sets}

Sie können eine von drei vorgegebenen Antwortvorlagen für die Anzeige von Text in einem Infofeld auswählen. Diese vorgegebenen Antwortvorlagen bestimmen, wie Ihre Informationen im Infofeld dargestellt werden: Anzahl der Spalten und Zeilen, Schriftbild, Größe, Schriftart usw. Sie können eine vorgegebene Antwortvorlage auswählen oder eine eigene erstellen.

**So richten Sie eine Antwortvorlage ein:**

1. Doppelklicken Sie auf Ihren Bildsatz, um ihn in der Detailansicht zu öffnen.
1. Klicken Sie auf **[!UICONTROL Infofeld-Einrichtung]**.
1. Führen Sie in der Dropdown-Liste „Antwortvorlage“ einen der folgenden Schritte aus:

   * Um die Standardantwort zu verwenden, wählen Sie **[!UICONTROL Standard]**. Im Textfeld „Benutzervorlage“ wird, abgeblendet, der XML-Code für den Vorlagenentwurf angezeigt.
   * Um eine eigene Antwortvorlage zu erstellen, wählen Sie **[!UICONTROL Benutzerdefiniert]**. Geben Sie in das Textfeld „Benutzervorlage“ die XML-Definition der Vorlage ein. Sie können die Standardvorlage verwenden, die im Textfeld als Basis für Ihre eigene Antwort bereits definiert ist.

1. (Optional) Geben Sie im Feld &quot;Standardantwort&quot;den Text ein, der angezeigt werden soll, wenn beim Abrufen von Informationen für eine Imagemap ein Fehler in Dynamic Media Classic auftritt. Wenn das System beispielsweise einen Firmennamen und einen Bildsatznamen, jedoch keinen Rollover-Bezeichner empfängt, wird dem Benutzer diese Meldung angezeigt.
1. Geben Sie in das Textfeld „Antwort-TTL“ die Anzahl der Stunden bis zum Zwischenspeichern der Daten ein.

   * Geben Sie eine niedrigere Zahl ein, wenn die Daten im Verlauf des Tages häufig aktualisiert werden.
   * Geben Sie eine höhere Zahl ein, falls die Daten relativ stabil sind und nicht so häufig aktualisiert werden müssen. Der Standardwert lautet zehn Stunden.

1. Klicken Sie auf **[!UICONTROL Hochladen]**, um den Inhalt des Infofelds basierend auf den rollover_key-Werten in s7info hochzuladen.
1. Navigieren Sie im Dialogfeld &quot;S7Info-Upload&quot;zu der gewünschten Datei und klicken Sie dann auf **[!UICONTROL Upload]**.

   Unterstützte Dateiformate sind TAB-getrennte Dateien mit UTF-16-Kodierung und CSV-Dateien mit ASCII-Kodierung. Bei CSV-Dateien müssen Nicht-ASCII-Zeichen HTML-kodiert sein.

1. Klicken Sie im Infofeld-Setup auf **[!UICONTROL Veröffentlichen]**.

## Importieren von Quellinhalt für das Infofeld in Bildsätzen {#import-source-content-for-the-info-panel-in-image-sets}

Sie können für den Quelltext eines Infofelds für einen Bildsatz eine CSV-Datei (kommagetrennte Werte) mit ASCII-Kodierung (Nicht-ASCII-Zeichen müssen HTML-kodiert sein) oder eine tabulatorgetrennte Datei verwenden. Tabulatorgetrennte Dateien müssen die UTF-16-Kodierung (Unicode) verwenden. Verschiedene Dateitypen werden mithilfe unterschiedlicher Methoden importiert.

Beachten Sie beim Formatieren von Quellinhalt die folgenden Richtlinien:

* Die tabulatorgetrennten und kommagetrennten Daten können so viele Spalten enthalten, wie für die Rollover-Vorlage erforderlich sind.
* Das erste Element oder die erste Datenspalte ist der Rollover-Bezeichner (verknüpft mit dem rollover_key-Wert aus den Imagemap-URLs).
* Stellen Sie sicher, dass jedes tabulatorgetrennte oder kommagetrennte Element nach dem Bezeichner das Element ist, das in der Antwortvorlage ersetzt werden soll. Die erste Spalte wird also in $1$, die zweite in $2$ usw. ersetzt.

### Importieren von CSV-Inhalten aus einem extern gehosteten Speicherort {#import-csv-content-into-image-sets-from-an-externally-hosted-location} in Bildsätze

1. Doppelklicken Sie auf den Bildsatz, um ihn in der Detailansicht zu öffnen.
1. Klicken Sie auf **[!UICONTROL Infofeld-Daten]**.
1. Geben Sie in das Textfeld der extern gehosteten CSV-Datei (HTTP) die URL der CSV-Datei ein.
1. (Optional) Geben Sie in den Feldern &quot;Planaktualisierung&quot;einen Zeitpunkt für die Aktualisierung des Inhalts ein und klicken Sie dann auf **[!UICONTROL Hinzufügen]**.

   Sie können mehrere Zeitpunkte für die Aktualisierung auswählen. Jede Aktualisierungszeit wird im Textfeld „Zeiten aktualisieren“ angegeben. Um eine geplante Zeit zu entfernen, wählen Sie sie aus und klicken Sie dann auf **[!UICONTROL Löschen]**.

1. (Optional) Klicken Sie auf **[!UICONTROL Aktualisierung ausführen]**, um den Inhalt sofort zu aktualisieren.
