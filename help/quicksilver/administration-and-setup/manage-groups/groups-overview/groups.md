---
title: Overzicht van groepen
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Een Workfront-beheerder kan groepen gebruikers maken die overeenkomen met de afdelingsstructuur. Groepen zijn vergelijkbaar met maar verschillen van teams en bedrijven.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: b5e0a590d258df4510a0bb6a44b57099f32ae6b9
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Overzicht van groepen

<!-- Audited: 01/2024 -->

Een Workfront-beheerder kan groepen gebruikers maken die overeenkomen met de afdelingsstructuur. Groepen zijn vergelijkbaar met maar verschillen van teams en bedrijven.

De beheerder van Workfront verleent groepen de toegang tot de gebieden van Workfront waar zij moeten werken en communiceren. Elke groep kan dan hun informatie van Workfront zoals gebruikers, malplaatjes, en douaneformulieren, en projecten gescheiden van die van andere afdelingen houden.

Ten minste één groepsbeheerder is vereist voor elke groep. Groepbeheerders kunnen de pagina Groepen gebruiken om hun groepen op één locatie te beheren. Zie voor meer informatie [Groepbeheerders](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

U kunt maximaal 14 niveaus subgroepen maken onder één groep. Zie voor meer informatie [Overzicht subgroepen](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) en [Een subgroep maken](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Groepen gebruiken om gebruikers te organiseren

Als Workfront-beheerder of groepsbeheerder kunt u gebruikers koppelen aan groepen en subgroepen. Als u een groep openbaar maakt, kunnen gebruikers met een Standard (nieuw) of Plan (huidig) vergunning gebruikers met het associëren. Voor meer informatie over groepsbeheerders en openbare groepen, zie [Een groep maken](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Wanneer u een gebruiker creeert, adviseren wij dat u die gebruiker aan de aangewezen Groep van het Huis en andere groepen toevoegt die de gebruiker zou moeten binnen werken. Een gebruiker kan slechts één Home Group hebben, maar kan in meerdere andere groepen zijn.

Als u deel uitmaakt van een groep, heeft de gebruiker toegang tot objecten die worden gedeeld met de groep en de subgroepen. Als u bijvoorbeeld een project deelt met een groep, hebben gebruikers in de groep en de subgroepen van de groep toegang tot de groep.

>[!TIP]
>
>Als afdelingen in uw organisatie vaak samenwerken om projecten en de middelen aan die projecten te beheren, zou het niet noodzakelijk kunnen zijn om afdelingen in vele kleinere groepen te verdelen. Een paar groepen op hoog niveau kunnen het beste werken.

Een groep kan een onbeperkt aantal gebruikers hebben.

Voor meer informatie over het maken van nieuwe gebruikers raadpleegt u [Gebruikers toevoegen](../../../administration-and-setup/add-users/add-users.md).

## Groepstoegang verlenen tot objecten

Wanneer u een object deelt met een groep, hebben alle leden van die groep (inclusief leden van subgroepen) toegang tot het object. Ga voor meer informatie over delen in Workfront naar [Overzicht van het delen van machtigingen voor objecten](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Een groep koppelen aan een object

Wanneer u een van de volgende Workfront-objecten maakt of bewerkt, kunt u deze koppelen aan een groep:

* **Project**: U kunt één groep koppelen aan een project om de eigendom van het project aan te geven.

  Dit verleent niet impliciet aan elk lid van de groep rechten op het project. Om rechten op het project te hebben moeten de gebruikers het project met hen hebben gedeeld.

  Terwijl de gebruikers lid van veelvoudige groepen kunnen zijn, kan een project één enkele groep hebben verbonden aan het. Gebruikers van andere groepen kunnen nog steeds aan hetzelfde project werken als het project met hen of hun groepen is gedeeld. De groep verbonden aan het project is gewoonlijk of de groep verantwoordelijk voor de voltooiing van het project, of de groep waarvoor het project wordt geleverd.

  Voor instructies bij het associëren van een project met een groep, zie [Informatie beheren in het gebied Projectoverzicht](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio, programma of bedrijf**: Wanneer u een portfolio, programma of bedrijf maakt of bewerkt, kunt u er één groep aan toewijzen om aan te geven dat de groep eigenaar is van of verantwoordelijk is voor de groep. Met deze vereniging wordt gemaakt, kunnen de beheerders en de gebruikers gemakkelijk identificeren aan welke portefeuilles, programma&#39;s, en bedrijven hun groepen werken aan.

  Bijvoorbeeld, kan een groepsbeheerder alle portefeuilles in de organisatie een lijst maken gebruikend een lijst of een rapport en nota in de kolom van de Groep welke portefeuilles zijn of haar groep worden toegewezen.

  >[!NOTE]
  >
  >Het toewijzen van een groep aan een portfolio, programma of bedrijf met een groep betekent niet automatisch dat de informatie in die zin dat de groep toegang heeft tot de gegevens. U moet de toegang tot de gegevens handmatig delen met de groep voordat ze deze kunnen zien.

  Zie voor instructies [Een portfolio maken](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [Een programma maken](../../../manage-work/portfolios/create-and-manage-programs/create-program.md), en [Bedrijven maken en bewerken](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **Goedkeuringsproces**: U kunt een goedkeuringsproces ter beschikking stellen voor projecten, taken en kwesties die tot een bepaalde groep behoren. Zie voor meer informatie [Een goedkeuringsproces voor werkitems maken](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **Mijlpad**: U kunt gebruikers in bepaalde groepen toestaan een mijlpaden te gebruiken voor hun projecten. Zie voor meer informatie [Een milestone-pad maken](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **Lay-outsjabloon**: U kunt de beheerders van een groep toestemming geven om een Malplaatje van de Lay-out te wijzigen. Zie voor instructies [Administratieve toegang verlenen voor een lay-outsjabloon](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **Tijdbladprofiel**: U kunt de beheerders van een groep toestemming geven om een timesheet profiel te wijzigen. Zie voor meer informatie [Werkbladprofielen maken, bewerken en toewijzen](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Planningen**: U kunt de beheerders van een groep toestemming geven om een programma te wijzigen. Zie voor meer informatie [Een schema maken](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **Teams**: U kunt een groep aan een team associëren zodat de beheerders van de groepen en zijn subgroepen met die teams van het gebied van Groepen kunnen bekijken en werken. Zie voor meer informatie [Een team maken](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) of [Teaminstellingen bewerken](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **Sjabloon**: U kunt een groep toewijzen aan een projectsjabloon. Dit kan u helpen het proces van de projectverwezenlijking stroomlijnen en u helpen gemakkelijker identificeren en rapporteren over welke groepen bezitten welke projectmalplaatjes. Zie de sectie voor meer informatie [Overzicht](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) in het artikel [Projectsjablonen bewerken](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **Onlangs verwijderde en herstelde items**: U kunt de groepen weergeven en beheren die onlangs zijn verwijderd. Zie voor meer informatie [Onlangs verwijderde items van een groep weergeven en beheren](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) en [Onlangs herstelde items van een groep weergeven en beheren](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
