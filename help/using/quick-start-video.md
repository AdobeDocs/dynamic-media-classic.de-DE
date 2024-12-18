---
title: 'Schnellstart: Video in Adobe Dynamic Media Classic'
description: Eine Einführung und eine Kurzanleitung in Adobe Dynamic Media Classic Video, um Ihnen den schnellen Einstieg zu erleichtern.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
topic: Content Management
level: Beginner
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1443'
ht-degree: 23%

---

# Schnellstart: Video in Adobe Dynamic Media Classic{#quick-start-video}

Adobe Dynamic Media Classic Video ist eine End-to-End-Lösung, mit der Sie hochwertige adaptive Videos für das Streaming auf mehreren Bildschirmen veröffentlichen können, einschließlich Desktop-Geräten, iOS, Android™, BlackBerry® und Windows®-Mobilgeräten. Bei adaptiven Videosets werden Versionen desselben Videos gruppiert, die in unterschiedlichen Bitraten und Formaten kodiert sind, z. B. mit 400 Kbit/s, 800 Kbit/s und 1000 Kbit/s. Der Desktop-Computer oder das Mobilgerät erkennt die verfügbare Bandbreite.

Zum Beispiel werden auf einem iOS-Mobilgerät Bandbreiten wie 3G, 4G oder Wi-Fi erkannt. Anschließend wird unter den verschiedenen Video-Bitraten innerhalb des adaptiven Videosets automatisch das richtig kodierte Video ausgewählt. Das Video wird auf Desktops, Mobilgeräte und Tablets gestreamt.

Außerdem wird die Videoqualität automatisch angepasst, wenn sich die Netzwerkbedingungen des Desktop- oder Mobilgeräts ändern. Wenn darüber hinaus ein Kunde den Vollbildmodus an einem Desktop aktiviert, reagiert das adaptive Videoset, indem eine bessere Auflösung verwendet wird, um das Anzeigeerlebnis des Kunden zu verbessern. Adaptive Videosets bieten Ihnen bestmögliche Wiedergabe. Dies eignet sich am besten für Kunden, die Adobe Dynamic Media Classic-Videos auf mehreren Bildschirmen und Geräten wiedergeben.

Die Logik, die ein Video-Player verwendet, um das richtige kodierte Video für die Wiedergabe auszuwählen, basiert auf dem folgenden Algorithmus:

1. Der Video-Player lädt das anfängliche Videofragment auf der Grundlage der Bitrate, die am nächsten an dem Wert liegt, der im Player selbst als „anfängliche Bitrate“ festgelegt wurde.
1. Video-Player wechselt auf der Grundlage von Änderungen an der Bandbreitengeschwindigkeit anhand der folgenden Kriterien:

   1. Der Player wählt den höchsten Bandbreitenstrom aus, der kleiner oder gleich der geschätzten Bandbreite ist.
   1. Player berücksichtigt nur 80 % der verfügbaren Bandbreite. Wenn er jedoch nach oben wechselt, ist er mit nur 70 % konservativer, um Überschätzungen zu vermeiden und sofort zurückzuwechseln.

Technische Informationen finden Sie in der Algorithmuslogik unter ](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp)0}https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp&quot;.[

Für die Verwaltung von Einzelvideos und adaptiven Videosets unterstützt Adobe Dynamic Media Classic Folgendes:

* Hochladen von Videos aus zahlreichen unterstützten Videoformaten. Und das Hochladen von Audioformaten und Kodieren von Videos in das MP4 H.264-Format für die Wiedergabe auf mehreren Bildschirmen. Sie können vordefinierte adaptive Adobe Dynamic Media Classic-Videovorgaben oder einzelne Videokodierungsvorgaben verwenden oder Ihre eigene Kodierung anpassen, um die Qualität und Größe des Videos zu steuern.

Siehe [Aktivieren oder Deaktivieren von adaptiven Videovorgaben](/help/using/application-setup.md#activating-or-deactivating-adaptive-video-presets)

Siehe auch [Videovorgaben](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) Schulungsvideo.

Wenn ein adaptives Videoset generiert wird, enthält es MP4-Videos.

>[!NOTE]
>
>Primär-/Quellvideos und andere Quellvideos werden *nicht* einem adaptiven Videoset hinzugefügt.

* Videountertitelung in den Viewern „Universal_HTML5_Video“, „Universal_HTML5_MixedMedia_dark“ und „Universal_HTML5_MixedMedia_light“ sowie Videokapitelnavigation in den Viewern „Universal_HTML5_Video“, „Universal_HTML5_MixedMedia_dark“ und „Universal_HTML5_MixedMedia_light“.

  Siehe [Hinzufügen von Untertiteln zu einem Video](adding-captions-video.md).

  Siehe [Hinzufügen von Kapitelmarken zu einem Video](adding-chapter-markers-video.md).

* Organisieren, Durchsuchen und Suchen von Videos mit vollständiger Metadatenunterstützung für eine effiziente Verwaltung von Video-Assets.
* Stellen Sie adaptive Videosets im Internet sowie für Desktops und Mobilgeräte bereit, einschließlich iPhone, iPad, Android™, BlackBerry® und Windows® Phone.

  Adaptives Video-Streaming wird auf verschiedenen iOS-Plattformen unterstützt.

  Die neueste Unterstützung finden Sie im [Adobe Viewer-Referenzhandbuch](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources).

  Adobe Dynamic Media Classic unterstützt die mobile Videowiedergabe für MP4 H.264-Videos. <!-- LINK IS 404; NO SUITABLE REPLACEMENT WAS FOUND You can find BlackBerry&reg; devices that support this video format at the following website: -->

  <!-- See [Supported video formats on BlackBerry&reg;](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482). -->

  Welche Windows®-Geräte dieses Videoformat unterstützen, können Sie hier einsehen:

  [Unterstützte Videoformate unter Windows® Phone](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs).

* Wiedergabe von Videos mit Adobe Dynamic Media Classic-Viewer-Vorgaben, einschließlich der folgenden:

   * Einzelne Video-Viewer.
   * Viewer für gemischte Medien, die Video- und Bildinhalte kombinieren

* Konfigurieren von Video-Playern für individuelle Branding-Anforderungen
* Integrieren Sie Videos mit einer einfachen URL oder mit Einbettungs-Code in Ihre Website, mobile Site oder mobile Anwendung.

Siehe die folgenden Schulungsvideos:
* [MP4-Videoübersicht](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [MP4-Videovorschau](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [MP4-Video-Upload](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [Streaming - Übersicht](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**Schnellstart**

Die folgende schrittweise Workflow-Beschreibung soll Ihnen den schnellen Einstieg in adaptive Videosets in Adobe Dynamic Media Classic erleichtern. Nach jedem Schritt finden Sie einen Querverweis auf eine Themenüberschrift, unter der Sie weitere Informationen finden.

## 1. Videos hochladen und kodieren

Generieren und laden Sie adaptive Videosets mithilfe eines der beiden folgenden Szenarien hoch:

* **Vorkodierte Videos hochladen**: Wenn Ihre Videos bereits extern in Adobe Dynamic Media Classic kodiert wurden, wählen Sie in der Symbolleiste für globale Navigation **[!UICONTROL Hochladen]** aus. Durchsuchen Sie MP4-Videodateien und laden Sie sie direkt in Adobe Dynamic Media Classic hoch. Navigieren Sie dann zu **[!UICONTROL Erstellen]** > **[!UICONTROL Adaptive Videosets]**. Navigieren Sie zu Ihren Videodateien. Ziehen Sie die gewünschten Videodateien per Drag-and-Drop in die Tabelle Adaptives Videoset und speichern Sie dann das Set.
* **Primärvideos hochladen**: Wenn Ihre Videos nicht kodiert sind, wählen Sie in der Symbolleiste für die globale Navigation die Option **[!UICONTROL Hochladen]** aus, um primäre Videoquelldateien (keine MP4) hochzuladen. Adobe Dynamic Media Classic kodiert sie für Sie in MP4-Dateien. Wählen **[!UICONTROL Dialogfeld Upload-Auftragsoptionen]** unter **[!UICONTROL EVideo-Optionen]** die Option **[!UICONTROL Adaptives Video]**.

  Mit dieser bevorzugten Option können Sie adaptive Videosets erstellen. Die richtige Kodierungsvorgabe wird automatisch auf das Video angewendet (16:9 oder 4:3), damit sie den Abmessungen des hochgeladenen Videos entspricht. Wenn Sie Ihren Upload-Auftrag übermitteln, wird automatisch ein adaptives Videoset erstellt, das drei Videocodierungseinstellungen im richtigen Seitenverhältnis enthält.

  Oder erweitern Sie im selben **[!UICONTROL Auftragsoptionen]**-Dialogfeld unter **[!UICONTROL EVideo-Optionen]** die Option **[!UICONTROL Einzelne Kodierungsvorgaben]**. Wählen Sie die gewünschten individuellen Videokodierungsvorgaben aus. Sie können **Desktop**, **Mobile (iPhone, iPad, Android™)** und **Tablet (iPad, Android™)** auswählen, um die MP4-Dateien zu erstellen.

* Sie können auch ein primäres Video mit der Funktion **[!UICONTROL Neuverarbeitung]** erneut verarbeiten. Die neu kodierten Videos werden dem vorhandenen adaptiven Videoset hinzugefügt.

Siehe [Hochladen und Kodieren von Videos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Optional**

Adobe Dynamic Media Classic bietet zahlreiche vordefinierte Videokodierungsvorgaben. Diese vordefinierten Vorgaben entsprechen den gängigsten Videokodierungseinstellungen, die heute verwendet werden, und sind für die Wiedergabe auf Zielseiten optimiert.

Außerdem können Administratoren, wenn eine weitere Anpassung erforderlich ist, Video-Vorgaben erstellen, um die Größe und Wiedergabe von eVideo für Endbenutzer anzupassen. Administratoren können Videovorgaben über die Seite „Videovorgaben“ unter &quot;****&quot; > &quot;**[!UICONTROL &quot; > &quot;]**&quot; > &quot;**[!UICONTROL &quot; > &quot;]**&quot; > &quot;**[!UICONTROL &quot; hinzufügen und]**. Auf der Seite „Video-Vorgaben“ finden Sie Optionen, um Video-Vorgaben hinzuzufügen, zu bearbeiten, zu löschen und zu aktivieren. 

Siehe [Arbeiten mit Videocodierungsvorgaben](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2. Vorschau von Videos in einem Video-Viewer

Um zu sehen, wie ein Video für Endbenutzende auf einem Desktop, einer Website oder einem Mobilgerät wiedergegeben wird, wählen Sie das Video im Durchsuchen-Panel aus. Wählen Sie dann **[!UICONTROL Vorschau]** aus.

Siehe [Vorschau von Videos in einem Video-Viewer](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Sie können das Video auf der Vorschauseite wiedergeben. Sie können auch verschiedene Video-Viewer auswählen, um herauszufinden, wie Ihr Video in verschiedenen Playern angezeigt wird. Wir empfehlen, dass Sie den HTML5 Video-Player für die Wiedergabe auf verschiedenen Anzeigegeräten wie Desktop, Tablet und Mobilgeräte verwenden.

**Optional**

Anpassung von Viewer-Vorgaben: Adobe Dynamic Media Classic bietet vordefinierte Viewer-Vorgaben für die Bereitstellung von Videos. Diese Vorgaben bestimmen das Aussehen des Viewers und die Funktionsweise der Wiedergabe-Steuerelemente. Zum Anpassen des Video-Viewers können Administratoren die Viewer-Vorgaben über die Seite „Viewer-Vorgaben“ hinzufügen und verwalten. Um diese Seite zu öffnen, klicken Sie in der rechten oberen Ecke von Adobe Dynamic Media Classic auf **[!UICONTROL Setup]** > **[!UICONTROL Viewer-Vorgaben]**. Auf der Seite „Viewer-Vorgaben“ finden Sie Befehle, um Viewer-Vorgaben hinzuzufügen, zu bearbeiten, zu löschen und zu aktivieren. 

Siehe [Arbeiten mit Video-Viewer-](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

Siehe auch [Videovorgaben](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) Schulungsvideo.

## 3. Bereitstellen von Videos auf Ihren Websites und mobilen Sites

Führen Sie einen der folgenden Schritte aus, um Video in Ihre Website zu integrieren:

* Zeigen Sie das Video in einem eigenen Popup- oder modalen Fenster an. Verwenden Sie in diesem Fall die Funktion **[!UICONTROL URL kopieren]**.

  Um die URL für ein Video abzurufen, wählen Sie sie in der Rasteransicht oder Listenansicht im Durchsuchen-Panel aus. Wählen Sie **[!UICONTROL Vorschau]** und dann **[!UICONTROL URL kopieren]** rechts von `Universal_HTML5_Viewer` aus.

  Wenn Sie **[!UICONTROL URL kopieren]** auswählen, wird die URL in die Zwischenablage kopiert. Fügen Sie diesen Code in den HTML-Code Ihrer Website, mobilen Site oder Anwendung ein. 

  >[!NOTE]
  >
  >URLs werden erst aktiv, nachdem Sie das Video oder das adaptive Videoset veröffentlicht haben.

* Zeigen Sie das auf der Web-Seite eingebettete Video an. Verwenden Sie in diesem Fall die Funktion **[!UICONTROL Einbettungs-Code]**.

  Um den Einbettungs-Code für ein Video abzurufen, wählen Sie in der Rasteransicht oder Listenansicht das Video im Durchsuchen-Panel aus. Navigieren Sie **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**. Wählen Sie in der Spalte Aktionen der Tabelle **[!UICONTROL Einbettungs-Code]** rechts von `Universal_HTML5_Video` aus. Das Bearbeiten des Codes ist nicht zulässig.

  Wählen Sie **[!UICONTROL Schließen]** und fügen Sie den Einbettungs-Code in eine oder mehrere Ihrer Web-Seiten ein.

  >[!NOTE]
  >
  >Der Einbettungs-Code wird erst aktiviert, nachdem Sie das Video oder adaptive Videoset veröffentlicht haben.

Siehe [Bereitstellen von Videos auf Ihren Websites und mobilen Sites](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Optimale Vorgehensweisen für die Videokodierung](uploading-encoding-videos.md#best_practices_for_video_encoding)
