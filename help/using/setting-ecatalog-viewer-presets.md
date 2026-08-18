---
title: Einrichten von Viewer-Vorgaben für E-Katalog
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic Viewer-Vorgaben für E-Kataloge einrichten.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:57:04.669Z'
TQID: 'https://experienceleague.adobe.com/Ej7QeFT62FLz2hWS2w-ll2H9m2pkHXlMSJJDJTsgERg'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: dbe8354bb3a9240d20af51249b4b61e2544120bd
workflow-type: tm+mt
source-wordcount: 464
ht-degree: 12%

---

# Viewer-Vorgaben für E-Katalog einrichten{#setting-up-ecatalog-viewer-presets}

Mit E-Katalog-Viewer-Vorgaben werden Stil, Verhalten und Aussehen von E-Katalog-Viewern bestimmt. Adobe Dynamic Media Classic umfasst E-Katalog-Viewer-Vorgaben. Wenn Sie über Administratorzugriff verfügen, können Sie benutzerdefinierte Vorgaben erstellen.

Um eine Vorgabe zu erstellen, können Sie eine neue Vorgabe erstellen oder mit einer von Adobe Dynamic Media Classic bereitgestellten E-Katalog-Viewer-Vorgabe beginnen und sie unter einem neuen Namen speichern. Um das gedruckte Material in Ihren Unternehmensfarben darzustellen und den Stil zu definieren, können Sie Ihre eigenen E-Katalog-Viewer-Vorgaben erstellen.

E-Katalog-Viewer-Vorgaben bieten viele Einstellungen für die Seitennavigation, das Zoomen, Suchen und Auswählen von „Designs“. Wie diese Steuerelemente aussehen und wie der Viewer angezeigt wird, hängt von der Auswahl der E-Katalog-Viewer-Vorgaben ab.

**So richten Sie eine E-Katalog-Viewer-Vorgabe ein (Sie benötigen Administratorzugriff):**

1. Wechseln Sie in der globalen Navigationsleiste zu **[!UICONTROL Einstellungen]** > **[!UICONTROL Viewer-Vorgaben]**.
1. Erstellen Sie auf dem Bildschirm „Viewer-Vorgaben“ eine Viewer-Vorgabe für einen E-Katalog, indem Sie eine neue Vorgabe erstellen oder mit einer vorhandenen Viewer-Vorgabe für einen E-Katalog beginnen:

   * **Erstellen einer E-Katalog-Viewer** Vorgabe: Wählen Sie **[!UICONTROL Hinzufügen]**. Wählen Sie im Dialogfeld „Viewer-Vorgabe hinzufügen“ eine Plattform und anschließend „eCatalog-Viewer“ und anschließend **[!UICONTROL Hinzufügen]**.

   * **Bearbeiten einer E-Katalog-Viewer** Vorgabe: Wählen Sie eine E-Katalog-Viewer-Vorgabe aus und klicken Sie dann auf **[!UICONTROL Bearbeiten]**. Wählen **[!UICONTROL Speichern unter]** nachdem Sie die Voreinstellung fertig erstellt haben.

1. Geben Sie auf der Seite `Configure Viewer` einen Namen für Ihre E-Katalog-Viewer-Vorgabe ein.
1. Legen Sie auf der Seite `Configure Viewer` die gewünschten Optionen fest.

   Klicken Sie auf **[!UICONTROL Info-]**) neben der Option, um die Beschreibung zu lesen.

   Auf der Seite Vorschau wird der Viewer angezeigt, während Sie die Einstellungen aktualisieren und ändern.

1. (Optional) In den **[!UICONTROL Einstellungen des Bedienfelds]** kann die Option **[!UICONTROL Informationsserver-URL]** die folgenden speziellen Token enthalten, die der Viewer ersetzt.

   | Platzhalter | Ersetzt durch | Anmerkungen |
   | --- | --- | --- |
   | `$1$` | „rollover_key“-Wert | Die Elementkennung aus dem `<area>` der Zuordnung. |
   | `$2$` | frame | Die Sequenznummer des momentan angezeigten Bildfelds im Bildsatz. |
   | `$3$` | Bildstamm | Das erste Pfadelement des ersten Elements, das im Bildbefehl angegeben wird (normalerweise die Katalog-ID des Katalogeintrags, der den Bildsatz bestimmt). |

1. (Optional) Geben Sie in **[!UICONTROL Einstellungen des Bedienfelds]** in das Feld **[!UICONTROL Antwortvorlage]** den Text ein, der angezeigt werden soll, wenn in Adobe Dynamic Media Classic beim Abrufen von Informationen für eine Imagemap ein Fehler auftritt. Wenn das System beispielsweise einen Firmen- und E-Katalog-Namen, aber keine Rollover-Kennung erhält, wird diese Meldung angezeigt.

>[!NOTE]
>
>Um diese Antwortvorlage anstelle der im E-Katalog selbst definierten Vorlage zu verwenden, fügen Sie am Ende der Informationsserver-URL `fmt=1` hinzu. Beispiel: `https://.../$3$/$4$/$1$/?FMT=1`.

1. Wählen Sie **[!UICONTROL Speichern]** aus.
1. Wählen Sie **[!UICONTROL Standard]** aus, damit die von Ihnen erstellte E-Katalog-Viewer-Vorgabe zum Anzeigen von E-Katalogen auf Ihrer Web-Seite verwendet wird.

Um eine E-Katalog-Viewer-Vorgabe zu löschen, wählen Sie sie auf dem Bildschirm „Viewer-Vorgaben“ aus und klicken Sie auf **[!UICONTROL Löschen]**.

>[!MORELIKETHIS]
>
>* [Viewer-Vorgaben](application-setup.md#viewer_presets)
