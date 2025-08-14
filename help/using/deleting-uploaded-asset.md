---
title: Löschen eines hochgeladenen Rasterbild-Assets
description: Erfahren Sie, wie Sie ein hochgeladenes Asset in Adobe Dynamic Media Classic löschen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: d845bcb2-f914-4727-8df2-049dc172f266
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 33%

---

# Löschen eines hochgeladenen Assets{#deleting-an-uploaded-asset}

Sie können den `delete`-Parameter in diesem Format verwenden, um ein Asset zu löschen:

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Hier ein Beispiel für eine Antwort, wenn ein Bild-Asset gelöscht wird:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>delete</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Delete request for1442564.tif</title> 
            <message>Your file was successfully deleted</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Folgende Felder können Sie in der URL-Anfragezeichenfolge zum Löschen eines Assets verwenden:

| URL-Parameter | Erforderlich/optional | Wert |
| --- | --- | --- |
| `op` | Erforderlich | löschen |
| `shared_secret` | Erforderlich | Der Schlüssel, der ein gemeinsam genutztes Geheimnis für das Unternehmen ist. |
| `image_name` | Erforderlich | Name des zu löschenden Assets. |

<!-- <li>For Vector:fxg_name</li> -->

>[!IMPORTANT]
>
>Ab dem 1. Mai 2023 stehen UGC-Assets in Dynamic Media bis zu 60 Tage ab dem Datum des Uploads zur Verwendung zur Verfügung. Nach 60 Tagen werden die Assets entfernt.

>[!NOTE]
>
>Die Unterstützung für neue oder vorhandene UGC-Vektorbild-Assets in Adobe Dynamic Media Classic endete am 30. September 2021.

**Beispielbild-URL:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg` -->
