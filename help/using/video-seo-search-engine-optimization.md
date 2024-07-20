---
title: Video SEO
description: Erfahren Sie, wie Sie Video SEO-Einstellungen in Adobe Dynamic Media Classic konfigurieren.
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

Die Suchmaschinenoptimierung (SEO) ist ein Vorgang, der die Erhöhung der Zugriffe auf eine Website über Suchmaschinen zum Ziel hat. Suchmaschinen eignen sich zwar hervorragend für die Erfassung von Informationen über textbasierte Inhalte, können jedoch keine Informationen über Videos abrufen. Diese Informationen sind ihnen vorzulegen.

Mit Adobe Dynamic Media Classic Video SEO können Sie Videometadaten anwenden, um Suchmaschinen Beschreibungen Ihrer Videos bereitzustellen. Mit Adobe Dynamic Media Classic können Sie Video-Sitemaps und mRSS-Feeds erstellen. Diese XML-Standarddateien werden zum Senden von Videoinformationen an Suchmaschinen verwendet:

* **Video-Sitemap**: Informiert Google genau, wo und was der Videoinhalt auf einer Site ist. Videos können also in Google vollständig durchsucht werden. Eine Video-Sitemap kann beispielsweise die Laufzeit und Kategorien von Videos angeben. Weitere Informationen zu Video-Sitemaps finden Sie unter [Video-Sitemaps und Video-Sitemap-Alternativen](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **mRSS (Media Really Simple Syndication)-Feed**: Wird von Inhaltsverlegern verwendet, um Mediendateien in Yahoo zu leiten! Videosuche einzuspeisen. Weitere Informationen zu mRSS-Feeds finden Sie unter [Video-Sitemaps und Video-Sitemap-Alternativen](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google unterstützt sowohl das Video-Sitemap- als auch das mRSS-Feed-Protokoll für die Übermittlung von Informationen an Suchmaschinen.

Adobe Dynamic Media Classic kann Video-Sitemaps und mRSS-Feeds aus Metadaten generieren, die mit jedem Video gespeichert werden. Beim Erstellen von Video-Sitemaps und mRSS-Feeds können Sie wählen, welche Metadatenfelder der Videos eingeschlossen werden sollen. Auf diese Weise beschreiben Sie Ihre Videos für Suchmaschinen, damit Suchmaschinen den Traffic präziser zu Videos auf Ihrer Website leiten können.

>[!NOTE]
>
>Ermitteln Sie vor der Erstellung einer Video-Sitemap oder eines mRSS-Feeds, welche Felder die XML-Datei für die Suchmaschine enthalten muss und wie diese Felder strukturiert sein müssen. Gute Video-Sitemaps oder mRSS-Feeds müssen die Anforderungen der Suchmaschine erfüllen.

Adobe Dynamic Media Classic erstellt Berichte über Video-Sitemaps und mRSS-Feeds, nachdem Sie sie generiert haben. Diese Berichte sind auf der Seite Video SEO-Bericht verfügbar.

>[!NOTE]
>
>Für die Video-Sitemaps und mRSS-Feeds erfasst Adobe Dynamic Media Classic Metadaten nur aus Videos, die zur Veröffentlichung markiert sind. Markieren Sie Videos zur Veröffentlichung, um ihre Metadaten in Video-Sitemaps und mRSS-Feeds einzuschließen.

## Video SEO-Einstellungen auswählen

Wählen Sie auf der Seite **[!UICONTROL Einstellungen für die Videosuchmaschinenoptimierung]** die Video SEO-Einstellungen für Video-Sitemaps und mRSS-Feeds aus. Um diese Seite zu öffnen, navigieren Sie in der Leiste &quot;Globale Navigation&quot;zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Einstellungen]**.

Wählen Sie im Bereich **[!UICONTROL Allgemeine Einstellung]** aus, ob Sie Video-Sitemaps, mRSS-Feeds oder beides generieren möchten. Ordnen Sie im Bereich **[!UICONTROL Erstellungseinstellungen]** Metadatenfelder Eingabefeldern zu.

Nachdem Sie die Einstellungen ausgewählt haben, wählen Sie **[!UICONTROL Speichern]** (oder **[!UICONTROL Speichern und generieren]**), um die Video-Sitemap, mRSS-Feeds oder beides zu erstellen.

### Einrichten allgemeiner Einstellungen {#choosing-general-settings}

Wählen Sie in der Dropdownliste **[!UICONTROL Erstellungsmodus]** einen Berichtsmodus aus:

* **Video-Sitemap**: Erstellen Sie eine Video-Sitemap.

* **mRSS-Feed**: Erstellen Sie einen Media RSS (mRSS)-Feed.

* **Beide**: Erstellen Sie beide Typen von XML-Dateien.

* **Aus**: Wählen Sie diese Option, um die Generierung von Video-Sitemaps und Media RSS (mRSS)-Feeds zu beenden.

Wählen Sie in der Dropdown-Liste **[!UICONTROL Automatischer/manueller Modus]** aus, ob automatisch oder manuell generiert werden soll:

* **Automatischer Modus**: Adobe Dynamic Media Classic generiert jeden Tag automatisch eine Video-Sitemap, einen Media RSS (mRSS)-Feed oder beides. Wählen Sie die Option **[!UICONTROL Für Publish markieren]** aus, damit Sie die von Adobe Dynamic Media Classic generierte XML-Datei automatisch zur Veröffentlichung markieren können.

   * **Markieren Sie für Publish** Markiert die erstellte XML-Datei zur Veröffentlichung.

* **Manueller Modus**: Adobe Dynamic Media Classic generiert die Video-Sitemap, den Media RSS (mRSS)-Feed oder beides, wenn Sie im Bildschirm &quot;Einstellungen für die Videosuche&quot;die Option **[!UICONTROL Generate]** oder **[!UICONTROL Save &amp; Generate]** auswählen. Wählen Sie außerdem aus den folgenden Optionen:

   * **Keine weiteren Einstellungen**: Markiert die generierte XML-Datei nicht zur Veröffentlichung.

   * **Für Publish markieren**: Markiert die generierte XML-Datei zum Veröffentlichen.

   * **Teilgenerierung zulassen**: Suchmaschinen können eine XML-Datei ablehnen, wenn sie keine vollständigen Metadateninformationen für alle Videos enthält. Mit dieser Option wird die XML-Datei generiert, selbst wenn für einige Videos keine Metadaten verfügbar sind. Im Anzeigebereich „Bericht“ wird eine Warnung registriert. Wählen Sie diese Option, wenn Sie die XML-Datei exportieren und die fehlenden Informationen manuell bearbeiten möchten.

### Auswählen von Erstellungseinstellungen {#choosing-generation-settings}

Im Bereich &quot;Erstellungseinstellungen&quot;werden Eingabefelder für die Video-Sitemap, den mRSS-Feed oder beides aufgelistet. Im Metadatenbedienfeld werden die Namen der Metadatenfelder aufgelistet. Verwenden Sie den Bereich „Allgemeine Einstellungen“, um Eingabefelder und Metadatenfelder zu verknüpfen. Dadurch teilen Sie Adobe Dynamic Media Classic mit, wo Metadaten für die Video-Sitemap und/oder den mRSS-Feed abgerufen werden sollen.

1. Wählen Sie im Menü „Metadaten-Ansichten“ eine Metadaten-Ansicht. Nachdem Sie eine Ansicht ausgewählt haben, werden die Namen der Metadatenfelder im Metadatenbedienfeld angezeigt.
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
>Publish Sie die Video-Sitemap oder den mRSS-Feed, bevor Sie sie an Suchmaschinen senden können. Video-Sitemap- und Media RSS (mRSS)-Feed-Dateien werden im Stammordner des Unternehmens gespeichert. Markieren Sie diese XML-Dateien gegebenenfalls zur Veröffentlichung und wählen Sie **[!UICONTROL Publish]** aus.

## Senden von Video-Sitemap- und mRSS-Feed-Dateien an eine Suchmaschine {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Video-Sitemap- und Media RSS (mRSS)-Feed-Dateien werden im Stammordner des Unternehmens gespeichert:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Kopieren Sie eine dieser URLs in die Webmaster-Tools der Suchmaschine, um Ihre Video-Sitemap- oder Media RSS (mRSS)-Feed-Datei an Suchmaschinen zu senden.

## Anzeigen von Video SEO-Berichten {#viewing-video-seo-reports}

Zeigen Sie Video SEO-Berichte auf der Seite Video Search Engine Optimization Report an. Um diese Seite zu öffnen, navigieren Sie in der Leiste &quot;Globale Navigation&quot;zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Berichte]**.

Wenn bei der Berichterstellung Fehler aufgetreten sind, werden diese auf der Seite Bericht aufgeführt.
