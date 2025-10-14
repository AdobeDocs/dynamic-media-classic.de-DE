---
title: Hinzufügen von Untertiteln zu Videos
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic Untertitel zu Videos hinzufügen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 17%

---

# Hinzufügen von Untertiteln zu Videos {#add-captions-to-video}

Erweitern der Reichweite Ihrer Videos auf globale Märkte. Dazu können Sie einzelnen Videos oder adaptiven Videosets Untertitel hinzufügen. Wenn Sie Untertitel hinzufügen, müssen Sie die Audiodaten nicht synchronisieren oder Muttersprachler damit beauftragen, die Audiodateien neu in einer anderen Sprache aufzuzeichnen. Das Video wird in der Sprache, in der es aufgenommen wurde, wiedergegeben. Fremdsprachliche Untertitel werden angezeigt, sodass auch Nutzer anderer Sprachen den Audioteil noch verstehen können.

Untertitel bieten zudem eine größere Barrierefreiheit, indem optional zuschaltbare Untertitel für Personen mit Hörbehinderung verwendet werden.

>[!NOTE]
>
>Der verwendete Video-Player muss die Anzeige von Untertiteln unterstützen. 

So konfigurieren Sie den Untertiteleffekt und bearbeiten Sie das Untertitelmenü selbst, einschließlich des Menütextes für einen der folgenden Viewer:

* `Universal_HTML5_Video` Viewer
* `Universal_HTML5_MixedMedia_dark` Viewer
* `Universal_HTML5_MixedMedia_light` Viewer

Siehe [Hinzufügen oder Bearbeiten einer Video-Viewer-Vorgabe](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Siehe auch [Hinzufügen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic kann Untertiteldateien in das JSON-Format (JavaScript Object Notation) konvertieren. Diese Konversion bedeutet, dass Sie den JSON-Text als verborgenes, aber vollständiges Transkript des Videos in eine Web-Seite einbetten können. Suchmaschinen können dann den Inhalt durchsuchen und indizieren, damit die Videos leichter auffindbar sind und Kunden weitere Details zum Videoinhalt erhalten.

Weitere [&#x200B; zur Verwendung der JSON-Funktion in einer URL &#x200B;](https://experienceleague.adobe.com/de/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents#image-serving-api) Sie unter „Statische Inhalte (keine Bilder) bereitstellen“ in .

**So fügen Sie einem Video Untertitel hinzu:**

1. Verwenden Sie außerhalb von Adobe Dynamic Media Classic ein Drittanbieterprogramm, um Ihre Videountertiteldatei basierend auf dem verwendeten Viewer-Typ zu erstellen.

   | Viewer-Typ | Untertiteldatei |
   |--- |--- |
   | HTML5 | Wenn Sie einen HTML5-Video-Viewer verwenden, stellen Sie sicher, dass die erstellte Untertiteldatei dem WebVTT-Standard (Web Video Text Tracks) folgt. Die Erweiterung der Untertiteldatei ist `.VTT`. Weitere Informationen zum WebVTT-Untertitelstandard<br><br>[Siehe WebVTT](https://w3c.github.io/webvtt/): The Web Video Text Tracks format. <br><br>Es gibt viele Websites, die sowohl kostenlose als auch kostenpflichtige Tools und Dienste anbieten, die Sie zum Erstellen von WebVTT-Untertiteldateien verwenden können. <br><br>Folgen Sie den Anweisungen auf dem Bildschirm von einer Website, um Ihre WebVTT-Datei zu erstellen und zu speichern. Wenn Sie fertig sind, kopieren Sie den Inhalt der Untertiteldatei und fügen Sie ihn in einen Texteditor ein. Speichern Sie ihn dann mit der Dateierweiterung VTT . <br><br><b>Hinweis</b> Für die globale Unterstützung von Videokapiteln in anderen Sprachen als Englisch erfordert der WebVTT-Standard, dass Sie separate `.VTT`-Dateien und Aufrufe für jede Sprache erstellen, die Sie unterstützen möchten. <br><br>Im Allgemeinen sollte die VTT-Untertiteldatei denselben Namen haben wie die Videodatei, an den aber Untertitel angehängt werden. Auf diese Weise können Sie die Generierung der Video-URLs mit Ihrem vorhandenen Web-Content-Management-System automatisieren. |

1. Laden Sie in Adobe Dynamic Media Classic Ihre WebVTT-, DFXP- oder SMPTE-XML-Untertiteldatei hoch.

   Siehe [Dateien hochladen](uploading-files.md#uploading_files).

1. Navigieren Sie im Bedienfeld „Asset-Bibliothek“ auf der linken Seite zum Asset-Ordner, der die Videodatei enthält, die mit der hochgeladenen Untertiteldatei verknüpft werden soll.
1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Video-Asset und dann unter dem Miniaturbild des Assets die Option **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.
1. Suchen Sie in der Viewer-Listentabelle den HTML5-Viewer mit dem Namen **Universal_HTML5_Video**, **Universal_HTML5_MixedMedia_dark** oder **Universal_HTML5_MixedMedia_light** und führen Sie einen der folgenden Schritte aus:

   * Um das Video in einem Popup-Fenster anzuzeigen, wählen **[!UICONTROL ganz rechts neben dem Namen]** URL kopieren“ aus.

     Hängen Sie die kopierte URL des Videos mit der folgenden Syntax an, um sie mit der kopierten URL Ihrer Untertiteldatei zu verknüpfen:

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     Notieren Sie den `,1` am Ende des URL-Pfads für die Beschriftung. Unmittelbar im Anschluss an die Dateierweiterung VTT haben Sie bei der Angabe des Pfads die Möglichkeit, die Schaltfläche für Untertitel durch Festlegen von `1` bzw. `0` in der Video-Player-Leiste zu aktivieren oder zu deaktivieren.

   * Um das Video in einem eingebetteten Viewer anzuzeigen, wählen **[!UICONTROL ganz rechts]** Namen „Einbettungs-Code“ aus.

     Wählen Sie im Dialogfeld „Einbettungs-Code“ die Option **[!UICONTROL In Zwischenablage kopieren]**.

     Hängen Sie für die HTML5 `Universal_HTML5_Video`-, `Universal_HTML5_MixedMedia_dark`- oder `Universal_HTML5_MixedMedia_light`-Viewer den kopierten Einbettungs-Code wie folgt an:

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     Notieren Sie die `,1` am Ende des URL-Pfads. Unmittelbar im Anschluss an die Dateierweiterung VTT haben Sie bei der Angabe des URL-Pfads die Möglichkeit, die Schaltfläche für Untertitel durch Festlegen von `1` bzw. `0` in der Video-Player-Leiste zu aktivieren oder zu deaktivieren.
