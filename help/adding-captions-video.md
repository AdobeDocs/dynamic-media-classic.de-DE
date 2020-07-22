---
title: Hinzufügen von Untertiteln zu Videos
seo-title: Hinzufügen von Untertiteln zu Videos
description: 'null'
seo-description: Informationen zum Hinzufügen von Untertiteln zu Videos
uuid: 4cc64469-4369-44a9-83db-63bad51aba8a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 64%

---


# Hinzufügen von Untertiteln zu Videos{#adding-captions-to-video}

Sie können die Relevanz Ihrer Videos global ausdehnen, indem Sie einzelnen Videos oder adaptive Video-Sets Untertitel hinzufügen. Wenn Sie Untertitel hinzufügen, müssen Sie die Audiodaten nicht synchronisieren oder Muttersprachler damit beauftragen, die Audiodateien neu in einer anderen Sprache aufzuzeichnen. Das Video wird in der Sprache, in der es aufgenommen wurde, wiedergegeben. Fremdsprachliche Untertitel werden angezeigt, sodass auch Nutzer anderer Sprachen den Audioteil noch verstehen können.

Untertitel bieten zudem eine größere Barrierefreiheit, indem optional zuschaltbare Untertitel für Personen mit Hörbehinderung verwendet werden.

>[!NOTE]
>
>Der verwendete Video-Player muss die Anzeige von Untertiteln unterstützen. 

Siehe [Hinzufügen und Bearbeiten von Video-Viewer-Vorgaben](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) für die Konfiguration des Untertitel-Effekts und zum Bearbeiten des Untertitelmenüs selbst, einschließlich des Menütextes für folgende Viewer:

* `Universal_HTML5_Video` Betrachter.
* `Universal_HTML5_MixedMedia_dark` Betrachter.
* `Universal_HTML5_MixedMedia_light` Betrachter.

Siehe auch [Hinzufügen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding_and_editing_viewer_presets).

Dynamic Media Classic kann Untertiteldateien in das JSON-Format (JavaScript Object Notation) konvertieren. Diese Konvertierung bedeutet, dass Sie den JSON-Text eine eine Webseite verborgen, aber als vollständiges Transkript des Video einfügen können. Suchmaschinen können dann den Inhalt durchsuchen und indizieren, damit Besucher die Videos leichter finden können und zusätzliche Details zum Videoinhalt erhalten.

See [Serving static (non-image) contents](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html) in the *Adobe Image Serving API Help* for more information about using the JSON function in a URL.

**So fügen Sie einem Video Untertitel hinzu**

1. Erstellen Sie mithilfe einer Drittanbieteranwendung außerhalb von Dynamic Media Classic Ihre Videountertiteldatei basierend auf dem von Ihnen verwendeten Viewer-Typ.

   | Viewer-Typ | Untertiteldatei |
   |--- |--- |
   | HTML5 | Wenn Sie einen HTML5-Video-Viewer verwenden, stellen Sie sicher, dass die erstellte Untertiteldatei dem WebVTT-Standard (Web Video Text Tracks) folgt. Die Erweiterung der Untertiteldatei lautet .vtt. Weitere Informationen zum WebVTT-Untertitelstandard<br><br>[Siehe WebVTT](https://dev.w3.org/html5/webvtt/): Das Format &quot;Web-Video-Textspuren&quot;. <br><br>Es gibt sowohl kostenlose als auch kostenpflichtige Tools und Dienste, die Sie zum Erstellen von Untertiteldateien außerhalb von Dynamic Media Classic verwenden können. Um beispielsweise eine einfache Videountertiteldatei ohne Stile zu erstellen, können Sie das folgende kostenlose Online-Werkzeug zum Erstellen und Bearbeiten von Untertiteln verwenden: <br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) Verwenden Sie <br><br>für optimale Ergebnisse das Tool in Internet Explorer 9 oder höher, Google Chrome oder Safari. <br><br>Fügen Sie im Programm im Feld <b>Enter URL of video file</b> (URL der Videodatei eingeben) die URL Ihrer Videodatei ein und klicken Sie anschließend auf <b>Load</b> (Laden). <br><br>Wenn Sie beispielsweise eine Dynamic Media Classic-URL für Ihre Videodatei verwenden, klicken Sie in DMC mit der Dublette auf ein einzelnes Video-Asset (kein adaptives Video-Set oder Übergeordnet-Video), um es in der Detail-Ansicht zu öffnen. Erweitern Sie im rechten Bereich der Detailansicht URLs und Code einbetten. Klicken Sie dann in der Gruppe „Mobil“ rechts neben „Mobil (Progressiv)“ auf URL kopieren. This process gives you the URL to the video file itself which you can then paste into the <b>Enter URL of video file</b> field. Internet Explorer, Chrome oder Safari können das Video dann nativ wiedergeben. Folgen Sie jetzt auf der Website den Anweisungen auf dem Bildschirm, um Ihre WebVTT-Datei zu erstellen und zu speichern. Wenn Sie fertig sind, kopieren Sie den Inhalt der Untertiteldatei und fügen Sie ihn in einen Texteditor ein. Speichern Sie ihn nun mit der Dateierweiterung .vtt. <br><br><b>Hinweis:</b> Für die globale Unterstützung von Videobeschriftungen in anderen Sprachen als Englisch müssen Sie beachten, dass der WebVTT-Standard separate .vtt-Dateien und Aufrufe für jede Sprache erfordert, die Sie unterstützen möchten. <br><br>Im Allgemeinen sollte der Name der Untertitel-VTT-Datei denselben Namen haben wie die Videodatei und über den Dateinamenanhang captions verfügen. Dies kann Ihnen bei der Automatisierung der Generierung von Videos URLs mit Ihrem vorhandenen Web-Inhalt-Managementsystem helfen. |

1. Laden Sie in Dynamic Media Classic Ihre WebVTT-, DFXP- oder SMPTE-XML-Untertiteldatei hoch.

   Siehe [Hochladen von Dateien](uploading-files.md#uploading_files).

1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der die Videodatei enthält, die Sie der hochgeladenen Untertiteldatei zuordnen möchten.
1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Video-Asset aus und klicken Sie anschließend unterhalb des Miniaturbilds des Assets auf **Vorschau** > **Viewer-Liste**.
1. In the Viewer List table, find the HTML5 viewer named **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark**, or **Universal_HTML5_MixedMedia_light**, then do one of the following:

   * Klicken Sie für einen Popup-Video-Viewer rechts neben dem Namen auf „**URL kopieren**“.

      Hängen Sie an die kopierte URL des Videos die folgende Syntax an, um es mit der kopierten URL der Untertiteldatei zuzuordnen:

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      Note the `,1` at the end of the caption URL path. Direkt nach der Dateierweiterung .vtt können Sie im Pfad die Untertitel-Schaltfläche in der Video-Player-Leiste aktivieren oder deaktivieren, indem Sie die Einstellung `1` bzw. `0` wählen.

   * Klicken Sie für einen eingebetteten Video-Viewer rechts neben dem Namen auf „**Code einbetten**“.

      Klicken Sie im Dialogfeld „Code einbetten“ auf „**In Zwischenablage kopieren**“.

      For the HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`, or `Universal_HTML5_MixedMedia_light` viewers, append the copied embed code with the following:

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      Note the `,1` at the end of the URL path. Direkt nach der Dateierweiterung .vtt können Sie im URL-Pfad die Untertitel-Schaltfläche in der Video-Player-Leiste aktivieren oder deaktivieren, indem Sie die Einstellung `1` bzw. `0` wählen.

