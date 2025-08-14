---
title: Video SEO
description: Erfahren Sie, wie Sie Video-SEO-Einstellungen in Adobe Dynamic Media Classic konfigurieren.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 27%

---

# Video SEO{#video-seo-search-engine-optimization}

Die Suchmaschinenoptimierung (SEO) ist ein Vorgang, der die Erhöhung der Zugriffe auf eine Website über Suchmaschinen zum Ziel hat. Suchmaschinen sind zwar hervorragend darin, Informationen über textbasierte Inhalte zu sammeln, sie können jedoch keine Informationen über Videos auf angemessene Weise erfassen. Diese Informationen müssen ihnen zur Verfügung gestellt werden.

Mit Adobe Dynamic Media Classic Video SEO können Sie Videometadaten anwenden, um Suchmaschinen Beschreibungen Ihrer Videos bereitzustellen. Mit Adobe Dynamic Media Classic können Sie Video-Sitemaps und RSS-Feeds erstellen. Diese Standard-XML-Dateien werden zum Senden von Videoinformationen an Suchmaschinen verwendet:

* **Video-Sitemap**: Informiert Google genau darüber, wo und was der Videoinhalt auf einer Site ist. Videos können also in Google vollständig durchsucht werden. Eine Video-Sitemap kann beispielsweise die Laufzeit und Kategorien von Videos angeben. Informationen zu Video-Sitemaps finden Sie unter [Video-Sitemaps und Video-Sitemap-Alternativen](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&rd=1).

* **mRSS (Media Really Simple Syndication)-Feed**: Wird von Content-Herausgebern verwendet, um Mediendateien in Yahoo einzuspeisen! Videosuche einzuspeisen. Informationen zu mRSS-Feeds finden Sie unter [Video-Sitemaps und Video-Sitemap-Alternativen](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&rd=1).

>[!NOTE]
>
>Google unterstützt sowohl das Video-Sitemap- als auch das mRSS-Feed-Protokoll für die Übermittlung von Informationen an Suchmaschinen.

Adobe Dynamic Media Classic kann Video-Sitemaps und mRSS-Feeds aus Metadaten generieren, die mit jedem Video gespeichert werden. Beim Erstellen von Video-Sitemaps und mRSS-Feeds können Sie wählen, welche Metadatenfelder der Videos eingeschlossen werden sollen. Auf diese Weise beschreiben Sie Ihre Videos Suchmaschinen, damit Suchmaschinen den Traffic genauer zu Videos auf Ihrer Website leiten können.

>[!NOTE]
>
>Ermitteln Sie vor der Erstellung einer Video-Sitemap oder eines mRSS-Feeds, welche Felder die XML-Datei für die Suchmaschine enthalten muss und wie diese Felder strukturiert sein müssen. Gute Video-Sitemaps oder mRSS-Feeds müssen die Anforderungen der Suchmaschine erfüllen.

Adobe Dynamic Media Classic erstellt Berichte zu Video-Sitemaps und mRSS-Feeds, nachdem Sie sie generiert haben. Diese Berichte sind auf der Seite Video SEO-Bericht verfügbar.

>[!NOTE]
>
>Für die Video-Sitemaps und RSS-Feeds erfasst Adobe Dynamic Media Classic Metadaten nur aus Videos, die zur Veröffentlichung markiert sind. Markieren Sie Videos zur Veröffentlichung, um ihre Metadaten in Video-Sitemaps und RSS-Feeds einzuschließen.

## Video-SEO-Einstellungen auswählen

Wählen Sie Video-SEO-Einstellungen für Video-Sitemaps und mRSS-Feeds auf der Seite **[!UICONTROL Einstellungen für die Suchmaschinenoptimierung]**. Um diese Seite zu öffnen, gehen Sie in der globalen Navigationsleiste zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Einstellungen]**.

Im Bereich **[!UICONTROL Allgemeine Einstellungen]** können Sie auswählen, ob Sie Video-Sitemaps, mRSS-Feeds oder beides generieren möchten. Ordnen Sie **[!UICONTROL Bereich &quot;]**&quot; Metadatenfelder Eingabefeldern zu.

Nachdem Sie die Einstellungen ausgewählt haben **[!UICONTROL wählen Sie &quot;]**&quot; (oder **[!UICONTROL Speichern und generieren]** aus, um die Video-Sitemap, mRSS-Feeds oder beides zu erstellen.

### Allgemeine Einstellungen einrichten {#choosing-general-settings}

Wählen Sie in **[!UICONTROL Dropdown]** Liste „Erzeugungsmodus“ einen Berichtsmodus aus:

* **Video-Sitemap**: Erstellen einer Video-Sitemap.

* **mRSS-Feed**: Erstellen eines Medien-RSS-Feeds (mRSS).

* **Beide**: Erstellen Sie beide Arten von XML-Dateien.

* **Aus**: Wählen Sie diese Option, um die Erstellung von Video-Sitemaps und Medien-RSS-Feeds (mRSS) zu stoppen.

Wählen Sie in **[!UICONTROL Dropdown-Liste]** Automatischer/Manueller Modus“ aus, ob automatisch oder manuell generiert werden soll:

* **Automatikmodus**: Adobe Dynamic Media Classic generiert jeden Tag automatisch eine Video-Sitemap, einen Medien-RSS-Feed oder beides. Wählen Sie die Option **[!UICONTROL Zur Veröffentlichung markieren]** aus, damit Sie die von Adobe Dynamic Media Classic generierte XML-Datei automatisch zur Veröffentlichung markieren können.

   * **Zur Veröffentlichung markieren** Markiert die generierte XML-Datei zur Veröffentlichung.

* **Manueller Modus**: Adobe Dynamic Media Classic generiert die Video-Sitemap, den Medien-RSS-Feed (mRSS) oder beides, wenn Sie **[!UICONTROL Generieren]** oder **[!UICONTROL Speichern und]**) im Bildschirm „Einstellungen für die Suchoptimierung“ auswählen. Wählen Sie außerdem aus den folgenden Optionen:

   * **Keine weiteren Einstellungen**: Markiert die generierte XML-Datei nicht zur Veröffentlichung.

   * **Zur Veröffentlichung markieren**: Markiert die generierte XML-Datei zur Veröffentlichung.

   * **Teilweise Generierung zulassen**: Suchmaschinen können eine XML-Datei ablehnen, wenn sie nicht vollständige Metadateninformationen für alle Videos enthält. Diese Option generiert die XML-Datei auch dann, wenn für einige Videos keine Metadaten verfügbar sind. Im Anzeigebereich „Bericht“ wird eine Warnung registriert. Wählen Sie diese Option, wenn Sie die XML-Datei exportieren und die fehlenden Informationen manuell bearbeiten möchten.

### Auswählen von Erstellungseinstellungen {#choosing-generation-settings}

Im Bereich Erzeugungseinstellungen werden Eingabefelder für die Video-Sitemap, den RSS-Feed oder beides aufgelistet. Im Bedienfeld Metadaten werden die Namen der Metadatenfelder aufgelistet. Verwenden Sie den Bereich „Allgemeine Einstellungen“, um Eingabefelder und Metadatenfelder zu verknüpfen. Auf diese Weise teilen Sie Adobe Dynamic Media Classic mit, wo Metadaten für die Video-Sitemap und/oder den mRSS-Feed abgerufen werden sollen.

1. Wählen Sie im Menü „Metadaten-Ansichten“ eine Metadaten-Ansicht. Nachdem Sie eine Ansicht ausgewählt haben, werden die Namen der Metadatenfelder im Bedienfeld „Metadaten“ angezeigt.
Siehe [Metadaten-Ansichten](application-setup.md#metadata_views).
1. Ziehen Sie die Metadatenfeldnamen vom Metadatenbedienfeld zu den Eingabefeldern „Startseite“, „Titel“, „Beschreibung“, „Tags“ und „Kategorie“. Die Felder „Startseite“, „Titel“ und „Beschreibung“ sind obligatorisch.

   >[!NOTE]
   >
   >Sie können auch manuell Daten in die Eingabefelder eintragen.

1. Führen Sie einen der folgenden Schritte aus:

   * Um Ihre Einstellungen zu speichern, ohne die XML-Datei zu generieren, wählen Sie **[!UICONTROL Speichern]** aus.
   * Um die Datei zu speichern und zu generieren, wählen Sie **[!UICONTROL Speichern und generieren]**.

     Die XML-Datei wird erstellt und in das Auftragsprotokoll eingetragen. Video-Sitemap-Dateien (video-sitemap) und Media RSS (mRSS)-Feed-Dateien (mrss-feed) werden im Stammordner Ihres Unternehmens gespeichert.

>[!NOTE]
>
>Veröffentlichen Sie die Video-Sitemap oder den RSS-Feed, bevor Sie sie an Suchmaschinen senden können. Video-Sitemap- und Media RSS (mRSS)-Feed-Dateien werden im Stammordner des Unternehmens gespeichert. Markieren Sie diese XML-Dateien bei Bedarf zur Veröffentlichung und wählen Sie **[!UICONTROL Veröffentlichen]** aus.

## Video-Sitemap und RSS-Feed-Dateien an eine Suchmaschine senden {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Video-Sitemap- und Media RSS (mRSS)-Feed-Dateien werden im Stammordner des Unternehmens gespeichert:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Kopieren Sie eine dieser URLs in die Webmaster-Tools der Suchmaschine, um Ihre Video-Sitemap oder Ihre Medien-RSS-Feed-Datei (mRSS) an Suchmaschinen zu senden.

## Video-SEO-Berichte anzeigen {#viewing-video-seo-reports}

Sehen Sie sich Video-SEO-Berichte auf der Berichtseite zur Video-Suchmaschinenoptimierung an. Zum Öffnen dieser Seite navigieren Sie in der globalen Navigationsleiste zu **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Berichte]**.

Wenn bei der Erstellung eines Berichts Fehler aufgetreten sind, werden diese auf der Seite Bericht aufgeführt.
