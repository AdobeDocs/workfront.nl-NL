---
title: Groepsoverzicht
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Een Workfront-beheerder kan groepen gebruikers maken die overeenkomen met de afdelingsstructuur. Groepen zijn vergelijkbaar met maar verschillen van teams en bedrijven.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Overzicht van groepen

<!-- Audited: 01/2024 -->

Een Workfront-beheerder kan groepen gebruikers maken die overeenkomen met de afdelingsstructuur. Groepen zijn vergelijkbaar met maar verschillen van teams en bedrijven.

De beheerder van Workfront verleent groepen de toegang tot de gebieden van Workfront waar zij moeten werken en communiceren. Elke groep kan dan hun informatie van Workfront zoals gebruikers, malplaatjes, en douaneformulieren, en projecten gescheiden van die van andere afdelingen houden.

Ten minste één groepsbeheerder is vereist voor elke groep. Groepbeheerders kunnen de pagina Groepen gebruiken om hun groepen op één locatie te beheren. Voor meer informatie, zie [&#x200B; de beheerders van de Groep &#x200B;](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

U kunt maximaal 14 niveaus subgroepen maken onder één groep. Voor meer informatie, zie [&#x200B; Subgroups overzicht &#x200B;](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) en [&#x200B; een subgroep &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md) creëren.

## Groepen gebruiken om gebruikers te organiseren

Als Workfront-beheerder of groepsbeheerder kunt u gebruikers koppelen aan groepen en subgroepen. Als u een groep openbaar maakt, kunnen gebruikers met een Standard (nieuw) of Plan (huidig) vergunning gebruikers met het associëren. Voor meer informatie over groepsbeheerders en openbare groepen, zie [&#x200B; een groep &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) creëren.

Wanneer u een gebruiker creeert, adviseren wij dat u die gebruiker aan de aangewezen Groep van het Huis en andere groepen toevoegt die de gebruiker zou moeten binnen werken. Een gebruiker kan slechts één Home Group hebben, maar kan in meerdere andere groepen zijn.

Als u deel uitmaakt van een groep, heeft de gebruiker toegang tot objecten die worden gedeeld met de groep en de subgroepen. Als u bijvoorbeeld een project deelt met een groep, hebben gebruikers in de groep en de subgroepen van de groep toegang tot de groep.

>[!TIP]
>
>Als afdelingen in uw organisatie vaak samenwerken om projecten en de middelen aan die projecten te beheren, zou het niet noodzakelijk kunnen zijn om afdelingen in vele kleinere groepen te verdelen. Een paar groepen op hoog niveau kunnen het beste werken.

Een groep kan een onbeperkt aantal gebruikers hebben.

Voor meer informatie over het creëren van nieuwe gebruikers, zie [&#x200B; gebruikers &#x200B;](../../../administration-and-setup/add-users/add-users.md) toevoegen.

## Groepstoegang verlenen tot objecten

Wanneer u een object deelt met een groep, hebben alle leden van die groep (inclusief leden van subgroepen) toegang tot het object. Voor meer informatie over het delen in Workfront, zie [&#x200B; Overzicht van het delen van toestemmingen op voorwerpen &#x200B;](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Een groep koppelen aan een object

Wanneer u een van de volgende Workfront-objecten maakt of bewerkt, kunt u deze koppelen aan een groep:

* **Project**: U kunt één enkele groep met een project associëren om op eigendom van het project te wijzen.

  Dit verleent niet impliciet aan elk lid van de groep rechten op het project. Om rechten op het project te hebben moeten de gebruikers het project met hen hebben gedeeld.

  Terwijl de gebruikers lid van veelvoudige groepen kunnen zijn, kan een project één enkele groep hebben verbonden aan het. Gebruikers van andere groepen kunnen nog steeds aan hetzelfde project werken als het project met hen of hun groepen is gedeeld. De groep verbonden aan het project is gewoonlijk of de groep verantwoordelijk voor de voltooiing van het project, of de groep waarvoor het project wordt geleverd.

  Voor instructies bij het associëren van een project met een groep, zie [&#x200B; informatie in het gebied van het projectoverzicht &#x200B;](../../../manage-work/projects/manage-projects/understand-project-overview-area.md) leiden.

* **Portfolio, programma, of bedrijf**: Wanneer u creeert of een portefeuille, een programma, of een bedrijf uitgeeft, kunt u één enkele groep aan het toewijzen om erop te wijzen dat de groep bezit of verantwoordelijkheid voor het heeft. Met deze vereniging wordt gemaakt, kunnen de beheerders en de gebruikers gemakkelijk identificeren aan welke portefeuilles, programma&#39;s, en bedrijven hun groepen werken aan.

  Bijvoorbeeld, kan een groepsbeheerder alle portefeuilles in de organisatie een lijst maken gebruikend een lijst of een rapport en nota in de kolom van de Groep welke portefeuilles zijn of haar groep worden toegewezen.

  >[!NOTE]
  >
  >Het toewijzen van een groep aan een portfolio, programma of bedrijf met een groep betekent niet automatisch dat de informatie in die zin dat de groep toegang heeft tot de gegevens. U moet de toegang tot de gegevens handmatig delen met de groep voordat ze deze kunnen zien.

  Voor instructies, zie [&#x200B; tot een portefeuille &#x200B;](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md) leiden, [&#x200B; tot een programma &#x200B;](../../../manage-work/portfolios/create-and-manage-programs/create-program.md), en [&#x200B; creeer en geef bedrijven &#x200B;](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md) uit.

* **Proces van de Goedkeuring**: U kunt een goedkeuringsproces ter beschikking stellen voor projecten, taken, en kwesties die tot een bepaalde groep behoren. Voor meer informatie, zie [&#x200B; een goedkeuringsproces voor het werkpunten &#x200B;](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) creëren.
* **Weg van de Mijlpaal**: U kunt gebruikers in bepaalde groepen toestaan om een milestone weg met hun projecten te gebruiken. Voor meer informatie, zie [&#x200B; een milestone weg &#x200B;](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) creëren.
* **Malplaatje van de Lay-out**: U kunt de beheerderstoestemming van een groep geven om een Malplaatje van de Lay-out te wijzigen. Voor instructies, zie [&#x200B; administratieve toegang van de Verlening voor een lay-outmalplaatje &#x200B;](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **Profiel van de Tijdopnemer**: U kunt de beheerderstoestemming van een groep geven om een timesheet profiel te wijzigen. Voor meer informatie, zie [&#x200B; creeer, geef uit, en wijs timesheet profielen &#x200B;](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md) toe.

* **Programma&#39;s**: U kunt de beheerderstoestemming van een groep geven om een programma te wijzigen. Voor meer informatie, zie [&#x200B; een programma &#x200B;](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.
* **Teams**: U kunt een groep met een team associëren zodat de beheerders van de groepen en zijn subgroups met die teams van het gebied van Groepen kunnen bekijken en werken. Voor meer informatie, zie [&#x200B; een team &#x200B;](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) creëren of [&#x200B; teammontages &#x200B;](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md) uitgeven.
* **Malplaatje**: U kunt een groep aan een projectmalplaatje toewijzen. Dit kan u helpen het proces van de projectverwezenlijking stroomlijnen en u helpen gemakkelijker identificeren en rapporteren over welke groepen bezitten welke projectmalplaatjes. Voor meer informatie, zie het sectie [&#x200B; Overzicht &#x200B;](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) in het artikel [&#x200B; projectmalplaatjes &#x200B;](../../../manage-work/projects/create-and-manage-templates/edit-templates.md) uitgeven.

* **onlangs schrapte en herstelde punten**: U kunt de groepen onlangs geschrapte punten bekijken en beheren. Voor meer informatie, zie [&#x200B; Mening en beheer onlangs geschrapte punten van een groep &#x200B;](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) en [&#x200B; Mening en beheer onlangs herstelde punten van een groep &#x200B;](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
