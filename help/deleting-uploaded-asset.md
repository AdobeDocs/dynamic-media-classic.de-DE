---
title: Löschen eines hochgeladenen Assets
description: Erfahren Sie, wie Sie ein hochgeladenes Asset in Dynamic Media Classic löschen.
uuid: edd2b688-c377-4be1-ba16-d2dd2e6f716d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: dd338c8c-06c6-44d5-8493-dc2087eeeafb
feature: Dynamic Media Classic
role: User
exl-id: d845bcb2-f914-4727-8df2-049dc172f266
source-git-commit: 47845c30311fb9afb3fffb8502b6e7c534e4bfdb
workflow-type: tm+mt
source-wordcount: '95'
ht-degree: 84%

---

# Löschen eines hochgeladenen Assets{#deleting-an-uploaded-asset}

Verwenden Sie den Parameter `delete` in folgendem Format, um ein Asset zu löschen:

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Hier ein Beispiel für eine Antwort, wenn ein Bild-Asset gelöscht wird:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
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
| `shared_secret` | Erforderlich | Der gemeinsame geheime Schlüssel für das Unternehmen. |
| <ul><li>Für Bilder:image_name</li><li>Bei Vektoren:fxg_name</li></ul> | Erforderlich | Name des Assets, das gelöscht werden soll. |

**Beispielbild-URL:**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Beispiel-Vektor-URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg`
