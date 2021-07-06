---
title: Erstellen eines E-Katalogs
description: Erfahren Sie, wie Sie einen eCatalog erstellen.
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 79%

---

# Erstellen eines E-Katalogs{#creating-an-ecatalog}

Zum Erstellen eines E-Katalogs müssen die Seiten geordnet, das Seitenlayout ausgewählt und die Seiten durch Zeichnen von Imagemaps und Eingabe von Rollover- und Hypertext-Verknüpfungsdaten verknüpft werden. Optional können Sie das Inhaltsverzeichnis so anpassen, dass die Betrachter der Website anstelle von Seitenzahlen individuelle Seitennamen im E-Katalog-Viewer sehen.

## Erstellen eines E-Katalogs {#create}

Sie können Bilddateien und PDF-Dateien in Ihren E-Katalog aufnehmen.

Wenn Sie einen E-Katalog erstellen, wirkt sich die Option **Nach dem Speichern veröffentlichen** wie folgt auf das Set und die Set-Mitglieder aus:

| Option „Nach dem Speichern veröffentlichen“ vor dem Speichern ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |
| Ja | Veröffentlicht | Veröffentlicht |
| Nein | Unveröffentlicht | Mitglieder behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So erstellen Sie einen E-Katalog**

1. Wählen Sie zu Beginn der Erstellung eines E-Katalogs eine der folgenden Vorgehensweisen:

   * **Wählen Sie zuerst**  die Dateien aus - Wählen Sie im Durchsuchenbedienfeld die gewünschten Dateien aus und klicken Sie dann auf  **[!UICONTROL Erstellen]**  >  **[!UICONTROL E-Kataloge]**.

   * **Starten Sie im eCatalog-Bildschirm**  - Klicken Sie auf  **[!UICONTROL Erstellen]**  >  **[!UICONTROL E-Kataloge]**. Wählen Sie in der Asset-Bibliothek einen Ordner aus und ziehen Sie die gewünschten Dateien dann aus dem Ordner auf die Registerkarte „Seiten ordnen“ der Seite „E-Katalog“.

      >[!NOTE]
      >
      >Um die Elemente in der Asset-Bibliothek als Liste der Namen anzuzeigen statt als Miniaturansichten, wählen Sie unter „Persönliche Einstellungen“ als Standardansicht für die Asset-Bibliothek die Option „Name“ aus.

1. Wählen Sie ein Gesamtlayout für den E-Katalog aus. Klicken Sie für Einzelseiten auf „1-fach“ , für doppelseitige Druckbögen auf „2-fach“  oder für Druckbögen mit mehr als zwei Seiten auf „Benutzerdefiniert“ . Das Dialogfeld „E-Katalog-Layout ändern“ wird angezeigt. Wählen Sie die Optionen Alle Spreads aus und klicken Sie auf **[!UICONTROL OK]**.
1. Optional können Sie das Layout einzelner Seiten oder Seitenaufteilungen ändern, indem Sie darauf klicken und dann **[!UICONTROL 1 Up]**, **[!UICONTROL 2 Up]** oder **[!UICONTROL Custom]** auswählen. Das Dialogfeld „E-Katalog-Layout ändern“ wird angezeigt. Wählen Sie die Optionen Ausgewählte Druckbögen aus und klicken Sie auf **[!UICONTROL OK]**.
1. Ordnen Sie die Seiten mit einem der folgenden Verfahren nach Bedarf neu an:

   * **Ziehen**  - Ziehen Sie eine Seite oder einen Seitenstrich an eine neue Position. Die vertikale Leiste zeigt an, wohin die Seite verschoben wird.

   * **Schaltfläche &quot;Verschieben nach&quot;** : Wählen Sie eine Seite oder einen Seitenstrich aus, klicken Sie auf &quot; **[!UICONTROL Verschieben nach]**&quot;und wählen Sie im Menü die Seite aus, vor der die Seite erscheinen soll.

   * **Sequenz #**  - Geben Sie in der Listenansicht Seitenzahlen in die Felder Sequenz # ein.

1. Wenn Sie fertig sind, stellen Sie sicher, dass rechts unten auf der Seite die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** ausgewählt ist (Standard).
1. Klicken Sie auf **[!UICONTROL Speichern]**.
1. Wählen Sie im Dialogfeld „Speichern“ einen Ordner aus, in dem der E-Katalog gespeichert werden soll. Geben Sie in das Feld „Dateiname“ den Namen des Rotationssets ein.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Nach dem Speichern können Sie eine Vorschau des E-Katalogs anzeigen, indem Sie auf **[!UICONTROL Vorschau]** klicken.

## Bearbeiten eines E-Katalogs {#editing-an-ecatalog}

Abhängig davon, ob Sie ein veröffentlichtes oder unveröffentlichtes Set bearbeiten, wirkt sich die Option **[!UICONTROL Nach dem Speichern veröffentlichen]** wie folgt auf das Set und die Set-Mitglieder aus:

| Set bereits veröffentlicht? | Option „Nach dem Speichern veröffentlichen“ vor dem Speichern Ihrer Bearbeitungen ausgewählt? | Status des Sets nach dem Speichern | Status der Set-Mitglieder nach dem Speichern |
|--- |--- |--- |--- |
| Ja | Ja | Veröffentlicht | Veröffentlicht |
| Ja | Nein | Veröffentlicht | Vorhandene Set-Mitglieder behalten den Status „veröffentlicht“ bei. Alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |
| Nein | Ja | Veröffentlicht | Veröffentlicht |
| Nein | Nein | Unveröffentlicht | Vorhandene Set-Mitglieder und alle neuen Set-Mitglieder, die Sie während der Bearbeitung hinzugefügt haben, behalten ihren Status „veröffentlicht“ oder „unveröffentlicht“ bei. |

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So bearbeiten Sie einen E-Katalog:**

1. Klicken Sie auf die Rollover-Schaltfläche **[!UICONTROL Bearbeiten]** des E-Katalogs.
1. Nehmen Sie die erforderlichen Änderungen vor.
1. Wenn Sie die Bearbeitung abgeschlossen haben, stellen Sie sicher, dass rechts unten auf der Seite die Option **Nach dem Speichern veröffentlichen** ausgewählt ist (Standard).
1. Klicken Sie auf **Speichern**, wählen Sie einen Speicherordner aus, geben Sie einen Namen für das Set ein und klicken Sie dann auf **Speichern**.

## Löschen eines E-Katalogs {#deleting-an-ecatalog}

Wenn Sie ein Set löschen, wird das Set in den Papierkorb verschoben. Die Mitglieder (bzw. die untergeordneten Elemente) innerhalb des Sets sind davon jedoch nicht betroffen; sie behalten ihren jeweiligen Status „veröffentlicht“ oder „unveröffentlicht“ bei.

Siehe auch [Manuelles Veröffentlichen von Assets](publishing-files.md#manually_publishing_assets) und [Manuelles Rückgängigmachen der Veröffentlichung von Assets](publishing-files.md#manually_unpublishing_assets).

**So löschen Sie einen E-Katalog**

1. Wählen Sie in der Rasteransicht, Listenansicht oder Detailansicht einen oder mehrere E-Kataloge aus.
1. Klicken Sie in der globalen Navigationsleiste auf **Datei** > **Löschen** > **Löschen**.

## Anpassen des Inhaltsverzeichnisses {#customizing-the-table-of-contents-toc}

Dynamic Media Classic stellt in Ihrem E-Katalog auf der Registerkarte &quot;Seiten bestellen&quot;des E-Katalog-Bildschirms die standardmäßigen Seitenzahlen bereit. Um benutzerdefinierte Seitennamen zu verwenden, können Sie die Seitenbeschriftungen ändern, aus denen das Inhaltsverzeichnis erstellt wird. Eine Umbenennung der Vorder- und Rückseite wird empfohlen. Beispielsweise kann die Titelseite &quot;Cover&quot;anstelle von &quot;Page 0-1&quot;lauten.

Sie können ein angepasstes Inhaltsverzeichnis für den E-Katalog erstellen: entweder manuell oder durch das Importieren der Seitennamen aus einer CSV- (nur Mac) oder XML-Datei.

>[!NOTE]
>
>Um die standardmäßigen Seitentitel wiederherzustellen, klicken Sie auf der Registerkarte „Seiten ordnen“ auf „Inhaltsverz.“ und wählen Sie „Standardw. wiederherstellen (alle)“.

### Manuelles Eingeben von Seitennamen {#manually-entering-page-names}

Um Seitennamen einzeln von Hand einzugeben, rufen Sie im Anzeigebereich „E-Katalog“ die Registerkarte „Seiten ordnen“ auf. Klicken Sie dann in das Seitenzahlenfeld und geben Sie einen Namen ein. Geben Sie für alle Seiten, deren Namen Sie festlegen möchten, einen Namen ein.

### Importieren von Seitennamen {#importing-page-names}

Das Importieren von Seitennamen wird für einen E-Katalog mit sehr vielen Seiten empfohlen. Sie haben die Möglichkeit, die Namen aus einer tabulatorgetrennten Datei oder einer XML-Datei zu importieren.

Die Bezeichnung des Inhaltsverzeichnisses wird im Feld &quot;Benutzerdaten&quot;eines Bildes gespeichert. diese Daten als Liste von `name=<value>` ` pairs separated by two question marks “??” ` formatieren. Um beispielsweise eine Beschriftung für ein Inhaltsverzeichnisfeld mit dem Namen `tocEN` festzulegen, setzen Sie im Feld „Benutzerdaten“ des Bilds folgenden Wert:

`tocEN=&lt;EN_page_label>`

So legen Sie separate Beschriftungen für TOC-Felder mit den Namen `tocEN` und `tocFR` fest:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

Um das Feld &quot;Benutzerdaten&quot;in eine tabulatorgetrennte Datei zu importieren, fügen Sie die Benutzerdaten des Felds ein:

| IPSID | Benutzerdaten |
|--- |--- |
| `<image_IPS_ID>` | tocEN=&lt;EN_Seitenbeschriftung>??tocFR=&lt;FR_Seitenbeschriftung> |

Um das Feld „Benutzerdaten“ in eine XML-Datei zu importieren, fügen Sie das Attribut `vc_userdata` ein:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

Um Seitennamen aus einer tabulatorgetrennten Datei oder XML-Datei zu importieren, klicken Sie auf „Inhaltsverz.“ und wählen Sie die Option „Importieren“. Das Dialogfeld „Metadaten hochladen“ wird angezeigt. Klicken Sie auf „Durchsuchen“ und importieren Sie die CSV- (nur Mac) oder XML-Datei, die jeder Seite einen Seitennamen zuordnet. 
