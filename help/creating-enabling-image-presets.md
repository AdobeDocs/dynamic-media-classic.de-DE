---
title: Erstellen und Aktivieren von Bildvorgaben
description: Erfahren Sie, wie Sie Bildvorgaben in Adobe Dynamic Media Classic erstellen und aktivieren.
uuid: 62cfc6fa-da91-4c42-a3ed-10956384d633
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 84257b2a-681c-4fe9-a6e5-3633c1d61d8c
feature: Dynamic Media Classic,Collaboration,Image Presets,Asset Management
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 72%

---

# Erstellen und Aktivieren von Bildvorgaben{#creating-and-enabling-image-presets}

Wenn Benutzer Bildassets aus Media Portal exportieren, können sie im Dialogfeld „Ausgewählte Assets exportieren“ eine Bildvorgabe auswählen. Eine Bildvorgabe ist eine Sammlung vordefinierter Einstellungen, mit denen Größe, Qualität, Format, Auflösung und andere Darstellungsaspekte für ein Bild beim Exportieren festgelegt werden.

Mit Bildvorgaben können Media Portal-Administratoren kontrollieren, wie Bilder beim Exportieren umformatiert werden. Bildvorgaben formatieren Bilder gemäß den Spezifikationen Ihres Unternehmens neu, wenn Benutzer Bilder aus der Adobe Dynamic Media Classic exportieren. Benutzer müssen Bilder also nicht selbst neu formatieren, sondern können sie entsprechend den präzisen Einstellungen einer Bildvorgabe exportieren.

Die folgenden Einschränkungen gelten, wenn Sie Bild-Assets exportieren:

* Die Breite x Höhe muss kleiner als oder gleich 100 MB pro Bild sein. Beispielsweise kann das Bild nicht 10K x 10K oder eine Seitenverhältnisvariation darunter wie z. B. 8K x 12K überschreiten.
* Pro Exportauftrag gibt es eine maximale Dateigröße von 1 GB.
* Sie können maximal 500 Assets pro Exportauftrag haben.

>[!NOTE]
>
>Diese Einschränkungen gelten nur für den Export von abgeleiteten Bild-Assets, nicht für den Export von Primärdateien.

Hinweise zum Erstellen von Bildvorgaben finden Sie unter [Bildvorgaben](application-setup.md#image_presets).

Informationen dazu, wie Sie Benutzern erlauben, beim Exportieren von Bildern Bildvorgaben auszuwählen, finden Sie unter [Festlegen, welche Exportoptionen Media Portal-Benutzern zur Verfügung stehen](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

Informationen dazu, wie Sie festlegen, welche Bildvorgaben den Mitgliedern einer Gruppe zur Verfügung stehen, finden Sie unter [Auswählen der Bildvorgabezugriffsberechtigungen für eine Gruppe](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).
