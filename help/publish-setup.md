---
title: Veröffentlichungseinstellungen
seo-title: Veröffentlichungseinstellungen
description: 'null'
seo-description: Die Einstellungen im Anzeigebereich "Veröffentlichungseinstellungen"bestimmen, wie Assets standardmäßig von den Servern von Dynamic Media Classic an Websites oder Anwendungen gesendet werden.
uuid: 196f25c8-abf5-4c5d-8f6f-bc70007a0301
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: cba59093-28b6-4490-b838-d942b72ad1ec
translation-type: tm+mt
source-git-commit: df88ca77d3f9c40c59d796e6854942b93cef5729
workflow-type: tm+mt
source-wordcount: '2421'
ht-degree: 64%

---


# Veröffentlichungseinstellungen {#publish-setup}

Die Einstellungen im Anzeigebereich &quot;Veröffentlichungseinstellungen&quot;bestimmen, wie Assets standardmäßig von den Servern von Dynamic Media Classic an Websites oder Anwendungen gesendet werden. Wenn keine Einstellung angegeben ist, stellt der Server für dynamische Medien Classic ein Asset gemäß einer Standardeinstellung im Anzeigebereich &quot;Veröffentlichungseinstellungen&quot;bereit. Bei der Anforderung zum Senden eines Bilds, in der beispielsweise kein Auflösungswert angegeben ist, wird das Bild mit der Auflösung gesendet, die im Anzeigebereich „Image-Server“ als Wert für „Standardobjektauflösung“ angegeben ist.

Administratoren können die Standardeinstellungen in den Anzeigebereichen „Image-Server“, „Bild-Renderer“ und „Vignette“ ändern, um festzulegen, wie Assets standardmäßig von den Servern gesendet werden.

Um den Anzeigebereich „Veröffentlichungseinstellungen“ zu öffnen, wählen Sie „Einstellungen“ > „Administrationseinstellungen“ > „Veröffentlichungseinstellungen“.

>[!NOTE]
>
>Die Optionen im Anzeigebereich „Veröffentlichungseinstellungen“ sollten nur von erfahrenen Website-Entwicklern und Programmierern geändert werden. Bei Dynamic Media Classic wird davon ausgegangen, dass Benutzer, die Einstellungen auf diesen Bildschirmen ändern, mit Dynamic Media Classic, den Standards und Konventionen des HTTP-Protokolls und der grundlegenden Imaging-Technologie vertraut sind.

## Image-Server {#image-server}

Im Anzeigebereich „Image-Server“ werden Standardeinstellungen für das Senden von Bildern von den Image-Servern festgelegt. Es sind Einstellungen in den folgenden fünf Kategorien verfügbar (detaillierte Beschreibungen der Einstellungen finden Sie direkt im Anzeigebereich „Image-Server“):

Ändern Sie diese Einstellungen nur mithilfe des Support-Mitarbeiters von Dynamic Media Classic.

**Katalogverwaltung** Diese Einstellungen bestimmen die Interaktion von Dynamic Media Classic und dem Katalog. Anders als bei den meisten Webservern gehen URL-Aufrufe des dynamischen Medienservers an eine Manifest- oder Katalogdatei und nicht an eine Bilddatei. Die Katalogdatei (nicht zu verwechseln mit einem E-Katalog) enthält eine Liste mit dem gesamten Inhalt, der auf dem Image-Server veröffentlicht wurde, und den Pfaden aller Bilddateien. Wenn Sie über eine Digimarc-ID verfügen, geben Sie Ihre Benutzerdaten im Abschnitt „Benutzerinformationen für Digimarc“ ein.

**Anforderungsattribute** Diese Einstellungen setzen Beschränkungen für Bilder fest, die vom Server bereitgestellt werden können. Beispielsweise ist die maximale ** Antwortbildgröße **[!UICONTROL auf]** Breite **[!UICONTROL 5000 und]** Höhe **** 5000 begrenzt.

**Standardmäßige Anforderungsattribute** Diese Einstellungen beziehen sich auf das standardmäßige Erscheinungsbild von Bildern.

**Allgemeine Attribute** für Miniaturansichten Diese Einstellungen beziehen sich auf das Standardbild und die Ausrichtung von Miniaturbildern.

**Standardwerte für Katalogfelder** Diese Einstellungen beziehen sich auf die Auflösung und den Standard-Miniaturansichtstyp von Bildern.

**Farbmanagementattribute** Diese Einstellungen bestimmen, welche ICC-Profil verwendet werden.

**Kompatibilitätsattribute** Mit dieser Einstellung können führende und nachgestellte Absätze in Textebenen wie in Version 3.6 behandelt werden, um die Abwärtskompatibilität zu gewährleisten.

**Unterstützung** von lokale Anpassungen Mit diesen Einstellungen können Sie mehrere Gebietsschemaattribute verwalten. Damit können Sie außerdem eine Zeichenfolge für Gebietsschemakarten angeben, um zu definieren, welche Sprachen Sie für die verschiedenen QuickInfos in den Viewern unterstützen möchten.

Wenn Sie beispielsweise eine multinationale Marke sind mit Vertrieb in verschiedenen Ländern, können Sie sicherstellen, dass jedes Land seinen eigenen Gebietsschema-spezifischen Viewer hat. Für diese Funktion geben Sie eine Zeichenfolge für Gebietsschemakarten an. Bearbeiten Sie anschließend den QuickInfo-Text in der Vorgabe eines Viewer, indem Sie die übersetzten Zeichenfolgen für die gewünschte Sprache hinzufügen. 

>[!NOTE]
> Um die Support-Optionen für Lokale Anpassungen einzurichten, [verwenden Sie die Admin Console, um einen Support-Fall zu erstellen.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) Wenn Sie Unterstützung benötigen, bitten Sie um Hilfe beim Setup.

Weitere Informationen zum Einrichten von **Lokalisierungsunterstützung** finden Sie unter [Betrachtungen beim Planen der Asset-Lokalisierung](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Betrachtungen beim Planen der Asset-Lokalisierung {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Wenn Sie Optionen zur Unterstützung von Lokale Anpassungen in Dynamic Media Classic einrichten möchten, z. B. das Feld &quot;Gebietsschemakarte&quot;, [verwenden Sie die Admin Console, um eine Unterstützungsaktion zu erstellen.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) Wenn Sie Unterstützung benötigen, bitten Sie um Hilfe beim Setup.

Eine gängige Möglichkeit zur Verwendung von Dynamic Media Classic besteht darin, die Produktbilder auf E-Commerce-Websites zu verwalten. Internationale Unternehmen haben das Problem, dass Assets für ähnliche Produkte je nach Land ganz anders aussehen. Normalerweise betreffen die Unterschiede nur sehr wenige Bereiche des gesamten Mediums. Es ist unglaublich aufwändig, aufgrund dieser Unterschiede sämtliche Assets für jedes der Länder zu kopieren und nur die Unterschiede zu überschreiben. Dies widerspricht der Metapher von einem Master-Asset. Solche Unterschiede bei Assets können von länderspezifischen Videos mit verschiedenen Audiospuren bis zu minimalen aber wichtigen Unterschieden bei einem Netzkabel reichen, das im Lieferumfang des Produkts enthalten ist. Dynamic Media Classic verwendet einen grundlegenden Suchmechanismus. Sie definieren eine Reihenfolge der Asset-Suffixe, in denen Image Server beginnend mit dem erforderlichen Gebietsschema sucht.

**So werden Assets lokalisiert**

Das Gebietsschema für eine IS-Anfrage (Image Serving) wird mit dem folgenden IS/IR-Befehl (Image Rendering) identifiziert:

`locale=`

Dieser Befehl akzeptiert eine Zeichenfolge mit der Gebietsschema-ID (locId), bei der die Groß- und Kleinschreibung nicht berücksichtigt werden muss. Bei der Gebietsschema-ID handelt es sich im Allgemeinen um eine Zeichenfolge mit 2-6 Zeichen, die aus Buchstaben und „_“ besteht.

IS supports arbitrary printable ASCII strings.The `locale=` command has a global scope, meaning that it is applied to the entire request, including all nested IS and IR requests, referenced templates, and image layers. Mehrere Gebietsschemas pro Abfrage, wie ein verschiedenes Gebietsschema für jede Ebene, werden nicht unterstützt. Es ist jedoch denkbar, explizite Überschreibvorgänge in verschachtelten Abfragen zuzulassen.

If `locale=` is not specified, `attribute::DefaultLocale` is passed to the translation engines. Limited input validation is applied to the `locale=` value. Empty `locale=` values are permitted. Because `locale=` has a global scope, `attribute::DefaultLocale` is provided by the main catalog for the entire request.

Some of the benefits of using `locale=` and `attribute::DefaultLocale` include the following:

* Freigeben von Inhalten für mehrere Gebietsschemas.
* Zugriff auf Gebietsschema-spezifische Inhalte mit generischen IDs.
* Zulassen von Flexibilität bei Benennungskonventionen und Verwaltung Gebietsschema-spezifischer Inhalte wie Gebietsschema-Präfix und -Suffix oder Gebietsschema-spezifischer Inhalte in einem separaten Katalog.
* Unterstützung für direkten Zugriff auf Gebietsschema-spezifische Versionen.
* Sammelobjekte wie Bildsets können generische Verweise auf möglicherweise Gebietsschema-spezifische Inhalte enthalten.
* Unterstützt alle von Katalogen verwaltete Inhalte, die unter Umständen lokalisiert werden müssen, einschließlich Bildern, Bildsets, Vignetten, Materialien und Viewer-Konfigurations-Datensätzen.
* Minimieren von Änderungen an der IPS-Datenbank und IS-Manifestmechanismen.
* Unterstützung für statische Inhalte wie Videos und Skins wird bei der Implementierung von RFC IS-63 hinzugefügt.
* Das Standard-Gebietsschema kann konfiguriert werden.

**Anwendungsszenarios**

| Anwendung | Szenario |
|--- |--- |
| Viewer-Lokalisierung | Nachdem statische Inhaltskataloge implementiert wurden, wird die Lokalisierung ausschließlich mit dem Parameter locale= gesteuert, der an alle durchgeführten IS-Abfragen angehängt wird. Konfigurationsdatensätze, Skins, Splashscreens usw. können über Gebietsschema-spezifische Varianten verfügen. Der korrekte Inhalt wird über IS bereitgestellt, ohne dass der Viewer wissen muss, welche Inhalte lokalisiert sind und wie die entsprechenden IDs lauten. |
| Bilder und Videos | Internationale Konzerne verwenden häufig eine Mischung aus generischen und Gebietsschema-spezifischen Inhalten. Mit diesem Mechanismus kann ein Verweis auf ein Bild oder Video generisch sein. Und IS stellt die Gebietsschema-spezifischen Inhalte bereit, sofern diese vorhanden sind. |
| Bildsätze und Mediensets | Der gesamte Bildsatz kann für einige Gebietsschemata unterschiedlich sein - z. B. wenn ein E-Katalog komplett anders ist -, wobei die Übersetzung von einem generischen zu einem gebietsschemaspezifischen Bildsatz vom Viewer verarbeitet wird. In der Regel beziehen sich einzelne IDs in einem generischen Satz auf lokalisierte Inhalte. Die meisten Fotos eines Geräts, bis auf das Foto des Bedienfeldes, können beispielsweise in allen Sprachen verwendet werden. IS übersetzt automatisch IDs, sodass keine Gebietsschema-spezifischen Bildsets erstellt werden müssen. |

**Implementieren von Asset-Lokalisierung**

Dynamic Media Classic und Image Serving verfügen über eine Oberfläche, die die lokale Anpassung von Bildern und statischen Inhalten ermöglicht.

Ohne Lokalisierung sieht eine Image Server-URL wie folgt aus:

`https://server/is/image/company/image`

With localization, an Image Server URL adds the `locale=` parameter to the path, as in the following:

`https://server/is/image/company/image?locale=de_DE`

On receipt of the http call by the Image Server, the `locale=` parameter is parsed through the localeMap field found in **Setup** > **Application Setup** > **Publish Setup** > **Image Server** > **Localization Support** group.

Das Feld „Gebietsschemakarte“ enthält eine Liste mit Einträgen, die durch einen senkrechten Strich (|) getrennt sind.

Jeder Eintrag besteht aus einer durch Kommas getrennten Liste von Werten. The first value is the search value that is passed by the `locale=` parameter. Bei den verbleibenden Werten handelt es sich um Suffix-/Ersetzungswerte, die nachfolgend verwendet werden, bis einer davon zu einem vorhandenen Bild führt.

Ob ein Suffixwert oder ein Ersetzungswert angewendet wird, hängt von der Einstellung „Globales Gebietsschema“ in der Gruppe **Einstellungen** > **Anwendungseinstellungen** > **Veröffentlichungseinstellungen** > **Image-Server** > **Lokalisierungsunterstützung** ab.

>[!NOTE]
>
>Die Einstellung &quot;Globales Gebietsschema&quot;ist derzeit nur möglich, wenn Sie sie über die API festlegen, nicht über die Benutzeroberfläche von Dynamic Media Classic.

**Beispiel für ein Suffix**

| URL | localeMap-IDs | Ergebnis |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | Beachten Sie, dass kein GlobalLocale definiert ist. Der Gebietsschema-Parameter de_DE wird mit dem ersten Eintrag in der localeMap abgeglichen. Der erste entsprechende Wert _DE wird dem Asset als Suffix angehängt image_DE und er wird auf dem Image-Server gesucht. Wenn er auf dem Server gefunden wird, wird er zurückgegeben. Andernfalls wird der zweite Wert „“ als Suffix verwendet, wodurch das Bild selbst zurückgegeben wird. |

**Beispiel für eine Ersetzung**

| URL | GlobalLocale- und localeMap-IDs | Ergebnis |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | Im Ersetzungsbeispiel oben ist GlobalLocale auf main eingestellt. Der Gebietsschema-Parameter de_DE wird mit dem ersten Eintrag in der localeMap abgeglichen. Der GlobalLocale-Teilstring wird gefunden und durch den ersten entsprechenden Wert in localeMap ersetzt: image-de-01. Wenn er auf dem Image-Server gefunden wird, wird er zurückgegeben. Andernfalls wird der zweite Wert ersetzt, was zu image-main-01 führt. |

Wenn in der URL kein Gebietsschema definiert ist, verwendet der Image-Server DefaultLocale, sofern definiert, und wendet es auf die URL an.

If an unknown or empty locale parameter is supplied with `locale=`, then the localeMap is scanned for the empty value “starting with,”. Es ist wichtig, diese Option so zu konfigurieren, dass für nicht bekannte Gebietsschemas ein Standard-Gebietsschema angewendet wird.

**defaultImage**

Der Image-Server versucht nacheinander, die Optionen für das angeforderte Gebietsschema zu verwenden. Wenn keine Übereinstimmung gefunden wird, werden die Gebietsschema-Optionen auf das defaultImage angewendet und die übereinstimmende Version wird zurückgegeben. Daher sollte entweder jedes Gebietsschema eine Option für das Bild ohne lokale Anpassung enthalten oder die lokalisierten defaultImage-Versionen sollten in Dynamic Media Classic verfügbar sein.

**Szenarios für die Suche nach der localeMap**

Angenommen, Sie möchten die folgenden Gebietsschemas unterstützen:

`en, en_us, en_uk, de, de_at, de_de, fr`

You map these locales to the suffixes `_E`, `_G`, and `_F`, for English, German, and French, respectively. Bei allen Beispielen lautet die generische Eingabebild-ID `myImg`.

*Standardverhalten bei der Suche nach der localeMap*

Die Gebietsschema-IDs werden den entsprechenden Suffixen zugeordnet. Wenn keine Gebietsschema-spezifische ID im Katalog gefunden wird, wird die generische ID verwendet. Beachten Sie die leeren locSuffix-Werte, die der generischen ID zugeordnet sind.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | Zu durchsuchende Ausgabe-IDs |
|--- |--- |
| en,en_us, en_uk | myImg_E,myImg |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| Alle anderen | - |

*Suchen der localeMap bei unbekanntem Gebietsschema*

Sie können unbekannte Gebietsschemas bestimmten IDs oder generischen IDs zuordnen. Beispiel: Sie können unbekannte Gebietsschemas den englischen IDs zuordnen oder, wenn diese nicht vorhanden sind, den generischen IDs.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | Zu durchsuchende Ausgabe-IDs |
|--- |--- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| Alle anderen | myImg_E,myImg |

You could also have a dedicated locSuffix, such as U, just for unknown locales, and force to the default image if no `_U` exists, as in the following:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Oder Sie können wie im folgenden Beispiel direkt die generische ID zuordnen:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

*Suchen der localeMap mit einer mehrstufigen Suche*

Häufig ist es hilfreich, Gebietsschemas zu gruppieren, z. B. nach den Regionen Europa, Naher Osten und Nordamerika, um so regionalen Standards wie Sonneneinstrahlung zu berücksichtigen. Diesen Effekt erzielen Sie mit einer mehrstufigen Suche.

In diesem Beispiel gehen wir davon aus, dass Sie Sammlungen für die Verwendung in Europa und den USA bzw. im Nahen Osten unterstützen möchten. Beide Sammlungen basieren auf der generischen Bildsammlung und in beiden werden einige Bilder hinzugefügt oder angepasst. Both collections are then further refined for specific locales, such as `m1, m2` for two middle-eastern variants, and `w1, w2,` and `w3` for three Western locales, except that images are shared for `w1` and `w3`. Unbekannte Gebietsschemas sind nur der generischen Sammlung zugeordnet und haben keinen Zugriff auf Gebietsschema-spezifische Bilder. Die Karte würde wie folgt aussehen:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | Zu durchsuchende Ausgabe-IDs |
|--- |--- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| Alle anderen | mylmg |

*Suchen der localeMap über die Suche nach bestimmten IDs*

Einige Bildbenennungskonventionen unterstützen unter Umständen keine generischen Bild-IDs. Die generischen IDs aus der Abfrage müssen einer bestimmten ID im Katalog zugeordnet werden. In einigen Fällen ist die exakte spezifische ID jedoch unter Umständen unbekannt.

Using the first example as a basis, images for all languages may have the suffixes `_1`, `_2`, or `_3`. Images that are specific to French locales may have the suffixes `_22` or `_23` suffix. And images that are specific to German locales may have the suffixes `_470` or `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | Zu durchsuchende Ausgabe-IDs |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Alle anderen | myImg_1, myImg_2, myImg_3 |

**Wichtige Überlegungen bei der Implementierung von Lokalisierungsunterstützung**

* Die Lokalisierung ist auf ID-basierte Asset-Abrufe beschränkt und kann nicht für pfadbasierte Asset-Abrufe verwendet werden. Wenn also Videos mit einem Gebietsschema abgerufen werden sollen, müssen sie als Unternehmens-/Asset-ID abgerufen werden, nicht über den vollständigen Pfad zum Video. Dies bedeutet, dass Sie rtmp bei der Lokalisierung nicht verwenden können, da bei dieser Methode nur pfadbasierte Videoabrufe möglich sind.
* Sie können kein gemischtes Medienset verwenden, das ein einzelnes Video enthält, wenn localeMap aktiv ist. Andernfalls schlägt der Abruf der Set-Inhalte fehl. Im dieses Problem zu umgehen, können Sie einem adaptiven Videoset ein einzelnes Video hinzufügen. Fügen Sie das adaptive Videoset anschließend einem gemischten Medienset hinzu.
* Bestimmte Abfragen sind nicht lokalisiert. Dies gilt beispielsweise für die Abfrage der Inhalte eines adaptiven Videosets. Wenn Sie also adaptive Videosets mit Lokalisierung verwenden möchten, müssen Sie das adaptive Videoset in einem gemischten Medienset platzieren. Then, call the set into a Mixed Media viewer with the `locale=` parameter.

## Bild-Renderer {#image-renderer}

Im Anzeigebereich „Bild-Renderer“ werden Standardeinstellungen für das Senden von Bildern von den Bild-Renderer-Servern festgelegt. Es sind Einstellungen in den folgenden fünf Kategorien verfügbar (detaillierte Beschreibungen der Einstellungen finden Sie direkt im Anzeigebereich „Image-Server“):

**Katalogverwaltung** Diese Einstellungen bestimmen, wie Dynamic Media Classic und die Katalogdatei interagieren. URL-Aufrufe des Dynamic Media Classic Render-Servers werden an den Katalog gesendet, der wiederum Aufrufe zur Bereitstellung von Bildern vom Server ausführt. Ändern Sie diese Einstellungen nur mithilfe des Support-Mitarbeiters von Dynamic Media Classic.

**Sitzungsattribute** Mit diesen Einstellungen werden Fehlerparameter, die URL für relative Bild-URLs und die Zulässigkeit von überlappenden Objekten festgelegt.

**Standardmäßige Materialattribute** Diese Einstellungen legen Standardeinstellungen für Auflösung und Scharfzeichnung für Bilder fest.

**Attribute** des Antwortbilds Diese Einstellungen beziehen sich auf das standardmäßige Erscheinungsbild von Bildern.

**Farbmanagementattribute** Diese Einstellungen beziehen sich auf die Standardfarbeinstellungen von Bildern.

## Vignette {#vignette}

Der Anzeigebereich „Vignette“ enthält Einstellungen zum Festlegen der standardmäßigen Darstellung von Vignetten (eine detaillierte Beschreibung der Optionen finden Sie im Anzeigebereich selbst).
