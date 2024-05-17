---
title: Erstellen und Verwalten von Media Portal-Gruppen
description: Erfahren Sie, wie Sie Media Portal-Gruppen in Adobe Dynamic Media Classic erstellen und verwalten.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 49%

---

# Erstellen und Verwalten von Media Portal-Gruppen{#creating-and-managing-media-portal-groups}

Mithilfe von *Gruppen* können Sie die Media Portal-Benutzer leichter verwalten. Um auf ein Asset zugreifen zu können, muss ein Benutzer Mitglied mindestens einer Gruppe mit den erforderlichen Berechtigungen für dieses Asset sein. Wenn Sie einen Benutzer hinzufügen, weisen Sie ihm eine oder mehrere Rollen zu. Dabei gewähren Sie dem Benutzer Zugriff auf Ordner, denen die Gruppe zugewiesen wurde. Sie können auch angeben, welche Bildvorgaben einer Gruppe zur Verfügung stehen.

## Verwenden Sie Gruppen, um den Zugriff auf Ordner, Assets und Bildvorgaben zu beschränken. {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

Wenn Sie Gruppen erstellen, können Sie Zugriffsrechte auf unterschiedlichen Ebenen gewähren. Für jede Gruppe weisen Sie Lese-, Schreib- und Löschberechtigungen für unterschiedliche Ordner und Assets in den Ordnern zu. Außerdem legen Sie fest, welche Bildvorgaben der Gruppe zur Verfügung stehen. Anschließend weisen Sie Benutzer den Gruppen zu. Ein Benutzer kann Mitglied mehrerer Gruppen sein. Durch das Gruppenkonzept können Sie flexibel Zugriffsrechte für einen Teil des Gesamtinhalts zuweisen.

Wenn Sie einem Asset oder Ordner ausdrücklich keine Gruppenberechtigung erteilen, erbt dieses Asset oder Ordner die Berechtigungen, die Sie seinem übergeordneten Ordner (dem Ordner darüber in der Ordnerhierarchie) zugewiesen haben. Wenn Sie einem Ordner Rechte zuweisen, werden dieselben Rechte für sämtliche darin enthaltenen Ordner übernommen.

>[!NOTE]
>
>Benutzer können mehreren Gruppen angehören. Wenn ein Benutzer zwei Gruppen mit unterschiedlichen Zugriffsrechten für einen Ordner angehört, werden jeweils die höchsten Zugriffsrechte angewendet.

## Hinzufügen einer Gruppe {#adding-a-group}

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Media Portal-Einrichtung]** > **[!UICONTROL Gruppen]**.
1. Auswählen **[!UICONTROL Hinzufügen]**.
1. Geben Sie im Dialogfeld Gruppe hinzufügen im Feld Gruppenname einen Namen für die Gruppe ein und wählen Sie dann **[!UICONTROL Gruppe hinzufügen]**.
1. Bei Bedarf können Sie die Kontrollkästchen neben den Namen von Benutzern aktivieren, um diese Benutzer der neuen Gruppe hinzuzufügen.
1. Wenn Sie jetzt Zugriffsberechtigungen festlegen möchten, wählen Sie die **[!UICONTROL Asset-Zugriffsberechtigungen]** und geben Sie die gewünschten Optionen an.

   Siehe [Einrichten von Asset-Zugriffsberechtigungen für eine Gruppe](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. Sie können auswählen, welche Bildvorgaben für die Gruppe verfügbar sind. Klicken Sie einfach auf **[!UICONTROL Zugriffsberechtigungen für Bildvorgaben]** und wählen Sie Bildvorgaben aus, die die Gruppe verwenden kann.

   Siehe [Auswählen der Bildvorgabezugriffsberechtigungen für eine Gruppe](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Auswählen **[!UICONTROL Schließen]**.

## Einrichten von Asset-Zugriffsberechtigungen für eine Gruppe {#establishing-asset-access-permissions-for-a-group}

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Media Portal-Einrichtung]** > **[!UICONTROL Gruppen]**.
1. Führen Sie auf der Seite „Gruppen“ einen der folgenden Schritte aus:

   * Um eine Gruppe hinzuzufügen und Berechtigungen festzulegen, wählen Sie **[!UICONTROL Hinzufügen]**. Geben Sie im Dialogfeld Gruppe hinzufügen einen Namen für die Gruppe ein und wählen Sie **[!UICONTROL Gruppe hinzufügen]** und fügen Sie Benutzer zur Gruppe hinzu.
   * Um die Berechtigungen einer Gruppe zu bearbeiten, wählen Sie die Gruppe aus und klicken Sie auf **[!UICONTROL Bearbeiten]**.

1. Wählen Sie im Dialogfeld Gruppe hinzufügen oder Gruppe bearbeiten die **[!UICONTROL Asset-Zugriffsberechtigungen]** Registerkarte. Über die Kontrollkästchen auf der rechten Seite der Registerkarte können Sie Rechte zum Lesen, Schreiben und Löschen für Ordner und Assets festlegen. Im linken Fensterbereich können Sie Ordner und Unterordner erweitern und minimieren.
1. Um Ordnern oder einzelnen Assets Rechte zuzuweisen, wählen Sie den Ordner im linken Fensterbereich aus. Der Inhalt des Ordners wird im rechten Fensterbereich angezeigt. Weisen Sie dann der Gruppe Berechtigungen zu, indem Sie die Felder für die entsprechenden Dateien auswählen. Oder wählen Sie die Ordner im rechten Bereich aus.

   In dieser Tabelle werden verschiedenen Aufgaben Berechtigungen zum Lesen, Schreiben und Löschen zugewiesen.

   | Aufgabe | Lesen | Schreiben | Löschen |
   | --- | --- | --- | --- |
   | Ordner und Dateien durchsuchen | X | | |
   | Dateien bearbeiten (zuschneiden, scharfzeichnen, anpassen) | | X | |
   | Dateinamen ändern | | X | |
   | Dateien in andere Ordner verschieben | | X | |
   | Dateien umbenennen | | X | |
   | Dateien löschen | | | X |

1. Auswählen **[!UICONTROL Schließen]**.

>[!NOTE]
>
>Zugriffsrechte werden eingerichtet, wenn Sie ein Kästchen aktivieren. Wenn Sie einem Ordner Berechtigungen zugewiesen haben, erhalten dessen Unterordner und alle darin enthaltenen Dateien dieselben Berechtigungen wie der übergeordnete Ordner. Sie können jedoch auch abweichende Rechte für einzelne Unterordner und Asset-Dateien festlegen.

## Auswählen der Bildvorgabezugriffsberechtigungen für eine Gruppe

Wählen Sie Bildvorgabezugriffsberechtigungen für eine Gruppe, wenn Sie festlegen möchten, welche Bildvorgaben den Gruppenmitgliedern beim Exportieren von Assets mit dem Media Portal zur Verfügung stehen sollen.

Siehe auch [Festlegen von Exportoptionen, die für Media Portal-Benutzer verfügbar sind](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

**So wählen Sie Zugriffsberechtigungen für Bildvorgabe für eine Gruppe aus:**

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Media Portal-Einrichtung]** > **[!UICONTROL Gruppen]**.
1. Führen Sie auf der Seite „Gruppen“ einen der folgenden Schritte aus:

   * Um eine Gruppe hinzuzufügen und anzugeben, welche Bildvorgaben ihr zur Verfügung stehen, wählen Sie **[!UICONTROL Hinzufügen]**. Geben Sie im Dialogfeld Gruppe hinzufügen einen Namen für die Gruppe ein und wählen Sie **[!UICONTROL Gruppe hinzufügen]** und fügen Sie Benutzer zur Gruppe hinzu.
   * Um die Bildvorgabenoptionen einer Gruppe zu bearbeiten, wählen Sie die Gruppe aus und klicken Sie auf **[!UICONTROL Bearbeiten]**.

1. Wählen Sie im Dialogfeld Gruppe hinzufügen oder Gruppe bearbeiten die **[!UICONTROL Zugriffsberechtigungen für Bildvorgaben]** Registerkarte.
1. Um festzulegen, welche Vorgaben für Media Portal-Benutzer beim Exportieren von Assets verfügbar sind, wählen Sie Bildvorgaben aus oder deaktivieren Sie sie.
1. Auswählen **[!UICONTROL Schließen]**.

## Bearbeiten und Löschen von Gruppen {#edit-and-delete-groups}

1. Navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Media Portal-Einrichtung]** > **[!UICONTROL Gruppen]**.
1. Wählen Sie auf der Seite „Gruppenliste“ eine Gruppe aus und bearbeiten oder löschen Sie sie.

   **Eine Gruppe bearbeiten**: Auswählen **[!UICONTROL Bearbeiten]** und wählen Sie dann die Optionen im Dialogfeld Gruppe bearbeiten aus.

   **Gruppe löschen**: Auswählen **[!UICONTROL Löschen]**.
