---
title: Persönliche Einstellungen
seo-title: Persönliche Einstellungen
description: 'null'
seo-description: Alle Benutzer können die Einstellungen im Anzeigebereich "Persönliche Einstellungen" von Dynamic Media Classic ändern.
uuid: 29 cb 825 a-f 158-4 a 1 e -9 d 5 f -7636 ee 411 b 6 e
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/setup
discoiquuid: 6314 e 7 b 7-5 bde -4 fe 2-8674-e 4 fc 525 d 4 d 1 c
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Persönliche Einstellungen {#personal-setup}

Die Einstellungen im Anzeigebereich „Persönliche Einstellungen“ können von allen Benutzern geändert werden. Um den Anzeigebereich „Persönliche Einstellungen“ zu öffnen, wählen Sie „Einstellungen“ &gt; „Persönliche Einstellungen“.

>[!NOTE]
>
>Im Anzeigebereich „Persönliche Einstellungen“ ist die Benutzerrolle angegeben, die Ihnen im Scene7 Publishing System zugeordnet ist: „Unternehmensadministrator“, „Administrator“ oder „Benutzer“.

Die persönlichen Einstellungen steuern das Standardverhalten des Durchsuchenbedienfelds, den E-Mail-Empfang und die Kennworteinstellungen. Vergessen Sie nicht, nach dem Ändern dieser Einstellungen auf „Speichern“ zu klicken.

## Eigene Konto-Informationen

Identifiziert Ihren Kontonamen, Namen, Benutzernamen (E-Mail-Adresse) und zugewiesene Benutzerrolle.

### Desktop-Version

Um die Desktop-Version vom Scene 7 Publishing System auf Ihrem lokalen Festplattenlaufwerk zu installieren, klicken Sie auf „Jetzt installieren“. Alternativ dazu können Sie auf „Jetzt neu installieren“ klicken, um die Desktop-Version erneut zu installieren.

### Illustrator-Zusatzmodul für Web-to-Print

Auf Computern, die Windows 7 oder 8 ausführen, müssen Sie über Administratorrechte verfügen und als Administrator angemeldet sein, um das Adobe Illustrator-Zusatzmodul für Web-to-Print zu installieren. Das Zusatzmodul ist nach der Installation in Adobe Illustrator verfügbar.

Das Zusatzmodul wird von folgenden Adobe Illustrator-Versionen unterstützt:

* Adobe Illustrator 18 in Adobe Creative Cloud 2014
* Adobe Illustrator 17 in Adobe Creative Cloud
* Adobe Illustrator 16 in Adobe Creative Suite 6

Die folgenden Adobe Illustrator-Plattformen werden unterstützt:

* Apple Mac OS X 10.7 oder höher
* Windows 8 32-Bit und 64-Bit
* Windows 7 32-Bit und 64-Bit
* Windows XP 32-Bit und 64-Bit (für Adobe Illustrator 16 in Adobe Creative Suite 6)

Siehe auch [Vorlagen für Veröffentlichungen](quick-start-template-publishing.md)

## So installieren Sie das Zusatzmodul auf Ihrer lokalen Festplatte

1. Klicken Sie im Scene7 Publishing System auf der Seite „Persönliche Einstellungen“ unter dem Illustrator-Zusatzmodul für Web-to-Print auf **Jetzt herunterladen**, um die Datei **Illustrator Plug-in for Web-to-Print.zip** herunterzuladen.
1. Entpacken Sie die ZIP-Datei in einen temporären Ordner.

   Im Stammverzeichnis der entpackten ZIP-Datei ist eine Readme-Datei enthalten, in der Sie zusätzliche Informationen zum Zusatzmodul finden.

1. Führen Sie je nach installiertem Betriebssystem einen der folgenden Schritte durch:

### Windows

| Bei der Ausführung von | Schritte |
|--- |--- |
| Adobe Illustrator 18 in Adobe Creative Cloud 2014 | <ul><li>Klicken Sie im Stammverzeichnis des entpackten Ordners auf CC-2014.</li><li>Je nachdem, welche Adobe Illustrator-Version Sie verwenden, klicken Sie auf win32 oder win64.</li><li>Klicken Sie auf libraries &gt; flame und kopieren Sie die Datei `aflame.dll` in den ausführbaren Adobe Illustrator-Ordner. Beispiel, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Hinweis**: Dieser Beispielpfad bezieht sich auf den 64-Bit-Speicherort. der 32-Bit-Speicherort kann stattdessen unter Programme (x 86) fallen. <br/><ul><li>Kehren Sie zum selben Ordner libraries zurück, klicken Sie auf flamingo und kopieren Sie die Datei `aflamingo.dll` in denselben ausführbaren Adobe Illustrator-Ordner, den Sie im vorherigen Schritt verwendet haben. </li><li>Je nachdem, welchen Ordner Sie in Schritt 2 ausgewählt haben, kehren Sie zum win32- oder win64-Ordner zurück und kopieren Sie die Datei `AdobeS7FXGFileFormat.aip` in den Adobe Illustrator-Ordner für Zusatzmodule. Beispiel, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Hinweis**: Dieser Beispielpfad bezieht sich auf den 64-Bit-Speicherort. der 32-Bit-Speicherort kann stattdessen unter Programme (x 86) fallen. |
| Adobe Illustrator 17 in Adobe Creative Cloud | <ul><li>Klicken Sie im Stammverzeichnis des entpackten Ordners auf CC. </li><li>Je nachdem, welche Adobe Illustrator-Version Sie verwenden, klicken Sie auf win32 oder win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. Beispiel, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Hinweis**: Dieser Beispielpfad bezieht sich auf den 64-Bit-Speicherort. der 32-Bit-Speicherort kann stattdessen unter Programme (x 86) fallen. |
| Adobe Illustrator 16 in Adobe Creative Suite 6 | <ul><li>Klicken Sie im Stammverzeichnis des entpackten Ordners auf 6.0. </li><li>Je nachdem, welche Adobe Illustrator-Version Sie verwenden, klicken Sie auf win32 oder win64. </li><li>Kopieren Sie die Datei AdobeS7FXGFileFormat.aip in den Adobe Illustrator-Ordner für Zusatzmodule. Beispiel, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Hinweis**: Dieser Beispielpfad bezieht sich auf den 64-Bit-Speicherort. der 32-Bit-Speicherort kann stattdessen unter Programme (x 86) fallen. |

### Mac

| Bei der Ausführung von | Schritte |
|--- |--- |
| Adobe Illustrator 18 in Adobe Creative Cloud 2014 | <ul><li>Klicken Sie im Stammverzeichnis des entpackten Ordners auf CC-64 &gt; mac64.</li><li>Klicken Sie auf libraries &gt; flame und kopieren Sie den Ordner `aflame.framework` in den Adobe Illustrator-Ordner für Paketinhalte. Beispiel, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (Um den Adobe Illustrator-Ordner für Paketinhalte zu öffnen, klicken Sie mit der rechten Maustaste auf das Symbol Adobe Illustrator CC 2014 und anschließend im Kontextmenü auf Paketinhalt anzeigen.)</li><li>Kehren Sie zum selben Ordner libraries zurück, klicken Sie auf `flamingo` und kopieren Sie den Ordner `aflamingo.framework` in denselben Adobe Illustrator-Ordner für Paketinhalte, den Sie im vorherigen Schritt verwendet haben.</li><li>Kehren Sie zum Ordner mac64 zurück, den Sie in Schritt 1 ausgewählt haben, und kopieren Sie den Ordner `AdobeS7FXGFileFormat.aip` in den Adobe Illustrator-Ordner für Zusatzmodule. Beispiel, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 17 in Adobe Creative Cloud | <ul><li>Klicken Sie im Stammverzeichnis des entpackten Ordners auf CC &gt; mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. Beispiel, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Illustrator 16 in Adobe Creative Suite 6 | <ul><li>Klicken Sie im Stammverzeichnis des entpackten Ordners auf 6.0 &gt; mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. Beispiel, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul> |

Das Zusatzmodul ist nun in Adobe Illustrator verfügbar und kann verwendet werden.

### Browser

* **Größe für Miniaturansichten**
   * Legt die Standardgröße für Miniaturansichten in der Rasteransicht im Durchsuchenbedienfeld fest.
* **Standardansicht für Asset-Bibliothek**
   * Legt fest, ob die Assets in der Asset-Bibliothek als Miniaturansichten oder als Liste von Namen angezeigt werden sollen. Wenn Sie mit einer Vielzahl von Assets in der Asset-Bibliothek arbeiten, können Sie diese Assets dem Namen nach geordnet anzeigen. Wenn Sie zum Beispiel einen großen E-Katalog mit vielen PDF-Dateien erstellen, können Sie die Assets dem Namen nach geordnet anzeigen, damit die Liste kürzer wird.
* **Standardsortierreihenfolge für das Durchsuchen**
   * Legt die Reihenfolge fest, in der Assets standardmäßig im Durchsuchenbedienfeld angezeigt werden. Im Menü können Sie ein Sortierungskriterium auswählen und sich zwischen aufsteigender und absteigender Sortierung entscheiden.
* **Standard-Speicherort für Durchsuchen**
   * Hiermit können Sie die Suchposition auf Standard, den zuletzt durchsuchten Ordner oder eine bestimmte Position festlegen, zu der Sie navigieren und sie identifizieren. Außerdem können Sie festlegen, dass die Dateien und Ordner an der Suchposition in absteigender oder aufsteigender Reihenfolge angezeigt werden.
* **Standardansicht beim Durchsuchen**
   * Legt fest, ob beim ersten Öffnen des Durchsuchenbedienfelds standardmäßig die Rasteransicht oder die Listenansicht angezeigt werden soll.
* **Darstellung von Vorschaltseiten**
   * Legt fest, ob Vorschaltseiten wie der Begrüßungsbildschirm angezeigt werden sollen.
* **QuickInfo einblenden**
   * Legt fest, ob QuickInfos angezeigt werden sollen, wenn Sie den Mauszeiger über Schaltflächen, Menüs und Navigationsverknüpfungen bewegen. QuickInfos enthalten Beschreibungen der angezeigten Elemente.
* **Schachbretthintergrund**
   * Zeigt hinter Bildern eine Ebene mit Schachbrettmuster an, sodass bei Bildern mit Alpha-Kanal die transparenten Bereiche leicht erkennbar sind.
* **Dateigröße anzeigen**
   * Zeigt beim Durchsuchen die Dateigröße eines Assets an.
* **Beim Verlassen von SPS bestätigen**
   * Zeigt ein Bestätigungsfenster an, bevor Sie das Scene7 Publishing System verlassen.
* **Ben.-def. Felder in Suche einschließen**
   * Deaktiviert (Standard), um die Systemleistung bei den meisten möglichen Metadaten-Suchen zu verbessern.

Wenn für die meisten Ihrer Metadaten-Suchen die Einbeziehung benutzerdefinierter Felder hilfreich ist, können Sie diese Option aktivieren. Alternativ bietet Ihnen die erweiterte Suche eine zielgerichtetere und schnellere Suche als bei der Verwendung benutzerdefinierter Felder.

Siehe [Durchführen einer erweiterten Suche](searching-assets.md#conducting_an_advanced_search).

Siehe auch [Benutzerdefinierte Felder](application-setup.md#user_defined_fields).

* **Einfacher Suchtyp**
   * Wählen Sie einen Standardsuchtyp, „Enthält“ oder „Beginnt mit“.
* **Media Portal-Funktionen anzeigen**
   * Wählen Sie diese Option, um auf Media Portal-Funktionen wie den Warenkorb zuzugreifen.
* **Befehlsfeedback anzeigen**
   * Zeigt Befehlsanfragen an den Server an.
* **Dialog beim Exportieren anzeigen**
   * Zeigt beim Exportieren ein Dialogfeld an. Wenn Sie die Auswahl dieser Option aufheben, können Sie trotzdem die Ergebnisse des Exports auf der Seite „Aufträge“ abrufen.

## E-Mail an Freunde senden

* **E-Mail-Optionen**
   * Geben Sie an, wie dynamisches Media Classic Sie per E-Mail benachrichtigen soll, wenn Upload- und Veröffentlichungsaufträge abgeschlossen sind. Sie können beispielsweise festlegen, dass Sie nur über den Abschluss von Aufträgen informiert werden, wenn zuvor Warnungen und Fehlermeldungen aufgetreten sind.
* **E-Mail-Umfang**
   * Legt fest, ob Sie E-Mails für alle Aufträge Ihres Unternehmens erhalten möchten oder nur für Upload-Aufträge und Veröffentlichungsaufträge, die Sie selbst gestartet haben.
* **E-Mail-Typen**
   * Legt fest, ob Sie darüber informiert werden möchten, wenn Upload-Aufträge und Veröffentlichungsaufträge abgeschlossen sind.
* **Sprache**
* **Bevorzugte Sprache**
   * Bestimmt die Sprache der Oberfläche.
* **Kennwort**
* **Neues Kennwort**
   * Geben Sie ein neues gültiges Kennwort ein. Ihr Kennwort muss die folgenden Anforderungen erfüllen:
      * Zwischen 8-25 Zeichen lang
      * Mindestens einen Kleinbuchstaben-Brief enthalten
      * Mindestens einen Großbuchstaben enthalten
      * Enthält mindestens eine Zahl
      * Enthält mindestens eines der folgenden Sonderzeichen: # $ &amp;-_: {}

* **Kennwort erneut eingeben**
   * Geben Sie das neue Kennwort zur Bestätigung erneut ein.
* **Ablaufdatum des Kennworts**
   * Legt fest, ob Ihr Kennwort aus Sicherheitsgründen nach 72 Tagen ablaufen soll. Wenn Sie „Ja“ wählen, werden Sie nach 72 Tagen aufgefordert, ein neues Kennwort zu erstellen.
