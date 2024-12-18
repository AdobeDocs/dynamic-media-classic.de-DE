---
title: Hinzufügen von Kapitelmarken zu Videos
description: Erfahren Sie, wie Sie einem Video in Adobe Dynamic Media Classic Kapitelmarken hinzufügen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 24%

---

# Hinzufügen von Kapitelmarken zu Videos {#adding-chapter-markers-to-video}

Um das Ansehen und Navigieren in langformatigen Videos zu vereinfachen, können Sie einzelnen Videos oder adaptiven Videosets Kapitelmarken hinzufügen. Wenn ein Benutzer das Video abspielt, kann er auf die Kapitelmarken in der Video-Zeitleiste (auch als Video-Scrubber bezeichnet) klicken. Dadurch können sie einfach zu ihrem Zielpunkt navigieren oder sofort zu neuen Inhalten, Demonstrationen, Tutorials usw. springen.

>[!NOTE]
>
>Der verwendete Video-Player muss die Verwendung von Kapitelmarken unterstützen. 

Siehe [Hinzufügen oder Bearbeiten einer Video-Viewer](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)-Vorgabe, wenn Sie die Kapitel-Navigations-Cue-Punkte und den Kapiteltitel-Popup-Text für den `Universal_HTML5_Video`-Viewer (HTML5) konfigurieren möchten.

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

Im obigen Beispiel ist `Chapter 1` die Cue-Point-Kennung. Diese ist optional. Die Cue-Point-Zeit `00:00:000 --> 01:04:364` gibt die Start- und Endzeit des Kapitels im Format 00:00:000 an. Die letzten drei Ziffern geben die Millisekunden an und können auf „000“ belassen werden. Der Kapiteltitel von `The bicycle store behind it all` ist die eigentliche Beschreibung des Kapitelinhalts. Die Cue-Point-Kennung, die Cue-Point-Startzeit und der Kapiteltitel werden im Video-Player in einem Popup-Fenster angezeigt, wenn der Mauszeiger über einen visuellen Cue-Point in der Video-Zeitleiste bewegt wird.

Da Sie einen HTML5-Video-Viewer verwenden, stellen Sie sicher, dass die erstellte Kapiteldatei dem WebVTT (Web Video Text Tracks)-Standard folgt. Die Erweiterung des Kapiteldateinamens ist `.VTT`. Weitere Informationen zum WebVTT-Untertitelstandard

Siehe [WebVTT: The Web Video Text Tracks format](https://w3c.github.io/webvtt/).

**So fügen Sie einem Video Kapitelmarken hinzu:**

1. Erstellen Sie Ihre Videokapiteldatei mit einem einfachen Texteditor außerhalb von Adobe Dynamic Media Classic.

   >[!NOTE]
   >
   >Für die globale Unterstützung von Videokapiteln in anderen Sprachen als Englisch erfordert der WebVTT-Standard, dass Sie separate `.VTT`-Dateien und Aufrufe für jede Sprache erstellen, die Sie unterstützen möchten.

1. Speichern Sie die VTT-Datei mit UTF-8-Kodierung, um Problemen mit der Zeichendarstellung im Text der Kapiteltitel vorzubeugen.

   Im Allgemeinen sollte die Kapitel-VTT-Datei denselben Namen haben wie die Videodatei, an den jedoch `chapters` angehängt wird. Auf diese Weise können Sie die Generierung der Video-URLs mit Ihrem vorhandenen Web-Content-Management-System automatisieren.

1. Laden Sie in Adobe Dynamic Media Classic Ihre WebVTT-Kapiteldatei hoch.

   Siehe [Dateien hochladen](uploading-files.md#uploading_files).

1. Navigieren Sie im Bedienfeld „Asset-Bibliothek“ auf der linken Seite zum Asset-Ordner, der die Videodatei enthält, die mit der hochgeladenen Kapiteldatei verknüpft werden soll.
1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Video-Asset und dann unter dem Miniaturbild des Assets die Option **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.
1. Suchen Sie in der Tabelle „Viewer-Liste“ den HTML5-Viewer mit dem Namen **Universal_HTML5_Video** und führen Sie einen der folgenden Schritte aus:

   * Um das Video in einem Popup-Fenster anzuzeigen, wählen **[!UICONTROL ganz rechts neben dem Namen]** URL kopieren“ aus.

     Hängen Sie die kopierte URL des Videos mit der folgenden Syntax an, um sie mit der kopierten URL Ihrer Untertiteldatei zu verknüpfen:

     `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Um das Video in einem eingebetteten Viewer anzuzeigen, wählen **[!UICONTROL ganz rechts]** Namen „Einbettungs-Code“ aus.

     Wählen Sie im Dialogfeld „Einbettungs-Code“ die Option **[!UICONTROL In Zwischenablage kopieren]**.

     Hängen Sie für den HTML5-`Universal_HTML5_Video`-Viewer den kopierten Einbettungs-Code wie folgt an:

     `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*"`
