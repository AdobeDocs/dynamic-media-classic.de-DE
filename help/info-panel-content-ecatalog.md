---
title: Verwalten von Inhalten im Informationsbereich in E-Katalogen
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic den Inhalt des Info-Bedienfelds in E-Katalogen verwalten.
uuid: 5aa634f9-0874-4bb5-a3d9-8ce4d5577941
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: be277831-77cc-4011-ae30-e75c18eec99b
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 59%

---

# Verwalten von Inhalten im Informationsbereich in E-Katalogen{#managing-info-panel-content-in-ecatalogs}

Sie können den Imagemap-Text für Ihre Rollover in E-Katalogen verwenden. Darüber hinaus besteht jedoch auch die Möglichkeit, anhand eines Infofelds größere Mengen von Rollover-Text, einschließlich Links, hinzuzufügen. Zur Verwaltung des Infofelds können Sie zeitlich begrenztes Caching und geplante Inhaltsaktualisierungen verwenden.

Sie können Ihre InfoPanel-Einrichtung und Ihre Daten mithilfe der folgenden Funktionen in Adobe Dynamic Media Classic verwalten:

* Im Bedienbereich „Infofeld-Einrichtung“ können Sie Folgendes angeben: die Vorlage, die für die Anzeige des Infofeldtexts verwendet werden soll, eine Standardantwort bei Fehlern sowie die Dauer (in Stunden), die diese Informationen zwischengespeichert werden sollen. Zusätzlich können Sie festlegen, ob der E-Katalog automatisch veröffentlicht werden soll.
* Im Bedienfeld &quot;InfoPanel-Datenfluss&quot;können Sie eine CSV-Datei angeben, die den Text enthält, der im Rollover-Text des InfoPanel angezeigt werden soll, und Zeitpläne für die Aktualisierung der Informationen festlegen.
* Über das Dialogfeld „Metadaten importieren“ (Zugriff über die Ansicht „Imagemap-Seiten“) können Sie eine tabulatorgetrennte TXT-Datei mit den Informationen zum Rollover-Text importieren. Sie können diese TXT-Option oder das Datafeed-Bedienfeld mit der CSV-Dateioption für Ihren Rollover-Text verwenden.
* In der Ansicht „Imagemap-Seiten“ steht eine Option zur Verfügung, mit der Sie eine Vorschau des XML-Codes für die einzelnen Imagemaps aufrufen können.

## Einrichten einer Antwortvorlage für E-Kataloge {#set-up-a-response-template-for-ecatalogs}

Sie können eine von drei vorgegebenen Antwortvorlagen für die Anzeige von Text in einem Infofeld auswählen. Diese vorgegebenen Antwortvorlagen bestimmen, wie Ihre Informationen im Infofeld dargestellt werden: Anzahl der Spalten und Zeilen, Schriftbild, Größe, Schriftart usw. Sie können eine vorgegebene Antwortvorlage auswählen oder eine eigene erstellen.

>[!NOTE]
>
>Sie können die Antwortvorlage auch in der Viewer-Vorgabe einrichten. Um stattdessen die Antwortvorlage in der Viewer-Vorgabe zu verwenden, fügen Sie `fmt=1` am Ende der URL des Informationsservers in der Viewer-Vorgabe hinzu.
>
>Siehe [E-Katalog-Viewer-Vorgaben einrichten](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. Doppelklicken Sie auf Ihren eCatalog, damit er in der Detailansicht geöffnet wird.
1. Wählen Sie das Bedienfeld **[!UICONTROL InfoPanel Setup]** aus.
1. Wählen Sie eine Antwortvorlage aus:

   * Wählen Sie eine Vorgabe aus dem Menü „Antwortvorlage“ aus. Der XML-Code für den Vorlagenentwurf wird im Feld „Benutzervorlage“ angezeigt.
   * Um eine eigene Antwortvorlage zu erstellen, wählen Sie **[!UICONTROL Benutzerdefiniert]** aus. Geben Sie die XML-Definition der Vorlage in das Feld „Benutzervorlage“ ein. Sie können die vorgegebenen Vorlagen als Grundlage für Ihre eigenen verwenden. 

1. (Optional) Geben Sie im Feld &quot;Standardantwort&quot;den Text ein, der angezeigt werden soll, wenn in Adobe Dynamic Media Classic beim Abrufen von Informationen für eine Imagemap ein Fehler auftritt. Wenn das System beispielsweise einen Firmennamen und einen E-Katalog-Namen, jedoch keinen Rollover-Bezeichner empfängt, so wird dem Benutzer diese Meldung angezeigt.
1. Geben Sie die Anzahl der Stunden bis zum Zwischenspeichern der Daten in das Feld „Antwort-TTL“ ein:

   * Geben Sie eine niedrigere Zahl ein, wenn die Daten im Verlauf des Tages häufig aktualisiert werden.
   * Geben Sie eine höhere Zahl ein, falls die Daten relativ stabil sind und nicht so häufig aktualisiert werden müssen. Der Standardwert lautet zehn Stunden.

1. Wählen Sie **[!UICONTROL Publish]** aus.

## Importieren von Quellinhalten für das Info-Bedienfeld in E-Katalogen {#import-source-content-for-the-info-panel-in-ecatalogs}

Sie können eine kommagetrennte (CSV) oder tabulatorgetrennte (TXT) Datei für den Quelltext des Infofelds für einen E-Katalog verwenden. Tabulatorgetrennte Dateien müssen die UTF16-Kodierung (Unicode) verwenden. Verschiedene Dateitypen werden mithilfe unterschiedlicher Methoden importiert.

Beachten Sie beim Formatieren von Quellinhalt die folgenden Richtlinien:

* Stellen Sie sicher, dass die tabulator- und kommagetrennten Daten so viele Spalten enthalten, wie für die Rollover-Vorlage benötigt werden.
* Stellen Sie sicher, dass das erste Element bzw. die erste Datenspalte der Rollover-Bezeichner ist (verknüpft mit dem rollover_key-Wert aus der URL der Imagemap).
* Stellen Sie sicher, dass jedes tabulatorgetrennte oder kommagetrennte Element nach der Kennung das Element ist, das in der Antwortvorlage ersetzt werden soll. Die erste Spalte wird also in $1$, die zweite in $2$ usw. ersetzt.

### Importieren von CSV-Inhalten aus einem extern gehosteten Speicherort in E-Kataloge {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Doppelklicken Sie auf den eCatalog, damit er in der Detailansicht geöffnet wird.
1. Wählen Sie das Bedienfeld **[!UICONTROL InfoPanel Datafeed]** aus.
1. Geben Sie die URL für die CSV-Datei in das Feld „Speicherort der extern gehosteten CSV-Datei (HTTP)“ ein. Sie können diese URL in das Feld kopieren oder sie direkt eintippen.
1. (Optional) Geben Sie einen Zeitpunkt für die Inhaltsaktualisierung mithilfe der Menüs Zeitplanaktualisierung an und wählen Sie **[!UICONTROL Hinzufügen]** aus. Sie können mehrere Zeitpunkte für die Aktualisierung auswählen. Jede Aktualisierungszeit wird im Feld „Zeiten aktualisieren“ angegeben. (Um eine Zeit zu entfernen, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Löschen]**.)
1. (Optional) Wählen Sie **[!UICONTROL Jetzt aktualisieren ausführen]** aus, um den Inhalt sofort zu aktualisieren.

### Importieren einer tabulatorgetrennten oder CSV-Datei {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Doppelklicken Sie auf den eCatalog, damit er in der Detailansicht geöffnet wird.
1. Wählen Sie das Bedienfeld **[!UICONTROL InfoPanel Setup]** aus.
1. Wählen Sie **[!UICONTROL S7Info Content]** hochladen.
1. Wählen Sie **[!UICONTROL Durchsuchen]**, wählen Sie die tabulatorgetrennte TXT-, CSV- oder SSV-Datei aus, die Sie verwenden möchten, und wählen Sie **[!UICONTROL Öffnen]** aus.
1. Wählen Sie **[!UICONTROL Upload]** aus.

Adobe Dynamic Media Classic sendet Ihnen eine E-Mail, in der Sie darüber informiert werden, ob der Upload erfolgreich war oder nicht.

## Anzeigen der Vorschau für Rollover-Text für eine Imagemap {#preview-rollover-key-text-for-an-image-map}

Im Anzeigebereich „Imagemap-Seiten“ können Sie einfach und schnell den Infofeldtext für die Imagemaps auf einer bestimmten Seite Ihres E-Katalogs anzeigen.

1. Wählen Sie die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** des Katalogs aus.
1. Wählen Sie **[!UICONTROL Seiten zuordnen]** aus.
1. Wählen Sie oben in der Tabelle auf der rechten Bildschirmseite **[!UICONTROL Infofeld]** aus dem Menü Anzeigen .

   Der Rollover-Schlüssel-Text wird neben jeder Image Map angezeigt, die Informationsfenster-Text enthält.
