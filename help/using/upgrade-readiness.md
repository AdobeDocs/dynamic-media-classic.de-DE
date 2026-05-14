---
title: Upgrade-Bereitschaft
description: Eine Checkliste für die Upgrade-Bereitschaft , wenn Sie von  [!DNL Adobe Dynamic Media Classic]  zu  [!DNL Dynamic Media]  wechseln  [!DNL Adobe Experience Manager].
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
autotag-review: '2026-05-13T20:16:07.073Z'
TQID: 'https://experienceleague.adobe.com/3Kcp3UwvJV8Mkzk6RBRgOJQ7JKF3Ldek-SiOeqS5EKE'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 221
ht-degree: 1%

---

# Checkliste für die Upgrade-Bereitschaft

Verwenden Sie die folgende Checkliste, um ein Upgrade von [!DNL Dynamic Media Classic] auf [!DNL Dynamic Media] zu verstehen und sich darauf vorzubereiten.

|  | Aufgabe | Beschreibung |
| :--- | :--- | --- |
| **Phase 1: Lizenzierung** | Vertrag ausführen | Basierend auf Traffic und Speicher arbeitet das Adobe Account Team mit Ihnen zusammen, um von der [!DNL Dynamic Media Classic] Lizenz zur Verlängerung der [!DNL Dynamic Media] Lizenz zu wechseln. |
| **Phase 2: Vorbereitung** | Validieren der Funktionsnutzung | Vergewissern Sie sich, dass die in [!DNL Dynamic Media Classic] verwendeten Funktionen in [!DNL Dynamic Media] verfügbar sind. Siehe Seite [Funktionsvergleich](/help/using/upgrade-feature-comparison.md). Zu den wichtigsten Funktionen, die in [!DNL Dynamic Media] noch nicht verfügbar sind, gehören die folgenden:<br>・ Visual Configurator (Image Author, Image Render).<br>・ Bildvorlagen (1:1 Templating).<br>・ eCatalogs.<br>Wenn die oben genannten Funktionen verwendet werden, kann das Upgrade dennoch unter der Annahme erfolgen, dass diese Funktionen über [!DNL Dynamic Media Classic] zugänglich wären. |
|   | Identifizieren von Assets | Suchen Sie Assets und Vorgaben, die für das Upgrade verwendet werden können, und bereiten Sie sie vor. |
| **Phase 3: Umwelt** | Upgrade-[!DNL Adobe Experience Manager] | Alle Instanzen von [!DNL Adobe Experience Manager] müssen auf die neueste Version aktualisiert werden. |
|   | Setup-[!DNL Dynamic Media] | Adobe Consulting oder Partner konfiguriert [!DNL Dynamic Media] mit Ihren Anmeldeinformationen. |
| **Phase 4: Upgrade** | Replizieren von Assets | Während des Upgrade-Prozesses werden designierte [!DNL Dynamic Media Classic]-Assets auf Dynamic Media repliziert. |
| **Phase 5: Einrichten der Verwaltung** | Einrichten von Benutzern und Berechtigungen | Erstellen Sie Benutzer und gewähren Sie entsprechende Berechtigungen. |
|   | Einrichten von Videocodierungsprofilen | Erstellen Sie Videokodierungsprofile. |
|   | Viewer-Vorgaben einrichten | Erstellen Sie Viewer-Vorgaben. |
|   | Festlegen von Bildvorgaben | Einrichten von Bildvorgaben. |
| **Phase 6: Validierung** | Validierung | Überprüfen Sie Anwendungsfälle, Assets, Links und APIs. |
