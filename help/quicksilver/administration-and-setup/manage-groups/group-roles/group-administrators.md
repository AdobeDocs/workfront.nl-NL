---
title: Groepbeheerders
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: De beheerders van Adobe Workfront in een grote organisatie met vele afdelingen zouden niet alle afdelingen en groepen van de organisatie binnen die afdelingen kunnen willen beheren. In plaats daarvan, kunnen zij een groep voor elke afdeling en subgroepen binnen die groep tot stand brengen, elk geleid door een groepsbeheerder.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: 03667fbdd1b0d68b9ad2d2db4a1ed85b8136062b
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 0%

---

# Groepbeheerders

De beheerders van Adobe Workfront in een grote organisatie met vele afdelingen zouden niet alle afdelingen en groepen van de organisatie binnen die afdelingen kunnen willen beheren. In plaats daarvan, kunnen zij een groep voor elke afdeling en subgroepen binnen die groep tot stand brengen, elk geleid door een groepsbeheerder.

Een groepsbeheerder kan de behoeften van een groep beheren, zoals gebruikerslidmaatschap, lay-outmalplaatjes, douanegegevens, statussen, en voorkeur.

Tot 14 niveaus van subgroepen kunnen onder één groep bestaan.

>[!NOTE]
>
>Alle groepsbeheerders in de hiërarchie boven een subgroep hebben beheerdersrechten om die subgroep te beheren.

Voor informatie over het creëren van en het leiden van groepen, zie [Een groep maken](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) en [Een groep beheren](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). Zie ook [Overzicht subgroepen](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Groepbeheerders aanwijzen

Elke top-level groep moet minstens één groepsbeheerder hebben. Een Workfront-beheerder of beheerder van een groep kan groepsbeheerders toewijzen aan de subgroepen van de groep, maar dit is niet verplicht. Zie voor meer informatie [Een groep maken](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Als u een beheerder van Workfront bent, adviseren wij dat u het volgende doet alvorens gebruikers als groepsbeheerders aan te wijzen:

* Let op het huidige aantal Workfront-beheerders in uw systeem.
* Let op het aantal groepen dat u in uw systeem hebt.
* Bepaal of u het toegangsniveau van sommige beheerders van Workfront kunt veranderen en hen in plaats daarvan als groepsbeheerders aanwijzen.

   Voor meer informatie over de mogelijkheden van groepsbeheerders, zie [Taken die door groepsbeheerders worden gedaan](#tasks-done-by-group-administrators).

* Bepaal of u groepsbeheerders als andere gebruikers wilt kunnen aanmelden, of wachtwoorden voor gebruikers in de groepen wilt terugstellen u beheert. Er is aanvullende toegang nodig om deze taken uit te voeren, zoals in [Toegang vereist voor groepbeheerders](#access-needed-for-group-administrators).
* Voor een beter gebruikersbeheer kunt u groepen of subgroepen toewijzen in plaats van gebruikers aan de volgende objecten:

   * Lay-outsjablonen
   * Planningen
   * Tijdbladprofielen

## Toegang vereist voor groepbeheerders {#access-needed-for-group-administrators}

Elke groepsbeheerder moet een licentie voor het abonnement hebben.

Wij adviseren dat de groepsbeheerders Edit toegang tot gebruikers hebben zodat zij de volgende taken kunnen uitvoeren:

* Meld u aan als andere gebruikers in de groepen en subgroepen die ze beheren.
* Stel het wachtwoord van een andere gebruiker in de groepen die zij beheren opnieuw in.

>[!IMPORTANT]
>
>Groepsbeheerders moeten een hogere toegang hebben dan degenen die zij beheren; anders, zullen zij geen lagere toegangsniveaus kunnen bekijken of wijzigen.
>Voor instructies over het verlenen van deze toegang raadpleegt u [Aangepaste toegangsniveaus maken of wijzigen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Voor een groepsbeheerder die timesheet profielen aan gebruikers in hun groepen en subgroepen moet toewijzen, adviseren wij ook Administratieve toegang tot timesheets en uren. Voor instructies over het verlenen van deze toegang raadpleegt u [Gebruikers administratieve toegang verlenen tot bepaalde gebieden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Taken die door groepsbeheerders worden gedaan {#tasks-done-by-group-administrators}

Als groepsbeheerder, kunt u de taken uitvoeren hieronder om de groepen te beheren die u controleert. Sommige hiervan zijn hetzelfde als de mogelijkheden die aan een Workfront-beheerder worden geboden.

* [Groepsleden beheren](#manage-group-members)
* [Groepsobjecten beheren](#manage-group-objects)
* [Groepvoorkeuren en -gereedschappen beheren](#manage-group-preferences-and-tools)

### Groepsleden beheren {#manage-group-members}

* Subgroepen maken, bewerken en verwijderen binnen de groepen en subgroepen die u beheert. Zie voor instructies [Een subgroep maken](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* Voeg om het even welke gebruikers toe voor wie u Edit toegang tot uw groepen en subgroups hebt. U kunt gebruikers ook toevoegen aan groepen en subgroepen door hun profielen te bewerken.

   U kunt de velden in het profiel van een groepslid ook bijwerken als u de machtiging Gebruikersbeheer (Groepgebruikers) hebt ingeschakeld op uw toegangsniveau.

   Zie voor meer informatie [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   >[!NOTE]
   >
   >Workfront-beheerders kunnen wijzigingen in groepslidmaatschappen die door een groepsbeheerder zijn aangebracht, negeren.

* Wachtwoorden voor gebruikers opnieuw instellen die lid zijn van de groepen die u beheert. Zie voor meer informatie [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* Meld u aan als gebruikers die lid zijn van de groepen die u beheert. Zie voor meer informatie [Aanmelden als een andere gebruiker](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* Bekijk het aantal beschikbare licenties voor uw groep en de subgroepen eronder. Zie voor meer informatie [Beschikbare licenties in uw systeem beheren](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### Groepsobjecten beheren {#manage-group-objects}

* Maak lay-outsjablonen op groepsniveau en koppel deze aan de groepen en subgroepen die u beheert. Zie voor meer informatie [Lay-outsjablonen maken en beheren](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* Creeer groep-vlakke timesheet profielen, associeer hen met gebruikers en groepen u beheert, en produceer manueel timesheets. Zie voor meer informatie [Werkbladprofielen maken, bewerken en toewijzen](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* Zonder administratieve toegang tot goedkeuringsprocessen, creeer en geef goedkeuringsprocessen voor de groepen en subgroepen uit u beheert. Zie voor meer informatie [Een goedkeuringsproces voor werkitems maken](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   Voor informatie over administratieve toegang tot goedkeuringsprocessen raadpleegt u [Gebruikers administratieve toegang verlenen tot bepaalde gebieden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Creeer programma&#39;s en associeer hen met een groep u leidt. Zie voor meer informatie [Een schema maken](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* Een team beheren dat is toegewezen aan een groep die u beheert, zonder lid te zijn van het team. Ook, creeer een teamrapport dat op het gebied van de Groep wordt gebaseerd om te identificeren aan welke groep een bepaald team wordt toegewezen. Zie voor meer informatie [Een team maken](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* Herstel een project dat met een groep wordt geassocieerd u, samen met om het even welke taken, kwesties, of documenten verbonden aan het project beheert. Zie voor meer informatie [Verwijderde items herstellen](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### Groepvoorkeuren en -gereedschappen beheren {#manage-group-preferences-and-tools}

* Wanneer een projectvoorkeur, taak of uitgiftevoorkeur, of timesheets en urenvoorkeur voor groepen door het systeem wordt ontgrendeld, geef die voorkeur voor groepen uit u leidt. Deze voorkeuren zijn van invloed op project, taak en probleemgedrag. Raadpleeg de volgende secties voor meer informatie:

   * [Projectvoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [Taak- en uitgavevoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* Groepstatussen maken en bewerken voor groepen die u beheert. Zie voor meer informatie [Een groepsstatus maken of bewerken](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Configureer een gebeurtenismelding voor groepen die u beheert. Dit kunt u alleen doen nadat een Workfront-beheerder de mogelijkheid heeft ontgrendeld om gebeurtenismeldingen voor groepen via het systeem te configureren. Zie voor meer informatie [Gebeurtenismeldingen voor een groep weergeven en configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
