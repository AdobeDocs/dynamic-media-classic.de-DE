---
title: 'Schnellstart: Video in Adobe Dynamic Media Classic'
description: Eine Einführung und ein Schnellstart zum Adobe Dynamic Media Classic-Video, mit dem Sie schnell anfangen können.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
topic: Content Management
level: Beginner
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '1443'
ht-degree: 28%

---

# Schnellstart: Video in Adobe Dynamic Media Classic{#quick-start-video}

Adobe Dynamic Media Classic Video ist eine End-to-End-Lösung, mit der Sie hochwertige adaptive Videos für das Streaming auf mehreren Bildschirmen veröffentlichen können, darunter Desktop-, iOS-, Android™-, BlackBerry®- und Windows®-Mobilgeräte. Bei adaptiven Videosets werden Versionen desselben Videos gruppiert, die in unterschiedlichen Bitraten und Formaten kodiert sind, z. B. mit 400 Kbit/s, 800 Kbit/s und 1000 Kbit/s. Der Desktop-Computer oder das Mobilgerät erkennt die verfügbare Bandbreite.

Zum Beispiel werden auf einem iOS-Mobilgerät Bandbreiten wie 3G, 4G oder Wi-Fi erkannt. Anschließend wird unter den verschiedenen Video-Bitraten innerhalb des adaptiven Videosets automatisch das richtig kodierte Video ausgewählt. Das Video wird auf Desktops, Mobilgeräte und Tablets gestreamt.

Außerdem wird die Videoqualität automatisch angepasst, wenn sich die Netzwerkbedingungen des Desktop- oder Mobilgeräts ändern. Wenn ein Kunde auf einem Desktop in den Vollbildmodus wechselt, antwortet das adaptive Videoset mit einer besseren Auflösung, wodurch das Anzeigeerlebnis des Kunden verbessert wird. Mit adaptiven Videosets erhalten Sie die bestmögliche Wiedergabe. Dies eignet sich am besten für Kunden, die Adobe Dynamic Media Classic-Videos auf mehreren Bildschirmen und Geräten wiedergeben.

Die Logik, die ein Video-Player verwendet, um das richtige kodierte Video für die Wiedergabe auszuwählen, basiert auf dem folgenden Algorithmus:

1. Der Videoplayer lädt das anfängliche Videofragment basierend auf der Bitrate, die dem für &quot;initiale Bitrate&quot;im Player selbst festgelegten Wert am nächsten ist.
1. Der Videoplayer wechselt auf der Grundlage von Änderungen der Bandbreitengeschwindigkeit mithilfe der folgenden Kriterien:

   1. Der Player wählt den höchsten Bandbreitenstream aus, der unter der geschätzten Bandbreite liegt oder dieser entspricht.
   1. Der Player berücksichtigt nur 80 % der verfügbaren Bandbreite. Wenn er jedoch nach oben wechselt, ist er bei nur 70 % konservativer, um Überschätzungen zu vermeiden und sofort zurückzuwechseln.

Die Logik des Algorithmus finden Sie unter [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) für technische Informationen.

Für die Verwaltung von einzelnen Videos und adaptiven Videosets unterstützt Adobe Dynamic Media Classic Folgendes:

* Hochladen von Videos aus zahlreichen unterstützten Videoformaten. Außerdem können Sie Audioformate hochladen und Videos in das MP4 H.264-Format kodieren, um sie auf mehreren Bildschirmen wiederzugeben. Sie können vordefinierte Adobe Dynamic Media Classic Adaptive Video-Vorgaben oder einzelne Videokodierungsvorgaben verwenden oder Ihre eigene Kodierung anpassen, um die Qualität und Größe des Videos zu steuern.

Siehe [Aktivieren oder Deaktivieren von adaptiven Videovorgaben](/help/using/application-setup.md#activating-or-deactivating-adaptive-video-presets)

Siehe auch [Videovorgaben](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) Schulungsvideo.

Wenn ein adaptives Videoset generiert wird, enthält es MP4-Videos.

>[!NOTE]
>
>Primäre/Quellvideos und andere Quellvideos sind *not* zu einem adaptiven Videoset hinzugefügt.

* Videountertitel in den Viewern Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark, Universal_HTML5_MixedMedia_light und Videokapitelnavigation in den Viewern Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark und Universal_HTML5_MixedMedia_light.

  Siehe [Hinzufügen von Untertiteln zu Videos](adding-captions-video.md).

  Siehe [Hinzufügen von Kapitelmarken zu einem Video](adding-chapter-markers-video.md).

* Organisieren, Durchsuchen und Suchen von Videos mit vollständiger Metadatenunterstützung für eine effiziente Verwaltung von Video-Assets.
* Stellen Sie adaptive Videosets für das Web sowie für Desktops und Mobilgeräte bereit, einschließlich iPhone, iPad, Android™, BlackBerry® und Windows® Phone.

  Das adaptive Video-Streaming wird auf verschiedenen iOS-Plattformen unterstützt.

  Siehe neueste Unterstützung im Abschnitt . [Adobe Viewer-Referenzhandbuch](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources).

  Adobe Dynamic Media Classic unterstützt die mobile Videowiedergabe für MP4 H.264-Videos. <!-- LINK IS 404; NO SUITABLE REPLACEMENT WAS FOUND You can find BlackBerry&reg; devices that support this video format at the following website: -->

  <!-- See [Supported video formats on BlackBerry&reg;](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482). -->

  Windows®-Geräte, die dieses Videoformat unterstützen, finden Sie unter:

  [Unterstützte Videoformate auf Windows® Phone](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs).

* Wiedergabe des Videos mit Adobe Dynamic Media Classic-Viewer-Vorgaben, einschließlich der folgenden:

   * Einzelvideo-Viewer.
   * Viewer für gemischte Medien, die Video- und Bildinhalte kombinieren

* Konfigurieren von Video-Playern für individuelle Branding-Anforderungen
* Integrieren von Videos in Websites, mobile Sites oder mobile Anwendungen über eine einfache URL oder einen eingebetteten Code.

Sehen Sie sich die folgenden Schulungsvideos an:
* [MP4-Videoübersicht](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [MP4-Videovorschau](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [MP4-Video-Upload](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [Streaming-Übersicht](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**Schnellstart**

Die folgende schrittweise Workflow-Beschreibung soll Ihnen dabei helfen, in Adobe Dynamic Media Classic schnell mit adaptiven Videosets zu arbeiten. Nach jedem Schritt gibt es einen Querverweis zu einer Themenüberschrift, in der Sie weitere Informationen finden können.

## 1. Hochladen und Kodieren von Videos

Generieren und laden Sie adaptive Videosets mithilfe eines der beiden folgenden Szenarien hoch:

* **Hochladen vorkodierter Videos**: Wenn Ihre Videos bereits extern aus Adobe Dynamic Media Classic kodiert wurden, wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Hochladen]**. Suchen Sie nach MP4-Videodateien und laden Sie sie direkt in Adobe Dynamic Media Classic hoch. Gehen Sie dann zu **[!UICONTROL Build]** > **[!UICONTROL Adaptive Videosets]**. Navigieren Sie zu Ihren Videodateien. Ziehen Sie die gewünschten Videodateien per Drag-and-Drop in die Tabelle Adaptives Videoset und speichern Sie das Set.
* **Hochladen von Primärvideos**: Wenn Ihre Videos nicht kodiert sind, wählen Sie in der Symbolleiste für globale Navigation die Option **[!UICONTROL Hochladen]** , um die Primärvideoquelldateien (nicht MP4) hochzuladen. Adobe Dynamic Media Classic kodiert sie in MP4-Dateien für Sie. Im **[!UICONTROL Upload-Auftragsoptionen]** Dialogfeld, unter **[!UICONTROL eVideooptionen]** auswählen **[!UICONTROL Adaptives Video]**.

  Mit dieser bevorzugten Option können Sie adaptive Videosets erstellen. Die richtige Kodierungsvorgabe wird automatisch auf das Video angewendet, unabhängig davon, ob es sich um 16:9 oder 4:3 handelt, um sie an die Abmessungen des hochgeladenen Videos anzupassen. Wenn Sie Ihren Upload-Auftrag senden, wird automatisch ein adaptives Videoset erstellt, das drei Videoparameter für die Videokodierung im richtigen Seitenverhältnis enthält.

  Oder im selben **[!UICONTROL Auftragsoptionen]** Dialogfeld, unter **[!UICONTROL eVideooptionen]**, erweitern **[!UICONTROL Einzelne Kodierungsvorgaben]**. Wählen Sie die gewünschten individuellen Videokodierungsvorgaben aus. Sie können **Desktop**, **Mobil (iPhone, iPad, Android™)**, und **Tablet (iPad, Android™)** , um die MP4-Dateien zu erstellen.

* Alternativ können Sie ein Primärvideo mithilfe der **[!UICONTROL Wiederaufbereitung]** Funktion. Die neu kodierten Videos werden dem vorhandenen adaptiven Videoset hinzugefügt.

Siehe [Hochladen und Kodieren von Videos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Optional**

Adobe Dynamic Media Classic bietet zahlreiche vordefinierte Vorgaben für die Videokodierung. Diese vordefinierten Vorgaben spiegeln die am häufigsten verwendeten Videokodierungsparameter wider und sind für die Wiedergabe auf Zielseiten optimiert.

Außerdem können Administratoren, wenn eine weitere Anpassung erforderlich ist, Video-Vorgaben erstellen, um die Größe und Wiedergabe von eVideo für Endbenutzer anzupassen. Administratoren können Videovorgaben über die Seite &quot;Videovorgaben&quot;hinzufügen und verwalten, die unter **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Videovorgaben]** > **[!UICONTROL Einzelne Kodierungsvorgaben]**. Auf der Seite „Video-Vorgaben“ finden Sie Optionen, um Video-Vorgaben hinzuzufügen, zu bearbeiten, zu löschen und zu aktivieren. 

Siehe [Arbeiten mit Videokodierungsvorgaben](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2. Vorschau von Videos in einem Video-Viewer

Um zu sehen, wie ein Video für Endbenutzer auf einem Desktop, Ihrer Website oder einem Mobilgerät wiedergegeben wird, wählen Sie das Video im Durchsuchenbedienfeld aus. Wählen Sie anschließend **[!UICONTROL Vorschau]**.

Siehe [Vorschau von Videos in einem Video-Viewer](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Sie können das Video auf der Seite &quot;Vorschau&quot;abspielen. Sie können auch verschiedene Video-Viewer auswählen, um herauszufinden, wie Ihr Video in verschiedenen Playern angezeigt wird. Wir empfehlen, dass Sie den HTML5 Video-Player für die Wiedergabe auf verschiedenen Anzeigegeräten wie Desktop, Tablet und Mobilgeräte verwenden.

**Optional**

Anpassung von Viewer-Vorgaben - Adobe Dynamic Media Classic bietet vordefinierte Viewer-Vorgaben für die Bereitstellung von Videos. Diese Vorgaben bestimmen das Aussehen des Viewers und die Funktionsweise der Wiedergabe-Steuerelemente. Zum Anpassen des Video-Viewers können Administratoren die Viewer-Vorgaben über die Seite „Viewer-Vorgaben“ hinzufügen und verwalten. Um diese Seite zu öffnen, navigieren Sie oben rechts in Adobe Dynamic Media Classic zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Viewer-Vorgaben]**. Auf der Seite „Viewer-Vorgaben“ finden Sie Befehle, um Viewer-Vorgaben hinzuzufügen, zu bearbeiten, zu löschen und zu aktivieren. 

Siehe [Arbeiten mit Video-Viewer-Vorgaben](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

Siehe auch [Videovorgaben](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) Schulungsvideo.

## 3. Bereitstellen von Videos auf Ihren Websites und mobilen Sites

Führen Sie einen der folgenden Schritte aus, um Video in Ihre Website zu integrieren:

* Zeigen Sie das Video in einem eigenen Popup- oder modalen Fenster an. Verwenden Sie in diesem Fall die **[!UICONTROL URL kopieren]** Funktion.

  Um eine URL für ein Video entweder in der Raster- oder Listenansicht zu erhalten, wählen Sie das Video im Bedienfeld „Durchsuchen“ aus. Auswählen **[!UICONTROL Vorschau]** und wählen Sie **[!UICONTROL URL kopieren]** auf das Recht `Universal_HTML5_Viewer`.

  Wenn Sie **[!UICONTROL URL kopieren]**, wird die URL in die Zwischenablage kopiert. Fügen Sie diesen Code in den HTML-Code Ihrer Website, mobilen Site oder Anwendung ein. 

  >[!NOTE]
  >
  >URLs werden erst aktiv, nachdem Sie das Video oder das adaptive Videoset veröffentlicht haben.

* Zeigen Sie das eingebettete Video auf der Web-Seite an. Verwenden Sie in diesem Fall die **[!UICONTROL Einbettungscode]** Funktion.

  Um den Einbettungscode für ein Video entweder in der Raster- oder Listenansicht zu erhalten, wählen Sie das Video im Bedienfeld „Durchsuchen“ aus. Navigieren Sie zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**. Wählen Sie in der Spalte Aktionen der Tabelle die Option **[!UICONTROL Einbettungscode]** auf das Recht `Universal_HTML5_Video`. Das Bearbeiten des Codes ist nicht zulässig.

  Auswählen **[!UICONTROL Schließen]** und fügen Sie den Einbettungscode in eine oder mehrere Ihrer Webseiten ein.

  >[!NOTE]
  >
  >Der Einbettungscode wird erst aktiviert, nachdem Sie das Video oder das adaptive Videoset veröffentlicht haben.

Siehe [Bereitstellen von Videos auf Ihren Websites und mobilen Sites](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Optimale Vorgehensweisen für die Videokodierung](uploading-encoding-videos.md#best_practices_for_video_encoding)
