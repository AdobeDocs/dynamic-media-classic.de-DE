---
title: Adobe Dynamic Media Classic-Desktop-Programm - jetzt verfügbar
description: Erfahren Sie mehr über die Adobe Dynamic Media Classic-Desktop-Applikation.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
source-git-commit: 4e42d90747af895d27c64fa3fb5830f73e3a0a95
workflow-type: tm+mt
source-wordcount: '1937'
ht-degree: 1%

---

# Jetzt verfügbar: Adobe Dynamic Media Classic-Desktop-Programm {#dynamic-media-classic-desktop-app}

Adobe Dynamic Media Classic-Benutzer haben jetzt Zugriff auf ein neues Desktop-Programm-Erlebnis, das nicht mehr auf die Adobe Flash-Technologie im Browser angewiesen ist.

Diese neue App ist jetzt für Windows® und macOS verfügbar.

>[!IMPORTANT]
>
>Adobe empfiehlt, die neue Adobe Dynamic Media Classic-Desktop-App bis zum 1. Oktober 2020 zu installieren. Dadurch wird sichergestellt, dass Sie einen reibungslosen Übergang haben, bevor der Adobe-Flash Player am 31. Dezember 2020 eingestellt wird. Nach diesem Datum können Sie sich nicht mehr bei der Browserversion der Benutzeroberfläche von Adobe Dynamic Media Classic anmelden, die im Produkt als Adobe Dynamic Media Classic bezeichnet wird.

Siehe Häufig gestellte Fragen zum [neuen Adobe Dynamic Media Classic-Anmeldeerlebnis jetzt verfügbar.](/help/new-ui-2020.md)

## Systemanforderungen für das Adobe Dynamic Media Classic-Desktop-Programm {#system-requirements-dmc-app}

Das Adobe Dynamic Media Classic-Desktop-Programm ist mit den folgenden Betriebssystemen kompatibel:

* macOS 10.10 oder höher.
* Windows® 7 oder höher.

>[!NOTE]
>
>Aktualisierungsbenachrichtigung innerhalb der Adobe Dynamic Media Classic-Desktop-Applikation wird nicht für *Nebenversionen* generiert. Kunden, die von Fehlerbehebungen in einer kleineren Version profitieren, können ein Upgrade durchführen.

## Fehlerbehebungen in der neuesten Version (20.21.3) {#release-sept2021}

* Beschädigte Miniaturansichten für Assets, die nach einer Inaktivität im Desktop-Programm angezeigt wurden.
* Das Desktop-Programm reagiert nicht mehr, normalerweise nach den Vorgängen &quot;Set&quot;.
* Verschleierung und Sperrmodus für Anfragen automatisch aktiviert unter **[!UICONTROL Image-Serving testen]**.

   Siehe [Testen des Secure Testing Service](/help/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* Der Authentifizierungsmechanismus wurde mit Adobe Analytics aktualisiert. Relevant für neue Integrationen oder wenn einige Analytics-Variablen vom Dynamic Media Classic-Desktop-Programm aus aktualisiert werden müssen.

   Die aktualisierten Schritte finden Sie unter [Bei Adobe Analytics anmelden](/help/log-analytics.md) .

## Fehlerbehebungen in Version 20.21.2 {#minor-release}

* Bekannte Einschränkung in Version 20.21.1: Die Dropdownliste **[!UICONTROL Server]** auf dem Anmeldebildschirm war leer.
* In **[!UICONTROL Upload-Auftragsoptionen]** ist der Standardwert für die Ebenenbenennung unter **[!UICONTROL Photoshop-Optionen]** jetzt **[!UICONTROL Photoshop und der Ebenenname]**. Die Ebenen der PSD-Datei werden als getrennte Bilder hochgeladen.
   * Der frühere Standard von **[!UICONTROL Ebenenname]** benannte die Bilder nach ihrem Ebenennamen oder ihrer Ebenennummer in der PSD-Datei. Die Ebenennummer wurde verwendet, wenn die Ebenennamen in der PSD-Datei standardmäßige Photoshop-Ebenennamen waren.
   * Die neue Standardeinstellung von **[!UICONTROL Photoshop und Ebenenname]** benennt die Bilder nach der PSD-Datei, gefolgt vom Ebenennamen oder der Ebenennummer. Die Nummern der Ebenen werden verwendet, wenn es sich bei den Namen der Ebenen in der PSD-Datei um standardmäßige Photoshop-Ebenennamen handelt.
   * Da Ebenenbilder in Adobe Dynamic Media Classic jetzt eindeutige Namen haben, werden keine Änderungen an vorhandenen PSD- oder Vorlagen vorgenommen (die in den Original-PSD-Dateien gemeinsame Ebenennamen enthalten).
* Beschädigte Miniaturansichten von Assets.

## Fehlerbehebungen in Version 20.21.1 {#latest-fixes-desktop-app}

* Probleme bei der Anmeldung aufgrund eines Timeouts, was zu folgender Meldung führt: *Dieser Benutzer kann der Gruppe oder den Gruppen ohne Berechtigung zugewiesen werden. Wenden Sie sich an Ihren Administrator.*
* Viewer-Vorgaben werden bei jedem falschen Kennwortversuch dupliziert.
* Das Desktop-Programm reagiert aufgrund vieler Assets im Stammordner nicht mehr. (Behoben unter Windows®; Arbeiten wie gewünscht unter macOS.)

## Fehlerbehebungen in Version 20.20.2 {#previous-version-fixes-desktop-app}

* Keine Begrenzung der Anzahl der Dateien, die Sie über die Benutzeroberfläche des Desktop-Programms sowohl für macOS als auch für Windows® hochladen können.
* Sie müssen sich nicht von der Desktop-App abmelden, um zwischen Unternehmen zu wechseln.
* Strg+V zum Einfügen funktioniert jetzt unter Windows®.
* Wenn in Zukunft eine neue Version des Desktop-Programms veröffentlicht wird, werden Benutzer über das Desktop-Programm selbst benachrichtigt.

## Laden Sie das neueste Adobe Dynamic Media Classic-Desktop-Programm unter macOS oder Windows® herunter und installieren Sie es. {#installation-dmc-app}

Verwandte Themen:

* [Laden Sie das neueste Adobe Dynamic Media Classic-Desktop-Programm herunter und installieren Sie es still unter Mac](#install-silent-mac-dmc-app)
* [Laden Sie das neueste Adobe Dynamic Media Classic-Desktop-Programm herunter und installieren Sie es still unter Windows®](#install-silent-windows-dmc-app)

1. Deinstallieren Sie alle älteren Adobe Dynamic Media Classic Desktop-Programm-Versionen auf Ihrem System.

1. Laden Sie das neueste Installationsprogramm für das Adobe Dynamic Media Classic-Desktop-Programm herunter.

   * Die neueste Version (20.21.3) ist verfügbar unter:

      * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg)
      * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)
   * Die vorherige Version (20.21.2) ist verfügbar unter:

      * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
      * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)


<!--         * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Führen Sie je nach heruntergeladenem Installationsprogramm einen der folgenden Schritte aus.

   * **macOS**  - Ziehen Sie im Dialogfeld  **[!UICONTROL Drag &amp; Drop zum]** Installationsprogramm die  **[!UICONTROL Adobe Dynamic Media]** Classic und legen Sie sie auf  **[!UICONTROL Anwendungen]** ab.

      ![Installieren per Drag-and-Drop auf macOS](/help/assets/dragondrop-install1.png)

   * Tippen Sie im Ordner **[!UICONTROL Anwendungen]** auf das Symbol Adobe Dynamic Media Classic .
   * Tippen Sie im Dialogfeld auf **[!UICONTROL Öffnen Sie]**, um das Adobe Dynamic Media Classic-Desktop-Programm zu öffnen.

      ![Heruntergeladene App öffnen](/help/assets/open-dmclassicapp1.png)

   * **Windows**  - Führen Sie die Binärdatei des Installationsprogramms aus und befolgen Sie die Anweisungen auf dem Bildschirm, um das Desktop-Programm zu installieren.

1. Wenn Sie die Anwendung öffnen, wird die neue Adobe Dynamic Media Classic-Anmeldeseite angezeigt:

   ![Anmeldung bei Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Um sich beim Adobe Dynamic Media Classic-Desktop-Programm anzumelden, verwenden Sie dieselben Anmeldedaten wie für die Anmeldung bei Adobe Dynamic Media Classic im Browser.

   Informationen zur Verwendung von **[!UICONTROL Server]** finden Sie in der folgenden Zuordnung für die Produktionsumgebung:

   | Server | Browser-URL |
   | --- | --- |
   | NA Produktion (Nordamerika) | https://s7sps1.scene7.com/ |
   | EMEA-Produktion (Europa, Naher Osten und Afrika) | https://s7sps3.scene7.com/ |
   | APAC-Produktion (Asien-Pazifik) | https://s7sps5.scene7.com/ |

1. Beachten Sie nach der Anmeldung die bekannte Benutzeroberfläche des Browsers. Sie können die tägliche Adobe der Dynamic Media Classic-Aktivität wie gewohnt im Desktop-Programm fortsetzen.

## Laden Sie die neueste Adobe Dynamic Media Classic-Desktop-App unter macOS herunter und installieren Sie *silent*. {#install-silent-mac-dmc-app}

Verwandte Themen:

* [Laden Sie das neueste Adobe Dynamic Media Classic-Desktop-Programm unter Mac oder Windows® herunter und installieren Sie es.](#installation-dmc-app)
* [Laden Sie das neueste Adobe Dynamic Media Classic-Desktop-Programm herunter und installieren Sie es still unter Windows®](#install-silent-windows-dmc-app)

So laden Sie die neueste Adobe Dynamic Media Classic Desktop App unter macOS herunter und installieren Sie *silent*:

1. Deinstallieren Sie alle älteren Adobe Dynamic Media Classic Desktop-Programm-Versionen auf Ihrem System.

1. Laden Sie das neueste Installationsprogramm für das Adobe Dynamic Media Classic-Desktop-Programm für macOS herunter.

   * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg)

1. Stellen Sie das heruntergeladene Disk Image (.DMG) mithilfe des folgenden Befehls an einen Bereitstellungspunkt-Speicherort bereit:

   `hdiutil attach adobe-dynamic-media-classic-20.21.3.dmg -mountpoint <mount_point_path>`

1. Kopieren Sie die .APP-Datei mit dem folgenden Befehl in **[!UICONTROL Applications]**:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. Wenn Sie die Anwendung öffnen, wird die neue Adobe Dynamic Media Classic-Anmeldeseite angezeigt:

   ![Anmeldung bei Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Um sich beim Adobe Dynamic Media Classic-Desktop-Programm anzumelden, verwenden Sie dieselben Anmeldedaten wie für die Anmeldung bei Adobe Dynamic Media Classic im Browser.

   Informationen zur Verwendung von **[!UICONTROL Server]** finden Sie in der folgenden Zuordnung für die Produktionsumgebung:

   | Server | Browser-URL |
   | --- | --- |
   | NA Produktion (Nordamerika) | https://s7sps1.scene7.com/ |
   | EMEA-Produktion (Europa, Naher Osten und Afrika) | https://s7sps3.scene7.com/ |
   | APAC-Produktion (Asien-Pazifik) | https://s7sps5.scene7.com/ |

## Laden Sie die neueste Adobe Dynamic Media Classic-Desktop-App unter Windows® herunter und installieren Sie *silent*. {#install-silent-windows-dmc-app}

Der von Ihnen verwendete Befehl ist für eine einfache, unbeaufsichtigte MSI-Installation. Das Installationsprogramm für das Adobe Dynamic Media Classic-Desktop-Programm ist jedoch ein InstallScript-MSI-Installationsprogramm, das mit InstallShield erstellt wurde. Wenn Sie das Installationsprogramm im Datensatzmodus ausführen, wird jede Benutzerinteraktion in einer Antwortdatei aufgezeichnet. Diese Antwortdatei wird dann für eine unbeaufsichtigte Installation verwendet, wie unter [Ausführen von Installationen im unbeaufsichtigten Modus beschrieben.](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

Verwandte Themen:

* [Laden Sie das neueste Adobe Dynamic Media Classic-Desktop-Programm unter Mac oder Windows® herunter und installieren Sie es.](#installation-dmc-app)
* [Laden Sie das neueste Adobe Dynamic Media Classic-Desktop-Programm herunter und installieren Sie es auf macOS](#install-silent-mac-dmc-app)

So laden Sie die neueste Version des Dynamic Media Classic-Desktop-Programms unter Windows® herunter und installieren Sie *silent*:

1. Deinstallieren Sie alle älteren Adobe Dynamic Media Classic Desktop-Programm-Versionen auf Ihrem System.

1. Laden Sie das neueste Installationsprogramm für das Adobe Dynamic Media Classic-Desktop-Programm herunter.

   * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)

1. Führen Sie das Installationsprogramm im Datensatzmodus mit dem folgenden Befehl aus:

   `adobe-dynamic-media-classic-20.21.3.exe /r /f1"C:\Setup.iss"`

1. Führen Sie im Fenster des GUI-Installationsprogramms die Schritte zum Installieren aus, damit Interaktionen/Eingaben, wie der Installationsspeicherort, in der Datei `Setup.iss` aufgezeichnet werden.

1. Kopieren Sie die erstellte Datei `Setup.iss` und `adobe-dynamic-media-classic-20.21.3.exe` auf einen anderen Computer.

1. Führen Sie den folgenden Befehl für eine unbeaufsichtigte Installation aus:

   `adobe-dynamic-media-classic-20.21.3.exe /s /f1"C:\Setup.iss"`

   Details zu Befehlszeilenparametern finden Sie unter [Setup.exe und Update.exe Befehlszeilenparameter.](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. Wenn Sie die Anwendung öffnen, wird die neue Adobe Dynamic Media Classic-Anmeldeseite angezeigt:

   ![Anmeldung bei Adobe Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Um sich beim Adobe Dynamic Media Classic-Desktop-Programm anzumelden, verwenden Sie dieselben Anmeldedaten wie für die Anmeldung bei Adobe Dynamic Media Classic im Browser.

   Informationen zur Verwendung von **[!UICONTROL Server]** finden Sie in der folgenden Zuordnung für die Produktionsumgebung:

   | Server | Browser-URL |
   | --- | --- |
   | NA Produktion (Nordamerika) | https://s7sps1.scene7.com/ |
   | EMEA-Produktion (Europa, Naher Osten und Afrika) | https://s7sps3.scene7.com/ |
   | APAC-Produktion (Asien-Pazifik) | https://s7sps5.scene7.com/ |

## Video-exemplarische Vorgehensweise zur Verwendung der Adobe Dynamic Media Classic Desktop App {#dmc-app-video-walk-through}

Sehen Sie sich ein [Video-Beispiel zur Verwendung der Adobe Dynamic Media Classic Desktop App](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) an (Länge: 2 Minuten 36 Sekunden).

## Löschen des Bild-Cache und des Asset-Cache auf Ihrem Computer mithilfe des Desktop-Programms {#clear-cache}

1. Tippen Sie in der Adobe Dynamic Media Classic Desktop App oben rechts auf **[!UICONTROL Setup]** > **[!UICONTROL Persönliche Einstellungen]**.
1. Führen Sie auf der Seite **[!UICONTROL Persönliche Einstellungen]** unter der Überschrift **[!UICONTROL Desktop]** einen der folgenden Schritte aus:
   * Um alle Adobe-Bilddateien zu entfernen, die von Dynamic Media zwischengespeichert wurden, tippen Sie auf **[!UICONTROL Image-Cache löschen]** und dann auf **[!UICONTROL OK]**.
   * Um alle Adobe-Asset-Dateien zu entfernen, die von Dynamic Media zwischengespeichert wurden, tippen Sie auf **[!UICONTROL Asset-Cache löschen]** und dann auf **[!UICONTROL OK]**.
1. Tippen Sie in der rechten unteren Ecke der Seite auf **[!UICONTROL Close]**.

### Manuelles Löschen des Bild-Caches und des Asset-Caches

Sie können den Bild- und Asset-Cache nicht nur mit dem Desktop-Programm löschen, sondern auch den Cache direkt aus dem Dateisystem löschen.

1. Navigieren Sie je nach Betriebssystem zu Folgendem:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Bekannte Einschränkungen in Adobe Dynamic Media Classic 20.21.1

* Die Dropdownliste **[!UICONTROL Server]** ist nach dem Aktualisieren auf die Adobe Dynamic Media Classic Desktop App 20.21.1 - Szenario leer: Sie installieren und melden sich bei Adobe Dynamic Media Classic 20.20.1 oder 20.20.2 an und schließen dann das Programm. Anschließend aktualisieren Sie auf Adobe Dynamic Media Classic 20.21.1. Wenn Sie versuchen, sich anzumelden, ist die Dropdownliste **[!UICONTROL Server]** im Dialogfeld **[!UICONTROL Anmelden bei Ihrem Konto]** leer. Um dieses Problem zu umgehen, müssen Sie [den Cache](#clear-cache) manuell löschen (siehe obige Schritte).

## Bekannte Einschränkungen in Adobe Dynamic Media Classic 20.20.1 (behoben in 20.20.2)

**_Gilt nur für Windows® - Gibt es eine Beschränkung für die Anzahl der Dateien, die über die Benutzeroberfläche des Desktop-Programms hochgeladen werden können?_**<br>Ja, über die Benutzeroberfläche des Desktop-Programms können maximal 150 Dateien gleichzeitig hochgeladen werden.

**_Gilt für Windows® und macOS - Wie kann ich zwischen Unternehmen wechseln?_**<br>Gehen Sie wie folgt vor, um zwischen Unternehmen zu wechseln:

* Wählen Sie in der Adobe Dynamic Media Classic-App das neue Unternehmen aus der Dropdownliste &quot;Unternehmen&quot;aus.
* Wenn das Popup-Fenster angezeigt wird, tippen Sie auf **[!UICONTROL OK]**, um sich abzumelden und die App zu schließen.

   ![Um das neue Unternehmen zu verwenden, starten Sie das Programm neu](/help/assets/dmclassic-new-company1.png)

* Starten Sie Adobe Dynamic Media Classic neu und melden Sie sich wie gewohnt an, um mit dem neuen Unternehmen zu arbeiten.

## Tipps und Tricks

**_Auf der Landingpage von Adobe Dynamic Media Classic kann ich das Bedienfeld &quot;Warenkorb&quot;nicht sehen._**<br>Tippen Sie in Adobe Dynamic Media Classic auf**[!UICONTROL Einstellungen > Persönliche Einstellungen ]**. Stellen Sie im Abschnitt Browser sicher, dass**[!UICONTROL MediaPortal-Funktionen anzeigen ]**ausgewählt ist (markiert). Tippen Sie auf**[!UICONTROL Speichern > Schließen ]**.

**_Der Veröffentlichungsstatus (grüne Anzeige) eines Assets wird nicht korrekt angezeigt._**<br>In der Browser-Benutzeroberfläche war eine erneute Anmeldung bei der Benutzeroberfläche erforderlich, um den korrekten Veröffentlichungsstatus der Assets anzuzeigen. Im Desktop-Programm hat Adobe in der Symbolleiste das Symbol**[!UICONTROL Aktualisieren ]**rechts neben der Schaltfläche**[!UICONTROL Keine auswählen ]**eingeführt. Tippen Sie auf das Symbol**[!UICONTROL Aktualisieren ]**, um den neuesten Status aller Assets auf der angegebenen Seite anzuzeigen. Wie bei der Browser-Benutzeroberfläche ist keine erneute Anmeldung erforderlich.

![Symbol ](/help/assets/refresh-icon1.png)
*&quot;Aktualisieren&quot;*

**_Stapelsatzvorgaben funktionieren nicht im Desktop-Programm._**<br>Tippen Sie auf**[!UICONTROL Hochladen > Auftragsoptionen > Stapelsatzvorgaben ]**. Stellen Sie sicher, dass die entsprechende**[!UICONTROL Stapelsatzvorgabe ]**aktiviert ist. Klicken Sie auf**[!UICONTROL Upload speichern und senden ]**.
