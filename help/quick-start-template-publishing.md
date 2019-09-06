---
title: '" Kurzanleitung: Vorlagen für Veröffentlichungen "'
seo-title: '" Kurzanleitung: Vorlagen für Veröffentlichungen "'
description: 'null'
seo-description: Eine Einführung und Schnellstart zu Vorlagen für Vorlagen, die Ihnen helfen, schnell zu arbeiten.
uuid: 101 b 6211-2421-4565-8635-944315 a 5 c 512
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/template-publishing
discoiquuid: 03671 fc 1-ce 3 b -4 fae-ad 1 f -53 c 99 abcabde
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Quick Start: Template publishing{#quick-start-template-publishing}

Mit Adobe Dynamic Media Classic Web-to-Print können Sie professionell markierte Inhalte erstellen, die Ihren Kunden, Kunden und Mitarbeitern leicht anzupassen und personalisieren zu können. Auf diese Weise wird dafür gesorgt, dass Unternehmensinhalte und die Markenidentität im gesamten Veröffentlichungsprozess konsistent einheitlich präsentiert wird. Die Endbenutzer können die Druckinhalte individuell anpassen, allerdings nur in dem Rahmen, den Sie ihnen erlauben. Beispiele für solche angepasste Druckprodukte sind personalisiertes Briefpapier, Visitenkarten, Poster, Grußkarten, Etiketten, Schecks, Geschenke, Kleidungsstücke, Kalender, Sammelalben und Fotoalben. Unternehmen können so für eine einheitliche Markenidentität in ihren Materialien sorgen, die für die einzelnen Regionen, Franchisepartner, Geschäfte und Niederlassungen angepasst werden kann.

Zunächst erstellen Sie eine Vorlage in Adobe Illustrator. Mit der Vorlage legen Sie genau fest, was konstant und was variabel ist. Die variablen Komponenten sind dann die Komponenten, die angepasst werden können. So können Endbenutzer z. B. in einer Illustrator-Datei Text, der als variable Komponente parametrisiert wurde, durch eigenen Text ersetzen. Auch eine Hintergrundfarbe kann, nachdem sie als variable Komponente parametrisiert wurde, gegen eine andere Hintergrundfarbe ausgetauscht werden.

Dynamic Media Classic bietet zwei Workflows für Vorlagen für Veröffentlichungen, eine für einfache Verwendungen und eine für erweiterte Anwendungsfälle. Bei einfachen Anwendungsfällen muss in Adobe Illustrator ein Entwurf erstellt werden, das Sie dann in dynamisches Media Classic hochladen und Variablenelemente mit Parametern im SPS definieren können. Der Workflow für erweiterte Verwendungen erfordert eine umfangreichere Definition der Variabilität. Für erweiterte Anwendungsfälle ist es erforderlich, variable Elemente in Adobe Illustrator zu erstellen, die Datei in Dynamic Media Classic hochzuladen und diese Elemente direkt auf einer XML-Ebene mit URL-Aufrufen zu manipulieren. Dieses Szenario wird aufgerufen *`*DOM manipulation*`*.

>[!NOTE]
>
>For more information about Dynamic Media Classic web-to-print workflows, template creation, parameterization, DOM manipulation, and more, see the Web-to-Print Workflow Guide here: [www.adobe.com/go/learn_s7_webtoprint_en](https://www.adobe.com/go/learn_s7_webtoprint_en) . Laden Sie die ZIP-Datei auf Ihre Festplatte herunter und extrahieren Sie den Inhalt (das dynamische Media-to-printworkflow-Übungsdokument und Übungselemente).

**Kurzanleitung**

In dieser Kurzanleitung wird der Workflow für einfache Verwendungen beschrieben, mit dem anhand von Illustrator-Dateien hochwertige, anpassbare Druckprodukte erstellt werden können.

**1. Entwerfen Ihrer Illustrator-Datei für das Veröffentlichen von Vorlagen**

Entwerfen Sie die Vorlage in Illustrator. Wenn Sie zum Anpassen Ihrer Vorlage die DOM-Manipulation verwenden möchten, definieren Sie in Illustrator s7:elementIDs für die variablen Elemente.

Informationen dazu finden Sie in den Abschnitten [Erstellen der Ausgangsvorlage in Illustrator](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator) und [DOM-Manipulation](dom-manipulation.md#dom_manipulation).

**2. Convert your template to Dynamic Media Classic FXG and upload it to Scene7 Publishing System**

Adobe Creative Cloud-Benutzer können das Adobe Illustrator-Zusatzmodul für Web-to-Print verwenden. Dieses Plug-In konvertiert Vorlagen in Dynamic Media Classic FXG. Wenn eine Vorlage Schriftarten enthält, müssen die entsprechenden Schriftartdateien in das Scene7 Publishing System hochgeladen werden, bevor die FXG-Datei hochgeladen wird.

Informationen dazu finden Sie im Abschnitt [Hochladen von Dateien für Vorlagen für Veröffentlichungen](upload-files-template-publishing.md#upload_files_for_template_publishing).

**3. Anzeigen, Definieren oder Verfeinern von Parametern in Dynamic Media Classic**

In den Anzeigebereichen „Vorschau“ und „Erstellen“ von Vorlagen für Veröffentlichungen können Sie variable Elemente über Parameter definieren und verfeinern, sich eine Vorschau der Ergebnisse ansehen und die Ergebnisse testen. Diese Anzeigebereiche bieten die folgenden Möglichkeiten:

* Erstellen und Bearbeiten von Parametern
* Festlegen von Standardwerten für Parametereigenschaften und -attribute
* Kopieren der Vorschau-URL in die Zwischenablage durch Klicken auf „URL kopieren“, um sich das Ergebnis in einem Browserfenster als Vorschau anzeigen zu lassen.

Siehe [Parametrisieren einer Vorlage in Dynamic Media Classic](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7).

**4. Veröffentlichen der FXG-Vorlage**

Wenn Sie mit dem Definieren und Testen der Parameter und Attribute fertig sind, können Sie die Datei veröffentlichen. Durch das Veröffentlichen der FXG-Vorlage wird diese auf den Image-Servern für dynamische Medien platziert und die URL aktiviert.

Achten Sie darauf, alle Bilder und Schriftarten zu veröffentlichen, die der FXG-Vorlage zugeordnet sind. 

Siehe [Veröffentlichen von FXG-Vorlagen](dom-manipulation.md#publish_fxg_templates).

**5. Abrufen der URL**

Über ihre URL kann die Vorlage jetzt in Ihre Website eingebettet werden und die Endbenutzer können den variablen Inhalt personalisieren. 

Siehe [Verknüpfen einer FXG-Vorlage mit einer Webseite](linking-fxg-template-web-page.md#linking_an_fxg_template_to_a_web_page).
