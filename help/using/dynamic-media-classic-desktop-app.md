---
title: Adobe Dynamic Media Classic-Desktop-Programm - jetzt verfügbar
description: Erfahren Sie mehr über das Adobe Dynamic Media Classic-Desktop-Programm.
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
topic: Administration
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '2035'
ht-degree: 1%

---

# Jetzt verfügbar: Adobe Dynamic Media Classic-Desktop-Programm {#dynamic-media-classic-desktop-app}

Adobe Dynamic Media Classic-Benutzer haben jetzt Zugriff auf ein neues Desktop-Programm-Erlebnis, das im Browser nicht mehr auf Adobe-Flash-Technologie angewiesen ist.

Diese neue App ist jetzt für Windows® und macOS verfügbar.

>[!IMPORTANT]
>
>Adobe empfiehlt, das neue Adobe Dynamic Media Classic-Desktop-Programm bis zum 1. Oktober 2020 zu installieren. Dadurch wird sichergestellt, dass Sie einen reibungslosen Übergang haben, bevor Adobe Flash Player am 31. Dezember 2020 eingestellt wird. Nach diesem Datum können Sie sich nicht mehr bei der Browserversion der Adobe Dynamic Media Classic-Benutzeroberfläche anmelden, die im Produkt als Adobe Dynamic Media Classic bezeichnet wird.

Siehe FAQs für die [Die neue Adobe Dynamic Media Classic-Anmeldung ist jetzt verfügbar.](/help/using/new-ui-2020.md)

## Systemanforderungen für das Adobe Dynamic Media Classic-Desktop-Programm {#system-requirements-dmc-app}

Das Adobe Dynamic Media Classic-Desktop-Programm ist mit den folgenden Betriebssystemen kompatibel:

* macOS 10.10 oder höher.
* Windows® 7 oder höher.

Die vollständigen Systemanforderungen finden Sie unter [Systemanforderungen für das Adobe Dynamic Media Classic-Desktop-Programm](/help/using/system-requirements.md).

Die Aktualisierungsbenachrichtigung innerhalb der Adobe Dynamic Media Classic-Desktop-Applikation wird nicht für *klein* veröffentlicht. Kunden, die von Fehlerbehebungen in einer kleineren Version profitieren, können ein Upgrade durchführen.

## Nur in der neuesten Version (20.22.2) von macOS behoben {#release-feb2022}

* macOS Monterey - Datei-Upload-Seite wird bei nachfolgenden Uploads nicht mehr angezeigt. <!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## Fehlerbehebungen in der neuesten Version (20.22.1) {#release-jan2022}

* Bildbearbeitung **[!UICONTROL Speichern]** -Schaltflächen funktionierten nicht.
* Im Set-Editor wird die **[!UICONTROL Schließen]**, **[!UICONTROL Speichern]**, und **[!UICONTROL Speichern unter]** -Schaltflächen werden nach dem Scrollen von Assets im **[!UICONTROL Hinzufügen von Assets]** Bedienfeld.
* **[!UICONTROL Play]** -Schaltfläche in der Videodetailansicht nicht funktionierte.
* Nicht eingeben `d` und `e` in **[!UICONTROL Benutzername]** und **[!UICONTROL Passwort]** Felder beim Ausführen von macOS Monterey.
* Die verbleibenden Analyse-APIs wurden in Version 2.0 verschoben.

## Fehlerbehebungen in Version 20.21.3 {#release-sept2021}

* Beschädigte Miniaturansichten für Assets, die nach einer Inaktivität im Desktop-Programm angezeigt wurden.
* Das Desktop-Programm reagiert nicht mehr, normalerweise nach den Vorgängen &quot;Set&quot;.
* Verschleierung und Sperrmodus für Anfragen automatisch aktiviert unter **[!UICONTROL Image-Serving testen]**.

  Siehe [Testen des Secure Testing-Dienstes](/help/using/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* Der Authentifizierungsmechanismus wurde mit Adobe Analytics aktualisiert. Relevant für neue Integrationen oder wenn einige Analytics-Variablen vom Dynamic Media Classic-Desktop-Programm aus aktualisiert werden müssen.

  Siehe [Bei Adobe Analytics anmelden](/help/using/log-analytics.md) für aktualisierte Schritte.

## Fehlerbehebungen in Version 20.21.2 {#minor-release}

* Bekannte Einschränkung in Version 20.21.1: die **[!UICONTROL Server]** auf der Dropdown-Liste auf dem Anmeldebildschirm war leer.
* In **[!UICONTROL Upload-Auftragsoptionen]**, Standardwert für die Ebenenbenennung unter **[!UICONTROL Photoshop-Optionen]**, ist jetzt **[!UICONTROL Photoshop und Ebenenname]**. Die Ebenen der PSD-Datei werden als getrennte Bilder hochgeladen.
   * Der frühere Standardwert von **[!UICONTROL Ebenenname]**, die Bilder nach ihrem Ebenennamen oder ihrer Ebenennummer in der PSD-Datei benannt. Die Ebenennummer wurde verwendet, wenn die Ebenennamen in der PSD-Datei standardmäßige Photoshop-Ebenennamen waren.
   * Die neue Standardeinstellung von **[!UICONTROL Photoshop und Ebenenname]** bezeichnet die Bilder nach der PSD-Datei, gefolgt vom Ebenennamen oder der Ebenennummer. Die Nummern der Ebenen werden verwendet, wenn es sich bei den Namen der Ebenen in der PSD-Datei um standardmäßige Photoshop-Ebenennamen handelt.
   * Da Ebenenbilder in Adobe Dynamic Media Classic jetzt eindeutige Namen haben, werden keine Änderungen an bestehenden PSD oder Vorlagen vorgenommen (die in den Originaldateien gemeinsame Ebenennamen haben).
* Beschädigte Miniaturen von Assets.

## Fehlerbehebungen in Version 20.21.1 {#latest-fixes-desktop-app}

* Probleme bei der Anmeldung aufgrund eines Timeouts, was zu folgender Meldung führt: *Dieser Benutzer kann der Gruppe oder den Gruppen ohne Berechtigung zugewiesen werden. Wenden Sie sich an Ihren Administrator.*
* Viewer-Vorgaben werden bei jedem falschen Kennwortversuch dupliziert.
* Das Desktop-Programm reagiert aufgrund vieler Assets im Stammordner nicht mehr. (Behoben unter Windows®; funktioniert wie gewünscht unter macOS.)

## Fehlerbehebungen in Version 20.20.2 {#previous-version-fixes-desktop-app}

* Keine Begrenzung der Anzahl der Dateien, die Sie über die Benutzeroberfläche des Desktop-Programms für macOS und Windows® hochladen können.
* Sie müssen sich nicht von der Desktop-App abmelden, um zwischen Unternehmen zu wechseln.
* Strg+V zum Einfügen funktioniert jetzt unter Windows®.
* Wenn in Zukunft eine neue Version des Desktop-Programms veröffentlicht wird, werden Benutzer über das Desktop-Programm selbst benachrichtigt.

## Herunterladen und Installieren des neuesten Adobe Dynamic Media Classic-Desktop-Programms unter macOS oder Windows® {#installation-dmc-app}

Verwandte Themen:

* [Herunterladen und unbeaufsichtigte Installation des neuesten Adobe Dynamic Media Classic-Desktop-Programms auf Mac](#install-silent-mac-dmc-app)
* [Herunterladen und unbeaufsichtigte Installation des neuesten Adobe Dynamic Media Classic-Desktop-Programms unter Windows](#install-silent-windows-dmc-app)

1. Deinstallieren Sie alle älteren Versionen des Adobe Dynamic Media Classic-Desktop-Programms auf Ihrem System.

1. Laden Sie das neueste Installationsprogramm für das Adobe Dynamic Media Classic-Desktop-Programm herunter.

   * Die neueste Version ist unter folgender Adresse verfügbar:

      * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

   * Die vorherige Version ist unter folgender Adresse verfügbar:

      * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)

<!--         * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows&reg; (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. Führen Sie je nach heruntergeladenem Installationsprogramm einen der folgenden Schritte aus.

   * **macOS** -Im **[!UICONTROL Drag &amp; Drop zum Installieren]** Dialogfeld, ziehen **[!UICONTROL Adobe Dynamic Media Classic]** und legen Sie sie auf **[!UICONTROL Anwendungen]**.

     ![Installieren per Drag &amp; Drop in macOS](/help/using/assets/dragondrop-install1.png)

   * Im **[!UICONTROL Anwendungen]** auf das Adobe Dynamic Media Classic-Symbol.
   * Tippen Sie im Dialogfeld auf **[!UICONTROL Öffnen]** , um das Adobe Dynamic Media Classic-Desktop-Programm zu öffnen.

     ![Heruntergeladene App öffnen](/help/using/assets/open-dmclassicapp1.png)

   * **Windows** - Führen Sie die Binärdatei des Installationsprogramms aus und befolgen Sie die Anweisungen auf dem Bildschirm, um das Desktop-Programm zu installieren.

1. Wenn Sie die Anwendung öffnen, wird die neue Adobe Dynamic Media Classic-Anmeldeseite angezeigt:

   ![Adobe Dynamic Media Classic-Anmeldung](/help/using/assets/dmclassic-login1.png)

1. Um sich beim Adobe Dynamic Media Classic-Desktop-Programm anzumelden, verwenden Sie dieselben Anmeldedaten wie für die Anmeldung bei Adobe Dynamic Media Classic im Browser.

   Für **[!UICONTROL Server]** Informationen zur Verwendung finden Sie in der folgenden Zuordnung für die Produktionsumgebung:

   | Server | Browser-URL |
   | --- | --- |
   | Produktion der NA (Nordamerika) | https://s7sps1.scene7.com/ |
   | EMEA-Produktion (Europa, Naher Osten und Afrika) | https://s7sps3.scene7.com/ |
   | APAC-Produktion (Asien-Pazifik) | https://s7sps5.scene7.com/ |

1. Beachten Sie nach der Anmeldung die bekannte Benutzeroberfläche des Browsers. Sie können Ihre tägliche Adobe Dynamic Media Classic-Aktivität wie gewohnt im Desktop-Programm fortsetzen.

## Herunterladen und *stumm* Installieren des neuesten Adobe Dynamic Media Classic-Desktop-Programms auf macOS {#install-silent-mac-dmc-app}

Verwandte Themen:

* [Herunterladen und Installieren des neuesten Adobe Dynamic Media Classic-Desktop-Programms unter Mac oder Windows](#installation-dmc-app)
* [Herunterladen und unbeaufsichtigte Installation des neuesten Adobe Dynamic Media Classic-Desktop-Programms unter Windows](#install-silent-windows-dmc-app)

Zum Herunterladen und *stumm* Installieren Sie die neueste Version des Adobe Dynamic Media Classic-Desktop-Programms auf macOS:

1. Deinstallieren Sie alle älteren Versionen des Adobe Dynamic Media Classic-Desktop-Programms auf Ihrem System.

1. Laden Sie das neueste Installationsprogramm für das Adobe Dynamic Media Classic-Desktop-Programm für macOS herunter.

   * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. Stellen Sie das heruntergeladene Disk Image (.DMG) mithilfe des folgenden Befehls an einen Bereitstellungspunkt-Speicherort bereit:

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. Kopieren Sie die .APP-Datei nach **[!UICONTROL Anwendungen]** mit dem folgenden Befehl:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. Wenn Sie die Anwendung öffnen, wird die neue Adobe Dynamic Media Classic-Anmeldeseite angezeigt:

   ![Adobe Dynamic Media Classic-Anmeldung](/help/using/assets/dmclassic-login1.png)

1. Um sich beim Adobe Dynamic Media Classic-Desktop-Programm anzumelden, verwenden Sie dieselben Anmeldedaten wie für die Anmeldung bei Adobe Dynamic Media Classic im Browser.

   Für **[!UICONTROL Server]** Informationen zur Verwendung finden Sie in der folgenden Zuordnung für die Produktionsumgebung:

   | Server | Browser-URL |
   | --- | --- |
   | Produktion der NA (Nordamerika) | https://s7sps1.scene7.com/ |
   | EMEA-Produktion (Europa, Naher Osten und Afrika) | https://s7sps3.scene7.com/ |
   | APAC-Produktion (Asien-Pazifik) | https://s7sps5.scene7.com/ |

## Herunterladen und *stumm* Installieren des neuesten Adobe Dynamic Media Classic-Desktop-Programms unter Windows® {#install-silent-windows-dmc-app}

Der von Ihnen verwendete Befehl ist für eine einfache, unbeaufsichtigte MSI-Installation. Das Installationsprogramm für das Adobe Dynamic Media Classic-Desktop-Programm ist jedoch ein InstallScript-MSI-Installationsprogramm, das mit InstallShield erstellt wurde. Wenn Sie das Installationsprogramm im Datensatzmodus ausführen, wird jede Benutzerinteraktion in einer Antwortdatei aufgezeichnet. Diese Antwortdatei wird dann für eine unbeaufsichtigte Installation verwendet, wie unter [Laufende Installationen im Ruhezustand](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm).

Verwandte Themen:

* [Herunterladen und Installieren des neuesten Adobe Dynamic Media Classic-Desktop-Programms unter Mac oder Windows](#installation-dmc-app)

* [Herunterladen und unbeaufsichtigte Installation des neuesten Adobe Dynamic Media Classic-Desktop-Programms auf macOS](#install-silent-mac-dmc-app)

Zum Herunterladen und *stumm* Installieren Sie die neueste Version des Adobe Dynamic Media Classic-Desktop-Programms unter Windows®:

1. Deinstallieren Sie alle älteren Versionen des Adobe Dynamic Media Classic-Desktop-Programms auf Ihrem System.

1. Laden Sie das neueste Installationsprogramm für das Adobe Dynamic Media Classic-Desktop-Programm herunter.

   * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. Führen Sie das Installationsprogramm im Datensatzmodus mit dem folgenden Befehl aus:

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. Führen Sie im Fenster des GUI-Installationsprogramms die Schritte zum Installieren aus, damit Interaktionen/Eingaben, wie z. B. der Installationsspeicherort, in aufgezeichnet werden. `Setup.iss` -Datei.

1. Kopieren Sie die erstellte `Setup.iss` Datei und `adobe-dynamic-media-classic-20.22.1.exe` auf einen anderen Computer.

1. Führen Sie den folgenden Befehl für eine unbeaufsichtigte Installation aus:

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   Details zu Befehlszeilenparametern finden Sie unter [Befehlszeilenparameter &quot;Setup.exe&quot;und &quot;Update.exe&quot;](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters).

1. Wenn Sie die Anwendung öffnen, wird die neue Adobe Dynamic Media Classic-Anmeldeseite angezeigt:

   ![Adobe Dynamic Media Classic-Anmeldung](/help/using/assets/dmclassic-login1.png)

1. Um sich beim Adobe Dynamic Media Classic-Desktop-Programm anzumelden, verwenden Sie dieselben Anmeldedaten wie für die Anmeldung bei Adobe Dynamic Media Classic im Browser.

   Für **[!UICONTROL Server]** Informationen zur Verwendung finden Sie in der folgenden Zuordnung für die Produktionsumgebung:

   | Server | Browser-URL |
   | --- | --- |
   | Produktion der NA (Nordamerika) | https://s7sps1.scene7.com/ |
   | EMEA-Produktion (Europa, Naher Osten und Afrika) | https://s7sps3.scene7.com/ |
   | APAC-Produktion (Asien-Pazifik) | https://s7sps5.scene7.com/ |

## Video-exemplarische Vorgehensweise zur Verwendung der Adobe Dynamic Media Classic Desktop App {#dmc-app-video-walk-through}

Sehen Sie sich eine [Video-exemplarische Vorgehensweise zur Verwendung der Adobe Dynamic Media Classic Desktop App](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (Länge: 2 Minuten, 36 Sekunden).

## Löschen des Bild-Cache und des Asset-Cache auf Ihrem Computer mithilfe des Desktop-Programms {#clear-cache}

1. Tippen Sie im Adobe Dynamic Media Classic-Desktop-Programm in der Nähe der oberen rechten Ecke auf **[!UICONTROL Einrichtung]** > **[!UICONTROL Persönliche Einstellungen]**.
1. Im **[!UICONTROL Persönliche Einstellungen]** Seite, unter der **[!UICONTROL Desktop]** -Überschrift einen der folgenden Schritte ausführen:
   * Um alle im Adobe Dynamic Media-Cache gespeicherten Bilddateien von Ihrem Computer zu entfernen, tippen Sie auf **[!UICONTROL Bild-Cache löschen]** und tippen Sie dann auf **[!UICONTROL OK]**.
   * Tippen Sie zum Entfernen aller zwischengespeicherten Asset-Dateien von Adobe Dynamic Media von Ihrem Computer auf **[!UICONTROL Asset-Cache löschen]** und tippen Sie dann auf **[!UICONTROL OK]**.
1. Tippen Sie unten rechts auf der Seite auf **[!UICONTROL Schließen]**.

### Manuelles Löschen des Bild-Cache und des Asset-Cache

Sie können den Bild- und Asset-Cache nicht nur mit dem Desktop-Programm löschen, sondern auch den Cache direkt aus dem Dateisystem löschen.

1. Navigieren Sie je nach Betriebssystem zu Folgendem:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Bekannte Einschränkungen in Adobe Dynamic Media Classic 20.21.1

* Die **[!UICONTROL Server]** Die Dropdownliste ist nach dem Aktualisieren auf das Adobe Dynamic Media Classic-Desktop-Programm 20.21.1 - Szenario: Sie installieren und melden sich bei Adobe Dynamic Media Classic 20.20.1 oder 20.20.2 an und schließen dann das Programm. Dann aktualisieren Sie auf Adobe Dynamic Media Classic 20.21.1. Wenn Sie versuchen, sich anzumelden, wird die **[!UICONTROL Server]** Dropdown-Liste im **[!UICONTROL Bei Ihrem Konto anmelden]** leer ist. Um dieses Problem zu umgehen, müssen Sie [Cache manuell löschen](#clear-cache) (siehe obige Schritte).

## Bekannte Einschränkungen in Adobe Dynamic Media Classic 20.20.1 (behoben in 20.20.2)

**_Gilt nur für Windows® - Gibt es eine Beschränkung für die Anzahl der Dateien, die über die Benutzeroberfläche des Desktop-Programms hochgeladen werden können?_**<br>Ja, über die Benutzeroberfläche des Desktop-Programms können maximal 150 Dateien gleichzeitig hochgeladen werden.

**_Gilt für Windows® und macOS - Wie kann ich zwischen Unternehmen wechseln?_**<br>Gehen Sie wie folgt vor, um zwischen Unternehmen zu wechseln:

* Wählen Sie in der Adobe Dynamic Media Classic-App das neue Unternehmen aus der Dropdownliste &quot;Unternehmen&quot;aus.
* Wenn das Popup-Fenster angezeigt wird, tippen Sie auf **[!UICONTROL OK]** , um sich abzumelden und die App zu schließen.

  ![Um das neue Unternehmen zu verwenden, starten Sie das Programm neu](/help/using/assets/dmclassic-new-company1.png)

* Starten Sie Adobe Dynamic Media Classic neu und melden Sie sich wie gewohnt an, um mit dem neuen Unternehmen zusammenzuarbeiten.

## Tipps und Tricks

**_Auf der Landingpage von Adobe Dynamic Media Classic kann ich das Bedienfeld &quot;Warenkorb&quot;nicht sehen._**<br>Tippen Sie in Adobe Dynamic Media Classic auf**[!UICONTROL Einrichtung > Persönliche Einstellungen ]**. Stellen Sie im Abschnitt Browser sicher, dass**[!UICONTROL MediaPortal-Funktionen anzeigen ]**aktiviert (markiert). Tippen**[!UICONTROL Speichern > Schließen ]**.

**_Der Veröffentlichungsstatus (grüne Anzeige) eines Assets wird nicht korrekt angezeigt._**<br>In der Browser-Benutzeroberfläche war eine erneute Anmeldung bei der Benutzeroberfläche erforderlich, um den korrekten Veröffentlichungsstatus der Assets anzuzeigen. Im -Desktop-Programm hat Adobe eine**[!UICONTROL Aktualisieren ]**in der Symbolleiste rechts neben**[!UICONTROL Keine auswählen ]**Schaltfläche. Tippen Sie auf**[!UICONTROL Aktualisieren ]**-Symbol, um den neuesten Status aller Assets auf der angegebenen Seite anzuzeigen. Wie bei der Browser-Benutzeroberfläche ist keine erneute Anmeldung erforderlich.

![Aktualisierungssymbol](/help/using/assets/refresh-icon1.png)
*Aktualisierungssymbol*

**_Stapelsatzvorgaben funktionieren nicht im Desktop-Programm._**<br>Tippen**[!UICONTROL Hochladen > Auftragsoptionen > Stapelsatzvorgaben ]**. Stellen Sie die relevanten**[!UICONTROL Stapelsatzvorgabe ]**aktiviert ist. Klicks**[!UICONTROL Upload speichern und senden ]**.
