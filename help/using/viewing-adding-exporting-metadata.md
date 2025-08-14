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

Sie können spezifische Informationen zu den Dateien speichern, mit denen Sie in Adobe Dynamic Media Classic arbeiten. Diese Informationen werden als &quot;*&quot;*. Sie können Metadaten in Adobe Dynamic Media Classic zum Organisieren, Suchen, Filtern und Sortieren von Assets verwenden.

Metadaten werden in der Detailansicht angezeigt. Es wird zusammen mit von Adobe Dynamic Media Classic generierten Informationen angezeigt. Beispielsweise das Erstellungsdatum einer Datei, das Veröffentlichungsdatum und Schlüsselwörter. Um Metadaten anzuzeigen, öffnen Sie das Asset in der Detailansicht und wählen Sie dann das Metadaten-Bedienfeld aus. Sie können Metadaten in der Detailansicht eingeben und bearbeiten.

Manche Metadaten sind direkt in eine Datei eingebettet. Wenn eine Datei diese Metadaten enthält, lädt Adobe Dynamic Media Classic sie automatisch mit der -Datei hoch. Sie können Metadaten in Quell-Assets in Adobe Photoshop, InDesign, Illustrator und andere Programme einbetten. Adobe Dynamic Media Classic erkennt diese Metadaten. Sie können auch im Bedienfeld „Metadaten“ in der Detailansicht Metadaten zu einzelnen Dateien hinzufügen. Damit die Einheitlichkeit Asset-übergreifend gewährleistet werden kann, können Unternehmensadministratoren Metadatenvorlagen mit den zu verwendenden Metadatenfeldern erstellen.

Weitere Informationen zu eingebetteten Metadaten finden Sie unter [Extensible Metadata Platform](https://www.adobe.com/products/xmp.html).

## Anzeigen von Metadaten {#view-metadata}

Um die Metadaten eines Assets anzuzeigen, öffnen Sie das Asset in der Detailansicht und tippen Sie auf das Bedienfeld „Metadaten“. Um einen Satz von Metadatenfeldern auszuwählen, wählen Sie eine Option im Menü „Metadatenansicht“. Adobe Dynamic Media Classic bietet die folgenden Metadatenansichten:

* **Kompakte Ansicht**: Eine einfache Werteliste.

* **IPTC**: Werte, wie sie vom International Press Telecommunications Council definiert wurden.

* **XMP**: Werte, wie vom Extensible Metadata-Programm definiert.

Administratoren können Metadaten-Ansichten erstellen. Diese Ansichten werden auch im Menü Metadatenansichten angezeigt.

Informationen [ Erstellen von Metadatenansichten finden ](application-setup.md#metadata_views) unter „Metadatenansichten“.

## Manuelles Eingeben von Metadaten für ein Asset {#manually-enter-metadata-for-an-asset}

1. Öffnen Sie das Asset in der Detailansicht.
1. Öffnen Sie das Metadatenbedienfeld und führen Sie einen oder beide der folgenden Schritte aus:

   * Wählen Sie die Metadatenansicht aus, um festzustellen, welche Metadatenfelder im Bedienfeld angezeigt werden.
   * Wählen Sie einen Vorgabewert aus und klicken Sie dann auf **[!UICONTROL Anwenden]**, um Metadatenfelder mit Vorgabewerten zu füllen. Diese Vorgabewerte werden von Unternehmensadministratoren erstellt.

1. Geben Sie die Werte im Bedienfeld „Metadaten“ ein.

>[!NOTE]
>
>Wenn Sie die Metadaten mehrerer Assets gleichzeitig bearbeiten möchten, wählen Sie die Assets aus und gehen Sie zu **[!UICONTROL Datei]** > **[!UICONTROL Info bearbeiten]**. Änderungen, die Sie im Fenster Info bearbeiten an Metadaten vorgenommen haben, werden auf alle ausgewählten Assets angewendet.

## Hinzufügen oder Bearbeiten von Schlüsselwörtern {#add-or-edit-keywords}

Zusätzlich zu Metadaten können Sie Keywords verwenden, um die Suche und Verwaltung Ihrer Assets zu erleichtern.

Wenn Sie während dieser Sitzung Keywords zu anderen Dateien hinzugefügt oder Keywords aus Ihrer Liste entfernt haben, erscheinen diese in der Tabelle der Keyword-Vorschläge.

1. Öffnen Sie die Datei in der Detailansicht.
1. Wählen Sie **[!UICONTROL Keywords]** aus.
1. Führen Sie einen der folgenden Schritte aus, um Schlüsselwörter hinzuzufügen:

   * Geben Sie einen Suchbegriff in das Textfeld ein und wählen Sie **[!UICONTROL Hinzufügen]**.
   * Wählen Sie ein Keyword in der Tabelle **[!UICONTROL Keyword-]**&quot; aus.

1. Um ein Keyword zu entfernen, wählen Sie es aus und klicken Sie auf **[!UICONTROL Entfernen]**. Es wird in die Tabelle für Schlüsselwortvorschläge verschoben.

>[!NOTE]
>
>Sie können Schlüsselwörter zu Dateien hinzufügen, während Sie sie in Adobe Dynamic Media Classic hochladen. Wählen Sie im Dialogfeld Upload-Auftragsoptionen die Option **[!UICONTROL Weitere Metadaten]** und geben Sie Schlüsselwörter ein.
>>Siehe [Optionen für das Hochladen](uploading-files.md#upload_options).

## Importieren von Metadaten {#import-metadata}

Statt Metadaten für jedes Asset manuell einzugeben, können Sie Metadaten aus einer tabulatorgetrennten Datei oder XML-Datei für mehrere Assets gleichzeitig importieren. Die Metadaten in eine tabulatorgetrennte Datei oder XML-Datei einzugeben und diese Datei dann zu importieren, ist weniger zeitaufwendig, als die Metadaten für einzelne Assets manuell einzugeben. Geben Sie in der ersten Zeile der tabulatorgetrennten Datei die ID und die Namen der gewünschten Metadatenfelder ein. Geben Sie in die nächsten Zeilen jeweils einen Asset-ID-Namen gefolgt von den Metadaten-Werten ein. Felder, die nicht in der tabulatorgetrennten Datei oder in der XML-Datei enthalten sind, werden nicht geändert. Wenn Sie Metadaten aus einer XML-Datei importieren möchten, müssen Sie sicherstellen, dass diese DTD-konform ist.

>[!NOTE]
>
>Sie können eine Vorlage für die Eingabe von Metadaten erstellen, damit sie ordnungsgemäß in Adobe Dynamic Media Classic importiert werden können. Nachdem Sie die Vorlage erstellt haben, können Sie sie zur Eingabe der Metadaten verwenden.
>>Siehe [Erstellen einer Vorlage zum Eingeben und Hochladen von Metadaten](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

Weitere Informationen über standardisierte Eigenschaften finden Sie im [Adobe XMP Developer Center](https://www.adobe.com/devnet/xmp.html).

1. Wählen Sie im Durchsuchen-Panel die Bilder aus, denen Sie Metadaten aus der durch Tabulatoren getrennten oder XML-Datei hinzufügen möchten.
1. Navigieren Sie **[!UICONTROL Datei]** > **[!UICONTROL Metadaten importieren]**.
1. Wählen **[!UICONTROL Dialogfeld „Metadaten hochladen]** die Option **[!UICONTROL Durchsuchen]** aus.
1. Wählen Sie im Dialogfeld **[!UICONTROL Hochzuladende Dateien auswählen]** die tabulatorgetrennte Datei bzw. die XML-Datei mit den Metadaten aus.
1. Geben Sie einen Auftragsnamen ein.
1. Wählen Sie **[!UICONTROL Hochladen]** aus.

### Identifizieren verschiedener Metadatentypen beim Import

Beachten Sie Folgendes, wenn verschiedene Metadaten-Typen für den Import identifiziert werden:

* Die Namen der benutzerdefinierten Felder werden wie unter **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinrichtung]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Benutzerdefinierte Felder]** erstellt. Mit der Funktion `Generate file` können Sie eine Liste aller definierten UDFs im richtigen Importformat abrufen.
* Bei den XMP-Metadaten-Eigenschaften muss das entsprechende XMP-Präfix vor dem Namen (der Eigenschaft) stehen. Präfix und Name werden durch einen Doppelpunkt voneinander getrennt. Das XMP-Präfix finden Sie unter **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinrichtung]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Metadatenschema]** Editor. Die technischen Namen finden Sie in der Dokumentation zum jeweiligen XMP-Schema. XMP-Eigenschaftsnamen werden in der `Generate file`-Funktion nicht angezeigt.
* Bei den Metadaten-Eigenschaften muss das entsprechende Präfix vor dem Namen (der Eigenschaft) stehen. Präfix und Name werden durch einen Doppelpunkt voneinander getrennt. Das Präfix und die Eigenschaftsnamen werden im Metadatenschema-Editor definiert. Namen von Metadatenschema-Eigenschaften werden in der `Generate file`-Funktion nicht angezeigt.

Beispiel: Die XMP-Eigenschaft für Schlüsselwörter ist das XMP-Schema „Dublin Core“ mit dem Präfix `dc` und `subject` der technische XMP-Name. Das Präfix und der technische XMP-Name werden zum `dc:subject` vollständigen Eigenschaftsnamen kombiniert. Im Importformat der XML-Metadaten muss `dc.subject` der Eigenschaftsname sein. Im tabulatorgetrennten Importformat muss es die Spaltenüberschrift sein.

### Importieren von Schlüsselwörtern

Keywords können als kommagetrennte Liste importiert werden. Wenn ein Komma in einem der einzelnen Werte angezeigt wird, führen Sie eine Escape-Operation mit einem umgekehrten Schrägstrich (\) durch. Ein umgekehrter Schrägstrich muss mit einem doppelten umgekehrten Schrägstrich (\\) angegeben werden.

Beispielsweise legt eine Metadaten-Importdatei, die den für `Hello\, World!,back\\slash,foo` `dc:subject` Wert enthält, drei XMP-Schlüsselwörter für das Asset fest: `Hello, World!,` `back\slash,` und `foo`.

### Importieren von XMP- und Metadaten-Schema-XMP-Dateien

Der XML-Import akzeptiert nur gültige XML. Beim Importieren von XMP- oder Metadatenschemafeldern wird das Namespace-Präfix hinzugefügt und verhält sich hier wie ein XMP-Namespace. Dieser Namespace muss deklariert werden. Zum Beispiel im Tag der obersten Ebene.

Beispiel:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

### Durch Tabulatoren getrennte Dateien mit XMP- und Metadatenschema-Metadaten importieren

Das Präfix muss in der entsprechenden Spaltenüberschrift im Importfeld hinzugefügt werden.

## Importieren von Metadaten (über FTP) {#import-metadata-via-ftp}

Sie können Metadaten für mehrere Dateien importieren. Die Metadaten werden in einer durch Tabulatoren getrennten oder XML-Datei eingegeben. Wählen Sie anschließend **[!UICONTROL Metadatendateien verarbeiten]** auf der Seite Upload-Auftragsoptionen (über FTP) aus.

Stellen Sie sicher, dass die Daten in der tabulatorgetrennten Datei oder in der XML-Datei im korrekten Format vorliegen. Geben Sie in die erste Zeile das ID-Feld, gefolgt von den Namen der Metadaten-Felder ein, die geändert werden sollen. Geben Sie in die nächsten Zeilen jeweils einen Asset-ID-Namen gefolgt von den Metadaten-Werten ein. Felder, die nicht in der tabulatorgetrennten Datei oder in der XML-Datei enthalten sind, werden nicht geändert.

Wählen Sie in der Symbolleiste für globale Navigation **[!UICONTROL Hochladen]** aus. Um die Metadaten zu importieren, klicken Sie auf der Seite Hochladen auf die Registerkarte **[!UICONTROL Per FTP]** und wählen Sie dann **[!UICONTROL Auftragsoptionen]** aus. Wählen Sie im Dialogfeld Upload-Auftragsoptionen die Option **[!UICONTROL Auftrag]** und aktivieren Sie dann das Kontrollkästchen **[!UICONTROL Metadatendateien verarbeiten]**.

## Stapel-Umbenennung von IDs mit Metadaten {#batch-rename-ids-using-metadata}

Mithilfe von Metadaten, die aus einer tabulatorgetrennten Datei oder XML-Datei importiert wurden, können Sie Adobe Dynamic Media Classic-IDs umbenennen. Die importierten Metadaten werden nur auf die in der Metadatendatei selbst angegebenen Bilder angewendet. Es spielt keine Rolle, ob Bilder im Durchsuchen-Panel ausgewählt sind.

Um die Adobe Dynamic Media Classic-ID eines Bildes umzubenennen, fügen Sie der durch Tabulatoren getrennten Datei eine Spalte mit *newipsid* hinzu oder fügen Sie den XML-Daten ein Feld mit dem Namen `new_vc_objectname` hinzu.

Beispiel:

| | newipsid |
| --- | --- |
| testjacket_1 | Jacket_test_1 |
| testjacket_blue | Jacket_test_2 |

Das Vorgangslog für den Metadatenvorgang zeigt an, welche IDs erfolgreich umbenannt wurden und welche nicht.

## Erstellen einer Vorlage zum Eingeben und Hochladen von Metadaten {#create-a-template-for-entering-metadata-to-upload}

Adobe Dynamic Media Classic bietet einen Befehl zum Erstellen einer Vorlage für die Aufzeichnung von Metadaten. Durch die Verwendung der Vorlage wird sichergestellt, dass die Metadaten im richtigen Format eingegeben werden, damit sie korrekt in Adobe Dynamic Media Classic hochgeladen werden können. Gehen Sie wie folgt vor, um eine Vorlage zur Verwendung beim Aufzeichnen und Importieren von Metadaten in Adobe Dynamic Media Classic zu erstellen:

1. Wählen Sie Bild-Assets mit Metadatenfeldern aus, die Sie für Ihre Vorlage verwenden möchten.
1. Navigieren Sie **[!UICONTROL Datei]** > **[!UICONTROL Metadaten importieren]**.
1. Wählen Sie für **[!UICONTROL Asset-Eigenschaftstyp]** die Option **[!UICONTROL Bild]** aus.
1. Wählen Sie aus der Dropdown-Liste **[!UICONTROL `Generate File`]** die Option **[!UICONTROL Tabulatorgetrennte Vorlage]**, **[!UICONTROL XML-Metadaten des Assets]** oder **[!UICONTROL XML-DTD]**.
1. Wählen Sie **[!UICONTROL Generieren]** aus.
1. Kopieren Sie die Daten im daraufhin angezeigten Dialogfeld. Verwenden Sie diese Daten, um die Vorlage zu erstellen.

## Arbeiten mit Metadaten-Schemata {#working-with-metadata-schemas}

Ein Unternehmensadministrator kann eine Liste aller verfügbaren Schemata anzeigen. Wechseln Sie in der globalen Navigationsleiste zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Metadaten]** > **[!UICONTROL Metadatenschema]**.

Zunächst wird die Liste der globalen Standardschemata wie XMP ausgeblendet. Sie können mithilfe des Kontrollkästchens unten in der Liste angezeigt werden.

Der Unternehmensadministrator kann ein benutzerdefiniertes Schema erstellen oder ein vorhandenes benutzerdefiniertes Schema bearbeiten.

Sie können den Metadaten-Schema-Editor verwenden, um die folgenden Aktionen ausführen:

| Aktion | Beschreibung |
| --- | --- |
| Hinzufügen | Fügt dem Schema eine Eigenschaft hinzu. Ein modales Dialogfeld erfasst die folgenden Informationen: ID, Beschriftung, Struktur und Datentyp. |
| Auswahlwert hinzufügen | Fügt einer Eigenschaft mit „Offene Auswahl“ oder „Geschlossene Auswahl“ eine neue Auswahloption hinzu. Alle Auswahlwerte haben den gleichen Typ. Wählen Sie die Eigenschaft selbst aus, um die Schaltfläche zu aktivieren. |
| Bearbeiten | Bearbeiten der Beschriftung einer Eigenschaft oder eines Auswahlwertes. Sie können nur die Beschriftung und ID ändern, nicht aber die Typinformationen. |
| Nach oben/Nach unten | Die Reihenfolge im Schema wird in der Benutzeroberfläche übernommen. Um die Reihenfolge zu ändern, wählen Sie eine Eigenschaft oder einen Auswahlwert aus und verschieben diese mit den Schaltflächen. Drag &amp; Drop wird derzeit nicht unterstützt. |
| Löschen | Löscht eine Eigenschaft oder einen Auswahlwert aus dem Schema. Es werden keine Werte aus dem XMP-Block oder der Datenbank gelöscht. Die Eigenschaft ist nicht mehr für Metadatenansichten verfügbar und wird aus der Asset-Detailansicht entfernt. Wenn die Eigenschaft auf dem Metadaten-Server veröffentlicht wurde, führen Sie eine erzwungene Veröffentlichung durch, um die Daten vom öffentlich zugänglichen Metadaten-Server zu entfernen. |

Das System generiert automatisch ein benutzerdefiniertes Schema für benutzerdefinierte Felder mit dem Präfix `s7udf`. Das Schema besteht aus vorhandenen benutzerdefinierten Feldern, die in ihrem eigenen Setup-Abschnitt bearbeitet werden.

>[!NOTE]
>
>Von Änderungen am Schema bleiben die Asset-Metadaten unberührt. Sie sind jedoch nicht für alle Adobe Dynamic Media Classic- und Metadaten-Server-Funktionen sichtbar und können nach einer Änderung nicht mehr aufgerufen werden. Wenn Metadaten für ein Asset vorhanden sind, macht die Erstellung des entsprechenden Schemas die Metadaten in Adobe Dynamic Media Classic und auf dem Metadatenserver nutzbar.

Der Metadatenschema-Editor bietet eine grafische Möglichkeit, ein benutzerdefiniertes Unternehmensschema in Adobe Dynamic Media Classic hinzuzufügen oder zu bearbeiten. Ein Schema wird durch ein Präfix, einen Namespace und eine Liste von Eigenschaften definiert.

* **[!UICONTROL Name]**: UI-Name für das Schema. Wird verwendet, um die Eigenschaften in den Metadaten-Ansichten und bei der erweiterten Suche zu identifizieren. Vergleichbar mit XMP-Abschnitten wie Basic, IPTC, PDF.

* **[!UICONTROL Präfix]**: Technische eindeutige Kennung für das Schema. Beschränkung auf die Buchstaben a-z und A-Z. Das Präfix ist in der Benutzeroberfläche von Adobe Dynamic Media Classic nicht sichtbar, wird jedoch verwendet, wenn Metadaten für ein Asset im XMP-Block und in der Datenbank gespeichert werden. Das Präfix identifiziert Metadatenfelder in Metadatensuchabfragen auf dem Metadaten-Server oder beim Import eindeutig.

* **[!UICONTROL Namespace]**: Technische eindeutige Kennung für das Schema, normalerweise eine URL im `https://your.company.com/name/version/`. Weitere Informationen finden Sie in der Liste der Standardschemata für Beispiele. Der Namespace ist in der Adobe Dynamic Media Classic-Benutzeroberfläche nicht sichtbar, wird jedoch zum Speichern von Metadaten im XMP-Block verwendet.

* **[!UICONTROL Beschreibung]**: Freiformbeschreibung des Schemas.

>[!NOTE]
>
>Präfix und Namespace können nicht bearbeitet werden. Um diese Eigenschaften zu ändern, müssen Sie das Schema löschen und neu erstellen.

Eigenschaften beschreiben die Metadaten, die mit diesem Schema im XMP-Block gespeichert werden können. Eine Eigenschaft besteht aus:

| Eigenschaft | Beschreibung |
| --- | --- |
| ID | Technischer Identifikator für diese Eigenschaft. Die ID ist in der Benutzeroberfläche von Adobe Dynamic Media Classic nicht sichtbar, wird jedoch verwendet, wenn Metadaten für ein Asset im XMP-Block und in der Datenbank gespeichert werden. Die ID wird verwendet, um Suchabfragen auf dem Metadaten-Server zu erstellen. Die ID weist einige Einschränkungen auf, z. B`<ul><li>No spaces</li><li>No ".", ":", "$"</li><li>No number as first character</li><li>Best practice is to use a-z or A-Z as first character</li></ul>`: <br>Nach ihrer Erstellung kann die ID nicht mehr geändert werden. |
| Beschriftung | Name dieser Eigenschaft in der Benutzeroberfläche. |
| Struktur | Legt die Art der Eigenschaft zusammen mit dem Datentyp fest. Eine Struktur kann sein:<ul><li>Einfacher Typ: Einzelwert des Datentyps</li><li>Sequenz: eine Liste von Werten desselben Datentyps</li><li>Auswahl öffnen : Wählen Sie ein Element aus einer Liste vordefinierter Werte aus oder geben Sie einen Text ein. Sie kann nur vom Datentyp „String“ oder „Integer“ sein</li><li>Geschlossene Auswahl: Wählen Sie ein Element aus einer zuvor festgelegten Liste von Werten aus (ein Popup- oder ein Kombinationsfeld).</li></ul> |
| Datentyp | Wählen Sie aus den verfügbaren Typen aus: <ul><li>Zeichenfolge</li><li>Integer</li><li>Float</li><li>Ja/Nein (Boolescher Wert)</li><li>Datum</li></ul> |

Wenn die Eigenschaft die Struktur Offene Auswahl oder Geschlossene Auswahl aufweist, müssen Sie mindestens einen Auswahlwert angeben. Eine offene Auswahl kann geändert werden. Eine geschlossene Auswahl kann nicht geändert werden. Alle Auswahlwerte haben den Datentyp der Eigenschaft.

| Eigenschaft | Beschreibung |
| --- | --- |
| ID | Technischer Identifikator für diesen Wert. Die ID ist in der Benutzeroberfläche von Adobe Dynamic Media Classic nicht sichtbar, wird jedoch verwendet, wenn Metadaten für ein Asset im XMP-Block und in der Datenbank gespeichert werden. Die ID wird für Suchanfragen auf dem Metadatenserver verwendet. Die ID darf keine Leerzeichen enthalten. Sobald erstellt, kann die ID nicht geändert werden. |
| Beschriftung | Name dieses Wertes in der Benutzeroberfläche. |

>[!MORELIKETHIS]
>
>* [Viewer-Vorgaben](application-setup.md#viewer_presets)
>* [Metadaten-Vorgaben](application-setup.md#metadata_presets)
