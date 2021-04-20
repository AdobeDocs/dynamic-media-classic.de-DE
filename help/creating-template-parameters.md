---
title: Erstellen von Vorlagenparametern
description: Erfahren Sie, wie Sie Vorlagenparameter erstellen.
uuid: d17168a8-4776-4761-b022-8258d5997604
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: d263f041-5a0d-4c4f-9266-aeff51a5a7e2
feature: Dynamic Media Classic
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 97%

---


# Erstellen von Vorlagenparametern{#creating-template-parameters}

Durch Parameter können Sie Vorlagen mit maximaler Flexibilität verwenden, da Parameter die dynamische Anpassung eines Vorlagenbilds ermöglichen. Sie können festlegen, welche Text- und Bildebenen in das Vorlagenbild eingefügt und welche Parameter für die einzelnen Ebenen angezeigt werden sollen. Um beispielsweise die Aufmerksamkeit auf ein Produkt zu lenken, das im Ausverkauf ist, können Sie die Textebene „Ausverkauf“ erstellen. Später können Sie diese Ebene entfernen, das übrige Vorlagenbild jedoch beibehalten, indem Sie nur den Parameter „Ausverkauf“ entfernen.

Beim Erstellen von Vorlagenparametern legen Sie im Endeffekt fest, welche Teile der Vorlage in einer URL-Zeichenfolge aufgerufen werden. Das Einfügen bestimmter Parameter in eine URL-Zeichenfolge bewirkt, dass die den Parametern zugeordneten Elemente angezeigt werden. Mithilfe der Parameter können Sie also dynamisch beeinflussen, wie das vom Image-Server erstellte Vorlagenbild aussehen wird, und daraus benutzerdefinierte Ergebnisse erzeugen. Auf diese Weise können Sie eine Vorlage dynamisch ändern, indem Sie einige oder alle Parameter über die URL aufrufen.

Bei den Parametern für Textebenen können Sie auch die Textzeichenfolge zu einem dynamischen Feld machen, dem Werte in der Datenbank zugeordnet sind. Die Möglichkeit, Text mit einer Datenbank zu verknüpfen, ist beispielsweise für Werbekampagnen nützlich. Sie können dadurch benutzerdefinierte Vorlagenbilder erstellen, auf denen die Namen der Kunden angezeigt werden. Sie können beispielsweise auch einen Textebenenparameter mit einer Preisdatenbank verknüpfen, um den Preis eines Produkts in einem Vorlagenbild anzuzeigen.

Sie können einen Parameter mehrmals referenzieren. Verwenden Sie das Kombinationsfeld für jeden Befehl im Parameterdialogfeld, um alle Parameter auszuwählen, die zum jeweiligen Befehl passen. (Beispielsweise sind alle Größenparameter für den Befehl „size=“ verfügbar usw.) Sie können die Parameterreferenz einem beliebigen Parameter neu zuweisen, der bereits im Kombinationsfeld enthalten ist, und ihr einen neuen Namen geben, der nicht bereits im Kombinationsfeld vorhanden ist. Im letzteren Fall muss der Name eindeutig sein. Andernfalls wird eine Fehlermeldung angezeigt, die besagt, dass der Parameter bereits vorhanden ist. Wenn Sie eine Parameterreferenz löschen, wird der Parameter aus der URL gelöscht, wenn er nicht an einer anderen Stelle referenziert wird. Wenn Sie den Standardwert für einen Textparameter ändern, werden alle Referenzen zu diesem Parameter aktualisiert. Die Aktualisierung ist in der Ebenentabelle, in der Vorlagenanzeige und in der URL sichtbar. Wenn Sie ein Ebenenattribut ändern, indem Sie Griffpunkte verschieben oder im Eigenschaftenbedienfeld Werte eingeben, werden der Parameterwert sowie alle Referenzen zu diesem Parameter aktualisiert. Wenn Sie beispielsweise die Größe zweier Ebenen mithilfe eines Parameters festgelegt haben, werden beide Ebenengrößen aktualisiert, wenn eine der beiden Ebenengrößen geändert wird. Wenn Sie eine Vorlage in der Vorschau anzeigen und dort einen Parameter ändern, werden alle Referenzen zu diesem Parameter aktualisiert.

## Einstellen einer Parametervorgabe für eine Ebene  {#parameterizing-a-layer}

Führen Sie für jede Ebene in der Vorlage folgende Schritte zum Erstellen von Vorlagenparametern aus:

1. Klicken Sie in der Liste „Ebenen“ neben dem Namen der Ebene, für die Sie Parameter erstellen möchten, auf „Parameter“ . Der Anzeigebereich „Parameter“ wird geöffnet. Darin werden die Namen aller Parameter in der Ebene, deren Werte und deren Typ aufgelistet.
1. Aktivieren Sie neben dem Namen jedes Parameters, der in das Vorlagenbild eingefügt werden soll, die Option „Ein“.
1. Wählen Sie **Schließen**, um den Bildschirm &quot;Parameter&quot;zu verlassen.

>[!NOTE]
>
>Im Anzeigebereich „Parameter“ können Sie Parameter umbenennen. Durch das Umbenennen ist ein Parameter leichter in der URL-Zeichenfolge zu erkennen und kann einfacher als Datenbankwert verwendet werden. Um einen Parameter umzubenennen, aktivieren Sie dessen Option „Ein“, klicken Sie auf dessen Namen und geben Sie im Feld „Name“ einen neuen Namen ein.

Um eine Liste der Parameter anzuzeigen, die Sie für eine Vorlage erstellt haben, klicken Sie im Anzeigebereich „Vorlage“ auf „Parameterzusammenfassung“. Der Anzeigebereich „Parameterzusammenfassung“ wird angezeigt. Darin werden die Namen aller Ebenen und, falls Sie für eine Ebene Parameter erstellt haben, die Namen und Werte der Parameter aufgelistet.

## Festlegen dynamischer Textparameter  {#creating-dynamic-text-parameters}

Bei Textebenen können Sie außerdem die Textzeichenfolge zu einem dynamischen Feld machen, dem ein Datenbankwert zugeordnet ist. Führen Sie folgende Schritte aus:

1. Klicken Sie im Anzeigebereich „Vorlage“ neben dem Namen der Textebene, für die Sie dynamische Textparameter erstellen möchten, auf „Parameter“ . Der Anzeigebereich „Parameter“ wird geöffnet.
1. Aktivieren Sie die Option „Ein“ neben dem Namen des Textattributs (textAttr).
1. Rufen Sie im Anzeigebildschirm „Parameter“ die Registerkarte „Text“ auf.
1. Klicken Sie auf die Schaltfläche „Parameter hinzufügen“. Der standardmäßige Parametername wird angezeigt. Sie können diesen Namen ersetzen, indem Sie ihn markieren und dann überschreiben. Die aktuelle Textzeichenfolge wird der neue Name des Parameters.
1. Klicken Sie auf „Schließen“, um den Anzeigebereich „Parameter“ zu schließen.

Um dem Parameternamen einen Datenbankwert zuzuordnen, fügen Sie folgende Zeichenfolge an die Vorlagen-URL an:

```as3
?$_2(parameter name)=(database value)
```

Der Parametername wird durch Namen in einem Datenbankfeld oder durch Java-Code ersetzt, der z. B. auf den aktuellen Preis eines Produkts oder auf einen Kundennamen verweist.
