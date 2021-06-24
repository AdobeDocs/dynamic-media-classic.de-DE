---
title: Erstellen und Verwalten von Media Portal-Gruppen
description: Erfahren Sie, wie Sie Media Portal-Gruppen erstellen und verwalten.
uuid: 23f360e1-ddcb-491b-ab9f-428f3ac9c316
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 91524d36-b77a-4dc4-acba-a7bd85297e98
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Administrator,Business Practitioner
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 86%

---

# Erstellen und Verwalten von Media Portal-Gruppen{#creating-and-managing-media-portal-groups}

Mithilfe von *Gruppen* können Sie die Media Portal-Benutzer leichter verwalten. Um auf ein Asset zugreifen zu können, muss ein Benutzer Mitglied mindestens einer Gruppe mit den erforderlichen Berechtigungen für dieses Asset sein. Wenn Sie einen Benutzer hinzufügen, weisen Sie ihm eine oder mehrere Rollen zu. Dadurch gewähren Sie dem Benutzer Zugriffsrechte für die Ordner, denen die Gruppe zugewiesen wurde. Sie können auch angeben, welche Bildvorgaben einer Gruppe zur Verfügung stehen.

## Verwenden von Gruppen zum Beschränken des Zugriffs auf Ordner, Assets und Bildvorgaben {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

Wenn Sie Gruppen erstellen, können Sie Zugriffsrechte auf unterschiedlichen Ebenen gewähren. Für jede Gruppe weisen Sie Lese-, Schreib- und Löschberechtigungen für unterschiedliche Ordner und Assets in den Ordnern zu. Außerdem legen Sie fest, welche Bildvorgaben der Gruppe zur Verfügung stehen. Anschließend weisen Sie Benutzer den Gruppen zu. Ein Benutzer kann Mitglied mehrerer Gruppen sein. Durch das Gruppenkonzept können Sie flexibel Zugriffsrechte für einen Teil des Gesamtinhalts zuweisen.

Wenn Sie einem Asset oder Ordner keine Gruppenberechtigungen gewähren, erbt dieses Asset oder Ordner die Berechtigungen, die Sie seinem übergeordneten Ordner (dem Ordner darüber in der Ordnerhierarchie) zugewiesen haben. Wenn Sie einem Ordner Rechte zuweisen, werden dieselben Rechte für sämtliche darin enthaltenen Ordner übernommen.

>[!NOTE]
>
>Benutzer können mehreren Gruppen angehören. Wenn ein Benutzer zwei Gruppen mit unterschiedlichen Zugriffsrechten für einen Ordner angehört, werden jeweils die höchsten Zugriffsrechte angewendet.

## Hinzufügen einer Gruppe {#adding-a-group}

1. Klicken Sie auf **[!UICONTROL „Einstellungen“]** > **[!UICONTROL „Media Portal-Einrichtung“]** > **[!UICONTROL „Gruppen“]**.
1. Klicken Sie auf **[!UICONTROL „Hinzufügen“]**.
1. Geben Sie im Dialogfeld „Gruppe hinzufügen“ im Feld „Gruppenname“ einen Namen für die Gruppe ein und klicken Sie dann auf **[!UICONTROL „Gruppe hinzufügen“]**.
1. Bei Bedarf können Sie die Kontrollkästchen neben den Namen von Benutzern aktivieren, um diese Benutzer der neuen Gruppe hinzuzufügen.
1. Wenn Sie jetzt Zugriffsberechtigungen festlegen möchten, klicken Sie auf die Registerkarte **[!UICONTROL Asset Access Permissions]** und geben Sie dann die gewünschten Optionen an.

   Siehe [Einrichten von Asset-Zugriffsberechtigungen für eine Gruppe](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. Wenn Sie wählen möchten, welche Bildvorgaben für die Gruppe verfügbar sein sollen, klicken Sie auf die Registerkarte **[!UICONTROL „Bildvorgabezugriffsberechtigungen“]** und wählen Sie Bildvorgaben aus, die die Gruppe verwenden kann.

   Siehe [Auswählen der Bildvorgabezugriffsberechtigungen für eine Gruppe](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Klicken Sie auf **[!UICONTROL Schließen]**.

## Einrichten von Asset-Zugriffsberechtigungen für eine Gruppe {#establishing-asset-access-permissions-for-a-group}

1. Klicken Sie auf **[!UICONTROL „Einstellungen“]** > **[!UICONTROL „Media Portal-Einrichtung“]** > **[!UICONTROL „Gruppen“]**.
1. Führen Sie auf der Seite „Gruppen“ einen der folgenden Schritte aus:

   * Um eine Gruppe hinzuzufügen und Berechtigungen festzulegen, klicken Sie auf **[!UICONTROL „Hinzufügen“]**. Geben Sie im Dialogfeld „Gruppe hinzufügen“ einen Namen für die Gruppe ein, klicken Sie auf **[!UICONTROL „Gruppe hinzufügen“]** und fügen Sie der Gruppe Benutzer hinzu.
   * Um die Berechtigungen einer Gruppe zu bearbeiten, wählen Sie die Gruppe aus und klicken dann auf **[!UICONTROL „Bearbeiten“]**.

1. Klicken Sie im Dialogfeld „Gruppe hinzufügen“ bzw. „Gruppe bearbeiten“ auf die Registerkarte **[!UICONTROL „Asset-Zugriffsberechtigungen“]**. Über die Kontrollkästchen auf der rechten Seite der Registerkarte können Sie Rechte zum Lesen, Schreiben und Löschen für Ordner und Assets festlegen. Im linken Fensterbereich können Sie Ordner und Unterordner erweitern und minimieren.
1. Um Ordnern oder einzelnen Assets Rechte zuzuweisen, wählen Sie den Ordner im linken Fensterbereich aus. Der Inhalt des Ordners wird im rechten Fensterbereich angezeigt. Legen Sie dann die Rechte für die Gruppe fest, indem Sie im rechten Fensterbereich die Kontrollkästchen für die entsprechenden Dateien bzw. Ordner aktivieren.

   In dieser Tabelle werden verschiedenen Aufgaben Berechtigungen zum Lesen, Schreiben und Löschen zugewiesen.

   | Aufgabe | Lesen | Schreiben | Löschen |
   |--- |--- |--- |--- |
   | Ordner und Dateien durchsuchen | X |  |  |
   | Dateien bearbeiten (zuschneiden, scharfzeichnen, anpassen) |  | X |  |
   | Dateinamen ändern |  | X |  |
   | Dateien in andere Ordner verschieben |  | X |  |
   | Dateien umbenennen |  | X |  |
   | Dateien löschen |  |  | X |

1. Klicken Sie auf **[!UICONTROL Schließen]**.

>[!NOTE]
>
>Zugriffsrechte werden eingerichtet, wenn Sie ein Kästchen aktivieren. Wenn Sie einem Ordner Rechte zuweisen, werden dieselben Rechte auch den darin enthaltenen Ordner und Dateien zugewiesen. Sie können jedoch auch abweichende Rechte für einzelne Unterordner und Asset-Dateien festlegen.

## Auswählen der Bildvorgabezugriffsberechtigungen für eine Gruppe {#choosing-image-preset-access-permissions-for-a-group}

Wählen Sie Bildvorgabezugriffsberechtigungen für eine Gruppe, wenn Sie festlegen möchten, welche Bildvorgaben den Gruppenmitgliedern beim Exportieren von Assets mit dem Media Portal zur Verfügung stehen sollen.

Siehe auch [Festlegen, welche Exportoptionen Media Portal-Benutzern zur Verfügung stehen](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

1. Klicken Sie auf **[!UICONTROL „Einstellungen“]** > **[!UICONTROL „Media Portal-Einrichtung“]** > **[!UICONTROL „Gruppen“]**.
1. Führen Sie auf der Seite „Gruppen“ einen der folgenden Schritte aus:

   * Um eine Gruppe hinzuzufügen und anzugeben, welche Bildvorgaben ihr zur Verfügung stehen sollen, klicken Sie auf **[!UICONTROL „Hinzufügen“]**. Geben Sie im Dialogfeld „Gruppe hinzufügen“ einen Namen für die Gruppe ein, klicken Sie auf **[!UICONTROL „Gruppe hinzufügen“]** und fügen Sie der Gruppe Benutzer hinzu.
   * Um die Bildvorgabe-Optionen einer Gruppe zu bearbeiten, wählen Sie die Gruppe aus und klicken dann auf **[!UICONTROL „Bearbeiten“]**.

1. Klicken Sie im Dialogfeld „Gruppe hinzufügen“ bzw. „Gruppe bearbeiten“ auf die Registerkarte **[!UICONTROL „Bildvorgabezugriffsberechtigungen“]**.
1. Um festzulegen, welche Vorgaben für Media Portal-Benutzer beim Exportieren von Assets verfügbar sind, wählen Sie Bildvorgaben aus oder deaktivieren Sie sie.
1. Klicken Sie auf **[!UICONTROL Schließen]**.

## Bearbeiten und Löschen von Gruppen {#edit-and-delete-groups}

1. Klicken Sie auf **[!UICONTROL „Einstellungen“]** > **[!UICONTROL „Media Portal-Einrichtung“]** > **[!UICONTROL „Gruppen“]**.
1. Wählen Sie auf der Seite „Gruppenliste“ eine Gruppe aus und bearbeiten oder löschen Sie sie.

   **Bearbeiten einer Gruppe**  - Klicken Sie auf  **[!UICONTROL Bearbeiten]** und wählen Sie dann im Dialogfeld &quot;Gruppe bearbeiten&quot;Optionen aus.

   **Löschen einer Gruppe**  - Klicken Sie auf  **[!UICONTROL Löschen]**.
