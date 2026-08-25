---
title: Asset-Änderungen mit Peer-Clients in Echtzeit freigeben
description: Erfahren Sie, wie Sie in Adobe Dynamic Media Classic Asset-Änderungen in Echtzeit für Kollegen freigeben können.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
topic: Administration, Collaboration
level: Intermediate
autotag-review: '2026-05-13T20:12:54.992Z'
TQID: 'https://experienceleague.adobe.com/Yn5GsnQ4cM3Byk18iEB8Z4uGsTt9FjEZOBP17Yt-K8M'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 4c8d0e861708e8931bbefe55260c7704c43e0ce6
workflow-type: tm+mt
source-wordcount: 285
ht-degree: 14%

---

# Asset-Änderungen mit Peer-Clients in Echtzeit freigeben{#sharing-asset-changes-with-peers-in-real-time}

Es werden mehrere Instanzen von Adobe Dynamic Media Classic auf Computern in derselben Organisation ausgeführt. In einem solchen Fall werden die folgenden Aktionen von einem beliebigen Dynamic Media Classic-Client in Echtzeit auf allen Peer-Clients aktualisiert:

* Bearbeiten von Assets (Builder, Bildeditor usw.)
* Umbenennung eines Assets
* Löschung eines Assets
* Verschiebung eines Assets
* Hochladen mindestens eines Assets (sowohl Desktop als auch FTP)
* Erstellung, Löschung oder Umbenennung eines Ordners

Nachdem eine Änderung am ursprünglichen Client vorgenommen wurde, werden alle Peer-Clients, die bei derselben Firma angemeldet sind, mit der Änderung aktualisiert. Änderungen werden automatisch auf Kollegen angewendet, sofern die Kollegen das Asset in keinem der Bildeditoren oder -ersteller bearbeiten.

Wenn Sie sich anmelden, werden Sie aufgefordert, Peer-Aktualisierungen zuzulassen oder abzulehnen. Sie können die Auswahl speichern, sodass Sie nur einmal dazu aufgefordert werden. Um Ihre Auswahl zu löschen, löschen Sie die jeweilige Site in den globalen Einstellungen aus dem Anzeigebereich „Peer-Netzwerk“.

Wenn Sie ein von einem Peer geändertes Asset bearbeitet haben, werden Sie aufgefordert, die Änderung in den Builder oder Editor aufzunehmen. Bei Auswahl von **[!UICONTROL Ja]** verwirft der Builder oder Editor alle am Asset vorgenommenen Änderungen und importiert das aktualisierte Asset. Wenn Sie **[!UICONTROL Nein]** wählen, ist das Asset im Builder oder Editor unverändert und alle von Ihnen vorgenommenen Änderungen bleiben in dieser Sitzung bestehen.

Beim Speichern des Assets werden Sie darüber informiert, dass eine neuere Version vorhanden ist. Sie werden dann aufgefordert zu bestätigen, ob Sie das Asset mit Ihren Änderungen überschreiben möchten.
