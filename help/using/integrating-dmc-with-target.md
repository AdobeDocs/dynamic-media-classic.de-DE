---
title: Integrieren von Adobe Dynamic Media Classic mit Adobe Target Standard/Premium
description: Erfahren Sie, wie Sie Adobe Dynamic Media Classic mit Adobe Target Standard/Premium integrieren.
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
topic: Integrations, Development
level: Experienced
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---

# Integrieren von Adobe Dynamic Media Classic mit Adobe Target Standard/Premium {#integrating-dmc-with-target}

Vor der Integration [!DNL Adobe Dynamic Media Classic] mit [!DNL Target Standard/Premium]müssen Sie Ihre Target-URL in der Variablen [!DNL Adobe Dynamic Media Classic] Bildschirm &quot;Allgemeine Programmeinstellungen&quot;. Um Ihre Target-URL abzurufen und sie auf der Seite &quot;Allgemeine Programmeinstellungen&quot;einzugeben, gehen Sie wie folgt vor:

1. In [!DNL Adobe Experience Cloud]anmelden, [!DNL Target Standard/Premium] -Konto.
1. Kopieren Sie nach der Anmeldung in die Adressleiste Ihres Browsers die URL bis einschließlich `.com`.

   Wenn beispielsweise die Variable *fiktiv* URL (URL-Pfade enthalten immer Schrägstriche, nicht umgekehrte Schrägstriche wie in diesem Beispiel) in der Adressleiste `https:\\www.myfictionalsite.com/categories/admin/home.do`, kopieren Sie nur diesen Teil der *fiktiv* URL: `https:\\www.myfictionalsite.com`.

1. In [!DNL Adobe Dynamic Media Classic], gehen Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL Anwendungseinstellungen]**.
1. Auf der Seite &quot;Allgemeine Programmeinstellungen&quot;im **[!UICONTROL Test&amp;Target-Server-Name]** ein, fügen Sie die URL ein, die Sie in Schritt 2 kopiert haben.
1. Auswählen **[!UICONTROL Schließen]**.
