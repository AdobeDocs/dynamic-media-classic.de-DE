---
title: Verwalten von Inhalten im Informationsbereich in E-Katalogen
description: Erfahren Sie, wie Sie den Inhalt des Infofelds in E-Katalogen in Adobe Dynamic Media Classic verwalten.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 40%

---

# Verwalten von Inhalten im Informationsbereich in E-Katalogen{#managing-info-panel-content-in-ecatalogs}

Sie können den Imagemap-Text für Ihre Rollover in E-Katalogen verwenden. Darüber hinaus besteht jedoch auch die Möglichkeit, anhand eines Infofelds größere Mengen von Rollover-Text, einschließlich Links, hinzuzufügen. Sie können das InfoPanel auch verwalten, indem Sie zeitgesteuerte Zwischenspeicherung verwenden und Inhaltsaktualisierungen planen.

Sie können die Einrichtung und die Daten des InfoPanel mit den folgenden Funktionen in Adobe Dynamic Media Classic verwalten:

* Im Bereich &quot;InfoPanel-Einrichtung&quot;können Sie die Vorlage für die Anzeige des Infofeldtexts, eine Standardantwort für Fehler und die Anzahl der Stunden angeben, in denen die Informationen zwischengespeichert werden. Zusätzlich können Sie festlegen, ob der E-Katalog automatisch veröffentlicht werden soll.
* Im Feed-Bedienfeld &quot;InfoPanel-Daten&quot;können Sie eine CSV-Datei angeben, die den Text enthält, der im Rollover-Text des InfoPanel angezeigt werden soll, und Zeitpläne für die Aktualisierung der Informationen festlegen.
* Im Dialogfeld Metadaten importieren (Zugriff über die Ansicht &quot;Zuordnungsseiten&quot;) können Sie eine tabulatorgetrennte TXT-Datei importieren, die die Rollover-Textinformationen enthält. Sie können diese TXT-Option oder das Daten-Feed-Bedienfeld mit der CSV-Dateioption für Ihren Rollover-Text verwenden.
* Die Ansicht &quot;Zuordnungsseiten&quot;bietet eine Option zur Vorschau der XML-Datei, die für bestimmte Imagemaps angezeigt wird.

## Einrichten einer Antwortvorlage für E-Kataloge {#set-up-a-response-template-for-ecatalogs}

Sie können eine von drei vorgegebenen Antwortvorlagen für die Anzeige von Text in einem Infofeld auswählen. Diese vorgegebenen Antwortvorlagen bestimmen, wie Ihre Informationen im Infofeld dargestellt werden: Anzahl der Spalten und Zeilen, Schriftbild, Größe, Schriftart usw. Sie können eine vordefinierte Antwortvorlage auswählen oder eine eigene erstellen.

>[!NOTE]
>
>Sie können die Antwortvorlage auch in der Viewer-Vorgabe einrichten. Um stattdessen die Antwortvorlage in der Viewer-Vorgabe zu verwenden, fügen Sie in der Viewer-Vorgabe am Ende der URL für den Informationsserver &quot;`fmt=1`&quot;hinzu.
>
>Siehe [Einrichten von E-Katalog-Viewer-Vorgaben](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. Doppelklicken Sie auf Ihren eCatalog, damit er in der Detailansicht geöffnet wird.
1. Wählen Sie den Bereich **[!UICONTROL InfoPanel Setup]** aus.
1. Wählen Sie eine Antwortvorlage aus:

   * Wählen Sie eine Vorgabe aus dem Menü „Antwortvorlage“ aus. Der XML-Code für den Vorlagenentwurf wird im Feld „Benutzervorlage“ angezeigt.
   * Um eine eigene Antwortvorlage zu erstellen, wählen Sie **[!UICONTROL Benutzerdefiniert]** aus. Geben Sie die XML-Definition der Vorlage in das Feld „Benutzervorlage“ ein. Sie können die vorgegebenen Vorlagen als Grundlage für Ihre eigenen verwenden. 

1. (Optional) Geben Sie im Feld &quot;Standardantwort&quot;den Text ein, der angezeigt werden soll, wenn in Adobe Dynamic Media Classic beim Abrufen von Informationen für eine Imagemap ein Fehler auftritt. Wenn das System beispielsweise einen Firmennamen und einen E-Katalog-Namen, jedoch keinen Rollover-Bezeichner empfängt, so wird dem Benutzer diese Meldung angezeigt.
1. Geben Sie die Anzahl der Stunden bis zum Zwischenspeichern der Daten in das Feld „Antwort-TTL“ ein:

   * Geben Sie eine niedrigere Zahl ein, wenn die Daten im Verlauf des Tages häufig aktualisiert werden.
   * Legen Sie eine höhere Zahl fest, wenn die Daten relativ stabil sind und nicht häufig täglich aktualisiert werden müssen. Der Standardwert lautet zehn Stunden.

1. Wählen Sie **[!UICONTROL Publish]** aus.

## Importieren von Quellinhalten für das Info-Bedienfeld in E-Katalogen {#import-source-content-for-the-info-panel-in-ecatalogs}

Sie können eine kommagetrennte (CSV) oder tabulatorgetrennte (TXT) Datei für den Quelltext des Infofelds für einen E-Katalog verwenden. Tabulatorgetrennte Dateien müssen die UTF16-Kodierung (Unicode) verwenden. Sie können die verschiedenen Dateitypen mit verschiedenen Methoden importieren.

Beachten Sie beim Formatieren von Quellinhalt die folgenden Richtlinien:

* Stellen Sie sicher, dass die tabulator- und kommagetrennten Daten so viele Spalten enthalten, wie für die Rollover-Vorlage benötigt werden.
* Stellen Sie sicher, dass das erste Element oder die erste Datenspalte die Rollover-ID ist (die mit dem Wert rollover_key aus den Imagemap-URLs verknüpft ist).
* Stellen Sie sicher, dass jedes tabulatorgetrennte oder kommagetrennte Element nach dem Bezeichner das Element ist, das in der Antwortvorlage ersetzt werden soll. Die erste Spalte wird also in $1$, die zweite in $2$ usw. ersetzt.

### Importieren von CSV-Inhalten aus einem extern gehosteten Speicherort in E-Kataloge {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Doppelklicken Sie auf den eCatalog, damit er in der Detailansicht geöffnet wird.
1. Wählen Sie den Bereich **[!UICONTROL InfoPanel-Daten-Feed]** aus.
1. Geben Sie die URL für die CSV-Datei in das Feld „Speicherort der extern gehosteten CSV-Datei (HTTP)“ ein. Sie können diese URL in das Feld kopieren oder sie direkt eintippen.
1. (Optional) Geben Sie im Menü &quot;Zeitplanaktualisierung&quot;einen Zeitpunkt für die Aktualisierung des Inhalts an und wählen Sie **[!UICONTROL Hinzufügen]** aus. Sie können mehrere Zeitpunkte für die Aktualisierung auswählen. Jede Aktualisierungszeit wird im Feld „Zeiten aktualisieren“ angegeben. (Um eine Zeit zu entfernen, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Löschen]**.)
1. (Optional) Wählen Sie **[!UICONTROL Update jetzt ausführen]** aus, damit Sie den Inhalt sofort aktualisieren können.

### Importieren einer tabulatorgetrennten oder CSV-Datei {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Doppelklicken Sie auf den eCatalog, damit er in der Detailansicht geöffnet wird.
1. Wählen Sie den Bereich **[!UICONTROL InfoPanel Setup]** aus.
1. Wählen Sie **[!UICONTROL S7Info-Inhalt hochladen]** aus.
1. Wählen Sie **[!UICONTROL Durchsuchen]**, wählen Sie die TXT-Datei, CSV- oder SSV-Datei mit Tabulatortrennzeichen aus, die Sie verwenden möchten, und wählen Sie **[!UICONTROL Öffnen]** aus.
1. Wählen Sie **[!UICONTROL Upload]** aus.

Adobe Dynamic Media Classic sendet Ihnen eine E-Mail, in der Sie darüber informiert werden, ob der Upload erfolgreich war oder nicht.

## Anzeigen der Vorschau für Rollover-Text für eine Imagemap {#preview-rollover-key-text-for-an-image-map}

Im Anzeigebereich „Imagemap-Seiten“ können Sie einfach und schnell den Infofeldtext für die Imagemaps auf einer bestimmten Seite Ihres E-Katalogs anzeigen.

1. Wählen Sie die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** des Katalogs aus.
1. Wählen Sie **[!UICONTROL Seiten zuordnen]** aus.
1. Wählen Sie oben in der Tabelle rechts auf dem Bildschirm im Menü &quot;Anzeigen&quot;die Option **[!UICONTROL Infofeld]**.

   Der Rollover-Text wird neben jeder Imagemap mit Infofeld-Text angezeigt.
