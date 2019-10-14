---
title: Konfigurieren von Adobe Analytics-Berichten
seo-title: Konfigurieren von Adobe Analytics-Berichten
description: 'null'
seo-description: Erfahren Sie, wie Sie Adobe Analytics-Berichte konfigurieren.
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: Verweis
products: SG_EXPERIENCEMANAGER/Dynamic Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Konfigurieren von Adobe Analytics-Berichten{#configuring-adobe-analytics-reports}

Um in Adobe Analytics festzulegen, welche Informationen in Adobe Analytics-Berichten enthalten sein sollen, rufen Sie den Anzeigebereich „Adobe Analytics-Konfiguration“ auf. Nach der Konfiguration von Berichten werden in diesem Anzeigebereich für jedes Viewer-Ereignis, über das Sie Informationen erhalten möchten, eine entsprechende Adobe Analytics-Variable und eine dynamische Media Classic-Variable aufgelistet. Diese Kombinationen aus Viewer-Ereignissen und Adobe Analytics-Variablen und dynamischen Media Classic-Variablen bestimmen, welche Informationen gemeldet werden.

Neben der Möglichkeit, Viewer-Ereignisse mit Variablen zu verknüpfen, umfasst der Anzeigebereich „Adobe Analytics-Konfiguration“ auch Funktionen zum Aktivieren, Bearbeiten und Löschen von Viewer-Ereignissen.

>[!NOTE]
>
>Wenn Sie Adobe Analytics-Berichtseinstellungen in Adobe Analytics ändern, müssen Sie sich unbedingt wieder vom Adobe Scene7 Publishing System aus bei Adobe Analytics anmelden, Ihre Adobe Analytics-Konfigurationseinstellungen erneut speichern und dann die Veröffentlichung erneut durchführen.

Siehe [Anmelden bei Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Siehe [Veröffentlichen von Konfigurationsinformationen](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Zuweisen von Adobe Analytics-Variablen zu Dynamischen Media Classic-Viewer-Ereignissen und -Variablen {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Verwenden Sie den Anzeigebereich "Adobe Analytics-Konfiguration", um Viewer-Ereignisse mit Adobe Analytics-Variablen und dynamischen Media Classic-Variablen zu verknüpfen. Wählen Sie für jedes Viewer-Ereignis eine Adobe Analytics-Variable und eine Dynamic Media Classic-Variable aus. Anweisungen zum Öffnen des Anzeigebereichs „Adobe Analytics-Konfiguration“ finden Sie unter [Anmelden bei Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**So weisen Sie Dynamischen Media Classic-Viewer-Ereignissen und -Variablen Adobe Analytics-Variablen zu**

1. After you log in to Adobe Analytics from within Dynamic Media Classic and select a report suite, on the Adobe Analytics Configuration page, in the far right column of the table, activate a viewer event by clicking **Enable**.
1. Zeigen Sie in der Spalte „Variablen“ die Variablenpaarauswahl an, indem Sie für das gewünschte Viewer-Ereignis auf die Pfeilschaltfläche klicken.

   Siehe [Viewer-Ereignisse](configuring-analytics-reports.md#viewer_events).

1. Fügen Sie eine Variable für Dynamic Media Classic hinzu.

   Siehe [Dynamic Media Classic-Variablen](configuring-analytics-reports.md#scene7_variables).

1. Fügen Sie eine Adobe Analytics-Variable hinzu.
1. (Optional) Klicken Sie auf **Hinzufügen**, um ein weiteres Variablenpaar hinzuzufügen.
1. Klicken Sie auf **Speichern**.

   Nachdem Sie auf "Speichern"geklickt haben, werden das Viewer-Ereignis, seine Adobe Analytics-Variable und seine Variable "Dynamic Media Classic"im Anzeigebereich "Adobe Analytics-Konfiguration"aufgelistet.

1. Klicken Sie in der rechten unteren Ecke auf **Schließen**.
1. Klicken Sie auf **Veröffentlichen** &gt; **Veröffentlichung starten**, um eine Image-Serving-Veröffentlichung durchzuführen.

   Die Veröffentlichung ist erforderlich, damit die in den Viewern enthaltenen Informationen auf den Servern von Dynamic Media Classic verfügbar sind.

### Viewer-Ereignisse {#viewer-events}

Viewer-Ereignisse beschreiben Aktionen, die Benutzer mit Dynamischen Media Classic-Viewern ausführen. Wenn ein Benutzer eine bestimmte Aktion startet, z. B. wenn er auf eine Miniatur klickt oder ein Video startet oder anhält, „überträgt“ der Viewer ein Ereignis sowie die mit diesem Ereignis zusammenhängenden Daten an die Webseite.

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
| PLAY | **X** (Video) | Wenn ein Benutzer in Video-Viewern auf „Wiedergabe“ klickt, um ein Video wiederzugeben<br><br>**** Hinweis: Wenn Sie Adobe Analytics Heartbeat-basierte Videoberichte verwenden, müssen Sie diesem Viewer-Ereignis keine Variablen zuordnen, wenn Sie Adobe Analytics in Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit vordefinierten HTML5-Video- und MixedMedia-Viewern für dynamische Medien und Classic. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten. See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| PAUSE | **X** (Video) | Wenn ein Benutzer in Video-Viewern auf „Pause“ klickt, um ein Video anzuhalten<br><br>**** Hinweis: Wenn Sie Adobe Analytics Heartbeat-basierte Videoberichte verwenden, müssen Sie diesem Viewer-Ereignis keine Variablen zuordnen, wenn Sie Adobe Analytics in Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit vordefinierten HTML5-Video- und MixedMedia-Viewern für dynamische Medien und Classic. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten. See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| STOP | **X** (Video) | Wenn ein Benutzer in Video-Viewern auf „Stopp“ klickt, um ein Video abzubrechen.<br><br>**** Hinweis: Wenn Sie Adobe Analytics Heartbeat-basierte Videoberichte verwenden, müssen Sie diesem Viewer-Ereignis keine Variablen zuordnen, wenn Sie Adobe Analytics in Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit vordefinierten HTML5-Video- und MixedMedia-Viewern für dynamische Medien und Classic. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten. See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| MILESTONE | **X**  (Video) | In Video-Viewern werden Meilensteinereignisse generiert, wenn der Benutzer jeweils 0, 25, 50, 75 oder 100 Prozent des Videos gesehen hat.<br><br>**** Hinweis: Wenn Sie Adobe Analytics Heartbeat-basierte Videoberichte verwenden, müssen Sie diesem Viewer-Ereignis keine Variablen zuordnen, wenn Sie Adobe Analytics in Dynamic Media Classic konfigurieren. Video Heartbeat funktioniert mit vordefinierten HTML5-Video- und MixedMedia-Viewern für dynamische Medien und Classic. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten. See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| SWATCH | X (Flyout, Zoom) | Dieses Viewer-Ereignis wird mit dem PAGE-Viewer-Ereignis im Scene7 Publishing System verknüpft. |
| ZOOM | **X** (E-Katalog, Rotationsset, Zoom) | Wird nicht von Adobe Analytics verfolgt.<br> |
| PAN | **X** (E-Katalog, Rotationsset, Zoom) | Wird nicht von Adobe Analytics verfolgt.<br> |
| SPIN | **X** (Rotationsset) | Wird nicht von Adobe Analytics verfolgt.<br> |


### Dynamische Medien - Classic-Variablen {#scene-variables}

For each viewer event on Adobe Analytics Configuration screen, choose a Adobe Analytics variable and a *Dynamic Media Classic variable*. Dynamische Medienklassische Variablen stellen Daten dar, die Sie für einen Bericht abrufen können. Zum Beispiel listet die Variable `searchTerm` Schlüsselwörter auf, die in E-Katalog-Suchvorgängen verwendet wurden.

In der folgenden Tabelle werden die Variablen "Dynamic Media Classic"beschrieben.

| Variable "Dynamic Media Classic" | Beschreibung |
|--- |:--- |
| asset | Asset-ID oder Videopfaddatei im Scene7 Publishing System. |
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

* **Aktivieren** Klicken Sie auf **[!UICONTROL Aktivieren]** , um ein ausgewähltes Viewer-Ereignis zu aktivieren oder zu **[!UICONTROL deaktivieren]** .

* **Bearbeiten** Wählen Sie ein Viewer-Ereignis aus und klicken Sie auf die graue Schaltfläche "Variablen **[!UICONTROL anzeigen/bearbeiten]** ". Wählen Sie in den Dropdownlisten "Dynamische Medienklassische Variable"und "Adobe Analytics-Variable"aus den jeweiligen Listen eine andere Variable aus. Weitere Informationen finden Sie unter Zuweisen von Adobe Analytics-Variablen zu Dynamischen Media Classic-Viewer-Ereignissen und -Variablen.

* **Löschen** eines Viewer-Ereignisses und Klicken Sie auf die graue Schaltfläche "Variablen **[!UICONTROL anzeigen/bearbeiten]** ". Klicken Sie auf **[!UICONTROL Löschen]**.
