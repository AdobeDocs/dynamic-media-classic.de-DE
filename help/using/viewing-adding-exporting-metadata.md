---
title: Anzeigen, Hinzufügen und Exportieren von Metadaten
description: Erfahren Sie, wie Sie Metadaten in Adobe Dynamic Media Classic anzeigen, hinzufügen und exportieren.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Metadata
role: User
exl-id: 2be50cc7-9a8b-4f7b-8ebf-18a3208654f2
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '2225'
ht-degree: 34%

---

# Anzeigen, Hinzufügen und Exportieren von Metadaten{#viewing-adding-and-exporting-metadata}

Sie können Informationen speichern, die für die Dateien gelten, mit denen Sie in Adobe Dynamic Media Classic arbeiten. Diese Informationen werden als *Metadaten* bezeichnet. Sie können Metadaten in Adobe Dynamic Media Classic zum Organisieren, Suchen, Filtern und Sortieren Ihrer Assets verwenden.

Metadaten werden in der Detailansicht angezeigt. Sie wird zusammen mit Adobe Dynamic Media Classic-generierten Informationen angezeigt. Beispielsweise das Erstellungsdatum der Datei, das Veröffentlichungsdatum und Schlüsselwörter. Um Metadaten anzuzeigen, öffnen Sie das Asset in der Detailansicht und wählen Sie dann das Metadatenbedienfeld aus. Sie können Metadaten in der Detailansicht eingeben und bearbeiten.

Manche Metadaten sind direkt in eine Datei eingebettet. Wenn eine Datei diese Metadaten enthält, lädt Adobe Dynamic Media Classic sie automatisch mit der Datei hoch. Sie können Metadaten in Quell-Assets in Adobe Photoshop, InDesign, Illustrator und andere Anwendungen einbetten. Adobe Dynamic Media Classic erkennt diese Metadaten. Sie können auch einzelnen Dateien Metadaten im Metadatenbedienfeld in der Detailansicht hinzufügen. Damit die Einheitlichkeit Asset-übergreifend gewährleistet werden kann, können Unternehmensadministratoren Metadatenvorlagen mit den zu verwendenden Metadatenfeldern erstellen.

Weitere Informationen zu eingebetteten Metadaten finden Sie unter [Extensible Metadata Platform](https://www.adobe.com/products/xmp.html).

## Anzeigen von Metadaten {#view-metadata}

Um die Metadaten eines Assets anzuzeigen, öffnen Sie das Asset in der Detailansicht und tippen Sie auf das Metadatenbedienfeld. Um einen Satz von Metadatenfeldern auszuwählen, wählen Sie eine Option im Menü Metadatenansicht . Adobe Dynamic Media Classic bietet diese Metadaten-Ansichten:

* **Kompakte Ansicht**: Eine einfache Liste von Werten.

* **IPTC**: Werte gemäß der Definition des International Press Telecommunications Council.

* **XMP**: Werte, die vom erweiterbaren Metadatenprogramm definiert werden.

Administratoren können Metadaten-Ansichten erstellen. Diese Ansichten werden auch im Menü Metadaten-Ansichten angezeigt.

Informationen zum Erstellen von Metadaten-Ansichten finden Sie unter [Metadaten-Ansichten](application-setup.md#metadata_views) .

## Manuelles Eingeben von Metadaten für ein Asset {#manually-enter-metadata-for-an-asset}

1. Öffnen Sie das Asset in der Detailansicht.
1. Öffnen Sie das Metadatenbedienfeld und führen Sie einen oder beide der folgenden Schritte aus:

   * Wählen Sie die Metadatenansicht aus, um festzustellen, welche Metadatenfelder im Bedienfeld angezeigt werden.
   * Wählen Sie einen Vorgabewert und dann **[!UICONTROL Anwenden]** aus, um Metadatenfelder mit Vorgabewerten zu füllen. Diese Vorgabewerte werden von Unternehmensadministratoren erstellt.

1. Geben Sie die Werte im Metadatenbedienfeld ein.

>[!NOTE]
>
>Um die Metadaten mehrerer Assets gleichzeitig zu bearbeiten, wählen Sie die Assets aus und gehen Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Informationen bearbeiten]**. Die Änderungen, die Sie im Fenster &quot;Informationen bearbeiten&quot;an Metadaten vorgenommen haben, gelten für alle ausgewählten Assets.

## Hinzufügen oder Bearbeiten von Schlüsselwörtern {#add-or-edit-keywords}

Zusätzlich zu den Metadaten können Sie Keywords verwenden, um die Suche und Verwaltung Ihrer Assets zu unterstützen.

Wenn Sie während dieser Sitzung Suchbegriffe zu anderen Dateien hinzugefügt haben oder wenn Sie Suchbegriffe aus Ihrer Liste entfernt haben, werden diese in der Tabelle Suchbegriffvorschläge angezeigt.

1. Öffnen Sie die Datei in der Detailansicht.
1. Wählen Sie **[!UICONTROL Suchbegriffe]** aus.
1. Führen Sie einen der folgenden Schritte aus, um Schlüsselwörter hinzuzufügen:

   * Geben Sie einen Suchbegriff in das Textfeld ein und wählen Sie **[!UICONTROL Hinzufügen]** aus.
   * Wählen Sie einen Suchbegriff in der Tabelle **[!UICONTROL Suchbegriffvorschläge]** aus.

1. Um einen Suchbegriff zu entfernen, wählen Sie ihn aus und klicken Sie auf **[!UICONTROL Entfernen]**. Es wird in die Tabelle für Schlüsselwortvorschläge verschoben.

>[!NOTE]
>
>Sie können Dateien beim Hochladen in Adobe Dynamic Media Classic Suchbegriffe hinzufügen. Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL Mehr Metadaten]** und geben Sie Suchbegriffe ein.
>Siehe [Optionen für das Hochladen](uploading-files.md#upload_options).

## Importieren von Metadaten {#import-metadata}

Statt Metadaten für jedes Asset manuell einzugeben, können Sie Metadaten aus einer tabulatorgetrennten Datei oder XML-Datei für mehrere Assets gleichzeitig importieren. Die Metadaten in eine tabulatorgetrennte Datei oder XML-Datei einzugeben und diese Datei dann zu importieren, ist weniger zeitaufwendig, als die Metadaten für einzelne Assets manuell einzugeben. Geben Sie in der ersten Zeile der tabulatorgetrennten Datei die ID und die Namen der gewünschten Metadatenfelder ein. Geben Sie in die nächsten Zeilen jeweils einen Asset-ID-Namen gefolgt von den Metadaten-Werten ein. Felder, die nicht in der tabulatorgetrennten Datei oder in der XML-Datei enthalten sind, werden nicht geändert. Wenn Sie Metadaten aus einer XML-Datei importieren möchten, müssen Sie sicherstellen, dass diese DTD-konform ist.

>[!NOTE]
>
>Sie können eine Vorlage für die Eingabe von Metadaten erstellen, damit sie ordnungsgemäß in Adobe Dynamic Media Classic importiert werden können. Nachdem Sie die Vorlage erstellt haben, können Sie sie zur Eingabe der Metadaten verwenden.
>Siehe [Erstellen einer Vorlage zum Eingeben und Hochladen von Metadaten](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

Weitere Informationen zu standardisierten Eigenschaften finden Sie im [Adobe XMP Developer Center](https://www.adobe.com/devnet/xmp.html).

1. Wählen Sie im Bedienfeld Durchsuchen die Bilder aus, denen Sie Metadaten aus der tabulatorgetrennten Datei oder XML-Datei hinzufügen möchten.
1. Wechseln Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Metadaten importieren]**.
1. Wählen Sie im Dialogfeld **[!UICONTROL Metadaten hochladen]** die Option **[!UICONTROL Durchsuchen]**.
1. Wählen Sie im Dialogfeld **[!UICONTROL Hochzuladende Dateien auswählen]** die tabulatorgetrennte Datei bzw. die XML-Datei mit den Metadaten aus.
1. Geben Sie einen Auftragsnamen ein.
1. Wählen Sie **[!UICONTROL Upload]** aus.

### Identifizieren verschiedener Metadatentypen im Import

Beachten Sie Folgendes, wenn verschiedene Metadaten-Typen für den Import identifiziert werden:

* Namen von benutzerdefinierten Feldern werden wie in **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Benutzerdefinierte Felder]** erstellt. Verwenden Sie die Funktion &quot;`Generate file`&quot;, um eine Liste aller definierten UDFs im richtigen Importformat zu erhalten.
* Bei den XMP-Metadaten-Eigenschaften muss das entsprechende XMP-Präfix vor dem Namen (der Eigenschaft) stehen. Präfix und Name werden durch einen Doppelpunkt voneinander getrennt. Das XMP-Präfix finden Sie im Editor **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Metadatenschema]** . Die technischen Namen finden Sie in der Dokumentation zum jeweiligen XMP-Schema. XMP Eigenschaftsnamen werden nicht in der Funktion `Generate file` angezeigt.
* Bei den Metadaten-Eigenschaften muss das entsprechende Präfix vor dem Namen (der Eigenschaft) stehen. Präfix und Name werden durch einen Doppelpunkt voneinander getrennt. Das Präfix und die Eigenschaftsnamen werden im Metadatenschema-Editor definiert. Namen von Metadatenschema-Eigenschaften werden nicht in der Funktion `Generate file` angezeigt.

Beispiel: Die XMP Eigenschaft für Suchbegriffe ist das XMP Schema &quot;Dublin Core&quot;mit dem Präfix `dc` und `subject` ist der technische XMP. Das Präfix und der technische XMP werden in den vollständigen Eigenschaftsnamen `dc:subject` kombiniert. Im XML-Metadaten-Importformat muss `dc.subject` der Eigenschaftsname sein. Im tabulatorgetrennten Importformat muss es sich um die Spaltenüberschrift handeln.

### Importieren von Schlüsselwörtern

Schlüsselwörter können als kommagetrennte Liste importiert werden. Wenn ein Komma in einem der einzelnen Werte angezeigt wird, maskieren Sie es mit einem umgekehrten Schrägstrich (\). Ein umgekehrter Schrägstrich muss mit einem doppelten umgekehrten Schrägstrich (\\) angegeben werden.

Eine Metadaten-Importdatei mit dem Wert `Hello\, World!,back\\slash,foo` für `dc:subject` legt beispielsweise drei XMP Schlüsselwörter für das Asset fest: `Hello, World!,` `back\slash,` und `foo`.

### Importieren von XMP- und Metadaten-Schema-XMP-Dateien

Der XML-Import akzeptiert nur gültige XML. Beim Import von XMP- oder Metadatenschema-Feldern wird das Namespace-Präfix hinzugefügt und verhält sich hier wie ein XMP-Namespace. Dieser Namespace muss deklariert werden. Beispiel: im Tag der obersten Ebene.

Beispiel:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

### Importieren von XMP- und Metadatenschema-Metadaten in tabulatorgetrennte Dateien

Das Präfix muss in der entsprechenden Spaltenüberschrift im Importfeld hinzugefügt werden.

## Importieren von Metadaten (über FTP) {#import-metadata-via-ftp}

Sie können Metadaten für mehrere Dateien importieren. Sie geben die Metadaten in einer tabulatorgetrennten oder XML-Datei ein. Wählen Sie dann **[!UICONTROL Metadatendateien verarbeiten]** auf der Seite &quot;Upload-Auftragsoptionen&quot;(Registerkarte &quot;Über FTP&quot;).

Stellen Sie sicher, dass die Daten in der tabulatorgetrennten Datei oder in der XML-Datei im korrekten Format vorliegen. Geben Sie in die erste Zeile das ID-Feld, gefolgt von den Namen der Metadaten-Felder ein, die geändert werden sollen. Geben Sie in die nächsten Zeilen jeweils einen Asset-ID-Namen gefolgt von den Metadaten-Werten ein. Felder, die nicht in der tabulatorgetrennten Datei oder in der XML-Datei enthalten sind, werden nicht geändert.

Wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Upload]** aus. Um die Metadaten zu importieren, wählen Sie auf der Seite &quot;Hochladen&quot;die Registerkarte **[!UICONTROL Über FTP]** und dann **[!UICONTROL Auftragsoptionen]** aus. Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option **[!UICONTROL Auftrag]** und aktivieren Sie dann das Kontrollkästchen **[!UICONTROL Metadatendateien verarbeiten]** .

## Stapel-Umbenennung von IDs mit Metadaten {#batch-rename-ids-using-metadata}

Mithilfe von Metadaten, die aus einer tabulatorgetrennten Datei oder einer XML-Datei importiert wurden, können Sie Adobe Dynamic Media Classic-IDs umbenennen. Die importierten Metadaten werden nur auf die in der Metadatendatei selbst angegebenen Bilder angewendet. Es spielt keine Rolle, ob Bilder im Bedienfeld &quot;Durchsuchen&quot;ausgewählt sind.

Um die Adobe Dynamic Media Classic ID eines Bildes umzubenennen, fügen Sie der tabulatorgetrennten Datei eine Spalte mit der Bezeichnung *newipsid* hinzu oder fügen Sie den XML-Daten ein Feld mit der Bezeichnung `new_vc_objectname` hinzu.

Beispiel:

| | newipsid |
| --- | --- |
| testjacket_1 | Jacket_test_1 |
| testjacket_blue | Jacket_test_2 |

Das Auftragsprotokoll für den Metadatenauftrag zeigt an, welche IDs erfolgreich umbenannt wurden und welche nicht.

## Erstellen einer Vorlage zum Eingeben und Hochladen von Metadaten {#create-a-template-for-entering-metadata-to-upload}

Adobe Dynamic Media Classic bietet einen Befehl zum Erstellen einer Vorlage zum Aufzeichnen von Metadaten. Die Verwendung der Vorlage stellt sicher, dass die Metadaten im richtigen Format eingegeben werden, damit sie korrekt in Adobe Dynamic Media Classic hochgeladen werden können. Gehen Sie wie folgt vor, um eine Vorlage für die Aufzeichnung und den Import von Metadaten in Adobe Dynamic Media Classic zu erstellen:

1. Wählen Sie Bild-Assets mit Metadatenfeldern aus, die Sie für Ihre Vorlage verwenden möchten.
1. Wechseln Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Metadaten importieren]**.
1. Wählen Sie für den **[!UICONTROL Asset-Eigenschaftstyp]** **[!UICONTROL Bild]** aus.
1. Wählen Sie aus der Dropdownliste **[!UICONTROL `Generate File`]** die Option **[!UICONTROL tabulatorgetrennte Vorlage]**, die XML-Metadaten des Assets ]**oder die**[!UICONTROL  XML-DTD ]**aus.**[!UICONTROL 
1. Wählen Sie **[!UICONTROL Erzeugen]** aus.
1. Kopieren Sie die Daten im daraufhin angezeigten Dialogfeld. Verwenden Sie diese Daten, um die Vorlage zu erstellen.

## Arbeiten mit Metadaten-Schemata {#working-with-metadata-schemas}

Ein Unternehmensadministrator kann eine Liste aller verfügbaren Schemas anzeigen. Wechseln Sie in der globalen Navigationsleiste zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Metadatenschema]**.

Zunächst wird die Liste der globalen Standardschemata wie XMP ausgeblendet. Sie können mithilfe des Kontrollkästchens unten in der Liste angezeigt werden.

Der Unternehmensadministrator kann ein benutzerdefiniertes Schema erstellen oder ein vorhandenes benutzerdefiniertes Schema bearbeiten.

Sie können den Metadaten-Schema-Editor verwenden, um die folgenden Aktionen ausführen:

| Aktion | Beschreibung |
| --- | --- |
| Hinzufügen | Fügt dem Schema eine Eigenschaft hinzu. Ein modales Dialogfeld erfasst die Informationen: ID, Titel, Struktur und Datentyp. |
| Auswahlwert hinzufügen | Fügt einer Eigenschaft mit „Offene Auswahl“ oder „Geschlossene Auswahl“ eine neue Auswahloption hinzu. Alle Auswahlwerte haben den gleichen Typ. Wählen Sie die Eigenschaft selbst aus, um die Schaltfläche zu aktivieren. |
| Bearbeiten | Bearbeiten der Beschriftung einer Eigenschaft oder eines Auswahlwertes. Sie können nur die Beschriftung und ID ändern, nicht aber die Typinformationen. |
| Nach oben/Nach unten | Die Reihenfolge im Schema wird in der Benutzeroberfläche übernommen. Um die Reihenfolge zu ändern, wählen Sie eine Eigenschaft oder einen Auswahlwert aus und verschieben diese mit den Schaltflächen. Drag &amp; Drop wird derzeit nicht unterstützt. |
| Löschen | Löscht eine Eigenschaft oder einen Auswahlwert aus dem Schema. Werte werden nicht aus dem XMP oder der Datenbank gelöscht. Die Eigenschaft ist nicht mehr für Metadaten-Ansichten verfügbar und wird aus der Asset-Detailansicht entfernt. Wenn die Eigenschaft auf dem Metadaten-Server veröffentlicht wurde, führen Sie eine erzwungene Veröffentlichung durch, um die Daten vom öffentlich zugänglichen Metadaten-Server zu entfernen. |

Das System generiert automatisch ein benutzerdefiniertes Schema für benutzerdefinierte Felder mit dem Präfix &quot;`s7udf`&quot;. Das Schema besteht aus vorhandenen benutzerdefinierten Feldern, die in ihrem eigenen Setup-Bereich bearbeitet werden.

>[!NOTE]
>
>Von Änderungen am Schema bleiben die Asset-Metadaten unberührt. Sie sind jedoch nicht für alle Adobe Dynamic Media Classic- und Metadaten-Server-Funktionen sichtbar und können nach einer Änderung nicht mehr aufgerufen werden. Wenn Metadaten für ein Asset vorhanden sind, werden die Metadaten durch die Erstellung des entsprechenden Schemas in Adobe Dynamic Media Classic und auf dem Metadatenserver verwendet.

Der Metadatenschema-Editor bietet eine grafische Möglichkeit, ein benutzerdefiniertes Unternehmensschema in Adobe Dynamic Media Classic hinzuzufügen oder zu bearbeiten. Ein Präfix, ein Namespace und eine Liste von Eigenschaften definieren ein Schema.

* **[!UICONTROL Name]**: UI-Name für das Schema. Wird verwendet, um die Eigenschaften in den Metadaten-Ansichten und bei der erweiterten Suche zu identifizieren. Vergleichbar mit XMP-Abschnitten wie Basic, IPTC, PDF.

* **[!UICONTROL Präfix]**: Technische eindeutige Kennung für das Schema. Beschränkt auf die Buchstaben a-z und A-Z. Das Präfix ist nicht in der Benutzeroberfläche von Adobe Dynamic Media Classic sichtbar, wird jedoch verwendet, wenn Metadaten für ein Asset im XMP und in der Datenbank gespeichert werden. Mit dem Präfix werden Metadatenfelder in Metadaten-Suchabfragen auf dem Metadaten-Server oder -Import eindeutig identifiziert.

* **[!UICONTROL Namespace]**: Technische eindeutige Kennung für das Schema, normalerweise eine URL im Formular `https://your.company.com/name/version/`. Weitere Informationen finden Sie in der Liste der Standardschemata für Beispiele. Der Namespace ist in der Adobe Dynamic Media Classic-Benutzeroberfläche nicht sichtbar, wird jedoch zum Speichern von Metadaten im XMP-Block verwendet.

* **[!UICONTROL Beschreibung]**: Freiformbeschreibung des Schemas.

>[!NOTE]
>
>Präfix und Namespace können nicht bearbeitet werden. Um diese Eigenschaften zu ändern, müssen Sie das Schema löschen und neu erstellen.

Eigenschaften beschreiben die Metadaten, die mit diesem Schema im XMP-Block gespeichert werden können. Eine Eigenschaft besteht aus:

| Eigenschaft | Beschreibung |
| --- | --- |
| ID | Technischer Identifikator für diese Eigenschaft. Die ID ist nicht in der Adobe Dynamic Media Classic-Benutzeroberfläche sichtbar, wird jedoch verwendet, wenn Metadaten für ein Asset im XMP und in der Datenbank gespeichert werden. Die ID wird verwendet, um Suchanfragen auf dem Metadaten-Server zu erstellen. Die ID weist einige Einschränkungen auf, z. B.: `<ul><li>No spaces</li><li>No ".", ":", "$"</li><li>No number as first character</li><li>Best practice is to use a-z or A-Z as first character</li></ul>` <br>Nach der Erstellung kann die ID nicht mehr geändert werden. |
| Beschriftung | Name dieser Eigenschaft in der Benutzeroberfläche. |
| Struktur | Legt die Art der Eigenschaft zusammen mit dem Datentyp fest. Eine Struktur kann sein:<ul><li>Einfacher Typ: Einzelwert des Datentyps</li><li>Sequenz: eine Liste von Werten desselben Datentyps</li><li>Auswahl öffnen: Wählen Sie ein Element aus einer Liste vordefinierter Werte aus oder geben Sie Text ein. Sie kann nur vom Datentyp String oder Integer sein</li><li>Geschlossene Auswahl: Wählen Sie ein Element aus einer zuvor festgelegten Liste von Werten aus (ein Popup- oder ein Kombinationsfeld).</li></ul> |
| Datentyp | Wählen Sie aus den verfügbaren Typen aus: <ul><li>Zeichenfolge</li><li>Integer</li><li>Float</li><li>Ja/Nein (Boolescher Wert)</li><li>Datum</li></ul> |

Wenn die Eigenschaft die Struktur &quot;Open Choice&quot;oder &quot;Closed Choice&quot;aufweist, müssen Sie mindestens einen Auswahlwert angeben. Eine offene Auswahl kann geändert werden. Eine geschlossene Auswahl kann nicht geändert werden. Alle Auswahlwerte haben den Datentyp der Eigenschaft .

| Eigenschaft | Beschreibung |
| --- | --- |
| ID | Technischer Identifikator für diesen Wert. Die ID ist nicht in der Adobe Dynamic Media Classic-Benutzeroberfläche sichtbar, wird jedoch verwendet, wenn Metadaten für ein Asset im XMP und in der Datenbank gespeichert werden. Die ID wird für Suchanfragen auf dem Metadatenserver verwendet. Die ID darf keine Leerzeichen enthalten. Sobald erstellt, kann die ID nicht geändert werden. |
| Beschriftung | Name dieses Wertes in der Benutzeroberfläche. |

>[!MORELIKETHIS]
>
>* [Viewer-Vorgaben](application-setup.md#viewer_presets)
>* [Metadaten-Vorgaben](application-setup.md#metadata_presets)
