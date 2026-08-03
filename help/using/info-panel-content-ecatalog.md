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
autotag-review: '2026-05-13T19:51:12.585Z'
TQID: 'https://experienceleague.adobe.com/KZEo-DNrfZJt66xzSAHpLX6A8j1evxOBtwSxQfk44Wc'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: a6556d91057da7b0cd02523a48f97e2eadcebb88
workflow-type: tm+mt
source-wordcount: 889
ht-degree: 26%

---

# Verwalten von Inhalten des Infobereichs in E-Katalogen{#managing-info-panel-content-in-ecatalogs}

Sie können den Imagemap-Text für Ihre Rollover in E-Katalogen verwenden. Darüber hinaus besteht jedoch auch die Möglichkeit, anhand eines Infofelds größere Mengen von Rollover-Text, einschließlich Links, hinzuzufügen. Sie können das Infobedienfeld auch verwalten, indem Sie die zeitgesteuerte Zwischenspeicherung verwenden und Inhaltsaktualisierungen planen.

Sie können die Einrichtung und die Daten des Info-Panels mit den folgenden Funktionen in Adobe Dynamic Media Classic verwalten:

* Im Bedienfeld „InfoPanel-Einrichtung“ können Sie die Vorlage für die Anzeige des Textes im InfoPanel, eine Standardantwort bei Fehlern und die Anzahl der Stunden, in denen die Informationen zwischengespeichert werden, angeben. Darüber hinaus können Sie festlegen, ob die E-Kataloge automatisch veröffentlicht werden sollen.
* Im Bedienfeld „Info-Bedienfeld“ für den Daten-Feed können Sie eine CSV-Datei angeben. Diese Datei enthält den Text, der im Rollover-Text des Infobereichs angezeigt werden soll. Sie können auch Zeiten für die Aktualisierung der Informationen planen.
* Das Dialogfeld „Metadaten importieren“ (das über die Ansicht „Seiten zuordnen“ aufgerufen wird) ermöglicht den Import einer durch Tabulatoren getrennten TXT-Datei mit den Rollover-Textinformationen. Sie können diese TXT-Option für das Bedienfeld „Daten-Feed“ mit der CSV-Datei-Option für Ihren Rollover-Text verwenden.
* Die Seitenansicht „Zuordnen“ bietet eine Option für die Vorschau des XML-Codes, der für bestimmte Imagemaps angezeigt wird.

## Einrichten einer Antwortvorlage für E-Kataloge {#set-up-a-response-template-for-ecatalogs}

Sie können eine von drei voreingestellten Antwortvorlagen zur Anzeige von Text in einem Informationsbereich auswählen. Diese voreingestellten Antwortvorlagen bestimmen, wie Ihre Informationen im Infobereich angezeigt werden: Anzahl der Spalten und Zeilen, Schriftgröße, Schriftart und andere Einstellungen. Sie können eine voreingestellte Antwortvorlage auswählen oder eine eigene erstellen.

>[!NOTE]
>
>Sie können die Antwortvorlage auch in der Viewer-Vorgabe einrichten. Um stattdessen die Antwortvorlage in der Viewer-Vorgabe zu verwenden, fügen Sie am Ende der Informationsserver-URL in der Viewer-Vorgabe `fmt=1` hinzu.
>
>Siehe [Einrichten von E-Katalog-Viewer-Vorgaben](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. Doppelklicken Sie auf Ihren E-Katalog, damit er in der Detailansicht geöffnet wird.
1. Wählen Sie das Bedienfeld **[!UICONTROL InfoPanel-]**) aus.
1. Wählen Sie eine Antwortvorlage aus:

   * Wählen Sie eine Vorgabe aus dem Menü „Antwortvorlage“ aus. Der XML-Code für den Vorlagenentwurf wird im Feld „Benutzervorlage“ angezeigt.
   * Um Ihre eigene Antwortvorlage zu erstellen, wählen Sie **[!UICONTROL Benutzerdefiniert]** aus. Geben Sie die XML-Definition der Vorlage in das Feld „Benutzervorlage“ ein. Sie können die voreingestellten Vorlagen als Ausgangspunkt für Ihre eigenen verwenden.

1. (Optional) Geben Sie in das Feld „Standardantwort“ den Text ein, der angezeigt werden soll, wenn Adobe Dynamic Media Classic beim Abrufen von Informationen für eine Imagemap auf einen Fehler stößt. Wenn das System beispielsweise einen Firmen- und E-Katalog-Namen, aber keine Rollover-Kennung erhält, wird diese Meldung für den Benutzer angezeigt.
1. Geben Sie die Anzahl der Stunden bis zum Zwischenspeichern der Daten in das Feld „Antwort-TTL“ ein:

   * Legen Sie eine niedrigere Zahl fest, wenn die Daten häufig während des Tages aktualisiert werden.
   * Legen Sie eine höhere Zahl fest, wenn die Daten relativ stabil sind und während des Tages keine häufigen Aktualisierungen erfordern. Der Standardwert lautet zehn Stunden.

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

Adobe Dynamic Media Classic sendet Ihnen eine E-Mail-Nachricht, die Sie darüber informiert, ob der Upload erfolgreich war.

## Anzeigen der Vorschau für Rollover-Text für eine Imagemap {#preview-rollover-key-text-for-an-image-map}

Auf dem Bildschirm Seiten zuordnen können Sie den Text des Infobereichs für die Imagemaps auf einer bestimmten Seite Ihres E-Katalogs anzeigen.

1. Wählen Sie die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** des Katalogs aus.
1. Wählen Sie **[!UICONTROL Seiten zuordnen]** aus.
1. Wählen Sie oben in der Tabelle rechts im Bildschirm im Menü „Anzeigen **[!UICONTROL die Option &quot;]**&quot;.

   Der Rollover-Text wird neben jeder Imagemap mit Infofeld-Text angezeigt.
