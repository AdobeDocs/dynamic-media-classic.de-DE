---
title: Persönliche Einstellungen
description: Alle Benutzer können die Einstellungen im Anzeigebereich "Persönliche Einstellungen"von Dynamic Media Classic ändern.
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
exl-id: a019f973-7647-466f-8af3-5312e9225e89
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 28%

---

# Persönliche Einstellungen {#personal-setup}

Die Einstellungen im Anzeigebereich „Persönliche Einstellungen“ können von allen Benutzern geändert werden. Um den Anzeigebereich „Persönliche Einstellungen“ zu öffnen, wählen Sie „Einstellungen“ > „Persönliche Einstellungen“.

>[!NOTE]
>
>Der Anzeigebereich &quot;Persönliche Einstellungen&quot;Liste die Benutzerrolle, die Sie in Dynamic Media Classic haben: Firma Administrator, Administrator oder User.

Die persönlichen Einstellungen steuern das Standardverhalten des Durchsuchenbedienfelds, den E-Mail-Empfang und die Kennworteinstellungen. Vergessen Sie nicht, nach dem Ändern dieser Einstellungen auf „Speichern“ zu klicken.

## Eigene Konto-Informationen

Identifiziert Ihren Kontonamen, Namen, Benutzernamen (E-Mail-Adresse) und zugewiesene Benutzerrolle.

## Desktop

* **Bildcache**  löschen: Entfernt alle Adobe-Dynamic Media-zwischengespeicherten Bilddateien von Ihrem Computer.
* **Asset-Cache löschen** : Entfernt alle Adoben, in denen Dynamic Media Asset-Dateien zwischenspeichert.

Neben dem Löschen des Bild- und Asset-Cache mit der Desktop-App können Sie den Cache auch direkt aus dem Dateisystem löschen. Navigieren Sie je nach Betriebssystem zu den folgenden Schritten:

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**So installieren Sie Adobe Dynamic Media Creative Suite Extension:**

1. Klicken Sie in Dynamic Media Classic auf der Symbolleiste auf **[!UICONTROL Setup]** > **[!UICONTROL Persönliche Einstellungen]** und klicken Sie unter &quot;Creative Suite Extension&quot;auf **[!UICONTROL Jetzt herunterladen]**, um die Datei `s7csxs.zxp` herunterzuladen.
1. Klicken Sie auf die Links **[!UICONTROL Installation]** und **[!UICONTROL Systemanforderungen]**, um weitere Informationen zur Erweiterung anzuzeigen.

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li>Click libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, click flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014 > mac64.</li><li>Click libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator’s package contents folder, right-click on the Adobe illustrator CC 2014 icon and click Show Package Contents from context menu).</li><li>Return to the same libraries folder, click `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## Browser

* **Größe**  der Miniaturansichten: Legt die Standardgröße der Miniaturansichten in der Ansicht &quot;Raster&quot;im Durchsuchenbedienfeld fest.
* **Standardmäßige Ansicht**  der Asset-Bibliothek: Legt fest, ob die Assets in der Asset-Bibliothek für Buildsätze als Miniaturansichten oder anhand des Namens angezeigt werden. Wenn Sie mit einer Vielzahl von Assets in der Asset-Bibliothek arbeiten, können Sie diese Assets dem Namen nach geordnet anzeigen. Wenn Sie zum Beispiel einen großen E-Katalog mit vielen PDF-Dateien erstellen, können Sie die Assets dem Namen nach geordnet anzeigen, damit die Liste kürzer wird.
* **Standardmäßige Sortierreihenfolge**  für Durchsuchen: Legt fest, in welcher Reihenfolge Assets standardmäßig im Durchsuchenbedienfeld angezeigt werden. Im Menü können Sie ein Sortierungskriterium auswählen und sich zwischen aufsteigender und absteigender Sortierung entscheiden.
* **Standardspeicherort**  für Durchsuchen: Hiermit können Sie den Durchsuchenspeicherort auf den Standard- oder den zuletzt durchsuchten Ordner oder auf einen bestimmten Speicherort festlegen, zu dem Sie navigieren und diesen identifizieren. Außerdem können Sie festlegen, dass die Dateien und Ordner an der Suchposition in absteigender oder aufsteigender Reihenfolge angezeigt werden.
* **Standardmäßige Durchsuchen-Ansicht** : Legt fest, ob die Ansicht der Rastereinstellungen oder der Listen die Ansicht ist, die beim ersten Öffnen des Durchsuchenbedienfelds standardmäßig angezeigt wird.
* **Startbildschirm** : Legt fest, ob Startbildschirme einschließlich des Begrüßungsbildschirms angezeigt werden.
* **QuickInfos**  anzeigen: Legt fest, ob QuickInfos angezeigt werden, wenn Sie den Mauszeiger über Schaltflächen, Menüs und Navigationslinks bewegen. QuickInfos beschreiben Elemente der Benutzeroberfläche auf dem Bildschirm.
* **Schachbretthintergrund** : Zeigt hinter Bildern eine Schachbrettebene an, sodass Sie die transparenten Bereiche eines Bildes mit einem Alpha-Kanal leicht erkennen können.
* **Dateigröße**  anzeigen: Zeigt die Dateigröße eines Assets beim Durchsuchen an.
* **UDFs in Suche**  einbeziehen - Zur Verbesserung der Systemleistung bei den meisten von Ihnen ausgeführten Metadaten-Suchen deaktivieren Sie die Option (Standard).

   Wenn für die meisten Ihrer Metadaten-Suchen die Einbeziehung benutzerdefinierter Felder hilfreich ist, können Sie diese Option aktivieren. Alternativ bietet Ihnen die erweiterte Suche eine zielgerichtetere und schnellere Suche als bei der Verwendung benutzerdefinierter Felder.

   Siehe [Durchführen einer erweiterten Suche](searching-assets.md#conducting_an_advanced_search).

   Siehe auch [Benutzerdefinierte Felder](application-setup.md#user_defined_fields).

* **Einfacher Suchtyp** : Sie können aus zwei Optionen auswählen:  **** Enthält die vollständige Zeichenfolge nach dem angegebenen Wert;  **[!UICONTROL Starts]** Entzieht Suchläufen am Anfang der Zeichenfolge und gibt Ergebnisse schneller zurück als  **[!UICONTROL Enthält]**. Bei beiden Optionen wird die Standardeinstellung außer Kraft gesetzt, die unter **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Programmeinstellungen]** vom Administrator festgelegt wurde.
* **Befehlsfeedback**  anzeigen: Wählen Sie diese Option, um die Anzeige der Befehlsanforderungen an den Server zu aktivieren. deaktivieren.
* **Dialogfeld während Export**  anzeigen: Wählen Sie diese Option, um während des Exports ein Popup-Dialogfeld anzuzeigen. Wenn Sie diese Option deaktivieren (deaktivieren), können Sie trotzdem zur Seite &quot;Aufträge&quot;wechseln, um die Ergebnisse Ihres Exports abzurufen.

## E-Mail an Freunde senden

* **E-Mail-Optionen** : Wählen Sie aus, wie Dynamic Media Classic Sie per E-Mail informieren soll, wenn Upload- und Veröffentlichungsaufträge abgeschlossen sind. Sie können beispielsweise festlegen, dass Sie nur über den Abschluss von Aufträgen informiert werden, wenn zuvor Warnungen und Fehlermeldungen aufgetreten sind.
* **E-Mail-Umfang** : Bestimmt, ob Sie für Ihre Firma die gesamte Auftrags-E-Mail oder nur eine E-Mail mit den von Ihnen initiierten Upload- und Veröffentlichungsaufträgen erhalten.
* **E-Mail-Typen** : Legt fest, ob Sie informiert werden, wenn Upload-Aufträge und Veröffentlichungsaufträge abgeschlossen sind.

## Sprache

* **Bevorzugte Sprache** : Bestimmt die Sprache, die Sie für die Benutzeroberfläche verwenden möchten.

## Kennwort

* **Aktuelles Passwort**  - Geben Sie das Passwort ein.
* **Neues Kennwort**  - Geben Sie ein neues, gültiges Kennwort ein. Ihr Kennwort muss die folgenden Anforderungen erfüllen:
   * Sie müssen zwischen 8 und 25 Zeichen lang sein.
   * Enthält mindestens einen Kleinbuchstaben.
   * Enthält mindestens einen Großbuchstaben.
   * Enthält mindestens eine Zahl.
   * enthält mindestens eines der folgenden Sonderzeichen: `# $ & - _ : { }`
* **Kennwort**  erneut eingeben - Geben Sie das neue Kennwort erneut ein, um sicherzustellen, dass Sie es korrekt eingeben.
* **Passwortablauf**  - Bestimmt, ob Ihr Passwort als Sicherheitsmaßnahme nach 72 Tagen abläuft. Wenn Sie „Ja“ wählen, werden Sie nach 72 Tagen aufgefordert, ein neues Kennwort zu erstellen.
