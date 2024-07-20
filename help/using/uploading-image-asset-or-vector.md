---
title: Hochladen eines Rasterbild-Assets
description: Erfahren Sie, wie Sie ein Rasterbild-Asset in Adobe Dynamic Media Classic hochladen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: 2ef78fe6-1e7c-4f48-86da-137ddaa55bbf
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 51%

---

# Hochladen eines Rasterbild-Assets {#uploading-an-image-asset-or-a-vector-asset}

Bevor Sie ein Bild-Asset hochladen können, fordern Sie zunächst einen gemeinsamen geheimen Schlüssel an. Mit diesem gemeinsamen geheimen Schlüssel können Sie ein Upload-Token abrufen. Anschließend verwenden Sie das Upload-Token, um Rasterbild-Assets hochzuladen.

>[!IMPORTANT]
>
>Ab dem 1. Mai 2023 stehen UGC-Assets in Dynamic Media bis zu 60 Tage ab dem Datum des Uploads zur Verfügung. Nach 60 Tagen werden die Assets entfernt.

>[!NOTE]
>
>Die Unterstützung für neue oder vorhandene UGC-Vektor-Assets in Adobe Dynamic Media Classic wurde am 30. September 2021 eingestellt.

## Anfordern eines gemeinsamen geheimen Schlüssels {#requesting-a-shared-secret-key}

Fordern Sie einen *gemeinsamen geheimen Schlüssel* von [ an, indem Sie die Admin Console verwenden, um einen Support-Fall zu erstellen.](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) Fordern Sie im Fall des technischen Supports einen gemeinsam genutzten geheimen Schlüssel an.

Geben Sie in der E-Mail-Nachricht den Unternehmensnamen an, den Sie verwenden möchten, um Bild-Assets hochzuladen. Nachdem Sie den Schlüssel von Adobe Dynamic Media Classic erhalten haben, speichern Sie ihn lokal für die zukünftige Verwendung.

## Upload-Token abrufen {#retrieving-the-upload-token}

Das *Upload-Token* stellt sicher, dass niemand denselben gemeinsamen geheimen Schlüssel zum Hochladen von Assets verwenden kann. Außerdem stellt es sicher, dass der Upload zulässig ist und von einer vertrauenswürdigen Quelle stammt.

Das Upload-Token besteht aus einer alphanumerischen Zeichenfolge, die nur für eine begrenzte Zeitspanne gültig ist. Verwenden Sie die folgenden URLs und ersetzen Sie den gemeinsam genutzten geheimen Schlüssel, damit Sie das Upload-Token abrufen können.

* Rasterbild
  `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`In diesem Beispiel lautet der Schlüssel für den gemeinsamen geheimen Schlüssel `fece4b21-87ee-47fc-9b99-2e29b78b602`

<!-- * Vector
  `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`In this example, the shared-secret key is `2d19f60e-890a-4e79-a1a5-9ac2875429b9` -->

Standardmäßig läuft das Upload-Token 5 Minuten (300 Sekunden) nach dem Abrufen ab. Um mehr Zeit anzufordern, fügen Sie `expires` in die URL ein und geben Sie die benötigte Zeit in Sekunden an. So wird bei der folgenden URL für ein Beispielbild ein Upload-Token abgerufen, das 1800 Sekunden gültig ist:

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

Die erfolgreiche Antwort für Bilder sieht in etwa wie folgt aus:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
        <serviceName>User Generated Content: Images</serviceName> 
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
| --- | --- | --- |
| op | Erforderlich | get_uploadtoken |
| shared_secret | Erforderlich | Der gemeinsam genutzte geheime Schlüssel für das Unternehmen, das den Upload durchführt. |
| expires | Optional | Anzahl der Sekunden, die das Upload-Token gültig ist. Der Standardwert beträgt 300 Sekunden, falls nicht anders angegeben. |

**Beispiel-Rasterbild-URL:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000` -->

**Zulässige HTTP-Methoden:**
`GET` und `POST`

Sie können nun ein Bild-Asset hochladen.

Siehe [Hochladen eines Bild-Assets](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## Hochladen eines Rasterbild-Assets {#uploading-an-image-asset}

Wenn Sie ein Upload-Token abgerufen haben, das für eine bestimmte Zeitspanne gültig ist, können Sie ein Bild-Asset hochladen. Sie laden das Asset mit der POST-Methode als mehrteilige Formulardaten hoch, während Sie die übrigen Werte als URL-Anfragezeichenfolge senden, wie im nachfolgenden Beispiel gezeigt:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

Die Felder `upload_token` und `company_name` sind erforderlich.

Siehe [Abrufen des Upload-Tokens](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

Siehe [Abrufen eines gemeinsamen geheimen Schlüssels](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

Sie können auch andere optionale Werte als URL-Anfragezeichenfolgen senden, wie das nachfolgende Beispiel zeigt:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

Der Parameter `file_limit` gibt die maximale Dateigröße in Byte an. Der Parameter `file_exts` gibt die Dateinamenerweiterungen an, die hochgeladen werden dürfen. Diese beiden Werte sind optional.

In der Anwendung sind globale Beschränkungen für die maximale Dateigröße und zulässigen Dateierweiterungen festgelegt. Wenn es sich bei dem, was Sie in der Anfrage gesendet haben, um eine Untergruppe der globalen Beschränkungen handelt, wird dies berücksichtigt. Die globalen Beschränkungen lauten wie folgt:

| Globale Beschränkung | Wert |
| --- | --- |
| Dateigröße für alle Clients | 20 MB |
| Unterstützte Bilddateiformate zum Hochladen | BMP, GIF, JPG, PNG, PSD, TIFF |

Mit dem folgenden HTML-Formular können Benutzer Assets hochladen. In dem Formular wird der Benutzer aufgefordert, die folgenden Informationen einzugeben:

* Ein Unternehmensname.
* Ein Upload-Token.
* Eine Dateigrößenbeschränkung.
* Eine Liste der Dateinamenerweiterungen.
* Gibt an, ob das Farbprofil und der Dateiname des Assets beibehalten werden sollen.
* Gibt an, ob ein Knock-out-Hintergrund verwendet werden soll. Wenn Sie &quot;Hintergrund aussparen&quot;aktivieren, legen Sie die Methode &quot;Ecke&quot;, &quot;Toleranz&quot;und &quot;Füllung&quot;fest.
Siehe &quot;Hintergrund aussparen&quot;in den [Optionen zur Feinabstimmung des Bildes beim Hochladen](image-editing-options-upload.md#image-editing-options-at-upload).
* Der Name der hochzuladenden Datei.

Sie können den mit dem obigen Formular verknüpften HTML-Quellcode anzeigen, indem Sie [https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html) auswählen

Klicken Sie in Firefox mit der rechten Maustaste in das Browserfenster und wählen Sie dann **[!UICONTROL Seite Source anzeigen]** aus. Der Code zeigt die entsprechende URL-Abfragezeichenfolge und die POST an, die ausgeführt wird, wenn der Benutzer **[!UICONTROL Senden]** auswählt.

Um die XML-Antwort in Internet Explorer anzuzeigen, gehen Sie zu **[!UICONTROL Ansicht]** > **[!UICONTROL Source]**. Um die XML-Antwort in Firefox anzuzeigen, gehen Sie zu &quot;**[!UICONTROL Tools]**&quot;> &quot;**[!UICONTROL Browser-Tools]**&quot;> &quot;**[!UICONTROL Web Developer Tools]**&quot;. Zur Anzeige von XML-Antworten wird Firefox empfohlen.

Hier eine Beispielantwort für einen erfolgreiche Upload:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
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

Das Asset kann wie jede andere Image-Server-Ressource gehandhabt werden; Sie können auch Verarbeitungsanfragen darauf anwenden. Beispielsweise fordert die folgende URL ein Asset an, das bis zur angegebenen Breite und Höhe gestreckt ist.

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

Senden Sie das hochzuladende Asset mit der POST-Methode als mehrteilige Formulardaten, während Sie die übrigen Werte als URL-Anfragezeichenfolge senden. Folgende Felder können Sie in der URL-Anfragezeichenfolge zum Hochladen eines Assets verwenden:

| URL-Parameter | Erforderlich oder optional | Wert |
| --- | --- | --- |
| `op` | Erforderlich | Hochladen |
| `upload_token` | Erforderlich | Laden Sie ein Token für den gemeinsamen geheimen Schlüssel hoch, der mit dem Unternehmen verknüpft ist. |
| `company_name` | Erforderlich | Name des hochladenden Unternehmens. |
| `file_limit` | Optional | Maximale Dateigröße (in Byte) für das Asset. |
| `file_exts` | Optional | Liste der zulässigen Erweiterungen für die Bild-Asset-Datei. |
| `preserve_colorprofile` | Optional | Behält eingebettete Farbprofile bei der Konvertierung der hochgeladenen Datei in das PTIFF-Format bei. Mögliche Werte sind „true“ oder „false“. Der Standardwert ist „false“. |
| `preserve_filename` | Optional | Behält den Dateinamen des hochgeladenen Assets bei. Mögliche Werte sind „true“ oder „false“. Der Standardwert ist „false“. |

>[!NOTE]
>
>Das hochzuladende Asset muss als einziges Feld in einer mehrteiligen POST-Anfrage hochgeladen werden.

**Beispiel-URL:**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**Zulässige HTTP-Methode:**

POST

### Abrufen von Asset-Metadaten für Bilder {#getting-asset-metadata-for-images}

Sie können `image_info` verwenden, um Metadaten für ein hochgeladenes Asset abzurufen, wie im folgenden Beispiel gezeigt:

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

Ein Beispiel für eine erfolgreiche Antwort wird in etwa wie folgt angezeigt:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
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
| --- | --- | --- |
| `op` | Erforderlich | image_info |
| `shared_secret` | Erforderlich | Der Schlüssel, der für das Unternehmen gemeinsam geheim gehalten wird. |
| `image_name` | Erforderlich | Name des Bildes. |

**Beispiel-URL:**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**Zulässige HTTP-Methode:**

GET und POST

<!-- ## Upload a vector asset {#uploading-a-vector-asset}

>[!IMPORTANT]
>
>Support for new or existing UGC vector image assets in Adobe Dynamic Media Classic end on September 30, 2021.

After you retrieve an upload token that is valid for a specific amount of time, you can upload a vector asset. You upload the asset as a multipart/form post while sending the rest of the values as a URL query string, as shown in this example:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

See [Retrieve the upload token](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

See [Retrieve a shared-secret key](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

You can also send other optional values as URL query strings, as in this example:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

The `file_limit` parameter specifies the file-size limit in bytes. The `file_exts` parameter specifies the filename extensions that are allowed for upload. Both of these values are optional.

A global limit is set in the application for the file size limit and the filename extensions allowed. If what you send in the request is a subset of the global limits, it is honored. The global limits are the following:

| Global limit | Value |
| --- | --- |
| File size for all clients | 20 MB |
| Supported vector file formats for upload | AI, EPS, PDF (only when the PDF is previously opened and saved in Adobe Illustrator CS6) |

The following HTML form lets a user upload an asset. The form asks the user to enter the following information:

* A company name.
* An upload token.
* A file size limit.
* A list of filename extensions.
* Whether to preserve the color profile and file name associated with the asset.
* Whether to use Knockout Background. If you enable Knockout Background, set the Corner, Tolerance, and Fill Method.
See Knockout Background in [Image fine-tuning options at upload](image-editing-options-upload.md#image-editing-options-at-upload).
* The name of the file to upload.

The following HTML code is displayed when you right-click in the browser window, and then select **[!UICONTROL View Source]** for the form shown in the example. The code shows the corresponding URL query string and the POST method that are run when the user selects **[!UICONTROL Submit]**.

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
<td><strong>Select Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

To view the XML response in Internet Explorer, go to **[!UICONTROL View]** > **[!UICONTROL Source]**. To view XML response in Firefox, go to **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Page Source]**. Firefox is recommended for viewing XML responses.

The following is a sample response from a successful upload:

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
>The uploaded asset (AI, EPS, PDF so on) is converted to the FXG format and the response sends a direct link to that FXG asset.

The asset is like any other Web-to-print resource; you apply processing queries to it. For example, the following URL converts an FXG resource into a 500x500 png image.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Send the asset to upload as a multipart/form post while sending the rest of the values as a URL query string. You can use the following fields in the URL query string to upload an asset:

| URL Parameter | Required or Optional | Value |
| --- | --- | --- |
| `op` | Required | upload |
| `upload_token` | Required | Upload token for the shared-secret key associated with the company. |
| `company_name` | Required | Name of the company performing the upload. |
| `file_limit` | Optional | File size limit, in bytes, for the asset. |
| `file_exts` | Optional | List of allowable extensions for the asset file. |

>[!NOTE]
>
>You are required to send the asset to be uploaded as the only field in a multipart POST request.

**Sample URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Allowed HTTP method:**

POST
 -->