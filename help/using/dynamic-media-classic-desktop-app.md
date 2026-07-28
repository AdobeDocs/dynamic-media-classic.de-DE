---
title: Adobe Dynamic Media Classic-Desktop-Programm
description: Erfahren Sie mehr über das Adobe Dynamic Media Classic-Desktop-Programm, das jetzt verfügbar ist.
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
topic: Administration
level: Intermediate
autotag-review: '2026-05-13T19:46:24.807Z'
TQID: 'https://experienceleague.adobe.com/w-jPQYG7xGeBmC8fOzcPzi6ZZ-urf0C0-HoDKVbjCWk'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: fcd8f761bcc746c402db2f06347b77352d1488f7
workflow-type: tm+mt
source-wordcount: 2124
ht-degree: 0%

---

# Jetzt verfügbar: Adobe Dynamic Media Classic Desktop App {#dynamic-media-classic-desktop-app}

Adobe Dynamic Media Classic-Benutzer haben jetzt Zugriff auf ein neues Desktop-Programm, das nicht mehr auf die Adobe Flash-Technologie im Browser angewiesen ist.

Diese neue App ist jetzt für Windows® und macOS verfügbar.

>[!IMPORTANT]
>
>Adobe empfiehlt, das neue Adobe Dynamic Media Classic-Desktop-Programm bis zum 1. Oktober 2020 zu installieren. Dadurch wird sichergestellt, dass Sie einen Übergangszeitraum haben, bevor Adobe Flash Player am 31. Dezember 2020 eingestellt wird. Nach diesem Datum können Sie sich nicht mehr bei der Browser-Version der Adobe Dynamic Media Classic-Benutzeroberfläche anmelden, die im Produkt als Adobe Dynamic Media Classic gekennzeichnet ist.

Siehe die häufig gestellten Fragen zu [Neue Adobe Dynamic Media Classic-Anmeldung jetzt verfügbar.](/help/using/new-ui-2020.md)

## Systemanforderungen für das Adobe Dynamic Media Classic-Desktop-Programm {#system-requirements-dmc-app}

Das Adobe Dynamic Media Classic-Desktop-Programm ist mit den folgenden Betriebssystemen kompatibel:

* macOS 10.10 oder neuer.
* Windows® 7 oder neuer.

Die vollständigen Systemanforderungen finden Sie unter [Systemanforderungen für das Adobe Dynamic Media Classic-Desktop-Programm](/help/using/system-requirements.md).

Eine Upgrade-Benachrichtigung innerhalb des Adobe Dynamic Media Classic-Desktop-Programms wird nicht für *Versionen*. Kunden, die von Fehlerbehebungen in einer Nebenversion profitieren, können ein Upgrade durchführen.

## Korrektur nur in der neuesten Version (20.22.2) von macOS {#release-feb2022}

* macOS Monterey: Seite zum Hochladen von Dateien wurde bei nachfolgenden Uploads eingefroren. <!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## Fehlerbehebungen in der neuesten Version (20.22.1) {#release-jan2022}

* Beim Bearbeiten eines Bildes **[!UICONTROL die Schaltflächen]** Speichern“ nicht funktioniert.
* In den Set-Editoren werden **[!UICONTROL Schaltflächen „Schließen]**, **[!UICONTROL Speichern]** und **[!UICONTROL Speichern unter]** deaktiviert, nachdem Assets im Bedienfeld **[!UICONTROL Assets hinzufügen]** gescrollt wurden.
* Die **[!UICONTROL Wiedergabe]**-Schaltfläche in der Videodetailansicht funktionierte nicht.
* Benutzende können `d` und `e` nicht in die Felder **[!UICONTROL Benutzername]** und **[!UICONTROL Kennwort]** eingeben, wenn sie macOS Monterey ausführen.
* Verbleibende Analytics-APIs wurden in Version 2.0 verschoben.

## Fehlerbehebungen in Version 20.21.3 {#release-sept2021}

* Beschädigte Miniaturansichten von Assets, die nach einer gewissen Zeit der Inaktivität in der Desktop-Anwendung angezeigt wurden.
* Das Desktop-Programm reagiert nicht mehr, normalerweise nach Set-Vorgängen.
* Verschleierung von Anfragen und Sperrmodus automatisch unter „Bereitstellung von **[!UICONTROL -Bildern“]**.

  Siehe [Der Secure Testing-Service](/help/using/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* Der Authentifizierungsmechanismus wurde mit Adobe Analytics aktualisiert. Relevant für neue Integrationen oder wenn einige Analytics-Variablen in der Dynamic Media Classic-Desktop-App aktualisiert werden müssen.

  Siehe [Anmelden bei Adobe Analytics](/help/using/log-analytics.md) für aktualisierte Schritte.

## Fehlerbehebungen in Version 20.21.2 {#minor-release}

* Bekannte Einschränkung in 20.21.1: Die **[!UICONTROL Server]**-Dropdown-Liste auf dem Anmeldebildschirm war leer.
* In **[!UICONTROL Upload-Auftragsoptionen]** ist der standardmäßige Ebenenname-Wert unter **[!UICONTROL Photoshop-Optionen]** jetzt **[!UICONTROL Photoshop und Ebenenname]**. Die Ebenen der PSD-Datei werden als getrennte Bilder hochgeladen.
  * Der frühere Standardwert (**[!UICONTROL )]** die Bilder nach ihrem Ebenennamen oder ihrer Ebenennummer in der PSD-Datei. Die Ebenennummer wurde verwendet, wenn die Ebenennamen in der PSD-Datei standardmäßige Adobe Photoshop-Ebenennamen waren.
  * Der neue Standardwert **[!UICONTROL Photoshop und Ebenenname]** benennt die Bilder nach der PSD-Datei, gefolgt vom Ebenennamen oder der Ebenennummer. Die Ebenennummer wird verwendet, wenn es sich bei den Ebenennamen in der PSD-Datei um standardmäßige Adobe Photoshop-Ebenennamen handelt.
  * Da Ebenenbilder in Adobe Dynamic Media Classic jetzt eindeutige Namen haben, werden bestehende PSD oder Vorlagen nicht aktualisiert (die Ebenennamen in den Original-PSD-Dateien freigegeben haben).
* Beschädigte Miniaturen von Assets.

## Fehlerbehebungen in Version 20.21.1 {#latest-fixes-desktop-app}

* Anmeldeprobleme aufgrund einer Zeitüberschreitung, die zu folgender Meldung führen: *Dieser Benutzer ist der Gruppe oder den Gruppen ohne Berechtigung zugewiesen. Wenden Sie sich an Ihren Administrator.*
* Viewer-Vorgaben werden bei jedem falschen Passwortversuch dupliziert.
* Desktop-Programm reagiert nicht mehr, da sich viele Assets im Stammordner befinden. (Behoben unter Windows®; funktioniert wie gewünscht auf macOS.)

## Fehlerbehebungen in Version 20.20.2 {#previous-version-fixes-desktop-app}

* Keine Begrenzung der Anzahl der Dateien, die Sie über die Benutzeroberfläche des Desktop-Programms für macOS und Windows® hochladen können.
* Sie müssen sich nicht vom Desktop-Programm abmelden, um zwischen Unternehmen zu wechseln.
* Strg+V für das Einfügen funktioniert jetzt unter Windows®.
* Wenn künftig eine neue Version des Desktop-Programms veröffentlicht wird, werden die Benutzer innerhalb des Desktop-Programms selbst benachrichtigt.

## Herunterladen und Installieren der neuesten Adobe Dynamic Media Classic Desktop-App unter macOS oder Windows® {#installation-dmc-app}

Siehe auch:

* [Herunterladen und automatische Installation der neuesten Adobe Dynamic Media Classic Desktop-App auf Mac](#install-silent-mac-dmc-app)
* [Laden Sie die neueste Adobe Dynamic Media Classic Desktop-App unter Windows herunter und installieren Sie sie im Hintergrund®](#install-silent-windows-dmc-app)

1. Deinstallieren Sie alle älteren Adobe Dynamic Media Classic Desktop-Anwendungsversionen auf Ihrem System.

1. Laden Sie das neueste Installationsprogramm für das Adobe Dynamic Media Classic-Desktop-Programm herunter.

   * Die neueste Version ist unter folgender Adresse verfügbar:

     * [macOS (.DMG): Herunterladen](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
     * [Windows (.EXE): Herunterladen](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

   * Die vorherige Version ist unter folgender Adresse verfügbar:

     * [macOS (.DMG): Herunterladen](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
     * [Windows® (.EXE): Herunterladen](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)

<!--
         * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) 
-->

<!--
        * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows&reg; (.EXE): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) 
-->

<!--
    * [macOS (.DMG): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
    * [Windows (.EXE): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) 
-->


1. Führen Sie je nach heruntergeladenem Installationsprogramm einen der folgenden Schritte aus.

   * **macOS** - Ziehen Sie im Dialogfeld **[!UICONTROL Drag &amp; Drop zur Installation]** **[!UICONTROL Adobe Dynamic Media Classic]** und legen Sie es auf **[!UICONTROL Programme]** ab.

     ![Installation per Drag-and-Drop auf macOS](/help/using/assets/dragondrop-install1.png)

   * Tippen **[!UICONTROL im Ordner]** Programme“ auf das Adobe Dynamic Media Classic-Symbol.
   * Tippen Sie im Dialogfeld auf **[!UICONTROL Öffnen]**, um das Adobe Dynamic Media Classic-Desktop-Programm zu öffnen.

     ![Heruntergeladene App öffnen](/help/using/assets/open-dmclassicapp1.png)

   * **Windows** - Führen Sie die Installationsprogrammbinärdatei aus und folgen Sie den Anweisungen auf dem Bildschirm, um das Desktop-Programm zu installieren.

1. Wenn Sie die Anwendung öffnen, wird die neue Adobe Dynamic Media Classic-Anmeldeseite angezeigt:

   ![Adobe Dynamic Media Classic-Anmeldung](/help/using/assets/dmclassic-login1.png)

1. Verwenden Sie zum Anmelden bei der Adobe Dynamic Media Classic-Desktop-App dieselben Anmeldeinformationen wie beim Anmelden bei Adobe Dynamic Media Classic im Browser.

   Informationen zur Verwendung **[!UICONTROL Servers]** finden Sie in der folgenden Zuordnung für die Produktionsumgebung:

   | Server | Browser-URL |
   | --- | --- |
   | NA Production (Nordamerika) | https://s7sps1.scene7.com/ |
   | EMEA-Produktion (Europa, Naher Osten und Afrika) | https://s7sps3.scene7.com/ |
   | APAC-Produktion (Asien-Pazifik) | https://s7sps5.scene7.com/ |

1. Nach der Anmeldung wird die Benutzeroberfläche des Browsers angezeigt. Sie können Ihre Adobe Dynamic Media Classic-Aktivität wie gewohnt im -Desktop-Programm fortsetzen.

## Herunterladen und *im Hintergrund* Installieren des neuesten Adobe Dynamic Media Classic-Desktop-Programms auf macOS {#install-silent-mac-dmc-app}

Siehe auch:

* [Herunterladen und Installieren der neuesten Adobe Dynamic Media Classic Desktop-App unter Mac oder Windows®](#installation-dmc-app)
* [Laden Sie die neueste Adobe Dynamic Media Classic Desktop-App unter Windows herunter und installieren Sie sie im Hintergrund®](#install-silent-windows-dmc-app)

So laden Sie *neueste Version* Adobe Dynamic Media Classic-Desktop-Programms auf macOS herunter und installieren Sie sie im Hintergrund:

1. Deinstallieren Sie alle älteren Adobe Dynamic Media Classic Desktop-Anwendungsversionen auf Ihrem System.

1. Laden Sie das neueste Installationsprogramm für das Adobe Dynamic Media Classic-Desktop-Programm für macOS herunter.

   * [macOS (.DMG): Herunterladen](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. Stellen Sie das heruntergeladene Disk Image (.DMG) mit dem folgenden Befehl an einen Bereitstellungspunkt bereit:

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. Kopieren Sie die `.APP`-Datei **[!UICONTROL Anwendungen]** mithilfe des folgenden Befehls:

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG: hdiutil detach <mount_point_path>
   ```

1. Wenn Sie die Anwendung öffnen, wird die neue Adobe Dynamic Media Classic-Anmeldeseite angezeigt:

   ![Adobe Dynamic Media Classic-Anmeldung](/help/using/assets/dmclassic-login1.png)

1. Verwenden Sie zum Anmelden bei der Adobe Dynamic Media Classic-Desktop-App dieselben Anmeldeinformationen wie beim Anmelden bei Adobe Dynamic Media Classic im Browser.

   Informationen zur Verwendung **[!UICONTROL Servers]** finden Sie in der folgenden Zuordnung für die Produktionsumgebung:

   | Server | Browser-URL |
   | --- | --- |
   | NA Production (Nordamerika) | https://s7sps1.scene7.com/ |
   | EMEA-Produktion (Europa, Naher Osten und Afrika) | https://s7sps3.scene7.com/ |
   | APAC-Produktion (Asien-Pazifik) | https://s7sps5.scene7.com/ |

## Herunterladen und *im*) Installieren des neuesten Adobe Dynamic Media Classic-Desktop-Programms unter Windows® {#install-silent-windows-dmc-app}

Der von Ihnen verwendete Befehl ist für eine einfache, automatische MSI-Installation. Das Adobe Dynamic Media Classic-Desktop-Programm-Installationsprogramm ist jedoch ein mit InstallShield erstelltes InstallScript-MSI-Installationsprogramm. Wenn Sie das Installationsprogramm im Datensatzmodus ausführen, wird jede Benutzerinteraktion in einer Antwortdatei aufgezeichnet. Diese Antwortdatei wird dann für eine automatische Installation verwendet, wie unter „Ausführen [&#x200B; Installationen im Hintergrund](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm) beschrieben.

Siehe auch:

* [Herunterladen und Installieren der neuesten Adobe Dynamic Media Classic Desktop-App unter Mac oder Windows®](#installation-dmc-app)

* [Herunterladen und automatische Installation der neuesten Adobe Dynamic Media Classic Desktop-App auf macOS](#install-silent-mac-dmc-app)

® So laden Sie *neueste Version* Adobe Dynamic Media Classic-Desktop-Programms unter Windows herunter und installieren Sie sie im:

1. Deinstallieren Sie alle älteren Adobe Dynamic Media Classic Desktop-Anwendungsversionen auf Ihrem System.

1. Laden Sie das neueste Installationsprogramm für das Adobe Dynamic Media Classic-Desktop-Programm herunter.

   * [Windows® (.EXE): Herunterladen](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. Führen Sie das Installationsprogramm im Datensatzmodus mit dem folgenden Befehl aus:

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. Führen Sie im Fenster des GUI-Installationsprogramms die Installationsschritte aus, damit Interaktionen/Eingaben, wie z. B. der Installationsort, in `Setup.iss` Datei aufgezeichnet werden.

1. Kopieren Sie die erstellte `Setup.iss`-Datei und `adobe-dynamic-media-classic-20.22.1.exe` auf einen anderen Computer.

1. Führen Sie den folgenden Befehl für eine automatische Installation aus:

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   Details zu Befehlszeilenparametern finden Sie unter [Setup.exe und Update.exe Befehlszeilenparameter](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters).

1. Wenn Sie die Anwendung öffnen, wird die neue Adobe Dynamic Media Classic-Anmeldeseite angezeigt:

   ![Adobe Dynamic Media Classic-Anmeldung](/help/using/assets/dmclassic-login1.png)

1. Verwenden Sie zum Anmelden bei der Adobe Dynamic Media Classic-Desktop-App dieselben Anmeldeinformationen wie beim Anmelden bei Adobe Dynamic Media Classic im Browser.

   Informationen zur Verwendung **[!UICONTROL Servers]** finden Sie in der folgenden Zuordnung für die Produktionsumgebung:

   | Server | Browser-URL |
   | --- | --- |
   | NA Production (Nordamerika) | https://s7sps1.scene7.com/ |
   | EMEA-Produktion (Europa, Naher Osten und Afrika) | https://s7sps3.scene7.com/ |
   | APAC-Produktion (Asien-Pazifik) | https://s7sps5.scene7.com/ |

## Videoanleitung zur Verwendung des Adobe Dynamic Media Classic-Desktop-Programms {#dmc-app-video-walk-through}

Sehen Sie sich [&#x200B; Videoanleitung zur Verwendung des Adobe Dynamic Media Classic-Desktop-Programms &#x200B;](https://experienceleague.adobe.com/de/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application#dynamic-media) (Länge: 2 Minuten 36 Sekunden).

## Löschen des Bild- und Asset-Cache auf dem Computer mithilfe des Desktop-Programms {#clear-cache}

1. Tippen Sie im Adobe Dynamic Media Classic-Desktop-Programm rechts oben auf **[!UICONTROL Setup]** > **[!UICONTROL Persönliches Setup]**.
1. Führen Sie auf **[!UICONTROL Seite]** Persönliches Setup“ unter der Überschrift **[!UICONTROL Desktop]** einen der folgenden Schritte aus:
   * Um alle in Adobe Dynamic Media zwischengespeicherten Bilddateien von Ihrem Computer zu entfernen, tippen Sie auf **[!UICONTROL Bildcache löschen]** und dann auf **[!UICONTROL OK]**.
   * Um alle in Adobe Dynamic Media zwischengespeicherten Asset-Dateien von Ihrem Computer zu entfernen, tippen Sie auf **[!UICONTROL Asset-Cache löschen]** und dann auf **[!UICONTROL OK]**.
1. Tippen Sie unten rechts auf der Seite auf **[!UICONTROL Schließen]**.

### Manuelles Löschen des Bild- und Asset-Cache

Neben dem Löschen des Bild- und Asset-Cache mithilfe des -Desktop-Programms können Sie den Cache auch manuell direkt aus dem Dateisystem löschen.

1. Gehen Sie je nach Betriebssystem wie folgt vor:

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Bekannte Einschränkungen in Adobe Dynamic Media Classic 20.21.1

* Die Dropdown-Liste **[!UICONTROL Server]** ist nach der Aktualisierung auf Adobe Dynamic Media Classic Desktop-Programm 20.21.1 leer: Szenario: Sie installieren und melden sich bei Adobe Dynamic Media Classic 20.20.1 oder 20.20.2 an und schließen dann die Anwendung. Dann aktualisieren Sie auf Adobe Dynamic Media Classic 20.21.1. Wenn Sie versuchen, sich anzumelden, ist die Dropdown **[!UICONTROL Liste]** Server“ im Dialogfeld **[!UICONTROL Bei Konto anmelden]** leer. Um dieses Problem zu umgehen, müssen Sie [den Cache manuell löschen](#clear-cache) (siehe oben stehende Schritte).

## Bekannte Einschränkungen in Adobe Dynamic Media Classic 20.20.1 (behoben in 20.20.2)

**_Gilt nur für Windows® - Gibt es eine Begrenzung für die Anzahl der Dateien, die über die Benutzeroberfläche des Desktop-Programms hochgeladen werden können?_**<br>Ja, es können maximal 150 Dateien gleichzeitig über die Benutzeroberfläche des Desktop-Programms hochgeladen werden.

**_Gilt für Windows® und macOS - Wie wechsele ich zwischen Unternehmen?_**<br>Um zwischen Unternehmen zu wechseln, gehen Sie wie folgt vor:

* Wählen Sie in der Adobe Dynamic Media Classic-App das neue Unternehmen aus der Dropdown-Liste Firma aus.
* Wenn das Popup-Fenster angezeigt wird, tippen Sie auf **[!UICONTROL OK]**, um sich abzumelden und die App zu schließen.

  ![Um das neue Unternehmen zu verwenden, starten Sie die App neu](/help/using/assets/dmclassic-new-company1.png)

* Starten Sie Adobe Dynamic Media Classic neu und melden Sie sich wie gewohnt an, um mit dem neuen Unternehmen zu arbeiten.

## Best Practices

***Ich kann das Medienportal-Bedienfeld auf der Landingpage von Adobe Dynamic Media Classic nicht sehen.***<br>Tippen Sie in Adobe Dynamic Media Classic auf **[!UICONTROL Setup > Persönliches Setup]**. Stellen Sie im Browser-Bereich sicher **[!UICONTROL dass „MediaPortal-Funktionen]**&quot; ausgewählt (aktiviert) ist. Tippen Sie auf **[!UICONTROL Speichern > Schließen]**.

***Veröffentlichungsstatus (grüner Indikator) eines Assets wird nicht korrekt angezeigt.***<br>In der Browser-Benutzeroberfläche war eine erneute Anmeldung bei der Benutzeroberfläche erforderlich, um den korrekten Veröffentlichungsstatus von Assets anzuzeigen. In der Desktop-Anwendung hat Adobe ein **[!UICONTROL Aktualisieren]**-Symbol in der Symbolleiste rechts neben der Schaltfläche **[!UICONTROL Keine auswählen]** hinzugefügt. Um den neuesten Status aller Assets auf der angegebenen Seite anzuzeigen, tippen Sie auf das Symbol **[!UICONTROL Aktualisieren]**. Wie bei der Browser-Benutzeroberfläche ist keine erneute Authentifizierung erforderlich.

![Aktualisierungssymbol](/help/using/assets/refresh-icon1.png)
*Aktualisierungssymbol*

***In der Desktop-Anwendung funktionieren keine Stapelsatzvorgaben.***<br>Tippen Sie auf **[!UICONTROL Hochladen > Auftragsoptionen > Stapelsatzvorgaben]**. Stellen Sie sicher **[!UICONTROL dass die entsprechende Stapelsatzvorgabe]** ist. Klicken Sie **[!UICONTROL Speichern und Upload starten]**.
