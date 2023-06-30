---
title: Verwalten des Infofeldinhalts in Bildsets
description: Erfahren Sie, wie Sie den Inhalt des Infofelds in Bildsets in Adobe Dynamic Media Classic verwalten.
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 51%

---

# Verwalten des Infofeldinhalts in Bildsets{#managing-info-panel-content-in-image-sets}

Zusätzlich zur Verwendung von Imagemap-Text für Ihre Rollover in Bildsätzen können Sie zum Hinzufügen größerer Mengen von Rollover-Text, einschließlich Links, ein Infofeld verwenden. Sie können das Infofeld auch mithilfe von zeitlich begrenztem Caching und geplanten Inhaltsaktualisierungen verwalten.

Sie können die Einrichtung und die Daten des InfoPanel mit den folgenden Funktionen in Adobe Dynamic Media Classic verwalten:

* Im Bedienbereich „Infofeld-Einrichtung“ können Sie Folgendes angeben: die Vorlage, die für die Anzeige des Infofeldtexts verwendet werden soll, eine Standardantwort bei Fehlern sowie die Dauer (in Stunden), die diese Informationen zwischengespeichert werden sollen. Zusätzlich können Sie festlegen, ob der Bildsatz automatisch veröffentlicht werden soll.
* Im Bedienfeld &quot;InfoPanel-Datenfluss&quot;können Sie eine CSV-Datei angeben, die den Text enthält, der im Rollover-Text des Infofelds angezeigt werden soll, und Zeitpläne für die Aktualisierung der Informationen festlegen.
* Mit dem Dialogfeld „Metadaten importieren“ können Sie eine tabulatorgetrennte TXT-Datei importieren, die die Rollover-Textdaten enthält. Sie können diese TXT-Option oder das InfoPanel-Daten-Feed-Bedienfeld mit der CSV-Dateioption für Ihren Rollover-Text verwenden.

## Einrichten einer Antwortvorlage für Bildsets {#set-up-a-response-template-for-image-sets}

Sie können eine von drei vorgegebenen Antwortvorlagen für die Anzeige von Text in einem Infofeld auswählen. Diese vorgegebenen Antwortvorlagen bestimmen, wie Ihre Informationen im Infofeld dargestellt werden: Anzahl der Spalten und Zeilen, Schriftbild, Größe, Schriftart usw. Sie können eine vorgegebene Antwortvorlage auswählen oder eine eigene erstellen.

**So richten Sie eine Antwortvorlage für Bildsets ein:**

1. Doppelklicken Sie auf das Bildset, damit es in der Detailansicht geöffnet wird.
1. Auswählen **[!UICONTROL InfoPanel-Einrichtung]**.
1. Führen Sie in der Dropdown-Liste „Antwortvorlage“ einen der folgenden Schritte aus:

   * Um die Standardantwort zu verwenden, wählen Sie **[!UICONTROL Standard]**. Im Textfeld „Benutzervorlage“ wird, abgeblendet, der XML-Code für den Vorlagenentwurf angezeigt.
   * Um eine eigene Antwortvorlage zu erstellen, wählen Sie **[!UICONTROL Benutzerdefiniert]**. Geben Sie in das Textfeld „Benutzervorlage“ die XML-Definition der Vorlage ein. Sie können die Standardvorlage verwenden, die im Textfeld als Basis für Ihre eigene Antwort bereits definiert ist.

1. (Optional) Geben Sie im Feld &quot;Standardantwort&quot;den Text ein, der angezeigt werden soll, wenn bei Adobe Dynamic Media Classic beim Abrufen von Informationen für eine Imagemap ein Fehler auftritt. Wenn das System beispielsweise einen Firmennamen und einen Bildsatznamen, jedoch keinen Rollover-Bezeichner empfängt, wird dem Benutzer diese Meldung angezeigt.
1. Geben Sie in das Textfeld „Antwort-TTL“ die Anzahl der Stunden bis zum Zwischenspeichern der Daten ein.

   * Geben Sie eine niedrigere Zahl ein, wenn die Daten im Verlauf des Tages häufig aktualisiert werden.
   * Geben Sie eine höhere Zahl ein, falls die Daten relativ stabil sind und nicht so häufig aktualisiert werden müssen. Der Standardwert lautet zehn Stunden.

1. Auswählen **[!UICONTROL Hochladen]** , um Informationsbereichsinhalte basierend auf den rollover_key -Werten in s7info hochzuladen.
1. Navigieren Sie im Dialogfeld &quot;S7Info Upload&quot;zu der Datei, die Sie verwenden möchten, und wählen Sie **[!UICONTROL Hochladen]**.

   Unterstützte Dateiformate sind TAB-getrennte Dateien mit UTF-16-Kodierung und CSV-Dateien mit ASCII-Kodierung. Bei CSV-Dateien müssen Nicht-ASCII-Zeichen HTML-kodiert sein.

1. Wählen Sie im Bereich &quot;InfoPanel Setup&quot;die Option **[!UICONTROL Veröffentlichen]**.

## Importieren des Quellinhalts für das Info-Bedienfeld in Bildsets {#import-source-content-for-the-info-panel-in-image-sets}

Sie können für den Quelltext eines Infofelds für einen Bildsatz eine CSV-Datei (kommagetrennte Werte) mit ASCII-Kodierung (Nicht-ASCII-Zeichen müssen HTML-kodiert sein) oder eine tabulatorgetrennte Datei verwenden. Tabulatorgetrennte Dateien müssen die UTF-16-Kodierung (Unicode) verwenden. Verschiedene Dateitypen werden mithilfe unterschiedlicher Methoden importiert.

Beachten Sie beim Formatieren von Quellinhalt die folgenden Richtlinien:

* Die tabulatorgetrennten und kommagetrennten Daten können so viele Spalten enthalten, wie für die Rollover-Vorlage erforderlich sind.
* Das erste Element bzw. die erste Datenspalte ist die Rollover-ID (verknüpft mit dem Wert rollover_key aus den Imagemap-URLs).
* Stellen Sie sicher, dass jedes tabulatorgetrennte oder kommagetrennte Element nach der Kennung das Element ist, das in der Antwortvorlage ersetzt werden soll. Die erste Spalte wird also in $1$, die zweite in $2$ usw. ersetzt.

### Importieren von CSV-Inhalten in Bildsets von einem extern gehosteten Speicherort {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. Doppelklicken Sie auf das Bildset, damit es in der Detailansicht geöffnet wird.
1. Auswählen **[!UICONTROL InfoPanel Datafeed]**.
1. Geben Sie in das Textfeld der extern gehosteten CSV-Datei (HTTP) die URL der CSV-Datei ein.
1. (Optional) Geben Sie in den Feldern Planung aktualisieren einen Zeitpunkt für die Inhaltsaktualisierung an und wählen Sie dann **[!UICONTROL Hinzufügen]**.

   Sie können mehrere Zeitpunkte für die Aktualisierung auswählen. Jede Aktualisierungszeit wird im Textfeld „Zeiten aktualisieren“ angegeben. Um eine geplante Zeit zu entfernen, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Löschen]**.

1. (Optional) Wählen Sie **[!UICONTROL Update ausführen]** , um den Inhalt sofort zu aktualisieren.
