---
title: Upgrade-Bereitschaft
description: Eine Checkliste zur Upgrade-Bereitschaft, wenn Sie von  [!DNL Adobe Dynamic Media Classic] auf [!DNL Dynamic Media] auf [!DNL Adobe Experience Manager] wechseln möchten.
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 1%

---

# Checkliste zur Upgrade-Bereitschaft

Verwenden Sie die folgende Checkliste, um ein Upgrade von [!DNL Dynamic Media Classic] auf [!DNL Dynamic Media] vorzubereiten.

|  | Aufgabe | Beschreibung |
| :--- | :--- | --- |
| **Phase 1: Lizenzierung** | Vertrag ausführen | Je nach Traffic und Speicher arbeitet das Adobe-Account-Team mit Ihnen zusammen, um von der [!DNL Dynamic Media Classic] -Lizenz zu wechseln und die [!DNL Dynamic Media] -Lizenz zu verlängern. |
| **Phase 2: Vorbereitung** | Überprüfen der Funktionsnutzung | Vergewissern Sie sich, dass die in [!DNL Dynamic Media Classic] verwendeten Funktionen in [!DNL Dynamic Media] verfügbar sind. Siehe Seite [Funktionsvergleich](/help/using/upgrade-feature-comparison.md) . Zu den wichtigsten Funktionen, die noch nicht in [!DNL Dynamic Media] verfügbar sind, zählen:<br> ・ Visual Configurator (Image Author, Image Render).<br> ・ Bildvorlagen (1:1-Vorlagen).<br> E-Kataloge ・.<br>Wenn die oben genannten Funktionen verwendet werden, kann das Upgrade dennoch unter der Annahme durchgeführt werden, dass auf diese Funktionen über [!DNL Dynamic Media Classic] zugegriffen werden kann. |
|   | Identifizieren von Assets | Suchen und bereiten Sie Assets und Vorgaben für die Aktualisierung vor. |
| **Phase 3: Umgebung** | Upgrade [!DNL Adobe Experience Manager] | Alle Instanzen von [!DNL Adobe Experience Manager] müssen auf die neueste Version aktualisiert werden. |
|   | Einrichten [!DNL Dynamic Media] | Adobe Consulting oder Partner konfiguriert [!DNL Dynamic Media] mit Ihren Anmeldedaten. |
| **Phase 4: Upgrade** | Replizieren von Assets | Während des Aktualisierungsprozesses werden bestimmte [!DNL Dynamic Media Classic] -Assets nach Dynamic Media repliziert. |
| **Phase 5: Administrative Einrichtung** | Einrichten von Benutzern und Berechtigungen | Erstellen Sie Benutzer und gewähren Sie entsprechende Berechtigungen. |
|   | Videokodierungsprofile einrichten | Erstellen Sie Videokodierungsprofile. |
|   | Einrichten von Viewer-Vorgaben | Erstellen von Viewer-Vorgaben. |
|   | Festlegen von Bildvorgaben | Einrichten von Bildvorgaben. |
| **Phase 6: Validierung** | Validierung | Überprüfen Sie Anwendungsfälle, Assets, Links und APIs. |
