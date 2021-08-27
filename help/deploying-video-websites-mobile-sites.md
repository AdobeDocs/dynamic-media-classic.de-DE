---
title: Bereitstellen von Videos auf Websites und mobilen Sites
description: Erfahren Sie, wie Sie von Adobe Dynamic Media Classic aus Videos auf Ihren Websites und mobilen Sites bereitstellen.
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '1704'
ht-degree: 35%

---

# Bereitstellen von Videos auf Websites und mobilen Sites{#deploying-video-to-your-websites-and-mobile-sites}

Websites, mobile Sites und Desktop-Anwendungen greifen mithilfe von URL-Zeichenfolgen oder eingebettetem Code auf den Serverinhalt von Adobe Dynamic Media Classic zu, einschließlich Videos. Adobe Dynamic Media Classic aktiviert diese URL-Zeichenfolgen während des Veröffentlichungsvorgangs. Um die URL-Zeichenfolge oder den Einbettungscode für Ihr Video in Ihre Webseiten, mobilen Seiten und Desktop-Applikationen zu platzieren, kopieren Sie ihn aus der Adobe Dynamic Media Classic.

>[!NOTE]
>
>Diese URL bzw. der Einbettungscode wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Veröffentlichen von Videos {#publishing-video}

Durch das Veröffentlichen eines Videos können Adobe Dynamic Media Classic-Server Videos für Ihre Website, mobile Site oder Anwendung bereitstellen.

Es gibt zwei unterschiedliche Methoden zum Veröffentlichen von Video:

* **Videos sofort beim Hochladen automatisch veröffentlichen** - Im Rahmen des Video-Upload-Prozesses kann Adobe Dynamic Media Classic automatisch Videos veröffentlichen, wenn sie hochgeladen und kodiert werden. Durch das sofortige Veröffentlichen entfällt die Anforderung, Video nach dem Hochladen separat zu veröffentlichen.

* **Videos nach dem Hochladen manuell veröffentlichen** - Wenn Sie Videos nach dem Hochladen nicht sofort veröffentlichen möchten, können Sie Videos jederzeit manuell veröffentlichen.

Nach der Veröffentlichung von Videos aktiviert Adobe Dynamic Media Classic die URL-Zeichenfolgen für Ihre HTML-Seite oder Ihren Anwendungscode.

**So Veröffentlichen Sie Video:**

1. Führen Sie einen der folgenden Schritte aus:

   * Um Videos automatisch und sofort beim Hochladen zu veröffentlichen, wählen Sie auf der Seite &quot;Hochladen&quot;die Option **[!UICONTROL Nach dem Hochladen veröffentlichen]** aus. An dieser Stellen ist der Vorgang abgeschlossen, Sie müssen keine weiteren Schritte ausführen.
   * Um Videos nach dem Hochladen manuell zu veröffentlichen, wählen Sie im Durchsuchenbedienfeld die Videos aus und klicken Sie dann in der Symbolleiste für globale Navigation auf **Veröffentlichen**.

## Verknüpfen einer Video-URL mit einer mobilen Site oder Website {#linking-a-video-url-to-a-mobile-site-or-a-website}

Nach dem Veröffentlichen eines Videos können Sie dessen URL abrufen, um sie auf Ihrer Website, mobilen Site oder in Ihrer Anwendung zu verwenden. Verwenden Sie die Video-URL, wenn Videos in einem Popup-Menü oder einem modalen Fenster auf die Webseite angezeigt werden sollen.

Wenn ein Kunde den Link auswählt, werden sein Gerät, die Bandbreite und die Bildschirmgröße automatisch erkannt. Das entsprechende Video wird zur Wiedergabe in einem vordefinierten Viewer für Desktop-PCs oder mit dem systemeigenen Videoplayer für Smartphones und Tablets des Mobilgeräts angezeigt. 

Siehe auch [Einbetten des Video-Viewers auf einer Web-Seite](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**So verknüpfen Sie eine Video-URL mit einer mobilen Site oder Website:**

1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets in der Dropdown-Liste **[!UICONTROL Anzeigen]** die Option **[!UICONTROL Video]** oder **[!UICONTROL Adaptives Videoset]**.
1. Im Bedienfeld „Asset-Bibliothek“ auf der linken Seite navigieren Sie zu dem Asset-Ordner, in dem das Video bzw. das adaptive Videoset enthalten ist, für das Sie eine Verknüpfung erstellen möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** oder **[!UICONTROL Listenansicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf eine Videominiatur, um sie in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld &quot;URLs&quot;und &quot;Einbettungscode&quot;auf der rechten Seite unter &quot;HTTP Streaming&quot;die Option **[!UICONTROL URL]** rechts neben dem gewünschten Viewer kopieren. Kopieren Sie als Best Practice die URL, die mit dem Viewer `Universal_HTML5_Video` verknüpft ist.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL URL kopieren]** aus. Kopieren Sie als Best Practice die URL, die mit dem Viewer `Universal_HTML5_Video` verknüpft ist.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL URL kopieren]** aus. Kopieren Sie als Best Practice die URL, die mit dem Viewer `Universal_HTML5_Video` verknüpft ist.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Navigieren Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL URL kopieren]** aus. Kopieren Sie als Best Practice die URL, die mit dem Viewer `Universal_HTML5_Video` verknüpft ist.

1. Fügen Sie die HTML5 Video-URL auf Ihrer Website und Ihrer mobilen Site ein.

## Einbetten des Video-Viewers auf einer Web-Seite {#embedding-the-video-viewer-on-a-web-page}

Verwenden Sie die Funktion zum Einbetten von Code, wenn Sie das auf Ihrer Website eingebettete Video wiedergeben möchten. Kopieren Sie den Einbettungscode in die Zwischenablage, damit Sie ihn in Ihre Webseiten einfügen können. Die Bearbeitung des Codes ist im Dialogfeld Einbettungscode nicht zulässig.

Siehe auch [Verknüpfen einer Video-URL mit einer mobilen Site oder Website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**So betten Sie den Video-Viewer in einer Webseite ein:**

1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets in der Dropdown-Liste Anzeigen die Option **[!UICONTROL Video]** oder **[!UICONTROL Adaptives Videoset]**.
1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der das Video bzw. das adaptive Videoset enthält, dessen Einbettungscode Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** oder **[!UICONTROL Listenansicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf eine Videominiatur, um sie in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld URLs und Einbettungscode auf der rechten Seite unter HTTP Streaming **[!UICONTROL Einbettungscode]** rechts neben dem gewünschten Viewer aus. Wählen Sie als Best Practice **[!UICONTROL Einbettungscode]** aus, der mit dem Viewer `Universal_HTML5_Video` verknüpft ist.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und klicken Sie dann unter dem Videominiaturbild auf **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL Einbettungscode]** aus. Wählen Sie als Best Practice **[!UICONTROL Einbettungscode]** aus, der mit dem Viewer `Universal_HTML5_Video` verknüpft ist.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL Einbettungscode]** aus. Wählen Sie als Best Practice **[!UICONTROL Einbettungscode]** aus, der mit dem Viewer `Universal_HTML5_Video` verknüpft ist.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Navigieren Sie in derselben Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

      Wählen Sie auf der Seite &quot;Viewer-Liste&quot;unter der Spalte &quot;Aktionen&quot;der Tabelle **[!UICONTROL Einbettungscode]** aus. Wählen Sie als Best Practice **[!UICONTROL Einbettungscode]** aus, der mit dem Viewer `Universal_HTML5_Video` verknüpft ist.

1. Wählen Sie im Dialogfeld &quot;Einbettungscode&quot;die Option **[!UICONTROL In Zwischenablage kopieren]**.

   Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

1. Wählen Sie **[!UICONTROL Close]** aus.
1. Fügen Sie den Einbettungscode in Ihre Webseiten ein.

### Implementieren von Einbettungscode für die Verwendung von HTML5-Videos mit MP4-Video-Assets {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Wenn Sie nicht den Adobe Dynamic Media Classic HTML5-Videoplayer, sondern stattdessen das native HTML5 `<video>`-Tag mit MP4-Video-Assets verwenden möchten, können Sie das folgende Einbettungscode-Beispiel verwenden:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Ersetzen Sie `"S7 video thumbnail URL"` durch die Miniatur-URL des Videos, die das Miniaturbild des Videos darstellt, das ein Benutzer vor der Wiedergabe des Videos sieht.

   Siehe [Abrufen von URLs für Videominiaturen](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Ersetzen Sie `"S7 OGG video asset URL (no player)"` durch die progressive URL des Videos für OGG-Videos.

   Siehe [Verknüpfen einer Video-URL mit einer mobilen Site oder Website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Ersetzen Sie `"S7 MP4 mobile progressive video asset URL (no player)"` durch die progressive mobile URL des Videos.

   Siehe [Verknüpfen einer Video-URL mit einer mobilen Site oder Website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Bereitstellen von Videos mit einem Video-Player eines Drittanbieters {#deploying-video-using-a-third-party-video-player}

Wenn Sie einen Video-Player eines Drittanbieters oder einen benutzerdefinierten Video-Player anstelle eines Video-Viewers der Adobe Dynamic Media Classic verwenden, erhalten Sie die direkte Video-URL, die für HLS-Video-Streaming mit mehreren Bitraten oder progressiven Download funktioniert.

**So stellen Sie ein Video mit einem Video-Player eines Drittanbieters bereit:**

1. Navigieren Sie in Adobe Dynamic Media Classic auf der Symbolleiste für globale Navigation zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Einstellungen]**.
1. Abhängig vom URL-Typ, die Sie verwenden möchten, führen Sie einen der folgenden Schritte aus:

* So generieren Sie eine direkte HLS-Streaming-Video-URL (Multi-Bitrate)

   Erstellen Sie auf der Seite **[!UICONTROL Application General Settings]** in der Gruppe **[!UICONTROL Servers]** im Textfeld **[!UICONTROL Veröffentlichter Servername]** die direkte URL. Verwenden Sie die folgende Syntax: `server/is/content/company/folder/filename.m3u8`

   Angenommen, der Name des veröffentlichten Servers ist `https://s7d9.scene7.com/.` Die direkte URL könnte unter Verwendung der Syntax in Schritt 2 wie folgt aussehen:
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* So generieren Sie eine direkte HLS-Streaming-Video-URL (Einzelbit-Rate)

   Erstellen Sie auf der Seite **[!UICONTROL Application General Settings]** in der Gruppe **[!UICONTROL Servers]** im Textfeld **[!UICONTROL HLS Streaming Server Name]** die direkte URL unter Verwendung der folgenden Syntax:

   `server/company/folder/filename.ext.m3u8`

   Angenommen, der Name des HLS-Streaming-Servers ist `https://s7mbrstream.scene7.com/hls-vod/`. Unter Verwendung der Syntax in Schritt 2 könnte die direkte URL wie folgt aussehen:
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* So generieren Sie eine direkte URL für ein progressives Video

   Erstellen Sie auf der Seite **[!UICONTROL Allgemeine Programmeinstellungen]** in der Gruppe **[!UICONTROL Server]** im Textfeld **[!UICONTROL Servername für progressives Video]** die direkte URL für das eVideo unter Verwendung der folgenden Syntax:

   `server/company/folder/filename`

   Angenommen, der progressive Video-Server-Name ist `https://s7d9.scene7.com/is/content/`. Unter Verwendung der Syntax in Schritt 2 könnte die direkte URL wie folgt aussehen:
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Arbeiten mit Videominiaturen {#working-with-video-thumbnails}

Adobe Dynamic Media Classic generiert Miniaturansichten für kodierte Videos und vorkodierte Videos. Videominiaturen können wie alle anderen Bild-Assets verwendet werden. Darüber hinaus können Sie URLs für die Videominiaturen abrufen, die von Adobe Dynamic Media Classic generiert werden, und diese URLs außerhalb von Adobe Dynamic Media Classic bereitstellen. Beispielsweise können Sie die Miniaturansichten in Suchergebnissen, relevanten Videolisten und Videowiedergabelisten auf einer Website bereitstellen.

Miniaturansichten werden basierend auf dem ersten heterogenen Frame (d. h. kein vollständig schwarzer oder vollständig weißer Frame usw.) des Videos generiert.

### Abrufen von URLs für Videominiaturen {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classic generiert während des Upload-Prozesses automatisch Videominiaturen. Die Miniaturansichten werden im Bedienfeld &quot;Durchsuchen&quot;in der Listen- und Rasteransicht angezeigt.

Führen Sie zum Erstellen von URLs für Videominiaturen einen Veröffentlichungsvorgang durch.

Siehe [Video veröffentlichen](deploying-video-websites-mobile-sites.md#publishing_video).

Nach der Veröffentlichung können Sie Videominiatur-URLs in der Detailansicht im URL-Bedienfeld sowie im Code-einbetten-Bedienfeld abrufen. Wählen Sie **[!UICONTROL URL]** rechts neben der Videominiatur kopieren aus, um die URL zu kopieren.

### Ändern von Standbildern in Video-Viewern {#modifying-poster-frames-in-video-viewers}

Das *Standbild* ist das erste Bild, das in Video-Viewern angezeigt wird, bevor die Wiedergabe beginnt. Adobe Dynamic Media Classic verwendet Videominiaturen als Posterrahmen.

Sie können auch Bildmodifikatoren auf das Standbild anwenden. Sie können das Standbild beispielsweise beschneiden oder transparent machen. Öffnen Sie zum Bearbeiten des Standbilds den Anzeigebereich „Konfiguration“ des Video-Viewers und geben Sie unter „Standbildmodifikatoren“ Modifikatoren ein. 

Siehe [Hinzufügen oder Bearbeiten einer Video-Viewer-Vorgabe](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Siehe [Image Serving Guide](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home.html?lang=en#image-serving-api).

Sie können auch Videominiaturen bearbeiten, indem Sie Modifikatoren an die Videominiatur-URLs anhängen.

>[!MORELIKETHIS]
>
>* [Veröffentlichen von Dateien](publishing-files.md#publishing_files)