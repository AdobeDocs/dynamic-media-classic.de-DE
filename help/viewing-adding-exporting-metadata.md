---
title: Anzeigen, Hinzufügen und Exportieren von Metadaten
seo-title: Anzeigen, Hinzufügen und Exportieren von Metadaten
description: 'null'
seo-description: Erfahren Sie, wie Sie Metadaten anzeigen, hinzufügen und exportieren.
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: admin
content-type: Verweis
products: SG_EXPERIENCEMANAGER/Dynamic Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Anzeigen, Hinzufügen und Exportieren von Metadaten{#viewing-adding-and-exporting-metadata}

Sie haben die Möglichkeit, spezifische Informationen über die Dateien, mit denen Sie arbeiten, im Scene7 Publishing System zu speichern. Diese Informationen werden als *Metadaten* bezeichnet. Sie können in Dynamic Media Classic Metadaten zum Organisieren, Suchen, Filtern und Sortieren Ihrer Assets verwenden.

Metadaten werden in der Detailansicht zusammen mit von Dynamic Media Classic generierten Informationen wie dem Dateierstellungsdatum, dem Veröffentlichungsdatum und Schlüsselwörtern angezeigt. Um Metadaten anzuzeigen, öffnen Sie das Asset in der Detailansicht und wählen Sie das Metadatenbedienfeld aus. Sie können Metadaten in der Detailansicht eingeben und bearbeiten.

Manche Metadaten sind direkt in eine Datei eingebettet. Wenn eine Datei diese Metadaten enthält, lädt Dynamic Media Classic sie automatisch mit der Datei hoch. Sie können Metadaten in Adobe Fotoshop, InDesign, Illustrator und anderen Anwendungen in Quellelemente einbetten. Dynamic Media Classic erkennt diese Metadaten. Sie können in der Detailansicht über das Metadatenbedienfeld auch einzelnen Dateien Metadaten hinzufügen. Damit die Einheitlichkeit Asset-übergreifend gewährleistet werden kann, können Unternehmensadministratoren Metadatenvorlagen mit den zu verwendenden Metadatenfeldern erstellen.

For more information about embedded metadata, see [www.adobe.com/go/learn_s7_xmp_en](https://www.adobe.com/go/learn_s7_xmp_en).

## Anzeigen von Metadaten {#view-metadata}

Um die Metadaten eines Assets anzuzeigen, öffnen Sie es in der Detailansicht und klicken Sie auf das Metadatenbedienfeld. Wählen Sie anschließend eine Option aus dem Menü „Metadaten-Ansichten“ aus, um einen Metadatenfeldersatz auszuwählen. Dynamic Media Classic bietet folgende Metadaten-Ansichten:

* **Kompakte Ansicht** Eine grundlegende Liste von Werten.

* **IPTC**-Werte, wie vom International Press Telecommunications Council definiert.

* **XMP**-Werte, wie von der Extensible Metadata Platform definiert.

Administratoren können Metadaten-Ansichten erstellen. Diese Ansichten werden auch im Menü „Metadaten-Ansichten“ angezeigt. Weitere Informationen zum Erstellen von Metadaten-Ansichten finden Sie unter [Metadaten-Ansichten](application-setup.md#metadata_views).

## Manuelles Eingeben von Metadaten für ein Asset {#manually-enter-metadata-for-an-asset}

1. Zeigen Sie das Asset in der Detailansicht an.
1. Öffnen Sie das Metadatenbedienfeld und führen Sie einen oder beide der folgenden Schritte aus:

   * Wählen Sie die Metadatenansicht aus, um festzustellen, welche Metadatenfelder im Bedienfeld angezeigt werden.
   * Wählen Sie einen Vorgabewert aus und klicken Sie auf „Übernehmen“, um die Metadatenfelder mit den Vorgabewerten zu füllen. Diese Vorgabewerte werden von Unternehmensadministratoren erstellt.

1. Geben Sie Werte in das Metadatenbedienfeld ein.

>[!NOTE]
>
>Um die Metadaten mehrerer Assets gleichzeitig zu bearbeiten, wählen Sie „Datei“ &gt; „Informationen bearbeiten“. Bearbeitungen, die Sie im Fenster „Informationen bearbeiten“ an Metadaten vornehmen, werden auf alle ausgewählten Assets angewendet.

## Hinzufügen oder Bearbeiten von Schlüsselwörtern {#add-or-edit-keywords}

Neben Metadaten können Sie Schlüsselwörter verwenden, um die Durchsuchung und Verwaltung Ihrer Assets zu unterstützen.

Wenn Sie während dieser Sitzung Schlüsselwörter zu anderen Dateien hinzugefügt oder aus Ihrer Liste entfernt haben, werden Sie in der Tabelle für Schlüsselwortvorschläge angezeigt.

1. Öffnen Sie die Datei in der Detailansicht.
1. Klicken Sie auf „Schlüsselwörter“.
1. Führen Sie einen der folgenden Schritte aus, um Schlüsselwörter hinzuzufügen:

   * Geben Sie ein Schlüsselwort in das Textfeld ein und klicken Sie auf „Hinzufügen“.
   * Klicken Sie in der Tabelle für Schlüsselwortvorschläge auf ein Schlüsselwort.

1. Um ein Schlüsselwort zu entfernen, wählen Sie es aus und klicken dann auf „Entfernen“. Es wird in die Tabelle für Schlüsselwortvorschläge verschoben.

>[!NOTE]
Sie können Dateien beim Hochladen in Dynamic Media Classic Suchbegriffe hinzufügen. Klicken Sie dazu im Dialogfeld „Upload-Auftragsoptionen“ auf „Zusätzliche Metadaten“ und geben Sie die Schlüsselwörter ein. Siehe [Optionen für das Hochladen](uploading-files.md#upload_options).

## Importieren von Metadaten {#import-metadata}

Statt Metadaten für jedes Asset manuell einzugeben, können Sie Metadaten aus einer tabulatorgetrennten Datei oder XML-Datei für mehrere Assets gleichzeitig importieren. Die Metadaten in eine tabulatorgetrennte Datei oder XML-Datei einzugeben und diese Datei dann zu importieren, ist weniger zeitaufwendig, als die Metadaten für einzelne Assets manuell einzugeben. Geben Sie in der ersten Zeile der tabulatorgetrennten Datei die ID und die Namen der gewünschten Metadatenfelder ein. Geben Sie in die nächsten Zeilen jeweils einen Asset-ID-Namen gefolgt von den Metadaten-Werten ein. Felder, die nicht in der tabulatorgetrennten Datei oder in der XML-Datei enthalten sind, werden nicht geändert. Wenn Sie Metadaten aus einer XML-Datei importieren möchten, müssen Sie sicherstellen, dass diese DTD-konform ist.

>[!NOTE]
Sie können eine Vorlage zum Eingeben von Metadaten erstellen, damit diese ordnungsgemäß in das Scene7 Publishing System importiert werden. Nach dem Erstellen der Vorlage können Sie sie zum Eingeben der Metadaten verwenden. Siehe [Erstellen einer Vorlage zum Eingeben und Hochladen von Metadaten](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

Weitere Informationen zu standardisierten Eigenschaften finden Sie unter: https://www.adobe.com/devnet/xmp.html

1. Wählen Sie im Durchsuchenbedienfeld die Bilder aus, denen Sie Metadaten aus der tabulatorgetrennten oder XML-Datei hinzufügen möchten.
1. Wählen Sie **Datei** &gt; **Metadaten importieren**.
1. Klicken Sie im Dialogfeld **Metadaten hochladen** auf **Durchsuchen**.
1. Wählen Sie im Dialogfeld **Hochzuladende Dateien auswählen** die tabulatorgetrennte Datei bzw. die XML-Datei mit den Metadaten aus.
1. Geben Sie einen Auftragsnamen ein.
1. Klicken Sie auf **Hochladen**.

**Identifizieren von verschiedenen Metadaten-Typen beim Import**

Beachten Sie Folgendes, wenn verschiedene Metadaten-Typen für den Import identifiziert werden:

* Benutzerdefinierte Felder werden anhand des Namens identifiziert, der unter „Einstellungen“ &gt; „Anwendungseinstellungen“ &gt; „Metadaten“ &gt; „Benutzerdefinierte Felder“ angegeben wurde. Lassen Sie sich mit der Funktion „Datei generieren“ eine Liste mit allen definierten UDFs im richtigen Importformat anzeigen.
* Bei den XMP-Metadaten-Eigenschaften muss das entsprechende XMP-Präfix vor dem Namen (der Eigenschaft) stehen. Präfix und Name werden durch einen Doppelpunkt voneinander getrennt. Das XMP-Präfix finden Sie unter „Einstellungen &gt; „Anwendungseinstellungen“ &gt; „Metadaten“ &gt; „Schema-Editor“. Die technischen Namen finden Sie in der Dokumentation zum jeweiligen XMP-Schema. Beachten Sie, dass XMP-Eigenschaftsnamen nicht bei der Funktion „Datei generieren“ angezeigt werden.
* Bei den Metadaten-Eigenschaften muss das entsprechende Präfix vor dem Namen (der Eigenschaft) stehen. Präfix und Name werden durch einen Doppelpunkt voneinander getrennt. Das Präfix und die Eigenschaftsnamen werden im Metadaten-Schema-Editor definiert. Beachten Sie, dass die Eigenschaftsnamen von Metadaten-Schematas nicht bei der Funktion „Datei generieren“ angezeigt werden.

Beispiel: Die XMP-Eigenschaft für Schlüsselwörter ist das XMP-Schema „Dublin Core“ mit dem Präfix „dc“ und „subject“ ist der technische XMP-Name. Das Präfix und der technische XMP-Name werden zu „dc:subject“ kombiniert und bilden den Namen der Eigenschaft. Im Importformat der XML-Metadaten muss der Eigenschaftsname „dc:subject“ lauten. Im tabulatorgetrennten Importformat muss es die Spaltenüberschrift sein.

**Importieren von Schlüsselwörtern**

Schlüsselwörter lassen sich als Komma getrennte Liste importieren. Wenn ein Komma in einem der einzelnen Werte angezeigt wird, muss ihm ein umgekehrter Schrägstrich (\) (Backslash) vorangestellt werden. Ein umgekehrter Schrägstrich muss mit einem doppelten umgekehrten Schrägstrich (\\) angegeben werden.

Beispiel: Eine Metadaten-Importdatei mit dem Wert „Hello\, World!,back\\slash,foo“ für „dc: subject“ legt drei XMP-Schlüsselwörter für das Asset fest: „Hello, World!“, „back\slash“ und „foo“.

**Importieren von XMP- und Metadaten-Schema-XMP-Dateien**

Der XML-Import akzeptiert nur gültige XML. Wenn Sie XMP- oder Metadaten-Schema-Felder importieren, wird das Namespace-Präfix hinzugefügt und wie ein XMP-Namespace behandelt. Dieser Namespace muss (z. B. auf oberster Tag-Ebene) angegeben werden.

Beispiel:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

**Importieren von XMP und tabulatorgetrennten Metadata-Schema-Metadata-Dateien**

Das Präfix muss in der entsprechenden Spaltenüberschrift im Importfeld hinzugefügt werden.

## Importieren von Metadaten (über FTP) {#import-metadata-via-ftp}

Sie können Metadaten für mehrere Dateien importieren, indem Sie die Metadaten in eine tabulatorgetrennte Datei oder in eine XML-Datei eingeben und im Anzeigebereich „Hochladen (über FTP)“ die Option „Metadaten-Dateien verarbeiten“ auswählen.

Stellen Sie sicher, dass die Daten in der tabulatorgetrennten Datei oder in der XML-Datei im korrekten Format vorliegen. Geben Sie in die erste Zeile das ID-Feld, gefolgt von den Namen der Metadaten-Felder ein, die geändert werden sollen. Geben Sie in die nächsten Zeilen jeweils einen Asset-ID-Namen gefolgt von den Metadaten-Werten ein. Felder, die nicht in der tabulatorgetrennten Datei oder in der XML-Datei enthalten sind, werden nicht geändert.

Klicken Sie in der Symbolleiste für globale Navigation auf die Schaltfläche „Hochladen“ und wählen Sie im Anzeigebereich „Aufträge“ die Registerkarte „Über FTP“ aus, um die Metadaten zu importieren. Klicken Sie dann auf „Auftragsoptionen“. Wählen Sie im Dialogfeld „Upload-Auftragsoptionen“ die Option „Metadaten-Dateien verarbeiten“.

## Stapel-Umbenennung von IDs mit Metadaten {#batch-rename-ids-using-metadata}

Sie können Scene7 Publishing System-IDs unter Verwendung von Metadaten umbenennen, die aus einer tabulatorgetrennten Textdatei oder einer XML-Datei importiert wurden. Die importierten Metadaten werden nur auf die in der Metadatendatei selbst angegebenen Bilder angewendet. Dabei ist es unerheblich, ob Bilder im Durchsuchenbedienfeld ausgewählt sind oder nicht.

To rename an image’s Scene7 Publishing System ID, add a column labeled *newipsid* to the tab-delimited file, or add a field called* new_vc_objectname* to the XML data.

Beispiel:

| ipsid | newipsid |
|--- |--- |
| testjacket_1 | Jacket_test_1 |
| testjacket_blue | Jacket_test_2 |


Im Auftragsprotokoll für den Metadatenauftrag wird festgehalten, welche IDs erfolgreich umbenannt wurden und welche nicht.

## Erstellen einer Vorlage zum Eingeben und Hochladen von Metadaten {#create-a-template-for-entering-metadata-to-upload}

Dynamic Media Classic bietet einen Befehl zum Erstellen einer Vorlage zum Aufzeichnen von Metadaten. Mit dieser Vorlage können Sie sicherstellen, dass die Metadaten im richtigen Format eingegeben und fehlerlos in das Scene7 Publishing System importiert werden. Gehen Sie folgendermaßen vor, um eine Vorlage zum Eingeben und Importieren von Metadaten in das Scene7 Publishing System zu erstellen:

1. Wählen Sie Bildassets mit Metadatenfeldern aus, die Sie in der Vorlage verwenden möchten.
1. Wählen Sie „Datei“ &gt; „Metadaten importieren“.
1. Wählen Sie ein Bild vom Typ „Asset-Eigenschaften“ aus.
1. Wählen Sie im Menü „Datei“ unter „Erstellen“ die Option „Tabulatorgetrennte Vorlage“, „XML-Metadaten des Assets“ oder „XML-DTD“.
1. Klicken Sie auf „Erstellen“.
1. Kopieren Sie die Daten im daraufhin angezeigten Dialogfeld. Verwenden Sie diese Daten, um die Vorlage zu erstellen.

## Arbeiten mit Metadaten-Schemata {#working-with-metadata-schemas}

Ein Unternehmensadministrator kann eine Liste aller verfügbaren Schemata anzeigen. Öffnen Sie „Anwendungseinstellungen“ &gt; „Metadaten¬&gt; „Metadaten-Schema“.

Zunächst werden die Listen der globalen Standardschemata wie XMP ausgeblendet. Sie können mithilfe des Kontrollkästchens unten in der Liste angezeigt werden.

Der Unternehmensadministrator kann ein neues benutzerdefiniertes Schema erstellen oder ein vorhandenes benutzerdefiniertes Schema bearbeiten.

Sie können den Metadaten-Schema-Editor verwenden, um die folgenden Aktionen ausführen:

| Aktion | Beschreibung |
|--- |--- |
| Hinzufügen | Fügt eine neue Eigenschaft zum Schema hinzu. Ein modaler Dialog erfasst die Informationen: ID, Beschriftung, Struktur und Datentyp. |
| Auswahlwert hinzufügen | Fügt einer Eigenschaft mit „Offene Auswahl“ oder „Geschlossene Auswahl“ eine neue Auswahloption hinzu. Alle Auswahlwerte haben den gleichen Typ. Sie müssen die Eigenschaft auswählen, um die Schaltfläche zu aktivieren. |
| Bearbeiten | Bearbeiten der Beschriftung einer Eigenschaft oder eines Auswahlwertes. Sie können nur die Beschriftung und ID ändern, nicht aber die Typinformationen. |
| Nach oben verschieben/Nach unten verschieben | Die Reihenfolge im Schema wird in der Benutzeroberfläche übernommen. Um die Reihenfolge zu ändern, wählen Sie eine Eigenschaft oder einen Auswahlwert aus und verschieben diese mit den Schaltflächen. Ziehen und Ablegen wird derzeit nicht unterstützt. |
| Löschen | Löscht eine Eigenschaft oder einen Auswahlwert aus dem Schema. Damit werden keine Werte aus dem XMP-Block oder der Datenbank gelöscht. Die Eigenschaft ist nicht mehr für Metadaten-Ansichten verfügbar und wird aus der Asset-Detailansicht entfernt. Wenn die Eigenschaft auf dem Metadatenserver veröffentlicht wurde, erzwingen Sie eine Veröffentlichung, um die Daten von dem öffentlich zugänglichen Metadaten-Server zu entfernen. |

Das System generiert automatisch ein benutzerdefiniertes Schema für benutzerdefinierte Felder mit dem Präfix „s7udf“. Dies sind die vorhandenen benutzerdefinierten Felder, die in ihrem eigenen Einstellungsbereich bearbeitet werden.

>[!NOTE]
Von Änderungen am Schema bleiben die Asset-Metadaten unberührt. Sie werden jedoch nicht für alle SPS- und Metadatenserver-Funktionen angezeigt und nach dem Ändern kann darauf nicht mehr zugegriffen werden. Ähnlich verhält es sich, wenn Metadaten für ein Asset vorhanden sind. Dann werden durch die Erstellung des passenden Schemas die Metadaten in SPS und auf dem Metadatenserver verwendbar.

Der Metadaten-Schema-Editor bietet eine grafische Möglichkeit, um ein unternehmenseigenes Schema in SPS hinzuzufügen oder zu bearbeiten. Ein Schema wird durch ein Präfix, einen Namespace und eine Liste von Eigenschaften definiert.

* Name

   Name der Benutzeroberfläche für das Schema. Wird verwendet, um die Eigenschaften in den Metadaten-Ansichten und bei der erweiterten Suche zu identifizieren. Vergleichbar mit XMP-Abschnitten wie Basic, IPTC, PDF.

* Präfix

   Technischer, eindeutiger Identifikator für das Schema. Beschränkt auf die Buchstaben a-z und A-Z. Das Präfix ist nicht in der Benutzeroberfläche von SPS sichtbar, wird aber verwendet, wenn die Metadaten für ein Asset im XMP-Block und in der Datenbank gespeichert werden. Das Präfix wird verwendet, um Metadaten-Felder bei Metadaten-Suchanfragen beim Metadatenserver oder beim Importieren eindeutig zu identifizieren.

* Namespace

   Technischer eindeutiger Bezeichner für das Schema, normalerweise eine URL im Formular `https://your.company.com/name/version/`. Weitere Informationen finden Sie in der Liste der Standardschemata für Beispiele. Der Namespace wird nicht in der Benutzeroberfläche von SPS angezeigt, jedoch verwendet, um Metadaten im XMP-Block zu speichern.

* Beschreibung

   Freie Formularbeschreibung des Schemas.

>[!NOTE]
Präfix und Namespace können nicht bearbeitet werden. Um diese Eigenschaften zu ändern, müssen Sie das Schema löschen und neu erstellen.

Eigenschaften beschreiben die Metadaten, die mit diesem Schema im XMP-Block gespeichert werden können. Eine Eigenschaft besteht aus:

| Eigenschaft | Beschreibung |
|--- |--- |
| ID | Technischer Identifikator für diese Eigenschaft. Die ID ist in der SPS-Benutzeroberfläche nicht sichtbar, wird aber verwendet, wenn die Metadaten für ein Asset im XMP-Block und in der Datenbank gespeichert werden. Die ID wird verwendet, um Suchanfragen auf dem Metadatenserver zu erstellen. Die ID hat einige Einschränkungen wie folgende: <ul><li>Keine Leerzeichen</li><li>Kein „.“, „:“, „$“</li><li>Keine Zahl als erstes Zeichen</li><li>Es empfiehlt sich, a-z oder A-Z als erstes Zeichen zu verwenden</li></ul> <br>Sobald erstellt, kann die ID nicht geändert werden. |
| Beschriftung | Name dieser Eigenschaft in der Benutzeroberfläche. |
| Struktur | Legt die Art der Eigenschaft zusammen mit dem Datentyp fest. Eine Struktur kann sein:<ul><li>Einfacher Typ: Einzelwert des Datentyps</li><li>Sequenz: eine Liste von Werten desselben Datentyps</li><li>Offene Auswahl: Wählen Sie ein Element aus einer zuvor festgelegten Liste von Werten aus oder geben Sie einen beliebigen Text ein. Kann nur vom Datentyp „Zeichenfolge“ oder „Integer“ sein.</li><li>Geschlossene Auswahl: Wählen Sie ein Element aus einer zuvor festgelegten Liste von Werten aus (ein Popup- oder ein Kombinationsfeld).</li></ul> |
| Datentyp | Wählen Sie aus den verfügbaren Typen aus: <ul><li>Zeichenfolge</li><li>Integer</li><li>Float</li><li>Ja/Nein (Boolescher Wert)</li><li>Datum</li></ul> |


Wenn die Eigenschaft als Struktur eine offene oder geschlossene Auswahl verwendet, müssen Sie mindestens einen Auswahlwert zur Verfügung stellen. Eine offene Auswahl kann geändert werden. Eine geschlossene Auswahl kann nicht geändert werden. Alle Auswahlwerte haben den Datentyp der Eigenschaft.

| Eigenschaft | Beschreibung |
|--- |--- |
| ID | Technischer Identifikator für diesen Wert. Die ID ist in der SPS-Benutzeroberfläche nicht sichtbar, wird aber verwendet, wenn die Metadaten für ein Asset im XMP-Block und in der Datenbank gespeichert werden. Die ID wird für Suchanfragen auf dem Metadatenserver verwendet. Die ID darf keine Leerzeichen enthalten. Sobald erstellt, kann die ID nicht geändert werden. |
| Beschriftung | Name dieses Wertes in der Benutzeroberfläche. |

>[!MORELIKETHIS]
* [Viewer-Vorgaben](application-setup.md#viewer_presets)
* [Metadaten-Vorgaben](application-setup.md#metadata_presets)

