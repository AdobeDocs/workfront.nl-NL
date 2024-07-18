---
title: Groepbeheerders
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: De beheerders van Adobe Workfront in een grote organisatie met vele afdelingen zouden niet alle afdelingen en groepen van de organisatie binnen die afdelingen kunnen willen beheren. In plaats daarvan, kunnen zij een groep voor elke afdeling en subgroepen binnen die groep tot stand brengen, elk beheerd door een groepsbeheerder.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: 850e0801511177efc5189258acd9b88234cf59c9
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 0%

---

# Groepbeheerders

<!-- Audited: 12/2023 -->

De beheerders van Adobe Workfront in een grote organisatie met vele afdelingen zouden niet alle afdelingen en groepen van de organisatie binnen die afdelingen kunnen willen beheren. In plaats daarvan, kunnen zij een groep voor elke afdeling en subgroepen binnen die groep tot stand brengen, elk geleid door een groepsbeheerder.

Een groepsbeheerder kan de behoeften van een groep beheren, zoals gebruikerslidmaatschap, lay-outsjablonen, aangepaste gegevens, statussen en voorkeuren.

Onder één groep kunnen maximaal 14 niveaus van subgroepen bestaan.

>[!NOTE]
>
>Alle groepsbeheerders in de hiërarchie boven een subgroep hebben beheerdersrechten om die subgroep te beheren.

Voor informatie over het creëren van en het leiden van groepen, zie [ een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) creëren en [ leiden een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). Ook, zie [ Overzicht Subgroups ](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Groepbeheerders toewijzen

Elke top-level groep moet minstens één groepsbeheerder hebben. Een Workfront-beheerder of beheerder van een groep kan groepsbeheerders toewijzen aan de subgroepen van de groep, maar dit is niet verplicht. Voor meer informatie, zie [ een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) creëren.

Als u een beheerder van Workfront bent, adviseren wij dat u het volgende doet alvorens gebruikers als groepsbeheerders aan te wijzen:

* Let op het huidige aantal Workfront-beheerders in uw systeem.
* Let op het aantal groepen dat u in uw systeem hebt.
* Bepaal of u het toegangsniveau van sommige beheerders van Workfront kunt veranderen en hen in plaats daarvan als groepsbeheerders aanwijzen.

  Voor meer informatie over de mogelijkheden van groepsbeheerders, zie [ Taken die door groepsbeheerders ](#tasks-done-by-group-administrators) in dit artikel worden gedaan.

* Bepaal of u groepsbeheerders als andere gebruikers wilt kunnen aanmelden, of wachtwoorden voor gebruikers in de groepen wilt terugstellen u beheert. De extra toegang is nodig om deze taken uit te voeren, zoals hieronder verklaard in [ Toegang nodig voor groepsbeheerders ](#access-needed-for-group-administrators).
* Voor een beter gebruikersbeheer kunt u groepen of subgroepen toewijzen in plaats van gebruikers aan de volgende objecten:

   * Layoutsjablonen
   * Planningen
   * Tijdbladprofielen

## Toegang vereist voor groepbeheerders {#access-needed-for-group-administrators}

Elke groepsbeheerder moet

* Een planlicentie in het huidige prijsmodel en verpakkingsmodel
* Een standaardlicentie in het nieuwe prijs- en verpakkingsmodel

We raden aan dat groepsbeheerders bewerkingstoegang tot gebruikers hebben, zodat ze de volgende taken kunnen uitvoeren:

* Meld u aan als andere gebruikers in de groepen en subgroepen die ze beheren.
* Stel het wachtwoord van een andere gebruiker in de groepen die ze beheren opnieuw in.

>[!IMPORTANT]
>
>Groepsbeheerders moeten meer toegang hebben dan degenen die ze beheren. Als dit niet het geval is, kunnen ze geen lagere toegangsniveaus weergeven of wijzigen.
>Voor instructies bij het verlenen van deze toegang, zie [ tot douanetoegangsniveaus ](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

Voor een groepsbeheerder die timesheet profielen aan gebruikers in hun groepen en subgroepen moet toewijzen, adviseren wij ook Administratieve toegang tot timesheets en uren. Voor instructies bij het verlenen van deze toegang, zie [ gebruikers administratieve toegang van de Verlening tot bepaalde gebieden ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Taken die door groepsbeheerders worden gedaan {#tasks-done-by-group-administrators}

Als groepsbeheerder kunt u de hieronder beschreven taken uitvoeren om de groepen te beheren waarop u toezicht houdt. Sommige hiervan zijn hetzelfde als de mogelijkheden die aan een Workfront-beheerder worden geboden.

>[!NOTE]
>
>In het nieuwe prijs en verpakkingsmodel, moet u een Primair plan of hoger hebben om het volgende uit te voeren:
>
> * Groepsgebeurtenismeldingen maken
> * Groepsprojectvoorkeuren configureren
> * Groepstaken en probleemvoorkeuren configureren
> * Configuratie van voorkeuren voor subgroepen ontgrendelen
> * Groeptimesheet en voorkeuren voor uren
> * Timesheet en uurvoorkeur ontgrendelen

### Groepsleden beheren {#manage-group-members}

* Subgroepen maken, bewerken en verwijderen binnen de groepen en subgroepen die u beheert. Voor instructies, zie [ een subgroep ](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md) creëren.
* Voeg om het even welke gebruikers toe voor wie u Edit toegang tot uw groepen en subgroups hebt. U kunt gebruikers ook toevoegen aan groepen en subgroepen door hun profielen te bewerken.

  U kunt de velden in het profiel van een groepslid ook bijwerken als u de machtiging Gebruikersbeheer (Groepgebruikers) hebt ingeschakeld op uw toegangsniveau.

  Voor meer informatie, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

  >[!NOTE]
  >
  >Workfront-beheerders kunnen wijzigingen in groepslidmaatschappen die door een groepsbeheerder zijn aangebracht, negeren.

* Wachtwoorden voor gebruikers opnieuw instellen die lid zijn van de groepen die u beheert. Voor meer informatie, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.
* Meld u aan als gebruikers die lid zijn van de groepen die u beheert. Voor meer informatie, zie [ Login als een andere gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* Bekijk het aantal beschikbare licenties voor uw groep en de subgroepen eronder. Voor meer informatie, zie [ beschikbare vergunningen in uw systeem ](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md) beheren.

### Groepsobjecten beheren {#manage-group-objects}

* Maak lay-outsjablonen op groepsniveau en koppel deze aan de groepen en subgroepen die u beheert. Voor meer informatie, zie [ lay-outmalplaatjes ](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) creëren en beheren.
* Creeer groep-vlakke timesheet profielen, associeer hen met gebruikers en groepen u beheert, en produceer manueel timesheets. Voor meer informatie, zie [ creeer, geef uit, en wijs timesheet profielen ](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md) toe.
* Zonder administratieve toegang tot goedkeuringsprocessen, creeer en geef goedkeuringsprocessen voor de groepen en subgroepen uit u beheert. Voor meer informatie, zie [ een goedkeuringsproces voor het werkpunten ](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) creëren.

  Voor informatie over administratieve toegang tot goedkeuringsprocessen, zie [ gebruikers administratieve toegang verlenen tot bepaalde gebieden ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Maak schema&#39;s en koppel ze aan een groep die u beheert. Voor meer informatie, zie [ een programma ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.
* Een team beheren dat is toegewezen aan een groep die u beheert, zonder lid te zijn van het team. Ook, creeer een teamrapport dat op het gebied van de Groep wordt gebaseerd om te identificeren aan welke groep een bepaald team wordt toegewezen. Voor meer informatie, zie [ een team ](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) creëren.
* Herstel een project dat met een groep wordt geassocieerd u, samen met om het even welke taken, kwesties, of documenten verbonden aan het project beheert. Voor meer informatie, zie [ geschrapte punten ](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md) herstellen.

### Groepvoorkeuren en -gereedschappen beheren {#manage-group-preferences-and-tools}

* Wanneer een projectvoorkeur, taak- of uitgiftevoorkeur of tijdbladen en uren voor groepen in het systeem worden ontgrendeld, bewerkt u die voorkeur voor groepen die u beheert. Deze voorkeuren zijn van invloed op project-, taak- en probleemgedrag. Raadpleeg de volgende bronnen voor meer informatie:

   * [ vorm projectvoorkeur voor een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [Taak- en uitgavevoorkeuren voor een groep configureren](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* Groepstatussen maken en bewerken voor groepen die u beheert. Voor meer informatie, zie [ creeer of geef een groepsstatus ](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md) uit.
* Configureer een gebeurtenismelding voor groepen die u beheert. Dit kunt u alleen doen nadat een Workfront-beheerder de mogelijkheid heeft ontgrendeld om gebeurtenismeldingen voor groepen via het systeem te configureren. Voor meer informatie, zie [ Mening en vorm gebeurtenisberichten voor een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
