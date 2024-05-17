---
title: Persönliche Einstellungen
description: Alle Benutzer können die Einstellungen im Bildschirm "Persönliche Einstellungen"von Adobe Dynamic Media Classic ändern.
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

Die Einstellungen im Anzeigebereich „Persönliche Einstellungen“ können von allen Benutzern geändert werden. Navigieren Sie zum Öffnen des Bildschirms Persönliche Einstellungen zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Persönliche Einstellungen]**.

>[!NOTE]
>
>Im Bildschirm Persönliche Einstellungen wird angezeigt, welche Benutzerrolle Sie in Adobe Dynamic Media Classic haben: Unternehmensadministrator, Administrator oder Benutzer.

Die persönlichen Einstellungen steuern das Standardverhalten des Bedienfelds Durchsuchen , den E-Mail-Empfang und die Kennworteinstellungen. Auswahl speichern **[!UICONTROL Speichern]** nachdem Sie diese Einstellungen geändert haben.

## Eigene Konto-Informationen

Identifiziert Ihren Kontonamen, Namen, Benutzernamen (E-Mail-Adresse) und zugewiesene Benutzerrolle.

## Desktop

* **Bild-Cache löschen**: Entfernt alle im Adobe Dynamic Media-Cache gespeicherten Bilddateien von Ihrem Computer.
* **Asset-Cache löschen**: Entfernt alle Adobe Dynamic Media-Caches von Asset-Dateien von Ihrem Computer.

Sie können den Bild- und Asset-Cache nicht nur mit dem Desktop-Programm löschen, sondern auch den Cache direkt aus dem Dateisystem löschen. Navigieren Sie je nach Betriebssystem zu Folgendem:

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**So installieren Sie die Adobe Dynamic Media Creative Suite Extension:**

1. Navigieren Sie in Adobe Dynamic Media Classic in der Symbolleiste zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Persönliche Einstellungen]** Wählen Sie unter &quot;Creative Suite Extension&quot;die Option **[!UICONTROL Jetzt herunterladen]** zum Herunterladen der `s7csxs.zxp` -Datei.
1. Wählen Sie die **[!UICONTROL Installation]** und **[!UICONTROL Systemanforderungen]** Links für weitere Informationen zur Erweiterung.

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

* **[!UICONTROL Größe der Miniaturansichten]**: Legt die Standardgröße von Miniaturbildern in der Rasteransicht im Bedienfeld &quot;Durchsuchen&quot;fest.
* **[!UICONTROL Standardansicht der Asset-Bibliothek]**: Bestimmt, ob die Assets in der Asset-Bibliothek für Buildsets als Miniaturansichten oder nach Namen angezeigt werden. Wenn Sie mit einer Vielzahl von Assets in der Asset-Bibliothek arbeiten, können Sie diese Assets dem Namen nach geordnet anzeigen. Wenn Sie zum Beispiel einen großen E-Katalog mit vielen PDF-Dateien erstellen, können Sie die Assets dem Namen nach geordnet anzeigen, damit die Liste kürzer wird.
* **[!UICONTROL Standardmäßige Sortierreihenfolge für Durchsuchen]**: Bestimmt die Reihenfolge, in der Assets standardmäßig im Bedienfeld Durchsuchen angezeigt werden. Im Menü können Sie ein Sortierungskriterium auswählen und sich zwischen aufsteigender und absteigender Sortierung entscheiden.
* **[!UICONTROL Standardspeicherort für Durchsuchen]**: Hiermit können Sie den Durchsuchspeicherort auf den Standardwert, den zuletzt durchsuchten Ordner oder auf einen bestimmten Speicherort festlegen, zu dem Sie navigieren und ihn identifizieren. Außerdem können Sie festlegen, dass die Dateien und Ordner an der Suchposition in absteigender oder aufsteigender Reihenfolge angezeigt werden.
* **[!UICONTROL Standardmäßige Durchsuchen-Ansicht]**: Bestimmt, ob die Rasteransicht oder Listenansicht die Standardansicht ist, die Sie beim ersten Öffnen des Bedienfelds &quot;Durchsuchen&quot;sehen.
* **[!UICONTROL Splash Screen Display]**: Bestimmt, ob Begrüßungsbildschirme einschließlich des Begrüßungsbildschirms angezeigt werden.
* **[!UICONTROL ToolTips anzeigen]**: Bestimmt, ob QuickInfos angezeigt werden, wenn Sie den Mauszeiger über Schaltflächen, Menüs und Navigationslinks bewegen. QuickInfos beschreiben Elemente der Benutzeroberfläche auf dem Bildschirm.
* **[!UICONTROL Hintergrund der Tafel]**: Zeigt hinter Bildern eine Schachbrettebene an, mit der Sie die transparenten Bereiche eines Bildes mit einem Alphakanal leicht sehen können.
* **[!UICONTROL Dateigröße anzeigen]**: Zeigt die Dateigröße eines Assets beim Durchsuchen an.
* **[!UICONTROL Einschließen von UDFs in die Suche]**: Um die Systemleistung für die meisten von Ihnen ausgeführten Metadatensuchen zu verbessern, deaktivieren Sie (Standard).

  Wenn für die meisten Ihrer Metadaten-Suchen die Einbeziehung benutzerdefinierter Felder hilfreich ist, können Sie diese Option aktivieren. Verwenden Sie alternativ die erweiterte Suche , um eine zielgerichtetere und schnellere Suche zu ermöglichen, als durch Einbeziehung benutzerdefinierter Felder.

  Siehe [Durchführen einer erweiterten Suche](searching-assets.md#conducting_an_advanced_search).

  Siehe auch [Benutzerdefinierte Felder](application-setup.md#user_defined_fields).

* **[!UICONTROL Einfacher Suchtyp]**: Sie können aus zwei Optionen auswählen: **[!UICONTROL Enthält]** durchsucht die vollständige Zeichenfolge nach dem angegebenen Wert; **[!UICONTROL StartsWith]** sucht am Anfang der Zeichenfolge und gibt Ergebnisse schneller zurück als **[!UICONTROL Enthält]**. Jede der Optionen setzt die in **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Programmeinstellungen]** durch den Administrator.
* **[!UICONTROL Befehls-Feedback anzeigen]**: Wählen Sie diese Option aus, um die Anzeige von Befehlsanforderungen an den Server zu aktivieren. Deaktivieren Sie diese Option, um sie zu deaktivieren.
* **[!UICONTROL Dialogfeld beim Export anzeigen]**: Wählen Sie diese Option, um während eines Exports ein Popup-Dialogfeld anzuzeigen. Wenn Sie diese Option deaktivieren (deaktivieren), können Sie weiterhin zur Seite &quot;Aufträge&quot;navigieren, um die Ergebnisse Ihres Exports abzurufen.

## E-Mail an Freunde senden

* **[!UICONTROL E-Mail-Optionen]**: Wählen Sie aus, wie Adobe Dynamic Media Classic Sie per E-Mail informieren soll, wenn Upload- und Veröffentlichungsaufträge abgeschlossen sind. Sie können beispielsweise festlegen, dass Sie nur über den Abschluss von Aufträgen informiert werden, wenn zuvor Warnungen und Fehlermeldungen aufgetreten sind.
* **[!UICONTROL E-Mail-Umfang]**: Bestimmt, ob Sie die gesamte Auftrags-E-Mail für Ihr Unternehmen erhalten oder nur E-Mails zu Upload- und Veröffentlichungsaufträgen erhalten, die Sie initiieren.
* **[!UICONTROL E-Mail-Typen]**: Bestimmt, ob Sie informiert werden, wenn Upload-Aufträge und Veröffentlichungsaufträge abgeschlossen sind.

## Sprache

* **[!UICONTROL Bevorzugte Sprache]**: Bestimmt die Sprache, die Sie für die Benutzeroberfläche verwenden möchten.

## Kennwort

* **[!UICONTROL Aktuelles Passwort]**: Geben Sie das Passwort Ihres aktuellen Passworts ein.
* **[!UICONTROL Neues Kennwort]**: Geben Sie ein neues gültiges Kennwort ein. Ihr Kennwort muss die folgenden Anforderungen erfüllen:
   * Sie muss zwischen 8 und 25 Zeichen lang sein.
   * mindestens einen Kleinbuchstaben enthalten.
   * mindestens einen Großbuchstaben enthalten.
   * mindestens eine Zahl enthalten.
   * mindestens eines der folgenden Sonderzeichen enthalten: `# $ &: _ : { }`
* **[!UICONTROL Kennwort erneut eingeben]**: Geben Sie das neue Kennwort erneut ein, um zu bestätigen, dass Sie es korrekt eingegeben haben.
* **[!UICONTROL Passwortablauf]**: Bestimmt, ob Ihr Kennwort als Sicherheitsmaßnahme nach 72 Tagen abläuft. Wenn Sie &quot;Ja&quot;ausgewählt haben, werden Sie nach 72 Tagen aufgefordert, ein Kennwort zu erstellen.
