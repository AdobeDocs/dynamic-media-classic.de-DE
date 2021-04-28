---
title: '"Kurzanleitung: Video"'
description: Eine Einführung und ein kurzer Beginn zur Adobe von Dynamic Media Classic Video, mit dem Sie schnell und einfach loslegen können.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic, Viewer, Video
role: Business Practitioner
exl-id: 1157400c-b33a-422e-848c-258660ddc748
translation-type: tm+mt
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '1425'
ht-degree: 43%

---

# Kurzanleitung: Video{#quick-start-video}

Adobe Dynamic Media Classic Video ist eine Komplettlösung, mit der Sie hochwertige adaptive Videos für das Streaming auf verschiedenen Anzeigemedien wie Desktop, iOS, Android™, BlackBerry® und Windows® mühelos veröffentlichen können. Bei adaptiven Videosets werden Versionen desselben Videos gruppiert, die in unterschiedlichen Bitraten und Formaten kodiert sind, z. B. mit 400 Kbit/s, 800 Kbit/s und 1000 Kbit/s. Der Desktop-Computer oder das Mobilgerät erkennt die verfügbare Bandbreite.

Zum Beispiel werden auf einem iOS-Mobilgerät Bandbreiten wie 3G, 4G oder Wi-Fi erkannt. Anschließend wird unter den verschiedenen Video-Bitraten innerhalb des adaptiven Videosets automatisch das richtig kodierte Video ausgewählt. Das Video wird auf Desktops, Mobilgeräte und Tablets gestreamt.

Außerdem wird die Videoqualität automatisch angepasst, wenn sich die Netzwerkbedingungen des Desktop- oder Mobilgeräts ändern. Wenn ein Kunde auf einem Desktop in den Vollbildmodus wechselt, reagiert das adaptive Video-Set mit einer besseren Auflösung, wodurch die Anzeige des Kunden verbessert wird. Mit adaptiven Video-Sets erhalten Sie die bestmögliche Wiedergabe von Dynamic Media Classic-Videos auf mehreren Bildschirmen und Geräten.

Die Logik, die ein Video-Player verwendet, um das richtige kodierte Video für die Wiedergabe auszuwählen, basiert auf dem folgenden Algorithmus:

1. Der Videoplayer lädt das anfängliche Videofragment basierend auf der Bitrate, die dem Wert am nächsten kommt, der für &quot;initiale Bitrate&quot;im Player selbst festgelegt wurde.
1. Video-Player-Switches basierend auf Änderungen der Bandbreitengeschwindigkeit unter Verwendung der folgenden Kriterien:

   1. Der Player wählt den Stream mit der höchsten Bandbreite unterhalb oder gleich der geschätzten Bandbreite aus.
   1. Der Player berücksichtigt nur 80 % der verfügbaren Bandbreite. Wenn sie jedoch nach oben wechselt, ist sie bei nur 70 % konservativer, um Überschätzungen zu vermeiden und sofort zurückzuschalten.

Technische Informationen dazu finden Sie in der Logik des Algorithmus unter [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp).

Für die Verwaltung von einzelnen Videos und adaptiven Videosets unterstützt Dynamic Media Classic Folgendes:

* Das Hochladen von Video aus verschiedenen unterstützten Videoformaten und Audioformaten und das Kodieren von Video im MP4 H.264-Format für die Wiedergabe auf verschiedenen Anzeigemedien. Sie können vordefinierte adaptive Video-Vorgaben für Dynamic Media Classic oder einzelne Videokodierungsvorgaben verwenden oder Ihre eigene Kodierung anpassen, um Qualität und Größe des Videos zu steuern.

   Wenn ein adaptives Videoset generiert wird, enthält es MP4-Videos.

   `**Note:**` Übergeordnet-/Quellvideos und andere Quellvideoformate werden keinem adaptiven Videoset  ** hinzugefügt.

* Videountertitel in den Viewern Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark und Universal_HTML5_MixedMedia_light sowie Videokapitelnavigation in den Viewern Univeral_HTML5_Video, Universal_HTML5_MixedMedia_dark und Universal_HTML5_MixedMedia_light.

   Siehe [Hinzufügen von Untertiteln zu Video](adding-captions-video.md).

   Siehe [Hinzufügen von Kapitelmarken zu Video](adding-chapter-markers-video.md).

* Organisieren, Durchsuchen und Suchen von Videos mit vollständiger Metadatenunterstützung für eine effiziente Verwaltung von Video-Assets.
* Stellen Sie adaptive Video-Sets für das Web, Desktop-PCs und Mobilgeräte bereit, einschließlich iPhone, iPad, Android™, BlackBerry® und Windows® Phone.

   Das adaptive Video-Streaming wird auf verschiedenen iOS-Plattformen unterstützt.

   Weitere Informationen finden Sie im [Adobe Viewer-Referenzhandbuch](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

   Dynamic Media Classic unterstützt die Wiedergabe von mobilen Videos für MP4 H.264-Videos. BlackBerry®-Geräte, die dieses Videoformat unterstützen, finden Sie auf folgender Website:

   Siehe [Unterstützte Videoformate auf BlackBerry®](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   Windows®-Geräte, die dieses Videoformat unterstützen, finden Sie unter:

   Siehe [Unterstützte Videoformate unter Windows® Phone](https://docs.microsoft.com/en-us/).

* Wiedergabe des Videos mit Dynamic Media Classic Viewer-Vorgaben, einschließlich der folgenden:

   * Einzel-Video-Viewer
   * Viewer für gemischte Medien, die Video- und Bildinhalte kombinieren

* Konfigurieren von Video-Playern für individuelle Branding-Anforderungen
* Integrieren von Videos in Websites, mobile Sites oder mobile Anwendungen über eine einfache URL oder einen eingebetteten Code.

**Quick Beginn**

Die folgende Workflow-Beschreibung hilft Ihnen, sich schnell mit adaptiven Videosets in Dynamic Media Classic vertraut zu machen. Nach jedem Schritt wird auf ein Thema mit weiteren Informationen verwiesen.

## 1. Hochladen und Kodieren von Videos

Generieren und laden Sie adaptive Videosets mithilfe eines der beiden folgenden Szenarien hoch:

* **Hochladen vorkodierter Videos** : Wenn Ihre Videos bereits außerhalb von Dynamic Media Classic kodiert wurden, klicken Sie in der Symbolleiste für globale Navigation auf &quot; **** Hochladen&quot;, um die MP4-Videodateien direkt nach Dynamic Media Classic zu suchen und hochzuladen. Klicken Sie dann auf **[!UICONTROL Erstellen]** > **[!UICONTROL Adaptive Videosets]**. Navigieren Sie zu Ihren Videodateien. Fügen Sie die gewünschten Videodateien per Drag &amp; Drop in die Tabelle für adaptive Videosets ein und speichern Sie das Set.
* **Übergeordnet Quellvideos**  hochladen: Wenn Ihre Videos nicht kodiert sind, klicken Sie in der Symbolleiste für globale Navigation auf &quot; **** Hochladen&quot;, um Übergeordnet-Videoquelldateien (nicht MP4) hochzuladen und Dynamic Media Classic diese in MP4-Dateien kodieren zu lassen. Wählen Sie im Dialogfeld **[!UICONTROL Upload-Auftragsoptionen]** unter **[!UICONTROL eVideo-Optionen]** **[!UICONTROL Adaptives Video]**.

   Mit dieser bevorzugten Option können Sie ein adaptives Videoset erstellen, das automatisch die korrekte Kodierungsvorgabe (16:9 oder 4:3) entsprechend den Abmessungen des hochgeladenen Videos anpasst. Wenn Sie den Hochladeauftrag senden, wird automatisch ein adaptives Videoset erstellt, das drei Videokodierungen im korrekten Seitenverhältnis enthält.

   Oder erweitern Sie im selben Dialogfeld **[!UICONTROL Auftragsoptionen]** unter **[!UICONTROL eVideo-Optionen]** **[!UICONTROL Einzelne Kodierungsvorgaben]**. Wählen Sie die gewünschten individuellen Videokodierungsvorgaben von **Desktop**, **Mobil (iPhone, iPad, Android™)** und **Tablet (iPad, Android™)** aus, um die MP4-Dateien zu erstellen.

* Oder Sie können ein Übergeordnet Video mit der Funktion **[!UICONTROL Neu verarbeiten]** erneut verarbeiten. Die neu kodierten Videos werden dem vorhandenen adaptiven Videoset hinzugefügt.

Siehe [Hochladen und Kodieren von Video](uploading-encoding-videos.md#uploading_and_encoding_videos).

**Optional**

Dynamic Media Classic-Angebote verfügen über zahlreiche vordefinierte Videokodierungsvorgaben. Diese vordefinierten Vorgaben spiegeln die am häufigsten verwendeten Videokodierungseinstellungen wider und sind für die Wiedergabe auf Zielgruppen optimiert.

Außerdem können Administratoren, wenn eine weitere Anpassung erforderlich ist, Video-Vorgaben erstellen, um die Größe und Wiedergabe von eVideo für Endbenutzer anzupassen. Administratoren können auf der Seite &quot;Video-Vorgaben&quot;unter **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Video-Vorgaben]** > **[!UICONTROL Einzelne Kodierungsvorgaben]** Video-Vorgaben hinzufügen und verwalten. Auf der Seite „Video-Vorgaben“ finden Sie Optionen, um Video-Vorgaben hinzuzufügen, zu bearbeiten, zu löschen und zu aktivieren. 

Siehe [Arbeiten mit Videokodierungsvorgaben](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2. Anzeigen einer Vorschau von Videos in einem Video-Viewer

Um zu überprüfen, wie die Video-Ausgabe für Endbenutzer auf einem Desktop-PC, Ihrer Website bzw. dem mobilen Gerät aussieht, wählen Sie das Video im Bedienfeld „Durchsuchen“ aus und klicken Sie dann auf **[!UICONTROL Vorschau]**. 

Siehe [Anzeigen einer Vorschau von Videos in einem Video-Viewer](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

Sie können das Video auf der Seite &quot;Vorschau&quot;abspielen. Sie können auch verschiedene Video-Viewer auswählen, um herauszufinden, wie Ihr Video in verschiedenen Playern angezeigt wird. Wir empfehlen, dass Sie den HTML5 Video-Player für die Wiedergabe auf verschiedenen Anzeigegeräten wie Desktop, Tablet und Mobilgeräte verwenden.

**optional**

Anpassung der Viewer-Vorgaben - Vordefinierte Viewer-Vorgaben für Dynamic Media Classic-Angebot für die Bereitstellung von Videos Diese Vorgaben bestimmen das Aussehen des Viewers und die Funktionsweise der Wiedergabe-Steuerelemente. Zum Anpassen des Video-Viewers können Administratoren die Viewer-Vorgaben über die Seite „Viewer-Vorgaben“ hinzufügen und verwalten. Um diese Seite zu öffnen, klicken Sie oben rechts in Dynamic Media Classic auf **[!UICONTROL Setup]** > **[!UICONTROL Viewer-Vorgaben]**. Auf der Seite „Viewer-Vorgaben“ finden Sie Befehle, um Viewer-Vorgaben hinzuzufügen, zu bearbeiten, zu löschen und zu aktivieren. 

Siehe [Arbeiten mit Video-Viewer-Vorgaben](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

## 3. Bereitstellen von Videos auf Ihren Websites und mobilen Sites

Führen Sie einen der folgenden Schritte aus, um Video in Ihre Website zu integrieren:

* Zeigen Sie das Video in einem eigenen Popup- oder modalen Fenster an. Verwenden Sie in diesem Fall die Funktion **[!UICONTROL URL kopieren]**.

   Um eine URL für ein Video entweder in der Raster- oder Listenansicht zu erhalten, wählen Sie das Video im Bedienfeld „Durchsuchen“ aus. Klicken Sie auf **[!UICONTROL Vorschau]** und dann auf **[!UICONTROL URL kopieren]** rechts neben `Universal_HTML5_Viewer`.

   Wenn Sie auf **[!UICONTROL URL kopieren]** klicken, wird die URL in die Zwischenablage kopiert. Fügen Sie diesen Code in den HTML-Code Ihrer Website, mobilen Site oder Anwendung ein. 

   >[!NOTE]
   >
   >URLs werden erst aktiv, nachdem Sie das Video oder das adaptive Videoset veröffentlicht haben.

* Zeigen Sie das auf der Webseite eingebettete Video an. Verwenden Sie in diesem Fall die Funktion **[!UICONTROL Code einbetten]**.

   Um den Einbettungscode für ein Video entweder in der Raster- oder Listenansicht zu erhalten, wählen Sie das Video im Bedienfeld „Durchsuchen“ aus. Klicken Sie auf **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**. Klicken Sie in der Spalte Aktionen der Tabelle rechts neben `Universal_HTML5_Video` auf **[!UICONTROL Code einbetten]**. Das Bearbeiten des Codes ist nicht zulässig.

   Klicken Sie auf **[!UICONTROL Schließen]** und fügen Sie den Einbettungscode in Ihre Webseiten ein.

   >[!NOTE]
   >
   >Der Einbettungscode wird erst aktiv, nachdem Sie das Video oder das adaptive Videoset veröffentlicht haben.

Siehe [Bereitstellen von Videos auf Websites und mobilen Sites](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [Optimale Vorgehensweisen für die Videokodierung](uploading-encoding-videos.md#best_practices_for_video_encoding)

