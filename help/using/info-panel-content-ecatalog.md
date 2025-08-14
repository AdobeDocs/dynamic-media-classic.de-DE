---
title: Verwalten von Inhalten des Infobereichs in E-Katalogen
description: Erfahren Sie, wie Sie den Inhalt des Infobereichs in E-Katalogen in Adobe Dynamic Media Classic verwalten.
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

# Verwalten von Inhalten des Infobereichs in E-Katalogen{#managing-info-panel-content-in-ecatalogs}

Sie können den Imagemap-Text für Ihre Rollover in E-Katalogen verwenden. Darüber hinaus besteht jedoch auch die Möglichkeit, anhand eines Infofelds größere Mengen von Rollover-Text, einschließlich Links, hinzuzufügen. Sie können das InfoPanel auch verwalten, indem Sie eine zeitgesteuerte Zwischenspeicherung verwenden und Inhaltsaktualisierungen planen.

Sie können Ihre InfoPanel-Einrichtung und -Daten mithilfe der folgenden Funktionen in Adobe Dynamic Media Classic verwalten:

* Im Bedienfeld „InfoPanel-Einrichtung“ können Sie die Vorlage für die Anzeige des Textes im InfoPanel, eine Standardantwort bei Fehlern und die Anzahl der Stunden, in denen die Informationen zwischengespeichert werden, angeben. Zusätzlich können Sie festlegen, ob der E-Katalog automatisch veröffentlicht werden soll.
* Im Bedienfeld InfoPanel-Datenfeed können Sie eine CSV-Datei angeben, die den Text enthält, der im InfoPanel-Rollover-Text angezeigt werden soll, und Zeiten für die Aktualisierung der Informationen planen.
* Das Dialogfeld „Metadaten importieren“ (das über die Ansicht „Seiten zuordnen“ aufgerufen wird) ermöglicht den Import einer durch Tabulatoren getrennten TXT-Datei mit den Rollover-Textinformationen. Sie können diese TXT-Option für das Bedienfeld „Daten-Feed“ mit der CSV-Datei-Option für Ihren Rollover-Text verwenden.
* Die Seitenansicht „Zuordnen“ bietet eine Option für die Vorschau des XML-Codes, der für bestimmte Imagemaps angezeigt wird.

## Einrichten einer Antwortvorlage für E-Kataloge {#set-up-a-response-template-for-ecatalogs}

Sie können eine von drei vorgegebenen Antwortvorlagen für die Anzeige von Text in einem Infofeld auswählen. Diese vorgegebenen Antwortvorlagen bestimmen, wie Ihre Informationen im Infofeld dargestellt werden: Anzahl der Spalten und Zeilen, Schriftbild, Größe, Schriftart usw. Sie können eine voreingestellte Antwortvorlage auswählen oder eine eigene erstellen.

>[!NOTE]
>
>Sie können die Antwortvorlage auch in der Viewer-Vorgabe einrichten. Um stattdessen die Antwortvorlage in der Viewer-Vorgabe zu verwenden, fügen Sie am Ende der Informationsserver-URL in der Viewer-Vorgabe `fmt=1` hinzu.
>
>Siehe [Einrichten von E-Katalog-Viewer-Vorgaben](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. Doppelklicken Sie auf Ihren E-Katalog, damit er in der Detailansicht geöffnet wird.
1. Wählen Sie das Bedienfeld **[!UICONTROL InfoPanel-]**) aus.
1. Wählen Sie eine Antwortvorlage aus:

   * Wählen Sie eine Vorgabe aus dem Menü „Antwortvorlage“ aus. Der XML-Code für den Vorlagenentwurf wird im Feld „Benutzervorlage“ angezeigt.
   * Um Ihre eigene Antwortvorlage zu erstellen, wählen Sie **[!UICONTROL Benutzerdefiniert]** aus. Geben Sie die XML-Definition der Vorlage in das Feld „Benutzervorlage“ ein. Sie können die vorgegebenen Vorlagen als Grundlage für Ihre eigenen verwenden. 

1. (Optional) Geben Sie in das Feld „Standardantwort“ den Text ein, der angezeigt werden soll, wenn Adobe Dynamic Media Classic beim Abrufen von Informationen für eine Imagemap auf einen Fehler stößt. Wenn das System beispielsweise einen Firmennamen und einen E-Katalog-Namen, jedoch keinen Rollover-Bezeichner empfängt, so wird dem Benutzer diese Meldung angezeigt.
1. Geben Sie die Anzahl der Stunden bis zum Zwischenspeichern der Daten in das Feld „Antwort-TTL“ ein:

   * Geben Sie eine niedrigere Zahl ein, wenn die Daten im Verlauf des Tages häufig aktualisiert werden.
   * Legen Sie eine höhere Anzahl fest, wenn die Daten relativ stabil sind und nicht häufig über den Tag aktualisiert werden müssen. Der Standardwert lautet zehn Stunden.

1. Wählen Sie **[!UICONTROL Veröffentlichen]** aus.

## Importieren von Quellinhalten für das Infobedienfeld in E-Kataloge {#import-source-content-for-the-info-panel-in-ecatalogs}

Sie können eine kommagetrennte (CSV) oder tabulatorgetrennte (TXT) Datei für den Quelltext des Infofelds für einen E-Katalog verwenden. Tabulatorgetrennte Dateien müssen die UTF16-Kodierung (Unicode) verwenden. Sie können die verschiedenen Dateitypen mit verschiedenen Methoden importieren.

Beachten Sie beim Formatieren von Quellinhalt die folgenden Richtlinien:

* Stellen Sie sicher, dass die tabulator- und kommagetrennten Daten so viele Spalten enthalten, wie für die Rollover-Vorlage benötigt werden.
* Stellen Sie sicher, dass das erste Datenelement oder die erste Datenspalte die Rollover-Kennung ist (die mit dem Wert rollover_key aus den Imagemap-URLs verknüpft ist).
* Stellen Sie sicher, dass jedes durch Tabulatoren oder Kommas getrennte Element nach der Kennung das Element ist, das Sie in die Antwortvorlage ersetzen möchten. Die erste Spalte wird also durch $1$ ersetzt, die zweite Spalte durch $2$ usw.

### CSV-Inhalt von einem extern gehosteten Speicherort in E-Kataloge importieren {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. Doppelklicken Sie auf den E-Katalog, damit er in der Detailansicht geöffnet wird.
1. Wählen Sie das Bedienfeld **[!UICONTROL InfoPanel-Daten-Feed]** aus.
1. Geben Sie die URL für die CSV-Datei in das Feld „Speicherort der extern gehosteten CSV-Datei (HTTP)“ ein. Sie können diese URL in das Feld kopieren oder sie direkt eintippen.
1. (Optional) Geben Sie über das Menü Aktualisierung planen einen Zeitpunkt für die Aktualisierung des Inhalts an und wählen Sie **[!UICONTROL Hinzufügen]**. Sie können mehrere Zeitpunkte für die Aktualisierung auswählen. Jede Aktualisierungszeit wird im Feld „Zeiten aktualisieren“ angegeben. (Um eine Uhrzeit zu entfernen, wählen Sie sie aus und klicken Sie auf **[!UICONTROL Löschen]**.)
1. (Optional) Wählen Sie **[!UICONTROL Jetzt aktualisieren]** aus, damit Sie den Inhalt sofort aktualisieren können.

### Importieren einer tabulatorgetrennten oder CSV-Datei {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. Doppelklicken Sie auf den E-Katalog, damit er in der Detailansicht geöffnet wird.
1. Wählen Sie das Bedienfeld **[!UICONTROL InfoPanel-]**) aus.
1. Wählen **[!UICONTROL s7info-Inhalt hochladen]** aus.
1. Wählen Sie **[!UICONTROL Durchsuchen]**, wählen Sie die durch Tabulatoren getrennte TXT-Datei, CSV- oder SSV-Datei aus, die Sie verwenden möchten, und klicken Sie auf **[!UICONTROL Öffnen]**.
1. Wählen Sie **[!UICONTROL Hochladen]** aus.

Adobe Dynamic Media Classic sendet Ihnen eine E-Mail-Nachricht, die Sie darüber informiert, ob der Upload erfolgreich war oder nicht.

## Anzeigen der Vorschau für Rollover-Text für eine Imagemap {#preview-rollover-key-text-for-an-image-map}

Im Anzeigebereich „Imagemap-Seiten“ können Sie einfach und schnell den Infofeldtext für die Imagemaps auf einer bestimmten Seite Ihres E-Katalogs anzeigen.

1. Klicken Sie auf die Schaltfläche Rollover **[!UICONTROL Bearbeiten]** des Katalogs.
1. Wählen Sie **[!UICONTROL Seiten zuordnen]** aus.
1. Wählen Sie oben in der Tabelle rechts im Bildschirm im Menü „Anzeigen **[!UICONTROL die Option &quot;]**&quot;.

   Der Rollover-Text wird neben jeder Imagemap mit Infofeld-Text angezeigt.
