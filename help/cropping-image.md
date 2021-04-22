---
title: Beschneiden eines Bildes
description: Erfahren Sie, wie Sie ein Bild beschneiden.
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic, Asset Management
role: Business Practitioner
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
translation-type: tm+mt
source-git-commit: 4e79c98b92dfa4e1a9890ed8a291cdf564126466
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 51%

---

# Beschneiden eines Bildes{#cropping-an-image}

Sie können Bilder in Dynamic Media Classic beschneiden. Die Informationen zu den beschnittenen Bildern werden im System gespeichert, damit sie in ihrem ursprünglichen Zustand wiederhergestellt werden können. Sie können ein Bild auch beschneiden und die beschnittene Version unter einem neuen Namen speichern.

Sie haben die Möglichkeit, durch Beschneiden den weißen Bereich um das Bild herum zu entfernen oder einen beliebigen Bildbereich zu isolieren.

>[!NOTE]
>
>Sie können die beschnittene Version des Bilds unter einem anderen Namen speichern, indem Sie auf die Schaltfläche „Speichern unter“ klicken. Wählen Sie im Fenster „Speichern unter“ die Option „Als neue Masterversion speichern“, um eine zweite Kopie des Bilds zu speichern. Klicken Sie auf **[!UICONTROL Als zusätzliche Ansicht von Übergeordnet]** speichern, um das Original und die zugeschnittene Version unter einem anderen Namen zu speichern. Klicken Sie auf **[!UICONTROL Original ersetzen]**, um die Originaldatei zu löschen, von der Sie das Bild beschnitten haben. Geben Sie dann einen Namen für das Bild ein und klicken Sie auf **[!UICONTROL Senden]**.

## Beschneiden zum Entfernen des weißen Bereichs am Bildrand {#crop-to-remove-white-space-around-an-image}

Sie können die transparenten oder einfarbigen Pixel am Rand eines Bilds durch Beschneiden entfernen.

1. Um ein Bild zu beschneiden, klicken Sie auf dessen Rollover **[!UICONTROL Bearbeiten]** und wählen Sie **[!UICONTROL Zuschneiden]** oder zeigen Sie es im Durchsuchenbedienfeld in der Ansicht &quot;Details&quot;an und klicken Sie auf die Schaltfläche **[!UICONTROL Beschneiden]**.
1. Führen Sie auf der Seite &quot;Beschneidungseditor&quot;einen der folgenden Schritte aus:

   * Klicken Sie zum Beschneiden von Farbpixeln auf **[!UICONTROL Beschneiden]** > **[!UICONTROL Farbe]**. Das Dialogfeld „Nach Farbe zuschneiden“ wird angezeigt. Klicken Sie auf das Menü **[!UICONTROL Ecke]** und wählen Sie eine Ecke mit der Hintergrundfarbe aus, die entfernt werden soll. Geben Sie dann die Einstellung **[!UICONTROL Toleranz]** zwischen 0 und 1 ein. Wenn Sie den Wert 0 einstellen, werden Pixel nur abgeschnitten, wenn sie exakt der Farbe entsprechen, die Sie in der Bildecke ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu. Klicken Sie auf die Schaltfläche **[!UICONTROL Zuschneiden]**.
   * Um transparente Pixel zu beschneiden, klicken Sie auf **[!UICONTROL Beschneiden]** > **[!UICONTROL Transparent]**. Das Dialogfeld „Auto-Zuschneiden nach Transparenz“ wird angezeigt. Geben Sie für die Einstellung „Toleranz“ einen Wert zwischen 0 und 1 ein. Bei der Einstellung 0 werden Pixel nur abgeschnitten, wenn sie transparent sind. Werte, die näher an 1 liegen, lassen eine größere Transparenzabweichung zu. Klicken Sie auf **[!UICONTROL Zuschneiden]**.

1. Klicken Sie auf „**[!UICONTROL Speichern]**“.

>[!NOTE]
>
>Um ein Bild nach dem Beschneiden in den Originalzustand zu versetzen, zeigen Sie das Bild im Anzeigebereich &quot;Beschneidungseditor&quot;an und klicken Sie auf **[!UICONTROL Zurücksetzen]**.

## Auswählen eines zu beschneidenden Bereichs {#select-an-area-to-crop}

1. Um ein Bild zu beschneiden, klicken Sie auf dessen Rollover **[!UICONTROL Bearbeiten]** und wählen Sie **[!UICONTROL Beschneiden]** oder zeigen Sie es im Durchsuchenbedienfeld in der Ansicht &quot;Details&quot;an und klicken Sie auf **[!UICONTROL Beschneiden]**.

1. Platzieren Sie im Fenster &quot;Beschneidungseditor&quot;den Bildausschnitt, den Sie nicht beschneiden möchten, im Feld &quot;Beschneiden&quot;. Im Feld wird angezeigt, was bleibt, wenn Sie auf **[!UICONTROL Speichern]** klicken und das Bild beschneiden.
1. Führen Sie zum Anpassen des zu beschneidenden Bereichs einen der folgenden Schritte aus:

   * Ziehen Sie eine Seite oder Ecke des Rahmens. Halten Sie beim Ziehen die Umschalttaste gedrückt, um die Größe zu ändern, dabei jedoch das Seitenverhältnis (die Form) des zu beschneidenden Bereichs beizubehalten.
   * Geben Sie in den Feldern unter „Größe“ die gewünschten Pixelmaße an.
   * Verschieben Sie den Rahmen. Bewegen Sie den Zeiger in das Innere des Feldes. Wenn der Mauszeiger als Vierfachpfeil dargestellt wird, ziehen Sie den Rahmen an die gewünschte Position.

1. Klicken Sie auf „**[!UICONTROL Speichern]**“.

>[!NOTE]
>
>Um ein Bild nach dem Beschneiden in seinen ursprünglichen Zustand wiederherzustellen, zeigen Sie das Bild im Anzeigebereich &quot;Beschneidungseditor&quot;an und klicken Sie auf **[!UICONTROL Zurücksetzen]**.

>[!MORELIKETHIS]
>
>* [Bildbearbeitungsoptionen beim Hochladen](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Beschneiden weißer Flächen in PDF-Dateien](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Beschneiden der Kanten von PDF-Seiten](pdfs.md#cropping_from_the_sides_of_pdf_pages)

