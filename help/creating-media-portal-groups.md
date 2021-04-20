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
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 95%

---


# Erstellen und Verwalten von Media Portal-Gruppen{#creating-and-managing-media-portal-groups}

Mithilfe von *Gruppen* können Sie die Media Portal-Benutzer leichter verwalten. Um auf ein Asset zugreifen zu können, muss ein Benutzer Mitglied mindestens einer Gruppe mit den erforderlichen Berechtigungen für dieses Asset sein. Wenn Sie einen Benutzer hinzufügen, weisen Sie ihm eine oder mehrere Rollen zu. Dadurch gewähren Sie dem Benutzer Zugriffsrechte für die Ordner, denen die Gruppe zugewiesen wurde. Sie können auch angeben, welche Bildvorgaben einer Gruppe zur Verfügung stehen.

## Verwenden von Gruppen zum Beschränken des Zugriffs auf Ordner, Assets und Bildvorgaben  {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

Wenn Sie Gruppen erstellen, können Sie Zugriffsrechte auf unterschiedlichen Ebenen gewähren. Für jede Gruppe weisen Sie Lese-, Schreib- und Löschberechtigungen für unterschiedliche Ordner und Assets in den Ordnern zu. Außerdem legen Sie fest, welche Bildvorgaben der Gruppe zur Verfügung stehen. Anschließend weisen Sie Benutzer den Gruppen zu. Ein Benutzer kann Mitglied mehrerer Gruppen sein. Durch das Gruppenkonzept können Sie flexibel Zugriffsrechte für einen Teil des Gesamtinhalts zuweisen.

Wenn Sie einer Gruppe keine speziellen Zugriffsrechte für ein Asset oder einen Ordner zuweisen, erbt das Asset bzw. der Ordner die Rechte von dem in der Ordnerhierarchie jeweils übergeordneten Ordner. Wenn Sie einem Ordner Rechte zuweisen, werden dieselben Rechte für sämtliche darin enthaltenen Ordner übernommen.

>[!NOTE]
>
>Benutzer können mehreren Gruppen angehören. Wenn ein Benutzer zwei Gruppen mit unterschiedlichen Zugriffsrechten für einen Ordner angehört, werden jeweils die höchsten Zugriffsrechte angewendet.

## Hinzufügen einer Gruppe  {#adding-a-group}

1. Klicken Sie auf **„Einstellungen“** > **„Media Portal-Einrichtung“** > **„Gruppen“**.
1. Klicken Sie auf **„Hinzufügen“**.
1. Geben Sie im Dialogfeld „Gruppe hinzufügen“ im Feld „Gruppenname“ einen Namen für die Gruppe ein und klicken Sie dann auf **„Gruppe hinzufügen“**.
1. Bei Bedarf können Sie die Kontrollkästchen neben den Namen von Benutzern aktivieren, um diese Benutzer der neuen Gruppe hinzuzufügen.
1. Wenn Sie an dieser Stelle Zugriffsberechtigungen festlegen möchten, klicken Sie auf die Registerkarte **„Asset-Zugriffsberechtigungen“** und legen Sie dann die gewünschten Optionen fest.

   Siehe [Einrichten von Asset-Zugriffsberechtigungen für eine Gruppe](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group).

1. Wenn Sie wählen möchten, welche Bildvorgaben für die Gruppe verfügbar sein sollen, klicken Sie auf die Registerkarte **„Bildvorgabezugriffsberechtigungen“** und wählen Sie Bildvorgaben aus, die die Gruppe verwenden kann.

   Siehe [Auswählen der Bildvorgabezugriffsberechtigungen für eine Gruppe](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group).

1. Klicken Sie auf „**Schließen**“.

## Einrichten von Asset-Zugriffsberechtigungen für eine Gruppe  {#establishing-asset-access-permissions-for-a-group}

1. Klicken Sie auf **„Einstellungen“** > **„Media Portal-Einrichtung“** > **„Gruppen“**.
1. Führen Sie auf der Seite „Gruppen“ einen der folgenden Schritte aus:

   * Um eine Gruppe hinzuzufügen und Berechtigungen festzulegen, klicken Sie auf **„Hinzufügen“**. Geben Sie im Dialogfeld „Gruppe hinzufügen“ einen Namen für die Gruppe ein, klicken Sie auf **„Gruppe hinzufügen“** und fügen Sie der Gruppe Benutzer hinzu.
   * Um die Berechtigungen einer Gruppe zu bearbeiten, wählen Sie die Gruppe aus und klicken dann auf **„Bearbeiten“**.

1. Klicken Sie im Dialogfeld „Gruppe hinzufügen“ bzw. „Gruppe bearbeiten“ auf die Registerkarte **„Asset-Zugriffsberechtigungen“**. Über die Kontrollkästchen auf der rechten Seite der Registerkarte können Sie Rechte zum Lesen, Schreiben und Löschen für Ordner und Assets festlegen. Im linken Fensterbereich können Sie Ordner und Unterordner erweitern und minimieren.
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

1. Klicken Sie auf **Schließen**.

>[!NOTE]
>
>Zugriffsrechte werden eingerichtet, wenn Sie ein Kästchen aktivieren. Wenn Sie einem Ordner Rechte zuweisen, werden dieselben Rechte auch den darin enthaltenen Ordner und Dateien zugewiesen. Sie können jedoch auch abweichende Rechte für einzelne Unterordner und Asset-Dateien festlegen.

## Auswählen der Bildvorgabezugriffsberechtigungen für eine Gruppe  {#choosing-image-preset-access-permissions-for-a-group}

Wählen Sie Bildvorgabezugriffsberechtigungen für eine Gruppe, wenn Sie festlegen möchten, welche Bildvorgaben den Gruppenmitgliedern beim Exportieren von Assets mit dem Media Portal zur Verfügung stehen sollen.

Siehe auch [Festlegen, welche Exportoptionen Media Portal-Benutzern zur Verfügung stehen](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

1. Klicken Sie auf **„Einstellungen“** > **„Media Portal-Einrichtung“** > **„Gruppen“**.
1. Führen Sie auf der Seite „Gruppen“ einen der folgenden Schritte aus:

   * Um eine Gruppe hinzuzufügen und anzugeben, welche Bildvorgaben ihr zur Verfügung stehen sollen, klicken Sie auf **„Hinzufügen“**. Geben Sie im Dialogfeld „Gruppe hinzufügen“ einen Namen für die Gruppe ein, klicken Sie auf **„Gruppe hinzufügen“** und fügen Sie der Gruppe Benutzer hinzu.
   * Um die Bildvorgabe-Optionen einer Gruppe zu bearbeiten, wählen Sie die Gruppe aus und klicken dann auf **„Bearbeiten“**.

1. Klicken Sie im Dialogfeld „Gruppe hinzufügen“ bzw. „Gruppe bearbeiten“ auf die Registerkarte **„Bildvorgabezugriffsberechtigungen“**.
1. Wählen Sie Bildvorgaben aus bzw. heben Sie ihre Auswahl auf, um festzulegen, welche Bildvorgaben den Media Portal-Benutzern beim Exportieren von Assets zur Verfügung stehen.
1. Klicken Sie auf „**Schließen**“.

## Bearbeiten und Löschen von Gruppen  {#edit-and-delete-groups}

1. Klicken Sie auf **„Einstellungen“** > **„Media Portal-Einrichtung“** > **„Gruppen“**.
1. Wählen Sie auf der Seite „Gruppenliste“ eine Gruppe aus und bearbeiten oder löschen Sie sie.

   **Bearbeiten einer** GruppeKlicken Sie auf Bearbeiten und wählen Sie dann im Dialogfeld Gruppe bearbeiten die gewünschten Optionen aus.

   **Löschen einer** GruppeKlicken Sie auf Löschen.

