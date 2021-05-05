---
title: Video SEO
description: Erfahren Sie, wie Sie Video SEO-Einstellungen konfigurieren.
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Administrator
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
translation-type: tm+mt
source-git-commit: 06bd65c92c88595786b14213944a7cebd0d2590b
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 40%

---

# Video SEO{#video-seo-search-engine-optimization}

Die Suchmaschinenoptimierung (SEO) ist ein Vorgang, der die Erhöhung der Zugriffe auf eine Website über Suchmaschinen zum Ziel hat. Suchmaschinen zeigen beim Sammeln von Informationen zu textbasierten Inhalten ausgezeichnete Leistung. Bei Videoinhalten können sie jedoch nur dann zufriedenstellende Informationen aufweisen, wenn diese direkt in die Suchmaschine eingespeist werden.

Mit Dynamic Media Classic Video SEO können Sie Videometadaten anwenden, um Suchmaschinen Beschreibungen Ihrer Videos bereitzustellen. Mit Dynamic Media Classic können Sie Video-Sitemaps und mRSS-Feeds erstellen. Diese Standard-XML-Dateien dienen zum Übermitteln von Videoinformationen an Suchmaschinen:

* **Video-Sitemap**  - Informiert Google genau, wo und was der Videoinhalt auf einer Site ist. Videos können also in Google vollständig durchsucht werden. Eine Video-Sitemap kann beispielsweise die Laufzeit und Kategorien von Videos angeben. Weitere Informationen zu Video-Sitemaps finden Sie unter [Video-Sitemaps und Video-Sitemap-Alternativen](https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **mRSS (Media Really Simple Syndication)-Feed**  - Wird von Herausgebern von Inhalten verwendet, um Mediendateien in Yahoo!! Videosuche einzuspeisen. Weitere Informationen zu mRSS-Feeds finden Sie unter [Video-Sitemaps und Video-Sitemap-Alternativen](https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google unterstützt sowohl das Video-Sitemap- als auch das mRSS-Feed-Protokoll für die Übermittlung von Informationen an Suchmaschinen.

Dynamic Media Classic kann Video-Sitemaps und mRSS-Feeds aus Metadaten erstellen, die mit jedem Video gespeichert werden. Beim Erstellen von Video-Sitemaps und mRSS-Feeds können Sie wählen, welche Metadatenfelder der Videos eingeschlossen werden sollen. Auf diese Weise beschreiben Sie Suchmaschinen Ihre Videos, damit diese Besucher treffsicherer zu Videos auf Ihrer Website leiten können.

>[!NOTE]
>
>Ermitteln Sie vor der Erstellung einer Video-Sitemap oder eines mRSS-Feeds, welche Felder die XML-Datei für die Suchmaschine enthalten muss und wie diese Felder strukturiert sein müssen. Gute Video-Sitemaps oder mRSS-Feeds müssen die Anforderungen der Suchmaschine erfüllen.

Dynamic Media Classic erstellt Berichte zu Video-Sitemaps und mRSS-Feeds, nachdem Sie sie generiert haben. Diese Berichte sind auf der Seite &quot;Bericht für Video SEO&quot;verfügbar.

>[!NOTE]
>
>Für Video-Sitemaps und mRSS-Feeds erfasst Dynamic Media Classic nur Metadaten aus Videos, die zur Veröffentlichung markiert wurden. Markieren Sie Videos zur Veröffentlichung, um ihre Metadaten in Video-Sitemaps und mRSS-Feeds einzuschließen.

## Auswählen der Video SEO-Einstellungen {#choosing-video-seo-settings}

Klicken Sie auf der Seite **[!UICONTROL Einstellungen für Video-Suchmaschinen]** auf Video SEO-Einstellungen für Video-Sitemaps und mRSS-Feeds. Um diese Seite zu öffnen, klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Einstellungen]**.

Legen Sie im Bereich **[!UICONTROL Allgemeine Einstellung]** fest, ob Video-Sitemaps, mRSS-Feeds oder beides erstellt werden soll. Ordnen Sie im Bereich **[!UICONTROL Erstellungseinstellungen]** Metadatenfelder Eingabefeldern zu.

Nachdem Sie die Einstellungen ausgewählt haben, klicken Sie auf **[!UICONTROL Speichern]** (oder **[!UICONTROL Speichern und Erstellen]**), um die Video-Sitemap, mRSS-Feeds oder beide zu erstellen.

### Auswählen von allgemeinen Einstellungen {#choosing-general-settings}

Wählen Sie in der Dropdown-Liste **[!UICONTROL Erstellungsmodus]** einen Berichtsmodus:

* **Video-Sitemap**  - Erstellen einer Video-Sitemap.

* **mRSS-Feed**  - Erstellen Sie einen Media RSS (mRSS)-Feed.

* **Beide**  - Erstellen Sie beide Arten von XML-Dateien.

* **Aus** - Wählen Sie diese Option, um die Generierung von Video-Sitemaps und Media RSS (mRSS)-Feeds zu beenden.

Wählen Sie in der Dropdown-Liste **[!UICONTROL Automatischer/manueller Modus]** aus, ob die Erstellung automatisch oder manuell erfolgen soll:

* **Automatischer Modus** : Dynamic Media Classic erstellt jeden Tag automatisch eine Video-Sitemap, ein Media RSS (mRSS)-Feed oder beides. Wählen Sie die Option &quot;Zur Veröffentlichung markieren&quot;, um die von Dynamic Media Classic erstellte XML-Datei automatisch zur Veröffentlichung zu markieren.

   * **Markieren Sie die erstellte XML-Datei zur Veröffentlichung** von PublishMarks.

* **Manueller Modus** : Dynamic Media Classic generiert die Video-Sitemap, den Media RSS (mRSS)-Feed oder beide, wenn Sie im Anzeigebereich &quot;Einstellungen für die Videosuche&quot;auf &quot;Erstellen&quot;oder &quot;Speichern und Erstellen&quot;klicken. Wählen Sie außerdem aus den folgenden Optionen:

   * **Keine weiteren Einstellungen** : Markiert die erstellte XML-Datei nicht zur Veröffentlichung.

   * **Zur Veröffentlichung markieren**  - Markiert die erstellte XML-Datei zur Veröffentlichung.

   * **Partielle Erstellung**  zulassen: Suchmaschinen können eine XML-Datei ablehnen, wenn sie keine vollständigen Metadaten für alle Videos enthält. Mit dieser Option wird die XML-Datei erstellt, selbst wenn für einige Videos keine Metadaten verfügbar sind. Im Anzeigebereich „Bericht“ wird eine Warnung registriert. Wählen Sie diese Option, wenn Sie die XML-Datei exportieren und die fehlenden Informationen manuell bearbeiten möchten.

### Auswählen von Erstellungseinstellungen  {#choosing-generation-settings}

Im Bereich &quot;Erstellungseinstellungen&quot;werden Eingabefelder für die Video-Sitemap, den mRSS-Feed oder beide sowie im Metadatenbedienfeld die Namen der Metadatenfelder Liste. Verwenden Sie den Bereich „Allgemeine Einstellungen“, um Eingabefelder und Metadatenfelder zu verknüpfen. Auf diese Weise teilen Sie Dynamic Media Classic mit, wo Sie Metadaten für die Video-Sitemap und/oder den mRSS-Feed abrufen können.

1. Wählen Sie im Menü „Metadaten-Ansichten“ eine Metadaten-Ansicht. Wenn Sie eine Ansicht ausgewählt haben, werden die Namen der Metadatenfelder im Metadatenbedienfeld angezeigt.
Siehe [Metadaten-Ansichten](application-setup.md#metadata_views).
1. Ziehen Sie die Metadatenfeldnamen vom Metadatenbedienfeld zu den Eingabefeldern „Startseite“, „Titel“, „Beschreibung“, „Tags“ und „Kategorie“. Die Felder „Startseite“, „Titel“ und „Beschreibung“ sind obligatorisch.

   >[!NOTE]
   >
   >Sie können auch manuell Daten in die Eingabefelder eintragen.

1. Führen Sie einen der folgenden Schritte aus:

   * Um Ihre Einstellungen ohne Generierung der XML-Datei zu speichern, klicken Sie auf **[!UICONTROL Speichern]**.
   * Um die Datei zu speichern und zu generieren, klicken Sie auf **[!UICONTROL Speichern &amp; Generieren]**.

      Die XML-Datei wird erstellt und in das Auftragsprotokoll eingetragen. Video-Sitemap-Dateien (video-sitemap) und Media RSS (mRSS)-Feed-Dateien (mrss-feed) werden im Stammordner Ihres Unternehmens gespeichert.

>[!NOTE]
>
>Veröffentlichen Sie die Video-Sitemap oder den mRSS-Feed, bevor Sie sie an Suchmaschinen senden können. Video-Sitemap- und Media RSS (mRSS)-Feed-Dateien werden im Stammordner des Unternehmens gespeichert. Markieren Sie diese XML-Dateien ggf. zur Veröffentlichung und klicken Sie auf **[!UICONTROL Publish]**.

## Übermitteln von Video-Sitemap- und mRSS-Feed-Dateien an Suchmaschinen {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Video-Sitemap- und Media RSS (mRSS)-Feed-Dateien werden im Stammordner des Unternehmens gespeichert:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Kopieren Sie eine dieser URLs in die Webmaster-Tools einer Suchmaschine, um Ihre Video-Sitemap- oder Media RSS (mRSS)-Feed-Datei an diese Suchmaschine zu übermitteln.

## Anzeigen von Berichten für Video SEO  {#viewing-video-seo-reports}

Ansicht Video SEO-Berichte auf der Seite &quot;Video Search Engine Optimization Report&quot;. Um diese Seite zu öffnen, klicken Sie in der Symbolleiste für globale Navigation auf **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Berichte]**.

Wenn bei der Berichterstellung Fehler aufgetreten sind, werden diese auf der Berichtsseite aufgelistet.
