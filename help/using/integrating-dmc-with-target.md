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

Bevor Sie [!DNL Adobe Dynamic Media Classic] mit [!DNL Target Standard/Premium] integrieren können, müssen Sie Ihre Ziel-URL im Bildschirm [!DNL Adobe Dynamic Media Classic] Allgemeine Programmeinstellungen eingeben. Um Ihre Target-URL abzurufen und sie auf der Seite &quot;Allgemeine Programmeinstellungen&quot;einzugeben, gehen Sie wie folgt vor:

1. Melden Sie sich in [!DNL Adobe Experience Cloud] bei Ihrem [!DNL Target Standard/Premium] -Konto an.
1. Kopieren Sie nach der Anmeldung in der Adressleiste Ihres Browsers die URL bis einschließlich `.com`.

   Wenn beispielsweise die URL *fiktional* (URL-Pfade enthalten immer Schrägstriche, nicht umgekehrte Schrägstriche wie in diesem Beispiel) in der Adressleiste den Wert `https:\\www.myfictionalsite.com/categories/admin/home.do` aufweist, kopieren Sie nur diesen Teil der URL *fiktional*: `https:\\www.myfictionalsite.com`.

1. Wechseln Sie in &quot;[!DNL Adobe Dynamic Media Classic]&quot;zu &quot;**[!UICONTROL Setup]**&quot;> &quot;**[!UICONTROL Anwendungseinstellungen]**&quot;.
1. Fügen Sie auf der Seite &quot;Allgemeine Programmeinstellungen&quot;im Feld **[!UICONTROL Test&amp;Target-Server-Name]** die URL ein, die Sie in Schritt 2 kopiert haben.
1. Wählen Sie **[!UICONTROL Close]** aus.
