---
title: Erstellen von Vorlagenparametern
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic Vorlagenparameter erstellen.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 118806ea-c8a7-4aaf-9ae3-739c6b04ea77
topic: Development
level: Experienced
source-git-commit: 00591bdbe721035e25d3dea245a2110f978d19aa
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 45%

---

# Erstellen von Vorlagenparametern{#creating-template-parameters}

Parameter ermöglichen die Verwendung von Vorlagen mit maximaler Flexibilität. Sie ermöglichen die dynamische Anpassung eines Vorlagenbilds. Sie können festlegen, welche Text- und Bildebenen in das Vorlagenbild eingefügt und welche Parameter für die einzelnen Ebenen angezeigt werden sollen. Um beispielsweise die Aufmerksamkeit auf ein Produkt zu lenken, das im Angebot ist, können Sie eine Textebene &quot;Verkauf&quot;erstellen. Später können Sie diese Ebene entfernen, das übrige Vorlagenbild jedoch beibehalten, indem Sie nur den Parameter „Ausverkauf“ entfernen.

Beim Erstellen von Vorlagenparametern legen Sie im Endeffekt fest, welche Teile der Vorlage in einer URL-Zeichenfolge aufgerufen werden. Das Einfügen bestimmter Parameter in eine URL-Zeichenfolge bewirkt, dass die den Parametern zugeordneten Elemente angezeigt werden. Mithilfe der Parameter können Sie also dynamisch beeinflussen, wie das vom Image-Server erstellte Vorlagenbild aussehen wird, und daraus benutzerdefinierte Ergebnisse erzeugen. Auf diese Weise können Sie eine Vorlage dynamisch ändern, indem Sie einige oder alle Parameter über die URL aufrufen.

Bei den Parametern für Textebenen können Sie auch die Textzeichenfolge zu einem dynamischen Feld machen, dem Werte in der Datenbank zugeordnet sind. Die Möglichkeit, Text mit einer Datenbank zu verknüpfen, ist beispielsweise für Werbekampagnen nützlich. Sie können dadurch benutzerdefinierte Vorlagenbilder erstellen, auf denen die Namen der Kunden angezeigt werden. Sie können auch einen Text-Layer-Parameter mit einer Preisdatenbank verknüpfen, um den Preis eines Artikels in einem Vorlagenbild anzuzeigen.

Sie können einen Parameter mehrmals referenzieren. Verwenden Sie das Kombinationsfeld für jeden Befehl im Parameterdialogfeld, um alle Parameter auszuwählen, die zum jeweiligen Befehl passen. Beispielsweise sind alle Größenparameter für `size=` Befehl. Sie können die Parameterreferenz einem beliebigen Parameter neu zuweisen, der bereits im Kombinationsfeld enthalten ist, und ihr einen neuen Namen geben, der nicht bereits im Kombinationsfeld vorhanden ist. In letzterem Fall muss der Name eindeutig sein. Andernfalls gibt ein Fehler an, dass der Parameter vorhanden ist. Wenn Sie einen Parameterverweis löschen, wird der Parameter aus der URL entfernt, wenn er nirgendwo anders referenziert wird. Wenn Sie den Standardwert für einen Textparameter ändern, werden alle Verweise auf diesen Parameter aktualisiert. Die Aktualisierung wird in der Ebenentabelle, im Rendering der Vorlage und in der URL angezeigt. Wenn Sie ein Ebenenattribut ändern, indem Sie Größenänderungs-Handles bearbeiten oder Werte im Eigenschaftenbereich eingeben, wird der Parameterwert aktualisiert und alle Verweise auf den Parameter werden aktualisiert. Wenn Sie beispielsweise die Größe zweier Ebenen mithilfe eines Parameters festgelegt haben, werden beide Ebenengrößen aktualisiert, wenn eine der beiden Ebenengrößen geändert wird. Wenn Sie eine Vorlage in der Vorschau anzeigen und dort einen Parameter ändern, werden alle Referenzen zu diesem Parameter aktualisiert.

Siehe auch [Vorlagengrundlagen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) Schulungsvideo.

## Parametrisieren einer Ebene {#parameterizing-a-layer}

Führen Sie für jede Ebene in der Vorlage folgende Schritte zum Erstellen von Vorlagenparametern aus:

1. Wählen Sie in der Liste &quot;Ebenen&quot;die Schaltfläche Parameter neben dem Namen der Ebene aus, für die Sie Parameter erstellen möchten. Der Anzeigebereich „Parameter“ wird geöffnet. Er listet den Namen der einzelnen Parameter auf der Ebene, deren Wert und den Typ auf.
1. Wählen Sie die Option Ein neben dem Namen der einzelnen Parameter, die Sie in das Vorlagenbild aufnehmen möchten.
1. Auswählen **[!UICONTROL Schließen]** , um den Bildschirm Parameter zu verlassen.

>[!NOTE]
>
>Im Anzeigebereich „Parameter“ können Sie Parameter umbenennen. Durch das Umbenennen ist ein Parameter leichter in der URL-Zeichenfolge zu erkennen und kann einfacher als Datenbankwert verwendet werden. Um einen Parameter umzubenennen, wählen Sie dessen **[!UICONTROL on]** , wählen Sie den Namen aus und geben Sie einen neuen Namen in das Feld &quot;Name&quot;ein.

Um eine Liste der Parameter anzuzeigen, die Sie für Ihre Vorlage erstellt haben, wählen Sie im Bildschirm &quot;Vorlage&quot;die Schaltfläche Parameterzusammenfassung aus. Im Bildschirm &quot;Parameterzusammenfassung&quot;wird der Name jeder Ebene aufgelistet. Wenn Sie Parameter für eine Ebene erstellt haben, werden die Parameternamen und -werte aufgeführt.

## Dynamische Textparameter erstellen {#creating-dynamic-text-parameters}

Bei Textebenen können Sie die Textzeichenfolge auch zu einem dynamischen Feld machen, das mit einem Datenbankwert verknüpft ist. Führen Sie folgende Schritte aus:

1. Wählen Sie im Bildschirm &quot;Vorlage&quot;die Schaltfläche Parameter neben dem Namen der Textebene aus, für die Sie dynamische Textparameter erstellen möchten. Die Seite Parameter wird geöffnet.
1. Wählen Sie die **[!UICONTROL on]** neben dem Namen des Textattributs (textAttr).
1. Wählen Sie die **[!UICONTROL Text]** im Bildschirm &quot;Parameter&quot;angezeigt.
1. Auswählen **[!UICONTROL Parameter hinzufügen]**. Der standardmäßige Parametername wird angezeigt. Sie können diesen Namen ersetzen, indem Sie ihn markieren und dann überschreiben. Die aktuelle Textzeichenfolge wird der neue Name des Parameters.
1. Auswählen **[!UICONTROL Schließen]** , um die Seite Parameter zu schließen.

Um dem Parameternamen einen Datenbankwert zuzuordnen, fügen Sie folgende Zeichenfolge an die Vorlagen-URL an:

```as3
?$_2(parameter name)=(database value)
```

Namen in einem Datenbankfeld oder Java™-Code ersetzen die Parameternamen. Diese Funktion zeigt beispielsweise den aktuellen Preis eines Artikels oder einen Kundennamen an.
