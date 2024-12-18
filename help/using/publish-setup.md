---
title: Veröffentlichungseinstellungen
description: Mit den Publish-Setup-Einstellungen können Sie festlegen, wie Assets standardmäßig von Adobe Dynamic Media Classic-Servern an Websites oder Programme bereitgestellt werden.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 699d4c12-e47b-4c6b-86f3-dc7aaaa56c1e
topic: Administration, Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '2383'
ht-degree: 30%

---

# Veröffentlichungseinstellungen {#publish-setup}

Die Einstellungen der Publish-Setup-Seite bestimmen, wie Assets standardmäßig von Adobe Dynamic Media Classic-Servern an Websites oder Programme bereitgestellt werden. Wenn keine Einstellung festgelegt ist, stellt der Adobe Dynamic Media Classic-Server ein Asset gemäß einer Standardeinstellung auf der Publish-Setup-Seite bereit. Beispielsweise liefert eine Anforderung zum Bereitstellen eines Bildes, das kein Auflösungsattribut enthält, ein Bild mit der Einstellung „Standardobjektauflösung“ auf der Seite „Bild-Server“.

Admins können die Standardeinstellungen auf den Seiten „Image-Server“, „Image-Renderer“ und „Vignette“ ändern, um Standardeinstellungen für die Bereitstellung von Assets von Servern festzulegen.

Zum Öffnen der Seiten von Publish Setup navigieren Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Publish Setup]**.

>[!NOTE]
>
>Die Publish-Setup-Seiten sind für erfahrene Website-Entwickler und -Programmierer vorgesehen. Adobe Dynamic Media Classic geht davon aus, dass Benutzende, die Einstellungen auf diesen Seiten ändern, mit Adobe Dynamic Media Classic, HTTP-Protokollstandards und -Konventionen und grundlegender Bildverarbeitungstechnologie vertraut sind.

## Image-Server {#image-server}

Auf der Seite „Image-Server“ werden Standardeinstellungen für die Bereitstellung von Bildern von Image-Servern festgelegt. Die Einstellungen sind in diesen fünf Kategorien verfügbar (detaillierte Beschreibungen der Einstellungen finden Sie auf der Image-Server-Seite selbst).

Ändern Sie diese Einstellungen nur mithilfe eines Adobe Dynamic Media Classic-Support-Mitarbeiters.

* **[!UICONTROL Katalogverwaltung]**: Diese Einstellungen bestimmen, wie Adobe Dynamic Media Classic und der Katalog interagieren. Im Gegensatz zu den meisten Webservern werden Dynamic Media-Bildserver-URL-Aufrufe an eine Manifest- oder Katalogdatei und nicht an eine eigentliche Bilddatei gesendet. Die Katalogdatei (nicht zu verwechseln mit einem E-Katalog) enthält eine Liste aller auf dem Bildserver veröffentlichten Inhalte. Sie enthält auch den Pfad zu den einzelnen Bildern. Wenn Sie über eine Digimarc-ID verfügen, geben Sie Ihre Benutzerdaten im Abschnitt „Benutzerinformationen für Digimarc“ ein.

* **[!UICONTROL Anfrage-Attribute]**: Mit diesen Einstellungen werden Einschränkungen für die Bilder festgelegt, die über den Server bereitgestellt werden können. Die maximale Größe *max* für **[!UICONTROL Antwortbild]** beträgt beispielsweise **[!UICONTROL Breite]** 5000 und **[!UICONTROL Höhe]** 5000.

* **[!UICONTROL Standardattribute für Anfragen]**: Diese Einstellungen beziehen sich auf die standardmäßige Darstellung von Bildern.

* **[!UICONTROL Allgemeine Attribute für Miniaturen]**: Diese Einstellungen beziehen sich auf die standardmäßige Darstellung und Ausrichtung von Miniaturbildern.

* **[!UICONTROL Standardeinstellungen für Katalogfelder]**: Diese Einstellungen beziehen sich auf die Auflösung und den Standardtyp für Miniaturen von Bildern.

* **[!UICONTROL Farbverwaltungsattribute]**: Mit diesen Einstellungen wird festgelegt, welche ICC-Farbprofile verwendet werden.

* **[!UICONTROL Kompatibilitätsattribute]**: Diese Einstellung ermöglicht die Behandlung von Anfangs- und Endabsätzen in Textebenen wie in Version 3.6, um die Abwärtskompatibilität zu gewährleisten.

* **[!UICONTROL Lokalisierungsunterstützung]**: Mit diesen Einstellungen können mehrere Gebietsschemaattribute verwaltet werden. Damit können Sie außerdem eine Zeichenfolge für Gebietsschemakarten angeben, um zu definieren, welche Sprachen Sie für die verschiedenen QuickInfos in den Viewern unterstützen möchten.

  Wenn Sie beispielsweise eine multinationale Marke sind mit Vertrieb in verschiedenen Ländern, können Sie sicherstellen, dass jedes Land seinen eigenen Gebietsschema-spezifischen Viewer hat. Für diese Funktion geben Sie eine Zeichenfolge für Gebietsschemakarten an. Anschließend bearbeiten Sie den QuickInfo-Text in der Viewer-Vorgabe. Fügen Sie einfach die übersetzten Textzeichenfolgen für die gewünschte Sprache hinzu.

  >[!NOTE]
  > Um Optionen für die Lokalisierungsunterstützung einzurichten, [verwenden Sie die Admin Console , um einen Support-Fall zu erstellen.](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) Bitten Sie in Ihrem Support-Fall um Hilfe bei der Einrichtung.

  Weitere Informationen zum Einrichten von **[!UICONTROL Lokalisierungsunterstützung]** finden Sie unter [Betrachtungen beim Planen der Asset-Lokalisierung](publish-setup.md#considerations_when_setting_up_localization_of_assets).

### Betrachtungen beim Planen der Asset-Lokalisierung {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Wenn Sie Optionen für die Lokalisierungsunterstützung in Adobe Dynamic Media Classic einrichten möchten, wie z. B. das Feld „Gebietsschema-Zuordnung“, [ Sie mithilfe der -Admin Console einen Support-Fall erstellen.](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) Bitten Sie in Ihrem Support-Fall um Hilfe bei der Einrichtung.

Eine gängige Methode zur Verwendung von Adobe Dynamic Media Classic besteht darin, die Produktbilder auf E-Commerce-Websites zu verwalten. Internationale Unternehmen haben das Problem, dass Assets für ähnliche Produkte je nach Land ganz anders aussehen. Normalerweise bestehen die Unterschiede bei einigen Teilen des gesamten Mediums. Solche Unterschiede zu beheben, indem alle Vermögenswerte für jedes der Länder kopiert und nur die Unterschiede überschrieben werden, ist eine enorme Anstrengung und widerspricht der einzigen Metapher der primären Vermögenswerte. Solche Unterschiede bei Assets können von länderspezifischen Videos mit verschiedenen Audiospuren bis zu minimalen aber wichtigen Unterschieden bei einem Netzkabel reichen, das im Lieferumfang des Produkts enthalten ist. Adobe Dynamic Media Classic verwendet einen einfachen Suchmechanismus. Sie definieren eine Reihenfolge der Asset-Suffixe, in denen Image Server beginnend mit dem erforderlichen Gebietsschema sucht.

#### Lokalisieren von Assets

Das Gebietsschema für eine IS-Anfrage (Image Serving) wird mit dem folgenden IS/IR-Befehl (Image Rendering) identifiziert:

`locale=`

Dieser Befehl akzeptiert eine Zeichenfolge mit der Gebietsschema-ID (locId), bei der nicht zwischen Groß- und Kleinschreibung unterschieden wird. Die Gebietsschema-ID ist normalerweise eine Zeichenfolge mit 2-6 Zeichen, die aus Buchstaben und &quot;`_`&quot; besteht.

IS unterstützt beliebige druckbare ASCII-Zeichenfolgen. Der Befehl `locale=` hat einen globalen Gültigkeitsbereich, d. h. er wird auf die gesamte Anfrage angewendet, einschließlich aller verschachtelten IS- und IR-Anfragen, referenzierten Vorlagen und Bildebenen. Mehrere Gebietsschemas pro Abfrage, wie ein verschiedenes Gebietsschema für jede Ebene, werden nicht unterstützt. Es ist jedoch denkbar, explizite Überschreibvorgänge in verschachtelten Abfragen zuzulassen.

Wenn `locale=` nicht angegeben ist, wird `attribute::DefaultLocale` an die Übersetzungs-Engines übergeben. Auf den `locale=`-Wert wird eine eingeschränkte Eingabevalidierung angewendet. Leere `locale=` sind zulässig. Da `locale=` einen globalen Umfang hat, wird `attribute::DefaultLocale` vom Hauptkatalog für die gesamte Anfrage bereitgestellt.

Zu den Vorteilen der Verwendung von `locale=` und `attribute::DefaultLocale` gehören die folgenden:

* Freigeben von Inhalten für mehrere Gebietsschemas.
* Zugriff auf Gebietsschema-spezifische Inhalte mit generischen IDs.
* Zulassen von Flexibilität bei Benennungskonventionen und Verwaltung Gebietsschema-spezifischer Inhalte wie Gebietsschema-Präfix und -Suffix oder Gebietsschema-spezifischer Inhalte in einem separaten Katalog.
* Unterstützung des Zugriffs auf gebietsschemaspezifische Versionen.
* Aggregierte Objekte wie Bildsets können manchmal allgemeine Verweise auf potenziell gebietsschemaspezifische Inhalte enthalten.
* Unterstützt alle Inhalte, die von Katalogen verwaltet werden, die lokalisiert werden müssen, einschließlich Bilder, Bildsets, Vignetten, Materialien und Viewer-Konfigurationsdatensätze.
* Minimieren von Änderungen an der IPS-Datenbank und IS-Manifestmechanismen.
* Unterstützung für statische Inhalte wie Videos und Skins wird hinzugefügt, wenn RFC IS-63 implementiert ist.
* Das Standard-Gebietsschema kann konfiguriert werden.

#### Anwendungsszenarien

| Anwendung | Szenario |
| --- | --- |
| Viewer-Lokalisierung | Nachdem statische Inhaltskataloge implementiert wurden, wird die Lokalisierung vollständig mit dem Parameter locale= gesteuert, der an alle Anfragen angehängt wird, die an IMS gesendet werden. Konfigurationsdatensätze, Skins, Splashscreens usw. können über Gebietsschema-spezifische Varianten verfügen. Der korrekte Inhalt wird über IS bereitgestellt, ohne dass der Viewer wissen muss, welche Inhalte lokalisiert sind und wie die entsprechenden IDs lauten. |
| Bilder und Videos | Internationale Konzerne verwenden häufig eine Mischung aus generischen und Gebietsschema-spezifischen Inhalten. Mit diesem Mechanismus kann ein Verweis auf ein Bild oder Video generisch sein. Und IS stellt die Gebietsschema-spezifischen Inhalte bereit, sofern diese vorhanden sind. |
| Bildsets und Mediensets | Das gesamte Bildset kann für einige Gebietsschemata unterschiedlich sein, z. B. wenn ein eCatalog anders ist, wobei die Übersetzung von einem generischen zu einem gebietsschemaspezifischen Bildset vom Viewer verarbeitet wird. Häufiger kommt es vor, dass einzelne IDs in einem generischen Satz auf lokalisierte Inhalte verweisen können. Beispielsweise können die meisten Fotos einer Appliance in allen Sprachen identisch sein, mit Ausnahme des Fotos vom Control Panel. IS übersetzt IDs automatisch, sodass keine gebietsschemaspezifischen Bildsets generiert werden müssen. |

#### Asset-Lokalisierung implementieren

Adobe Dynamic Media Classic und Bildbereitstellung verfügen über eine Benutzeroberfläche, die die Lokalisierung von Bildern und statischen Inhalten ermöglicht.

Ohne Lokalisierung sieht eine Image Server-URL wie folgt aus:

`https://server/is/image/company/image`

Bei der Lokalisierung fügt eine Bild-Server-URL den `locale=`-Parameter zum Pfad hinzu, wie im Folgenden dargestellt:

`https://server/is/image/company/image?locale=de_DE`

Nach Erhalt des HTTP-Aufrufs durch den Bild-Server wird der `locale=` durch das `localeMap` geparst, das in der Gruppe **[!UICONTROL Setup]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Publish-Setup]** > **[!UICONTROL Bild-Server]** > **[!UICONTROL Lokalisierungsunterstützung]** ist.

Das Feld „Gebietsschemakarte“ enthält eine Liste mit Einträgen, die durch einen senkrechten Strich (|) getrennt sind.

Jeder Eintrag besteht aus einer durch Kommas getrennten Liste von Werten. Der erste Wert ist der Suchwert, der durch den `locale=` Parameter übergeben wird. Die restlichen Werte sind Suffix-/Ersatzwerte, die dann versucht werden, bis ein vorhandenes Bild entsteht.

Ob ein Suffixwert oder ein Ersetzungswert angewendet wird, hängt von der Einstellung „Globales Gebietsschema“ in der Gruppe **[!UICONTROL Einstellungen]** > **[!UICONTROL Anwendungseinstellungen]** > **[!UICONTROL Veröffentlichungseinstellungen]** > **[!UICONTROL Image-Server]** > **[!UICONTROL Lokalisierungsunterstützung]** ab.

>[!NOTE]
>
>Die Einstellung „Globales Gebietsschema“ ist nur möglich, wenn Sie sie über die API festlegen, nicht innerhalb der Adobe Dynamic Media Classic-Oberfläche.

**Beispiel für ein Suffix:**

| URL | localeMap-IDs | Ergebnis | Anmerkungen |
| --- | --- | --- | --- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,` | `fr_FR,_FR,` | Beachten Sie, dass kein GlobalLocale definiert ist. Der Gebietsschema-Parameter de_DE wird mit dem ersten Eintrag im `localeMap` abgeglichen. Der erste entsprechende Wert _DE wird dem Asset image_DE als Suffix hinzugefügt und versucht, ihn auf dem Image-Server zu finden. Wenn er auf dem Server gefunden wurde, wird er zurückgegeben. Andernfalls wird der zweite Wert &quot;&quot; als Suffix verwendet, wodurch das Bild selbst zurückgegeben wird. |

**Ersatzbeispiel:**

| URL | `GlobalLocale` und `localeMap` IDs | Ergebnis | Anmerkungen |
| --- | --- | --- | --- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main` | `fr_FR,fr,main` | Im obigen Ersatzbeispiel wird „GlobalLocale“ auf „main“ festgelegt. Der Gebietsschema-Parameter de_DE wird mit dem ersten Eintrag im `localeMap` abgeglichen. Die Teilzeichenfolge GlobalLocale wird gefunden und durch den ersten entsprechenden Wert `de` im `localeMap` ersetzt: `image-de-01`. Wenn er auf dem Bildserver gefunden wird, wird er zurückgegeben. Ist dies nicht der Fall, wird der zweite Wert ersetzt, was zu `image-main-01` führt. |

Wenn in der URL kein Gebietsschema definiert ist, verwendet der Image-Server DefaultLocale, sofern definiert, und wendet es auf die URL an.

Wenn ein unbekannter oder leerer Gebietsschemaparameter mit `locale=` angegeben wird, wird der `localeMap` auf den leeren Wert „Starting with“ (Beginnend mit) überprüft. Es ist wichtig, ein Standardgebietsschema für unbekannte Gebietsschemata anzuwenden.

#### Über defaultImage

Der Image-Server versucht nacheinander, die Optionen für das angeforderte Gebietsschema zu verwenden. Wenn keine Übereinstimmung gefunden wird, werden die Gebietsschema-Optionen auf defaultImage angewendet und die entsprechende Version wird zurückgegeben. Daher muss entweder jedes Gebietsschema eine Option für das Bild ohne Lokalisierung enthalten, oder lokalisierte „defaultImage“-Versionen werden in Adobe Dynamic Media Classic zur Verfügung gestellt.

#### Szenarien für die Suche nach localeMap

Angenommen, Sie möchten die folgenden Gebietsschemas unterstützen:

`en, en_us, en_uk, de, de_at, de_de, fr`

Sie ordnen diese Gebietsschemata den Suffixen `_E` (Englisch), `_G` (Deutsch) und `_F` (Französisch) zu. Für alle Beispiele ist die generische Eingabebild-ID `myImg`.

##### Standardverhalten für das Auffinden von localeMap

Die Gebietsschema-IDs werden den entsprechenden Suffixen zugeordnet. Wenn keine Gebietsschema-spezifische ID im Katalog gefunden wird, wird die generische ID verwendet. Beachten Sie die leeren locSuffix-Werte, die der generischen ID zugeordnet sind.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | Zu durchsuchende Ausgabe-IDs |
| --- | --- |
| en, en_us, en_uk | myImg_E, myImg |
| de, de_de, de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Alle anderen | : |

##### Suchen der localeMap bei unbekanntem Gebietsschema

Sie können unbekannte Gebietsschemas bestimmten IDs oder generischen IDs zuordnen. Sie können beispielsweise den englischen IDs unbekannte Gebietsschemata zuordnen oder, falls sie nicht vorhanden sind, den generischen IDs.

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | Zu durchsuchende Ausgabe-IDs |
| --- | --- |
| de, de_de, de_at | myImg_D, myImg |
| fr | myImg_F, myImg |
| Alle anderen | myImg_E, myImg |

Sie können auch ein dediziertes locSuffix wie z. B. U nur für unbekannte Gebietsschemata verwenden und das Standardbild erzwingen, wenn keine `_U` vorhanden ist, wie im Folgenden dargestellt:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

Oder Sie können wie im folgenden Beispiel direkt die generische ID zuordnen:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### Suchen der localeMap mithilfe einer mehrstufigen Suche

Häufig ist es hilfreich, Gebietsschemas zu gruppieren, z. B. nach den Regionen Europa, Naher Osten und Nordamerika, um so regionalen Standards wie Sonneneinstrahlung zu berücksichtigen. Diesen Effekt erzielen Sie mit einer mehrstufigen Suche.

Angenommen, Sie möchten Sammlungen für die Verwendung im Westen und Nahen Osten unterstützen. Beide Sammlungen basieren auf der generischen Bildsammlung und in beiden werden einige Bilder hinzugefügt oder angepasst. Beide Sammlungen werden dann für bestimmte Gebietsschemata weiter verfeinert. Zum Beispiel `m1, m2` für zwei Varianten im Nahen Osten und `w1, w2,` und `w3` für drei westliche Gebietsschemata, mit der Ausnahme, dass Bilder für `w1` und `w3` freigegeben werden. Unbekannte Gebietsschemas sind nur der generischen Sammlung zugeordnet und haben keinen Zugriff auf Gebietsschema-spezifische Bilder. Die Karte würde wie folgt aussehen:

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | Zu durchsuchende Ausgabe-IDs |
| --- | --- |
| W1, W3 | myImg-W, myImg |
| W2 | myImg-W2, myImg-W, myImg |
| M1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| Alle anderen | Mylmg |

##### Suchen der localeMap durch Suchen nach bestimmten IDs

Einige Bildnamenskonventionen unterstützen keine generischen Bild-IDs. Die generischen IDs aus der Abfrage müssen einer bestimmten ID im Katalog zugeordnet werden. Es gibt jedoch Fälle, in denen die genaue spezifische ID nicht bekannt ist.

Wenn Sie das erste Beispiel als Grundlage verwenden, könnten Bilder für alle Sprachen die Suffixe `_1`, `_2` oder `_3` aufweisen. Bilder, die für französische Gebietsschemata spezifisch sind, können die Suffixe `_22` oder `_23` Suffix aufweisen. Bilder, die für deutsche Gebietsschemata spezifisch sind, können die Suffixe `_470` oder `_480` aufweisen.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | Zu durchsuchende Ausgabe-IDs |
| --- | --- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| Alle anderen | myImg_1, myImg_2, myImg_3 |

##### Wichtige Aspekte bei der Implementierung der Lokalisierungsunterstützung

* Die Lokalisierung ist auf ID-basierte Asset-Abrufe beschränkt und kann nicht für pfadbasierte Asset-Abrufe verwendet werden. Wenn also Videos mit einem Gebietsschema abgerufen werden sollen, müssen sie als Unternehmens-/Asset-ID abgerufen werden, nicht über den vollständigen Pfad zum Video. Sie können `RTMP` nicht mit der Lokalisierung verwenden, da diese Methode nur für die Verwendung mit pfadbasierten Videoaufrufen vorgesehen ist.
* Sie können kein gemischtes Medienset verwenden, das ein einzelnes Video enthält, wenn localeMap aktiv ist. Andernfalls schlägt der Abruf der Set-Inhalte fehl. Um dieses Problem zu umgehen, können Sie einem adaptiven Videoset ein einzelnes Video hinzufügen. Fügen Sie das adaptive Videoset anschließend einem gemischten Medienset hinzu.
* Bestimmte Abfragen sind nicht lokalisiert. Dies gilt beispielsweise für die Abfrage der Inhalte eines adaptiven Videosets. Wenn Sie daher adaptive Videosets mit Lokalisierung verwenden möchten, platzieren Sie das adaptive Videoset in ein gemischtes Medienset. Rufen Sie dann das Set in einem Viewer für gemischte Medien mit dem `locale=` auf.

## Bild-Renderer {#image-renderer}

Auf der Seite „Bild-Renderer“ werden Standardeinstellungen für die Bereitstellung von Bildsets von Bild-Rendering-Servern festgelegt. Die Einstellungen sind in diesen fünf Kategorien verfügbar (detaillierte Beschreibungen der Einstellungen finden Sie auf der Image-Server-Seite selbst):

* **[!UICONTROL Katalogverwaltung]**: Diese Einstellungen bestimmen, wie Adobe Dynamic Media Classic und die Katalogdatei interagieren. Adobe Dynamic Media Classic Render-Server-URL-Aufrufe werden an den Katalog gesendet, der wiederum Aufrufe ausführt, um Bilder vom Server bereitzustellen. Ändern Sie diese Einstellungen nur mithilfe eines Adobe Dynamic Media Classic-Support-Mitarbeiters.

* **[!UICONTROL Sitzungsattribute]**: Mit diesen Einstellungen werden Fehlerparameter festgelegt sowie die URL für relative Bild-URLs und ob die Überlappung von Objekten zulässig ist.

* **[!UICONTROL Standardmaterialattribute]**: Mit diesen Einstellungen werden die Standardauflösungs- und Scharfzeichnungseinstellungen für Bilder festgelegt.

* **[!UICONTROL Antwort-]**: Diese Einstellungen beziehen sich auf die standardmäßige Darstellung von Bildern.

* **[!UICONTROL Farbverwaltungsattribute]**: Diese Einstellungen beziehen sich auf die standardmäßigen Farbeinstellungen von Bildern.

## Vignette {#vignette}

Die Seite Vignette bietet Einstellungen zum Festlegen des standardmäßigen Erscheinungsbilds von Vignetten (detaillierte Beschreibungen der Optionen finden Sie auf der Seite selbst).
