---
title: Bilder anpassen
description: Erfahren Sie, wie Sie ein Bild in Adobe Dynamic Media Classic anpassen.
uuid: c052acd3-e8c1-4134-ad21-b9c41578097f
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 47a23980-2886-4da3-ab2d-6cd50e00d188
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 880ee6d0-cb0a-4d53-9056-f0b8b292136e
source-git-commit: 972e5d4f468f14bd40e970c989465a639fd5e6fb
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 52%

---

# Bilder anpassen{#adjusting-an-image}

Adobe Dynamic Media Classic bietet verschiedene Befehle zum Anpassen des Erscheinungsbilds eines Bildes. Sie können ein Bild spiegeln, drehen, weichzeichnen, färben und dessen Farbbalance ändern. Während Sie mit diesen Befehlen experimentieren, können Sie deren Auswirkungen auf die Darstellung des bearbeiteten Bilds verfolgen.

Siehe auch [Erstellen eines Alias für ein Bild](adjusting-image.md#creating_an_alias_for_an_image).

**So passen Sie ein Bild an:**

1. Wählen Sie die Rollover-Schaltfläche &quot;Bearbeiten&quot;des Bildes aus und wählen Sie &quot;Anpassen&quot;oder doppelklicken Sie im Durchsuchenbedienfeld auf das Bild, damit es in der Detailansicht geöffnet wird.
1. Wählen Sie eine Größe und eine Bildvorgabe aus (unten in der Ansicht).
1. Mithilfe der Befehle auf der rechten Seite des Fensters „Anpassungseditor“ können Sie Anpassungen an dem Bild vornehmen:

   * Mit der Option „Spiegeln“ können Sie ein Bild horizontal bzw. vertikal spiegeln.
   * Mit dem Drehen-Regler können Sie das Bild drehen. Sie können das Bild auch drehen, indem Sie im Feld „Drehen“ entsprechende Werte eingeben. Bei positiven Werten wird es im Uhrzeigersinn, bei negativen Werten gegen den Uhrzeigersinn gedreht.
   * Mit dem Schieberegler „Weichzeichnen“ bzw. dem gleichnamigen Feld wird das Bild weichgezeichnet. Je höher der Wert, desto stärker wird das Bild weichgezeichnet.
   * Mithilfe der Optionen „Kontrast“, „Helligkeit“, „Sättigung“, „Farbton“ und „Farbbalance“ können Sie die Farbe und Helligkeit anpassen. Diese Effekte sind kumulativ. Beispielsweise werden Änderungen an den Einstellungen „Magenta“/„Grün“ zu den Änderungen an der Einstellung „Farbton“ hinzugefügt und summiert.
   * Mit der Option „Färben“ können Sie ein Bild färben und gleichzeitig dessen Einstellungen für Tiefen und Lichter beibehalten. Auch die Änderungen an den Einstellungen für „Färben“ sind kumulativ. Wählen Sie im Menü Helligkeit die Option **[!UICONTROL Keine Ausgleichszahlung]** sodass Sie die automatische Helligkeitskompensation deaktivieren. Setzen Sie den Kontrastwert auf 0, wenn Sie den Kontrastbereich des Originalbilds beibehalten möchten, oder geben Sie andernfalls einen Kontrastbereich mit einem Wert größer als 0 an. Mit dem Wert 100 erzielen Sie den maximalen Kontrast. Typische Werte liegen zwischen 30 und 70.

1. Wenn Sie das Anpassen des Bildes beendet haben, führen Sie einen der folgenden Schritte aus:

   * Auswählen **[!UICONTROL Speichern]**.

   * Um das Original des Bildes zu ersetzen, wählen Sie **[!UICONTROL Speichern unter]**.

      Wählen Sie in der Dropdown-Liste **[!UICONTROL Original ersetzen]** und wählen Sie **[!UICONTROL Speichern]**.

   * Um das Bild als neues Primärbild zu speichern, wählen Sie **[!UICONTROL Speichern unter]**.

      Wählen Sie in der Dropdownliste **[!UICONTROL Als neue Masterversion speichern]**.
Im **[!UICONTROL Ordnername]** Listenfeld den Ordner auswählen, in dem das neue Primärbild gespeichert werden soll.
Auswählen **[!UICONTROL Speichern]**.

   * So speichern Sie das Bild als eine andere Ansicht des Primärbilds. können Sie einen Alias erstellen. Auswählen **[!UICONTROL Speichern unter]**.

      Im **[!UICONTROL Speichern unter]** in der Dropdown-Liste wählen Sie **[!UICONTROL Als weitere Ansicht von Übergeordneten speichern]**.
Im **[!UICONTROL Ordnername]** Listenfeld den Ordner auswählen, in dem das neue Primärbild gespeichert werden soll.
Auswählen **[!UICONTROL Speichern]**.

## Erstellen eines Alias für ein Bild {#creating-an-alias-for-an-image}

Wenn Sie ein Bild angepasst haben, können Sie es als eine andere Ansicht des Primärbilds speichern. Hierfür können Sie mit der Funktion **[!UICONTROL Als zusätzliche Ansicht des Masterbilds speichern]** einen Alias des Bildes erstellen.

**So erstellen Sie einen Alias für ein Bild:**

1. In der Rasteransicht oder Listenansicht im **[!UICONTROL Bearbeiten]** Dropdown-Liste neben einem Bild, für das Sie einen Alias erstellen möchten, wählen Sie **[!UICONTROL Anpassen]**.
1. Wählen Sie in der rechten unteren Ecke der Seite die Option **[!UICONTROL Speichern unter]**.
1. Im **[!UICONTROL Speichern unter]** in der Dropdown-Liste wählen Sie **[!UICONTROL Als zusätzliche Ansicht von Übergeordneten speichern]**.
1. Wählen Sie im Listenfeld **[!UICONTROL Ordnername]** den Ordner, in dem Sie das Aliasbild speichern möchten.
1. Geben Sie im Feld **[!UICONTROL Dateiname]** den Namen ein, den Sie für den Alias verwenden möchten.
1. Auswählen **[!UICONTROL Speichern]**.
