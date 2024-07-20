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

Erweiterung der Reichweite Ihrer Videos auf globale Märkte. Fügen Sie dazu Untertitel zu einzelnen Videos oder adaptiven Videosets hinzu. Wenn Sie Untertitel hinzufügen, müssen Sie die Audiodaten nicht synchronisieren oder Muttersprachler damit beauftragen, die Audiodateien neu in einer anderen Sprache aufzuzeichnen. Das Video wird in der Sprache, in der es aufgenommen wurde, wiedergegeben. Fremdsprachliche Untertitel werden angezeigt, sodass auch Nutzer anderer Sprachen den Audioteil noch verstehen können.

Untertitel bieten zudem eine größere Barrierefreiheit, indem optional zuschaltbare Untertitel für Personen mit Hörbehinderung verwendet werden.

>[!NOTE]
>
>Der verwendete Video-Player muss die Anzeige von Untertiteln unterstützen. 

So konfigurieren Sie den Beschriftungseffekt und bearbeiten das Untertitelmenü selbst, einschließlich des Menütextes für einen der folgenden Viewer:

* `Universal_HTML5_Video` Viewer
* `Universal_HTML5_MixedMedia_dark` Viewer
* `Universal_HTML5_MixedMedia_light` Viewer

Siehe [Hinzufügen oder Bearbeiten einer Video-Viewer-Vorgabe](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

Siehe auch [Hinzufügen und Bearbeiten von Viewer-Vorgaben](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic kann Untertiteldateien in das JSON-Format (JavaScript Object Notation) konvertieren. Diese Konvertierung bedeutet, dass Sie den JSON-Text als ausgeblendetes, aber vollständiges Transkript des Videos in eine Webseite einbetten können. Suchmaschinen können dann den Inhalt durchsuchen und indizieren, um die Videos leichter auffindbar zu machen und Kunden mehr Details über den Videoinhalt zu geben.

Weitere Informationen zur Verwendung der JSON-Funktion in einer URL finden Sie unter [Serve static (non-image) contents](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents#image-serving-api) in .

**So fügen Sie einem Video Untertitel hinzu:**

1. Erstellen Sie mit einer Drittanbieteranwendung außerhalb von Adobe Dynamic Media Classic Ihre Videountertiteldatei basierend auf dem von Ihnen verwendeten Viewer-Typ.

   | Viewer-Typ | Untertiteldatei |
   |--- |--- |
   | HTML5 | Wenn Sie einen HTML5-Video-Viewer verwenden, stellen Sie sicher, dass die erstellte Untertiteldatei dem WebVTT-Standard (Web Video Text Tracks) folgt. Die Dateinamenerweiterung für die Untertitelung lautet `.VTT`. Weitere Informationen zum WebVTT-Untertitelstandard<br><br>[Siehe WebVTT](https://w3c.github.io/webvtt/): Das Format &quot;Text-Tracking für Webvideos&quot;. <br><br>Es gibt viele Websites, die sowohl kostenlose als auch gebührenbasierte Tools und Dienste anbieten, die Sie zum Erstellen von WebVTT-Untertiteldateien verwenden können. <br><br>Befolgen Sie die Anweisungen auf dem Bildschirm von einer Website, um Ihre WebVTT-Datei zu erstellen und zu speichern. Wenn Sie fertig sind, kopieren Sie den Inhalt der Untertiteldatei und fügen Sie ihn in einen Texteditor ein. Speichern Sie ihn dann mit der VTT-Dateinamenerweiterung. <br><br><b>Hinweis:</b> Zur globalen Unterstützung von Videobeschriftungen in anderen Sprachen als Englisch erfordert der WebVTT-Standard, dass Sie separate `.VTT`-Dateien und -Aufrufe für jede Sprache erstellen, die Sie unterstützen möchten. <br><br>Im Allgemeinen sollten Sie der VTT-Untertiteldatei denselben Namen geben wie der der Videodatei und sie mit Untertiteln anhängen. Auf diese Weise kann es Ihnen bei der Automatisierung der Generierung von Video-URLs mithilfe Ihres bestehenden Web Content Management-Systems helfen. |

1. Laden Sie in Adobe Dynamic Media Classic Ihre XML-Untertiteldatei WebVTT, DFXP oder SMPTE hoch.

   Siehe [Dateien hochladen](uploading-files.md#uploading_files).

1. Navigieren Sie auf der linken Seite der Asset-Bibliothek zum Asset-Ordner, der die Videodatei enthält, die mit der hochgeladenen Untertiteldatei verknüpft werden soll.
1. Wählen Sie im Bedienfeld zum Durchsuchen von Assets ein einzelnes Video-Asset aus und klicken Sie dann unter dem Miniaturbild des Assets auf **[!UICONTROL Vorschau]** > **[!UICONTROL Viewer-Liste]**.
1. Suchen Sie in der Tabelle &quot;Viewer-Liste&quot;den HTML5-Viewer mit dem Namen **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark** oder **Universal_HTML5_MixedMedia_light** und führen Sie einen der folgenden Schritte aus:

   * Wählen Sie für ein Popup-Video-Viewer-Erlebnis **[!UICONTROL URL kopieren]** rechts neben dem Namen aus.

     Hängen Sie die kopierte URL des Videos mit der folgenden Syntax an, damit Sie sie mit der kopierten URL Ihrer Untertiteldatei verknüpfen können:

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     Beachten Sie die `,1` am Ende des Pfad der Beschriftungs-URL. Unmittelbar nach der VTT-Dateinamenerweiterung im Pfad können Sie optional die Untertitelschaltfläche in der Video-Player-Leiste aktivieren oder deaktivieren, indem Sie auf `1` bzw. `0` festlegen.

   * Wählen Sie für ein eingebettetes Video-Viewer-Erlebnis **[!UICONTROL Einbettungscode]** rechts neben dem Namen aus.

     Wählen Sie im Dialogfeld &quot;Einbettungscode&quot;die Option **[!UICONTROL In Zwischenablage kopieren]**.

     Hängen Sie für die Viewer HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark` oder `Universal_HTML5_MixedMedia_light` den kopierten Einbettungscode wie folgt an:

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     Beachten Sie die `,1` am Ende des URL-Pfads. Unmittelbar nach der VTT-Dateinamenerweiterung im URL-Pfad können Sie die Untertitelschaltfläche in der Video-Player-Leiste optional aktivieren oder deaktivieren, indem Sie auf `1` bzw. `0` festlegen.
