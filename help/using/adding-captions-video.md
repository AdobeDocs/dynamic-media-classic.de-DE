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
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 32%

---

# Hinzufügen von Untertiteln zu Videos {#adding-captions-to-video}

Sie können die Relevanz Ihrer Videos global ausdehnen, indem Sie einzelnen Videos oder adaptive Video-Sets Untertitel hinzufügen. Wenn Sie Untertitel hinzufügen, müssen Sie die Audiodaten nicht synchronisieren oder Muttersprachler damit beauftragen, die Audiodateien neu in einer anderen Sprache aufzuzeichnen. Das Video wird in der Sprache, in der es aufgenommen wurde, wiedergegeben. Fremdsprachliche Untertitel werden angezeigt, sodass auch Nutzer anderer Sprachen den Audioteil noch verstehen können.

Untertitel bieten zudem eine größere Barrierefreiheit, indem optional zuschaltbare Untertitel für Personen mit Hörbehinderung verwendet werden.

>[!NOTE]
>
>Der verwendete Video-Player muss die Anzeige von Untertiteln unterstützen. 

So konfigurieren Sie den Beschriftungseffekt und bearbeiten das Untertitelmenü selbst, einschließlich des Menütextes für einen der folgenden Viewer:

* `Universal_HTML5_Video` Betrachter
* `Universal_HTML5_MixedMedia_dark` Betrachter
* `Universal_HTML5_MixedMedia_light` Betrachter

Siehe [Hinzufügen oder Bearbeiten von Video-Viewer-Vorgaben](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Siehe auch [Hinzufügen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic kann Untertiteldateien in das JSON-Format (JavaScript Object Notation) konvertieren. Diese Konvertierung bedeutet, dass Sie den JSON-Text eine eine Webseite verborgen, aber als vollständiges Transkript des Video einfügen können. Suchmaschinen können dann den Inhalt durchsuchen und indizieren, um die Videos leichter auffindbar zu machen und Kunden mehr Details über den Videoinhalt zu geben.

Siehe [Bereitstellen von statischen (Nicht-Bild-)Inhalten](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) im *Hilfe zur Adobe Image Serving-API* Weitere Informationen zur Verwendung der JSON-Funktion in einer URL.

**So fügen Sie einem Video Untertitel hinzu:**

1. Erstellen Sie mit einer Drittanbieteranwendung außerhalb von Adobe Dynamic Media Classic Ihre Videountertiteldatei basierend auf dem von Ihnen verwendeten Viewer-Typ.

   | Viewer-Typ | Untertiteldatei |
   |--- |--- |
   | HTML5 | Wenn Sie einen HTML5-Video-Viewer verwenden, stellen Sie sicher, dass die erstellte Untertiteldatei dem WebVTT-Standard (Web Video Text Tracks) folgt. Die Erweiterung der Untertiteldatei lautet .vtt. Weitere Informationen zum WebVTT-Untertitelstandard<br><br>[Siehe WebVTT](https://w3c.github.io/webvtt/): Das Webvideo-Text-Tracking-Format. <br><br>Es gibt sowohl kostenlose als auch kostenbasierte Tools und Dienste, mit denen Sie Untertiteldateien außerhalb von Adobe Dynamic Media Classic erstellen können. Um beispielsweise eine einfache Videountertiteldatei ohne Stile zu erstellen, können Sie das folgende kostenlose Online-Tool zur Erstellung und Bearbeitung von Untertiteln verwenden: <br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>Die besten Ergebnisse erzielen Sie mit dem Tool in Internet Explorer 9 oder höher, Google Chrome oder Safari. <br><br>Im Tool im <b>URL der Videodatei eingeben</b> ein, fügen Sie die URL Ihrer Videodatei ein und wählen Sie <b>Laden</b>. <br><br>Wenn Sie beispielsweise eine Adobe Dynamic Media Classic-URL für Ihre Videodatei verwenden, doppelklicken Sie auf ein einzelnes Video-Asset (kein adaptives Videoset oder Primäres Video), um es in der Detailansicht zu öffnen. Erweitern Sie im rechten Bereich der Detailansicht URLs und Code einbetten. Wählen Sie dann unter der Gruppe Mobile rechts neben Mobile (Progressiv) die Option <b>URL kopieren</b>. Durch diesen Prozess erhalten Sie die URL zur Videodatei selbst, die Sie dann in die <b>URL der Videodatei eingeben</b> -Feld. Internet Explorer, Chrome oder Safari können das Video dann nativ wiedergeben. Folgen Sie jetzt auf der Website den Anweisungen auf dem Bildschirm, um Ihre WebVTT-Datei zu erstellen und zu speichern. Wenn Sie fertig sind, kopieren Sie den Inhalt der Untertiteldatei und fügen Sie ihn in einen Texteditor ein. Speichern Sie ihn dann mit der VTT-Dateinamenerweiterung. <br><br><b>Hinweis:</b> Für die globale Unterstützung von Videobeschriftungen in anderen Sprachen als Englisch erfordert der WebVTT-Standard, dass Sie separate .vtt-Dateien und Aufrufe für jede Sprache erstellen, die Sie unterstützen möchten. <br><br>Im Allgemeinen sollte der Name der Untertitel-VTT-Datei denselben Namen haben wie die Videodatei und über den Dateinamenanhang captions verfügen. Dies kann Ihnen bei der Automatisierung der Generierung von Videos URLs mit Ihrem vorhandenen Web-Inhalt-Managementsystem helfen. |

1. Laden Sie in Adobe Dynamic Media Classic Ihre XML-Untertiteldatei WebVTT, DFXP oder SMPTE hoch.

   Siehe [Dateien hochladen](uploading-files.md#uploading_files).

1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zu dem Asset-Ordner, der die Videodatei enthält, die Sie der hochgeladenen Untertiteldatei zuordnen möchten.
1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Video-Asset aus und wählen Sie dann unter dem Miniaturbild des Assets die Option **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.
1. Suchen Sie in der Tabelle &quot;Viewer-Liste&quot;den HTML5-Viewer mit dem Namen **Universal_HTML5_Video**, **Universal_HTML5_MixedMedia_dark** oder **Universal_HTML5_MixedMedia_light**, führen Sie dann einen der folgenden Schritte aus:

   * Wählen Sie für ein Popup-Video-Viewer-Erlebnis **[!UICONTROL URL kopieren]** rechts vom Namen.

     Hängen Sie die kopierte URL des Videos mit der folgenden Syntax an, damit Sie sie mit der kopierten URL Ihrer Untertiteldatei verknüpfen können:

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     Beachten Sie die `,1` am Ende des Pfad der Beschriftungs-URL. Unmittelbar nach der VTT-Dateinamenerweiterung im Pfad können Sie optional die Untertitelschaltfläche in der Video-Player-Leiste aktivieren oder deaktivieren, indem Sie `1` oder `0`, bzw.

   * Für ein eingebettetes Video-Viewer-Erlebnis wählen Sie **[!UICONTROL Einbettungscode]** rechts vom Namen.

     Wählen Sie im Dialogfeld Einbettungscode die Option **[!UICONTROL In Zwischenablage kopieren]**.

     Für die HTML 5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`oder `Universal_HTML5_MixedMedia_light` -Viewer hängen Sie den kopierten Einbettungscode wie folgt an:

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     Beachten Sie die `,1` am Ende des URL-Pfads. Unmittelbar nach der VTT-Dateinamenerweiterung im URL-Pfad können Sie die Untertitelschaltfläche auf der Video-Player-Leiste optional aktivieren oder deaktivieren, indem Sie `1` oder `0`, bzw.
