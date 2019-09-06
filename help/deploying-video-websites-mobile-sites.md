---
title: Bereitstellen von Video auf Websites und mobilen Sites
seo-title: Bereitstellen von Video auf Websites und mobilen Sites
description: 'null'
seo-description: Erfahren Sie, wie Sie Videos auf Ihren Websites und mobilen Sites bereitstellen.
uuid: 22 bb 4402-c 0 ab -4 df 0-89 b 9-99707 d 111927
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/video
discoiquuid: 0 d 006314-c 4 cc -4 f 6 c-a 51 c -6075 bb 445 e 39
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Bereitstellen von Video auf Websites und mobilen Sites{#deploying-video-to-your-websites-and-mobile-sites}

Websites, mobile Sites und Desktopanwendungen greifen mithilfe von URL-Zeichenfolgen oder eingebettetem Code auf Dynamic Media Classic-Serverinhalte, einschließlich Videos, zu. Dynamic Media Classic aktiviert diese URL-Zeichenfolgen während des Veröffentlichungsvorgangs. Um die URL-Zeichenfolge oder den Einbettungscode für Ihr Video in Ihre Webseiten, mobilen Seiten und Desktop-Anwendungen einfügen zu können, kopieren Sie sie/ihn in Scene7 Publishing System.

>[!NOTE]
>
>Diese URL bzw. der Einbettungscode wird erst dann aktiv, wenn Sie das Asset veröffentlichen.

## Veröffentlichen von Videos {#publishing-video}

Durch das Veröffentlichen eines Videos können dynamische Media Classic-Server bereitgestellt werden, um Videos auf Ihrer Website, mobilen Site oder in Ihrer Anwendung bereitzustellen.

Es gibt zwei unterschiedliche Methoden zum Veröffentlichen von Video:

* **Videos sofort beim Hochladen automatisch veröffentlichen**

   Während des Hochladevorgangs von Videos kann Dynamic Media Classic Videos automatisch veröffentlichen, wenn sie hochgeladen und kodiert werden. Durch das sofortige Veröffentlichen entfällt die Anforderung, Video nach dem Hochladen separat zu veröffentlichen.

* **Videos nach dem Hochladen manuell veröffentlichen**

   Wenn Sie Videos nach dem Hochladen nicht sofort veröffentlichen möchten, können Sie Videos jederzeit manuell veröffentlichen.

Nach der Veröffentlichung von Videos aktiviert das Scene7 Publishing System die URL-Zeichenfolgen, die Sie im HTML-Code der Site bzw. Anwendung verwenden können.

**So Veröffentlichen Sie Video**

1. Führen Sie einen der folgenden Schritte aus:

   * Um Videos sofort nach dem Hochladen automatisch zu veröffentlichen, klicken Sie im Fenster „Hochladen“ auf **Nach dem Hochladen veröffentlichen**. An dieser Stellen ist der Vorgang abgeschlossen, Sie müssen keine weiteren Schritte ausführen.
   * Um Videos nach dem Hochladen manuell zu veröffentlichen, wählen Sie die entsprechenden Videos im Bedienfeld „Durchsuchen“ aus und klicken dann auf der globalen Navigationsleiste auf **Veröffentlichen**.

## Verknüpfen einer Video-URL mit einer mobilen Site oder Website {#linking-a-video-url-to-a-mobile-site-or-a-website}

Nach dem Veröffentlichen eines Videos können Sie dessen URL abrufen, um sie auf Ihrer Website, mobilen Site oder in Ihrer Anwendung zu verwenden. Verwenden Sie die Video-URL, wenn Videos in einem Popup-Menü oder einem modalen Fenster auf die Webseite angezeigt werden sollen.

Wenn ein Besucher auf den Link klickt, wird das Gerät, die Bandbreite oder die Bildschirmgröße automatisch erkannt. Das entsprechende Video wird zur Wiedergabe in einem vordefinierten Viewer für Desktop-PCs oder mit dem systemeigenen Videoplayer für Smartphones und Tablets des Mobilgeräts angezeigt. 

Siehe auch [Einbetten des Video-Viewers auf einer Webseite](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**So verknüpfen Sie eine Video-URL mit einer mobilen Site oder Website**

1. Klicken Sie im Bedienfeld zum Durchsuchen von Assets in der Dropdown-Liste auf **Video** oder **Adaptives Video-Set**.
1. Im Bedienfeld „Asset-Bibliothek“ auf der linken Seite navigieren Sie zu dem Asset-Ordner, in dem das Video bzw. das adaptive Videoset enthalten ist, für das Sie eine Verknüpfung erstellen möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Klicken Sie auf „**Rasteransicht**“ oder „**Listenansicht**“. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf eine Videominiatur, um sie in der Detailansicht zu öffnen. In dem Bedienfeld für URLs und Einbettungscode auf der rechten Seite klicken Sie unter „HTTP Streaming“ auf **URL kopieren** rechts neben dem gewünschten Viewer. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.
   * Klicken Sie auf „**Rasteransicht**“. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und klicken Sie anschließend unterhalb des Miniaturbilds auf „**Vorschau**“ &gt; „**Viewer-Liste**“.

      Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**URL kopieren**“. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

   * Klicken Sie auf „**Listenansicht**“. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und klicken Sie dann rechts neben dem Miniaturbild auf „**Vorschau**“ &gt; „**Viewer-Liste**“.

      Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**URL kopieren**“. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

   * Klicken Sie auf „**Rasteransicht**“, „**Listenansicht**“ oder „**Detailansicht**“. Klicken Sie in der gleichen Symbolleiste auf „**Vorschau**“ &gt; „**Viewer-Liste**“.

      Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**URL kopieren**“. As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

1. Fügen Sie die HTML5 Video-URL auf Ihrer Website und Ihrer mobilen Site ein.

## Einbetten des Video-Viewers auf einer Webseite {#embedding-the-video-viewer-on-a-web-page}

Verwenden Sie die Funktion zum Einbetten von Code, wenn Sie das auf Ihrer Website eingebettete Video wiedergeben möchten. Sie können den Einbettungscode auch in die Zwischenablage kopieren, um ihn von dort in Webseiten einfügen zu können. Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

Siehe auch [ Verknüpfen einer Video-URL mit einer mobilen Site oder Website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**So betten Sie den Video-Viewer in einer Webseite ein**

1. Klicken Sie im Bedienfeld zum Durchsuchen von Assets in der Dropdown-Liste auf **Video** oder **Adaptives Videoset**.
1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der das Video bzw. das adaptive Videoset enthält, dessen Einbettungscode Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Klicken Sie auf „**Rasteransicht**“ oder „**Listenansicht**“. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf eine Videominiatur, um sie in der Detailansicht zu öffnen. Klicken Sie im Bedienfeld für die URLs und den Einbettungscode auf der rechten Seite unter „HTTP Streaming“ auf **Code einbetten** rechts neben dem gewünschten Viewer. As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.
   * Klicken Sie auf „**Rasteransicht**“. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und klicken Sie anschließend unterhalb des Videominiaturbilds auf **Vorschau** &gt; **Viewer-Liste**.

      Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**Code einbetten**“. As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.

   * Klicken Sie auf „**Listenansicht**“. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und klicken Sie dann rechts neben dem Miniaturbild auf „**Vorschau**“ &gt; „**Viewer-Liste**“.

      Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**Code einbetten**“. As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.

   * Klicken Sie auf „**Rasteransicht**“, „**Listenansicht**“ oder „**Detailansicht**“. Klicken Sie in der gleichen Symbolleiste auf „**Vorschau**“ &gt; „**Viewer-Liste**“.

      Klicken Sie auf der Seite „Viewer-Liste“ in der Spalte „Aktionen“ der Tabelle auf „**Code einbetten**“. As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.

1. Klicken Sie im Dialogfeld „Code einbetten“ auf „**In Zwischenablage kopieren**“.

   Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

1. Klicken Sie auf „**Schließen**“.
1. Fügen Sie den Einbettungscode in Ihre Webseiten ein.

### Implementing embed code for using HTML5 video with MP4 video assets {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

If you do not use the Dynamic Media Classic HTML5 video player, but instead want to use the native HTML5 `<video>` tag with MP4 video assets, you can use the following embed code sample:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Replace `"S7 video thumbnail URL"` with the video’s thumbnail URL. Hierbei handelt es sich um das Miniaturbild des Videos, das Benutzer vor der Wiedergabe des Videos sehen.

   Siehe [Abrufen von Videominiatur-URLs](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Replace `"S7 OGG video asset URL (no player)"` with the video’s progressive URL for OGG video.

   Siehe [Verknüpfen einer Video-URL mit einer mobilen Site oder Website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Ersetzen `"S7 MP4 mobile progressive video asset URL (no player)"` Sie durch die progressive Mobil-URL des Videos.

   Siehe [Verknüpfen einer Video-URL mit einer mobilen Site oder Website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Bereitstellen von Videos mithilfe von Video-Playern von von Drittanbietern {#deploying-video-using-a-third-party-video-player}

Wenn Sie einen Video-Player eines Drittanbieters oder einen benutzerdefinierten Video-Player anstelle eines Video-Viewers für dynamische Medien verwenden, können Sie die direkte Video-URL abrufen, die für das Video-Streaming mit mehreren Bitraten oder progressiven Downloads verwendet werden kann.

**So stellen Sie ein Video mit einem Video-Player eines Drittanbieters bereit**

1. Klicken Sie im Scene7 Publishing System auf der Symbolleiste für globale Navigation auf **Einstellungen** &gt; **Anwendungseinstellungen** &gt; **Allgemeine Einstellungen**.
1. Abhängig vom URL-Typ, die Sie verwenden möchten, führen Sie einen der folgenden Schritte aus:
* So generieren Sie eine direkte URL für HLS-Streaming-Video (mehrere Bitraten)

   Erstellen Sie auf der Seite Allgemeine **Programmeinstellungen** in der **Gruppe Server** im Textfeld **Veröffentlichungsservername** die direkte URL mithilfe der folgenden Syntax: `server/is/content/company/folder/filename.m3u8`
Angenommen, der Name des Veröffentlichungsservers `https://s7d9.scene7.com/.` verwendet die Syntax in Schritt 2, die direkte URL könnte wie folgt aussehen:
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* So generieren Sie eine direkte URL für HLS-Streaming-Video (eine Bitrate)

   On the **Application General Settings** page, in the **Servers** group, in the **HLS Streaming Server Name** text field, construct the direct URL using the following syntax:
   `server/company/folder/filename.ext.m3u8`Angenommen, der Name des HLS-Streaming-Servers `https://s7mbrstream.scene7.com/hls-vod/`lautet. Bei Verwendung der Syntax in Schritt 2 könnte die direkte URL wie folgt aussehen:
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* So generieren Sie eine direkte URL für ein progressives Video

   Erstellen Sie auf der Seite **Allgemeine Programmeinstellungen** in der Gruppe **Server** im Textfeld **Servername für progressives Video** die direkte URL für das eVideo unter Verwendung der folgenden Syntax: `server/company/folder/filename`Angenommen, der Servername für den progressiven Video `https://s7d9.scene7.com/is/content/`lautet. Bei Verwendung der Syntax in Schritt 2 könnte die direkte URL wie folgt aussehen:
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Arbeiten mit Videominiaturen {#working-with-video-thumbnails}

Dynamic Media Classic erstellt Miniaturansichten für kodierte Videos und vorkodierte Videos. Videominiaturen können wie alle anderen Bild-Assets verwendet werden. Darüber hinaus können Sie urls für die Videominiaturen abrufen, die von Dynamic Media Classic erstellt und außerhalb von SPS bereitgestellt werden. Beispielsweise können Sie die Miniaturansichten in Suchergebnissen, relevanten Videolisten und Videowiedergabelisten auf einer Website bereitstellen.

Miniaturansichten werden basierend auf dem ersten heterogenen Frame (d. h. kein vollständig schwarzer oder vollständig weißer Frame usw.) des Videos generiert.

### Abrufen von Videominiatur-URLs {#obtaining-video-thumbnail-urls}

Dynamic Media Classic erstellt während des Upload-Vorgangs automatisch Videominiaturen. Die Miniaturansichten werden im Durchsuchenbedienfeld in der Listen- und Rasteransicht angezeigt.

Führen Sie zum Erstellen von URLs für Videominiaturen einen Veröffentlichungsvorgang durch.

Siehe [Veröffentlichen von Videos](deploying-video-websites-mobile-sites.md#publishing_video).

Nach der Veröffentlichung können Sie Videominiatur-URLs in der Detailansicht im URL-Bedienfeld sowie im Code-einbetten-Bedienfeld abrufen. Klicken Sie auf der rechten Seite der Videominiatur auf **„URL kopieren“**, um die entsprechende URL zu kopieren.

### Bearbeiten von Standbildern in Video-Viewern {#modifying-poster-frames-in-video-viewers}

Das *Standbild* ist das erste Bild, das in Video-Viewern angezeigt wird, bevor die Wiedergabe beginnt. Dynamic Media Classic verwendet Videominiaturen als Standbilder.

Sie können auch Bildmodifikatoren auf das Standbild anwenden. Sie können das Standbild beispielsweise beschneiden oder transparent machen. Öffnen Sie zum Bearbeiten des Standbilds den Anzeigebereich „Konfiguration“ des Video-Viewers und geben Sie unter „Standbildmodifikatoren“ Modifikatoren ein. 

Siehe [Hinzufügen oder Bearbeiten einer Video-Viewer-Vorgabe](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Siehe [www.adobe.com/go/learn_s7_image_server_guide_en](https://www.adobe.com/go/learn_s7_image_server_guide_en).

Sie können auch Videominiaturen bearbeiten, indem Sie Modifikatoren an die Videominiatur-URLs anhängen.

>[!MORELIKETHIS]
>
>* [Veröffentlichen von Dateien](publishing-files.md#publishing_files)

