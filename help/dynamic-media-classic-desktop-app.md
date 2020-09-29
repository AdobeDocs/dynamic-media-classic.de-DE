---
title: Adobe Dynamic Media Classic Desktop-App - jetzt verfügbar
seo-title: Adobe Dynamic Media Classic Desktop-App - jetzt verfügbar
description: 'null'
seo-description: Erfahren Sie mehr über die Desktop-App "Dynamic Media Classic".
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
translation-type: tm+mt
source-git-commit: 477a8fd6ffee00cd586d91f6eeda8e676753a90f
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 0%

---


# Jetzt verfügbar: Adobe Dynamic Media Classic Desktop-App {#dynamic-media-classic-desktop-app}

Benutzer von Dynamic Media Classic haben jetzt Zugriff auf eine neue Desktop-App, die nicht mehr auf Adobe Flash-Technologie im Browser zurückgreift.

Diese neue App ist jetzt für Windows und macOS verfügbar.

>[!IMPORTANT]
>
>Es wird empfohlen, die neue Adobe Dynamic Media Classic Desktop-App bis zum 1. Oktober 2020 zu installieren. Dadurch erhalten Sie eine reibungslose Transition, bevor der Flash Player der Adobe am 31. Dezember 2020 eingestellt wird. Ab diesem Datum können Sie sich nicht mehr bei der Browserversion der Benutzeroberfläche von Adobe Dynamic Media Classic anmelden, die im Produkt als &quot;Dynamischer Medienklassiker&quot;gekennzeichnet ist.

In den häufig gestellten Fragen finden Sie jetzt Informationen zur Anmeldung bei [New Dynamic Media Classic.](/help/new-ui-2020.md)

## Systemanforderungen für die Adobe der Dynamischen Media Classic-Desktop-App {#system-requirements-dmc-app}

Die Desktop-App &quot;Adobe Dynamic Media Classic&quot;ist mit den folgenden Betriebssystemen kompatibel:
* macOS X 10.10 oder neuer.
* Windows 7 oder neuer.

## Herunterladen und Installieren der Adobe Dynamic Media Classic Desktop-App unter Mac OS oder Windows {#installation-dmc-app}

Verwandte Themen:

* [Download und *unbeaufsichtigte* Installation der Adobe Dynamic Media Classic für die Desktop-App unter MacOS](#install-silent-mac-dmc-app)
* [Herunterladen und *automatische* Installation der Adobe Dynamic Media Classic für die Desktop-Anwendung unter Windows](#install-silent-windows-dmc-app)

1. Deinstallieren Sie alle älteren Desktop-App-Versionen von Dynamic Media Classic auf Ihrem System.

1. Laden Sie das neueste Installationsprogramm für die Desktop-App &quot;Adobe Dynamic Media Classic&quot;herunter.

   * [macOS (.DMG) - Herunterladen.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.dmg)
   * [Windows (.EXE) - Herunterladen.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.exe)

1. Führen Sie je nach heruntergeladenem Installationsprogramm einen der folgenden Schritte aus:

   * **Für macOS** : Ziehen Sie im Dialogfeld &quot; **[!UICONTROL Drag &amp; Drop zur Installation]** &quot;die **[!UICONTROL Adobe Dynamic Media Classic]** und legen Sie sie in **[!UICONTROL Anwendungen]** ab.

      ![Drag &amp; Drop der Installation unter macOS](/help/assets/dragondrop-install1.png)

   * Tippen Sie im Ordner **[!UICONTROL Applications]** auf das Symbol Adobe Dynamic Media Classic.
   * Tippen Sie im Dialogfeld auf **[!UICONTROL Öffnen]** , um die Desktop-App &quot;Adobe Dynamic Media Classic&quot;zu öffnen.

      ![Heruntergeladene App öffnen](/help/assets/open-dmclassicapp1.png)

   * **Windows** : Führen Sie die Binärdatei des Installationsprogramms aus und befolgen Sie die Anweisungen auf dem Bildschirm, um die Desktop-App zu installieren.

1. Wenn Sie die Anwendung öffnen, wird die neue Anmeldeseite für die dynamische Medienklassifizierung angezeigt:

   ![Anmeldung bei Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Verwenden Sie dieselben Anmeldedaten wie Ihr Browser, um sich bei Adobe Dynamic Media Classic anzumelden.

   Informationen zur Verwendung des **[!UICONTROL Servers]** finden Sie in der folgenden Zuordnung für die Produktions-Umgebung:

   | Browser-URL | Servername der Desktop-App |
   |---|---|
   | https://s7sps1.scene7.com/ | Produktion der NA (Nordamerika) |
   | https://s7sps3.scene7.com/ | Produktion von EMEA (Europa, Naher Osten und Afrika) |
   | https://s7sps5.scene7.com/ | APAC-Produktion (Asien-Pazifik) |

1. Wenn Sie die Benutzeroberfläche für die Anmeldung posten, werden Sie das übliche Benutzeroberflächenerlebnis des Browsers bemerken. Sie können Ihre tägliche Aktivität jetzt wie gewohnt in der Benutzeroberfläche der Desktop-App übernehmen.

## Download und *unbeaufsichtigte* Installation der Adobe Dynamic Media Classic für die Desktop-App unter MacOS {#install-silent-mac-dmc-app}

Verwandte Themen:

* [Herunterladen und Installieren der Adobe Dynamic Media Classic-Desktop-App unter Mac oder Windows](#installation-dmc-app)
* [Herunterladen und *automatische* Installation der Adobe Dynamic Media Classic für die Desktop-Anwendung unter Windows](#install-silent-windows-dmc-app)

So laden Sie die Adobe Dynamic Media Classic für die Desktop-App unter macOS herunter und *installieren sie* unbeaufsichtigt:

1. Deinstallieren Sie alle älteren Desktop-App-Versionen von Dynamic Media Classic auf Ihrem System.

1. Laden Sie das neueste Installationsprogramm für die Desktop-App &quot;Adobe Dynamic Media Classic&quot;für macOS herunter.

   * [macOS (.DMG) - Herunterladen.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.dmg)

1. Laden Sie das heruntergeladene Disk Image (.DMG) mithilfe des folgenden Befehls an einen Speicherort für den Mountpoint herunter:

   `hdiutil attach adobe-dynamic-media-classic-20.20.1.dmg -mountpoint <mount_point_path>`

1. Kopieren Sie die APP-Datei mit dem folgenden Befehl in **[!UICONTROL Anwendungen]** :

   `rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
Unmount DMG - hdiutil detach <mount_point_path>`

1. Wenn Sie die Anwendung öffnen, wird die Anmeldeseite der neuen Adobe &quot;Dynamische Medien - Classic&quot;angezeigt:

   ![Anmeldung bei Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Verwenden Sie dieselben Anmeldedaten wie Ihr Browser, um sich bei Adobe Dynamic Media Classic anzumelden.

   Informationen zur Verwendung des **[!UICONTROL Servers]** finden Sie in der folgenden Zuordnung für die Produktions-Umgebung:

   | Browser-URL | Servername der Desktop-App |
   |---|---|
   | https://s7sps1.scene7.com/ | Produktion der NA (Nordamerika) |
   | https://s7sps3.scene7.com/ | Produktion von EMEA (Europa, Naher Osten und Afrika) |
   | https://s7sps5.scene7.com/ | APAC-Produktion (Asien-Pazifik) |

## Herunterladen und *automatische* Installation der Adobe Dynamic Media Classic für die Desktop-Anwendung unter Windows {#install-silent-windows-dmc-app}

Der von Ihnen verwendete Befehl ist für eine einfache, unbeaufsichtigte MSI-Installation vorgesehen. Das Installationsprogramm für die Desktop-Anwendung &quot;Dynamic Media Classic&quot;ist jedoch ein InstallScript-MSI-Installationsprogramm, das mit InstallShield erstellt wurde. Wenn Sie das Installationsprogramm im Datensatzmodus ausführen, wird jede Benutzerinteraktion in einer Antwortdatei aufgezeichnet. Diese Antwortdatei wird dann für eine unbeaufsichtigte Installation verwendet, wie unter [Ausführen von Installationen im Hintergrund beschrieben.](https://docs.flexera.com/installshield19helplib/helplibrary/SilentInstall.htm)

Verwandte Themen:

* [Herunterladen und Installieren der Adobe Dynamic Media Classic-Desktop-App unter Mac oder Windows](#installation-dmc-app)
* [Herunterladen und *automatische* Installation der Adobe Dynamic Media Classic für die Desktop-Anwendung unter Windows](#install-silent-windows-dmc-app)

So laden Sie die Adobe Dynamic Media Classic für die Desktop-App unter Windows herunter und *installieren sie* im Hintergrund

1. Deinstallieren Sie alle älteren Desktop-App-Versionen von Dynamic Media Classic auf Ihrem System.

1. Laden Sie das neueste Installationsprogramm für die Desktop-App &quot;Adobe Dynamic Media Classic&quot;herunter.

   * [Windows (.EXE) - Herunterladen.](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.exe)

1. Führen Sie das Installationsprogramm mit dem folgenden Befehl im Datensatzmodus aus:

   `adobe-dynamic-media-classic-20.20.1.exe /r /f1"C:\Setup.iss"`

1. Führen Sie im Fenster des GUI-Installationsprogramms die Installationsschritte aus, damit Interaktionen/Eingaben, wie z. B. der Installationsort, in der `Setup.iss` Datei aufgezeichnet werden.

1. Kopieren Sie die erstellte `Setup.iss` Datei und `adobe-dynamic-media-classic-20.20.1.exe` auf einen anderen Computer.

1. Führen Sie den folgenden Befehl für eine unbeaufsichtigte Installation aus:

   `adobe-dynamic-media-classic-20.20.1.exe /s /f1"C:\Setup.iss"`

   Details zu Befehlszeilenparametern finden Sie unter [Setup.exe und Update.exe Befehlszeilenparameter.](https://docs.flexera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. Wenn Sie die Anwendung öffnen, wird die Anmeldeseite der neuen Adobe &quot;Dynamische Medien - Classic&quot;angezeigt:

   ![Anmeldung bei Dynamic Media Classic](/help/assets/dmclassic-login1.png)

1. Verwenden Sie dieselben Anmeldedaten wie Ihr Browser, um sich bei Adobe Dynamic Media Classic anzumelden.

   Informationen zur Verwendung des **[!UICONTROL Servers]** finden Sie in der folgenden Zuordnung für die Produktions-Umgebung:

   | Browser-URL | Servername der Desktop-App |
   |---|---|
   | https://s7sps1.scene7.com/ | Produktion der NA (Nordamerika) |
   | https://s7sps3.scene7.com/ | Produktion von EMEA (Europa, Naher Osten und Afrika) |
   | https://s7sps5.scene7.com/ | APAC-Produktion (Asien-Pazifik) |


## Video-Anleitung zur Verwendung der Desktop-App &quot;Dynamic Media Classic&quot;

Sehen Sie sich einen [Video-Durchgang zur Verwendung der Desktop-App](https://docs.adobe.com/content/help/en/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html) &quot;Dynamic Media Classic&quot;an (Länge: 2 Minuten, 36 Sekunden).

## Bekannte Einschränkungen in Dynamic Media Classic

**_Gilt nur für Windows - Gibt es eine Beschränkung für die Anzahl der Dateien, die über die Benutzeroberfläche der Desktop-App hochgeladen werden können?_**<br>Ja. Über die Benutzeroberfläche der Desktop-App können maximal 150 Dateien gleichzeitig hochgeladen werden.

**_Gilt für Windows und macOS - Wie kann ich zwischen Firmen wechseln?_**<br>Gehen Sie wie folgt vor, um zwischen Firmen zu wechseln:
* Wählen Sie in der App &quot;Dynamic Media Classic&quot;in der Dropdown-Liste &quot;Firma&quot;die neue Firma aus.
* Wenn das Popup angezeigt wird, tippen Sie auf **[!UICONTROL OK]** , um sich abzumelden und die App zu schließen.

   ![Starten Sie die App neu, um die neue Firma zu verwenden](/help/assets/dmclassic-new-company1.png)
* Starten Sie Dynamische Medien Classic neu und melden Sie sich wie gewohnt an, um mit der neuen Firma zu arbeiten.

## Tipps und Tricks

**_Das Warenkorbbedienfeld auf der Landingpage von Dynamic Media Classic kann nicht angezeigt werden._**<br>Tippen Sie in Dynamic Media Classic auf**[!UICONTROL Einstellungen > Persönliche Einstellungen ]**. Vergewissern Sie sich, dass im Abschnitt Browser die Option MediaPortal-Funktionen****anzeigen ausgewählt ist (aktiviert). Tippen Sie auf**[!UICONTROL Speichern > Schließen ]**.

**_Der Veröffentlichungsstatus (grüne Anzeige) eines Assets wird nicht korrekt dargestellt._**<br>In der Browser-Benutzeroberfläche war eine erneute Anmeldung bei der Benutzeroberfläche erforderlich, um den korrekten Veröffentlichungsstatus der Assets anzuzeigen. In der Desktop-App wurde in der Symbolleiste rechts neben der Schaltfläche &quot;Keine**[!UICONTROL auswählen&quot;das Symbol &quot;]**Aktualisieren**[!UICONTROL &quot;eingeführt ]**. Tippen Sie auf das Symbol &quot;**[!UICONTROL Aktualisieren ]**&quot;, um den neuesten Status aller Assets auf der jeweiligen Seite anzuzeigen. Es ist keine erneute Anmeldung erforderlich, wie bei der Browser-Benutzeroberfläche.

![Symbol](/help/assets/refresh-icon1.png)*Aktualisieren*

**_Stapelsatzvorgaben funktionieren nicht in der Desktop-App._**<br>Tippen Sie auf**[!UICONTROL Hochladen > Auftragsoptionen > Stapelsatzvorgaben ]**. Stellen Sie sicher, dass die entsprechende**[!UICONTROL Stapelsatzvorgabe ]**aktiviert ist. Klicken Sie auf**[!UICONTROL Speichern und Hochladen ]**senden.
