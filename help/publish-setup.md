---
title: Veröffentlichungseinstellungen
description: Mit den Einstellungen für Veröffentlichungseinstellungen können Sie festlegen, wie Assets standardmäßig von Dynamic Media Classic-Servern für Websites oder Anwendungen bereitgestellt werden.
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 699d4c12-e47b-4c6b-86f3-dc7aaaa56c1e
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '2403'
ht-degree: 47%

---

# Veröffentlichungseinstellungen {#publish-setup}

Die Einstellungen der Seite &quot;Veröffentlichungseinstellungen&quot;bestimmen, wie Assets standardmäßig von Dynamic Media Classic-Servern für Websites oder Anwendungen bereitgestellt werden. Wenn keine Einstellung festgelegt ist, stellt der Dynamic Media Classic-Server ein Asset gemäß einer Standardeinstellung auf der Seite &quot;Veröffentlichungseinstellungen&quot;bereit. Beispielsweise liefert eine Anfrage zum Bereitstellen eines Bildes, das kein Auflösungsattribut enthält, ein Bild mit der Einstellung &quot;Standardobjektauflösung&quot;auf der Image-Server-Seite.

Administratoren können die Standardeinstellungen auf den Seiten Image-Server, Image-Renderer und Vignette ändern, um Standardeinstellungen für die Bereitstellung von Assets von Servern festzulegen.

Um die Seiten zur Veröffentlichungseinstellungen zu öffnen, klicken Sie auf **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Veröffentlichungseinrichtung]**.

>[!NOTE]
>
>Die Seiten zur Veröffentlichungseinstellungen sind für erfahrene Website-Entwickler und -Programmierer geeignet. Dynamic Media Classic geht davon aus, dass Benutzer, die die Einstellungen auf diesen Seiten ändern, mit Dynamic Media Classic, den HTTP-Protokollstandards und -Konventionen und der grundlegenden Imaging-Technologie vertraut sind.

## Image-Server {#image-server}

Auf der Image-Server-Seite werden Standardeinstellungen für die Bereitstellung von Bildern von Image-Servern festgelegt. Einstellungen sind in diesen fünf Kategorien verfügbar (detaillierte Beschreibungen der Einstellungen finden Sie auf der Image-Server-Seite selbst ).

Ändern Sie diese Einstellungen nur mithilfe eines Dynamic Media Classic-Support-Mitarbeiters.

* **Katalogverwaltung**  - Diese Einstellungen bestimmen, wie Dynamic Media Classic und der Katalog interagieren. Im Gegensatz zu den meisten Webservern gehen Dynamic Media Image Server-URL-Aufrufe an eine Manifest- oder Katalogdatei und nicht an eine Bilddatei. Die Katalogdatei (nicht zu verwechseln mit einem E-Katalog) enthält eine Liste mit dem gesamten Inhalt, der auf dem Image-Server veröffentlicht wurde, und den Pfaden aller Bilddateien. Wenn Sie über eine Digimarc-ID verfügen, geben Sie Ihre Benutzerdaten im Abschnitt „Benutzerinformationen für Digimarc“ ein.

* **Anfrage-Attribute** : Mit diesen Einstellungen werden Einschränkungen für Bilder festgelegt, die vom Server bereitgestellt werden können. Beispielsweise ist *maximum* **[!UICONTROL Maximale Antwortbildgröße]** **[!UICONTROL Breite]** 5000 und **[!UICONTROL Höhe]** 5000.

* **Standardattribute für Anfragen**  - Diese Einstellungen beziehen sich auf das standardmäßige Erscheinungsbild von Bildern.

* **Allgemeine Attribute für Miniaturansichten** : Diese Einstellungen beziehen sich auf die standardmäßige Darstellung und Ausrichtung von Miniaturbildern.

* **Standardeinstellungen für Katalogfelder**  - Diese Einstellungen beziehen sich auf die Auflösung und den Standardtyp für Miniaturansichten von Bildern.

* **Farbverwaltungsattribute**  - Diese Einstellungen bestimmen, welche ICC-Farbprofile verwendet werden.

* **Kompatibilitätsattribute**  - Mit dieser Einstellung können führende und nachfolgende Absätze in Textebenen aus Gründen der Abwärtskompatibilität wie in Version 3.6 behandelt werden.

* **Lokalisierungsunterstützung**  - Mit diesen Einstellungen können Sie mehrere Gebietsschemaattribute verwalten. Damit können Sie außerdem eine Zeichenfolge für Gebietsschemakarten angeben, um zu definieren, welche Sprachen Sie für die verschiedenen QuickInfos in den Viewern unterstützen möchten.

   Wenn Sie beispielsweise eine multinationale Marke sind mit Vertrieb in verschiedenen Ländern, können Sie sicherstellen, dass jedes Land seinen eigenen Gebietsschema-spezifischen Viewer hat. Für diese Funktion geben Sie eine Zeichenfolge für Gebietsschemakarten an. Bearbeiten Sie anschließend den QuickInfo-Text in der Vorgabe eines Viewer, indem Sie die übersetzten Zeichenfolgen für die gewünschte Sprache hinzufügen. 

   >[!NOTE]
   > Verwenden Sie zum Einrichten von Support-Optionen für die Lokalisierung [die Admin Console, um einen Support-Fall zu erstellen.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) In Ihrem Support-Fall fordern Sie Hilfe bei der Einrichtung an.

   Weitere Informationen zum Einrichten von **Lokalisierungsunterstützung** finden Sie unter [Betrachtungen beim Planen der Asset-Lokalisierung](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Betrachtungen beim Planen der Asset-Lokalisierung {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Wenn Sie in Dynamic Media Classic Lokalisierungsunterstützung-Optionen einrichten möchten, z. B. das Feld &quot;Locale Map&quot;, verwenden Sie [die Admin Console, um einen Support-Fall zu erstellen.](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) In Ihrem Support-Fall fordern Sie Hilfe bei der Einrichtung an.

Eine gängige Möglichkeit zur Verwendung von Dynamic Media Classic besteht darin, die Produktbilder auf E-Commerce-Websites zu verwalten. Internationale Unternehmen haben das Problem, dass Assets für ähnliche Produkte je nach Land ganz anders aussehen. Normalerweise sind die Unterschiede für einige Teile der gesamten Medien. Es ist unglaublich aufwändig, aufgrund dieser Unterschiede sämtliche Assets für jedes der Länder zu kopieren und nur die Unterschiede zu überschreiben. Dies widerspricht der Metapher von einem Master-Asset. Solche Unterschiede bei Assets können von länderspezifischen Videos mit verschiedenen Audiospuren bis zu minimalen aber wichtigen Unterschieden bei einem Netzkabel reichen, das im Lieferumfang des Produkts enthalten ist. Dynamic Media Classic verwendet einen grundlegenden Suchmechanismus. Sie definieren eine Reihenfolge der Asset-Suffixe, in denen Image Server beginnend mit dem erforderlichen Gebietsschema sucht.

#### So werden Assets lokalisiert

Das Gebietsschema für eine IS-Anfrage (Image Serving) wird mit dem folgenden IS/IR-Befehl (Image Rendering) identifiziert:

`locale=`

Dieser Befehl akzeptiert eine Zeichenfolge mit der Gebietsschema-ID (locId), bei der die Groß- und Kleinschreibung nicht berücksichtigt werden muss. Bei der Gebietsschema-ID handelt es sich im Allgemeinen um eine Zeichenfolge mit 2-6 Zeichen, die aus Buchstaben und „_“ besteht.

IS unterstützt beliebige druckbare ASCII-Zeichenfolgen. Der Befehl `locale=` hat einen globalen Gültigkeitsbereich, d. h. er wird auf die gesamte Anforderung angewendet, einschließlich aller verschachtelten IS- und IR-Anforderungen, referenzierten Vorlagen und Bildebenen. Mehrere Gebietsschemas pro Abfrage, wie ein verschiedenes Gebietsschema für jede Ebene, werden nicht unterstützt. Es ist jedoch denkbar, explizite Überschreibvorgänge in verschachtelten Abfragen zuzulassen.

Wenn `locale=` nicht angegeben ist, wird `attribute::DefaultLocale` an die Übersetzungs-Engines übergeben. Eingeschränkte Eingabevalidierung wird auf den Wert `locale=` angewendet. Leere `locale=` Werte sind zulässig. Da `locale=` einen globalen Gültigkeitsbereich hat, wird `attribute::DefaultLocale` vom Hauptkatalog für die gesamte Anfrage bereitgestellt.

Zu den Vorteilen der Verwendung von `locale=` und `attribute::DefaultLocale` zählen unter anderem die folgenden:

* Freigeben von Inhalten für mehrere Gebietsschemas.
* Zugriff auf Gebietsschema-spezifische Inhalte mit generischen IDs.
* Zulassen von Flexibilität bei Benennungskonventionen und Verwaltung Gebietsschema-spezifischer Inhalte wie Gebietsschema-Präfix und -Suffix oder Gebietsschema-spezifischer Inhalte in einem separaten Katalog.
* Unterstützung des Zugriffs auf gebietsschemaspezifische Versionen.
* Aggregierte Objekte wie Bildsets können manchmal allgemeine Verweise auf potenziell gebietsschemaspezifische Inhalte enthalten.
* Unterstützt alle Inhalte, die von Katalogen verwaltet werden, die lokalisiert werden müssen, einschließlich Bildern, Bildsets, Vignetten, Materialien und Viewer-Konfigurationsdatensätzen.
* Minimieren von Änderungen an der IPS-Datenbank und IS-Manifestmechanismen.
* Unterstützung für statische Inhalte wie Videos und Skins wird hinzugefügt, wenn RFC IS-63 implementiert ist.
* Das Standard-Gebietsschema kann konfiguriert werden.

#### Anwendungsszenarios

| Anwendung | Szenario |
|--- |--- |
| Viewer-Lokalisierung | Nachdem statische Inhaltskataloge implementiert wurden, wird die Lokalisierung ausschließlich mit dem Parameter locale= gesteuert, der an alle durchgeführten IS-Abfragen angehängt wird. Konfigurationsdatensätze, Skins, Splashscreens usw. können über Gebietsschema-spezifische Varianten verfügen. Der korrekte Inhalt wird über IS bereitgestellt, ohne dass der Viewer wissen muss, welche Inhalte lokalisiert sind und wie die entsprechenden IDs lauten. |
| Bilder und Videos | Internationale Konzerne verwenden häufig eine Mischung aus generischen und Gebietsschema-spezifischen Inhalten. Mit diesem Mechanismus kann ein Verweis auf ein Bild oder Video generisch sein. Und IS stellt die Gebietsschema-spezifischen Inhalte bereit, sofern diese vorhanden sind. |
| Bildsätze und Mediensets | Das gesamte Bildset kann für einige Gebietsschemata unterschiedlich sein, z. B. wenn ein E-Katalog unterschiedlich ist, wobei die Übersetzung von einem generischen in ein gebietsschemaspezifisches Bildset vom Viewer verarbeitet wird. In der Regel können einzelne IDs in einem generischen Satz auf lokalisierte Inhalte verweisen. Beispielsweise können die meisten Fotos eines Geräts in allen Sprachen identisch sein, mit Ausnahme des Fotos des Control Panels. IS übersetzt automatisch IDs, sodass keine Gebietsschema-spezifischen Bildsets erstellt werden müssen. |

#### Implementieren von Asset-Lokalisierung

Dynamic Media Classic und Image Serving verfügen über eine Benutzeroberfläche, die die Lokalisierung von Bildern und statischen Inhalten ermöglicht.

Ohne Lokalisierung sieht eine Image Server-URL wie folgt aus:

`https://server/is/image/company/image`

Bei der Lokalisierung fügt eine Image-Server-URL den Parameter `locale=` wie im folgenden Beispiel zum Pfad hinzu:

`https://server/is/image/company/image?locale=de_DE`

Nach Erhalt des HTTP-Aufrufs durch den Image-Server wird der Parameter `locale=` durch das Feld localeMap geparst, das unter **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Veröffentlichungseinrichtung]** > **[!UICONTROL Image-Server]** > **[!UICONTROL Lokalisierungsunterstützung]** zu finden ist.

Das Feld „Gebietsschemakarte“ enthält eine Liste mit Einträgen, die durch einen senkrechten Strich (|) getrennt sind.

Jeder Eintrag besteht aus einer durch Kommas getrennten Liste von Werten. Der erste Wert ist der Suchwert, der vom Parameter `locale=` übergeben wird. Die verbleibenden Werte sind Suffix-/Ersatzwerte, die dann versucht werden, bis zu einem vorhandenen Bild zu gelangen.

Ob ein Suffixwert oder ein Ersetzungswert angewendet wird, hängt von der Einstellung „Globales Gebietsschema“ in der Gruppe **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Veröffentlichungseinstellungen]** > **[!UICONTROL Image-Server]** > **[!UICONTROL Lokalisierungsunterstützung]** ab.

>[!NOTE]
>
>Die Einstellung &quot;Globales Gebietsschema&quot;ist nur möglich, wenn Sie sie über die API festlegen, nicht über die Benutzeroberfläche von Dynamic Media Classic.

**Beispiel für ein Suffix:**

| URL | localeMap-IDs | Ergebnis |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | Beachten Sie, dass kein GlobalLocale definiert ist. Der Gebietsschema-Parameter de_DE wird mit dem ersten Eintrag in der localeMap abgeglichen. Der erste entsprechende Wert _DE wird dem Asset als Suffix angehängt image_DE und er wird auf dem Image-Server gesucht. Wenn er auf dem Server gefunden wird, wird er zurückgegeben. Andernfalls wird der zweite Wert „“ als Suffix verwendet, wodurch das Bild selbst zurückgegeben wird. |

**Beispiel für eine Ersetzung:**

| URL | GlobalLocale- und localeMap-IDs | Ergebnis |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | Im Ersetzungsbeispiel oben ist GlobalLocale auf main eingestellt. Der Gebietsschema-Parameter de_DE wird mit dem ersten Eintrag in der localeMap abgeglichen. Die GlobalLocale-Unterzeichenfolge wird gefunden und durch den ersten entsprechenden Wert `de` in der localeMap ersetzt: `image-de-01`. Wenn er auf dem Image-Server gefunden wird, wird er zurückgegeben. Andernfalls wird der zweite Wert ersetzt, was zu `image-main-01` führt. |

Wenn in der URL kein Gebietsschema definiert ist, verwendet der Image-Server DefaultLocale, sofern definiert, und wendet es auf die URL an.

Wenn ein unbekannter oder leerer Gebietsschemaparameter mit `locale=` bereitgestellt wird, wird die localeMap auf den leeren Wert &quot;Beginnt mit&quot; gescannt. Es ist wichtig, dass ein standardmäßiges Gebietsschema für unbekannte Gebietsschemata angewendet wird.

#### Über defaultImage

Der Image-Server versucht nacheinander, die Optionen für das angeforderte Gebietsschema zu verwenden. Wenn keine Übereinstimmung gefunden wird, werden die Gebietsschemaoptionen auf defaultImage angewendet und die entsprechende Version wird zurückgegeben. Daher muss entweder jedes Gebietsschema eine Option für das Bild ohne Lokalisierung enthalten oder die lokalisierten defaultImage-Versionen werden in Dynamic Media Classic zur Verfügung gestellt.

#### Szenarios für die Suche nach der localeMap

Angenommen, Sie möchten die folgenden Gebietsschemas unterstützen:

`en, en_us, en_uk, de, de_at, de_de, fr`

Sie ordnen diese Gebietsschemata den Suffixen `_E`, `_G` und `_F` für Englisch, Deutsch und Französisch zu. Bei allen Beispielen lautet die generische Eingabebild-ID `myImg`.

##### Standardverhalten bei der Suche nach der localeMap

Die Gebietsschema-IDs werden den entsprechenden Suffixen zugeordnet. Wenn keine Gebietsschema-spezifische ID im Katalog gefunden wird, wird die generische ID verwendet. Beachten Sie die leeren locSuffix-Werte, die der generischen ID zugeordnet sind.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | Zu durchsuchende Ausgabe-IDs |
|--- |--- |
| en,en_us, en_uk | myImg_E,myImg |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| Alle anderen | - |

##### Suchen der localeMap bei unbekanntem Gebietsschema

Sie können unbekannte Gebietsschemas bestimmten IDs oder generischen IDs zuordnen. Beispielsweise können Sie den englischen IDs unbekannte Gebietsschemata zuordnen oder, falls diese nicht vorhanden sind, den generischen IDs.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | Zu durchsuchende Ausgabe-IDs |
|--- |--- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| Alle anderen | myImg_E,myImg |

Sie können auch ein dediziertes locSuffix wie U für unbekannte Gebietsschemas verwenden und das Standardbild erzwingen, wenn kein `_U` vorhanden ist, wie im folgenden Beispiel:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Oder Sie können wie im folgenden Beispiel direkt die generische ID zuordnen:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### Suchen der localeMap mit einer mehrstufigen Suche

Häufig ist es hilfreich, Gebietsschemas zu gruppieren, z. B. nach den Regionen Europa, Naher Osten und Nordamerika, um so regionalen Standards wie Sonneneinstrahlung zu berücksichtigen. Diesen Effekt erzielen Sie mit einer mehrstufigen Suche.

In diesem Beispiel gehen wir davon aus, dass Sie Sammlungen für die Verwendung in Europa und den USA bzw. im Nahen Osten unterstützen möchten. Beide Sammlungen basieren auf der generischen Bildsammlung und in beiden werden einige Bilder hinzugefügt oder angepasst. Beide Sammlungen werden dann für bestimmte Gebietsschemata weiter verfeinert, z. B. `m1, m2` für zwei mittlere östliche Varianten und `w1, w2,` und `w3` für drei westliche Gebietsschemata, mit der Ausnahme, dass Bilder für `w1` und `w3` freigegeben werden. Unbekannte Gebietsschemas sind nur der generischen Sammlung zugeordnet und haben keinen Zugriff auf Gebietsschema-spezifische Bilder. Die Karte würde wie folgt aussehen:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | Zu durchsuchende Ausgabe-IDs |
|--- |--- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| Alle anderen | mylmg |

##### Suchen der localeMap über die Suche nach bestimmten IDs

Einige Bildbenennungskonventionen unterstützen keine allgemeinen Bild-IDs. Die generischen IDs aus der Abfrage müssen einer bestimmten ID im Katalog zugeordnet werden. Es gibt jedoch Fälle, in denen die genaue spezifische ID nicht bekannt ist.

Anhand des ersten Beispiels können Bilder für alle Sprachen die Suffixe `_1`, `_2` oder `_3` aufweisen. Für französische Gebietsschemas spezifische Bilder können die Suffixe `_22` oder `_23` haben. Bilder, die spezifisch für deutsche Gebietsschemata sind, könnten die Suffixe `_470` oder `_480` haben.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | Zu durchsuchende Ausgabe-IDs |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Alle anderen | myImg_1, myImg_2, myImg_3 |

##### Wichtige Überlegungen bei der Implementierung von Lokalisierungsunterstützung

* Die Lokalisierung ist auf ID-basierte Asset-Abrufe beschränkt und kann nicht für pfadbasierte Asset-Abrufe verwendet werden. Wenn also Videos mit einem Gebietsschema abgerufen werden sollen, müssen sie als Unternehmens-/Asset-ID abgerufen werden, nicht über den vollständigen Pfad zum Video. Sie können rtmp nicht mit Lokalisierung verwenden, da diese Methode nur für pfadbasierte Videoaufrufe verwendet werden kann.
* Sie können kein gemischtes Medienset verwenden, das ein einzelnes Video enthält, wenn localeMap aktiv ist. Andernfalls schlägt der Abruf der Set-Inhalte fehl. Um dieses Problem zu umgehen, können Sie einem adaptiven Videoset ein einzelnes Video hinzufügen. Fügen Sie das adaptive Videoset anschließend einem gemischten Medienset hinzu.
* Bestimmte Abfragen sind nicht lokalisiert. Dies gilt beispielsweise für die Abfrage der Inhalte eines adaptiven Videosets. Wenn Sie also adaptive Videosets mit Lokalisierung verwenden möchten, platzieren Sie das adaptive Videoset in einem gemischten Medienset. Rufen Sie dann das Set in einen Viewer für gemischte Medien mit dem Parameter `locale=` auf.

## Bild-Renderer {#image-renderer}

Auf der Seite Bild-Renderer werden Standardeinstellungen für die Bereitstellung von Bildsets von Bild-Rendering-Servern festgelegt. Einstellungen sind in diesen fünf Kategorien verfügbar (detaillierte Beschreibungen der Einstellungen finden Sie auf der Image-Server-Seite selbst ):

* **Katalogverwaltung**  - Diese Einstellungen bestimmen, wie Dynamic Media Classic und die Katalogdatei interagieren. Dynamic Media Classic Render Server URL-Aufrufe werden an den Katalog gesendet, der wiederum Aufrufe zur Bereitstellung von Bildern vom Server sendet. Ändern Sie diese Einstellungen nur mithilfe eines Dynamic Media Classic-Support-Mitarbeiters.

* **Sitzungsattribute**  - Mit diesen Einstellungen werden Fehlerparameter, die URL für relative Bild-URLs und die Berechtigung zur Überlappung von Objekten festgelegt.

* **Standardmäßige Materialattribute**  - Mit diesen Einstellungen werden standardmäßige Auflösungs- und Scharfzeichnungseinstellungen für Bilder festgelegt.

* **Bildattribute für Antworten**  - Diese Einstellungen beziehen sich auf das standardmäßige Erscheinungsbild von Bildern.

* **Farbverwaltungsattribute**  - Diese Einstellungen beziehen sich auf die Standardfarbeinstellungen von Bildern.

## Vignette {#vignette}

Die Vignette-Seite bietet Einstellungen zum Festlegen des standardmäßigen Erscheinungsbilds von Vignetten (detaillierte Beschreibungen der Optionen finden Sie auf der Seite selbst).
