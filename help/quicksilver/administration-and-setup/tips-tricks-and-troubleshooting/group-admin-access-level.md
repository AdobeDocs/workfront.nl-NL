---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Groepbeheerders moeten een hogere toegang hebben dan de beheerders
description: Als een groepsbeheerder toestemmingen in hun toegangsniveau lager heeft dan die zij leiden, zullen zij niet kunnen bekijken, wijzigen of, lagere toegangsniveaus toewijzen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2b501a1e-fb56-44fa-8518-07537dc90a5b
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---

# Groepbeheerders moeten een hogere toegang hebben dan de beheerders die ze beheren

Als een groepsbeheerder toestemmingen in hun toegangsniveau lager heeft dan die zij leiden, zullen zij niet kunnen bekijken, wijzigen of, lagere toegangsniveaus toewijzen.

## Probleem

Als een groepsbeheerder een gewijzigd de toegangsniveau van de Planner met de toestemmingen van de Mening voor Teams wordt toegewezen, maar bepaalde gebruikers een de toegangsniveau van de Arbeider met Edit toestemmingen voor Teams worden toegewezen, zal de groepsbeheerder niet met het gewijzigde de toegangsniveau van de Arbeider kunnen in wisselwerking staan.

![ Admin van de Groep veranderde toegang ](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Deze logica is ook van toepassing op het vervolgkeuzemenu Uw instellingen nauwkeurig instellen. Beide toegangsniveaus kunnen Edit toegang hebben, maar de montages in het Fijne vereffenings uw montages drop-down menu moeten hoger voor groepbeheer zijn.
> ![Uw instellingen nauwkeurig afstemmen ](assets/fine-tune-your-settings.png)

## Oplossing

Groepbeheerders moeten op alle gebieden in het toegangsniveau over hogere machtigingen beschikken dan de beheerders beheren.
