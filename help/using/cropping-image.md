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
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 31%

---

# Bilder zuschneiden{#cropping-an-image}

Sie können Bilder in der Adobe Dynamic Media Classic zuschneiden. Die Informationen zu den beschnittenen Bildern werden im System gespeichert, damit sie in ihrem ursprünglichen Zustand wiederhergestellt werden können. Sie können ein Bild auch beschneiden und die beschnittene Version unter einem neuen Namen speichern.

Sie haben die Möglichkeit, durch Beschneiden den weißen Bereich um das Bild herum zu entfernen oder einen beliebigen Bildbereich zu isolieren.

>[!NOTE]
>
>Nach dem Zuschneiden können Sie **[!UICONTROL Speichern unter]** und speichern Sie eine zugeschnittene Version des Bildes unter einem anderen Namen. Wählen Sie im Fenster Speichern unter die Option **[!UICONTROL Als neuen Primäre speichern]** , um eine zweite Kopie des Bildes zu speichern. Auswählen **[!UICONTROL Als zusätzliche Ansicht des Primären speichern]** sodass Sie das Original und die zugeschnittene Version unter einem anderen Namen speichern können. Auswählen **[!UICONTROL Original ersetzen]** , um die Originaldatei zu löschen, von der Sie das Bild beschnitten haben. Geben Sie dann einen Namen für das Bild ein und wählen Sie **[!UICONTROL Einsenden]**.

## Beschneiden zum Entfernen des weißen Bereichs am Bildrand {#crop-to-remove-white-space-around-an-image}

Sie können die transparenten oder einfarbigen Pixel am Rand eines Bilds durch Beschneiden entfernen.

1. Um ein Bild zuzuschneiden, wählen Sie dessen Rollover aus **[!UICONTROL Bearbeiten]** und wählen Sie **[!UICONTROL Zuschneiden]** oder zeigen Sie es im Durchsuchenbedienfeld in der Detailansicht an und wählen Sie die **[!UICONTROL Zuschneiden]** Schaltfläche.
1. Führen Sie auf der Seite &quot;Beschneidungseditor&quot;einen der folgenden Schritte aus:

   * Um Farbpixel zu beschneiden, gehen Sie zu **[!UICONTROL Zuschneiden]** > **[!UICONTROL Farbe]**. Im **[!UICONTROL Auto-Zuschneiden nach Farbe]** auswählen, wählen Sie das **[!UICONTROL Ecke]** und wählen Sie eine Ecke mit der Hintergrundfarbe aus, die Sie entfernen möchten. Geben Sie dann ein **[!UICONTROL Toleranz]** Einstellung von 0 bis 1. Wenn Sie den Wert 0 einstellen, werden Pixel nur abgeschnitten, wenn sie exakt der Farbe entsprechen, die Sie in der Bildecke ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu. Auswählen **[!UICONTROL Zuschneiden]**.
   * Um transparente Pixel zu beschneiden, gehen Sie zu **[!UICONTROL Zuschneiden]** > **[!UICONTROL Transparent]**. Im **[!UICONTROL Automatisch nach Transparenz zuschneiden]** eingeben, geben Sie eine Toleranzeinstellung von 0 bis 1 ein. Bei der Einstellung 0 werden Pixel nur dann abgeschnitten, wenn sie transparent sind. Werte, die näher an 1 liegen, lassen eine größere Transparenzabweichung zu. Auswählen **[!UICONTROL Zuschneiden]**.

1. Auswählen **[!UICONTROL Speichern]**.

>[!NOTE]
>
>Um das Bild nach dem Zuschneiden wieder in den Originalzustand zu versetzen, zeigen Sie es im Bildschirm &quot;Beschneiden-Editor&quot;an und wählen Sie **[!UICONTROL Zurücksetzen]**.

## Auswählen eines zu beschneidenden Bereichs {#select-an-area-to-crop}

1. Um ein Bild zuzuschneiden, wählen Sie dessen Rollover aus **[!UICONTROL Bearbeiten]** und wählen Sie **[!UICONTROL Zuschneiden]** oder zeigen Sie es im Durchsuchenbedienfeld in der Detailansicht an und wählen Sie **[!UICONTROL Zuschneiden]**.

1. Platzieren Sie im Fenster &quot;Beschneidungs-Editor&quot;den Teil des Bildes, den Sie nicht zuschneiden möchten, in das Zuschnittsfeld. Was auch immer innerhalb des Felds angezeigt wird, bleibt nach der Auswahl **[!UICONTROL Speichern]** und schneiden Sie das Bild ab.
1. Führen Sie zum Anpassen des zu beschneidenden Bereichs einen der folgenden Schritte aus:

   * Ziehen Sie eine Seite oder Ecke des Rahmens. Halten Sie beim Ziehen die Umschalttaste gedrückt, um die Größe zu ändern, wobei Sie jedoch das Seitenverhältnis (die Form) des Zuschnittrahmens beibehalten.
   * Geben Sie in den Feldern unter „Größe“ die gewünschten Pixelmaße an.
   * Verschieben Sie den Rahmen. Bewegen Sie den Zeiger in das Innere des Feldes. Wenn der Mauszeiger als Vierfachpfeil dargestellt wird, ziehen Sie den Rahmen an die gewünschte Position.

1. Auswählen **[!UICONTROL Speichern]**.

>[!NOTE]
>
>Um das Bild nach dem Zuschneiden wieder in den Originalzustand zu versetzen, zeigen Sie es im Bildschirm &quot;Beschneiden-Editor&quot;an und wählen Sie **[!UICONTROL Zurücksetzen]**.

>[!MORELIKETHIS]
>
>* [Optionen für die Bildbearbeitung beim Hochladen](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Leerraum aus einer PDF-Datei beschneiden](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Beschneiden von den Seiten der PDF-Seiten](pdfs.md#cropping_from_the_sides_of_pdf_pages)
