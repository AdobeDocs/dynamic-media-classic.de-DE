---
title: E-Katalog erstellen
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic einen E-Katalog erstellen.
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

Das Erstellen eines E-Katalogs umfasst das Sortieren der Seiten, das Auswählen des Seiten-Layouts und das Verknüpfen der Seiten durch Zeichnen von Imagemaps. Außerdem ist die Eingabe von Rollover- und Hypertext-Linkdaten erforderlich. Optional können Sie das Inhaltsverzeichnis so anpassen, dass die Betrachter der Website anstelle von Seitenzahlen individuelle Seitennamen im E-Katalog-Viewer sehen.

## E-Katalog erstellen {#create}

Sie können Bilddateien und PDF-Dateien in Ihren E-Katalog aufnehmen.

Beim Erstellen eines E-Katalogs wirkt sich die Option **[!UICONTROL Publish nach dem Speichern]** auf die Mitglieder des Sets und des Sets wie folgt aus:

| Vor dem Speichern die Option &quot;Publish nach dem Speichern“ ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie einen E-Katalog:**

1. Wählen Sie zu Beginn der Erstellung eines E-Katalogs eine der folgenden Vorgehensweisen:

   * **Zuerst die Dateien auswählen**: Wählen Sie im Durchsuchen-Bereich die Option Dateien aus und navigieren Sie dann zu **[!UICONTROL Erstellen]** > **[!UICONTROL eCatalogs]**.

   * **Vom E-Katalog-Bildschirm starten**: Gehen Sie zu **[!UICONTROL Erstellen]** > **[!UICONTROL E-Kataloge]**. Wählen Sie einen Ordner in der Asset-Bibliothek aus. Ziehen Sie Dateien aus dem Ordner auf die Registerkarte Seiten sortieren der Seite eCatalog .

     >[!NOTE]
     >
     >Um die Elemente in der Asset-Bibliothek als Liste der Namen anzuzeigen statt als Miniaturansichten, wählen Sie unter „Persönliche Einstellungen“ als Standardansicht für die Asset-Bibliothek die Option „Name“ aus.

1. Wählen Sie ein Gesamtlayout für den E-Katalog aus. Wählen Sie **[!UICONTROL 1 oben]** für einzelne Seiten, **[!UICONTROL 2 oben]** für doppelseitige Spreads oder **[!UICONTROL Benutzerdefiniert]** für Seitenspreads mit mehr als zwei Seiten aus. Wählen **[!UICONTROL Dialogfeld E-Katalog-Layout ändern]** die Optionen **[!UICONTROL Alle Spreads]** aus und klicken Sie auf **[!UICONTROL OK]**.
1. Optional können Sie das Layout einzelner Seiten oder Seiten-Spreads ändern, indem Sie sie auswählen und dann die Schaltfläche **[!UICONTROL 1 Nach oben]**, **[!UICONTROL 2 Nach oben]** oder **[!UICONTROL Benutzerdefiniert]** auswählen. Wählen **[!UICONTROL Dialogfeld E-Katalog-Layout ändern]** die Optionen **[!UICONTROL Ausgewählte Spreads]** aus und klicken Sie auf **[!UICONTROL OK]**.
1. Ordnen Sie die Seiten mit einem der folgenden Verfahren nach Bedarf neu an:

   * **Ziehen**: Ziehen Sie eine Seite oder einen Seitenbereich an eine neue Position. Die vertikale Leiste zeigt an, wohin die Seite verschoben wird.

   * **Schaltfläche „Verschieben nach**: Wählen Sie eine Seite oder Seitenübersicht aus, wählen Sie **[!UICONTROL Verschieben nach]** und wählen Sie im Menü die Seite aus, vor der Ihre Seite angezeigt werden soll.

   * **Sequenz Nr.**: Geben Sie in der Listenansicht die Seitenzahlen in die Felder der Sequenz Nr. ein.

1. Wenn Sie fertig sind, stellen Sie sicher, dass **[!UICONTROL Publish nach dem Speichern]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]** aus.
1. Wählen Sie im Dialogfeld „Speichern“ einen Ordner aus, in dem der E-Katalog gespeichert werden soll. Geben Sie im Feld Dateiname den Namen des Rotationssets ein.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

   Sie können Ihren E-Katalog nach dem Speichern in der Vorschau anzeigen, indem Sie **[!UICONTROL Vorschau]** auswählen.

## E-Katalog bearbeiten {#editing-an-ecatalog}

Unabhängig davon, ob Sie ein veröffentlichtes Set oder ein unveröffentlichtes Set bearbeiten, wirkt sich die Option **[!UICONTROL Publish nach dem Speichern]** auf die Mitglieder des Sets und des Sets wie folgt aus:

| Set bereits veröffentlicht? | Vor dem Speichern der Bearbeitung die Option &quot;Publish nach dem Speichern“ ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
| --- | --- | --- | --- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten ihren veröffentlichten Status bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie einen E-Katalog:**

1. Wählen Sie die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** des E-Katalogs aus.
1. Nehmen Sie die erforderlichen Änderungen vor.
1. Wenn Sie die Bearbeitung abgeschlossen haben, stellen Sie sicher, dass **[!UICONTROL Publish nach dem Speichern]** ausgewählt ist (Standard).
1. Wählen Sie **[!UICONTROL Speichern]**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **[!UICONTROL Speichern]**.

## E-Katalog löschen

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (oder „untergeordneten Elemente„) in diesem Set sind jedoch nicht betroffen. Stattdessen behalten sie jeweils ihren vorhandenen Status „Veröffentlicht“ oder „Unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie einen E-Katalog:**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht einen oder mehrere E-Kataloge aus.
1. Navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Datei]** > **[!UICONTROL Löschen]** > **[!UICONTROL Löschen]**.

## Anpassen des Inhaltsverzeichnisses {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic stellt die Standardseitennummern in Ihrem E-Katalog auf der Registerkarte Bestellseiten des E-Katalog-Bildschirms bereit. Um benutzerdefinierte Seitennamen zu verwenden, können Sie die Seitenbeschriftungen ändern, aus denen das Inhaltsverzeichnis erstellt wird. Eine Umbenennung der Vorder- und Rückseite wird empfohlen. Beispielsweise kann auf der Titelseite „Titelseite“ anstelle von „Seite 0-1“ stehen.

Sie können für Ihren E-Katalog manuell ein benutzerdefiniertes Inhaltsverzeichnis erstellen. Sie können die Seitennamen auch aus einer CSV- (nur Mac) oder XML-Datei importieren.

>[!NOTE]
>
>Um die Standardseitentitel wiederherzustellen, wählen Sie auf der Registerkarte **[!UICONTROL Bestellseiten]** die Option **[!UICONTROL Inhaltsverzeichnisbeschriftungen]** und dann **[!UICONTROL Standardeinstellungen wiederherstellen (Alle)]**.

### Manuelles Eingeben von Seitennamen {#manually-entering-page-names}

Geben Sie die Seitennamen einzeln manuell ein, indem Sie auf der Registerkarte Bestellseiten des Bildschirms E-Katalog zu navigieren. Geben Sie dann im Feld Seitennummer einen Namen für jede Seite ein, die Sie benennen möchten.

### Seitennamen importieren {#importing-page-names}

Das Importieren von Seitennamen wird für einen E-Katalog mit sehr vielen Seiten empfohlen. Sie haben die Möglichkeit, die Namen aus einer tabulatorgetrennten Datei oder einer XML-Datei zu importieren.

Das Inhaltsverzeichnis wird im Benutzerdatenfeld eines Bildes gespeichert. Formatieren Sie diese Daten als Liste `name=<value>` ` pairs separated by two question marks "??" `. Um beispielsweise eine Beschriftung für ein Inhaltsverzeichnisfeld festzulegen, das `tocEN` heißt, legen Sie für die Benutzerdaten des Bildes Folgendes fest:

`tocEN=&lt;EN_page_label>`

So legen Sie separate Beschriftungen für Inhaltsverzeichnisfelder mit den Namen `tocEN` und `tocFR` fest:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

Um das Benutzerdatenfeld in eine durch Tabulatoren getrennte Datei zu importieren, fügen Sie das Benutzerdatenfeld ein:

| IPSID | Benutzerdaten |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

Um das Benutzerdatenfeld in eine XML-Datei zu importieren, fügen Sie das `vc_userdata` ein:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Um Seitennamen aus einer tabulatorgetrennten oder XML-Datei zu importieren, klicken Sie auf die Schaltfläche **[!UICONTROL Inhaltsverzeichnisbeschriftungen]** und wählen Sie **[!UICONTROL Importieren]**. Wählen Sie im Dialogfeld Metadaten hochladen die Option **[!UICONTROL Durchsuchen]** aus und importieren Sie dann die CSV-Datei (nur Mac) oder XML-Datei, die jede Seite mit einem Seitennamen verknüpft.
