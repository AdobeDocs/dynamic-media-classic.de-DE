---
title: Abrufen von Informationen zur Festplattenauslastung
description: Erfahren Sie, wie Sie Informationen zur Festplattenauslastung in Adobe Dynamic Media Classic erhalten.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 337a4681-ac9a-40d9-82e8-1999bbed980c
topic: Administration, Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '91'
ht-degree: 42%

---

# Abrufen von Informationen zur Festplattenauslastung {#get-disk-usage-information}

Sie können den `disk_info`-Parameter verwenden, um Informationen über die Speicherplatznutzung eines Unternehmens abzurufen, wie im folgenden Beispiel gezeigt:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

Eine Antwort sieht beispielsweise folgendermaßen aus:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
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
| --- | --- | --- |
| op | Erforderlich | disk_info |
| shared_secret | Erforderlich | Der Schlüssel, der für das Unternehmen ein gemeinsam genutztes Geheimnis ist |

Der folgende Beispiel-Code ruft Speichernutzungsinformationen für das Unternehmen „000Company“ ab:

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```
