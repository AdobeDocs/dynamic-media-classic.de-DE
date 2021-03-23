---
title: Anzeigen, Hinzufügen und Exportieren von Metadaten
description: Erfahren Sie, wie Sie Metadaten Ansicht, Hinzufügen und Exportieren.
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
feature: Dynamic Media Classic, Asset Management, Metadaten
role: Geschäftspraktiker
translation-type: tm+mt
source-git-commit: 3def4a02eda8dc36f2811b3d4f0e870fff1994e4
workflow-type: tm+mt
source-wordcount: '2250'
ht-degree: 63%

---


# Anzeigen, Hinzufügen und Exportieren von Metadaten{#viewing-adding-and-exporting-metadata}

Sie können spezifische Informationen zu den Dateien speichern, mit denen Sie in Dynamic Media Classic arbeiten. Diese Informationen werden als *Metadaten* bezeichnet. Sie können in Dynamic Media Classic Metadaten zum Organisieren, Suchen, Filtern und Sortieren Ihrer Assets verwenden.

Metadaten werden in der Detail-Ansicht zusammen mit von Dynamic Media Classic generierten Informationen wie dem Dateierstellungsdatum, dem Veröffentlichungsdatum und Schlüsselwörtern angezeigt. Um Metadaten anzuzeigen, öffnen Sie das Asset in der Detailansicht und wählen Sie das Metadatenbedienfeld aus. Sie können Metadaten in der Detailansicht eingeben und bearbeiten.

Manche Metadaten sind direkt in eine Datei eingebettet. Wenn eine Datei diese Metadaten enthält, lädt Dynamic Media Classic sie automatisch mit der Datei hoch. Sie können Metadaten in Adobe Photoshop, InDesign, Illustrator und anderen Anwendungen in Quellelemente einbetten. Dynamic Media Classic erkennt diese Metadaten. Sie können in der Detailansicht über das Metadatenbedienfeld auch einzelnen Dateien Metadaten hinzufügen. Damit die Einheitlichkeit Asset-übergreifend gewährleistet werden kann, können Unternehmensadministratoren Metadatenvorlagen mit den zu verwendenden Metadatenfeldern erstellen.

Weitere Informationen zu eingebetteten Metadaten finden Sie unter [www.adobe.com/go/learn_s7_xmp_en](https://www.adobe.com/go/learn_s7_xmp_en).

## Anzeigen von Metadaten {#view-metadata}

Um die Metadaten eines Assets Ansicht, öffnen Sie das Asset in der Ansicht &quot;Details&quot;und tippen Sie auf das Metadatenbedienfeld. Um einen Satz von Metadatenfeldern auszuwählen, wählen Sie eine Option im Menü &quot;Metadaten-Ansicht&quot;. Dynamic Media Classic-Angebote: Diese Metadaten-Ansichten:

* **Kompakte**
AnsichtGrundlegende Liste von Werten.

* ****
IPTCValues, wie vom Internationalen Rat für Presse und Kommunikation definiert.

* ****
XMPValues, wie von der Extensible Metadata Platform definiert.

Administratoren können Metadaten-Ansichten erstellen. Diese Ansichten werden auch im Menü „Metadaten-Ansichten“ angezeigt. Weitere Informationen zum Erstellen von Metadaten-Ansichten finden Sie unter [Metadaten-Ansichten](application-setup.md#metadata_views).

## Manuelles Eingeben von Metadaten für ein Asset  {#manually-enter-metadata-for-an-asset}

1. Zeigen Sie das Asset in der Detailansicht an.
1. Öffnen Sie das Metadatenbedienfeld und führen Sie einen oder beide der folgenden Schritte aus:

   * Wählen Sie die Metadatenansicht aus, um festzustellen, welche Metadatenfelder im Bedienfeld angezeigt werden.
   * Wählen Sie einen Vorgabewert aus und klicken Sie auf „Übernehmen“, um die Metadatenfelder mit den Vorgabewerten zu füllen. Diese Vorgabewerte werden von Unternehmensadministratoren erstellt.

1. Geben Sie Werte in das Metadatenbedienfeld ein.

>[!NOTE]
>
>Um die Metadaten mehrerer Assets gleichzeitig zu bearbeiten, wählen Sie „Datei“ > „Informationen bearbeiten“. Bearbeitungen, die Sie im Fenster „Informationen bearbeiten“ an Metadaten vornehmen, werden auf alle ausgewählten Assets angewendet.

## Hinzufügen oder Bearbeiten von Schlüsselwörtern  {#add-or-edit-keywords}

Neben Metadaten können Sie Suchbegriffe verwenden, um die Suche und Verwaltung Ihrer Assets zu unterstützen.

Wenn Sie während dieser Sitzung Schlüsselwörter zu anderen Dateien hinzugefügt oder aus Ihrer Liste entfernt haben, werden Sie in der Tabelle für Schlüsselwortvorschläge angezeigt.

1. Öffnen Sie die Datei in der Detailansicht.
1. Klicken Sie auf „Schlüsselwörter“.
1. Führen Sie einen der folgenden Schritte aus, um Schlüsselwörter hinzuzufügen:

   * Geben Sie ein Schlüsselwort in das Textfeld ein und klicken Sie auf „Hinzufügen“.
   * Klicken Sie in der Tabelle für Schlüsselwortvorschläge auf ein Schlüsselwort.

1. Um ein Schlüsselwort zu entfernen, wählen Sie es aus und klicken dann auf „Entfernen“. Es wird in die Tabelle für Schlüsselwortvorschläge verschoben.

>[!NOTE]
>
>Sie können Dateien beim Hochladen in Dynamic Media Classic Suchbegriffe hinzufügen. Klicken Sie dazu im Dialogfeld „Upload-Auftragsoptionen“ auf „Zusätzliche Metadaten“ und geben Sie die Schlüsselwörter ein. Siehe [Optionen für das Hochladen](uploading-files.md#upload_options).

## Importieren von Metadaten  {#import-metadata}

Statt Metadaten für jedes Asset manuell einzugeben, können Sie Metadaten aus einer tabulatorgetrennten Datei oder XML-Datei für mehrere Assets gleichzeitig importieren. Die Metadaten in eine tabulatorgetrennte Datei oder XML-Datei einzugeben und diese Datei dann zu importieren, ist weniger zeitaufwendig, als die Metadaten für einzelne Assets manuell einzugeben. Geben Sie in der ersten Zeile der tabulatorgetrennten Datei die ID und die Namen der gewünschten Metadatenfelder ein. Geben Sie in die nächsten Zeilen jeweils einen Asset-ID-Namen gefolgt von den Metadaten-Werten ein. Felder, die nicht in der tabulatorgetrennten Datei oder in der XML-Datei enthalten sind, werden nicht geändert. Wenn Sie Metadaten aus einer XML-Datei importieren möchten, müssen Sie sicherstellen, dass diese DTD-konform ist.

>[!NOTE]
>
>Sie können eine Vorlage zum Eingeben von Metadaten erstellen, damit diese ordnungsgemäß in Dynamic Media Classic importiert werden können. Nach dem Erstellen der Vorlage können Sie sie zum Eingeben der Metadaten verwenden. Siehe [Erstellen einer Vorlage zum Eingeben und Hochladen von Metadaten](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload).

Weitere Informationen zu standardisierten Eigenschaften finden Sie unter: https://www.adobe.com/devnet/xmp.html

1. Wählen Sie im Durchsuchenbedienfeld die Bilder aus, denen Sie Metadaten aus der tabulatorgetrennten oder XML-Datei hinzufügen möchten.
1. Wählen Sie **Datei** > **Metadaten importieren**.
1. Klicken Sie im Dialogfeld **Metadaten hochladen** auf **Durchsuchen**.
1. Wählen Sie im Dialogfeld **Hochzuladende Dateien auswählen** die tabulatorgetrennte Datei bzw. die XML-Datei mit den Metadaten aus.
1. Geben Sie einen Auftragsnamen ein.
1. Klicken Sie auf **Hochladen**.

**Identifizieren von verschiedenen Metadaten-Typen beim Import**

Beachten Sie Folgendes, wenn verschiedene Metadaten-Typen für den Import identifiziert werden:

* Benutzerdefinierte Felder werden anhand ihres Namens identifiziert, der unter &quot;Einstellungen&quot;> &quot;Anwendungseinstellungen&quot;> &quot;Metadaten&quot;> &quot;Benutzerdefinierte Felder&quot;erstellt wurde. Lassen Sie sich mit der Funktion „Datei generieren“ eine Liste mit allen definierten UDFs im richtigen Importformat anzeigen.
* Bei den XMP-Metadaten-Eigenschaften muss das entsprechende XMP-Präfix vor dem Namen (der Eigenschaft) stehen. Präfix und Name werden durch einen Doppelpunkt voneinander getrennt. Das XMP-Präfix finden Sie unter „Einstellungen > „Anwendungseinstellungen“ > „Metadaten“ > „Schema-Editor“. Die technischen Namen finden Sie in der Dokumentation zum jeweiligen XMP-Schema. XMP Namen von Eigenschaften werden nicht in der Funktion Datei erstellen angezeigt.
* Bei den Metadaten-Eigenschaften muss das entsprechende Präfix vor dem Namen (der Eigenschaft) stehen. Präfix und Name werden durch einen Doppelpunkt voneinander getrennt. Das Präfix und die Eigenschaftsnamen werden im Metadaten-Schema-Editor definiert. Die Namen der Metadaten-Schema-Eigenschaften werden nicht in der Funktion &quot;Datei erstellen&quot;angezeigt.

Beispiel: Die XMP-Eigenschaft für Schlüsselwörter ist das XMP-Schema „Dublin Core“ mit dem Präfix „dc“ und „subject“ ist der technische XMP-Name. Das Präfix und der technische XMP-Name werden zu „dc:subject“ kombiniert und bilden den Namen der Eigenschaft. Im Importformat der XML-Metadaten muss der Eigenschaftsname „dc:subject“ lauten. Im tabulatorgetrennten Importformat muss es die Spaltenüberschrift sein.

**Importieren von Schlüsselwörtern**

Suchbegriffe können als kommagetrennte Liste importiert werden. Wenn ein Komma in einem der einzelnen Werte angezeigt wird, muss es mit einem umgekehrten Schrägstrich (\) versehen werden. Ein umgekehrter Schrägstrich muss mit einem doppelten umgekehrten Schrägstrich (\\) angegeben werden.

Beispiel: Eine Metadaten-Importdatei mit dem Wert „Hello\, World!,back\\slash,foo“ für „dc: subject“ legt drei XMP-Schlüsselwörter für das Asset fest: „Hello, World!“, „back\slash“ und „foo“.

**Importieren von XMP- und Metadaten-Schema-XMP-Dateien**

Der XML-Import akzeptiert nur gültige XML. Beim Importieren von Schema-Feldern XMP oder Metadaten wird das Präfix des Namensraums hinzugefügt und verhält sich hier wie ein XMP-Namensraum. Dieser Namensraum muss erklärt werden. Beispiel: im Tag der obersten Ebene.

Beispiel:

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

**Importieren von XMP und tabulatorgetrennten Metadata-Schema-Metadata-Dateien**

Das Präfix muss in der entsprechenden Spaltenüberschrift im Importfeld hinzugefügt werden.

## Importieren von Metadaten (über FTP)  {#import-metadata-via-ftp}

Sie können Metadaten für mehrere Dateien importieren, indem Sie die Metadaten in eine tabulatorgetrennte Datei oder in eine XML-Datei eingeben und im Anzeigebereich „Hochladen (über FTP)“ die Option „Metadaten-Dateien verarbeiten“ auswählen.

Stellen Sie sicher, dass die Daten in der tabulatorgetrennten Datei oder in der XML-Datei im korrekten Format vorliegen. Geben Sie in die erste Zeile das ID-Feld, gefolgt von den Namen der Metadaten-Felder ein, die geändert werden sollen. Geben Sie in die nächsten Zeilen jeweils einen Asset-ID-Namen gefolgt von den Metadaten-Werten ein. Felder, die nicht in der tabulatorgetrennten Datei oder in der XML-Datei enthalten sind, werden nicht geändert.

Klicken Sie in der Symbolleiste für globale Navigation auf die Schaltfläche &quot;Hochladen&quot;. Um die Metadaten zu importieren, wählen Sie im Anzeigebereich &quot;Aufträge&quot;die Registerkarte **[!UICONTROL Über FTP]** und klicken Sie dann auf **[!UICONTROL Auftragsoptionen]**. Wählen Sie im Dialogfeld &quot;Upload-Auftragsoptionen&quot;die Option Metadatendateien verarbeiten.

## Stapel-Umbenennung von IDs mit Metadaten {#batch-rename-ids-using-metadata}

Mithilfe von Metadaten, die aus einer tabulatorgetrennten Datei oder XML-Datei importiert wurden, können Sie Dynamic Media Classic-IDs umbenennen. Die importierten Metadaten werden nur auf die in der Metadatendatei selbst angegebenen Bilder angewendet. Dabei ist es unerheblich, ob Bilder im Durchsuchenbedienfeld ausgewählt sind oder nicht.

Um die Dynamic Media Classic-ID eines Bildes umzubenennen, fügen Sie der tabulatorgetrennten Datei eine Spalte mit der Bezeichnung *newipsid* hinzu oder fügen Sie den XML-Daten ein Feld mit der Bezeichnung* new_vc_objectname* hinzu.

Beispiel:

| ipsid | newipsid |
|--- |--- |
| testjacket_1 | Jacket_test_1 |
| testjacket_blue | Jacket_test_2 |

Das Auftragsprotokoll für den Metadatenauftrag zeigt an, welche IDs erfolgreich umbenannt wurden und welche nicht.

## Erstellen einer Vorlage zum Eingeben und Hochladen von Metadaten {#create-a-template-for-entering-metadata-to-upload}

Dynamic Media Classic-Angebote verwenden einen Befehl zum Erstellen einer Vorlage zum Aufzeichnen von Metadaten. Mithilfe der Vorlage wird sichergestellt, dass die Metadaten im richtigen Format eingegeben werden, damit sie korrekt in Dynamic Media Classic hochgeladen werden können. Gehen Sie wie folgt vor, um eine Vorlage zum Aufzeichnen und Importieren von Metadaten in Dynamic Media Classic zu erstellen:

1. Wählen Sie Bildassets mit Metadatenfeldern aus, die Sie in der Vorlage verwenden möchten.
1. Wählen Sie „Datei“ > „Metadaten importieren“.
1. Wählen Sie ein Bild vom Typ „Asset-Eigenschaften“ aus.
1. Wählen Sie im Menü „Datei“ unter „Erstellen“ die Option „Tabulatorgetrennte Vorlage“, „XML-Metadaten des Assets“ oder „XML-DTD“.
1. Klicken Sie auf „Erstellen“.
1. Kopieren Sie die Daten im daraufhin angezeigten Dialogfeld. Verwenden Sie diese Daten, um die Vorlage zu erstellen.

## Arbeiten mit Metadaten-Schemata {#working-with-metadata-schemas}

Ein Unternehmensadministrator kann eine Liste aller verfügbaren Schemata anzeigen. Öffnen Sie „Anwendungseinstellungen“ > „Metadaten¬> „Metadaten-Schema“.

Zunächst wird die Liste von Schemas wie XMP ausgeblendet. Sie können mithilfe des Kontrollkästchens unten in der Liste angezeigt werden.

Der Administrator der Firma kann ein benutzerdefiniertes Schema erstellen oder ein vorhandenes benutzerdefiniertes Schema bearbeiten.

Sie können den Metadaten-Schema-Editor verwenden, um die folgenden Aktionen ausführen:

| Aktion | Beschreibung |
|--- |--- |
| Hinzufügen | Fügt dem Schema eine Eigenschaft hinzu. In einem modalen Dialog werden die folgenden Informationen gesammelt: ID, Bezeichnung, Struktur und Datentyp. |
| Auswahlwert hinzufügen | Fügt einer Eigenschaft mit „Offene Auswahl“ oder „Geschlossene Auswahl“ eine neue Auswahloption hinzu. Alle Auswahlwerte haben den gleichen Typ. Wählen Sie die Eigenschaft selbst aus, um die Schaltfläche zu aktivieren. |
| Bearbeiten | Bearbeiten der Beschriftung einer Eigenschaft oder eines Auswahlwertes. Sie können nur die Beschriftung und ID ändern, nicht aber die Typinformationen. |
| Nach oben verschieben/Nach unten verschieben | Die Reihenfolge im Schema wird in der Benutzeroberfläche übernommen. Um die Reihenfolge zu ändern, wählen Sie eine Eigenschaft oder einen Auswahlwert aus und verschieben diese mit den Schaltflächen. Drag &amp; Drop wird derzeit nicht unterstützt. |
| Löschen | Löscht eine Eigenschaft oder einen Auswahlwert aus dem Schema. Es werden keine Werte aus dem XMP oder der Datenbank gelöscht. Die Eigenschaft ist für Metadaten-Ansichten nicht mehr verfügbar und wird aus der Ansicht &quot;Asset-Details&quot;entfernt. Wenn die Eigenschaft auf dem Metadaten-Server veröffentlicht wurde, führen Sie eine erzwungene Veröffentlichung durch, um die Daten vom öffentlich zugänglichen Metadaten-Server zu entfernen. |

Das System generiert automatisch ein benutzerdefiniertes Schema für benutzerdefinierte Felder mit dem Präfix „s7udf“. Es handelt sich um vorhandene benutzerdefinierte Felder, die in ihrem eigenen Setup-Abschnitt bearbeitet werden.

>[!NOTE]
>
>Von Änderungen am Schema bleiben die Asset-Metadaten unberührt. Sie sind jedoch nicht für alle Funktionen von Dynamic Media Classic und Metadata Server sichtbar und können nach einer Änderung nicht mehr aufgerufen werden. Wenn Metadaten für ein Asset vorhanden sind, werden die Metadaten auch bei der Erstellung des entsprechenden Schemas in Dynamic Media Classic und auf dem Metadatenserver verwendet.

Der Metadata Schema Editor Angebot eine grafische Möglichkeit, ein benutzerdefiniertes Firma-Schema in Dynamic Media Classic hinzuzufügen oder zu bearbeiten. Ein Schema wird durch ein Präfix, einen Namespace und eine Liste von Eigenschaften definiert.

* Name

   Name der Benutzeroberfläche für das Schema. Wird verwendet, um die Eigenschaften in den Metadaten-Ansichten und bei der erweiterten Suche zu identifizieren. Vergleichbar mit XMP-Abschnitten wie Basic, IPTC, PDF.

* Präfix

   Technischer, eindeutiger Identifikator für das Schema. Beschränkt auf die Buchstaben a-z und A-Z. Das Präfix ist in der Benutzeroberfläche von Dynamic Media Classic nicht sichtbar, wird aber verwendet, wenn Metadaten für ein Asset im XMP und in der Datenbank gespeichert werden. Das Präfix wird verwendet, um Metadaten-Felder bei Metadaten-Suchanfragen beim Metadatenserver oder beim Importieren eindeutig zu identifizieren.

* Namespace

   Technischer eindeutiger Bezeichner für das Schema, normalerweise eine URL im Format `https://your.company.com/name/version/`. Weitere Informationen finden Sie in der Liste der Standardschemata für Beispiele. Der Namensraum ist in der Benutzeroberfläche von Dynamic Media Classic nicht sichtbar, wird aber zum Speichern von Metadaten im XMP-Block verwendet.

* Beschreibung

   Freie Formularbeschreibung des Schemas.

>[!NOTE]
>
>Präfix und Namespace können nicht bearbeitet werden. Um diese Eigenschaften zu ändern, müssen Sie das Schema löschen und neu erstellen.

Eigenschaften beschreiben die Metadaten, die mit diesem Schema im XMP-Block gespeichert werden können. Eine Eigenschaft besteht aus:

| Eigenschaft | Beschreibung |
|--- |--- |
| ID | Technischer Identifikator für diese Eigenschaft. Die ID ist in der Benutzeroberfläche von Dynamic Media Classic nicht sichtbar, wird aber verwendet, wenn Metadaten für ein Asset im XMP und in der Datenbank gespeichert werden. Die ID wird verwendet, um Suchanfragen auf dem Metadatenserver zu erstellen. Die ID hat einige Einschränkungen wie folgende: <ul><li>Keine Leerzeichen</li><li>Kein „.“, „:“, „$“</li><li>Keine Zahl als erstes Zeichen</li><li>Es empfiehlt sich, a-z oder A-Z als erstes Zeichen zu verwenden</li></ul> <br>Sobald erstellt, kann die ID nicht geändert werden. |
| Beschriftung | Name dieser Eigenschaft in der Benutzeroberfläche. |
| Struktur | Legt die Art der Eigenschaft zusammen mit dem Datentyp fest. Eine Struktur kann sein:<ul><li>Einfacher Typ: Einzelwert des Datentyps</li><li>Sequenz: eine Liste von Werten desselben Datentyps</li><li>Offene Auswahl: Wählen Sie ein Element aus einer zuvor festgelegten Liste von Werten aus oder geben Sie einen beliebigen Text ein. Kann nur vom Datentyp „Zeichenfolge“ oder „Integer“ sein.</li><li>Geschlossene Auswahl: Wählen Sie ein Element aus einer zuvor festgelegten Liste von Werten aus (ein Popup- oder ein Kombinationsfeld).</li></ul> |
| Datentyp | Wählen Sie aus den verfügbaren Typen aus: <ul><li>Zeichenfolge</li><li>Integer</li><li>Float</li><li>Ja/Nein (Boolescher Wert)</li><li>Datum</li></ul> |


Wenn die Eigenschaft als Struktur eine offene oder geschlossene Auswahl verwendet, müssen Sie mindestens einen Auswahlwert zur Verfügung stellen. Eine offene Auswahl kann geändert werden. Eine geschlossene Auswahl kann nicht geändert werden. Alle Auswahlwerte haben den Datentyp der Eigenschaft.

| Eigenschaft | Beschreibung |
|--- |--- |
| ID | Technischer Identifikator für diesen Wert. Die ID ist in der Benutzeroberfläche von Dynamic Media Classic nicht sichtbar, wird jedoch verwendet, wenn Metadaten für ein Asset im XMP und in der Datenbank gespeichert werden. Die ID wird für Suchanfragen auf dem Metadatenserver verwendet. Die ID darf keine Leerzeichen enthalten. Sobald erstellt, kann die ID nicht geändert werden. |
| Beschriftung | Name dieses Wertes in der Benutzeroberfläche. |

>[!MORELIKETHIS]
>
>* [Viewer-Vorgaben](application-setup.md#viewer_presets)
>* [Metadaten-Vorgaben](application-setup.md#metadata_presets)

