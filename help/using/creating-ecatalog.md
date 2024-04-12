---
title: Erstellen eines eCatalog
description: Erfahren Sie, wie Sie einen eCatalog in Adobe Dynamic Media Classic erstellen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
topic: Integrations, Development
level: Experienced
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 44%

---

# Erstellen eines E-Katalogs {#creating-an-ecatalog}

Zum Erstellen eines E-Katalogs müssen die Seiten geordnet, das Seitenlayout ausgewählt und die Seiten durch Zeichnen von Imagemaps und Eingabe von Rollover- und Hypertext-Verknüpfungsdaten verknüpft werden. Optional können Sie das Inhaltsverzeichnis so anpassen, dass die Betrachter der Website anstelle von Seitenzahlen individuelle Seitennamen im E-Katalog-Viewer sehen.

## Erstellen eines eCatalog {#create}

Sie können Bilddateien und PDF-Dateien in Ihren eCatalog aufnehmen.

Wenn Sie einen E-Katalog erstellen, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| Option &quot;Nach dem Speichern veröffentlichen&quot;vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie einen eCatalog:**

1. Wählen Sie zu Beginn der Erstellung eines E-Katalogs eine der folgenden Vorgehensweisen:

   * **Wählen Sie zuerst die Dateien aus** - Wählen Sie im Durchsuchen-Bedienfeld Dateien aus und navigieren Sie zu **[!UICONTROL Build]** > **[!UICONTROL E-Kataloge]**.

   * **Vom eCatalog-Bildschirm starten** - Gehen Sie zu **[!UICONTROL Build]** > **[!UICONTROL E-Kataloge]**. Wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die gewünschten Dateien dann aus dem Ordner auf die Registerkarte „Seiten ordnen“ der Seite „E-Katalog“.

     >[!NOTE]
     >
     >Um die Elemente in der Asset-Bibliothek als Liste der Namen anzuzeigen statt als Miniaturansichten, wählen Sie unter „Persönliche Einstellungen“ als Standardansicht für die Asset-Bibliothek die Option „Name“ aus.

1. Wählen Sie ein Gesamtlayout für den E-Katalog aus. Auswählen **[!UICONTROL 1 Up]** für einzelne Seiten, **[!UICONTROL 2 Up]** bei doppelseitigen Tabellen oder **[!UICONTROL Benutzerdefiniert]** für Seitenaufschläge von mehr als zwei Seiten. Im **[!UICONTROL Ändern des eCatalog-Layouts]** auswählen, wählen Sie das **[!UICONTROL Alle Spreads]** Optionen und wählen Sie **[!UICONTROL OK]**.
1. Optional können Sie das Layout einzelner Seiten oder Seitenaufteilungen ändern, indem Sie sie auswählen und dann **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]** oder **[!UICONTROL Benutzerdefiniert]** Schaltfläche. Im **[!UICONTROL Ändern des eCatalog-Layouts]** auswählen, wählen Sie das **[!UICONTROL Ausgewählte Spreads]** Optionen und wählen Sie **[!UICONTROL OK]**.
1. Ordnen Sie die Seiten mit einem der folgenden Verfahren nach Bedarf neu an:

   * **Ziehen** - Ziehen Sie eine Seite oder einen Seitenstrich an eine neue Position. Die vertikale Leiste zeigt an, wohin die Seite verschoben wird.

   * **Schaltfläche &quot;Verschieben nach&quot;** - Wählen Sie eine Seite oder einen Seitenversatz aus. **[!UICONTROL Verschieben nach]** und wählen Sie die Seite im Menü aus, die Ihre Seite vor der Seite erscheinen soll.

   * **Sequenz #** - Geben Sie in der Listenansicht Seitenzahlen in die Felder der Sequenz-Nr. ein.

1. Wenn Sie fertig sind, stellen Sie sicher, dass rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Auswählen **[!UICONTROL Speichern]**.
1. Wählen Sie im Dialogfeld „Speichern“ einen Ordner aus, in dem der E-Katalog gespeichert werden soll. Geben Sie in das Feld „Dateiname“ den Namen des Rotationssets ein.
1. Auswählen **[!UICONTROL Speichern]**.

   Nach dem Speichern können Sie eine Vorschau des E-Katalogs anzeigen, indem Sie **[!UICONTROL Vorschau]**.

## Bearbeiten eines E-Katalogs {#editing-an-ecatalog}

Unabhängig davon, ob Sie ein veröffentlichtes Set oder ein nicht veröffentlichtes Set bearbeiten, wird die **[!UICONTROL Nach dem Speichern veröffentlichen]** -Option wirkt sich auf die Set- und Set-Mitglieder wie folgt aus:

| Set bereits veröffentlicht? | Option &quot;Nach dem Speichern veröffentlichen&quot;vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren Veröffentlichungsstatus bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie einen eCatalog:**

1. Rollover des E-Katalogs auswählen **[!UICONTROL Bearbeiten]** Schaltfläche.
1. Nehmen Sie die erforderlichen Änderungen vor.
1. Wenn Sie die Bearbeitung abgeschlossen haben, stellen Sie sicher, dass rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Auswählen **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und wählen Sie dann **[!UICONTROL Speichern]**.

## Löschen eines eCatalog

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (oder &quot;untergeordneten Elemente&quot;) in diesem Satz sind jedoch nicht betroffen. Stattdessen behalten sie ihren vorhandenen Status veröffentlicht oder unveröffentlicht bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie einen eCatalog:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht einen oder mehrere E-Kataloge aus.
1. Wechseln Sie in der Leiste Globale Navigation zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.

## Anpassen des Inhaltsverzeichnisses {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic stellt in Ihrem E-Katalog auf der Registerkarte &quot;Seiten bestellen&quot;des E-Katalog-Bildschirms die standardmäßigen Seitenzahlen bereit. Um benutzerdefinierte Seitennamen zu verwenden, können Sie die Seitenbeschriftungen ändern, aus denen das Inhaltsverzeichnis erstellt wird. Eine Umbenennung der Vorder- und Rückseite wird empfohlen. Beispielsweise kann die Titelseite &quot;Cover&quot;anstelle von &quot;Page 0-1&quot;lauten.

Sie können ein benutzerdefiniertes Inhaltsverzeichnis (TOC) für Ihren eCatalog manuell erstellen oder die Seitennamen aus einer CSV- (nur Mac) oder XML-Datei importieren.

>[!NOTE]
>
>So stellen Sie die standardmäßigen Seitentitel im **[!UICONTROL Bestellseiten]** Registerkarte auswählen **[!UICONTROL Inhaltsbezeichnungen]** und wählen Sie **[!UICONTROL Standardangaben wiederherstellen (alle)]**.

### Manuelles Eingeben von Seitennamen {#manually-entering-page-names}

Um Seitennamen einzeln von Hand einzugeben, rufen Sie im Anzeigebereich „E-Katalog“ die Registerkarte „Seiten ordnen“ auf. Geben Sie dann im Feld &quot;Seitenzahl&quot;einen Namen für jede Seite ein, die Sie benennen möchten.

### Importieren von Seitennamen {#importing-page-names}

Das Importieren von Seitennamen wird für einen E-Katalog mit sehr vielen Seiten empfohlen. Sie haben die Möglichkeit, die Namen aus einer tabulatorgetrennten Datei oder einer XML-Datei zu importieren.

Der Titel des Inhaltsverzeichnisses wird im Feld Benutzerdaten eines Bildes gespeichert. Formatieren Sie diese Daten als Liste von `name=<value>` ` pairs separated by two question marks "??" `. So legen Sie beispielsweise eine Beschriftung für ein TOC-Feld fest, das `tocEN`festlegen, setzen Sie die Benutzerdaten des Bildes auf:

`tocEN=&lt;EN_page_label>`

So legen Sie separate Beschriftungen für TOC-Felder fest: `tocEN` und `tocFR`:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

Um das Feld &quot;Benutzerdaten&quot;in eine tabulatorgetrennte Datei zu importieren, fügen Sie die Benutzerdaten des Felds ein:

| IPSID | Benutzerdaten |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

Um das Feld &quot;Benutzerdaten&quot;in eine XML-Datei zu importieren, fügen Sie das Attribut hinzu `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Um Seitennamen aus einer tabulatorgetrennten Datei oder einer XML-Datei zu importieren, wählen Sie die **[!UICONTROL Inhaltsbezeichnungen]** Schaltfläche und wählen Sie **[!UICONTROL Import]**. Wählen Sie im Dialogfeld Metadaten hochladen die Option **[!UICONTROL Durchsuchen]** und importieren Sie dann die CSV-Datei (nur Mac) oder die XML-Datei, die jede Seite mit einem Seitennamen verknüpft.
