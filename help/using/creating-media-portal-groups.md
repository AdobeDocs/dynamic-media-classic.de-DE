---
title: Erstellen und Verwalten von Medienportalgruppen
description: Erfahren Sie, wie Sie Medienportalgruppen in Adobe Dynamic Media Classic erstellen und verwalten.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
topic: Administration, Collaboration
level: Intermediate
autotag-review: '2026-05-13T17:41:54.576Z'
TQID: 'https://experienceleague.adobe.com/If0j5hWmxTOGGYshsqh2sa0iM3S2SvG57iPO2rtG1lY'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: b83425ec5382ae173947fa0c9321e734f14eaced
workflow-type: tm+mt
source-wordcount: 843
ht-degree: 39%

---

# Erstellen und Verwalten von Medienportalgruppen{#creating-and-managing-media-portal-groups}

Gruppen unterstützen Sie bei der Verwaltung von Medienportal-Benutzern. Um auf ein Asset zugreifen zu können, muss ein Benutzer Mitglied mindestens einer Gruppe mit den erforderlichen Berechtigungen für dieses Asset sein. Wenn Sie einen Benutzer hinzufügen, weisen Sie ihm eine oder mehrere Rollen zu. Auf diese Weise gewähren Sie dem Benutzer Zugriff auf Ordner, denen die Gruppe zugewiesen wurde. Sie können auch angeben, welche Bildvorgaben einer Gruppe zur Verfügung stehen.

## Verwenden von Gruppen, um den Zugriff auf Ordner, Assets und Bildvorgaben einzuschränken {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

Wenn Sie Gruppen erstellen, können Sie Zugriffsrechte auf unterschiedlichen Ebenen gewähren. Für jede Gruppe weisen Sie Lese-, Schreib- und Löschberechtigungen für unterschiedliche Ordner und Assets in den Ordnern zu. Außerdem können Sie festlegen, welche Bildvorgaben für die Gruppe verfügbar sein sollen. Anschließend weisen Sie Benutzer den Gruppen zu. Ein Benutzer kann Mitglied mehrerer Gruppen sein. Die Gruppenfunktion bietet die Flexibilität, den Zugriff auf begrenzte Mengen des gesamten Inhalts zuzuweisen.

Wenn Sie ausdrücklich keine Gruppenberechtigung für ein Asset oder einen Ordner erben, erbt das Asset oder der Ordner die Berechtigungen, die Sie dem übergeordneten Ordner zugewiesen haben (dem Ordner in der Ordnerhierarchie, der sich darüber befindet). Gewähren von Berechtigungen für einen übergeordneten Ordner. Verwenden Sie diese Option, wenn Sie sicherstellen möchten, dass alle untergeordneten Ordner dieselben Berechtigungen erben.

>[!NOTE]
>
>Benutzer können mehreren Gruppen angehören. Wenn ein Benutzer zwei Gruppen mit unterschiedlichen Zugriffsberechtigungen für einen Ordner angehört, erhält er den Zugriff mit den höchsten Berechtigungen.

## Hinzufügen einer Gruppe {#adding-a-group}

1. Navigieren Sie **[!UICONTROL Setup]** > **[!UICONTROL Medienportal-Setup]** > **[!UICONTROL Gruppen]**.
1. Wählen Sie **[!UICONTROL Hinzufügen]** aus.
1. Geben Sie im Dialogfeld Gruppe hinzufügen in das Feld Gruppenname einen Namen für die Gruppe ein und wählen Sie dann **[!UICONTROL Gruppe hinzufügen]**.
1. Bei Bedarf können Sie die Kontrollkästchen neben den Namen von Benutzern aktivieren, um diese Benutzer der neuen Gruppe hinzuzufügen.
1. Wenn Sie jetzt Zugriffsberechtigungen angeben möchten, wählen Sie die Registerkarte **[!UICONTROL Asset-Zugriffsberechtigungen]** und geben Sie dann die gewünschten Optionen an.

   Siehe [Einrichten von Asset-Zugriffsberechtigungen für eine Gruppe](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. Sie können auswählen, welche Bildvorgaben der Gruppe zur Verfügung stehen sollen. Klicken Sie auf **[!UICONTROL Bildvorgabe - Zugriffsberechtigungen]** und wählen Sie die Bildvorgaben aus, die die Gruppe verwenden kann.

   Siehe [Auswählen der Bildvorgabezugriffsberechtigungen für eine Gruppe](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Wählen Sie **[!UICONTROL Schließen]** aus.

## Einrichten von Asset-Zugriffsberechtigungen für eine Gruppe {#establishing-asset-access-permissions-for-a-group}

1. Navigieren Sie **[!UICONTROL Setup]** > **[!UICONTROL Medienportal-Setup]** > **[!UICONTROL Gruppen]**.
1. Führen Sie auf der Seite „Gruppen“ einen der folgenden Schritte aus:

   * Um eine Gruppe hinzuzufügen und Berechtigungen anzugeben, wählen Sie **[!UICONTROL Hinzufügen]** aus. Geben Sie im Dialogfeld Gruppe hinzufügen einen Namen für die Gruppe ein, wählen Sie **[!UICONTROL Gruppe hinzufügen]** und fügen Sie Benutzer zur Gruppe hinzu.
   * Um die Berechtigungen einer Gruppe zu bearbeiten, wählen Sie die Gruppe aus und klicken Sie dann auf **[!UICONTROL Bearbeiten]**.

1. Wählen Sie im Dialogfeld Gruppe hinzufügen oder Gruppe bearbeiten die Registerkarte **[!UICONTROL Asset-Zugriffsberechtigungen]** aus. Über die Kontrollkästchen auf der rechten Seite der Registerkarte können Sie Rechte zum Lesen, Schreiben und Löschen für Ordner und Assets festlegen. Im linken Fensterbereich können Sie Ordner und Unterordner erweitern und minimieren.
1. Um Ordnern oder einzelnen Assets Rechte zuzuweisen, wählen Sie den Ordner im linken Fensterbereich aus. Der Inhalt des Ordners wird im rechten Fensterbereich angezeigt. Weisen Sie dann Rechte für die Gruppe zu, indem Sie die Kästchen für die entsprechenden Dateien auswählen. Oder wählen Sie die Ordner im rechten Bereich aus.

   In dieser Tabelle werden verschiedenen Aufgaben Berechtigungen zum Lesen, Schreiben und Löschen zugewiesen.

   | Aufgabe | Lesen | Schreiben | Löschen |
   | --- | --- | --- | --- |
   | Ordner und Dateien durchsuchen | X | | |
   | Dateien bearbeiten (zuschneiden, scharfzeichnen, anpassen) | | X | |
   | Dateinamen ändern | | X | |
   | Dateien in andere Ordner verschieben | | X | |
   | Dateien umbenennen | | X | |
   | Dateien löschen | | | X |

1. Wählen Sie **[!UICONTROL Schließen]** aus.

>[!NOTE]
>
>Zugriffsrechte werden eingerichtet, wenn Sie ein Kästchen aktivieren. Wenn Sie einem Ordner Rechte zuweisen, werden dieselben Rechte auch den darin enthaltenen Ordner und Dateien zugewiesen. Sie können jedoch auch abweichende Rechte für einzelne Unterordner und Asset-Dateien festlegen.

## Auswählen der Bildvorgabezugriffsberechtigungen für eine Gruppe

Wählen Sie Bildvorgabe-Zugriffsberechtigungen für eine Gruppe aus. Verwenden Sie diese Option, um festzulegen, welche Bildvorgaben für Gruppenmitglieder verfügbar sind. Verwenden Sie diese Option, wenn Assets mit Media Portal exportiert werden.

Siehe auch [Angeben der für Media Portal-Benutzer verfügbaren Exportoptionen](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

**So wählen Sie Bildvorgabe-Zugriffsberechtigungen für eine Gruppe aus:**

1. Navigieren Sie **[!UICONTROL Setup]** > **[!UICONTROL Medienportal-Setup]** > **[!UICONTROL Gruppen]**.
1. Führen Sie auf der Seite „Gruppen“ einen der folgenden Schritte aus:

   * Um eine Gruppe hinzuzufügen und anzugeben, welche Bildvorgaben verfügbar sind, wählen Sie **[!UICONTROL Hinzufügen]** aus. Geben Sie im Dialogfeld Gruppe hinzufügen einen Namen für die Gruppe ein, wählen Sie **[!UICONTROL Gruppe hinzufügen]** und fügen Sie Benutzer zur Gruppe hinzu.
   * Um die Optionen für die Bildvorgabe einer Gruppe zu bearbeiten, wählen Sie die Gruppe aus und klicken Sie dann auf **[!UICONTROL Bearbeiten]**.

1. Wählen Sie im Dialogfeld Gruppe hinzufügen oder Gruppe bearbeiten die Registerkarte **[!UICONTROL Bildvorgabe -]**) aus.
1. Um festzulegen, welche Vorgaben Benutzern von Media Portal beim Exportieren von Assets zur Verfügung stehen, wählen Sie Bildvorgaben aus bzw. heben Sie die Auswahl auf.
1. Wählen Sie **[!UICONTROL Schließen]** aus.

## Bearbeiten und Löschen von Gruppen {#edit-and-delete-groups}

1. Navigieren Sie **[!UICONTROL Setup]** > **[!UICONTROL Medienportal-Setup]** > **[!UICONTROL Gruppen]**.
1. Wählen Sie auf der Seite „Gruppenliste“ eine Gruppe aus und bearbeiten oder löschen Sie sie.

   **Gruppe bearbeiten**: Klicken Sie auf **[!UICONTROL Bearbeiten]** und wählen Sie dann die Optionen im Dialogfeld Gruppe bearbeiten aus.

   **Gruppe löschen**: Wählen Sie **[!UICONTROL Löschen]**.
