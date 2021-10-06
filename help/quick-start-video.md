---
title: '"Schnellstart: Video in Adobe Dynamic Media Classic"'
description: Eine Einführung und ein Schnellstart zum Adobe Dynamic Media Classic-Video, mit dem Sie schnell anfangen können.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '1806'
ht-degree: 28%

---

# Schnellstart: Video in Adobe Dynamic Media Classic{#quick-start-video}

Adobe Dynamic Media Classic Video ist eine End-to-End-Lösung, mit der Sie hochwertige adaptive Videos für das Streaming auf mehreren Bildschirmen veröffentlichen können, darunter Desktop-, iOS-, Android™-, BlackBerry®- und Windows®-Mobilgeräte. Bei adaptiven Videosets werden Versionen desselben Videos gruppiert, die in unterschiedlichen Bitraten und Formaten kodiert sind, z. B. mit 400 Kbit/s, 800 Kbit/s und 1000 Kbit/s. Der Desktop-Computer oder das Mobilgerät erkennt die verfügbare Bandbreite.

Zum Beispiel werden auf einem iOS-Mobilgerät Bandbreiten wie 3G, 4G oder Wi-Fi erkannt. Anschließend wird unter den verschiedenen Video-Bitraten innerhalb des adaptiven Videosets automatisch das richtig kodierte Video ausgewählt. Das Video wird auf Desktops, Mobilgeräte und Tablets gestreamt.

Außerdem wird die Videoqualität automatisch angepasst, wenn sich die Netzwerkbedingungen des Desktop- oder Mobilgeräts ändern. Wenn ein Kunde auf einem Desktop in den Vollbildmodus wechselt, antwortet das adaptive Videoset mit einer besseren Auflösung, wodurch das Anzeigeerlebnis des Kunden verbessert wird. Mit adaptiven Videosets erhalten Sie die bestmögliche Wiedergabe für Kunden, die Adobe Dynamic Media Classic-Videos auf mehreren Bildschirmen und Geräten wiedergeben.

Die Logik, die ein Video-Player verwendet, um das richtige kodierte Video für die Wiedergabe auszuwählen, basiert auf dem folgenden Algorithmus:

1. Der Video-Player lädt das anfängliche Videofragment basierend auf der Bitrate, die dem für &quot;initiale Bitrate&quot;im Player selbst festgelegten Wert am nächsten ist.
1. Der Videoplayer wechselt anhand von Änderungen der Bandbreitengeschwindigkeit mithilfe der folgenden Kriterien:

   1. Der Player wählt den höchsten Bandbreitenstream aus, der unter der geschätzten Bandbreite liegt oder dieser entspricht.
   1. Der Player berücksichtigt nur 80 % der verfügbaren Bandbreite. Wenn es jedoch nach oben wechselt, ist es konservativer mit nur 70 %, um Überschätzungen zu vermeiden und sofort zurückzuwechseln.

Technische Informationen dazu finden Sie in der Logik des Algorithmus unter [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp).

Adobe Dynamic Media Classic unterstützt für die Verwaltung von Einzelvideo- und adaptiven Videosets Folgendes:

* Das Hochladen von Video aus verschiedenen unterstützten Videoformaten und Audioformaten und das Kodieren von Video im MP4 H.264-Format für die Wiedergabe auf verschiedenen Anzeigemedien. Sie können vordefinierte adaptive Adobe Dynamic Media Classic-Videovorgaben oder einzelne Videokodierungsvorgaben verwenden oder Ihre eigene Kodierung anpassen, um die Qualität und Größe des Videos zu steuern.

Siehe [Aktivieren oder Deaktivieren von adaptiven Videovorgaben](/help/application-setup.md#activating-or-deactivating-adaptive-video-presets)

Siehe auch Schulungsvideo zu [Videovorgaben](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS).

Wenn ein adaptives Videoset generiert wird, enthält es MP4-Videos.

>[!NOTE]
>
>Übergeordnete/Quellvideos und andere Quellvideos werden *nicht* zu einem adaptiven Videoset hinzugefügt.

* Videountertitel in den Viewern Universal_HTML5_Video, Universal_HTML5_MixedMedia_dark, Universal_HTML5_MixedMedia_light und Videokapitelnavigation in den Viewern Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark und Universal_HTML5_MixedMedia_light.

   Siehe [Hinzufügen von Untertiteln zu Video](adding-captions-video.md).

   Siehe [Hinzufügen von Kapitelmarken zu Video](adding-chapter-markers-video.md).

* Organisieren, Durchsuchen und Suchen von Videos mit vollständiger Metadatenunterstützung für eine effiziente Verwaltung von Video-Assets.
* Bereitstellen von adaptiven Videosets für das Web, Desktops und Mobilgeräte, einschließlich iPhone, iPad, Android™, BlackBerry® und Windows® Phone.

   Das adaptive Video-Streaming wird auf verschiedenen iOS-Plattformen unterstützt.

   Weitere Informationen finden Sie im [Adobe Viewer-Referenzhandbuch](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

   Adobe Dynamic Media Classic unterstützt die mobile Videowiedergabe für MP4 H.264-Videos. BlackBerry®-Geräte, die dieses Videoformat unterstützen, finden Sie auf folgender Website:

   Siehe [Unterstützte Videoformate auf BlackBerry®](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   Windows®-Geräte, die dieses Videoformat unterstützen, finden Sie unter:

   Siehe [Unterstützte Videoformate unter Windows® Phone](https://docs.microsoft.com/en-us/).

* Wiedergabe des Videos mit Adobe Dynamic Media Classic-Viewer-Vorgaben, einschließlich der folgenden:

   * Einzel-Video-Viewer
   * Viewer für gemischte Medien, die Video- und Bildinhalte kombinieren

* Konfigurieren von Video-Playern für individuelle Branding-Anforderungen
* Integrieren von Videos in Websites, mobile Sites oder mobile Anwendungen über eine einfache URL oder einen eingebetteten Code.

Sehen Sie sich die folgenden Schulungsvideos an:
* [MP4-Videoübersicht](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [MP4-Videovorschau](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [MP4-Video-Upload](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [Streaming-Übersicht](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**Schnellstart**

Die folgende schrittweise Workflow-Beschreibung soll Ihnen dabei helfen, adaptive Videosets in Adobe Dynamic Media Classic einzurichten und schnell auszuführen. Nach jedem Schritt wird auf ein Thema mit weiteren Informationen verwiesen.

## 1. Hochladen und Kodieren von Videos

Generieren und laden Sie adaptive Videosets mithilfe eines der beiden folgenden Szenarien hoch:

* **Vorkodierte Videos hochladen**  - Wenn Ihre Videos bereits außerhalb von Adobe Dynamic Media Classic kodiert wurden, wählen Sie in der Symbolleiste für globale Navigation die Option  **** Hochladen aus, um die MP4-Videodateien direkt zu durchsuchen und in Adobe Dynamic Media Classic hochzuladen. Gehen Sie dann zu **[!UICONTROL Build]** > **[!UICONTROL Adaptive Videosets]**. Navigieren Sie zu Ihren Videodateien. Fügen Sie die gewünschten Videodateien per Drag &amp; Drop in die Tabelle für adaptive Videosets ein und speichern Sie das Set.
* **Übergeordnete Quellvideos hochladen**  - Wenn Ihre Videos nicht kodiert sind, wählen Sie in der Symbolleiste für globale Navigation die Option  **** Hochladen aus, um Übergeordnete Videoquelldateien (nicht MP4) hochzuladen. Adobe Dynamic Media Classic kodiert sie in MP4-Dateien für Sie. Wählen Sie im Dialogfeld **[!UICONTROL Upload-Auftragsoptionen]** unter **[!UICONTROL eVideo-Optionen]** die Option **[!UICONTROL Adaptives Video]**.

   Mit dieser bevorzugten Option können Sie ein adaptives Videoset erstellen, das automatisch die korrekte Kodierungsvorgabe (16:9 oder 4:3) entsprechend den Abmessungen des hochgeladenen Videos anpasst. Wenn Sie Ihren Upload-Auftrag senden, wird automatisch ein adaptives Videoset erstellt, das drei Videoeinstellungen im richtigen Seitenverhältnis kodiert.

   Oder erweitern Sie im selben Dialogfeld **[!UICONTROL Auftragsoptionen]** unter **[!UICONTROL eVideo-Optionen]** **[!UICONTROL Einzelne Kodierungsvorgaben]**. Wählen Sie unter **Desktop**, **Mobil (iPhone, iPad, Android™)** und **Tablet (iPad, Android™)** die gewünschten Vorgaben für die Videokodierung aus, um die MP4-Dateien zu erstellen.

* Alternativ können Sie ein Übergeordnetes Video mit der Funktion **[!UICONTROL Reprocess]** erneut verarbeiten. Die neu kodierten Videos werden dem vorhandenen adaptiven Videoset hinzugefügt.

Siehe [Hochladen und Kodieren von Videos](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Optional**

Adobe Dynamic Media Classic bietet zahlreiche vordefinierte Vorgaben für die Videokodierung. Diese vordefinierten Vorgaben spiegeln die am häufigsten verwendeten Videokodierungsparameter wider und sind für die Wiedergabe auf Zielseiten optimiert.

Außerdem können Administratoren, wenn eine weitere Anpassung erforderlich ist, Video-Vorgaben erstellen, um die Größe und Wiedergabe von eVideo für Endbenutzer anzupassen. Administratoren können Videovorgaben über die Seite &quot;Videovorgaben&quot;hinzufügen und verwalten, die unter **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Videovorgaben]** > **[!UICONTROL Einzelne Kodierungsvorgaben]** verfügbar ist. Auf der Seite „Video-Vorgaben“ finden Sie Optionen, um Video-Vorgaben hinzuzufügen, zu bearbeiten, zu löschen und zu aktivieren. 

Siehe [Arbeiten mit Videokodierungsvorgaben](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2. Vorschau von Videos in einem Video-Viewer

Um zu sehen, wie ein Video für Endbenutzer auf einem Desktop, Ihrer Website oder einem Mobilgerät wiedergegeben wird, wählen Sie das Video im Durchsuchenbedienfeld aus und klicken Sie dann auf **[!UICONTROL Vorschau]**.

Siehe [Vorschau von Videos in einem Video-Viewer](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Sie können das Video auf der Seite &quot;Vorschau&quot;abspielen. Sie können auch verschiedene Video-Viewer auswählen, um herauszufinden, wie Ihr Video in verschiedenen Playern angezeigt wird. Wir empfehlen, dass Sie den HTML5 Video-Player für die Wiedergabe auf verschiedenen Anzeigegeräten wie Desktop, Tablet und Mobilgeräte verwenden.

**Optional**

Anpassung von Viewer-Vorgaben - Adobe Dynamic Media Classic bietet vordefinierte Viewer-Vorgaben für die Bereitstellung von Videos. Diese Vorgaben bestimmen das Aussehen des Viewers und die Funktionsweise der Wiedergabe-Steuerelemente. Zum Anpassen des Video-Viewers können Administratoren die Viewer-Vorgaben über die Seite „Viewer-Vorgaben“ hinzufügen und verwalten. Um diese Seite zu öffnen, navigieren Sie oben rechts in Adobe Dynamic Media Classic zu **[!UICONTROL Setup]** > **[!UICONTROL Viewer-Vorgaben]**. Auf der Seite „Viewer-Vorgaben“ finden Sie Befehle, um Viewer-Vorgaben hinzuzufügen, zu bearbeiten, zu löschen und zu aktivieren. 

Siehe [Arbeiten mit Video-Viewer-Vorgaben](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

Siehe auch Schulungsvideo zu [Videovorgaben](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS).

## 3. Bereitstellen von Videos auf Ihren Websites und mobilen Sites

Führen Sie einen der folgenden Schritte aus, um Video in Ihre Website zu integrieren:

* Zeigen Sie das Video in einem eigenen Popup- oder modalen Fenster an. Verwenden Sie in diesem Fall die Funktion **[!UICONTROL URL kopieren]** .

   Um eine URL für ein Video entweder in der Raster- oder Listenansicht zu erhalten, wählen Sie das Video im Bedienfeld „Durchsuchen“ aus. Wählen Sie **[!UICONTROL Vorschau]** und dann **[!UICONTROL URL]** rechts von `Universal_HTML5_Viewer` kopieren.

   Wenn Sie **[!UICONTROL URL kopieren]** auswählen, wird die URL in die Zwischenablage kopiert. Fügen Sie diesen Code in den HTML-Code Ihrer Website, mobilen Site oder Anwendung ein. 

   >[!NOTE]
   >
   >URLs werden erst aktiv, nachdem Sie das Video oder das adaptive Videoset veröffentlicht haben.

* Zeigen Sie das auf der Webseite eingebettete Video an. Verwenden Sie in diesem Fall die Funktion **[!UICONTROL Einbettungscode]** .

   Um den Einbettungscode für ein Video entweder in der Raster- oder Listenansicht zu erhalten, wählen Sie das Video im Bedienfeld „Durchsuchen“ aus. Gehen Sie zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**. Wählen Sie unter der Spalte Aktionen der Tabelle **[!UICONTROL Einbettungscode]** rechts von `Universal_HTML5_Video` aus. Das Bearbeiten des Codes ist nicht zulässig.

   Wählen Sie **[!UICONTROL Close]** und fügen Sie den Einbettungscode in Ihre Webseiten ein.

   >[!NOTE]
   >
   >Der Einbettungscode wird erst aktiv, nachdem Sie das Video oder das adaptive Videoset veröffentlicht haben.

Siehe [Bereitstellen von Videos auf Ihren Websites und mobilen Sites](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Optimale Vorgehensweisen für die Videokodierung](uploading-encoding-videos.md#best_practices_for_video_encoding)

