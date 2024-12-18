---
title: Bilder zuschneiden
description: Erfahren Sie, wie Sie ein Bild in Adobe Dynamic Media Classic zuschneiden.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 31%

---

# Bilder zuschneiden{#cropping-an-image}

Sie können Bilder in der Adobe Dynamic Media Classic zuschneiden. Die Informationen zu den beschnittenen Bildern werden im System gespeichert, damit sie in ihrem ursprünglichen Zustand wiederhergestellt werden können. Sie können ein Bild auch beschneiden und die beschnittene Version unter einem neuen Namen speichern.

Sie haben die Möglichkeit, durch Beschneiden den weißen Bereich um das Bild herum zu entfernen oder einen beliebigen Bildbereich zu isolieren.

>[!NOTE]
>
>Nach dem Zuschneiden können Sie **[!UICONTROL Speichern unter]** auswählen und eine zugeschnittene Version des Bildes unter einem anderen Namen speichern. Wählen Sie im Fenster Speichern unter **[!UICONTROL Als neue Primär speichern]**, um eine zweite Bildkopie zu speichern. Wählen Sie **[!UICONTROL Als Hinzufügungsansicht speichern von Primär]**, um das Original und die zugeschnittene Version unter einem anderen Namen zu speichern. Wählen Sie **[!UICONTROL Original ersetzen]**, um die Originaldatei, aus der Sie das Bild abgeschnitten haben, zu löschen. Geben Sie dann einen Namen für das Bild ein und wählen Sie **[!UICONTROL Senden]**.

## Beschneiden zum Entfernen des weißen Bereichs am Bildrand {#crop-to-remove-white-space-around-an-image}

Sie können die transparenten oder einfarbigen Pixel am Rand eines Bilds durch Beschneiden entfernen.

1. Um ein Bild zu beschneiden, klicken Sie auf die entsprechende **[!UICONTROL Bearbeiten]**-Schaltfläche und wählen Sie dann **[!UICONTROL Zuschneiden]** aus oder zeigen Sie es im Durchsuchen-Bedienfeld in der Detailansicht an und klicken Sie auf die Schaltfläche **[!UICONTROL Zuschneiden]**.
1. Führen Sie auf der Seite „Zuschnitt-Editor“ eine der folgenden Aktionen aus:

   * Zum Zuschneiden von Farbpixeln navigieren Sie **[!UICONTROL Zuschneiden]** > **[!UICONTROL Farbe]**. Wählen Sie im Dialogfeld **[!UICONTROL Automatisch nach Farbe]** im Menü **[!UICONTROL Ecke]** eine Ecke mit der Hintergrundfarbe aus, die Sie abschneiden möchten. Geben Sie dann eine **[!UICONTROL Toleranz]**-Einstellung von 0 bis 1 ein. Wenn Sie den Wert 0 einstellen, werden Pixel nur abgeschnitten, wenn sie exakt der Farbe entsprechen, die Sie in der Bildecke ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu. Wählen Sie **[!UICONTROL Zuschneiden]** aus.
   * Um transparente Pixel zu kürzen, gehen Sie **[!UICONTROL Kürzen]** > **[!UICONTROL Transparent]**. Geben **[!UICONTROL im Dialogfeld]** Automatisch zuschneiden nach Transparenz“ eine Toleranzeinstellung von 0 bis 1 ein. Mit der Einstellung 0 werden Pixel nur dann abgeschnitten, wenn sie transparent sind. Werte, die näher an 1 liegen, lassen eine größere Transparenzabweichung zu. Wählen Sie **[!UICONTROL Zuschneiden]** aus.

1. Wählen Sie **[!UICONTROL Speichern]** aus.

>[!NOTE]
>
>Um ein Bild nach dem Zuschneiden wieder in den Originalzustand zu versetzen, zeigen Sie es im Bildschirm des Zuschnittseditors an und wählen Sie **[!UICONTROL Zurücksetzen]**.

## Auswählen eines zu beschneidenden Bereichs {#select-an-area-to-crop}

1. Um ein Bild zu beschneiden, klicken Sie auf die entsprechende **[!UICONTROL Bearbeiten]**-Schaltfläche und wählen **[!UICONTROL Zuschneiden]** oder zeigen Sie es im Durchsuchen-Bedienfeld in der Detailansicht an und wählen Sie **[!UICONTROL Zuschneiden]**.

1. Platzieren Sie im Fenster „Beschneideditor“ den Teil des Bildes, den Sie nicht beschneiden möchten, in das Zuschnittsfeld. Was in dem Feld angezeigt wird, bleibt auch erhalten, wenn Sie auf **[!UICONTROL Speichern]** klicken und das Bild zuschneiden.
1. Führen Sie zum Anpassen des zu beschneidenden Bereichs einen der folgenden Schritte aus:

   * Ziehen Sie eine Seite oder Ecke des Rahmens. Halten Sie beim Ziehen die Umschalttaste gedrückt, um die Größe zu ändern, aber das Seitenverhältnis (Form) des Zuschnittsfeldes beizubehalten.
   * Geben Sie in den Feldern unter „Größe“ die gewünschten Pixelmaße an.
   * Verschieben Sie den Rahmen. Bewegen Sie den Zeiger in das Innere des Feldes. Wenn der Mauszeiger als Vierfachpfeil dargestellt wird, ziehen Sie den Rahmen an die gewünschte Position.

1. Wählen Sie **[!UICONTROL Speichern]** aus.

>[!NOTE]
>
>Um ein Bild nach dem Zuschneiden wieder in den Originalzustand zu versetzen, zeigen Sie es im Bildschirm des Zuschnittseditors an und wählen Sie **[!UICONTROL Zurücksetzen]**.

>[!MORELIKETHIS]
>
>* [Optionen für die Bildbearbeitung beim Hochladen](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Beschneiden Sie Leerzeichen von einer PDF-Datei](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Beschneiden Sie die PDF-Seiten seitlich](pdfs.md#cropping_from_the_sides_of_pdf_pages)
