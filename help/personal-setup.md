---
title: Persönliche Einstellungen
description: Alle Benutzer können die Einstellungen im Bildschirm "Persönliche Einstellungen"von Adobe Dynamic Media Classic ändern.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '822'
ht-degree: 25%

---

# Persönliche Einstellungen {#personal-setup}

Die Einstellungen im Anzeigebereich „Persönliche Einstellungen“ können von allen Benutzern geändert werden. Um den Bildschirm &quot;Persönliche Einstellungen&quot;zu öffnen, gehen Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Persönliche Einstellungen]**.

>[!NOTE]
>
>Im Bildschirm Persönliche Einstellungen wird angezeigt, welche Benutzerrolle Sie in Adobe Dynamic Media Classic haben: Unternehmensadministrator, Administrator oder Benutzer.

Die persönlichen Einstellungen steuern das Standardverhalten des Durchsuchenbedienfelds, den E-Mail-Empfang und die Kennworteinstellungen. Denken Sie daran, **[!UICONTROL Speichern]** auszuwählen, nachdem Sie diese Einstellungen geändert haben.

## Eigene Konto-Informationen

Identifiziert Ihren Kontonamen, Namen, Benutzernamen (E-Mail-Adresse) und zugewiesene Benutzerrolle.

## Desktop

* **Image-Cache löschen** : Entfernt alle Adobe-Dynamic Media-zwischengespeicherten Bilddateien von Ihrem Computer.
* **Asset-Cache löschen** : Entfernt alle Adoben, in denen Dynamic Media Asset-Dateien von Ihrem Computer zwischenspeichert.

Sie können den Bild- und Asset-Cache nicht nur mit dem Desktop-Programm löschen, sondern auch den Cache direkt aus dem Dateisystem löschen. Navigieren Sie je nach Betriebssystem zu Folgendem:

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**So installieren Sie die Adobe Dynamic Media Creative Suite Extension:**

1. Navigieren Sie in Adobe Dynamic Media Classic in der Symbolleiste zu **[!UICONTROL Setup]** > **[!UICONTROL Persönliche Einstellungen]** und wählen Sie unter &quot;Creative Suite Extension&quot;die Option **[!UICONTROL Jetzt herunterladen]** aus, um die Datei `s7csxs.zxp` herunterzuladen.
1. Wählen Sie die Links **[!UICONTROL Installation]** und **[!UICONTROL Systemanforderungen]** aus, um weitere Informationen zur Erweiterung zu erhalten.

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
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014 > mac64.</li><li>Select libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator’s package contents folder, right-select on the Adobe illustrator CC 2014 icon and select Show Package Contents from context menu).</li><li>Return to the same libraries folder, select `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## Browser

* **[!UICONTROL Größe der Miniaturansichten]**  - Bestimmt die Standardgröße der Miniaturansichten in der Rasteransicht im Durchsuchenbedienfeld.
* **[!UICONTROL Asset-Standardbibliothek-Ansicht]**  - Bestimmt, ob die Assets in der Asset-Bibliothek für Buildsets als Miniaturansichten oder nach Namen angezeigt werden. Wenn Sie mit einer Vielzahl von Assets in der Asset-Bibliothek arbeiten, können Sie diese Assets dem Namen nach geordnet anzeigen. Wenn Sie zum Beispiel einen großen E-Katalog mit vielen PDF-Dateien erstellen, können Sie die Assets dem Namen nach geordnet anzeigen, damit die Liste kürzer wird.
* **[!UICONTROL Standardsortierungsreihenfolge für Durchsuchen]**  - Bestimmt die Reihenfolge, in der Assets standardmäßig im Durchsuchenbedienfeld angezeigt werden. Im Menü können Sie ein Sortierungskriterium auswählen und sich zwischen aufsteigender und absteigender Sortierung entscheiden.
* **[!UICONTROL Standard-Durchsuchspeicherort]**  - Hier können Sie den Durchsuchspeicherort auf den Standard-, den zuletzt durchsuchten Ordner oder auf einen bestimmten Speicherort festlegen, zu dem Sie navigieren und ihn identifizieren. Außerdem können Sie festlegen, dass die Dateien und Ordner an der Suchposition in absteigender oder aufsteigender Reihenfolge angezeigt werden.
* **[!UICONTROL Standardmäßige Durchsuchen-Ansicht]**  - Bestimmt, ob die Rasteransicht oder Listenansicht die Standardansicht ist, die Sie beim ersten Öffnen des Bedienfelds &quot;Durchsuchen&quot;sehen.
* **[!UICONTROL Startbildschirm]**  - Bestimmt, ob Begrüßungsbildschirme einschließlich des Begrüßungsbildschirms angezeigt werden.
* **[!UICONTROL QuickInfos anzeigen]**  - Legt fest, ob QuickInfos angezeigt werden, wenn Sie den Mauszeiger über Schaltflächen, Menüs und Navigationslinks bewegen. QuickInfos beschreiben Elemente der Benutzeroberfläche auf dem Bildschirm.
* **[!UICONTROL Hintergrund]**  - Zeigt eine Schachbrettebene hinter Bildern an, sodass Sie die transparenten Bereiche eines Bildes mit einem Alphakanal leicht sehen können.
* **[!UICONTROL Dateigröße anzeigen]**  - Zeigt die Dateigröße eines Assets beim Durchsuchen an.
* **[!UICONTROL Benutzerdefinierte Felder in Suche einschließen]**  - Um die Systemleistung für die meisten von Ihnen ausgeführten Metadaten-Suchen zu verbessern, deaktivieren Sie (Standard).

   Wenn für die meisten Ihrer Metadaten-Suchen die Einbeziehung benutzerdefinierter Felder hilfreich ist, können Sie diese Option aktivieren. Alternativ bietet Ihnen die erweiterte Suche eine zielgerichtetere und schnellere Suche als bei der Verwendung benutzerdefinierter Felder.

   Siehe [Durchführen einer erweiterten Suche](searching-assets.md#conducting_an_advanced_search).

   Siehe auch [Benutzerdefinierte Felder](application-setup.md#user_defined_fields).

* **[!UICONTROL Grundlegender Suchtyp]**  - Sie können aus zwei Optionen auswählen:  **** Enthält die vollständige Zeichenfolge für den angegebenen Wert.  **** StartsWith Suchvorgänge vom Anfang der Zeichenfolge und gibt Ergebnisse schneller zurück als  **[!UICONTROL Contains]**. Jede der Optionen setzt die Standardeinstellung außer Kraft, die vom Administrator unter **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Programmeinstellungen]** festgelegt wurde.
* **[!UICONTROL Befehlseingabe anzeigen]**  - Wählen Sie diese Option aus, um die Anzeige von Befehlsanforderungen an den Server zu aktivieren. Deaktivieren Sie diese Option, um sie zu deaktivieren.
* **[!UICONTROL Dialogfeld während Export anzeigen]**  - Wählen Sie diese Option aus, um während eines Exports ein Popup-Dialogfeld anzuzeigen. Wenn Sie diese Option deaktivieren (deaktivieren), können Sie weiterhin zur Seite &quot;Aufträge&quot;wechseln, um die Ergebnisse Ihres Exports abzurufen.

## E-Mail an Freunde senden

* **[!UICONTROL E-Mail-Optionen]**  - Wählen Sie aus, wie Adobe Dynamic Media Classic Sie per E-Mail informieren soll, wenn Upload- und Veröffentlichungsaufträge abgeschlossen sind. Sie können beispielsweise festlegen, dass Sie nur über den Abschluss von Aufträgen informiert werden, wenn zuvor Warnungen und Fehlermeldungen aufgetreten sind.
* **[!UICONTROL E-Mail-Umfang]**  - Bestimmt, ob Sie die gesamte Auftrags-E-Mail für Ihr Unternehmen erhalten oder nur E-Mails zu Upload- und Veröffentlichungsaufträgen erhalten, die Sie initiieren.
* **[!UICONTROL E-Mail-Typen]**  - Bestimmt, ob Sie informiert werden, wenn Upload-Aufträge und Veröffentlichungsaufträge abgeschlossen sind.

## Sprache

* **[!UICONTROL Bevorzugte Sprache]**  - Bestimmt die Sprache, die Sie für die Benutzeroberfläche verwenden möchten.

## Kennwort

* **[!UICONTROL Aktuelles Passwort]**  - Geben Sie das Passwort Ihres aktuellen Passworts ein.
* **[!UICONTROL Neues Kennwort]**  - Geben Sie ein neues gültiges Kennwort ein. Ihr Kennwort muss die folgenden Anforderungen erfüllen:
   * Zwischen 8 und 25 Zeichen lang sein.
   * mindestens einen Kleinbuchstaben enthalten.
   * mindestens einen Großbuchstaben enthalten.
   * mindestens eine Zahl enthalten.
   * mindestens eines der folgenden Sonderzeichen enthalten: `# $ & - _ : { }`
* **[!UICONTROL Kennwort erneut eingeben]**  - Geben Sie das neue Kennwort erneut ein, um zu bestätigen, dass Sie es korrekt eingeben.
* **[!UICONTROL Passwortablauf]**  - Bestimmt, ob Ihr Passwort als Sicherheitsmaßnahme nach 72 Tagen abläuft. Wenn Sie „Ja“ wählen, werden Sie nach 72 Tagen aufgefordert, ein neues Kennwort zu erstellen.
