---
title: Über benutzergenerierte Inhalte in Adobe Dynamic Media Classic
description: Eine Einführung in benutzergenerierte Inhalte.
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/user_generated_content
feature: Dynamic Media Classic
role: Admin,User
exl-id: 14729192-7b9d-4f42-99da-6564a3f35959
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:34:44.287Z'
TQID: 'https://experienceleague.adobe.com/SwNEO6U33qx45AECK79nff9f9kABWuOdq91d4X8SHd0'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: fb3cf42c8b9b0b90e2378beedce15a20c086f1a9
workflow-type: tm+mt
source-wordcount: 173
ht-degree: 29%

---

# Über benutzergenerierte Inhalte in Adobe Dynamic Media Classic {#about-user-generated-content}

Bei der benutzergenerierten Inhalte (UGC) werden Assets in ein dediziertes [!DNL Adobe Dynamic Media Classic]-Speicher-Repository hochgeladen und die zugehörigen Vorgänge ausgeführt.

UGC unterstützt Rasterbilddateiformate BMP, GIF, JPG, PNG, PSD, TIFF.

>[!IMPORTANT]
>
>Ab dem 1. Mai 2023 bleiben UGC-Assets in Dynamic Media bis zu 60 Tage ab dem Datum des Uploads verfügbar. Nach 60 Tagen werden die Assets entfernt.

<!-- * Vector: AI, EPS (EPS files from Adobe Illustrator 2018 are not supported), PDF (only when the PDF file is previously opened and saved in Adobe Illustrator CS6) -->

>[!NOTE]
>
>Die Unterstützung für neue oder vorhandene UGC-Vektorbild-Assets in Adobe Dynamic Media Classic endete am 30. September 2021.

Vor dem Hochladen von Assets müssen Sie einen Schlüssel mit einem gemeinsamen geheimen Schlüssel erhalten. Verwenden Sie diesen Schlüssel, um ein Upload-Token abzurufen. Sie senden das Upload-Token, wenn Sie Assets hochladen und andere Aufgaben für benutzergenerierte Inhalte ausführen.

Wenn Sie einen gemeinsamen geheimen Schlüssel und ein Upload-Token erhalten haben, können Sie die folgenden Vorgänge für benutzergenerierte Inhalte ausführen:

* Asset hochladen.
* Abrufen von Asset-Metadaten für Bilder
* Löschen eines hochgeladenen Assets.
* Erhalten Sie Informationen über die Speicherplatznutzung eines Unternehmens.
