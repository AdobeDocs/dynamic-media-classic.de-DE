---
title: Einschränkungen bei Dynamic Media
description: Erfahren Sie mehr über die Best Practices und Einschränkungen beim Erstellen eines Bildsets oder Rotationssets oder beim Hochladen einer PDF. Erfahren Sie außerdem mehr über nicht unterstützte Webbrowser- und Betriebssystemkombinationen für Dynamic Media.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Asset Management,Image Sets,Spin Sets,eCatalog
role: User
exl-id: ee30a2c1-2b26-41bd-8758-e7337a3727bb
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:02:23.354Z'
TQID: 'https://experienceleague.adobe.com/7dtiaPb7sWkPb5gocOc8xLOnz3U3gJuSdaW2LSkajMk'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 352
ht-degree: 1%

---

# Grenzwerte für Dynamic Media

In den folgenden Abschnitten werden Einschränkungen in Dynamic Media beschrieben.

Dieses Thema enthält die folgenden Abschnitte:

* [Best Practices und Einschränkungen durch Dynamic Media bei Asset-Typen](#best-practice-enforced-limits)
* [Nicht unterstützte Webbrowser- und Betriebssystemkombinationen für Dynamic Media](#unsupported-browser-os)

## Best Practices und Einschränkungen durch Dynamic Media bei Asset-Typen {#best-practice-enforced-limits}

Wenn Sie ein Rotationsset oder Bildset erstellen oder PDFs zur Seitenextraktion hochladen, empfiehlt Adobe die folgenden Best Practices. Adobe setzt außerdem die folgenden Beschränkungen durch:

| Asset: Art des Limits | Optimale Vorgehensweise | Limit |
| --- | --- | --- |
| **image**: Anzahl der smarten Zuschnitte pro Bild | 5 | 100 |
| **Alle Sets**: Anzahl der doppelten Assets pro Set | Keine Duplikate | 20 ‡ |
| **Alle Sets**: Maximale Anzahl von Assets pro Set | 5-10 Bilder pro Set | 1000 |
| **Rotationsset**: Maximale Anzahl von Zeilen/Spalten pro 2D-Set | 12-18 Bilder pro Set | 1000 |
| **PDF**: Maximale Seitenzahl für eine PDF, damit eine Extraktion durchgeführt werden kann |  | 100 (für alle PDFs) |

‡ Best Practice ist es, keine doppelten Assets in einem Satz zu haben. Für ein einzelnes Asset sind maximal 20 Duplikate zulässig. Wenn Sie innerhalb dieses Sets ein weiteres Duplikat für dieses Asset hinzufügen, gibt die Anfrage entweder einen Fehler aus oder ignoriert das Duplikat.

<!-- See also [Dynamic Media limitations](/help/using/assets/limitations.md). -->

## Nicht unterstützte Webbrowser- und Betriebssystemkombinationen für Dynamic Media {#unsupported-browser-os}

<!-- CQDOC-19433 -->

Adobe Dynamic Media unterstützt nicht die folgenden Kombinationen aus Webbrowser und Betriebssystem.

* Internet Explorer 11 + Windows 7
* Internet Explorer 11 + Windows 8.1
* Internet Explorer 11 + Windows Phone 8.1
* Internet Explorer 11 + Windows Phone 8.1 Update
* Safari 6 + iOS 6.0.1
* Safari 7 + iOS 7.1
* Safari 7 + OS X 10.9 Mavericks
* Safari 8 + iOS 8.4
* Safari 8 + OS X 10.10 Yosemite

## Ende der Unterstützung für Secure Socket Layer 2.0 und 3.0 und Transport Layer Security 1.0 und 1.1 {#tls}

<!-- 
CQDOC-19433 (original ticket)
and CQDOC-19792 (removed as per this ticket December 5, 2022) 
-->

Ab dem 30. April 2024 stellt Adobe Dynamic Media die Unterstützung für Folgendes ein:

* SSL (Secure Socket Layer) 2.0
* SSL 3.0
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

