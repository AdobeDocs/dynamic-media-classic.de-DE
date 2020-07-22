---
title: Hochladen von Bild-Assets oder Vektor-Assets
seo-title: Hochladen von Bild-Assets oder Vektor-Assets
description: 'null'
seo-description: Erfahren Sie, wie Sie ein Bild- oder Vektor-Asset hochladen.
uuid: d0e4a754-8a49-4b0f-b202-e9003bdb8f20
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: de21dca9-99fe-4183-b647-debfe112fda4
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1522'
ht-degree: 86%

---


# Hochladen von Bild-Assets oder Vektor-Assets{#uploading-an-image-asset-or-a-vector-asset}

Bevor Sie ein Bild-Asset hochladen können, fordern Sie zunächst einen gemeinsamen geheimen Schlüssel an. Mit diesem gemeinsamen geheimen Schlüssel können Sie ein Upload-Token abrufen. Mit dem Upload-Token können Sie anschließend Bild- oder Vektor-Assets hochladen.

## Anfordern eines gemeinsamen geheimen Schlüssels {#requesting-a-shared-secret-key}

Fordern Sie einen *gemeinsamen geheimen Schlüssel* an, indem Sie eine E-Mail an den technischen Support von Scene7 senden (s7support@adobe.com).

Geben Sie in der E-Mail-Nachricht den Unternehmensnamen an, den Sie verwenden möchten, um Bild-Assets hochzuladen. Nachdem Sie den Schlüssel von Dynamic Media Classic erhalten haben, speichern Sie ihn lokal für die zukünftige Verwendung.

## Abrufen des Upload-Tokens {#retrieving-the-upload-token}

Das *Upload-Token* stellt sicher, dass niemand denselben gemeinsamen geheimen Schlüssel zum Hochladen von Assets verwenden kann. Außerdem stellt es sicher, dass der Upload zulässig ist und von einer vertrauenswürdigen Quelle stammt.

Das Upload-Token besteht aus einer alphanumerischen Zeichenfolge, die nur für eine begrenzte Zeitspanne gültig ist. Verwenden Sie die folgenden URLs und ersetzen Sie Ihren gemeinsamen geheimen Schlüssel, um das Upload-Token abzurufen.

* Bild
   `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`In diesem Beispiel lautet der gemeinsame geheime Schlüssel `fece4b21-87ee-47fc-9b99-2e29b78b602`

* Vektor
   `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`In diesem Beispiel lautet der gemeinsame geheime Schlüssel `2d19f60e-890a-4e79-a1a5-9ac2875429b9`

Standardmäßig läuft das Upload-Token 5 Minuten (300 Sekunden) nach dem Abrufen ab. Wenn Sie mehr Zeit benötigen, schließen Sie den Parameter `expires` und die gewünschte Zeit in Sekunden in die URL ein. So wird bei der folgenden URL für ein Beispielbild ein Upload-Token abgerufen, das 1800 Sekunden gültig ist:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

Die erfolgreiche Antwort für Bilder sieht folgendermaßen aus:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
        <serviceName>User Generated Content - Images</serviceName> 
        <version>1.0.0</version> 
        <operationName>get_uploadtoken</operationName> 
        <serviceStatus>SUCCESS</serviceStatus> 
        <title>Upload Token for fece4b21-87ee-47fc-9b99-2e29b78b602</title> 
        <message> 
            <uploadtoken>aa2a378a-cd25-4c80-994d-312094e0ef20_1800</uploadtoken> 
            <expiration_in_seconds>1800</expiration_in_seconds> 
        </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Speichern Sie das Upload-Token für zukünftige Anfragen lokal.

Folgende Felder können Sie in der URL-Anfragezeichenfolge zum Abrufen eines Upload-Tokens verwenden:

| URL-Parameter | Erforderlich oder optional | Wert |
|--- |--- |--- |
| op | Erforderlich | get_uploadtoken |
| shared_secret | Erforderlich | Der gemeinsame geheime Schlüssel für das Unternehmen, das den Upload ausführt. |
| expires | Optional | Anzahl der Sekunden, die das Upload-Token gültig ist. Der Standardwert ist 300 Sekunden, wenn nicht spezifiziert. |

**Beispielbild-URL:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

**Beispiel-Vektor-URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000`

**Zulässige HTTP-Methoden:** GET und POST

Sie können nun ein Bild-Asset hochladen.

Siehe [Hochladen von Bild-Assets](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Hochladen von Bild-Assets {#uploading-an-image-asset}

Wenn Sie ein Upload-Token abgerufen haben, das für eine bestimmte Zeitspanne gültig ist, können Sie ein Bild-Asset hochladen. Sie laden das Asset mit der POST-Methode als mehrteilige Formulardaten hoch, während Sie die übrigen Werte als URL-Anfragezeichenfolge senden, wie im nachfolgenden Beispiel gezeigt:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

Siehe [Abrufen des Upload-Tokens](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Siehe [Anfordern eines gemeinsamen geheimen Schlüssels](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Sie können auch andere optionale Werte als URL-Anfragezeichenfolgen senden, wie das nachfolgende Beispiel zeigt:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

The `file_limit` parameter specifies the file-size limit in bytes. Der Parameter `file_exts` gibt die für das Hochladen zulässigen Erweiterungen des Dateinamens an. Diese beiden Werte sind optional.

In der Anwendung sind globale Beschränkungen für die maximale Dateigröße und zulässigen Dateierweiterungen festgelegt. Wenn es sich bei der von Ihnen gesendeten Anforderung um eine Untergruppe der globalen Beschränkungen handelt, wird diese berücksichtigt. Die globalen Beschränkungen lauten wie folgt:

| Globale Beschränkung | Wert |
|--- |--- |
| Dateigröße für alle Clients | 20 MB |
| Unterstützte Bilddateiformate zum Hochladen | BMP, GIF, JPG, PNG, PSD |

Mit dem folgenden HTML-Formular können Benutzer Assets hochladen. In dem Formular wird der Benutzer aufgefordert, die folgenden Informationen einzugeben:

* Einen Unternehmensnamen.
* Ein Upload-Token.
* Eine Beschränkung für die Dateigröße.
* Eine Liste mit den Erweiterungen für Dateinamen.
* Gibt an, ob das Profil und der Dateiname des Assets beibehalten werden sollen.
* Gibt an, ob der Hintergrund &quot;Aussparen&quot;verwendet werden soll. Wenn Sie &quot;Hintergrund aussparen&quot;aktivieren, legen Sie die Methode &quot;Ecke&quot;, &quot;Toleranz&quot;und &quot;Füllmethode&quot;fest. Siehe Hintergrund aussparen in den [Bildbearbeitungsoptionen beim Hochladen](image-editing-options-upload.md#image-editing-options-at-upload).
* Den Namen der hochzuladenden Datei

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment&gt; elements under &lt;adobefig&gt;.</p>

 -->

![]()

Sie können den HTML-Quellcode, der mit dem oben stehenden Formular verknüpft ist, durch Klicken auf den folgenden Link Ansicht haben:

[https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

Klicken Sie in Firefox mit der rechten Maustaste in das Browserfenster und dann auf **Seitenquelle**. Der Code enthält die URL-Anfragezeichenfolge und die POST-Methode, die ausgeführt werden, wenn der Benutzer auf **„Absenden“** klickt.

Um die XML-Antwort im Internet Explorer anzuzeigen, klicken Sie auf **„Ansicht“ > „Quelltext“**. To view XML response in Firefox, click **Tools > Web Developer > Page Source**. Zur Anzeige von XML-Antworten wird Firefox empfohlen.

Hier eine Beispielantwort für einen erfolgreiche Upload:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>upload</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Your file has been uploaded Successfully.</title> 
            <message> 
            <url>https://s7w2p1.scene7.com/is/image/ </url> 
            <path>000Company/ugc/1442564.tif</path> 
            <fullurl>https://s7w2p1.scene7.com/is/image/000Company/ugc/1442564.tif </fullurl> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

>[!NOTE]
>
>Das hochgeladene Asset (JPG, GIF usw.) wird ins PTIFF-Format umgewandelt und mit der Antwort wird eine direkte Verknüpfung zu diesem PTIFF-Asset gesendet.

Das Asset kann wie jede andere Image-Server-Ressource gehandhabt werden; Sie können auch Verarbeitungsanfragen darauf anwenden. Mit der folgenden URL wird beispielsweise ein Asset in der angegebenen Breite und Höhe angefordert.

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

Senden Sie das hochzuladende Asset mit der POST-Methode als mehrteilige Formulardaten, während Sie die übrigen Werte als URL-Anfragezeichenfolge senden. Folgende Felder können Sie in der URL-Anfragezeichenfolge zum Hochladen eines Assets verwenden:

| URL-Parameter | Erforderlich oder optional | Wert |
|--- |--- |--- |
| op | Erforderlich | Hochladen |
| upload_token | Erforderlich | Upload-Token für den gemeinsamen geheimen Schlüssel für das Unternehmen. |
| company_name | Erforderlich | Name des hochladenden Unternehmens. |
| file_limit | Optional | Maximale Dateigröße (in Byte) für das Asset. |
| file_exts | Optional | Liste der zulässigen Erweiterungen für die Bild-Asset-Datei. |
| preserve_colorprofile | Optional | Behält eingebettete Farbprofile bei der Konvertierung der hochgeladenen Datei in das PTIFF-Format bei. Mögliche Werte sind „true“ oder „false“. Der Standardwert ist „false“.. |
| preserve_filename | Optional | Behält den Dateinamen des hochgeladenen Assets bei. Mögliche Werte sind „true“ oder „false“. Der Standardwert ist „false“.. |

>[!NOTE]
>
>Das hochzuladende Asset muss als einziges Feld in einer mehrteiligen POST-Anfrage hochgeladen werden.

**Beispiel-URL:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**Zulässige HTTP-Methode:**

POST

### Abrufen von Asset-Metadaten für Bilder {#getting-asset-metadata-for-images}

Mit `image_info` können Sie Metadaten für ein hochgeladenes Asset abrufen, wie im nachfolgenden Beispiel gezeigt:

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Hier ein Beispiel für eine erfolgreiche Antwort:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>image_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>More information on 1442564.tif</title> 
            <message> 
            File created on Tue Sep 08 19:02:04 CDT 2009, File Size = 243494 bytes 
            <imageFormat>Tiff</imageFormat> 
            <colorSpace>Rgb</colorSpace> 
            <width>686</width> 
            <height>457</height> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

Folgende Felder können Sie in der URL-Anfragezeichenfolge zum Abrufen von Informationen für ein Asset verwenden:

| URL-Parameter | Erforderlich oder optional | Wert |
|--- |--- |--- |
| op | Erforderlich | image_info |
| shared_secret | Erforderlich | Der gemeinsame geheime Schlüssel für das Unternehmen. |
| image_name | Erforderlich | Name des Bildes. |

**Beispiel-URL:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Zulässige HTTP-Methode:**

GET und POST

## Hochladen von Vektor-Assets {#uploading-a-vector-asset}

Wenn Sie ein Upload-Token abgerufen haben, das für eine bestimmte Zeitspanne gültig ist, können Sie ein Vektor-Asset hochladen. Sie laden das Asset mit der POST-Methode als mehrteilige Formulardaten hoch, während Sie die übrigen Werte als URL-Anfragezeichenfolge senden, wie im nachfolgenden Beispiel gezeigt:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

Siehe [Abrufen des Upload-Tokens](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Siehe [Anfordern eines gemeinsamen geheimen Schlüssels](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Sie können auch andere optionale Werte als URL-Anfragezeichenfolgen senden, wie das nachfolgende Beispiel zeigt:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

The `file_limit` parameter specifies the file-size limit in bytes. Der Parameter `file_exts` gibt die für das Hochladen zulässigen Erweiterungen des Dateinamens an. Diese beiden Werte sind optional.

In der Anwendung sind globale Beschränkungen für die maximale Dateigröße und zulässigen Dateierweiterungen festgelegt. Wenn es sich bei der von Ihnen gesendeten Anforderung um eine Untergruppe der globalen Beschränkungen handelt, wird diese berücksichtigt. Die globalen Beschränkungen lauten wie folgt:

| Globale Beschränkung | Wert |
|--- |--- |
| Dateigröße für alle Clients | 20 MB |
| Unterstützte Vektordateiformate zum Hochladen | AI, EPS, PDF (nur, wenn das PDF-Dokument zuvor in Adobe Illustrator CS6 geöffnet und gespeichert wurde) |

Mit dem folgenden HTML-Formular können Benutzer Assets hochladen. In dem Formular wird der Benutzer aufgefordert, die folgenden Informationen einzugeben:

* Einen Unternehmensnamen.
* Ein Upload-Token.
* Eine Beschränkung für die Dateigröße.
* Eine Liste mit den Erweiterungen für Dateinamen.
* Gibt an, ob das Profil und der Dateiname des Assets beibehalten werden sollen.
* Gibt an, ob der Hintergrund &quot;Aussparen&quot;verwendet werden soll. Wenn Sie &quot;Hintergrund aussparen&quot;aktivieren, legen Sie die Methode &quot;Ecke&quot;, &quot;Toleranz&quot;und &quot;Füllmethode&quot;fest. Siehe Hintergrund aussparen in den [Bildbearbeitungsoptionen beim Hochladen](image-editing-options-upload.md#image-editing-options-at-upload).
* Den Namen der hochzuladenden Datei

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment&gt; elements under &lt;adobefig&gt;.</p>

 -->

![]()

Der folgende HTML-Code wird angezeigt, wenn Sie im Browserfenster mit der rechten Maustaste klicken und anschließend für das in der Abbildung dargestellte Formular auf **„Quelltext anzeigen“** klicken. Der Code enthält die URL-Anfragezeichenfolge und die POST-Methode, die ausgeführt werden, wenn der Benutzer auf **„Absenden“** klickt.

```as3
<body> 
<script language="javascript"> 
function uploadImage() 
{ 
document.image_upload.action="vector?op=upload&company_name="+document.image_upload.company_name.value+"&upload_token="+document.image_upload.upload_token.value+"&file_limit="+document.image_upload.file_limit.value+"&file_exts="+document.image_upload.file_exts.value; 
return true; 
} 
</script> 
<form method="POST" enctype="multipart/form-data" name="image_upload" id="image_upload" onSubmit="return uploadImage();"> 
<table> 
<tr><td colspan="2"><strong> UGC Vector Upload Test Page: </strong></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr><td><strong> Company Name</strong></td><td><input type="text" size="40" name="company_name"></td></tr> 
<tr><td><strong> Upload Token </strong></td><td><input type="text" size="40" name="upload_token"></td></tr> 
<tr><td><strong> File Size Limit (in bytes) </strong></td><td><input type="text" size="40" name="file_limit"> bytes</td></tr> 
<tr><td><strong> File Extensions allowed </strong></td><td><input type="text" size="40" name="file_exts"></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>File to upload: : </strong></td> 
<td><input name="filename" type="file" id="filename" size="58" maxlength="1024" /></td> 
</tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>Click Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

Um die XML-Antwort im Internet Explorer anzuzeigen, klicken Sie auf **„Ansicht“** > **„Quelltext“**. Um die XML-Antwort in Firefox anzuzeigen, klicken Sie auf **„Ansicht“** > **„Seitenquelltext anzeigen“**. Zur Anzeige von XML-Antworten wird Firefox empfohlen.

Hier eine Beispielantwort für einen erfolgreiche Upload:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
    <scene7> 
    <user_generated_content> 
    <response> 
    <serviceName>User Generated Content -Vector</serviceName> 
    <version>1.0.0</version> 
    <operationName>upload</operationName> 
    <serviceStatus>SUCCESS</serviceStatus> 
    <title>Your file has been uploaded Successfully.</title> 
    <message> 
    <url>https://s7w2p1.scene7.com/is/agm</url> 
    <path>W2PTest/ugc/8875744.fxg</path> 
    <fullurl> 
        https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg 
    </fullurl> 
</message> 
</response> 
</user_generated_content> 
</scene7>
```

>[!NOTE]
>
>Das hochgeladene Asset (AI, EPS, PDF usw.) wird ins FXG-Format umgewandelt und mit der Antwort wird eine direkte Verknüpfung zu diesem FXG-Asset gesendet.

Das Asset kann wie jede andere Web-to-Print-Ressource gehandhabt werden; Sie können auch Verarbeitungsanfragen darauf anwenden. Beispielsweise wandelt die folgende URL eine FXG-Ressource in ein png-Bild mit 500x500 Pixeln um.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Senden Sie das hochzuladende Asset mit der POST-Methode als mehrteilige Formulardaten, während Sie die übrigen Werte als URL-Anfragezeichenfolge senden. Folgende Felder können Sie in der URL-Anfragezeichenfolge zum Hochladen eines Assets verwenden:

| URL-Parameter | Erforderlich oder optional | Wert |
|--- |--- |--- |
| op | Erforderlich | Hochladen |
| upload_token | Erforderlich | Upload-Token für den gemeinsamen geheimen Schlüssel für das Unternehmen. |
| company_name | Erforderlich | Name des hochladenden Unternehmens. |
| file_limit | Optional | Maximale Dateigröße (in Byte) für das Asset. |
| file_exts | Optional | Liste der zulässigen Erweiterungen für die Asset-Datei. |

>[!NOTE]
>
>Das hochzuladende Asset muss als einziges Feld in einer mehrteiligen POST-Anfrage hochgeladen werden.

**Beispiel-URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Zulässige HTTP-Methode:**

POST
