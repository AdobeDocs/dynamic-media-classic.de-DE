---
title: Hinzufügen von Kapitelmarken zu Video
description: Erfahren Sie, wie Sie einem Video Kapitelmarken hinzufügen.
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
feature: Dynamic Media Classic,Viewers,Video
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 87%

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

Im obigen Beispiel ist `Chapter 1` der Cue-Point-Bezeichner. Diese Angabe ist optional. Die Cue-Point-Zeit `00:00:000 --> 01:04:364` gibt die Start- und Endzeit des Kapitels im Format 00:00:000 an. Die letzten drei Ziffern geben die Millisekunden an und können auf „000“ belassen werden. Der Kapiteltitel von `The bicycle store behind it all` ist die eigentliche Beschreibung des Kapitelinhalts. Der Cue-Point-Bezeichner, die Cue-Point-Zeit und der Kapiteltitel werden im Video-Player in einem Popup angezeigt, wenn ein Benutzer mit dem Mauszeiger auf einen visuellen Cue-Point in der Video-Zeitleiste zeigt oder darüberfährt.

Da Sie einen HTML5-Video-Viewer verwenden, stellen Sie sicher, dass die erstellte Kapiteldatei dem WebVTT (Web Video Text Tracks)-Standard folgt. Die Erweiterung der Kapiteldatei lautet .vtt. Weitere Informationen zum WebVTT-Untertitelstandard

Siehe [WebVTT: Das Web-Video-Text-Verfolgungsformat](https://dev.w3.org/html5/webvtt/).

**So fügen Sie Kapitelmarken zu Video hinzu**

1. Erstellen Sie Ihre Videokapiteldatei mit einem einfachen Texteditor außerhalb von Dynamic Media Classic.

   >[!NOTE]
   >
   >Für globale Unterstützung von Videokapiteln in anderen Sprachen als Englisch erfordert der WebVTT-Standard separate .vtt-Dateien und Abrufe für jede Sprache, die unterstützt werden soll.

1. Speichern Sie die .vtt-Datei mit UTF-8-Kodierung, um Problemen mit der Zeichenwiedergabe im Text der Kapiteltitel vorzubeugen.

   Im Allgemeinen sollte die Kapitel-VTT-Datei denselben Namen haben wie die Videodatei und über den Dateinamenanhang `chapters` verfügen. Dies kann Ihnen bei der Automatisierung der Generierung von Videos URLs mit Ihrem vorhandenen Web-Inhalt-Managementsystem helfen.

1. Laden Sie in Dynamic Media Classic Ihre WebVTT-Kapiteldatei hoch.

   Siehe [Hochladen von Dateien](uploading-files.md#uploading_files).

1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der die Videodatei enthält, die Sie der hochgeladenen Kapiteldatei zuordnen möchten.
1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Video-Asset aus und klicken Sie anschließend unterhalb des Miniaturbildes des Assets auf **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.
1. Suchen Sie in der Tabelle „Viewer-Liste“ den HTML5-Viewer mit dem Namen **Universal_HTML5_Video** und führen Sie einen der folgenden Schritte aus:

   * Klicken Sie für einen Popup-Video-Viewer rechts neben dem Namen auf „**[!UICONTROL URL kopieren]**“.

      Hängen Sie an die kopierte URL des Videos die folgende Syntax an, um es mit der kopierten URL der Untertiteldatei zuzuordnen:

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Klicken Sie für einen eingebetteten Video-Viewer rechts neben dem Namen auf „**[!UICONTROL Code einbetten]**“.

      Klicken Sie im Dialogfeld „Code einbetten“ auf „**[!UICONTROL In Zwischenablage kopieren]**“.

      Für den HTML5-Viewer `Universal_HTML5_Video` hängen Sie den kopierten Einbettungscode wie folgt an:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`

