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
role: Data Engineer, Administrator, Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 50%

---


# Konfigurieren von Adobe Analytics-Berichten{#configuring-adobe-analytics-reports}

Um in Adobe Analytics festzulegen, welche Informationen in Adobe Analytics-Berichten enthalten sein sollen, rufen Sie den Anzeigebereich „Adobe Analytics-Konfiguration“ auf. Nach dem Konfigurieren von Berichten wird in diesem Anzeigebereich für jedes Viewer-Ereignis, für das Informationen benötigt werden, eine entsprechende Adobe Analytics-Variable und eine Dynamic Media Classic-Variable Liste. Diese Viewer-Ereignis-Adobe Analytics-Variablenkombinationen Dynamic Media Classic bestimmen, welche Informationen gemeldet werden.

Neben der Möglichkeit, Viewer-Ereignisse mit Variablen zu verknüpfen, umfasst der Anzeigebereich „Adobe Analytics-Konfiguration“ auch Funktionen zum Aktivieren, Bearbeiten und Löschen von Viewer-Ereignissen.

>[!NOTE]
>
>Wenn Sie die Adobe Analytics-Berichtseinstellungen in Adobe Analytics ändern, stellen Sie sicher, dass Sie sich von Adobe Dynamic Media Classic aus wieder bei Adobe Analytics anmelden, Ihre Adobe Analytics-Konfigurationseinstellungen erneut speichern und dann erneut veröffentlichen.

Siehe [Anmelden bei Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

Siehe [Veröffentlichen von Konfigurationsinformationen](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Zuweisen von Adobe Analytics-Variablen zu Dynamic Media Classic Viewer-Ereignissen und -Variablen {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Verwenden Sie den Anzeigebereich &quot;Adobe Analytics-Konfiguration&quot;, um Viewer-Ereignis mit Adobe Analytics-Variablen und Dynamic Media Classic-Variablen zu verknüpfen. Wählen Sie für jedes Viewer-Ereignis eine Adobe Analytics-Variable und eine Dynamic Media Classic-Variable aus. Anweisungen zum Öffnen des Anzeigebereichs „Adobe Analytics-Konfiguration“ finden Sie unter [Anmelden bei Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics).

**So weisen Sie Dynamic Media Classic-Viewer-Ereignissen und -Variablen Adobe Analytics-Variablen zu**

1. Nachdem Sie sich von Dynamic Media Classic aus bei Adobe Analytics angemeldet und eine Report Suite ausgewählt haben, aktivieren Sie auf der Seite &quot;Adobe Analytics-Konfiguration&quot;in der Tabellenspalte ganz rechts ein Viewer-Ereignis, indem Sie auf **Aktivieren** klicken.
1. Zeigen Sie in der Spalte „Variablen“ die Variablenpaarauswahl an, indem Sie für das gewünschte Viewer-Ereignis auf die Pfeilschaltfläche klicken.

   Siehe [Viewer-Ereignisse](configuring-analytics-reports.md#viewer_events).

1. hinzufügen einer Dynamic Media Classic-Variablen.

   Siehe [Dynamic Media Classic-Variablen](configuring-analytics-reports.md#scene7_variables).

1. Fügen Sie eine Adobe Analytics-Variable hinzu.
1. (Optional) Klicken Sie auf **Hinzufügen**, um ein weiteres Variablenpaar hinzuzufügen.
1. Klicken Sie auf **Speichern**.

   Nachdem Sie auf &quot;Speichern&quot;geklickt haben, werden das Viewer-Ereignis, seine Adobe Analytics-Variable und seine Dynamic Media Classic-Variable im Anzeigebereich &quot;Adobe Analytics-Konfiguration&quot;aufgelistet.

1. Klicken Sie in der rechten unteren Ecke auf **Schließen**.
1. Klicken Sie auf **Veröffentlichen** > **Veröffentlichung starten**, um eine Image-Serving-Veröffentlichung durchzuführen.

   Die Veröffentlichung ist erforderlich, damit die in den Viewern enthaltenen Informationen auf den Dynamic Media Classic-Servern verfügbar sind.

### Viewer-Ereignisse {#viewer-events}

Viewer-Ereignis beschreiben Aktionen, die Benutzer mit Dynamic Media Classic-Viewern ausführen. Wenn ein Benutzer eine bestimmte Aktion startet, z. B. wenn er auf eine Miniatur klickt oder ein Video startet oder anhält, „überträgt“ der Viewer ein Ereignis sowie die mit diesem Ereignis zusammenhängenden Daten an die Webseite.

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
| PLAY | **X** (Video) | Wenn ein Benutzer in Video-Viewern auf „Wiedergabe“ klickt, um ein Video wiederzugeben <br><br>**Hinweis:** Wenn Sie Adobe Analytics Heartbeat-basierten Video-Berichte verwenden, müssen Sie bei der Konfiguration von Adobe Analytics in Dynamic Media Classic diesem Viewer-Ereignis keine Variablen zuordnen. Video Heartbeat funktioniert mit vordefinierten Dynamic Media Classic HTML5 Video- und MixedMedia-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten. Siehe [Aktivieren von Adobe Analytics-Videoberichten](enabling-analytics-video-reports.md). |
| PAUSE | **X** (Video) | Wenn ein Benutzer in Video-Viewern auf „Pause“ klickt, um ein Video anzuhalten <br><br>**Hinweis:** Wenn Sie Adobe Analytics Heartbeat-basierten Video-Berichte verwenden, müssen Sie bei der Konfiguration von Adobe Analytics in Dynamic Media Classic diesem Viewer-Ereignis keine Variablen zuordnen. Video Heartbeat funktioniert mit vordefinierten Dynamic Media Classic HTML5 Video- und MixedMedia-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten. Siehe [Aktivieren von Adobe Analytics-Videoberichten](enabling-analytics-video-reports.md). |
| STOP | **X** (Video) | Wenn ein Benutzer in Video-Viewern auf „Stopp“ klickt, um ein Video abzubrechen.<br><br>**Hinweis:** Wenn Sie Adobe Analytics Heartbeat-basierten Video-Berichte verwenden, müssen Sie bei der Konfiguration von Adobe Analytics in Dynamic Media Classic diesem Viewer-Ereignis keine Variablen zuordnen. Video Heartbeat funktioniert mit vordefinierten Dynamic Media Classic HTML5 Video- und MixedMedia-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten. Siehe [Aktivieren von Adobe Analytics-Videoberichten](enabling-analytics-video-reports.md). |
| MILESTONE | **X**  (Video) | In Video-Viewern werden Meilensteinereignisse generiert, wenn der Benutzer jeweils 0, 25, 50, 75 oder 100 Prozent des Videos gesehen hat.<br><br>**Hinweis:** Wenn Sie Adobe Analytics Heartbeat-basierten Video-Berichte verwenden, müssen Sie bei der Konfiguration von Adobe Analytics in Dynamic Media Classic diesem Viewer-Ereignis keine Variablen zuordnen. Video Heartbeat funktioniert mit vordefinierten Dynamic Media Classic HTML5 Video- und MixedMedia-Viewern. Der Video-Player erzeugt Verfolgungsdaten für die Anzeige in Adobe Analytics-Berichten. Siehe [Aktivieren von Adobe Analytics-Videoberichten](enabling-analytics-video-reports.md). |
| SWATCH | X (Flyout, Zoom) | Dieses Viewer-Ereignis wird dem PAGE-Viewer-Ereignis in Dynamic Media Classic zugeordnet. |
| ZOOM | **X** (E-Katalog, Rotationsset, Zoom) | Wird nicht von Adobe Analytics verfolgt.<br> |
| PAN | **X** (E-Katalog, Rotationsset, Zoom) | Wird nicht von Adobe Analytics verfolgt.<br> |
| SPIN | **X** (Rotationsset) | Wird nicht von Adobe Analytics verfolgt.<br> |


### Dynamic Media Classic-Variablen {#scene-variables}

Wählen Sie für jedes Viewer-Ereignis im Bildschirm &quot;Adobe Analytics-Konfiguration&quot;eine Adobe Analytics-Variable und eine *Dynamic Media Classic-Variable*. Dynamic Media Classic-Variablen stellen Daten dar, die Sie für einen Bericht abrufen können. Zum Beispiel listet die Variable `searchTerm` Schlüsselwörter auf, die in E-Katalog-Suchvorgängen verwendet wurden.

In der folgenden Tabelle werden die Variablen von Dynamic Media Classic beschrieben.

| Dynamic Media Classic-Variable | Beschreibung |
|--- |:--- |
| asset | Dynamic Media Classic-Asset-ID oder Videopfaddatei. |
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

## Aktivieren, Bearbeiten und Löschen von Viewer-Ereignissen  {#activating-editing-and-deleting-viewer-events}

Im Anzeigebereich „Adobe Analytics-Konfiguration“ können Sie Viewer-Ereignisse aktivieren, bearbeiten und löschen:

* ****
AktivierenKlicken Sie auf  **** Aktivieren bzw.  **** Deaktivieren, um ein ausgewähltes Viewer-Ereignis zu deaktivieren.

* ****
BearbeitenWählen Sie ein Viewer-Ereignis aus und klicken Sie auf die graue Schaltfläche  **[!UICONTROL Ansicht/]** BearbeitenVariablen. Wählen Sie in den Dropdown-Listen &quot;Dynamic Media Classic Variable&quot;und &quot;Adobe Analytics Variable&quot;eine andere Variable aus den jeweiligen Listen. Weitere Informationen finden Sie unter Zuweisen von Adobe Analytics-Variablen zu Dynamic Media Classic Viewer-Ereignissen und -Variablen.

* **Löschen**
Wählen Sie ein Viewer-Ereignis aus und klicken Sie auf die graue Schaltfläche  **[!UICONTROL Ansicht/]** BearbeitenVariablen. Klicken Sie auf „**[!UICONTROL Löschen]**“.
