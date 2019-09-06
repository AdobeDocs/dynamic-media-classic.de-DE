---
title: Video SEO
seo-title: Video SEO
description: 'null'
seo-description: Erfahren Sie, wie Sie Video SEO-Einstellungen konfigurieren.
uuid: bac 2 c 6 a 9-8466-4 b 8 f-b 835-6 cb 0 b 4168513
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/setup
discoiquuid: 34 ecd 668-775 f -452 b-b 26 e-d 139 f 0 e 280 ae
translation-type: tm+mt
source-git-commit: de7d2608f94935f238a11d8310b97dddc5476f57

---


# Video SEO{#video-seo-search-engine-optimization}

Die Suchmaschinenoptimierung (SEO) ist ein Vorgang, der die Erhöhung der Zugriffe auf eine Website über Suchmaschinen zum Ziel hat. Suchmaschinen zeigen beim Sammeln von Informationen zu textbasierten Inhalten ausgezeichnete Leistung. Bei Videoinhalten können sie jedoch nur dann zufriedenstellende Informationen aufweisen, wenn diese direkt in die Suchmaschine eingespeist werden.

Mit Dynamic Media Classic Video SEO können Sie Videometadaten nutzen, um Suchmaschinen mit Beschreibungen Ihrer Videos bereitzustellen. Mit Dynamic Media Classic können Sie Video-Sitemaps und mrss-Feeds erstellen. Bei diesen Formaten handelt es sich um standardmäßige XML-Dateien, mit denen Videoinformationen an Suchmaschinen übermittelt werden:

**Video-Sitemap** informiert Google genau darüber, wo sich der Videoinhalt auf einer Site befindet. In der Folge sind die Videos vollständig auf Google suchbar. Eine Video-Sitemap kann beispielsweise die Laufzeit und Kategorien von Videos angeben. Weitere Informationen zu Video-Sitemaps finden Sie unter https://www.google.com/support/webmasters/bin/answer.py?answer=80471.

**Mrss (Media Really Simple Syndication) Feed** , der von Herausgebern von Inhalten verwendet wird, um Mediendateien in Yahoo! zu speisen! Videosuche einzuspeisen. Weitere Informationen zu mrss-Feeds finden Sie unter https://www.rssboard.org/media-rss.

>[!NOTE]
>
>Google unterstützt sowohl das Video-Sitemap- als auch das mRSS-Feed-Protokoll für die Übermittlung von Informationen an Suchmaschinen.

Dynamic Media Classic kann Video-Sitemaps und mrss-Feeds aus den mit jedem Video gespeicherten Metadaten generieren. Beim Erstellen von Video-Sitemaps und mRSS-Feeds können Sie wählen, welche Metadatenfelder der Videos eingeschlossen werden sollen. Auf diese Weise beschreiben Sie Suchmaschinen Ihre Videos, damit diese Besucher treffsicherer zu Videos auf Ihrer Website leiten können.

>[!NOTE]
>
>Ermitteln Sie vor der Erstellung einer Video-Sitemap oder eines mRSS-Feeds, welche Felder die XML-Datei für die Suchmaschine enthalten muss und wie diese Felder strukturiert sein müssen. Gute Video-Sitemaps oder mRSS-Feeds müssen die Anforderungen der Suchmaschine erfüllen.

Dynamic Media Classic erstellt Berichte zu Video-Sitemaps und mrss-Feeds, nachdem Sie sie generiert haben. Diese Berichte sind im Anzeigebereich „Bericht für Video SEO“ verfügbar.

>[!NOTE]
>
>Bei Video-Sitemaps und mrss-Feeds erfasst Dynamic Media Classic nur Metadaten aus Videos, die zur Veröffentlichung markiert sind. Markieren Sie Videos zur Veröffentlichung, um ihre Metadaten in Video-Sitemaps und mRSS-Feeds einzuschließen.

## Choosing video SEO settings {#choosing-video-seo-settings}

Wählen Sie im Anzeigebereich „Einstellungen für Video SEO“ die Video SEO-Einstellungen für Video-Sitemaps und mRSS-Feeds aus. Wählen Sie „Einstellungen“ &gt; „Anwendungseinstellungen“ &gt; „Video SEO“ &gt; „Einstellungen“, um diesen Anzeigebereich zu öffnen.

Wählen Sie im Bereich „Allgemeine Einstellung“, ob Video-Sitemaps, mRSS-Feeds oder beides erstellt werden sollen. Verknüpfen Sie im Bereich „Erstellungseinstellungen“ Metadatenfelder mit Eingabefeldern.

Wenn Sie die gewünschten Einstellungen ausgewählt haben, klicken Sie auf „Erstellen“ (oder „Speichern &amp; Erstellen“), um die Video-Sitemap, das mRSS-Feed oder beide zu erstellen.

### Auswählen von allgemeinen Einstellungen {#choosing-general-settings}

Wählen Sie in der Dropdown-Liste „Erstellungsmodus“ einen Berichtsmodus:

**Video Sitemap** Erstellen Sie eine Video-Sitemap.

**Mrss Feed** Erstellen Sie einen Media RSS (mrss)-Feed.

**Beide** erstellen beide XML-Dateien.

**Deaktivieren Sie** diese Option, um die Erstellung von Video-Sitemaps und Media RSS (mrss)-Feeds zu stoppen.

Wählen Sie in der Dropdown-Liste „Automatischer Modus“ bzw. „Manueller Modus“, ob die Erstellung automatisch oder manuell erfolgen soll:

**Automatischer Modus** Dynamic Media Classic erstellt jeden Tag automatisch eine Video-Sitemap, einen Media RSS (mrss)-Feed oder beides. Wählen Sie die Option "Zur Veröffentlichung markieren" , um die XML-Datei automatisch zur Veröffentlichung durch Dynamisches Media Classic zu markieren.

**Der manuelle Modus** für dynamische Medien erstellt die Video-Sitemap, den Media RSS (mrss)-Feed oder beides, wenn Sie im Anzeigebereich "Einstellungen für die Videosuche" auf" Erstellen" oder "Speichern &amp; Erstellen" klicken. Wählen Sie außerdem aus den folgenden Optionen:

**Keine weitere Einstellungen** zur Veröffentlichung der generierten XML-Datei markiert.

**Markieren Sie zur Veröffentlichung die zu veröffentlichende** XML-Datei.

**Suchmaschinen mit partiellen Generierung** können eine XML-Datei ablehnen, wenn sie keine vollständigen Metadateninformationen für alle Videos enthält. Mit dieser Option wird die XML-Datei erstellt, selbst wenn für einige Videos keine Metadaten verfügbar sind. Im Anzeigebereich „Bericht“ wird eine Warnung registriert. Wählen Sie diese Option, wenn Sie die XML-Datei exportieren und die fehlenden Informationen manuell bearbeiten möchten.

### Auswählen von Erstellungseinstellungen {#choosing-generation-settings}

Im Bereich „Erstellungseinstellungen“ sind Eingabefelder für die Video-Sitemap und/oder das mRSS-Feed aufgeführt, im Metadatenbedienfeld sind die Namen der Metadatenfelder aufgeführt. Verwenden Sie den Bereich „Allgemeine Einstellungen“, um Eingabefelder und Metadatenfelder zu verknüpfen. Auf diese Weise teilen Sie Dynamischer Media Classic mit, wo Metadaten für die Video-Sitemap und/oder mrss-Feed abgerufen werden sollen.

1. Wählen Sie im Menü „Metadaten-Ansichten“ eine Metadaten-Ansicht. Wenn Sie eine Ansicht ausgewählt haben, werden die Namen der Metadatenfelder im Metadatenbedienfeld angezeigt. (Weitere Informationen zu Metadaten-Ansichten finden Sie unter [Metadaten-Ansichten](application-setup.md#metadata_views).)
1. Ziehen Sie die Metadatenfeldnamen vom Metadatenbedienfeld zu den Eingabefeldern „Startseite“, „Titel“, „Beschreibung“, „Tags“ und „Kategorie“. Die Felder „Startseite“, „Titel“ und „Beschreibung“ sind obligatorisch.

   >[!NOTE]
   >
   >Sie können auch manuell Daten in die Eingabefelder eintragen.

1. Klicken Sie auf „Speichern“ (um die Einstellungen zu speichern, ohne die XML-Datei zu erstellen), „Erstellen“ (um die XML-Datei zu erstellen) oder „Speichern &amp; Erstellen“ (um zu speichern und die Datei zu erstellen).

   Die XML-Datei wird erstellt und in das Auftragsprotokoll eingetragen. Video-Sitemap-Dateien (video-sitemap) und Media RSS (mRSS)-Feed-Dateien (mrss-feed) werden im Stammordner Ihres Unternehmens gespeichert.

>[!NOTE]
>
>Sie müssen die Video-Sitemap oder das mRSS-Feed veröffentlichen, bevor Sie die Datei an Suchmaschinen übermitteln können. Video-Sitemap- und Media RSS (mRSS)-Feed-Dateien werden im Stammordner des Unternehmens gespeichert. Markieren Sie diese XML-Dateien gegebenenfalls zur Veröffentlichung und klicken Sie auf die Schaltfläche „Veröffentlichen“.

## Übermitteln von Video-Sitemap- und mRSS-Feed-Dateien an Suchmaschinen {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

Video-Sitemap- und Media RSS (mRSS)-Feed-Dateien werden im Stammordner des Unternehmens gespeichert:

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

Kopieren Sie eine dieser URLs in die Webmaster-Tools einer Suchmaschine, um Ihre Video-Sitemap- oder Media RSS (mRSS)-Feed-Datei an diese Suchmaschine zu übermitteln.

## Anzeigen von Berichten für Video SEO {#viewing-video-seo-reports}

Zeigen Sie Video SEO-Berichte im Anzeigebereich „Bericht für Video SEO“ an. Um diesen Anzeigebereich zu öffnen, klicken Sie auf "Einstellungen" &gt;" Anwendungseinstellungen" &gt; "Video SEO" &gt;" Berichte" .

Wenn bei der Erstellung des Berichts Fehler aufgetreten sind, werden diese im Anzeigebereich „Bericht“ aufgeführt.
