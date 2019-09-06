---
title: Abrufen von Speichernutzungsinformationen
seo-title: Abrufen von Speichernutzungsinformationen
description: 'null'
seo-description: Erfahren Sie, wie Sie Datenträgernutzungsinformationen erhalten.
uuid: 1361693-53 d 0-4072-b 7 c 3-f 284631 d 28 cf
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
discoiquuid: 6763546 d -83 c 4-42 dc -879 f -6 bbfc 8 b 56482
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# Abrufen von Speichernutzungsinformationen {#getting-disk-usage-information}

Mit dem Parameter `disk_info` können Sie Informationen zur Speichernutzung eines Unternehmens abrufen, wie im folgenden Beispiel gezeigt:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

Eine Antwort sieht beispielsweise folgendermaßen aus:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>disk_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Disk Information for d03b7e0b-c9dc-4c6c-af0b-419beeea1c63</title> 
            <message>Total Space available = 1395402342400 bytes. Total Space used = 0 bytes.</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Folgende Felder können Sie in der URL-Anfragezeichenfolge zum Abrufen von Speichernutzungsinformationen verwenden:

| URL-Parameter | Erforderlich/optional | Wert |
|--- |--- |--- |
| op | Erforderlich | disk_info |
| shared_secret | Erforderlich | Der gemeinsame geheime Schlüssel für das Unternehmen |

Der folgende Beispiel-Code ruft Speichernutzungsinformationen für das Unternehmen „000Company“ ab:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```

