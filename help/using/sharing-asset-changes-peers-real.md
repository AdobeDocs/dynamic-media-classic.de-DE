---
title: Freigeben von Asset-Änderungen für Kollegen in Echtzeit
description: Erfahren Sie, wie Sie Asset-Änderungen in Echtzeit in Adobe Dynamic Media Classic für andere freigeben können.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 163eb32112ec6fbefd1dacf48212353ff3053d54
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 26%

---

# Freigeben von Asset-Änderungen für Kollegen in Echtzeit{#sharing-asset-changes-with-peers-in-real-time}

Angenommen, Sie verfügen über mehrere Kopien von Adobe Dynamic Media Classic, die auf Computern im selben Unternehmen ausgeführt werden. In einem solchen Szenario werden die folgenden Aktionen eines Dynamic Media Classic-Clients in Echtzeit mit allen Peer-Clients aktualisiert:

* Bearbeiten eines Assets (Builder, Bildeditor usw.)
* Umbenennung eines Assets
* Löschung eines Assets
* Verschiebung eines Assets
* Hochladen mindestens eines Assets (sowohl Desktop als auch FTP)
* Erstellung, Löschung oder Umbenennung eines Ordners

Nachdem eine Änderung im ursprünglichen Client vorgenommen wurde, werden alle Peer-Clients, die in demselben Unternehmen angemeldet sind, mit der Änderung aktualisiert. Die Änderungen werden in den Peer-Clients ohne Benachrichtigung vorgenommen, es sei denn, ein geändertes Asset wird im Peer-Client in einem der Bild-Editoren oder Builder zur selben Zeit bearbeitet.

Als Sie sich angemeldet haben, wurden Sie aufgefordert, Peer-Aktualisierungen zuzulassen oder abzulehnen. Sie können festlegen, dass Ihre Auswahl gespeichert wird, sodass Sie die Eingabe nur einmal vornehmen müssen. Um Ihre Auswahl zu löschen, löschen Sie die jeweilige Site in den globalen Einstellungen aus dem Anzeigebereich „Peer-Netzwerk“.

Wenn Sie ein Asset bearbeitet haben, das von einem Gleichrangigen geändert wurde, werden Sie aufgefordert, die Änderung in den Builder oder Editor aufzunehmen. Wenn Sie **[!UICONTROL Ja]** auswählen, verwirft der Builder oder Editor alle Änderungen am Asset und importiert das aktualisierte Asset. Wenn Sie &quot;**[!UICONTROL Nein]**&quot;auswählen, bleibt das Asset im Builder oder Editor unverändert, und alle Änderungen, die Sie vorgenommen haben, bleiben in dieser Sitzung bestehen.

Beim Speichern des Assets wurden Sie benachrichtigt, dass eine neuere Version vorhanden ist, und Sie wurden gefragt, ob Sie das Asset mit Ihren Änderungen überschreiben möchten.
