---
title: Konfigurieren von Adobe Analytics-Berichten
description: Erfahren Sie, wie Sie Adobe Analytics-Berichte in Dynamic Media Classic konfigurieren.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
source-git-commit: 1d30c98b76ebe78ff60bae87bd112de7a577182d
workflow-type: tm+mt
source-wordcount: '1202'
ht-degree: 29%

---

# Konfigurieren von Adobe Analytics-Berichten{#configuring-adobe-analytics-reports}

Um in Adobe Analytics festzulegen, welche Informationen in Adobe Analytics-Berichten enthalten sein sollen, rufen Sie den Anzeigebereich „Adobe Analytics-Konfiguration“ auf. Nachdem Sie Berichte konfiguriert haben, werden in diesem Bildschirm für jedes Viewer-Ereignis, über das Informationen gewünscht werden, eine entsprechende Adobe Analytics-Variable und Dynamic Media Classic-Variable aufgelistet. Diese Viewer-Ereignisse - Variablenkombinationen Adobe Analytics und Dynamic Media Classic bestimmen, welche Informationen gemeldet werden.

Neben der Zuordnung von Viewer-Ereignissen zu Variablen bietet der Bildschirm &quot;Adobe Analytics-Konfiguration&quot;Tools zum Aktivieren, Bearbeiten und Löschen von Viewer-Ereignissen.

>[!NOTE]
>
>Wenn Sie die Adobe Analytics-Berichtseinstellungen in Adobe Analytics ändern, müssen Sie sich von Adobe Dynamic Media Classic aus wieder bei Adobe Analytics anmelden, die Adobe Analytics-Konfigurationseinstellungen erneut speichern und dann erneut veröffentlichen.

Siehe [Anmelden bei Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Siehe [Veröffentlichungskonfigurationsinformationen](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Zuweisen von Adobe Analytics-Variablen zu Dynamic Media Classic-Viewer-Ereignissen und -Variablen {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Verknüpfen Sie im Bildschirm &quot;Adobe Analytics-Konfiguration&quot;Viewer-Ereignisse mit Adobe Analytics-Variablen und Dynamic Media Classic-Variablen. Wählen Sie für jedes Viewer-Ereignis eine Adobe Analytics-Variable und eine Dynamic Media Classic-Variable aus. Anweisungen zum Öffnen des Anzeigebereichs „Adobe Analytics-Konfiguration“ finden Sie unter [Anmelden bei Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**So weisen Sie Adobe Analytics-Variablen zu Dynamic Media Classic-Viewer-Ereignissen und -Variablen zu**

1. Nachdem Sie sich von Dynamic Media Classic aus bei Adobe Analytics angemeldet und eine Report Suite ausgewählt haben, aktivieren Sie auf der Seite &quot;Adobe Analytics-Konfiguration&quot;in der rechten Tabellenspalte ein Viewer-Ereignis, indem Sie **[!UICONTROL Aktivieren]** auswählen.
1. Zeigen Sie unter der Spalte Variablen die Variablenpaarauswahl an, indem Sie die Pfeilschaltfläche für das gewünschte Viewer-Ereignis auswählen.

   Siehe [Viewer-Ereignisse](configuring-analytics-reports.md#viewer_events).

1. Fügen Sie eine Dynamic Media Classic-Variable hinzu.

   Siehe [Dynamic Media Classic-Variablen](configuring-analytics-reports.md#scene7_variables).

1. Fügen Sie eine Adobe Analytics-Variable hinzu.
1. (Optional) Um ein weiteres Variablenpaar hinzuzufügen, wählen Sie **[!UICONTROL Hinzufügen]** aus.
1. Wählen Sie **[!UICONTROL Save]** aus.

   Nachdem Sie **[!UICONTROL Save]** ausgewählt haben, werden das Viewer-Ereignis, die zugehörige Adobe Analytics-Variable und die Dynamic Media Classic-Variable im Bildschirm &quot;Adobe Analytics-Konfiguration&quot;aufgelistet.

1. Wählen Sie in der rechten unteren Ecke **[!UICONTROL Close]** aus.
1. Wählen Sie **[!UICONTROL Publish]** > **[!UICONTROL Submit Publish]** aus, um eine Image Serving-Veröffentlichung auszuführen.

   Die Veröffentlichung ist erforderlich, damit die in den Viewern enthaltenen Informationen auf den Dynamic Media Classic-Servern verfügbar sind.

### Viewer-Ereignisse {#viewer-events}

Viewer-Ereignisse beschreiben Aktionen, die Benutzer mit Dynamic Media Classic-Viewern ausführen. Wenn ein Benutzer eine bestimmte Aktion auslöst, z. B. eine Miniaturansicht auszuwählen oder ein Video zu starten oder zu stoppen, &quot;sendet&quot;der Viewer ein Ereignis zusammen mit den mit diesem Ereignis verknüpften Daten an die Webseite.

In der folgenden Tabelle werden Viewer-Ereignisse beschrieben, die Sie dem Anzeigebereich „Adobe Analytics-Konfiguration“ hinzufügen können.

| Viewer-Ereignis | Unterstützung und Viewer für die HTML5 Viewer-Plattform | Beschreibung |
|--- |--- |--- |
| LOAD | **X** (E-Katalog, Flyout, Rotationsset, Video, Zoom) | Wenn ein Benutzer einen Viewer startet |
| PAGE | **X** (E-Katalog) | Wenn ein Benutzer in E-Katalogen eine Seite umblättert; in zielgerichteten Zoom-Viewern, wenn ein Benutzer ein anderes Ziel oder ein Farbmuster auswählt |
| SWAP | **X** (E-Katalog, Flyout, Rotationsset, Video, Zoom) | Wenn ein Benutzer eine andere Miniaturansicht auswählt, um ein anderes Bild anzuzeigen |
| ITEM | **X** (E-Katalog) | In Viewern, die Imagemaps unterstützen, in denen Rollover definiert sind, wenn ein Benutzer den Mauszeiger über eine Imagemap bewegt, um den Rollover-Text zu lesen |
| HREF | **X** (E-Katalog) | In Viewern, die Imagemaps unterstützen, wenn ein Benutzer eine URL in einer Imagemap auswählt |
| TARGET |  | Wenn ein Benutzer in zielgerichteten Zoom-Viewern ein Zoomziel auswählt, um einen Teil eines Bildes zu vergrößern. |
| SEARCH |  | Wenn ein Benutzer in E-Katalogen eine Wortsuche durchführt |
| PLAY | **X** (Video) | Wenn ein Benutzer in Video-Viewern Play auswählt, um mit der Wiedergabe eines Videos zu beginnen.<br><br>**Hinweis:** Wenn Sie Heartbeat-basierte Videoberichte von Adobe Analytics verwenden, müssen Sie bei der Konfiguration von Adobe Analytics in Dynamic Media Classic diesem Viewer-Ereignis keine Variablen zuordnen. Video Heartbeat funktioniert mit nativen Dynamic Media Classic HTML5-Video- und MixedMedia-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten. Siehe [Adobe Analytics-Videoberichte aktivieren](enabling-analytics-video-reports.md). |
| PAUSE | **X** (Video) | Wenn ein Benutzer in Video-Viewern **[!UICONTROL Pause]** auswählt, um ein Video einzufrieren.<br><br>**Hinweis:** Wenn Sie Heartbeat-basierte Videoberichte von Adobe Analytics verwenden, müssen Sie bei der Konfiguration von Adobe Analytics in Dynamic Media Classic diesem Viewer-Ereignis keine Variablen zuordnen. Video Heartbeat funktioniert mit nativen Dynamic Media Classic HTML5-Video- und MixedMedia-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten. Siehe [Adobe Analytics-Videoberichte aktivieren](enabling-analytics-video-reports.md). |
| STOP | **X** (Video) | Wenn ein Benutzer in Video-Viewern **[!UICONTROL Stopp]** auswählt, um die Wiedergabe eines Videos zu beenden.<br><br>**Hinweis:** Wenn Sie Heartbeat-basierte Videoberichte von Adobe Analytics verwenden, müssen Sie bei der Konfiguration von Adobe Analytics in Dynamic Media Classic diesem Viewer-Ereignis keine Variablen zuordnen. Video Heartbeat funktioniert mit nativen Dynamic Media Classic HTML5-Video- und MixedMedia-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten. Siehe [Adobe Analytics-Videoberichte aktivieren](enabling-analytics-video-reports.md). |
| MILESTONE | **X**  (Video) | In Video-Viewern werden Meilensteinereignisse generiert, wenn der Benutzer jeweils 0, 25, 50, 75 oder 100 Prozent des Videos gesehen hat.<br><br>**Hinweis:** Wenn Sie Heartbeat-basierte Videoberichte von Adobe Analytics verwenden, müssen Sie bei der Konfiguration von Adobe Analytics in Dynamic Media Classic diesem Viewer-Ereignis keine Variablen zuordnen. Video Heartbeat funktioniert mit nativen Dynamic Media Classic HTML5-Video- und MixedMedia-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten. Siehe [Adobe Analytics-Videoberichte aktivieren](enabling-analytics-video-reports.md). |
| SWATCH | X (Flyout, Zoom) | Dieses Viewer-Ereignis wird dem SEITEN-Viewer-Ereignis in Dynamic Media Classic zugeordnet. |
| ZOOM | **X** (E-Katalog, Rotationsset, Zoom) | Wird nicht von Adobe Analytics verfolgt.<br> |
| PAN | **X** (E-Katalog, Rotationsset, Zoom) | Wird nicht von Adobe Analytics verfolgt.<br> |
| SPIN | **X** (Rotationsset) | Wird nicht von Adobe Analytics verfolgt.<br> |


### Dynamic Media Classic-Variablen {#scene-variables}

Wählen Sie für jedes Viewer-Ereignis auf dem Bildschirm &quot;Adobe Analytics-Konfiguration&quot;eine Adobe Analytics-Variable und eine *Dynamic Media Classic-Variable*. Dynamic Media Classic-Variablen stellen Daten dar, die Sie für einen Bericht abrufen können. Zum Beispiel listet die Variable `searchTerm` Schlüsselwörter auf, die in E-Katalog-Suchvorgängen verwendet wurden.

In der folgenden Tabelle werden Dynamic Media Classic-Variablen beschrieben:

| Dynamic Media Classic-Variable | Beschreibung |
|--- |:--- |
| asset | Dynamic Media Classic Asset-ID oder Videopfaddatei. |
| viewerId | Eine beliebige Zahl, die den verschiedenen Viewertypen zugeordnet wird. |
| pageLabel | Die Seite, die von einem Viewer in E-Katalogen angezeigt wird. |
| label | Der Beschriftungswert (eine Zeichenfolge). |
| frame | Die Seite oder Seitenreferenz in einem Bildsatz. |
| rollover_keyRaw | Der gesamte HREF-Wert, nicht nur ein verarbeiteter Teil. |
| rollover_keyProc | Die ID eines Elements, auf das in einer Imagemap verwiesen wird (gültig für Href- und Elementereignisse). |
| searchTerm | Ein Begriff, der bei der Suche in E-Katalogen verwendet wird. |
| timeStamp | In Video-Viewern ausgewählte Befehle zum Abspielen, Abbrechen und Anhalten. |
| progress | Der abgeschlossene Prozentsatz eines Meilensteinereignisses. |
| targetId | Der ID-Wert (eine Zahl). |

## Aktivieren, Bearbeiten und Löschen von Viewer-Ereignissen {#activating-editing-and-deleting-viewer-events}

Im Anzeigebereich „Adobe Analytics-Konfiguration“ können Sie Viewer-Ereignisse aktivieren, bearbeiten und löschen:

* ****
AktivierenWählen Sie  **** Aktivieren oder  **** Deaktivieren aus, um ein ausgewähltes Viewer-Ereignis zu deaktivieren.

* ****
BearbeitenWählen Sie ein Viewer-Ereignis aus und wählen Sie die graue Schaltfläche  **[!UICONTROL Anzeigen/]** Bearbeiten von Variablen . Wählen Sie in den Dropdownlisten Dynamic Media Classic-Variable und Adobe Analytics-Variable eine andere Variable aus den jeweiligen Listen aus. Weitere Informationen finden Sie unter Zuweisen von Adobe Analytics-Variablen zu Dynamic Media Classic-Viewer-Ereignissen und -Variablen.

* ****
LöschenWählen Sie ein Viewer-Ereignis aus und klicken Sie auf die grau  **[!UICONTROL Ansicht/]** Bearbeiten-Variablen-Schaltfläche. Wählen Sie **[!UICONTROL Löschen]** aus.
