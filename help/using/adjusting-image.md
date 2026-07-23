---
title: Bild anpassen
description: Erfahren Sie, wie Sie ein Bild in Adobe Dynamic Media Classic anpassen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 880ee6d0-cb0a-4d53-9056-f0b8b292136e
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:38:08.783Z'
TQID: 'https://experienceleague.adobe.com/Gze3kMTnn5xWFZ4uUW-aNo5VASF2ncV7T1jvcsRadaQ'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 4280c815eca0ff8828d350afe6de877f6160e9ae
workflow-type: tm+mt
source-wordcount: 535
ht-degree: 24%

---

# Bilder anpassen{#adjusting-an-image}

Adobe Dynamic Media Classic bietet verschiedene Befehle zum Anpassen des Erscheinungsbilds eines Bildes. Sie können das Bild spiegeln, drehen, unscharf machen, den Farbausgleich verändern und es einfärben. Beim Experimentieren mit diesen Befehlen können Sie deren Auswirkungen auf das Bild beobachten, mit dem Sie arbeiten.

Siehe auch [Alias für ein Bild erstellen](adjusting-image.md#creating_an_alias_for_an_image).

**So passen Sie ein Bild an:**

1. Wählen Sie die Rollover-Schaltfläche Bearbeiten des Bildes aus und wählen Sie Anpassen aus, oder doppelklicken Sie im Durchsuchen-Panel auf das Bild, damit es in der Detailansicht geöffnet wird.
1. Wählen Sie eine Bildgröße und eine Bildvorgabe aus (unten im Fenster).
1. Verwenden Sie die Befehle auf der rechten Seite des `Adjust Editor`, um das Bild anzupassen:

   * Mit der Option „Spiegeln“ können Sie ein Bild horizontal bzw. vertikal spiegeln.
   * Drehen Sie das **[!UICONTROL mit]** Schieberegler. Sie können Werte in das Feld **[!UICONTROL Rotator]** eingeben, um ein Bild zu drehen. Bei positiven Werten wird es im Uhrzeigersinn, bei negativen Werten gegen den Uhrzeigersinn gedreht.
   * Mit dem Schieberegler „Weichzeichnen“ bzw. dem gleichnamigen Feld wird das Bild weichgezeichnet. Höhere Werte erhöhen die Unschärfe des Bildes.
   * Mithilfe der Optionen „Kontrast“, „Helligkeit“, „Sättigung“, „Farbton“ und „Farbbalance“ können Sie die Farbe und Helligkeit anpassen. Diese Effekte sind kumulativ. Beispielsweise werden Änderungen an den Einstellungen „Magenta“/„Grün“ zu den Änderungen an der Einstellung „Farbton“ hinzugefügt und summiert.
   * Verwenden Sie die `Colorize` Optionen, um ein Bild einzufärben und gleichzeitig Schatten und Hervorhebungen beizubehalten. Auch die Änderungen an den Einstellungen für „Färben“ sind kumulativ. Wählen Sie im Menü Helligkeit die Option **[!UICONTROL Keine Kompensation]**, um die automatische Helligkeitskompensation zu deaktivieren. Um den Kontrastbereich des Originalbilds beizubehalten, setzen Sie den Kontrastwert auf 0 oder geben Sie einen Kontrastbereich mit einem Wert größer als 0 an. Mit dem Wert 100 erzielen Sie den maximalen Kontrast. Typische Werte liegen im Bereich von 30-70.

1. Wenn Sie das Anpassen des Bildes beendet haben, führen Sie einen der folgenden Schritte aus:

   * Wählen Sie **[!UICONTROL Speichern]** aus.

   * Um das Originalbild zu ersetzen, wählen Sie **[!UICONTROL Speichern unter]**.

     Wählen Sie in der Dropdown-Liste **[!UICONTROL Original ersetzen]** und dann **[!UICONTROL Speichern]** aus.

   * Um das Bild als neues primäres Bild zu speichern, wählen Sie **[!UICONTROL Speichern unter]**.

     Wählen Sie in der Dropdown-Liste **[!UICONTROL Als neue primäre Instanz speichern]** aus.
     Wählen **[!UICONTROL im Listenfeld]**&#x200B;Ordnername“ den Ordner aus, in dem das neue Primärbild gespeichert werden soll.
     Wählen Sie **[!UICONTROL Speichern]** aus.

   * Um das Bild als eine weitere Ansicht des Primärbilds zu speichern, können Sie einen Alias dafür erstellen. Wählen Sie **[!UICONTROL Speichern unter]**.

     Wählen Sie in der Dropdown-Liste im Dialogfeld **[!UICONTROL Speichern unter]** die Option **[!UICONTROL Als weitere Ansicht von Primär speichern]**.
     Wählen **[!UICONTROL im Listenfeld]**&#x200B;Ordnername“ den Ordner aus, in dem das neue Primärbild gespeichert werden soll.
     Wählen Sie **[!UICONTROL Speichern]** aus.

## Erstellen eines Alias für ein Bild {#creating-an-alias-for-an-image}

Wenn Sie ein Bild angepasst haben, können Sie es als eine andere Ansicht des Primärbilds speichern. Dazu können Sie einen Alias für das Bild erstellen, indem Sie die Funktion **[!UICONTROL Speichern als eine andere Ansicht der]**&quot; verwenden.

**So erstellen Sie einen Alias für ein Bild:**

1. Wählen Sie in der Rasteransicht oder Listenansicht in der **[!UICONTROL Bearbeiten]** Dropdown-Liste neben einem Bild, für das Sie einen Alias erstellen möchten, **[!UICONTROL Anpassen]**.
1. Klicken Sie unten rechts auf der Seite auf &quot;**[!UICONTROL &quot;]**.
1. Wählen Sie in der Dropdown-Liste im Dialogfeld **[!UICONTROL Speichern unter]** die Option **[!UICONTROL Als weitere Ansicht von Primär speichern]**.
1. Wählen Sie im Listenfeld **[!UICONTROL Ordnername]** den Ordner, in dem Sie das Aliasbild speichern möchten.
1. Geben Sie im Feld **[!UICONTROL Dateiname]** den Namen ein, den Sie für den Alias verwenden möchten.
1. Wählen Sie **[!UICONTROL Speichern]** aus.
