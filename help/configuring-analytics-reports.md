---
title: Konfigurieren von Adobe Analytics-Berichten
description: Erfahren Sie, wie Sie Adobe Analytics-Berichte konfigurieren.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
source-git-commit: 98463dbc24e141547d01bd3f71b1b9fe3a692c14
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 46%

---

# Konfigurieren von Adobe Analytics-Berichten{#configuring-adobe-analytics-reports}

Um in Adobe Analytics festzulegen, welche Informationen in Adobe Analytics-Berichten enthalten sein sollen, rufen Sie den Anzeigebereich „Adobe Analytics-Konfiguration“ auf. Nachdem Sie Berichte konfiguriert haben, werden in diesem Bildschirm für jedes Viewer-Ereignis, über das Informationen gewünscht werden, eine entsprechende Adobe Analytics-Variable und Dynamic Media Classic-Variable aufgelistet. Diese Viewer-Ereignisse - Variablenkombinationen Adobe Analytics und Dynamic Media Classic bestimmen, welche Informationen gemeldet werden.

Neben der Zuordnung von Viewer-Ereignissen zu Variablen bietet der Bildschirm &quot;Adobe Analytics-Konfiguration&quot;Tools zum Aktivieren, Bearbeiten und Löschen von Viewer-Ereignissen.

>[!NOTE]
>
>Wenn Sie die Adobe Analytics-Berichtseinstellungen in Adobe Analytics ändern, müssen Sie sich von Adobe Dynamic Media Classic aus wieder bei Adobe Analytics anmelden, die Adobe Analytics-Konfigurationseinstellungen erneut speichern und dann erneut veröffentlichen.

Siehe [Anmelden bei Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Siehe [Veröffentlichen von Konfigurationsinformationen](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Zuweisen von Adobe Analytics-Variablen zu Dynamic Media Classic-Viewer-Ereignissen und -Variablen {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Verknüpfen Sie im Bildschirm &quot;Adobe Analytics-Konfiguration&quot;Viewer-Ereignisse mit Adobe Analytics-Variablen und Dynamic Media Classic-Variablen. Wählen Sie für jedes Viewer-Ereignis eine Adobe Analytics-Variable und eine Dynamic Media Classic-Variable aus. Anweisungen zum Öffnen des Anzeigebereichs „Adobe Analytics-Konfiguration“ finden Sie unter [Anmelden bei Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**So weisen Sie Adobe Analytics-Variablen zu Dynamic Media Classic-Viewer-Ereignissen und -Variablen zu**

1. Nachdem Sie sich von Dynamic Media Classic aus bei Adobe Analytics angemeldet und eine Report Suite ausgewählt haben, aktivieren Sie auf der Seite &quot;Adobe Analytics-Konfiguration&quot;in der rechten Tabellenspalte ein Viewer-Ereignis, indem Sie auf **[!UICONTROL Aktivieren]** klicken.
1. Zeigen Sie in der Spalte „Variablen“ die Variablenpaarauswahl an, indem Sie für das gewünschte Viewer-Ereignis auf die Pfeilschaltfläche klicken.

   Siehe [Viewer-Ereignisse](configuring-analytics-reports.md#viewer_events).

1. Fügen Sie eine Dynamic Media Classic-Variable hinzu.

   Siehe [Dynamic Media Classic-Variablen](configuring-analytics-reports.md#scene7_variables).

1. Fügen Sie eine Adobe Analytics-Variable hinzu.
1. (Optional) Klicken Sie auf **Hinzufügen**, um ein weiteres Variablenpaar hinzuzufügen.
1. Klicken Sie auf **Speichern**.

   Nachdem Sie auf &quot;Speichern&quot;geklickt haben, werden das Viewer-Ereignis, die zugehörige Adobe Analytics-Variable und die Dynamic Media Classic-Variable im Bildschirm &quot;Adobe Analytics-Konfiguration&quot;aufgelistet.

1. Klicken Sie in der rechten unteren Ecke auf **Schließen**.
1. Klicken Sie auf **Veröffentlichen** > **Veröffentlichung starten**, um eine Image-Serving-Veröffentlichung durchzuführen.

   Die Veröffentlichung ist erforderlich, damit die in den Viewern enthaltenen Informationen auf den Dynamic Media Classic-Servern verfügbar sind.

### Viewer-Ereignisse {#viewer-events}

Viewer-Ereignisse beschreiben Aktionen, die Benutzer mit Dynamic Media Classic-Viewern ausführen. Wenn ein Benutzer eine bestimmte Aktion auslöst, z. B. durch Klicken auf eine Miniaturansicht oder Starten oder Anhalten eines Videos, &quot;sendet&quot;der Viewer ein Ereignis zusammen mit den mit diesem Ereignis verknüpften Daten an die Webseite.

In der folgenden Tabelle werden Viewer-Ereignisse beschrieben, die Sie dem Anzeigebereich „Adobe Analytics-Konfiguration“ hinzufügen können.

| Viewer-Ereignis | Unterstützung und Viewer für die HTML5 Viewer-Plattform | Beschreibung |
|--- |--- |--- |
| LOAD | **X** (E-Katalog, Flyout, Rotationsset, Video, Zoom) | Wenn ein Benutzer den Viewer startet |
| PAGE | **X** (E-Katalog) | Wenn ein Benutzer in E-Katalogen eine Seite umblättert oder in zielgerichteten Zoom-Viewern auf ein anderes Ziel oder Farbfeld klickt. |
| SWAP | **X** (E-Katalog, Flyout, Rotationsset, Video, Zoom) | Wenn ein Benutzer auf eine andere Miniatur klickt, um ein anderes Bild anzuzeigen |
| ITEM | **X** (E-Katalog) | Wenn ein Benutzer in Viewern, die Imagemaps unterstützen, in denen Rollover definiert sind, mit der Maus auf eine Imagemap zeigt, um den Rollover-Text zu lesen |
| HREF | **X** (E-Katalog) | Wenn ein Benutzer in Viewern, die Imagemaps unterstützen, auf eine URL in einer Imagemap klickt |
| TARGET |  | Wenn ein Benutzer in zielgerichteten Zoom-Viewern auf ein Zoomziel klickt, um einen Teil eines Bilds zu vergrößern |
| SEARCH |  | Wenn ein Benutzer in E-Katalogen eine Wortsuche durchführt |
| PLAY | **X** (Video) | Wenn ein Benutzer in Video-Viewern auf „Wiedergabe“ klickt, um ein Video wiederzugeben <br><br>**Hinweis:** Wenn Sie Heartbeat-basierte Videoberichte von Adobe Analytics verwenden, müssen Sie bei der Konfiguration von Adobe Analytics in Dynamic Media Classic diesem Viewer-Ereignis keine Variablen zuordnen. Video Heartbeat funktioniert mit nativen Dynamic Media Classic HTML5-Video- und MixedMedia-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten. Siehe [Aktivieren von Adobe Analytics-Videoberichten](enabling-analytics-video-reports.md). |
| PAUSE | **X** (Video) | Wenn ein Benutzer in Video-Viewern auf „Pause“ klickt, um ein Video anzuhalten <br><br>**Hinweis:** Wenn Sie Heartbeat-basierte Videoberichte von Adobe Analytics verwenden, müssen Sie bei der Konfiguration von Adobe Analytics in Dynamic Media Classic diesem Viewer-Ereignis keine Variablen zuordnen. Video Heartbeat funktioniert mit nativen Dynamic Media Classic HTML5-Video- und MixedMedia-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten. Siehe [Aktivieren von Adobe Analytics-Videoberichten](enabling-analytics-video-reports.md). |
| STOP | **X** (Video) | Wenn ein Benutzer in Video-Viewern auf „Stopp“ klickt, um ein Video abzubrechen.<br><br>**Hinweis:** Wenn Sie Heartbeat-basierte Videoberichte von Adobe Analytics verwenden, müssen Sie bei der Konfiguration von Adobe Analytics in Dynamic Media Classic diesem Viewer-Ereignis keine Variablen zuordnen. Video Heartbeat funktioniert mit nativen Dynamic Media Classic HTML5-Video- und MixedMedia-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten. Siehe [Aktivieren von Adobe Analytics-Videoberichten](enabling-analytics-video-reports.md). |
| MILESTONE | **X**  (Video) | In Video-Viewern werden Meilensteinereignisse generiert, wenn der Benutzer jeweils 0, 25, 50, 75 oder 100 Prozent des Videos gesehen hat.<br><br>**Hinweis:** Wenn Sie Heartbeat-basierte Videoberichte von Adobe Analytics verwenden, müssen Sie bei der Konfiguration von Adobe Analytics in Dynamic Media Classic diesem Viewer-Ereignis keine Variablen zuordnen. Video Heartbeat funktioniert mit nativen Dynamic Media Classic HTML5-Video- und MixedMedia-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten. Siehe [Aktivieren von Adobe Analytics-Videoberichten](enabling-analytics-video-reports.md). |
| SWATCH | X (Flyout, Zoom) | Dieses Viewer-Ereignis wird dem SEITEN-Viewer-Ereignis in Dynamic Media Classic zugeordnet. |
| ZOOM | **X** (E-Katalog, Rotationsset, Zoom) | Wird nicht von Adobe Analytics verfolgt.<br> |
| PAN | **X** (E-Katalog, Rotationsset, Zoom) | Wird nicht von Adobe Analytics verfolgt.<br> |
| SPIN | **X** (Rotationsset) | Wird nicht von Adobe Analytics verfolgt.<br> |


### Dynamic Media Classic-Variablen {#scene-variables}

Wählen Sie für jedes Viewer-Ereignis auf dem Bildschirm &quot;Adobe Analytics-Konfiguration&quot;eine Adobe Analytics-Variable und eine *Dynamic Media Classic-Variable*. Dynamic Media Classic-Variablen stellen Daten dar, die Sie für einen Bericht abrufen können. Zum Beispiel listet die Variable `searchTerm` Schlüsselwörter auf, die in E-Katalog-Suchvorgängen verwendet wurden.

In der folgenden Tabelle werden Dynamic Media Classic-Variablen beschrieben.

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
AktivierenKlicken Sie auf  **** Aktivieren , um ein ausgewähltes Viewer-Ereignis zu aktivieren oder zu  **** deaktivieren.

* ****
BearbeitenWählen Sie ein Viewer-Ereignis aus und klicken Sie auf die grau  **[!UICONTROL Schaltfläche Variablen anzeigen/]** bearbeiten . Wählen Sie in den Dropdownlisten Dynamic Media Classic-Variable und Adobe Analytics-Variable eine andere Variable aus den jeweiligen Listen aus. Weitere Informationen finden Sie unter Zuweisen von Adobe Analytics-Variablen zu Dynamic Media Classic-Viewer-Ereignissen und -Variablen.

* ****
LöschenWählen Sie ein Viewer-Ereignis aus und klicken Sie auf die graue Schaltfläche  **[!UICONTROL Variablen anzeigen/]** bearbeiten . Klicken Sie auf „**[!UICONTROL Löschen]**“.
