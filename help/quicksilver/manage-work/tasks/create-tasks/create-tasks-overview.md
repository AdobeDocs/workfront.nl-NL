---
product-area: projects
navigation-topic: create-tasks
title: Overzicht van taken maken
description: U kunt taken in een project slechts tot stand brengen nadat u het project creeerde.
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# Overzicht van taken maken

U kunt taken in een project slechts tot stand brengen nadat u het project creeerde.

Bijvoorbeeld, na het creëren van een project, zou u taken kunnen willen toevoegen en hen wijzigen om het projectplan te organiseren. Voor meer informatie over het creëren van een project, zie [&#x200B; een project &#x200B;](../../../manage-work/projects/create-projects/create-project.md) creëren. Voor informatie over het creëren van taken, zie [&#x200B; taken in een project &#x200B;](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) creëren.

In dit artikel worden overwegingen, beperkingen en standaardinstellingen beschreven die van toepassing zijn bij het maken van taken.

## Manieren om taken voor een project te maken

U kunt taken op een project op de volgende manieren tot stand brengen:

* Van kras, zoals die in [&#x200B; wordt beschreven creeer taken in een project &#x200B;](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).
* De taken van het exemplaar aan het zelfde project of aan een nieuw project of dubbele taken op het zelfde project, zoals die in [&#x200B; worden beschreven Exemplaar en dubbele taken &#x200B;](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* De taken van de beweging van een project aan een andere, zoals die in [&#x200B; worden beschreven de taken van de Beweging &#x200B;](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Beperkingen bij het maken van taken

Wanneer u de correcte toegang en de toestemmingen hebt kunt u taken op een project tot stand brengen. Het volgende is echter het geval wanneer u geen taken kunt maken:

* Uw Adobe Workfront-beheerder of een groepsbeheerder moet het toevoegen van taken aan een project in de status Voltooid of Dode inschakelen in het gedeelte Projectvoorkeuren. Voor informatie over het plaatsen van projectvoorkeur, zie [&#x200B; systeem-brede projectvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.
* U kunt geen taken aan een project toevoegen dat in Hangende Goedkeuring is.

## Het maximumaantal taken dat voor een project is toegestaan

Een project kan tot 5.000 taken bevatten. Er verschijnt een waarschuwingsbericht over het project wanneer u de limiet hebt bereikt, wanneer u de limiet hebt overschreden en wanneer u probeert de limiet te overschrijden.

Afhankelijk van het aantal taken in uw projecten toen deze beperking werd opgelegd, zou uw instantie van Workfront voor meer dan 5.000 taken in één enkel project kunnen toestaan.

Als u meer dan 5.000 taken in één enkel project kunt omvatten, ben zich van het volgende bewust:

* De taaklimiet voor uw Workfront-omgeving is ingesteld op het huidige aantal taken in uw grootste project plus nog eens 10%.

  Als een project in uw Workfront-instantie bijvoorbeeld 10.000 taken bevat, is uw limiet voor elk project in uw Workfront-instantie 11.000 taken.

* Kleinere projecten verbeteren de prestaties en minimaliseren de beheersuitdagingen die grote projecten begeleiden.

## De gebreken van de taak wanneer het toevoegen van taken aan een project

Er zijn twee typen standaardgegevens die Workfront automatisch bijwerkt voor taken wanneer u deze maakt:

* Standaardinformatie op systeemniveau

  Uw beheerder van Workfront of een groepsbeheerder vestigt de systeem-vlakke gebreken voor taken op het gebied van Taken &amp; van Kwesties van de Voorkeur van het Project. Voor informatie over taak en kwestie voorkeur, zie [&#x200B; de taak van het hele systeem vormen en voorkeur van de kwestie &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) of [&#x200B; vormt taak en geeft voorkeur voor een groep &#x200B;](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) uit.

* Standaardinformatie op projectniveau

  De rest van deze sectie beschrijft de project-vlakke gebreken u, als projectmanager, voor alle nieuwe taken kan bepalen die aan een project worden toegevoegd

Wanneer u een taak aan een project toevoegt, afhankelijk van hoe het project opstelling is, zou Workfront automatisch een goedkeuringsproces of douaneformulieren aan de taak kunnen vastmaken.

Voor informatie over het vormen van een project om deze door gebrek toe te voegen, zie de &quot;sectie van Taken&quot;in [&#x200B; projecten &#x200B;](../../../manage-work/projects/manage-projects/edit-projects.md) artikel uitgeven.

Wanneer het bepalen van standaardinformatie die met taken moet worden geassocieerd die aan een project op het projectniveau worden toegevoegd, overweeg het volgende:

* U moet over beheermachtigingen voor het project beschikken om de standaardinstellingen voor het goedkeuringsproces voor taken en aangepaste formulieren te definiëren.
* Alle nieuwe taken worden gemaakt met het goedkeuringsproces en de aangepaste formulieren die worden gedefinieerd tijdens het bewerken van het project.
* U kunt deze standaardinstellingen wijzigen wanneer u taken toevoegt via het vak Taak bewerken, maar niet wanneer u taken toevoegt in inline bewerken.
* U kunt het goedkeuringsproces en de douaneformulieren voor taken in een malplaatje bepalen.

   * Wanneer een project van dit malplaatje wordt gecreeerd, worden het goedkeuringsproces en de douaneformulieren automatisch toegepast op het project.
   * Wanneer een malplaatje aan een bestaand project in bijlage is, bewaart het project het originele proces van de taakgoedkeuring en de montages van douaneformulieren als zij worden bepaald. Als zij niet worden bepaald, worden de montages van het malplaatje de montages voor het project.
   * Wanneer een malplaatje aan een bestaand project in bijlage is, behouden de taken die aan het project van het malplaatje worden toegevoegd het goedkeuringsproces en de montages van douaneformulieren die zij op het malplaatje hadden, ongeacht de taakmontages op het project.

  Voor informatie over het vastmaken van een malplaatje aan een project, zie [&#x200B; een malplaatje aan een project &#x200B;](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md) vastmaken.

* Wanneer u het project kopieert, brengen de taak standaardmontages naar het nieuwe project over.

  Voor informatie over het kopiëren van een project, zie [&#x200B; een project &#x200B;](../../../manage-work/projects/manage-projects/copy-project.md) kopiëren.

* Wanneer u taken van één project aan een ander kopieert en het bestemmingsproject verschillende standaardmontages voor taken heeft, behouden de gekopieerde taken de standaardmontages van het originele project, tenzij zij in het het kopiëren proces worden ontruimd.
* Wanneer u een taak dupliceert voor hetzelfde project, worden de aangepaste formulieren en het goedkeuringsproces overgebracht naar de dubbele taak.

  Voor informatie over het kopiëren en het dupliceren van taken, zie [&#x200B; Kopiëren en dupliceren taken &#x200B;](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

* Wanneer u de taak naar een ander project verplaatst, worden de standaardtaakmontages bewaard op de taken van het originele project, ongeacht de taak standaardmontages op het nieuwe project.

  Voor informatie over het bewegen van taken, zie [&#x200B; de taken van de Beweging &#x200B;](../../../manage-work/tasks/manage-tasks/move-tasks.md).
