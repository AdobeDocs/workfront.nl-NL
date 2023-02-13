---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Groepbeheerders moeten een hogere toegang hebben dan de beheerders die ze beheren
description: Als een groepsbeheerder toestemmingen in hun Niveau van de Toegang heeft lager dan die zij leiden, zullen zij niet kunnen bekijken, wijzigen of, lagere toegangsniveaus toewijzen.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 458149110d71475820dc6f3b27f1e062c3fe66f6
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# Groepbeheerders moeten een hogere toegang hebben dan de beheerders die ze beheren

Als een groepsbeheerder toestemmingen in hun Niveau van de Toegang heeft lager dan die zij leiden, zullen zij niet kunnen bekijken, wijzigen of, lagere toegangsniveaus toewijzen.

## Probleem

Als een groepsbeheerder een gewijzigd de toegangsniveau van de Planner met de toestemmingen van de Mening voor Teams wordt toegewezen, maar bepaalde gebruikers een de toegangsniveau van de Arbeider met Edit toestemmingen voor Teams worden toegewezen, zal de groepsbeheerder niet met het gewijzigde de toegangsniveau van de Arbeider kunnen in wisselwerking staan.

![](assets/group-admin-modified-access.png)


>[!NOTE]
>
>Deze logica is ook van toepassing op het vervolgkeuzemenu Uw instellingen nauwkeurig instellen. Beide toegangsniveaus kunnen Edit toegang hebben, maar de montages in het Fijne vereffenings uw montages drop-down menu moeten hoger voor groepbeheer zijn.
> ![](assets/fine-tune-your-settings.png)

## Oplossing

Groepbeheerders moeten op alle gebieden in het toegangsniveau over hogere machtigingen beschikken dan de beheerders beheren.