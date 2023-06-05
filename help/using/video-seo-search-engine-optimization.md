---
title: Video SEO
description: Erfahren Sie, wie Sie SEO-Einstellungen für Videos in Adobe Dynamic Media Classic konfigurieren.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 37%

---

# Video SEO{#video-seo-search-engine-optimization}

Die Suchmaschinenoptimierung (SEO) ist ein Vorgang, der die Erhöhung der Zugriffe auf eine Website über Suchmaschinen zum Ziel hat. Suchmaschinen zeigen beim Sammeln von Informationen zu textbasierten Inhalten ausgezeichnete Leistung. Bei Videoinhalten können sie jedoch nur dann zufriedenstellende Informationen aufweisen, wenn diese direkt in die Suchmaschine eingespeist werden.

Mit Adobe Dynamic Media Classic Video SEO können Sie Videometadaten anwenden, um Suchmaschinen Beschreibungen Ihrer Videos bereitzustellen. Adobe Dynamic Media Classic bietet Ihnen die Möglichkeit, Video-Sitemaps und mRSS-Feeds zu erstellen. Diese XML-Standarddateien werden zum Senden von Videoinformationen an Suchmaschinen verwendet:

* **Video-Sitemap** - Informiert Google genau darüber, wo und was der Videoinhalt auf einer Site ist. Videos können also in Google vollständig durchsucht werden. Eine Video-Sitemap kann beispielsweise die Laufzeit und Kategorien von Videos angeben. Weitere Informationen zu Video-Sitemaps finden Sie unter [Video-Sitemaps und Video-Sitemap-Alternativen](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **mRSS-Feed (Media Really Simple Syndication)** - Wird von Content-Herausgebern verwendet, um Mediendateien in Yahoo! Videosuche einzuspeisen. Weitere Informationen zu mRSS-Feeds finden Sie unter [Video-Sitemaps und Video-Sitemap-Alternativen](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google unterstützt sowohl das Video-Sitemap- als auch das mRSS-Feed-Protokoll für die Übermittlung von Informationen an Suchmaschinen.

Adobe Dynamic Media Classic kann Video-Sitemaps und mRSS-Feeds aus Metadaten generieren, die mit jedem Video gespeichert werden. Beim Erstellen von Video-Sitemaps und mRSS-Feeds können Sie wählen, welche Metadatenfelder der Videos eingeschlossen werden sollen. Auf diese Weise beschreiben Sie Suchmaschinen Ihre Videos, damit diese Besucher treffsicherer zu Videos auf Ihrer Website leiten können.

>[!NOTE]
>
>Ermitteln Sie vor der Erstellung einer Video-Sitemap oder eines mRSS-Feeds, welche Felder die XML-Datei für die Suchmaschine enthalten muss und wie diese Felder strukturiert sein müssen. Gute Video-Sitemaps oder mRSS-Feeds müssen die Anforderungen der Suchmaschine erfüllen.

Adobe Dynamic Media Classic erstellt Berichte über Video-Sitemaps und mRSS-Feeds, nachdem Sie sie generiert haben. Diese Berichte sind auf der Seite Video SEO-Bericht verfügbar.

>[!NOTE]
>
>Für die Video-Sitemaps und mRSS-Feeds erfasst Adobe Dynamic Media Classic Metadaten nur aus Videos, die zur Veröffentlichung markiert sind. Markieren Sie Videos zur Veröffentlichung, um ihre Metadaten in Video-Sitemaps und mRSS-Feeds einzuschließen.

## Video SEO-Einstellungen auswählen {#choosing-video-seo-settings}

Wählen Sie Video SEO-Einstellungen für Video-Sitemaps und mRSS-Feeds auf der Seite **[!UICONTROL Optimierungseinstellungen für Video-Suchmaschinen]** Seite. Um diese Seite zu öffnen, navigieren Sie in der Symbolleiste für globale Navigation zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Einstellungen]**.

Im **[!UICONTROL Allgemeine Einstellung]** können Sie festlegen, ob Sie Video-Sitemaps, mRSS-Feeds oder beides generieren möchten. Im **[!UICONTROL Generierungseinstellungen]** -Bereich, ordnen Sie Metadatenfelder Eingabefeldern zu.

Nachdem Sie die Einstellungen ausgewählt haben, wählen Sie **[!UICONTROL Speichern]** (oder **[!UICONTROL Speichern und generieren]**), um die Video-Sitemap, mRSS-Feeds oder beides zu erstellen.

### Einrichten allgemeiner Einstellungen {#choosing-general-settings}

Im **[!UICONTROL Generierungsmodus]** Dropdownliste einen Berichtsmodus auswählen:

* **Video-Sitemap** - Erstellen einer Video-Sitemap.

* **mRSS-Feed** - Erstellen Sie einen Media RSS (mRSS)-Feed.

* **Beide** - Erstellen Sie beide Typen von XML-Dateien.

* **Aus** - Wählen Sie diese Option, um die Generierung von Video-Sitemaps und Media RSS (mRSS)-Feeds zu beenden.

Im **[!UICONTROL Automatischer/manueller Modus]** in der Dropdown-Liste auswählen, ob automatisch oder manuell generiert werden soll:

* **Automatischer Modus** - Adobe Dynamic Media Classic generiert täglich automatisch eine Video-Sitemap, einen Media RSS (mRSS)-Feed oder beides. Wählen Sie die **[!UICONTROL Zur Veröffentlichung markieren]** -Option, um die von Adobe Dynamic Media Classic generierte XML-Datei automatisch zur Veröffentlichung zu markieren.

   * **Zur Veröffentlichung markieren** Markiert die erstellte XML-Datei zur Veröffentlichung.

* **Manueller Modus** - Adobe Dynamic Media Classic generiert die Video-Sitemap, den Media RSS (mRSS)-Feed oder beides, wenn Sie **[!UICONTROL Erzeugen]** oder **[!UICONTROL Speichern und generieren]** im Bildschirm &quot;Einstellungen für die Videosuche&quot;. Wählen Sie außerdem aus den folgenden Optionen:

   * **Keine weiteren Einstellungen** - Markiert die erstellte XML-Datei nicht zur Veröffentlichung.

   * **Zur Veröffentlichung markieren** - Markiert die XML-Datei, die generiert wird, um sie zu veröffentlichen.

   * **Partielle Erstellung zulassen** - Suchmaschinen können eine XML-Datei ablehnen, wenn sie keine vollständigen Metadateninformationen für alle Videos enthält. Mit dieser Option wird die XML-Datei generiert, selbst wenn für einige Videos keine Metadaten verfügbar sind. Im Anzeigebereich „Bericht“ wird eine Warnung registriert. Wählen Sie diese Option, wenn Sie die XML-Datei exportieren und die fehlenden Informationen manuell bearbeiten möchten.

### Auswählen von Erstellungseinstellungen {#choosing-generation-settings}

Im Bereich &quot;Erstellungseinstellungen&quot;werden Eingabefelder für die Video-Sitemap, den mRSS-Feed oder beides sowie im Metadatenbedienfeld die Namen der Metadatenfelder aufgelistet. Verwenden Sie den Bereich „Allgemeine Einstellungen“, um Eingabefelder und Metadatenfelder zu verknüpfen. Auf diese Weise teilen Sie Adobe Dynamic Media Classic mit, wo Metadaten für die Video-Sitemap und/oder den mRSS-Feed abgerufen werden sollen.

1. Wählen Sie im Menü „Metadaten-Ansichten“ eine Metadaten-Ansicht. Wenn Sie eine Ansicht ausgewählt haben, werden die Namen der Metadatenfelder im Metadatenbedienfeld angezeigt.
Siehe [Metadaten-Ansichten](application-setup.md#metadata_views).
1. Ziehen Sie die Metadatenfeldnamen vom Metadatenbedienfeld zu den Eingabefeldern „Startseite“, „Titel“, „Beschreibung“, „Tags“ und „Kategorie“. Die Felder „Startseite“, „Titel“ und „Beschreibung“ sind obligatorisch.

   >[!NOTE]
   >
   >Sie können auch manuell Daten in die Eingabefelder eintragen.

1. Führen Sie einen der folgenden Schritte aus:

   * Um Ihre Einstellungen zu speichern, ohne die XML-Datei zu generieren, wählen Sie **[!UICONTROL Speichern]**.
   * Um die Datei zu speichern und zu generieren, wählen Sie **[!UICONTROL Speichern und generieren]**.

      Die XML-Datei wird erstellt und in das Auftragsprotokoll eingetragen. Video-Sitemap-Dateien (video-sitemap) und Media RSS (mRSS)-Feed-Dateien (mrss-feed) werden im Stammordner Ihres Unternehmens gespeichert.

>[!NOTE]
>
>Veröffentlichen Sie die Video-Sitemap oder den mRSS-Feed, bevor Sie ihn an Suchmaschinen senden können. Video-Sitemap- und Media RSS (mRSS)-Feed-Dateien werden im Stammordner des Unternehmens gespeichert. Markieren Sie diese XML-Dateien ggf. zur Veröffentlichung und wählen Sie **[!UICONTROL Veröffentlichen]**.

## Senden von Video-Sitemap- und mRSS-Feed-Dateien an eine Suchmaschine {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Video-Sitemap- und Media RSS (mRSS)-Feed-Dateien werden im Stammordner des Unternehmens gespeichert:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Kopieren Sie eine dieser URLs in die Webmaster-Tools einer Suchmaschine, um Ihre Video-Sitemap- oder Media RSS (mRSS)-Feed-Datei an diese Suchmaschine zu übermitteln.

## Anzeigen von Video SEO-Berichten {#viewing-video-seo-reports}

Zeigen Sie Video SEO-Berichte auf der Seite &quot;Video Search Engine Optimization Report&quot;an. Um diese Seite zu öffnen, navigieren Sie in der Symbolleiste für globale Navigation zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Berichte]**.

Wenn bei der Berichterstellung Fehler aufgetreten sind, werden diese auf der Seite Bericht aufgeführt.
