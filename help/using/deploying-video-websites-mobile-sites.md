---
title: Bereitstellen von Videos auf Websites und mobilen Sites
description: Erfahren Sie, wie Sie Videos von Adobe Dynamic Media Classic auf Ihren Websites und mobilen Sites bereitstellen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1703'
ht-degree: 23%

---

# Bereitstellen von Videos auf Websites und mobilen Sites{#deploying-video-to-your-websites-and-mobile-sites}

Websites, mobile Websites und Desktop-Programme greifen mithilfe von URL-Zeichenfolgen oder eingebettetem Code auf Adobe Dynamic Media Classic-Server-Inhalte (einschließlich Videos) zu. Adobe Dynamic Media Classic aktiviert diese URL-Zeichenfolgen während des Veröffentlichungsprozesses. Um die URL-Zeichenfolge oder den Einbettungs-Code für Ihr Video auf Ihren Webseiten, Mobilseiten und Desktop-Anwendungen zu platzieren, kopieren Sie sie bzw. ihn aus Adobe Dynamic Media Classic.

>[!NOTE]
>
>Die URL oder der Einbettungs-Code ist erst aktiv, wenn Sie das Asset veröffentlichen.

## Veröffentlichen von Videos {#publishing-video}

Das Veröffentlichen eines Videos ermöglicht es Adobe Dynamic Media Classic-Servern, Videos auf Ihrer Website, mobilen Site oder Anwendung bereitzustellen.

Es gibt zwei verschiedene Methoden zum Veröffentlichen von Videos:

* **Publish-Videos automatisch und sofort beim Hochladen**: Im Rahmen des Video-Upload-Prozesses kann Adobe Dynamic Media Classic Videos automatisch veröffentlichen, wenn sie hochgeladen und kodiert werden. Diese Fähigkeit zur sofortigen Veröffentlichung bedeutet, dass es nicht notwendig ist, Videos separat zu veröffentlichen.

* **Publish-Videos nach dem Hochladen manuell**: Wenn Sie Videos nicht sofort veröffentlichen möchten, können Sie Videos jederzeit manuell veröffentlichen.

Nach dem Veröffentlichen von Videos aktiviert Adobe Dynamic Media Classic die URL-Zeichenfolgen für Ihre HTML-Seite oder Ihren Programm-Code.

**So veröffentlichen Sie ein Video:**

1. Führen Sie einen der folgenden Schritte aus:

   * Um Videos beim Hochladen automatisch und sofort zu veröffentlichen, wählen Sie auf der Seite „Hochladen“ nach dem Hochladen **[!UICONTROL Publish]**. An dieser Stellen ist der Vorgang abgeschlossen, Sie müssen keine weiteren Schritte ausführen.
   * Um Videos nach dem Hochladen manuell zu veröffentlichen, wählen Sie im Durchsuchen-Panel die Videos aus und wählen Sie dann in der globalen Navigationsleiste **Publish**.

## Verknüpfen einer Video-URL mit einer mobilen Site oder einer Website {#linking-a-video-url-to-a-mobile-site-or-a-website}

Wenn Sie ein Video veröffentlichen, können Sie die zugehörige URL zur Verwendung auf Ihrer Website, auf einer mobilen Site oder in einer Desktop-Anwendung abrufen. Verwenden Sie die Video-URL, wenn Sie Videos in einem Popup- oder modalen Fenster über der Web-Seite anzeigen möchten.

Wenn ein Kunde den Link auswählt, werden Gerät, Bandbreite und Bildschirmgröße automatisch erkannt. Das entsprechende Video wird zur Wiedergabe in einem vordefinierten Viewer für Desktop-PCs oder mit dem systemeigenen Videoplayer für Smartphones und Tablets des Mobilgeräts angezeigt. 

Siehe auch [Einbetten des Video-Viewers auf einer Web-Seite](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**So verknüpfen Sie eine Video-URL mit einer mobilen Site oder einer Website:**

1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets in **[!UICONTROL Dropdown]** Liste „Anzeigen“ **[!UICONTROL Video]** oder **[!UICONTROL Adaptives Videoset]**.
1. Im Bedienfeld „Asset-Bibliothek“ auf der linken Seite navigieren Sie zu dem Asset-Ordner, in dem das Video bzw. das adaptive Videoset enthalten ist, für das Sie eine Verknüpfung erstellen möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** oder **[!UICONTROL Listenansicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf eine Videominiatur, um sie in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld „URLs und Einbettungs-Code“ auf der rechten Seite unter HTTP-Streaming **[!UICONTROL URL kopieren]** rechts neben dem gewünschten Viewer aus. Es empfiehlt sich, die mit dem `Universal_HTML5_Video` Viewer verknüpfte URL zu kopieren.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und navigieren Sie dann unter dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Klicken Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle auf **[!UICONTROL URL kopieren]**. Es empfiehlt sich, die mit dem `Universal_HTML5_Video` Viewer verknüpfte URL zu kopieren.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und gehen Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Klicken Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle auf **[!UICONTROL URL kopieren]**. Es empfiehlt sich, die mit dem `Universal_HTML5_Video` Viewer verknüpfte URL zu kopieren.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Wechseln Sie in der Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Klicken Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle auf **[!UICONTROL URL kopieren]**. Es empfiehlt sich, die mit dem `Universal_HTML5_Video` Viewer verknüpfte URL zu kopieren.

1. Fügen Sie die HTML5 Video-URL auf Ihrer Website und Ihrer mobilen Site ein.

## Einbetten des Video-Viewers auf einer Web-Seite {#embedding-the-video-viewer-on-a-web-page}

Verwenden Sie die Funktion Einbettungs-Code , wenn Sie das auf der Web-Seite eingebettete Video wiedergeben möchten. Sie kopieren den Einbettungs-Code in die Zwischenablage, damit Sie ihn in Ihre Web-Seiten einfügen können. Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

Siehe auch [Verknüpfen einer Video-URL mit einer mobilen Site oder einer Website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**So betten Sie den Video-Viewer auf einer Web-Seite ein:**

1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets in der Dropdown-Liste Anzeigen **[!UICONTROL Video]** oder **[!UICONTROL Adaptives Videoset]**.
1. Navigieren Sie im Bedienfeld „Asset-Bibliothek“ auf der linken Seite zum Asset-Ordner, der das Video oder adaptive Videoset enthält, dessen Einbettungs-Code Sie kopieren möchten.
1. Führen Sie über dem Bedienfeld zum Durchsuchen von Assets auf der rechten Seite der Symbolleiste einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Rasteransicht]** oder **[!UICONTROL Listenansicht]** aus. Doppelklicken Sie im Bedienfeld zum Durchsuchen von Assets auf eine Videominiatur, um sie in der Detailansicht zu öffnen. Wählen Sie im Bedienfeld „URLs und Einbettungs-Code“ auf der rechten Seite unter HTTP-Streaming **[!UICONTROL Einbettungs-Code]** rechts neben dem gewünschten Viewer aus. Wählen Sie als Best Practice **[!UICONTROL Einbettungs-Code]** aus, der mit dem `Universal_HTML5_Video`-Viewer verknüpft ist.
   * Wählen Sie **[!UICONTROL Rasteransicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset und dann unter dem Videominiaturbild die Option **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle **[!UICONTROL Einbettungs-Code]** aus. Wählen Sie als Best Practice **[!UICONTROL Einbettungs-Code]** aus, der mit dem `Universal_HTML5_Video`-Viewer verknüpft ist.

   * Wählen Sie **[!UICONTROL Listenansicht]** aus. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Asset aus und gehen Sie dann rechts neben dem Miniaturbild zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle **[!UICONTROL Einbettungs-Code]** aus. Wählen Sie als Best Practice **[!UICONTROL Einbettungs-Code]** aus, der mit dem `Universal_HTML5_Video`-Viewer verknüpft ist.

   * Wählen Sie **[!UICONTROL Rasteransicht]**, **[!UICONTROL Listenansicht]** oder **[!UICONTROL Detailansicht]**. Wechseln Sie in der Symbolleiste zu **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.

     Wählen Sie auf der Seite „Viewer-Liste“ unter der Spalte „Aktionen“ der Tabelle **[!UICONTROL Einbettungs-Code]** aus. Wählen Sie als Best Practice **[!UICONTROL Einbettungs-Code]** aus, der mit dem `Universal_HTML5_Video`-Viewer verknüpft ist.

1. Wählen Sie im Dialogfeld „Einbettungs-Code“ die Option **[!UICONTROL In Zwischenablage kopieren]**.

   Die Bearbeitung von Code im Dialogfeld „Code einbetten“ ist nicht zulässig.

1. Wählen Sie **[!UICONTROL Schließen]** aus.
1. Fügen Sie den Einbettungs-Code in Ihre Web-Seiten ein.

### Implementieren von Einbettungs-Code für die Verwendung von HTML5-Videos mit MP4-Video-Assets {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Sie möchten den Adobe Dynamic Media Classic HTML5-Videoplayer möglicherweise nicht verwenden. Wenn Sie stattdessen das native HTML5-`<video>`-Tag mit MP4-Video-Assets verwenden möchten, können Sie das folgende Einbettungs-Code-Beispiel verwenden:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Ersetzen Sie `"S7 video thumbnail URL"` durch die Miniatur-URL des Videos, also das Miniaturbild des Videos, das ein Benutzer vor der Wiedergabe des Videos sieht.

  Siehe [Abrufen von Videominiatur-URLs](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Ersetzen Sie `"S7 OGG video asset URL (no player)"` durch die progressive URL des Videos für OGG-Videos.

  Siehe [Verknüpfen einer Video-URL mit einer mobilen Site oder einer Website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Ersetzen Sie `"S7 MP4 mobile progressive video asset URL (no player)"` durch die progressive URL des Videos für Mobilgeräte.

  Siehe [Verknüpfen einer Video-URL mit einer mobilen Site oder einer Website](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## Bereitstellen von Videos mit einem Videoplayer eines Drittanbieters {#deploying-video-using-a-third-party-video-player}

Wenn Sie anstelle eines Dynamic Media Classic-Video-Viewers Videoplayer von Drittanbietern oder einen benutzerdefinierten Video-Player verwenden, erhalten Sie die direkte Video-URL, die für Multi-Bitrate-Video-Streaming oder progressiven Download von HLS funktioniert.

**So stellen Sie Videos mit einem Videoplayer eines Drittanbieters bereit:**

1. Wechseln Sie in Adobe Dynamic Media Classic in der globalen Navigationsleiste zu **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Allgemeine Einstellungen]**.
1. Abhängig vom URL-Typ, die Sie verwenden möchten, führen Sie einen der folgenden Schritte aus:

* So generieren Sie eine direkte Streaming-Video-URL für HLS (mit mehreren Bit-Raten)

  Erstellen Sie auf **[!UICONTROL Seite Allgemeine]** in der Gruppe **[!UICONTROL Server]** im Textfeld **[!UICONTROL Veröffentlichungs-Server-]** die direkte URL. Verwenden Sie die folgende Syntax: `server/is/content/company/folder/filename.m3u8`

  Angenommen, der Veröffentlichungs-Server-Name lautet `https://s7d9.scene7.com/.` Verwenden Sie die Syntax in Schritt 2, könnte die direkte URL wie folgt aussehen:
  `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* So generieren Sie eine direkte HLS-Streaming-Video-URL (Einzelbitrate)

  Erstellen Sie auf der Seite **[!UICONTROL Allgemeine Anwendungseinstellungen]** in der Gruppe **[!UICONTROL Server]** im Textfeld **[!UICONTROL HLS Streaming Server Name]** die direkte URL mit der folgenden Syntax:

  `server/company/folder/filename.ext.m3u8`

  Angenommen, der Name des HLS-Streaming-Servers ist `https://s7mbrstream.scene7.com/hls-vod/`. Bei Verwendung der Syntax in Schritt 2 könnte die direkte URL wie folgt aussehen:
  `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* So generieren Sie eine direkte URL für ein progressives Video

  Erstellen Sie auf der Seite **[!UICONTROL Allgemeine Programmeinstellungen]** in der Gruppe **[!UICONTROL Server]** im Textfeld **[!UICONTROL Servername für progressives Video]** die direkte URL für das eVideo unter Verwendung der folgenden Syntax:

  `server/company/folder/filename`

  Angenommen, der Name des progressiven Video-Servers ist `https://s7d9.scene7.com/is/content/`. Bei Verwendung der Syntax in Schritt 2 könnte die direkte URL wie folgt aussehen:
  `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## Arbeiten mit Videominiaturen {#working-with-video-thumbnails}

Adobe Dynamic Media Classic generiert Miniaturen für kodierte Videos und vorkodierte Videos. Videominiaturen können wie alle anderen Bild-Assets verwendet werden. Außerdem können Sie URLs für die von Adobe Dynamic Media Classic generierten Videominiaturen abrufen. Anschließend können Sie diese URLs außerhalb von Adobe Dynamic Media Classic bereitstellen. Beispielsweise können Sie die Miniaturansichten in Suchergebnissen, relevanten Videolisten und Videowiedergabelisten auf einer Website bereitstellen.

Miniaturansichten werden basierend auf dem ersten heterogenen Frame (d. h. kein vollständig schwarzer oder vollständig weißer Frame usw.) des Videos generiert.

### Abrufen von URLs für Videominiaturen {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classic generiert beim Hochladen automatisch Videominiaturansichten. Die Miniaturen werden im Durchsuchen-Panel in der Listen- und Rasteransicht angezeigt.

Führen Sie zum Erstellen von URLs für Videominiaturen einen Veröffentlichungsvorgang durch.

Siehe [Publish-Video](deploying-video-websites-mobile-sites.md#publishing_video).

Nach der Veröffentlichung können Sie Videominiatur-URLs in der Detailansicht im URL-Bedienfeld sowie im Code-einbetten-Bedienfeld abrufen. Wählen Sie **[!UICONTROL URL kopieren]** rechts neben der Videominiatur aus, damit Sie die zugehörige URL kopieren können.

### Ändern von Posterbildern in Video-Viewern {#modifying-poster-frames-in-video-viewers}

Das *Standbild* ist das erste Bild, das in Video-Viewern angezeigt wird, bevor die Wiedergabe beginnt. Adobe Dynamic Media Classic verwendet Videominiaturen als Standbilder.

Sie können auch Bildmodifikatoren auf das Standbild anwenden. Sie können das Standbild beispielsweise beschneiden oder transparent machen. Öffnen Sie zum Bearbeiten des Standbilds den Anzeigebereich „Konfiguration“ des Video-Viewers und geben Sie unter „Standbildmodifikatoren“ Modifikatoren ein. 

Siehe [Hinzufügen oder Bearbeiten einer Video-Viewer-Vorgabe](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Siehe [Image Serving Guide](https://experienceleague.adobe.com/de/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home#image-serving-api).

Sie können auch Videominiaturen bearbeiten, indem Sie Modifikatoren an die Videominiatur-URLs anhängen.

>[!MORELIKETHIS]
>
>* [Publish-Dateien](publishing-files.md#publishing_files)