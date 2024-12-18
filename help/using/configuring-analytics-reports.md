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
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1234'
ht-degree: 18%

---

# Konfigurieren von Adobe Analytics-Berichten{#configuring-adobe-analytics-reports}

Um Adobe Analytics mitzuteilen, welche Informationen Sie in Adobe Analytics-Berichten benötigen, wechseln Sie zum Bildschirm Adobe Analytics-Konfiguration . Im Anschluss an Ihre Konfigurationsberichte listet dieser Bildschirm für jedes Viewer-Ereignis, zu dem Sie Informationen benötigen, eine entsprechende Adobe Analytics-Variable und eine entsprechende Adobe Dynamic Media Classic-Variable auf. Diese Viewer-Ereignisse-Adobe Analytics-Variablen-Adobe Dynamic Media Classic-Variablenkombinationen bestimmen, welche Informationen gemeldet werden.

Neben der Verknüpfung von Viewer-Ereignissen mit Variablen bietet der Adobe Analytics-Konfigurationsbildschirm Tools zum Aktivieren, Bearbeiten und Löschen von Viewer-Ereignissen.

>[!NOTE]
>
>Wenn Sie Adobe Analytics-Berichteinstellungen in Adobe Analytics ändern, müssen Sie sich von Adobe Dynamic Media Classic aus wieder bei Adobe Analytics anmelden, Ihre Adobe Analytics-Konfigurationseinstellungen erneut speichern und dann erneut veröffentlichen.

Siehe [Anmelden bei Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Siehe [Publish-Konfigurationsinformationen](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Zuweisen von Adobe Analytics-Variablen zu Adobe Dynamic Media Classic-Viewer-Ereignissen und -Variablen {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Verwenden Sie den Adobe Analytics-Konfigurationsbildschirm, um Viewer-Ereignisse mit Adobe Analytics-Variablen und Adobe Dynamic Media Classic-Variablen zu verknüpfen. Wählen Sie für jedes Viewer-Ereignis eine Adobe Analytics-Variable und eine Adobe Dynamic Media Classic-Variable aus. Anweisungen zum Öffnen des Adobe Analytics-Konfigurationsbildschirms finden Sie unter [Bei Adobe Analytics anmelden](log-analytics.md#log_in_to_adobe_analytics).

**So weisen Sie Adobe Dynamic Media Classic-Viewer-Ereignissen und -Variablen Adobe Analytics-Variablen zu:**

1. Nachdem Sie sich von Dynamic Media Classic aus bei Adobe Analytics angemeldet und eine Report Suite ausgewählt haben, aktivieren Sie auf der Seite &quot;Adobe Analytics-Konfiguration“ in der rechten Tabellenspalte ein Viewer-Ereignis, indem Sie **[!UICONTROL Aktivieren]** auswählen.
1. Zeigen Sie in der Spalte Variablen die Variablenpaar-Auswahl an, indem Sie die Pfeilschaltfläche für das gewünschte Viewer-Ereignis auswählen.

   Siehe [Viewer-Ereignisse](configuring-analytics-reports.md#viewer_events).

1. Hinzufügen einer Adobe Dynamic Media Classic-Variablen.

   Siehe [Adobe Dynamic Media Classic-Variablen](configuring-analytics-reports.md#scene7_variables).

1. Fügen Sie eine Adobe Analytics-Variable hinzu.
1. (Optional) Um ein weiteres Variablenpaar hinzuzufügen, wählen Sie **[!UICONTROL Hinzufügen]** aus.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

   Nachdem Sie **[!UICONTROL Speichern]** ausgewählt haben, werden das Viewer-Ereignis, die zugehörige Adobe Analytics-Variable und die zugehörige Adobe Dynamic Media Classic-Variable im Adobe Analytics-Konfigurationsbildschirm aufgeführt.

1. Klicken Sie in der rechten unteren Ecke auf **[!UICONTROL Schließen]**.
1. Wechseln Sie zu **[!UICONTROL Publish]** > **[!UICONTROL Publish übermitteln]**, um eine Image-Serving-Veröffentlichung auszuführen.

   Die Veröffentlichung ist erforderlich, damit die in den Viewern enthaltenen Informationen auf Adobe Dynamic Media Classic-Servern verfügbar sind.

### Viewer-Ereignisse {#viewer-events}

Viewer-Ereignisse beschreiben Aktionen, die Benutzende mit Dynamic Media Classic-Viewern ausführen. Wenn ein Benutzer eine Aktion initiiert, z. B. ein Miniaturbild auswählen oder ein Video starten oder stoppen, „sendet“ der Viewer ein Ereignis an die Web-Seite. Daten, die mit diesem Ereignis verknüpft sind, werden ebenfalls gepusht.

In der folgenden Tabelle werden Viewer-Ereignisse beschrieben, die Sie dem Adobe Analytics-Konfigurationsbildschirm hinzufügen können.

| Viewer-Ereignis | Unterstützung und Viewer für die HTML5 Viewer-Plattform | Beschreibung |
| --- | --- | --- |
| LOAD | **X** (E-Katalog, Flyout, Rotationsset, Video, Zoom) | Wenn ein Benutzer einen Viewer startet |
| PAGE | **X** (E-Katalog) | Wenn ein(e) Benutzende(r) in E-Katalogen eine Seite umblättert, in zielgerichteten Zoom-Viewern ein anderes Ziel oder ein Farbfeld auswählt. |
| SWAP | **X** (E-Katalog, Flyout, Rotationsset, Video, Zoom) | Wenn Benutzende eine andere Miniaturansicht auswählen, um ein anderes Bild anzuzeigen. |
| ITEM | **X** (E-Katalog) | Wenn ein Benutzer in Viewern, die Imagemaps unterstützen, in denen Rollover definiert sind, mit der Maus auf eine Imagemap zeigt, um den Rollover-Text zu lesen |
| HREF | **X** (E-Katalog) | Wählen Sie in Viewern, die Imagemaps unterstützen, eine URL in einer Imagemap aus. |
| TARGET | | In zielgerichteten Zoom-Viewern gilt Folgendes: Wenn ein Benutzer ein Zoom-Ziel auswählt, um auf einen Teil eines Bildes zu zoomen. |
| SEARCH | | Wenn ein Benutzer in E-Katalogen eine Wortsuche durchführt |
| PLAY | **X** (Video) | In Video-Viewern, wenn ein Benutzer Abspielen auswählt, um die Wiedergabe eines Videos zu starten.<br><br>**Hinweis:** Wenn Sie Adobe Analytics Heartbeat-basierte Videoberichte verwenden, müssen Sie diesem Viewer-Ereignis keine Variablen zuordnen, wenn Sie Adobe Analytics in Adobe Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit nativen Adobe Dynamic Media Classic HTML5-Video- und MixedMedia-Viewern. Der Video-Player generiert Tracking-Daten zur Anzeige in Adobe Analytics-Videoberichten. Siehe [Aktivieren von Adobe Analytics-Videoberichten](enabling-analytics-video-reports.md). |
| PAUSE | **X** (Video) | In Video-Viewern, wenn Benutzende **[!UICONTROL Pause]** auswählen, um ein Video einzufrieren.<br><br>**Hinweis:** Wenn Sie Adobe Analytics Heartbeat-basierte Videoberichte verwenden, müssen Sie diesem Viewer-Ereignis keine Variablen zuordnen, wenn Sie Adobe Analytics in Adobe Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit nativen Adobe Dynamic Media Classic HTML5-Video- und MixedMedia-Viewern. Der Video-Player generiert Tracking-Daten zur Anzeige in Adobe Analytics-Videoberichten. Siehe [Aktivieren von Adobe Analytics-Videoberichten](enabling-analytics-video-reports.md). |
| STOP | **X** (Video) | In Video-Viewern, wenn Benutzende **[!UICONTROL Stopp]** wählen, um die Wiedergabe eines Videos zu beenden.<br><br>**Hinweis:** Wenn Sie Adobe Analytics Heartbeat-basierte Videoberichte verwenden, müssen Sie diesem Viewer-Ereignis keine Variablen zuordnen, wenn Sie Adobe Analytics in Adobe Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit nativen Adobe Dynamic Media Classic HTML5-Video- und MixedMedia-Viewern. Der Video-Player generiert Tracking-Daten zur Anzeige in Adobe Analytics-Videoberichten. Siehe [Aktivieren von Adobe Analytics-Videoberichten](enabling-analytics-video-reports.md). |
| MILESTONE | **X** (Video) | In Video-Viewern werden Meilensteinereignisse generiert, wenn der Benutzer jeweils 0, 25, 50, 75 oder 100 Prozent des Videos gesehen hat.<br><br>**Hinweis:** Wenn Sie Adobe Analytics Heartbeat-basierte Videoberichte verwenden, müssen Sie diesem Viewer-Ereignis keine Variablen zuordnen, wenn Sie Adobe Analytics in Adobe Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit nativen Adobe Dynamic Media Classic HTML5-Video- und MixedMedia-Viewern. Der Video-Player generiert Tracking-Daten zur Anzeige in Adobe Analytics-Videoberichten. Siehe [Aktivieren von Adobe Analytics-Videoberichten](enabling-analytics-video-reports.md). |
| SWATCH | **X** (Flyout, Zoom) | Dieses Viewer-Ereignis wird dem Seiten-Viewer-Ereignis in Adobe Dynamic Media Classic zugeordnet. |
| ZOOM | **X** (E-Katalog, Rotationsset, Zoom) | Wird nicht von Adobe Analytics verfolgt. |
| PAN | **X** (E-Katalog, Rotationsset, Zoom) | Wird nicht von Adobe Analytics verfolgt. |
| SPIN | **X** (Rotationsset) | Wird nicht von Adobe Analytics verfolgt. |

### Adobe Dynamic Media Classic-Variablen {#scene-variables}

Wählen Sie für jedes Viewer-Ereignis auf dem Adobe Analytics-Konfigurationsbildschirm eine Adobe Analytics-Variable und eine *Adobe Dynamic Media Classic-Variable*. Adobe Dynamic Media Classic-Variablen stellen Daten dar, die Sie für einen Bericht erhalten können. Beispielsweise listet die Variable `searchTerm` Schlüsselwörter auf, die in E-Katalog-Suchen verwendet werden.

In der folgenden Tabelle werden Adobe Dynamic Media Classic-Variablen beschrieben:

| Adobe Dynamic Media Classic-Variable | Beschreibung |
| --- | --- |
| asset | Adobe Dynamic Media Classic Asset-ID oder Videopfaddatei. |
| viewerId | Eine beliebige Zahl, die den verschiedenen Viewertypen zugeordnet wird. |
| pageLabel | Die Seite, die von einem Viewer in E-Katalogen angezeigt wird. |
| label | Der Beschriftungswert (eine Zeichenfolge). |
| frame | Die Seite oder Seitenreferenz in einem Bildset. |
| rollover_keyRaw | Der gesamte HREF-Wert, nicht nur ein verarbeiteter Teil davon. |
| rollover_keyProc | Die ID eines Elements, auf das in einer Imagemap verwiesen wird (gültig für Href- und Elementereignisse). |
| searchTerm | Ein Begriff, der bei der Suche in E-Katalogen verwendet wird. |
| timeStamp | Wiedergabe, Beenden und Pause, die in Video-Viewern ausgewählt wurden. |
| progress | Der abgeschlossene Prozentsatz eines Meilensteinereignisses. |
| targetId | Der ID-Wert (eine Zahl). |

## Viewer-Ereignisse aktivieren, bearbeiten und löschen {#activating-editing-and-deleting-viewer-events}

Im Anzeigebereich „Adobe Analytics-Konfiguration“ können Sie Viewer-Ereignisse aktivieren, bearbeiten und löschen:

* **Aktivieren**: Wählen Sie **[!UICONTROL Aktivieren]** aus, um ein ausgewähltes Viewer-Ereignis zu aktivieren oder **[!UICONTROL Deaktivieren]**, um es zu deaktivieren.

* **Bearbeiten**: Wählen Sie ein Viewer-Ereignis aus und klicken Sie auf die graue Schaltfläche **[!UICONTROL Anzeigen/]**). Wählen Sie in den Dropdown-Listen Adobe Dynamic Media Classic-Variable und Adobe Analytics-Variable eine andere Variable aus der jeweiligen Liste aus. Weitere Informationen finden Sie unter [Zuweisen von Adobe Analytics-Variablen zu Adobe Dynamic Media Classic-Viewer-Ereignissen und -Variablen](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables).

* **Löschen**: Wählen Sie ein Viewer-Ereignis aus und klicken Sie auf die graue Schaltfläche **[!UICONTROL Anzeigen/]**). Wählen Sie **[!UICONTROL Löschen]** aus.
