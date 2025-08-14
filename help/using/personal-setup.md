---
title: Persönliche Einstellungen
description: Alle Benutzer können die Einstellungen auf dem Bildschirm „Personal Setup“ von Adobe Dynamic Media Classic ändern.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 19%

---

# Persönliche Einstellungen {#personal-setup}

Die Einstellungen im Anzeigebereich „Persönliche Einstellungen“ können von allen Benutzern geändert werden. Um den Bildschirm Persönliches Setup zu öffnen, gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Persönliches Setup]**.

>[!NOTE]
>
>Im Bildschirm Persönliche Einrichtung wird angezeigt, welche Benutzerrolle Sie in Adobe Dynamic Media Classic haben: Unternehmensadministrator, Administrator oder Benutzer.

Die Einstellungen Persönliche Einrichtung steuern das Standardverhalten des Durchsuchen-Panels, den Empfang von E-Mails und die Passworteinstellungen. Denken Sie daran **[!UICONTROL nach]** Änderung dieser Einstellungen auf „Speichern“ zu klicken.

## Eigene Konto-Informationen

Identifiziert Ihren Kontonamen, Namen, Benutzernamen (E-Mail-Adresse) und zugewiesene Benutzerrolle.

## Desktop

* **Clear Image Cache**: Entfernt alle in Adobe Dynamic Media zwischengespeicherten Bilddateien vom Computer.
* **Asset-Cache löschen**: Entfernt alle Adobe Dynamic Media-Caches für Asset-Dateien von Ihrem Computer.

Neben dem Löschen des Bild- und Asset-Cache mithilfe des -Desktop-Programms können Sie den Cache auch manuell direkt aus dem Dateisystem löschen. Gehen Sie je nach Betriebssystem wie folgt vor:

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**So installieren Sie die Erweiterung Adobe Dynamic Media Creative Suite:**

1. Wechseln Sie in Adobe Dynamic Media Classic in der Symbolleiste zu **[!UICONTROL Setup]** > **[!UICONTROL Persönliches Setup]** und klicken Sie unter Creative Suite-Erweiterung auf **[!UICONTROL Jetzt herunterladen]**, um die `s7csxs.zxp`-Datei herunterzuladen.
1. Wählen Sie die **[!UICONTROL Installation]** und **[!UICONTROL Systemanforderungen]** aus, um weitere Informationen zur Erweiterung zu erhalten.

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li>Select libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, select flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014 > mac64.</li><li>Select libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator's package contents folder, right-select on the Adobe illustrator CC 2014 icon and select Show Package Contents from context menu).</li><li>Return to the same libraries folder, select `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## Browser

* **[!UICONTROL Größe der Miniaturen]**: Legt die Standardgröße der Miniaturen in der Rasteransicht im Durchsuchen-Panel fest.
* **[!UICONTROL Standardansicht der Asset]** Bibliothek: Bestimmt, ob die Assets in der Asset-Bibliothek für Build-Sets als Miniaturansichten oder nach Namen angezeigt werden. Wenn Sie mit einer Vielzahl von Assets in der Asset-Bibliothek arbeiten, können Sie diese Assets dem Namen nach geordnet anzeigen. Wenn Sie zum Beispiel einen großen E-Katalog mit vielen PDF-Dateien erstellen, können Sie die Assets dem Namen nach geordnet anzeigen, damit die Liste kürzer wird.
* **[!UICONTROL Standard-Durchsuchen-Sortierreihenfolge]**: Bestimmt die Reihenfolge, in der Assets standardmäßig im Durchsuchen-Bedienfeld angezeigt werden. Im Menü können Sie ein Sortierungskriterium auswählen und sich zwischen aufsteigender und absteigender Sortierung entscheiden.
* **[!UICONTROL Standardspeicherort durchsuchen]**: Hiermit können Sie den Durchsuchen-Speicherort auf den Standardwert, den zuletzt durchsuchten Ordner oder auf einen bestimmten Speicherort festlegen, zu dem Sie navigieren und den Sie identifizieren. Außerdem können Sie festlegen, dass die Dateien und Ordner an der Suchposition in absteigender oder aufsteigender Reihenfolge angezeigt werden.
* **[!UICONTROL Standardansicht durchsuchen]**: Legt fest, ob die Rasteransicht oder Listenansicht die Standardansicht ist, die Sie sehen, wenn Sie das Bedienfeld zum ersten Mal öffnen.
* **[!UICONTROL Begrüßungsbildschirm]**: Legt fest, ob Begrüßungsbildschirme angezeigt werden, einschließlich des Begrüßungsbildschirms.
* **[!UICONTROL QuickInfos anzeigen]**: Legt fest, ob QuickInfos angezeigt werden, wenn der Mauszeiger über Schaltflächen, Menüs und Navigations-Links bewegt wird. QuickInfos beschreiben Elemente der Benutzeroberfläche auf dem Bildschirm.
* **[!UICONTROL Schachbretthintergrund]**: Zeigt eine Schachbrettschicht hinter Bildern an, sodass Sie die transparenten Bereiche eines Bildes mit einem Alphakanal leicht sehen können.
* **[!UICONTROL Dateigröße anzeigen]**: Zeigt die Dateigröße eines Assets beim Durchsuchen an.
* **[!UICONTROL UDFs in Suche einbeziehen]**: Deaktivieren Sie diese Option (Standard), um die Systemleistung für die meisten von Ihnen ausgeführten Metadatensuchen zu verbessern.

  Wenn für die meisten Ihrer Metadaten-Suchen die Einbeziehung benutzerdefinierter Felder hilfreich ist, können Sie diese Option aktivieren. Alternativ können Sie die erweiterte Suche verwenden, um eine zielgerichtetere und schnellere Suche zu ermöglichen, als wenn Sie benutzerdefinierte Felder einbeziehen.

  Siehe [Durchführen einer erweiterten Suche](searching-assets.md#conducting_an_advanced_search).

  Siehe auch [Benutzerdefinierte Felder](application-setup.md#user_defined_fields).

* **[!UICONTROL Standardsuchtyp]**: Sie können aus zwei Optionen auswählen: **[!UICONTROL Enthält]** durchsucht die vollständige Zeichenfolge nach dem angegebenen Wert; **[!UICONTROL StartsWith]** sucht am Anfang der Zeichenfolge und gibt Ergebnisse schneller als **[!UICONTROL Enthält]** zurück. Jede dieser Optionen überschreibt die Standardeinstellung, die vom Administrator unter **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Anwendungseinstellungen]** festgelegt wurde.
* **[!UICONTROL Befehlsfeedback anzeigen]**: Wählen Sie diese Option, um die Anzeige von Befehlsanforderungen an den Server einzuschalten, oder deaktivieren Sie diese Option, um sie zu deaktivieren.
* **[!UICONTROL Dialogfeld beim Exportieren anzeigen]** Wählen Sie diese Option aus, um während eines Exports ein Popup-Dialogfeld anzuzeigen. Wenn Sie diese Option deaktivieren, können Sie dennoch zur Seite Vorgänge gehen, um die Ergebnisse Ihres Exports abzurufen.

## E-Mail an Freunde senden

* **[!UICONTROL E-Mail-Optionen]**: Wählen Sie aus, wie Adobe Dynamic Media Classic Sie per E-Mail über den Abschluss von Upload- und Veröffentlichungsaufträgen informieren soll. Sie können beispielsweise festlegen, dass Sie nur über den Abschluss von Aufträgen informiert werden, wenn zuvor Warnungen und Fehlermeldungen aufgetreten sind.
* **[!UICONTROL E-Mail-Umfang]**: Bestimmt, ob Sie alle E-Mail-Vorgangs-E-Mails für Ihr Unternehmen erhalten oder nur E-Mails zu von Ihnen initiierten Upload- und Veröffentlichungsvorgängen.
* **[!UICONTROL E-Mail-Typen]**: Legt fest, ob Sie informiert werden, wenn Upload- und Veröffentlichungsaufträge abgeschlossen sind.

## Sprache

* **[!UICONTROL Bevorzugte Sprache]**: Legt die Sprache fest, die für die Benutzeroberfläche verwendet werden soll.

## Kennwort

* **[!UICONTROL Aktuelles Kennwort]**: Geben Sie das Kennwort für das aktuelle Kennwort ein.
* **[!UICONTROL Neues Kennwort]**: Geben Sie ein neues, gültiges Kennwort ein. Ihr Kennwort muss die folgenden Anforderungen erfüllen:
   * Er muss zwischen 8 und 25 Zeichen lang sein.
   * enthält mindestens einen Kleinbuchstaben.
   * Enthält mindestens einen Großbuchstaben.
   * enthält mindestens eine Zahl.
   * Mindestens eines der folgenden Sonderzeichen enthalten: `# $ &: _ : { }`
* **[!UICONTROL Kennwort erneut eingeben]**: Geben Sie das neue Kennwort erneut ein, um zu bestätigen, dass Sie es korrekt eingeben.
* **[!UICONTROL Kennwortablauf]**: Legt als Sicherheitsmaßnahme fest, ob Ihr Kennwort nach 72 Tagen abläuft. Wenn Sie Ja ausgewählt haben, werden Sie nach 72 Tagen aufgefordert, ein Kennwort zu erstellen.
