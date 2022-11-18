---
title: Einschränkungen bei Dynamic Media
description: Erfahren Sie mehr über die Best Practices und erzwungenen Einschränkungen beim Erstellen eines Bildsets oder eines Rotationssets oder beim Hochladen einer PDF. Erfahren Sie auch mehr über nicht unterstützte Webbrowser- und Betriebssystemkombinationen für Dynamic Media.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Asset Management,Image Sets,Spin Sets,eCatalog
role: User
exl-id: ee30a2c1-2b26-41bd-8758-e7337a3727bb
source-git-commit: 10e603f566cd7f968c3a6aea1ba277697a1734ca
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 2%

---

# Dynamic Media-Einschränkungen

Die folgenden Abschnitte beschreiben Einschränkungen in Dynamic Media.

Dieses Thema enthält die folgenden Abschnitte:

* [Best Practices und erzwungene Einschränkungen von Dynamic Media für Asset-Typen](#best-practice-enforced-limits)
* [Nicht unterstützte Webbrowser- und Betriebssystemkombinationen für Dynamic Media](#unsupported-browser-os)

## Best Practices und erzwungene Einschränkungen von Dynamic Media für Asset-Typen {#best-practice-enforced-limits}

Wenn Sie ein Rotationsset oder Bildset erstellen oder PDF zur Seitenextrahierung hochladen, empfiehlt Adobe die folgenden Best Practices und setzt die folgenden Einschränkungen um:

| Asset - Limit-Typ | Optimale Vorgehensweise | Begrenzung auferlegt | Änderung der Beschränkung am 31. Dezember 2022 |
| --- | --- | --- | --- |
| **Bild** - Anzahl der smarten Zuschnitte pro Bild | 5 | 100 | Nicht anwendbar |
| **Alle Sets** - Anzahl doppelter Assets pro Satz | Keine Duplikate | 20 | Nicht anwendbar |
| **Alle Sets** - Maximale Anzahl von Assets pro Satz | 5 - 10 Bilder pro Set | 1000 | Nicht anwendbar |
| **Rotationsset** - Maximale Anzahl von Zeilen/Spalten pro 2D-Satz | 12-18 Bilder pro Set | 1000 | Nicht anwendbar |
| **PDF** - Maximale Seitenzahl für eine PDF, die für die Extraktion berücksichtigt werden soll |  | 5000 (für neue Uploads) | 100 (für alle PDF) |

<!-- See also [Dynamic Media limitations](/help/assets/limitations.md). -->

## Nicht unterstützte Webbrowser- und Betriebssystemkombinationen für Dynamic Media {#unsupported-browser-os}

<!-- CQDOC-19433 -->

Adobe Dynamic Media unterstützt die folgenden Webbrowser- und Betriebssystemkombinationen nicht.

* Internet Explorer 11 + Windows 7
* Internet Explorer 11 + Windows 8.1
* Internet Explorer 11 + Windows Phone 8.1
* Aktualisierung von Internet Explorer 11 und Windows Phone 8.1
* Safari 6 + iOS 6.0.1
* Safari 7 + iOS 7.1
* Safari 7 + OS X 10.9 - Mavericks
* Safari 8 + iOS 8.4
* Safari 8 + OS X 10.10 Yosemite

## Ende der Unterstützung für Transport Layer Security 1.0 und 1.1 {#tls}

<!-- CQDOC-19433 -->

Ab dem 30. September 2022 stellt Adobe Dynamic Media die Unterstützung für Folgendes ein:

* TLS (Transport Layer Security) 1.0 und 1.1
* Die folgenden schwachen Chiffren in TLS 1.2:
   * `TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384`
   * `TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA`
   * `TLS_RSA_WITH_AES_256_GCM_SHA384`
   * `TLS_RSA_WITH_AES_256_CBC_SHA256`
   * `TLS_RSA_WITH_AES_256_CBC_SHA`
   * `TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA256`
   * `TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA`
   * `TLS_RSA_WITH_AES_128_GCM_SHA256`
   * `TLS_RSA_WITH_AES_128_CBC_SHA256`
   * `TLS_RSA_WITH_AES_128_CBC_SHA`
   * `TLS_RSA_WITH_CAMELLIA_256_CBC_SHA`
   * `TLS_RSA_WITH_CAMELLIA_128_CBC_SHA`
   * `TLS_ECDHE_RSA_WITH_3DES_EDE_CBC_SHA`
   * `TLS_RSA_WITH_SDES_EDE_CBC_SHA`

