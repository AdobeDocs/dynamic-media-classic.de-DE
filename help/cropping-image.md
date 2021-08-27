---
title: Bilder zuschneiden
description: Erfahren Sie, wie Sie ein Bild in Adobe Dynamic Media Classic zuschneiden.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 35%

---

# Bilder zuschneiden{#cropping-an-image}

Sie können Bilder in der Adobe Dynamic Media Classic zuschneiden. Die Informationen zu den beschnittenen Bildern werden im System gespeichert, damit sie in ihrem ursprünglichen Zustand wiederhergestellt werden können. Sie können ein Bild auch beschneiden und die beschnittene Version unter einem neuen Namen speichern.

Sie haben die Möglichkeit, durch Beschneiden den weißen Bereich um das Bild herum zu entfernen oder einen beliebigen Bildbereich zu isolieren.

>[!NOTE]
>
>Nach dem Zuschneiden können Sie **[!UICONTROL Speichern unter]** auswählen und eine zugeschnittene Version des Bildes unter einem anderen Namen speichern. Wählen Sie im Fenster &quot;Speichern unter&quot;die Option **[!UICONTROL Als neu speichern]** aus, um eine zweite Bildkopie zu speichern. Wählen Sie **[!UICONTROL Als zusätzliche Ansicht von Übergeordnet speichern]** aus, damit Sie das Original und die zugeschnittene Version unter einem anderen Namen speichern können. Wählen Sie **[!UICONTROL Original ersetzen]** aus, um die Originaldatei zu löschen, von der Sie das Bild beschnitten haben. Geben Sie dann einen Namen für das Bild ein und wählen Sie **[!UICONTROL Submit]** aus.

## Beschneiden zum Entfernen des weißen Bereichs am Bildrand {#crop-to-remove-white-space-around-an-image}

Sie können die transparenten oder einfarbigen Pixel am Rand eines Bilds durch Beschneiden entfernen.

1. Um ein Bild zu beschneiden, klicken Sie auf den Rollover **[!UICONTROL Bearbeiten]** und wählen Sie dann **[!UICONTROL Zuschneiden]** oder zeigen Sie es im Durchsuchenbedienfeld in der Detailansicht an und wählen Sie die Schaltfläche **[!UICONTROL Zuschneiden]** aus.
1. Führen Sie auf der Seite &quot;Beschneidungseditor&quot;einen der folgenden Schritte aus:

   * Um Farbpixel zu beschneiden, gehen Sie zu **[!UICONTROL Trim]** > **[!UICONTROL Color]**. Wählen Sie im Dialogfeld **[!UICONTROL Automatisches Zuschneiden nach Farbe]** das Menü **[!UICONTROL Ecke]** aus und wählen Sie eine Ecke mit der Hintergrundfarbe, die Sie entfernen möchten. Geben Sie dann die Einstellung **[!UICONTROL Toleranz]** von 0 bis 1 ein. Wenn Sie den Wert 0 einstellen, werden Pixel nur abgeschnitten, wenn sie exakt der Farbe entsprechen, die Sie in der Bildecke ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu. Wählen Sie **[!UICONTROL Zuschneiden]** aus.
   * Um transparente Pixel zu beschneiden, gehen Sie zu **[!UICONTROL Trim]** > **[!UICONTROL Transparent]**. Geben Sie im Dialogfeld **[!UICONTROL Automatisches Zuschneiden nach Transparenz]** eine Toleranzeinstellung von 0 bis 1 ein. Bei der Einstellung 0 werden Pixel nur dann abgeschnitten, wenn sie transparent sind. Werte, die näher an 1 liegen, lassen eine größere Transparenzabweichung zu. Wählen Sie **[!UICONTROL Zuschneiden]** aus.

1. Wählen Sie **[!UICONTROL Save]** aus.

>[!NOTE]
>
>Um ein Bild nach dem Zuschneiden wieder in den Originalzustand zu versetzen, zeigen Sie es im Bildschirm &quot;Zuschnitt-Editor&quot;an und wählen Sie **[!UICONTROL Zurücksetzen]** aus.

## Auswählen eines zu beschneidenden Bereichs {#select-an-area-to-crop}

1. Um ein Bild zu beschneiden, klicken Sie auf den Rollover **[!UICONTROL Schaltfläche &quot;Bearbeiten]**&quot;und wählen Sie **[!UICONTROL Zuschneiden]** oder zeigen Sie es im Durchsuchenbedienfeld in der Detailansicht an und wählen Sie **[!UICONTROL Zuschneiden]** aus.

1. Platzieren Sie im Fenster &quot;Beschneidungs-Editor&quot;den Teil des Bildes, den Sie nicht zuschneiden möchten, in das Zuschnittsfeld. Was immer innerhalb des Felds angezeigt wird, bleibt bestehen, nachdem Sie **[!UICONTROL Speichern]** ausgewählt und das Bild beschnitten haben.
1. Führen Sie zum Anpassen des zu beschneidenden Bereichs einen der folgenden Schritte aus:

   * Ziehen Sie eine Seite oder Ecke des Rahmens. Halten Sie beim Ziehen die Umschalttaste gedrückt, um die Größe zu ändern, dabei jedoch das Seitenverhältnis (die Form) des zu beschneidenden Bereichs beizubehalten.
   * Geben Sie in den Feldern unter „Größe“ die gewünschten Pixelmaße an.
   * Verschieben Sie den Rahmen. Bewegen Sie den Zeiger in das Innere des Feldes. Wenn der Mauszeiger als Vierfachpfeil dargestellt wird, ziehen Sie den Rahmen an die gewünschte Position.

1. Wählen Sie **[!UICONTROL Save]** aus.

>[!NOTE]
>
>Um ein Bild nach dem Zuschneiden wieder in den Originalzustand zu versetzen, zeigen Sie es im Bildschirm &quot;Zuschnitt-Editor&quot;an und wählen Sie **[!UICONTROL Zurücksetzen]** aus.

>[!MORELIKETHIS]
>
>* [Optionen für die Bildbearbeitung beim Hochladen](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Leerraum aus einer PDF-Datei beschneiden](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Zuschneiden von den Seiten der PDF-Seiten](pdfs.md#cropping_from_the_sides_of_pdf_pages)

