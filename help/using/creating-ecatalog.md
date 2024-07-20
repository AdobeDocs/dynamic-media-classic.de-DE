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
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 30%

---

# Erstellen eines E-Katalogs {#creating-an-ecatalog}

Das Erstellen eines E-Katalogs umfasst das Sortieren der Seiten, das Auswählen des Seitenlayouts und das Verknüpfen der Seiten durch Zeichnen von Imagemaps. Außerdem müssen Rollover- und Hypertext-Link-Daten eingegeben werden. Optional können Sie das Inhaltsverzeichnis so anpassen, dass die Betrachter der Website anstelle von Seitenzahlen individuelle Seitennamen im E-Katalog-Viewer sehen.

## Erstellen eines eCatalog {#create}

Sie können Bilddateien und PDF-Dateien in Ihren eCatalog aufnehmen.

Wenn Sie einen E-Katalog erstellen, wirkt sich die Option **[!UICONTROL Publish nach dem Speichern]** wie folgt auf das Set und die Set-Mitglieder aus:

| Vor dem Speichern die Option &quot;Publish nach dem Speichern&quot;ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie einen eCatalog:**

1. Wählen Sie zu Beginn der Erstellung eines E-Katalogs eine der folgenden Vorgehensweisen:

   * **Wählen Sie zuerst die Dateien aus**: Wählen Sie im Bedienfeld &quot;Durchsuchen&quot;die Dateien aus und gehen Sie dann zu &quot;**[!UICONTROL Build]**&quot;> &quot;**[!UICONTROL eCatalog]**&quot;.

   * **Vom E-Katalog-Bildschirm starten**: Wechseln Sie zu &quot;**[!UICONTROL Build]**&quot;> &quot;**[!UICONTROL eCatalog]**&quot;. Wählen Sie einen Ordner in der Asset-Bibliothek aus. Ziehen Sie Dateien aus dem Ordner in die Registerkarte &quot;Seiten ordnen&quot;der eCatalog-Seite.

     >[!NOTE]
     >
     >Um die Elemente in der Asset-Bibliothek als Liste der Namen anzuzeigen statt als Miniaturansichten, wählen Sie unter „Persönliche Einstellungen“ als Standardansicht für die Asset-Bibliothek die Option „Name“ aus.

1. Wählen Sie ein Gesamtlayout für den E-Katalog aus. Wählen Sie **[!UICONTROL 1 Aufwärts]** für einzelne Seiten, **[!UICONTROL 2 Aufwärts]** für doppelseitige Druckbögen oder **[!UICONTROL Benutzerdefiniert]** für Seitenaufteilungen mit mehr als zwei Seiten. Wählen Sie im Dialogfeld **[!UICONTROL E-Katalog-Layout ändern]** die Optionen **[!UICONTROL Alle Druckbögen]** und dann **[!UICONTROL OK]** aus.
1. Optional können Sie das Layout einzelner Seiten oder Seitenaufteilungen ändern, indem Sie sie auswählen und dann die Schaltfläche **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]** oder **[!UICONTROL Custom]** auswählen. Wählen Sie im Dialogfeld **[!UICONTROL E-Katalog-Layout ändern]** die Optionen **[!UICONTROL Ausgewählte Druckbögen]** und danach **[!UICONTROL OK]** aus.
1. Ordnen Sie die Seiten mit einem der folgenden Verfahren nach Bedarf neu an:

   * **Ziehen**: Ziehen Sie eine Seite oder einen Seitenstrich an eine neue Position. Die vertikale Leiste zeigt an, wohin die Seite verschoben wird.

   * **Schaltfläche &quot;Verschieben nach&quot;**: Wählen Sie eine Seite oder einen Seitenstrich aus, klicken Sie auf **[!UICONTROL Verschieben nach]** und wählen Sie die Seite im Menü aus, vor der die Seite angezeigt werden soll.

   * **Sequenz #**: Geben Sie in der Listenansicht Seitenzahlen in die Felder der Sequenz # ein.

1. Wenn Sie fertig sind, stellen Sie sicher, dass rechts unten auf der Seite **[!UICONTROL Publish nach einem Speichern]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]** aus.
1. Wählen Sie im Dialogfeld „Speichern“ einen Ordner aus, in dem der E-Katalog gespeichert werden soll. Geben Sie im Feld Dateiname den Namen des Rotationssets ein.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

   Nachdem Sie den E-Katalog gespeichert haben, können Sie eine Vorschau des E-Katalogs anzeigen, indem Sie **[!UICONTROL Vorschau]** auswählen.

## Bearbeiten eines E-Katalogs {#editing-an-ecatalog}

Unabhängig davon, ob Sie einen veröffentlichten oder einen nicht veröffentlichten Satz bearbeiten, wirkt sich die Option **[!UICONTROL Publish nach dem Speichern]** wie folgt auf das Set und die Setmitglieder aus:

| Set bereits veröffentlicht? | Option &quot;Publish nach dem Speichern&quot;vor dem Speichern der Bearbeitung ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren Veröffentlichungsstatus bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie einen eCatalog:**

1. Wählen Sie die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** des E-Katalogs aus.
1. Nehmen Sie die erforderlichen Änderungen vor.
1. Wenn Sie die Bearbeitung abgeschlossen haben, stellen Sie sicher, dass rechts unten auf der Seite **[!UICONTROL Publish nach dem Speichern]** ausgewählt ist (Standard).
1. Wählen Sie &quot;**[!UICONTROL Speichern]**&quot;, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und wählen Sie dann &quot;**[!UICONTROL Speichern]**&quot;.

## Löschen eines eCatalog

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (oder &quot;untergeordneten Elemente&quot;) in diesem Satz sind jedoch nicht betroffen. Stattdessen behalten sie ihren vorhandenen Status veröffentlicht oder unveröffentlicht bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie einen eCatalog:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht einen oder mehrere E-Kataloge aus.
1. Wechseln Sie in der Leiste &quot;Globale Navigation&quot;zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.

## Anpassen des Inhaltsverzeichnisses {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic stellt in Ihrem E-Katalog auf der Registerkarte &quot;Seiten bestellen&quot;des E-Katalog-Bildschirms die standardmäßigen Seitenzahlen bereit. Um benutzerdefinierte Seitennamen zu verwenden, können Sie die Seitenbeschriftungen ändern, aus denen das Inhaltsverzeichnis erstellt wird. Eine Umbenennung der Vorder- und Rückseite wird empfohlen. Beispielsweise kann die Titelseite &quot;Cover&quot;anstelle von &quot;Page 0-1&quot;lauten.

Sie können ein benutzerdefiniertes Inhaltsverzeichnis (TOC) für Ihren eCatalog manuell erstellen. Sie können die Seitennamen auch aus einer CSV- (nur Mac) oder einer XML-Datei importieren.

>[!NOTE]
>
>Um die standardmäßigen Seitentitel wiederherzustellen, wählen Sie auf der Registerkarte **[!UICONTROL Seiten sortieren]** die Option **[!UICONTROL TOC-Beschriftungen]** und klicken Sie dann auf **[!UICONTROL Standardangaben wiederherstellen (Alle)]**.

### Manuelles Eingeben von Seitennamen {#manually-entering-page-names}

Geben Sie Seitennamen einzeln manuell ein, indem Sie im E-Katalog-Bildschirm auf die Registerkarte &quot;Seiten sortieren&quot;gehen. Geben Sie dann im Feld &quot;Seitenzahl&quot;einen Namen für jede Seite ein, die Sie benennen möchten.

### Importieren von Seitennamen {#importing-page-names}

Das Importieren von Seitennamen wird für einen E-Katalog mit sehr vielen Seiten empfohlen. Sie haben die Möglichkeit, die Namen aus einer tabulatorgetrennten Datei oder einer XML-Datei zu importieren.

Die Beschriftung des Inhaltsverzeichnisses wird im Feld &quot;Benutzerdaten&quot;eines Bildes gespeichert. Formatieren Sie diese Daten als Liste von `name=<value>` ` pairs separated by two question marks "??" `. Um beispielsweise eine Beschriftung für ein TOC-Feld mit dem Namen `tocEN` festzulegen, setzen Sie die Benutzerdaten des Bildes auf:

`tocEN=&lt;EN_page_label>`

So legen Sie separate Beschriftungen für TOC-Felder mit den Namen `tocEN` und `tocFR` fest:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

Um das Feld &quot;Benutzerdaten&quot;in eine tabulatorgetrennte Datei zu importieren, fügen Sie die Benutzerdaten des Felds ein:

| IPSID | Benutzerdaten |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

Um das Feld &quot;Benutzerdaten&quot;in eine XML-Datei zu importieren, fügen Sie das Attribut `vc_userdata` hinzu:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Um Seitennamen aus einer tabulatorgetrennten oder XML-Datei zu importieren, wählen Sie die Schaltfläche **[!UICONTROL TOC-Beschriftungen]** und danach **[!UICONTROL Importieren]** aus. Wählen Sie im Dialogfeld &quot;Metadaten hochladen&quot;die Option **[!UICONTROL Durchsuchen]** und importieren Sie dann die CSV-Datei (nur Mac) oder die XML-Datei, die jeder Seite einen Seitennamen zuordnet.
