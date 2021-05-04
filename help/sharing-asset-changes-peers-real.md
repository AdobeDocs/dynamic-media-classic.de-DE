---
title: Weitergeben von Asset-Änderungen an Peers in Echtzeit
description: Erfahren Sie, wie Sie Asset-Änderungen in Echtzeit an andere weitergeben können.
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
feature: Dynamic Media Classic, Asset Management, Zusammenarbeit
role: Administrator,Business Practitioner
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
translation-type: tm+mt
source-git-commit: 9d73e74ffc4a1e7e31c84720a9bae105b6afb1ae
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 50%

---

# Weitergeben von Asset-Änderungen an Peers in Echtzeit{#sharing-asset-changes-with-peers-in-real-time}

Wenn mehrere Exemplare von Dynamic Media Classic auf einem oder mehreren Computern in derselben Firma ausgeführt werden, werden die folgenden Aktionen von jedem Dynamic Media Classic-Client in Echtzeit mit allen Peer-Clients aktualisiert:

* Bearbeiten eines Assets (Builder, Bild-Editor usw.)
* Umbenennung eines Assets
* Löschung eines Assets
* Verschiebung eines Assets
* Hochladen mindestens eines Assets (sowohl Desktop als auch FTP)
* Erstellung, Löschung oder Umbenennung eines Ordners

Nachdem im ursprünglichen Client eine Änderung vorgenommen wurde, werden alle Peer-Clients, die in derselben Firma angemeldet sind, mit der Änderung aktualisiert. Die Änderungen werden in den Peer-Clients ohne Benachrichtigung vorgenommen, es sei denn, ein geändertes Asset wird im Peer-Client in einem der Bild-Editoren oder Builder zur selben Zeit bearbeitet.

Wenn Sie sich anmelden, werden Sie aufgefordert, Peer-Aktualisierungen zuzulassen oder abzulehnen. Sie können festlegen, dass Ihre Auswahl gespeichert wird, sodass Sie die Eingabe nur einmal vornehmen müssen. Um Ihre Auswahl zu löschen, löschen Sie die jeweilige Site in den globalen Einstellungen aus dem Anzeigebereich „Peer-Netzwerk“.

Wenn Sie ein Asset gerade bearbeiten, das von einem Peer geändert wurde, werden Sie aufgefordert, die Änderung in den Builder oder Editor zu übernehmen. Wenn Sie **[!UICONTROL Ja]** auswählen, verwirft der Builder oder Editor alle Änderungen, die am Asset vorgenommen wurden, und importiert das aktualisierte Asset. Wenn Sie **[!UICONTROL Nein]** wählen, bleibt das Asset im Builder oder Editor unverändert und alle Änderungen, die Sie vorgenommen haben, bleiben in dieser Sitzung erhalten.

Nach dem Speichern des Assets werden Sie informiert, dass eine aktuellere Version vorhanden ist und gefragt, ob Sie das Asset mit Ihren Änderungen überschreiben möchten.
