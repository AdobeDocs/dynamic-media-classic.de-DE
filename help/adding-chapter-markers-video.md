---
title: Hinzufügen von Kapitelmarken zu Videos
description: Erfahren Sie, wie Sie in Dynamic Media Classic Kapitelmarken zu einem Video hinzufügen.
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
feature: Dynamic Media Classic,Viewer,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
source-git-commit: 1d30c98b76ebe78ff60bae87bd112de7a577182d
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 42%

---

# Hinzufügen von Kapitelmarken zu Videos {#adding-chapter-markers-to-video}

Um das Betrachten von und das Navigieren in langen Videos zu vereinfachen, können Sie Kapitelmarken zu einzelnen Videos oder adaptiven Videosets hinzufügen. Wenn ein Benutzer das Video abspielt, kann er die Kapitelmarken in der Video-Timeline (auch als Video-Scrubber bezeichnet) auswählen. Auf diese Weise können sie einfach zu ihrem Zielpunkt navigieren oder sofort zu neuen Inhalten, Demonstrationen, Tutorials usw. springen.

>[!NOTE]
>
>Der verwendete Video-Player muss die Verwendung von Kapitelmarken unterstützen. 

Siehe [Hinzufügen oder Bearbeiten einer Video-Viewer-Vorgabe](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset), wenn Sie die Cue-Punkte für die Kapitelnavigation und den Popup-Text für Kapiteltitel für den Viewer `Universal_HTML5_Video` (HTML5) konfigurieren möchten.

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

Im obigen Beispiel ist `Chapter 1` der Cue-Point-Bezeichner. Diese Angabe ist optional. Die Cue-Point-Zeit von `00:00:000 --> 01:04:364` gibt die Start- und Endzeit des Kapitels im Format 00:00:000 an. Die letzten drei Ziffern geben die Millisekunden an und können auf „000“ belassen werden. Der Kapiteltitel von `The bicycle store behind it all` ist die tatsächliche Beschreibung des Kapitelinhalts. Die Cue-Point-ID, die Cue-Point-Zeit und der Kapiteltitel werden im Video-Player in einem Popup-Fenster angezeigt, wenn der Mauszeiger über einen visuellen Cue-Point in der Timeline des Videos bewegt wird.

Da Sie einen HTML5-Video-Viewer verwenden, stellen Sie sicher, dass die erstellte Kapiteldatei dem WebVTT (Web Video Text Tracks)-Standard folgt. Die Kapiteldateinamenerweiterung lautet .VTT. Weitere Informationen zum WebVTT-Untertitelstandard

Siehe [WebVTT: Der Web-Video-Text verfolgt das Format](https://w3c.github.io/webvtt/).

**So fügen Sie Kapitelmarken zu Video hinzu:**

1. Erstellen Sie Ihre Videokapiteldatei mit einem einfachen Texteditor außerhalb von Dynamic Media Classic.

   >[!NOTE]
   >
   >Für die globale Unterstützung von Videokapiteln in anderen Sprachen als Englisch erfordert der WebVTT-Standard, dass Sie separate .vtt-Dateien und Aufrufe für jede Sprache erstellen, die Sie unterstützen möchten.

1. Speichern Sie die VTT-Datei in UTF8-Kodierung, damit Sie Probleme mit der Zeichendarstellung im Text des Kapiteltitels vermeiden können.

   Im Allgemeinen sollte die Kapitel-VTT-Datei denselben Namen haben wie die Videodatei und über den Dateinamenanhang `chapters` verfügen. Dies kann Ihnen bei der Automatisierung der Generierung von Videos URLs mit Ihrem vorhandenen Web-Inhalt-Managementsystem helfen.

1. Laden Sie in Dynamic Media Classic Ihre WebVTT-Kapiteldatei hoch.

   Siehe [Hochladen von Dateien](uploading-files.md#uploading_files).

1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der die Videodatei enthält, die Sie der hochgeladenen Kapiteldatei zuordnen möchten.
1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Video-Asset aus und klicken Sie dann unter dem Miniaturbild des Assets auf **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.
1. Suchen Sie in der Tabelle „Viewer-Liste“ den HTML5-Viewer mit dem Namen **Universal_HTML5_Video** und führen Sie einen der folgenden Schritte aus:

   * Wählen Sie für ein Popup-Video-Viewer-Erlebnis **[!UICONTROL URL]** rechts neben dem Namen kopieren aus.

      Hängen Sie die kopierte URL des Videos mit der folgenden Syntax an, damit Sie sie mit der kopierten URL Ihrer Untertiteldatei verknüpfen können:

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * Wählen Sie für ein eingebettetes Video-Viewer-Erlebnis **[!UICONTROL Einbettungscode]** rechts neben dem Namen aus.

      Wählen Sie im Dialogfeld &quot;Einbettungscode&quot;die Option **[!UICONTROL In Zwischenablage kopieren]**.

      Hängen Sie für den HTML5 `Universal_HTML5_Video`-Viewer den kopierten Einbettungscode wie folgt an:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`
