---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: Overzicht subgroepen
description: U kunt maximaal 14 niveaus subgroepen maken onder één groep. Op elk van deze niveaus kunt u een onbeperkt aantal parallelle subgroepen maken.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# Overzicht subgroepen

U kunt maximaal 14 niveaus subgroepen maken onder één groep. Op elk van deze niveaus kunt u een onbeperkt aantal parallelle subgroepen maken. Voor instructies, zie [ een subgroep ](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md) creëren.

Voor informatie over groepen, zie [ Overzicht van Groepen ](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Wat erven subgroepen?

Subgroepen nemen het lidmaatschap van hun oudergroep over. Gebruikers en groepen in een subgroep hebben dus dezelfde zichtbaarheid, machtigingen en toegang tot alle objecten als gebruikers en groepen die behoren tot de bovenliggende groep die ze delen.

Ook, erft een subgroep automatisch de groepsbeheerders van zijn top-level groep, maar u kunt leden van een subgroep ook toewijzen om als zijn groepsbeheerders te handelen.

>[!TIP]
>
>Soms wilt u subgroepen gebruiken om meerdere gebruikers toe te voegen aan een bestaande groep, zodat ze toegang krijgen tot een object dat ze nodig hebben.
>
>Stel dat u een groep helpdesktechnici en een aparte groep IT-directeuren hebt. De helpdeskgroep heeft toestemmingen aan een bepaalde Rij van het Verzoek. U wilt de directeuren van IT aan de helpdeskgroep toevoegen zodat zij ook toestemmingen aan de Rij van het Verzoek hebben. Zonder de subgroepfunctionaliteit, zou u de directeuren van IT aan de helpdeskgroep manueel moeten toevoegen, die inefficiënt en moeilijk zou kunnen zijn te beheren. Als u de groep van de directeuren van IT aan de helpdeskgroep als subgroep toevoegt, voert u deze taak sneller met enkel één verandering uit.

>[!NOTE]
>
>Als een gebruiker afzonderlijk aan zowel een subgroep als aan zijn oudergroep werd toegevoegd, verwijdert het verwijderen van de gebruiker uit één niet de gebruiker uit andere. Als u niet wilt dat de gebruiker toegang voor de oudergroep wordt toegestaan, moet u de gebruiker zowel uit subgroup als uit de oudergroep verwijderen.

## Openbare en particuliere subgroepen

Voor een openbare groep kan elke gebruiker (in of uit de groep) die toegang heeft tot een gebruiker met bewerkingen de groep toevoegen aan het profiel van andere gebruikers. Ze kunnen dit niet doen voor een privégroep.

U kunt deze optie alleen bewerken in de bovenste bovenliggende groep in een hiërarchie van groepen met meer dan één niveau. Alle subgroepen van de bovenliggende groep nemen de instelling over.

Als u een subgroep onder een groep maakt die openbaar is, is de subgroep standaard ook openbaar. Voor meer informatie over het creëren van een groep en het maken van het openbaar, zie [ een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) creëren. Voor meer informatie over de toegang nodig om gebruikers uit te geven, zie [ toegang van de Verlening tot gebruikers ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Elke groep die u toevoegt aan een bestaande groep wordt automatisch een subgroep en is geen hoofdgroep meer. Nochtans, behoudt subgroup zijn bestaande gebruikers, evenals om het even welke verenigingen met projecten, kwesties, en taken, naast al project, taak, en uitgevende statussen die tot de nieuwe oudergroep behoren.

## Groepbeheerders voor subgroepen

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

U kunt subgroepsleden als groepsbeheerders toewijzen aan de subgroep wanneer u deze maakt of bewerkt. Voor instructies, zie [&#128279;](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) in het artikel [ een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) creëren.

Afwisselend, kunt u beleid van subgroup aan de groepsbeheerders verlaten die aan de groepen boven het worden toegewezen. Wanneer u een subgroep maakt, hebben groepsbeheerders boven de groepen erboven automatisch toegang om de subgroep te beheren.

>[!NOTE]
>
>Als u een gebruiker aan een subgroep toevoegt en die gebruiker een groepsbeheerder voor een groep overal boven de subgroep is, heeft die gebruiker administratieve rechten om de subgroep te beheren, zelfs zonder als groepsbeheerder voor het worden toegewezen.

Om te leren welke acties beschikbaar voor een beheerder van Adobe Workfront die het systeem van Workfront, een groepsbeheerder beheren een top-level groep, en een groepsbeheerder die een subgroep beheren, zie [ Acties toegestaan voor verschillende types van beheerders ](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md) beheren.
