---
title: Hinzufügen von Kapitelmarken zu Video
seo-title: Hinzufügen von Kapitelmarken zu Video
description: 'null'
seo-description: Erfahren Sie, wie Sie Kapitelmarken zu einem Video hinzufügen.
uuid: 4 e 1 e 6 daf-afc 6-49 d 9-ac 90-183 fe 2 a 903 b 2
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/video
discoiquuid: 8 bc 5 e 552-2 abb -41 f 0-89 d 2-bdf 3 ae 5 d 96 c 2
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Hinzufügen von Kapitelmarken zu Video{#adding-chapter-markers-to-video}

Um das Betrachten von und das Navigieren in langen Videos zu vereinfachen, können Sie Kapitelmarken zu einzelnen Videos oder adaptiven Videosets hinzufügen. Wenn Benutzer das Video abspielen, können sie in der Videozeitleiste (auch Video-Abspielleiste genannt) auf eine Kapitelmarke klicken, um zu einer bestimmten Stelle im Video oder direkt zu anderen Inhalten, Demos, Übungen usw. zu springen.

>[!NOTE]
>
>Der verwendete Video-Player muss die Verwendung von Kapitelmarken unterstützen. 

Informationen zum Konfigurieren der Cue-Points für die Kapitelnavigation und der in Popups angezeigten Kapiteltitel für den [-Viewer (HTML5) finden Sie unter ](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)Hinzufügen oder Bearbeiten einer Video-Viewer-Vorgabe`Universal_HTML5_Video`.

Siehe auch [Hinzufügen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding_and_editing_viewer_presets).

Das Erstellen einer Kapitelliste für ein Video ist mit dem Erstellen von Untertiteln vergleichbar. Das heißt, Sie müssen eine WebVTT-Datei erstellen. Beachten Sie jedoch, dass diese Datei getrennt von der WebVTT-Untertiteldatei erstellt werden muss. Untertitel und Kapitel dürfen nicht in derselben WebVTT-Datei enthalten sein.

Sie können die WebVTT-Datei für die Kapitelnavigation nach folgendem Beispiel erstellen:

```as3
WEBVTT 
Chapter 1 
00:00.000 --> 01:04.364 
The bicycle store behind it all. 
Chapter 2 
01:04.364 --> 02:00.944 
Creative Cloud. 
Chapter 3 
02:00.944 --> 03:02.937 
Ease of management for a working solution. 
Chapter 4 
03:02.937 --> 03:35.000 
Cost-efficient access to rapidly evolving technology.
```

Im obigen Beispiel ist `Chapter 1` der Cue-Point-Bezeichner. Diese Angabe ist optional. Die Cue-Point-Zeit `00:00:000 --> 01:04:364` gibt die Start- und Endzeit des Kapitels im Format 00:00:000 an. Die letzten drei Ziffern geben die Millisekunden an und können auf „000“ belassen werden. The chapter title of `The bicycle store behind it all` is the actual description of the chapter’s contents. Der Cue-Point-Bezeichner, die Cue-Point-Zeit und der Kapiteltitel werden im Video-Player in einem Popup angezeigt, wenn ein Benutzer mit dem Mauszeiger auf einen visuellen Cue-Point in der Video-Zeitleiste zeigt oder darüberfährt.

Da Sie einen HTML5-Video-Viewer verwenden, stellen Sie sicher, dass die erstellte Kapiteldatei dem WebVTT (Web Video Text Tracks)-Standard folgt. Die Erweiterung der Kapiteldatei lautet .vtt. Weitere Informationen zum WebVTT-Untertitelstandard

See [WebVTT: The Web Video Text Tracks format](https://dev.w3.org/html5/webvtt/).

**So fügen Sie Kapitelmarken zu Video hinzu**

1. Erstellen Sie die Videokapiteldatei in einem einfachen Texteditor außerhalb von Scene7 Publishing System.

   >[!NOTE]
   >
   >Für globale Unterstützung von Videokapiteln in anderen Sprachen als Englisch erfordert der WebVTT-Standard separate .vtt-Dateien und Abrufe für jede Sprache, die unterstützt werden soll.

1. Speichern Sie die .vtt-Datei mit UTF-8-Kodierung, um Problemen mit der Zeichenwiedergabe im Text der Kapiteltitel vorzubeugen.

   Im Allgemeinen sollte die Kapitel-VTT-Datei denselben Namen haben wie die Videodatei und über den Dateinamenanhang `chapters` verfügen. Dies kann Ihnen bei der Automatisierung der Generierung von Video-URLs mit Ihrem vorhandenen Web-Inhalt-Managementsystem helfen.

1. Laden Sie die WebVTT-Kapiteldatei in Scene7 Publishing System hoch.

   Siehe [Hochladen von Dateien](uploading-files.md#uploading_files).

1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der die Videodatei enthält, die Sie der hochgeladenen Kapiteldatei zuordnen möchten.
1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Video-Asset aus und klicken Sie anschließend unterhalb des Miniaturbildes des Assets auf **Vorschau** &gt; **Viewer-Liste**.
1. Suchen Sie in der Tabelle „Viewer-Liste“ den HTML5-Viewer mit dem Namen **Universal_HTML5_Video** und führen Sie einen der folgenden Schritte aus:

   * Klicken Sie für einen Popup-Video-Viewer rechts neben dem Namen auf „**URL kopieren**“.

      Hängen Sie an die kopierte URL des Videos die folgende Syntax an, um es mit der kopierten URL der Untertiteldatei zuzuordnen:

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Klicken Sie für einen eingebetteten Video-Viewer rechts neben dem Namen auf „**Code einbetten**“.

      Klicken Sie im Dialogfeld „Code einbetten“ auf „**In Zwischenablage kopieren**“.

      For the HTML5 `Universal_HTML5_Video` viewer, append the copied embed code with the following:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`

