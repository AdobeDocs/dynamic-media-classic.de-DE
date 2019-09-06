---
title: Weitergeben von Asset-Änderungen an Peers in Echtzeit
seo-title: Weitergeben von Asset-Änderungen an Peers in Echtzeit
description: 'null'
seo-description: Erfahren Sie, wie Sie Asset-Änderungen für Peers in Echtzeit freigeben.
uuid: 13 fa 4 f 6 e -66 bf -4682-96 a 9-0 e 7040706 f 53
contentOwner: admin
content-type: Verweis
products: SG_ EXPERIENCEMANAGER/Dynamic-Media-Scene -7
geptopics: SG_ SCENESEVENONDEMAND_ PK/categories/managing_ assets
discoiquuid: ca 7 c 8 a 7 f -76 f 4-4 a 25-8 c 36-617 a 029 e 55
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Weitergeben von Asset-Änderungen an Peers in Echtzeit{#sharing-asset-changes-with-peers-in-real-time}

Wenn mehrere Kopien von Dynamic Media Classic auf einem oder mehreren Computern im selben Unternehmen ausgeführt werden, werden die folgenden Aktionen von einem beliebigen dynamischen Media Classic-Client in Echtzeit mit allen Peer-Clients aktualisiert:

* Bearbeitung eines Assets (Builder, Bild-Editor usw.)
* Umbenennung eines Assets
* Löschung eines Assets
* Verschiebung eines Assets
* Hochladen mindestens eines Assets (sowohl Desktop als auch FTP)
* Erstellung, Löschung oder Umbenennung eines Ordners

Nach einer Änderung in einem Ausgangs-Client wird diese von allen Peer-Clients, die beim selben Unternehmen angemeldet sind, übernommen. Die Änderungen werden in den Peer-Clients ohne Benachrichtigung vorgenommen, es sei denn, ein geändertes Asset wird im Peer-Client in einem der Bild-Editoren oder Builder zur selben Zeit bearbeitet.

Bei der Anmeldung fordert Sie Flash Player auf, Peer-Aktualisierungen zuzulassen oder abzulehnen. Sie können festlegen, dass Ihre Auswahl gespeichert wird, sodass Sie die Eingabe nur einmal vornehmen müssen. Um Ihre Auswahl zu löschen, löschen Sie die jeweilige Site in den globalen Einstellungen aus dem Anzeigebereich „Peer-Netzwerk“.

Wenn Sie ein Asset gerade bearbeiten, das von einem Peer geändert wurde, werden Sie aufgefordert, die Änderung in den Builder oder Editor zu übernehmen. Wenn Sie „Ja“ auswählen, verwirft der Builder oder Editor Ihre eigenen Änderungen am Asset und importiert das aktualisierte Asset. Wenn Sie „Nein“ auswählen, wird das Asset im Builder oder Editor nicht aktualisiert und Ihre eigenen Änderungen bleiben in der Sitzung erhalten.

Nach dem Speichern des Assets werden Sie informiert, dass eine aktuellere Version vorhanden ist und gefragt, ob Sie das Asset mit Ihren Änderungen überschreiben möchten.
