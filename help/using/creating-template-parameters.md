---
title: Erstellen von Vorlagenparametern
description: Erfahren Sie, wie Sie Vorlagenparameter in Adobe Dynamic Media Classic erstellen.
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

Parameter ermöglichen es Ihnen, Vorlagen mit maximaler Flexibilität zu verwenden. Sie ermöglichen die dynamische Anpassung eines Vorlagenbilds. Sie können festlegen, welche Text- und Bildebenen in das Vorlagenbild eingefügt und welche Parameter für die einzelnen Ebenen angezeigt werden sollen. Um beispielsweise die Aufmerksamkeit auf ein Produkt zu lenken, das im Angebot ist, können Sie eine Textebene „Bei Verkauf“ erstellen. Später können Sie diese Ebene entfernen, das übrige Vorlagenbild jedoch beibehalten, indem Sie nur den Parameter „Ausverkauf“ entfernen.

Beim Erstellen von Vorlagenparametern legen Sie im Endeffekt fest, welche Teile der Vorlage in einer URL-Zeichenfolge aufgerufen werden. Das Einfügen bestimmter Parameter in eine URL-Zeichenfolge bewirkt, dass die den Parametern zugeordneten Elemente angezeigt werden. Mithilfe der Parameter können Sie also dynamisch beeinflussen, wie das vom Image-Server erstellte Vorlagenbild aussehen wird, und daraus benutzerdefinierte Ergebnisse erzeugen. Auf diese Weise können Sie eine Vorlage dynamisch ändern, indem Sie einige oder alle Parameter über die URL aufrufen.

Bei den Parametern für Textebenen können Sie auch die Textzeichenfolge zu einem dynamischen Feld machen, dem Werte in der Datenbank zugeordnet sind. Die Möglichkeit, Text mit einer Datenbank zu verknüpfen, ist beispielsweise für Werbekampagnen nützlich. Sie können dadurch benutzerdefinierte Vorlagenbilder erstellen, auf denen die Namen der Kunden angezeigt werden. Sie können auch einen Textebenenparameter mit einer Preisdatenbank verknüpfen, um den Preis eines Artikels in einem Vorlagenbild anzuzeigen.

Sie können einen Parameter mehrmals referenzieren. Verwenden Sie das Kombinationsfeld für jeden Befehl im Parameterdialogfeld, um alle Parameter auszuwählen, die zum jeweiligen Befehl passen. Beispielsweise stehen für den Befehl `size=` alle Größenparameter zur Verfügung. Sie können die Parameterreferenz einem beliebigen Parameter neu zuweisen, der bereits im Kombinationsfeld enthalten ist, und ihr einen neuen Namen geben, der nicht bereits im Kombinationsfeld vorhanden ist. In letzterem Fall muss der Name eindeutig sein. Andernfalls gibt ein Fehler an, dass der Parameter vorhanden ist. Wenn Sie einen Parameterverweis löschen, wird der Parameter aus der URL entfernt, sofern er nicht an anderer Stelle referenziert wird. Wenn Sie den Standardwert für einen Textparameter ändern, werden alle Verweise auf diesen Parameter aktualisiert. Sie können die Aktualisierung in der Ebenentabelle, im Rendering der Vorlage und in der URL sehen. Wenn Sie ein Ebenenattribut ändern, indem Sie Größenänderungsgriffe bearbeiten oder Werte in das Eigenschaftenbedienfeld eingeben, wird der Parameterwert aktualisiert und alle Verweise auf den Parameter werden aktualisiert. Wenn Sie beispielsweise die Größe zweier Ebenen mithilfe eines Parameters festgelegt haben, werden beide Ebenengrößen aktualisiert, wenn eine der beiden Ebenengrößen geändert wird. Wenn Sie eine Vorlage in der Vorschau anzeigen und dort einen Parameter ändern, werden alle Referenzen zu diesem Parameter aktualisiert.

Siehe auch [Vorlagengrundlagen](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) Schulungsvideo.

## Ebene parametrisieren {#parameterizing-a-layer}

Führen Sie für jede Ebene in der Vorlage folgende Schritte zum Erstellen von Vorlagenparametern aus:

1. Klicken Sie in der Liste Ebenen auf die Schaltfläche Parameter neben dem Namen der Ebene, für die Sie Parameter erstellen möchten. Der Anzeigebereich „Parameter“ wird geöffnet. Es listet den Namen jedes Parameters auf der Ebene, seinen Wert und seinen Typ auf.
1. Wählen Sie die Option Ein neben dem Namen jedes Parameters aus, den Sie in das Vorlagenbild aufnehmen möchten.
1. Wählen Sie **[!UICONTROL Schließen]**, um den Bildschirm „Parameter“ zu verlassen.

>[!NOTE]
>
>Im Anzeigebereich „Parameter“ können Sie Parameter umbenennen. Durch das Umbenennen ist ein Parameter leichter in der URL-Zeichenfolge zu erkennen und kann einfacher als Datenbankwert verwendet werden. Um einen Parameter umzubenennen, wählen Sie seine Option **[!UICONTROL Ein]**, wählen Sie seinen Namen aus und geben Sie einen neuen Namen in das Feld Name ein.

Um eine Liste der Parameter anzuzeigen, die Sie für Ihre Vorlage erstellt haben, klicken Sie im Vorlagenbildschirm auf die Schaltfläche Parameterübersicht . Im Bildschirm „Parameter-Zusammenfassung“ wird der Name jeder Ebene aufgelistet, und wenn Sie Parameter für eine Ebene erstellt haben, die Parameternamen und -werte.

## Erstellen dynamischer Textparameter {#creating-dynamic-text-parameters}

Bei Textebenen können Sie die Textzeichenfolge auch zu einem dynamischen Feld machen, das mit einem Datenbankwert verknüpft ist. Führen Sie folgende Schritte aus:

1. Wählen Sie im Vorlagenbildschirm die Schaltfläche Parameter neben dem Namen der Textebene, für die Sie dynamische Textparameter erstellen möchten. Die Seite „Parameter“ wird geöffnet.
1. Wählen Sie die **[!UICONTROL Ein]**-Option neben dem Namen des Textattributs (textAttr).
1. Wählen Sie die **[!UICONTROL Text]** im Bildschirm Parameter aus.
1. Wählen Sie **[!UICONTROL Parameter hinzufügen]** aus. Der standardmäßige Parametername wird angezeigt. Sie können diesen Namen ersetzen, indem Sie ihn markieren und dann überschreiben. Die aktuelle Textzeichenfolge wird der neue Name des Parameters.
1. Wählen Sie **[!UICONTROL Schließen]** aus, um die Seite „Parameter“ zu schließen.

Um dem Parameternamen einen Datenbankwert zuzuordnen, fügen Sie folgende Zeichenfolge an die Vorlagen-URL an:

```as3
?$_2(parameter name)=(database value)
```

Namen in einem Datenbankfeld oder Java™-Code ersetzen die Parameternamen. Eine solche Funktionalität zeigt beispielsweise den aktuellen Preis eines Artikels oder einen Kundennamen an.
