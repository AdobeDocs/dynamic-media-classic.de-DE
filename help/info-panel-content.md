---
title: Verwalten des Infofeldinhalts in E-Katalogen
description: Erfahren Sie, wie Sie Infofeldinhalte in E-Katalogen verwalten.
uuid: 5aa634f9-0874-4bb5-a3d9-8ce4d5577941
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: be277831-77cc-4011-ae30-e75c18eec99b
feature: Dynamic Media Classic, Viewer, E-Katalog
role: Business Practitioner
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
translation-type: tm+mt
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 67%

---

# Verwalten des Infofeldinhalts in E-Katalogen{#managing-info-panel-content-in-ecatalogs}

Sie können den Imagemap-Text für Ihre Rollover in E-Katalogen verwenden. Darüber hinaus besteht jedoch auch die Möglichkeit, anhand eines Infofelds größere Mengen von Rollover-Text, einschließlich Links, hinzuzufügen. Zur Verwaltung des Infofelds können Sie zeitlich begrenztes Caching und geplante Inhaltsaktualisierungen verwenden.

Sie können Ihre Infofeld-Einrichtung und Ihre Daten mithilfe der folgenden Funktionen in Dynamic Media Classic verwalten:

* Im Bedienbereich „Infofeld-Einrichtung“ können Sie Folgendes angeben: die Vorlage, die für die Anzeige des Infofeldtexts verwendet werden soll, eine Standardantwort bei Fehlern sowie die Dauer (in Stunden), die diese Informationen zwischengespeichert werden sollen. Zusätzlich können Sie festlegen, ob der E-Katalog automatisch veröffentlicht werden soll.
* Im Bedienfeld &quot;Infofeld-Daten-Feed&quot;können Sie eine CSV-Datei angeben, die den Text enthält, der im Rollover-Text des Infofelds angezeigt werden soll, sowie die Zeitpläne für die Aktualisierung der Informationen.
* Über das Dialogfeld „Metadaten importieren“ (Zugriff über die Ansicht „Imagemap-Seiten“) können Sie eine tabulatorgetrennte TXT-Datei mit den Informationen zum Rollover-Text importieren. Sie können diese TXT-Option oder das Datafeed-Bedienfeld mit der CSV-Dateioption für Ihren Rollover-Text verwenden.
* In der Ansicht „Imagemap-Seiten“ steht eine Option zur Verfügung, mit der Sie eine Vorschau des XML-Codes für die einzelnen Imagemaps aufrufen können.

## Einrichten einer Antwortvorlage für E-Kataloge {#set-up-a-response-template-for-ecatalogs}

Sie können eine von drei vorgegebenen Antwortvorlagen für die Anzeige von Text in einem Infofeld auswählen. Diese vorgegebenen Antwortvorlagen bestimmen, wie Ihre Informationen im Infofeld dargestellt werden: Anzahl der Spalten und Zeilen, Schriftbild, Größe, Schriftart usw. Sie können eine vorgegebene Antwortvorlage auswählen oder eine eigene erstellen.

>[!NOTE]
>
>Sie können die Antwortvorlage auch in der Viewer-Vorgabe einrichten. Um stattdessen die Antwortvorlage in der Viewer-Vorgabe zu verwenden, fügen Sie am Ende der Infoserver-URL in der Viewer-Vorgabe `fmt=1` hinzu.
>
>Siehe [Konfigurieren von E-Katalog-Viewer-Vorgaben](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. Doppelklicken Sie auf Ihren E-Katalog, um ihn in der Detailansicht zu öffnen.
1. Klicken Sie auf das Infofeld-Setup.
1. Wählen Sie eine Antwortvorlage aus:

   * Wählen Sie eine Vorgabe aus dem Menü „Antwortvorlage“ aus. Der XML-Code für den Vorlagenentwurf wird im Feld „Benutzervorlage“ angezeigt.
   * Um eine eigene Antwortvorlage zu erstellen, wählen Sie **[!UICONTROL Benutzerdefiniert]**. Geben Sie die XML-Definition der Vorlage in das Feld „Benutzervorlage“ ein. Sie können die vorgegebenen Vorlagen als Grundlage für Ihre eigenen verwenden. 

1. (Optional) Geben Sie im Feld &quot;Standardantwort&quot;den Text ein, der angezeigt werden soll, wenn beim Abrufen von Informationen für eine Imagemap ein Fehler in Dynamic Media Classic auftritt. Wenn das System beispielsweise einen Firmennamen und einen E-Katalog-Namen, jedoch keinen Rollover-Bezeichner empfängt, so wird dem Benutzer diese Meldung angezeigt.
1. Geben Sie die Anzahl der Stunden bis zum Zwischenspeichern der Daten in das Feld „Antwort-TTL“ ein:

   * Geben Sie eine niedrigere Zahl ein, wenn die Daten im Verlauf des Tages häufig aktualisiert werden.
   * Geben Sie eine höhere Zahl ein, falls die Daten relativ stabil sind und nicht so häufig aktualisiert werden müssen. Der Standardwert lautet zehn Stunden.

1. Klicken Sie auf **[!UICONTROL Veröffentlichen]**.

## Importieren von Quellinhalten für das Infofeld in E-Katalogen {#import-source-content-for-the-info-panel-in-ecatalogs}

Sie können eine kommagetrennte (CSV) oder tabulatorgetrennte (TXT) Datei für den Quelltext des Infofelds für einen E-Katalog verwenden. Tabulatorgetrennte Dateien müssen die UTF16-Kodierung (Unicode) verwenden. Verschiedene Dateitypen werden mithilfe unterschiedlicher Methoden importiert.

Beachten Sie beim Formatieren von Quellinhalt die folgenden Richtlinien:

* Stellen Sie sicher, dass die tabulator- und kommagetrennten Daten so viele Spalten enthalten, wie für die Rollover-Vorlage benötigt werden.
* Stellen Sie sicher, dass das erste Element bzw. die erste Datenspalte der Rollover-Bezeichner ist (verknüpft mit dem rollover_key-Wert aus der URL der Imagemap).
* Stellen Sie sicher, dass jedes tabulatorgetrennte oder kommagetrennte Element nach dem Bezeichner das Element ist, das in der Antwortvorlage ersetzt werden soll. Die erste Spalte wird also in $1$, die zweite in $2$ usw. ersetzt.

### Importieren von CSV-Inhalten aus einem extern gehosteten Speicherort {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location} in E-Kataloge

1. Doppelklicken Sie auf den E-Katalog, um ihn in der Detailansicht zu öffnen.
1. Klicken Sie auf das Bedienfeld Infofeld-Daten.
1. Geben Sie die URL für die CSV-Datei in das Feld „Speicherort der extern gehosteten CSV-Datei (HTTP)“ ein. Sie können diese URL in das Feld kopieren oder sie direkt eintippen.
1. (Optional) Geben Sie im Menü „Terminplanaktualisierung“ eine Zeit an, zu der die Aktualisierung der Inhalte stattfinden soll, und klicken Sie auf „Hinzufügen“. Sie können mehrere Zeitpunkte für die Aktualisierung auswählen. Jede Aktualisierungszeit wird im Feld „Zeiten aktualisieren“ angegeben. (Um eine Zeit zu löschen, wählen Sie diese aus und klicken dann auf „Löschen“).
1. (Optional) Klicken Sie auf „Aktualisierung jetzt ausführen“, um den Inhalt sofort zu aktualisieren.

### Importieren einer tabulatorgetrennten oder CSV-Datei  {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Doppelklicken Sie auf den E-Katalog, um ihn in der Detailansicht zu öffnen.
1. Klicken Sie auf das Infofeld-Setup.
1. Klicken Sie auf **[!UICONTROL S7Info-Inhalt hochladen]**.
1. Klicken Sie auf **[!UICONTROL Durchsuchen]**, wählen Sie die tabulatorgetrennte TXT-, CSV- oder SSV-Datei aus, die Sie verwenden möchten, und klicken Sie auf **[!UICONTROL Öffnen]**.
1. Klicken Sie auf **[!UICONTROL Hochladen]**.

Dynamic Media Classic sendet Ihnen eine E-Mail, in der Sie wissen, ob der Upload erfolgreich war oder nicht.

## Anzeigen der Vorschau für Rollover-Text für eine Imagemap {#preview-rollover-key-text-for-an-image-map}

Im Anzeigebereich „Imagemap-Seiten“ können Sie einfach und schnell den Infofeldtext für die Imagemaps auf einer bestimmten Seite Ihres E-Katalogs anzeigen.

1. Klicken Sie auf die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** des Katalogs.
1. Klicken Sie auf **[!UICONTROL Imagemap-Seiten]**.
1. Wählen Sie oben in der Tabelle auf der rechten Seite des Bildschirms im Menü &quot;Anzeigen&quot;die Option **[!UICONTROL Infofeld]**.

   Der Rollover-Schlüssel-Text wird neben jeder Image Map angezeigt, die Informationsfenster-Text enthält.
