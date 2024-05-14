---
title: Konfigurieren von Adobe Analytics-Berichten
description: Erfahren Sie, wie Sie Adobe Analytics-Berichte in Adobe Dynamic Media Classic konfigurieren.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
topic: Integrations, Development
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '1234'
ht-degree: 18%

---

# Konfigurieren von Adobe Analytics-Berichten{#configuring-adobe-analytics-reports}

Um Adobe Analytics mitzuteilen, welche Informationen Sie in Adobe Analytics-Berichten erhalten möchten, rufen Sie den Bildschirm Adobe Analytics-Konfiguration auf. In diesem Bildschirm werden nach Ihren Konfigurationsberichten für jedes Viewer-Ereignis, über das Sie Informationen erhalten möchten, eine entsprechende Adobe Analytics-Variable und Adobe Dynamic Media Classic-Variable aufgeführt. Diese Viewer-Ereignisse - Variablenkombinationen Adobe Analytics und Adobe Dynamic Media Classic bestimmen, welche Informationen gemeldet werden.

Neben der Zuordnung von Viewer-Ereignissen zu Variablen bietet der Bildschirm &quot;Adobe Analytics-Konfiguration&quot;Tools zum Aktivieren, Bearbeiten und Löschen von Viewer-Ereignissen.

>[!NOTE]
>
>Wenn Sie die Adobe Analytics-Berichtseinstellungen in Adobe Analytics ändern, stellen Sie sicher, dass Sie sich von Adobe Dynamic Media Classic aus wieder bei Adobe Analytics anmelden, Ihre Adobe Analytics-Konfigurationseinstellungen speichern und dann erneut veröffentlichen.

Siehe [Bei Adobe Analytics anmelden](log-analytics.md#log_in_to_adobe_analytics).

Siehe [Konfigurationsinformationen veröffentlichen](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Zuweisen von Adobe Analytics-Variablen zu Adobe Dynamic Media Classic-Viewer-Ereignissen und -Variablen {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Verknüpfen Sie im Bildschirm &quot;Adobe Analytics-Konfiguration&quot;Viewer-Ereignisse mit Adobe Analytics-Variablen und Adobe Dynamic Media Classic-Variablen. Wählen Sie für jedes Viewer-Ereignis eine Adobe Analytics-Variable und eine Adobe Dynamic Media Classic-Variable aus. Anweisungen zum Öffnen des Bildschirms &quot;Adobe Analytics-Konfiguration&quot;finden Sie unter [Bei Adobe Analytics anmelden](log-analytics.md#log_in_to_adobe_analytics).

**So weisen Sie Adobe Dynamic Media Classic-Viewer-Ereignissen und -Variablen Adobe Analytics-Variablen zu:**

1. Nachdem Sie sich von Dynamic Media Classic aus bei Adobe Analytics angemeldet und eine Report Suite ausgewählt haben, aktivieren Sie auf der Seite &quot;Adobe Analytics-Konfiguration&quot;in der rechten Tabellenspalte ein Viewer-Ereignis, indem Sie **[!UICONTROL Aktivieren]**.
1. Zeigen Sie unter der Spalte Variablen die Variablenpaarauswahl an, indem Sie die Pfeilschaltfläche für das gewünschte Viewer-Ereignis auswählen.

   Siehe [Viewer-Ereignisse](configuring-analytics-reports.md#viewer_events).

1. Fügen Sie eine Adobe Dynamic Media Classic-Variable hinzu.

   Siehe [Adobe Dynamic Media Classic-Variablen](configuring-analytics-reports.md#scene7_variables).

1. Fügen Sie eine Adobe Analytics-Variable hinzu.
1. (Optional) Um ein weiteres Variablenpaar hinzuzufügen, wählen Sie **[!UICONTROL Hinzufügen]**.
1. Auswählen **[!UICONTROL Speichern]**.

   Nachdem Sie **[!UICONTROL Speichern]**, werden das Viewer-Ereignis, die zugehörige Adobe Analytics-Variable und die Adobe Dynamic Media Classic-Variable im Bildschirm &quot;Adobe Analytics-Konfiguration&quot;aufgeführt.

1. Wählen Sie in der rechten unteren Ecke die Option **[!UICONTROL Schließen]**.
1. Navigieren Sie zu **[!UICONTROL Veröffentlichen]** > **[!UICONTROL Veröffentlichen senden]** , um eine Image Serving-Veröffentlichung auszuführen.

   Die Veröffentlichung ist erforderlich, damit die in den Viewern enthaltenen Informationen auf den Adobe Dynamic Media Classic-Servern verfügbar sind.

### Viewer-Ereignisse {#viewer-events}

Viewer-Ereignisse beschreiben Aktionen, die Benutzer mit Dynamic Media Classic-Viewern ausführen. Wenn ein Benutzer eine Aktion auslöst, z. B. eine Miniaturansicht auswählt oder ein Video startet oder stoppt, &quot;sendet&quot;der Viewer ein Ereignis an die Webseite. Mit diesem Ereignis verknüpfte Daten werden ebenfalls gesendet.

In der folgenden Tabelle werden Viewer-Ereignisse beschrieben, die Sie dem Bildschirm &quot;Adobe Analytics-Konfiguration&quot;hinzufügen können.

| Viewer-Ereignis | Unterstützung und Viewer für die HTML5 Viewer-Plattform | Beschreibung |
| --- | --- | --- |
| LOAD | **X** (E-Katalog, Flyout, Rotationsset, Video, Zoom) | Wenn ein Benutzer einen Viewer startet |
| PAGE | **X** (E-Katalog) | Wenn ein Benutzer in E-Katalogen eine Seite umdreht, in zielgerichteten Zoom-Viewern ein anderes Ziel oder ein Farbmuster auswählt. |
| SWAP | **X** (E-Katalog, Flyout, Rotationsset, Video, Zoom) | Wenn ein Benutzer eine andere Miniaturansicht auswählt, um ein anderes Bild anzuzeigen. |
| ITEM | **X** (E-Katalog) | Wenn ein Benutzer in Viewern, die Imagemaps unterstützen, in denen Rollover definiert sind, mit der Maus auf eine Imagemap zeigt, um den Rollover-Text zu lesen |
| HREF | **X** (E-Katalog) | In Viewern, die Imagemaps unterstützen, wenn ein Benutzer eine URL in einer Imagemap auswählt. |
| TARGET | | Wenn ein Benutzer in zielgerichteten Zoom-Viewern ein Zoomziel auswählt, um einen Teil eines Bildes zu vergrößern. |
| SEARCH | | Wenn ein Benutzer in E-Katalogen eine Wortsuche durchführt |
| PLAY | **X** (Video) | Wenn ein Benutzer in Video-Viewern Play auswählt, um mit der Wiedergabe eines Videos zu beginnen.<br><br>**Hinweis:** Wenn Sie Heartbeat-basierte Videoberichte von Adobe Analytics verwenden, müssen Sie diesem Viewer-Ereignis keine Variablen zuordnen, wenn Sie Adobe Analytics in Adobe Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit nativen Adobe Dynamic Media Classic HTML5 Video- und MixedMedia-Viewern. Der Videoplayer generiert Tracking-Daten zur Anzeige in Adobe Analytics-Videoberichten. Siehe [Adobe Analytics-Videoberichte aktivieren](enabling-analytics-video-reports.md). |
| PAUSE | **X** (Video) | Wenn ein Benutzer in Video-Viewern **[!UICONTROL Anhalten]** um ein Video einzufrieren.<br><br>**Hinweis:** Wenn Sie Heartbeat-basierte Videoberichte von Adobe Analytics verwenden, müssen Sie diesem Viewer-Ereignis keine Variablen zuordnen, wenn Sie Adobe Analytics in Adobe Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit nativen Adobe Dynamic Media Classic HTML5 Video- und MixedMedia-Viewern. Der Videoplayer generiert Tracking-Daten zur Anzeige in Adobe Analytics-Videoberichten. Siehe [Adobe Analytics-Videoberichte aktivieren](enabling-analytics-video-reports.md). |
| STOP | **X** (Video) | Wenn ein Benutzer in Video-Viewern **[!UICONTROL Anhalten]** , um die Wiedergabe eines Videos zu beenden.<br><br>**Hinweis:** Wenn Sie Heartbeat-basierte Videoberichte von Adobe Analytics verwenden, müssen Sie diesem Viewer-Ereignis keine Variablen zuordnen, wenn Sie Adobe Analytics in Adobe Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit nativen Adobe Dynamic Media Classic HTML5 Video- und MixedMedia-Viewern. Der Videoplayer generiert Tracking-Daten zur Anzeige in Adobe Analytics-Videoberichten. Siehe [Adobe Analytics-Videoberichte aktivieren](enabling-analytics-video-reports.md). |
| MILESTONE | **X** (Video) | In Video-Viewern werden Meilensteinereignisse generiert, wenn der Benutzer jeweils 0, 25, 50, 75 oder 100 Prozent des Videos gesehen hat.<br><br>**Hinweis:** Wenn Sie Heartbeat-basierte Videoberichte von Adobe Analytics verwenden, müssen Sie diesem Viewer-Ereignis keine Variablen zuordnen, wenn Sie Adobe Analytics in Adobe Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit nativen Adobe Dynamic Media Classic HTML5 Video- und MixedMedia-Viewern. Der Videoplayer generiert Tracking-Daten zur Anzeige in Adobe Analytics-Videoberichten. Siehe [Adobe Analytics-Videoberichte aktivieren](enabling-analytics-video-reports.md). |
| SWATCH | **X** (Flyout, Zoom) | Dieses Viewer-Ereignis wird dem SEITEN-Viewer-Ereignis in Adobe Dynamic Media Classic zugeordnet. |
| ZOOM | **X** (E-Katalog, Rotationsset, Zoom) | Wird nicht von Adobe Analytics verfolgt. |
| PAN | **X** (E-Katalog, Rotationsset, Zoom) | Wird nicht von Adobe Analytics verfolgt. |
| SPIN | **X** (Rotationsset) | Wird nicht von Adobe Analytics verfolgt. |

### Adobe Dynamic Media Classic-Variablen {#scene-variables}

Wählen Sie für jedes Viewer-Ereignis auf dem Bildschirm &quot;Adobe Analytics-Konfiguration&quot;eine Adobe Analytics-Variable und eine *Adobe Dynamic Media Classic-Variable*. Adobe Dynamic Media Classic-Variablen stellen Daten dar, die Sie für einen Bericht abrufen können. Beispiel: die `searchTerm` enthält Suchbegriffe, die in E-Katalog-Suchvorgängen verwendet werden.

In der folgenden Tabelle werden Adobe Dynamic Media Classic-Variablen beschrieben:

| Adobe Dynamic Media Classic-Variable | Beschreibung |
| --- | --- |
| asset | Adobe Dynamic Media Classic-Asset-ID oder Videopfaddatei. |
| viewerId | Eine beliebige Zahl, die den verschiedenen Viewertypen zugeordnet wird. |
| pageLabel | Die Seite, die von einem Viewer in E-Katalogen angezeigt wird. |
| label | Der Beschriftungswert (eine Zeichenfolge). |
| frame | Die Seiten- oder Seitenreferenz in einem Bildset. |
| rollover_keyRaw | Der gesamte HREF-Wert, nicht nur ein verarbeiteter Teil. |
| rollover_keyProc | Die ID eines Elements, auf das in einer Imagemap verwiesen wird (gültig für Href- und Elementereignisse). |
| searchTerm | Ein Begriff, der bei der Suche in E-Katalogen verwendet wird. |
| timeStamp | In Video-Viewern ausgewählte Optionen &quot;Abspielen&quot;, &quot;Beenden&quot;und &quot;Pause&quot;. |
| progress | Der abgeschlossene Prozentsatz eines Meilensteinereignisses. |
| targetId | Der ID-Wert (eine Zahl). |

## Viewer-Ereignisse aktivieren, bearbeiten und löschen {#activating-editing-and-deleting-viewer-events}

Im Anzeigebereich „Adobe Analytics-Konfiguration“ können Sie Viewer-Ereignisse aktivieren, bearbeiten und löschen:

* **Aktivieren** - Auswählen **[!UICONTROL Aktivieren]** aktivieren oder **[!UICONTROL Deaktivieren]** , um ein ausgewähltes Viewer-Ereignis zu deaktivieren.

* **Bearbeiten** - Wählen Sie ein Viewer-Ereignis aus und wählen Sie die **[!UICONTROL Anzeigen/Bearbeiten]** Variablengrauschaltfläche. Wählen Sie in den Dropdownlisten Adobe Dynamic Media Classic-Variable und Adobe Analytics-Variable eine andere Variable aus den jeweiligen Listen aus. Weitere Informationen finden Sie unter [Zuweisen von Adobe Analytics-Variablen zu Adobe Dynamic Media Classic-Viewer-Ereignissen und -Variablen](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables).

* **Löschen** - Wählen Sie ein Viewer-Ereignis aus und wählen Sie die **[!UICONTROL Anzeigen/Bearbeiten]** Variablengrauschaltfläche. Auswählen **[!UICONTROL Löschen]**.
