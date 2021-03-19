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
role: Geschäftspraktiker
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 85%

---


# Beschneiden eines Bildes{#cropping-an-image}

Sie können Bilder in Dynamic Media Classic beschneiden. Die Informationen zu den beschnittenen Bildern werden im System gespeichert, damit sie in ihrem ursprünglichen Zustand wiederhergestellt werden können. Sie können ein Bild auch beschneiden und die beschnittene Version unter einem neuen Namen speichern.

Sie haben die Möglichkeit, durch Beschneiden den weißen Bereich um das Bild herum zu entfernen oder einen beliebigen Bildbereich zu isolieren.

>[!NOTE]
>
>Sie können die beschnittene Version des Bilds unter einem anderen Namen speichern, indem Sie auf die Schaltfläche „Speichern unter“ klicken. Wählen Sie im Fenster „Speichern unter“ die Option „Als neue Masterversion speichern“, um eine zweite Kopie des Bilds zu speichern. Wählen Sie die Option „Als zusätzliche Ansicht des Masterbilds speichern“, um das Original und dessen beschnittene Version unter verschiedenen Namen zu speichern. Wählen Sie die Option „Original ersetzen“, um die Originaldatei, die Sie beschnitten haben, zu löschen. Geben Sie anschließend einen Namen für das Bild ein und klicken Sie auf „Absenden“.

## Beschneiden zum Entfernen des weißen Bereichs am Bildrand  {#crop-to-remove-white-space-around-an-image}

Sie können die transparenten oder einfarbigen Pixel am Rand eines Bilds durch Beschneiden entfernen.

1. Um ein Bild zu beschneiden, klicken Sie auf seine Rollover-Schaltfläche „Bearbeiten“ und wählen Sie „Beschneiden“ oder zeigen Sie es im Durchsuchenbedienfeld in der Detailansicht an und klicken Sie auf die Schaltfläche „Beschneiden“ . Der Anzeigebereich „Beschneidungseditor“ wird geöffnet.
1. Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie farbige Pixel beschneiden möchten, wählen Sie im Menü „Beschneiden“ den Befehl „Farbe“. Das Dialogfeld „Nach Farbe zuschneiden“ wird angezeigt. Wählen Sie im Menü „Ecke“ eine Ecke mit der Hintergrundfarbe aus, die abgeschnitten werden soll. Geben Sie für die Einstellung „Toleranz“ einen Wert zwischen 0 und 1 ein. Wenn Sie den Wert 0 einstellen, werden Pixel nur abgeschnitten, wenn sie exakt der Farbe entsprechen, die Sie in der Bildecke ausgewählt haben. Werte, die näher an 1 liegen, lassen eine größere Farbabweichung zu. Klicken Sie auf „Beschneiden“.
   * Wenn Sie transparente Pixel beschneiden möchten, wählen Sie im Menü „Beschneiden“ den Befehl „Transparent“. Das Dialogfeld „Auto-Zuschneiden nach Transparenz“ wird angezeigt. Geben Sie für die Einstellung „Toleranz“ einen Wert zwischen 0 und 1 ein. Wenn Sie den Wert 0 einstellen, werden nur vollkommen transparente Pixel abgeschnitten. Werte, die näher an 1 liegen, lassen eine größere Transparenzabweichung zu. Klicken Sie auf „Beschneiden“.

1. Klicken Sie auf „**Speichern**“.

>[!NOTE]
>
>Um ein Bild in seinen ursprünglichen Zustand zurück zu versetzen, nachdem Sie es beschnitten haben, zeigen Sie das Bild im Anzeigebereich „Beschneidungseditor“ an und klicken Sie auf „Zurücksetzen“.

## Auswählen eines zu beschneidenden Bereichs  {#select-an-area-to-crop}

1. Um ein Bild zu beschneiden, klicken Sie auf seine Rollover-Schaltfläche &quot;Bearbeiten&quot;und wählen Sie **Beschneiden** oder zeigen Sie es im Durchsuchenbedienfeld in der Ansicht &quot;Details&quot;an und klicken Sie auf **Beschneiden**.

1. Platzieren Sie im Fenster &quot;Beschneidungseditor&quot;den Bildausschnitt, den Sie nicht beschneiden möchten, im Feld &quot;Beschneiden&quot;. Was im Feld angezeigt wird, bleibt bestehen, wenn Sie auf **Speichern** klicken und das Bild beschneiden.
1. Führen Sie zum Anpassen des zu beschneidenden Bereichs einen der folgenden Schritte aus:

   * Ziehen Sie eine Seite oder Ecke des Rahmens. Halten Sie beim Ziehen die Umschalttaste gedrückt, um die Größe zu ändern, dabei jedoch das Seitenverhältnis (die Form) des zu beschneidenden Bereichs beizubehalten.
   * Geben Sie in den Feldern unter „Größe“ die gewünschten Pixelmaße an.
   * Verschieben Sie den Rahmen. Bewegen Sie den Zeiger in das Innere des Feldes. Wenn der Mauszeiger als Vierfachpfeil dargestellt wird, ziehen Sie den Rahmen an die gewünschte Position.

1. Klicken Sie auf „**Speichern**“.

>[!NOTE]
>
>Um ein Bild in seinen ursprünglichen Zustand zurück zu versetzen, nachdem Sie es beschnitten haben, zeigen Sie das Bild im Anzeigebereich „Beschneidungseditor“ an und klicken Sie auf „Zurücksetzen“.

>[!MORELIKETHIS]
>
>* [Bildbearbeitungsoptionen beim Hochladen](image-editing-options-upload.md#image-editing-options-at-upload)
>* [Beschneiden weißer Flächen in PDF-Dateien](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [Beschneiden der Kanten von PDF-Seiten](pdfs.md#cropping_from_the_sides_of_pdf_pages)

