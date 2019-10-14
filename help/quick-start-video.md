---
title: '"Kurzanleitung: Video"'
seo-title: '"Kurzanleitung: Video"'
description: 'null'
seo-description: Eine Einführung und eine Kurzanleitung zu Videos, die Ihnen helfen, sich schnell aufzumachen.
uuid: bf0ecf87-a1f2-4e83-8041-df5192dd26a1
contentOwner: admin
content-type: Verweis
products: SG_EXPERIENCEMANAGER/Dynamic Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 6cef541b-e9df-48eb-9a16-ca3e1f07238e
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Kurzanleitung: Video{#quick-start-video}

Adobe Dynamic Media Classic Video ist eine End-to-End-Lösung, mit der Sie hochwertige adaptive Videos für das Streaming auf verschiedenen Anzeigemedien wie Desktop, iOS, Android, Blackberry und Windows veröffentlichen können. Bei adaptiven Videosets werden Versionen desselben Videos gruppiert, die in unterschiedlichen Bitraten und Formaten kodiert sind, z. B. mit 400 Kbit/s, 800 Kbit/s und 1000 Kbit/s. Der Desktop-Computer oder das Mobilgerät erkennt die verfügbare Bandbreite.

Zum Beispiel werden auf einem iOS-Mobilgerät Bandbreiten wie 3G, 4G oder Wi-Fi erkannt. Anschließend wird unter den verschiedenen Video-Bitraten innerhalb des adaptiven Videosets automatisch das richtig kodierte Video ausgewählt. Das Video wird auf Desktops, Mobilgeräte und Tablets gestreamt.

Außerdem wird die Videoqualität automatisch angepasst, wenn sich die Netzwerkbedingungen des Desktop- oder Mobilgeräts ändern. Das adaptive Videoset reagiert auch, wenn der Vollbildmodus auf einem Desktop geöffnet wird. Es verwendet dann eine höhere Auflösung und verbessert so das Seherlebnis des Kunden. Mit adaptiven Video-Sets erhalten Sie die bestmögliche Wiedergabe von Videos, die von Kunden auf mehreren Bildschirmen und Geräten wiedergegeben werden.

Die Logik, die ein Video-Player verwendet, um das richtige kodierte Video für die Wiedergabe auszuwählen, basiert auf dem folgenden Algorithmus:

1. Der Videoplayer lädt das anfängliche Videofragment basierend auf der Bitrate, die dem für "initiale Bitrate"festgelegten Wert im Player am nächsten kommt.
1. Video-Player-Switches basierend auf Änderungen der Bandbreitengeschwindigkeit unter Verwendung der folgenden Kriterien:

   1. Der Player wählt den Stream mit der höchsten Bandbreite unterhalb oder gleich der geschätzten Bandbreite aus.
   1. Der Player berücksichtigt nur 80 % der verfügbaren Bandbreite. Wenn es jedoch nach oben wechselt, ist es bei nur 70 % umstrittener, Überschätzungen zu vermeiden und sofort zurückzuschalten.

Technische Informationen dazu finden Sie in der Logik des Algorithmus unter [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) .

Für die Verwaltung von einzelnen Videos und adaptiven Videosets unterstützt Dynamic Media Classic Folgendes:

* Das Hochladen von Video aus verschiedenen unterstützten Videoformaten und Audioformaten und das Kodieren von Video im MP4 H.264-Format für die Wiedergabe auf verschiedenen Anzeigemedien. Sie können vordefinierte Vorgaben für adaptive Video-Vorgaben für Dynamic Media Classic oder einzelne Videokodierungsvorgaben verwenden oder Ihre eigene Kodierung anpassen, um Qualität und Größe des Videos zu steuern.

   Wenn ein adaptives Videoset generiert wird, enthält es MP4-Videos.

   `**Note:**` Master-/Quellvideos und andere Quellvideoformate werden *keinem adaptiven Videoset hinzugefügt* .

* Videountertitel in den Viewern Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark und Universal_HTML5_MixedMedia_light sowie Videokapitelnavigation in den Viewern Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark und Universal_HTML5_MixedMedia_light.

   Siehe [Hinzufügen von Untertiteln zu Video](adding-captions-video.md).

   Siehe [Hinzufügen von Kapitelmarken zu Video](adding-chapter-markers-video.md).

* Organisieren, Durchsuchen und Suchen von Videos mit vollständiger Metadatenunterstützung für eine effiziente Verwaltung von Video-Assets.
* Stellen Sie adaptive Videosets für Websites, Desktop-PCs und Mobilgeräte zur Verfügung, einschließlich iPhone, iPad, Android™, Blackberry und Windows Phone.

   Das adaptive Video-Streaming wird auf zahlreichen iOS-Plattformen unterstützt.

   Weitere Informationen finden Sie unter der neuesten Unterstützung im [Adobe Viewer-Referenzhandbuch](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/).

   Dynamic Media Classic unterstützt die Wiedergabe von mobilen Videos für MP4 H.264-Videos. Blackberry-Geräte, die dieses Videoformat unterstützen, finden Sie auf der folgenden Website:

   Siehe [Unterstützte Videoformate in Blackberry](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   Windows-Geräte, die dieses Videoformat unterstützen, finden Sie hier:

   Siehe [Unterstützte Videoformate auf Windows Phone](https://msdn.microsoft.com/en-us/library/ff462087(v=vs.92).aspx).

* Wiedergabe des Videos mithilfe von Viewer-Vorgaben für dynamische Medien - Classic, einschließlich der folgenden:

   * Einzel-Video-Viewer
   * Viewer für gemischte Medien, die Video- und Bildinhalte kombinieren

* Konfigurieren von Video-Playern für individuelle Branding-Anforderungen
* Integrieren von Videos in Websites, mobile Sites oder mobile Anwendungen über eine einfache URL oder einen eingebetteten Code.

**Schnellstart**

Die folgende Workflow-Beschreibung hilft Ihnen, sich schnell mit adaptiven Videosets in Dynamic Media Classic vertraut zu machen. Nach jedem Schritt wird auf ein Thema mit weiteren Informationen verwiesen.

**1. Hochladen und Kodieren von Video**

Generieren und laden Sie adaptive Videosets mithilfe eines der beiden folgenden Szenarien hoch:

* **Hochladen vorkodierter Videos** Wenn Ihre Videos bereits außerhalb von Dynamic Media Classic kodiert wurden, klicken Sie in der Symbolleiste für globale Navigation auf " **Hochladen** ", um nach MP4-Videodateien zu suchen und sie direkt in das Scene7 Publishing System hochzuladen. Klicken Sie dann auf **Erstellen &gt; Adaptive Videosets**. Navigieren Sie zu Ihren Videodateien. Fügen Sie die gewünschten Videodateien per Drag &amp; Drop in die Tabelle für adaptive Videosets ein und speichern Sie das Set.
* **Hochladen von Master-Quellvideos** Wenn Ihre Videos nicht kodiert sind, klicken Sie in der Symbolleiste für globale Navigation auf " **Hochladen** ", um Master-Videoquelldateien (nicht MP4) hochzuladen und diese vom Scene7 Publishing System in MP4-Dateien kodieren zu lassen. Wählen Sie im Dialogfeld „Upload-Auftragsoptionen“ unter den eVideo-Optionen die Option **Adaptive Video**.

   Mit dieser bevorzugten Option können Sie ein adaptives Videoset erstellen, das automatisch die korrekte Kodierungsvorgabe (16:9 oder 4:3) entsprechend den Abmessungen des hochgeladenen Videos anpasst. Wenn Sie den Hochladeauftrag senden, wird automatisch ein adaptives Videoset erstellt, das drei Videokodierungen im korrekten Seitenverhältnis enthält.

   Alternativ können Sie im gleichen Dialogfeld „Auftragsoptionen“ unter den eVideo-Optionen die Option **Einzelne Kodierungsvorgaben** erweitern und einzelne Videokodierungsvorgaben in den Bereichen **Desktop**, **Mobil (iPhone, iPad, Android)** und **Tablet (iPad, Android)** auswählen, um die MP4-Dateien zu erstellen.

* Darüber hinaus besteht die Möglichkeit, ein Master-Video mithilfe der Funktion „Neu verarbeiten“ neu zu verarbeiten. Die neu kodierten Videos werden dem vorhandenen adaptiven Videoset hinzugefügt.

Siehe [Hochladen und Kodieren von Video](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Optional**

Dynamic Media Classic bietet zahlreiche vordefinierte Videokodierungsvorgaben. Diese vordefinierten Vorgaben decken die heutzutage am häufigsten verwendeten Videokodierungseinstellungen ab und wurden für die Wiedergabe auf den jeweiligen Zieldisplays optimiert.

Außerdem können Administratoren, wenn eine weitere Anpassung erforderlich ist, Video-Vorgaben erstellen, um die Größe und Wiedergabe von eVideo für Endbenutzer anzupassen. Administratoren können Video-Vorgaben über die Seite „Video-Vorgaben“ hinzufügen und verwalten. Zum Öffnen dieser Seite klicken Sie auf „Einstellungen“ &gt; „Anwendungseinstellungen“ &gt; „Video-Vorgaben“ &gt; „Einzelne Kodierungsvorgaben“. Auf der Seite „Video-Vorgaben“ finden Sie Optionen, um Video-Vorgaben hinzuzufügen, zu bearbeiten, zu löschen und zu aktivieren. 

Siehe [Arbeiten mit Videokodierungsvorgaben](uploading-encoding-videos.md#working_with_video_encoding_presets).

**2. Anzeigen einer Vorschau von Videos in einem Video-Viewer**

Um zu überprüfen, wie die Video-Ausgabe für Endbenutzer auf einem Desktop-PC, Ihrer Website bzw. dem mobilen Gerät aussieht, wählen Sie das Video im Bedienfeld „Durchsuchen“ aus und klicken Sie dann auf **Vorschau**. 

Siehe [Anzeigen einer Vorschau von Videos in einem Video-Viewer](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Sie können das Video im Anzeigebereich „Vorschau“ wiedergeben. Sie können auch verschiedene Video-Viewer auswählen, um auszuprobieren, wie das Video in den verschiedenen Playern dargestellt wird. Wir empfehlen, dass Sie den HTML5 Video-Player für die Wiedergabe auf verschiedenen Anzeigegeräten wie Desktop, Tablet und Mobilgeräte verwenden.

**Optional**

Anpassung von Viewer-Vorgaben - Dynamic Media Classic bietet vordefinierte Viewer-Vorgaben für die Bereitstellung von Videos. Diese Vorgaben bestimmen das Aussehen des Viewers und die Funktionsweise der Wiedergabe-Steuerelemente. Zum Anpassen des Video-Viewers können Administratoren die Viewer-Vorgaben über die Seite „Viewer-Vorgaben“ hinzufügen und verwalten. Um diese Seite zu öffnen, klicken Sie in rechts oben in Scene7 auf „Einstellungen“ &gt; „Video-Vorgaben“. Auf der Seite „Viewer-Vorgaben“ finden Sie Befehle, um Viewer-Vorgaben hinzuzufügen, zu bearbeiten, zu löschen und zu aktivieren. 

Siehe [Arbeiten mit Video-Viewer-Vorgaben](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

**3. Bereitstellen von Videos auf Websites und mobilen Sites**

Führen Sie einen der folgenden Schritte aus, um Video in Ihre Website zu integrieren:

* Zeigen Sie das Video in einem eigenen Popup- oder Modalfenster an; in diesem Fall sollten Sie die Funktion „URL kopieren“ verwenden.

   Um eine URL für ein Video entweder in der Raster- oder Listenansicht zu erhalten, wählen Sie das Video im Bedienfeld „Durchsuchen“ aus. Click Preview, and then click Copy URL to the right of `Universal_HTML5_Viewer`.

   Wenn Sie auf die Schaltfläche „URL kopieren“ klicken, wird die URL in die Zwischenablage kopiert. Fügen Sie diesen Code in den HTML-Code Ihrer Website, mobilen Site oder Anwendung ein. 

   >[!NOTE]
   >
   >URLs werden erst aktiv, nachdem Sie das Video oder das adaptive Videoset veröffentlicht haben.

* Zeigen Sie das in die Webseite eingebettete Video an. Verwenden Sie dazu die Funktion zum Einbetten von Code.

   Um den Einbettungscode für ein Video entweder in der Raster- oder Listenansicht zu erhalten, wählen Sie das Video im Bedienfeld „Durchsuchen“ aus. Klicken Sie auf „Vorschau“ &gt; „Viewer-Liste“ Klicken Sie unter der Spalte „Aktionen“ der Tabelle auf „Code einbetten“ rechts neben `Universal_HTML5_Video`. Das Bearbeiten des Codes ist nicht zulässig.

   Klicken Sie auf „Schließen“ und fügen Sie den Einbettungscode in Ihre Webseiten ein.

   >[!NOTE]
   >
   >Der Einbettungscode wird erst aktiv, nachdem Sie das Video oder das adaptive Videoset veröffentlicht haben.

Siehe [Bereitstellen von Videos auf Websites und mobilen Sites](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Optimale Vorgehensweisen für die Videokodierung](uploading-encoding-videos.md#best_practices_for_video_encoding)

