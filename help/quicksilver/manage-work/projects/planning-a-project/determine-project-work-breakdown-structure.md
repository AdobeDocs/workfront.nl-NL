---
product-area: projects
navigation-topic: plan-a-project
title: Structuur van werkverdeling in een project bepalen
description: Het bepalen van een Structuur van de Onderverdeling van het Werk (WBS) voor een project is een reeks activiteiten die uiteindelijk het projectplan schetst. De WBS verdeelt het resultaat van het project in beheersbare werkelementen, die kunnen worden gebruikt om mijlpalen te definiëren en werktoewijzingen te organiseren.
author: Alina
feature: Work Management
exl-id: a76c468d-6373-4dab-93ff-a0b3734f368c
source-git-commit: 7c373707f6e5ec1431e38cc0e103e25cd8cf2309
workflow-type: tm+mt
source-wordcount: '1745'
ht-degree: 0%

---

# Structuur van werkverdeling in een project bepalen

Het bepalen van een Structuur van de Onderverdeling van het Werk (WBS) voor een project is een reeks activiteiten die uiteindelijk het projectplan schetst. De WBS verdeelt het resultaat van het project in beheersbare werkelementen, die kunnen worden gebruikt om mijlpalen te definiëren en werktoewijzingen te organiseren.

U moet een vergunning van het Plan met Edit toegang tot Projecten hebben om de Structuur van de Onderverdeling van het Werk van een project te bouwen. Extra toegang tot andere gebieden van Adobe Workfront zou kunnen nodig zijn, afhankelijk van hoeveel activiteiten u terwijl de bouw van WBS uitvoert.

Wij adviseren dat u het project in een status van de Planning houdt terwijl u veranderingen in de Structuur van de Onderverdeling van het Werk aanbrengt, om berichten te vermijden om aan gebruikers op het Team van het Project teweeg te brengen.

## De te leveren projectresultaten definiëren

Het doel van een project is tastbare resultaten te leveren aan interne en externe belanghebbenden. De te leveren items van een project zijn de resultaten die u wilt bereiken door het project te voltooien. De resultaten worden bijna altijd geassocieerd met minstens één leverbaar, en alle te leveren producten zouden met een project moeten worden geassocieerd.

Projectproducten kunnen consumptiegoederen, intellectuele output (zoals rapporten) of diensten zijn. Bijvoorbeeld, als uw projectwerkingsgebied een huis moet bouwen, kunnen sommige te leveren punten omvatten:

* architectuurplannen maken
* afwerking
* elektrisch werk
* stichting
* ontwerp
* sluiting van de verkoop van de woning .

Afhankelijk van zijn grootte en werkingsgebied, kan een project uit veelvoudige te leveren punten worden samengesteld.

Nadat u de te leveren items hebt geïdentificeerd, kunt u deze in taken onderverdelen. De taken zijn de output die u bereikt om uw algemeen resultaat voor het project te leveren. Bij het definiëren van uw taken houdt u rekening met de volgende parameters:

* De tijd die nodig is om te worden voltooid.
* Begroting vereist voor de voltooiing van de werkzaamheden.
* De vereiste middelen waren nodig om het werk te voltooien.
* Het plannen van de middelen die op de logische chronologie van de taken worden gebaseerd.

Terwijl u taken definieert, moet u ervoor zorgen dat u niet teveel werk voor één individuele taak plant. Als het werk dat voor een taak wordt vereist meer dan 40 uren (een typische week van het werk) is, dan zou u die hoeveelheid werk in subtaken kunnen moeten onderbreken. De hoofdtaak wordt voltooid wanneer alle subtaken zijn voltooid.

Om WBS- resultaten en te bepalen leverables in Workfront, adviseren wij u de volgende activiteiten uit te voeren om een hiërarchische mening van projecttaken tot stand te brengen:

* Maak een nieuw project als u dat nog niet hebt gedaan.\
  Zie het artikel voor informatie over het maken van een project [Een project maken](../../../manage-work/projects/create-projects/create-project.md).

* Maak taken voor alle actiepunten die nodig zijn om elk resultaat en elke te leveren item te voltooien.\
  Zie het artikel voor informatie over het maken van taken [Taken maken in een project](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) .

* Van de taken u enkel creeerde, identificeer welke belangrijke resultaten zijn en associeer hen met mijlpalen.\
  Raadpleeg de artikelen voor informatie over het maken van mijlpaaltaken [Een milestone-pad maken](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) en [Mijlpalen koppelen aan taken](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

* Verdeel de taken met te groot een werkingsgebied in subtaken. Koppel ze aan het bovenliggende element dat uw te leveren item definieert.\
  Zie het artikel voor informatie over het maken van subtaken [Subtaken maken](../../../manage-work/tasks/create-tasks/create-subtasks.md).

* Identificeer afhankelijkheidsrelaties tussen subtaken en tussen mijlpalen.\
  In een afhankelijkheidsrelatie is het begin van een taak afhankelijk van de voltooiing van een andere taak of groep taken.\
  Zie de artikelen voor informatie over taakafhankelijkheden [Overzicht van voorgangers van taken](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) en [Een voorganger-relatie maken in de takenlijst](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

* Bepaal of op enig punt in de levensduur van het project goedkeuringen en beoordelingen nodig zijn. Goedkeuringsprocedures maken om aan deze behoefte te voldoen.\
  Raadpleeg het artikel voor informatie over goedkeuringen [Een goedkeuringsproces voor werkitems maken](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Schatting van de werkschema&#39;s en planningsbeperkingen

Zodra u de basismijlpaal en taakstructuur van het project creeert, kunt u schatten de tijd het zal vergen om het algemene project te voltooien door taakbeperkingen en duur te bepalen.

Overweeg het volgende:

* De beperkingen van de taak bepalen wanneer het werk aan een taak moet beginnen of beëindigen.

  Zie het artikel voor informatie over het definiëren van taakbeperkingen [Overzicht van taakbeperking](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* De duur van een taak is het beschikbare tijdkader om een taak te voltooien. Bij het schatten van Duur, kunt u een waarde willen ingaan die met de mogelijkheid van een vertraging rekening houdt. Als soortgelijke projecten in het verleden zijn voltooid, hebt u wellicht een goed idee waar u deze waarde wilt instellen.

  Aangezien de duur een schatting is, moet u optimistische tijdwaarden instellen om rekening te houden met factoren die de taak kunnen beïnvloeden, zoals weer, stroomuitval, problemen met leveranciers of andere onvoorziene gebeurtenissen. Bovendien ben zeker om te overwegen of er om het even welke bijbehorende voorganger of afhankelijkheidstaken zijn en hoe zij beperkingen op het werk kunnen plaatsen en taakvoltooiing kunnen beïnvloeden.

  Afhankelijk van het Type van Duur van de taak, kunt u de duur van een taak tijdens het leven van een project wijzigen, maar dit zal ook de chronologie van het project beïnvloeden. Raadpleeg het artikel voor informatie over de duur van een taak [Overzicht van het Type van Duur en van de Duur van de Taak](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) .

## Taken toewijzen

Nadat u de duur en de beperkingen van elke taak hebt bepaald, kunt u bepalen wie de tijd en de vaardigheden heeft om het werk te verwezenlijken. U kunt taken toewijzen aan de volgende entiteiten in Workfront:

* Gebruikers\
  Alleen gebruikers met een Planner- of Worker-toegangsniveau kunnen aan taken worden toegewezen. Hoewel u taken kunt toewijzen aan aanvragers en revisoren, kunnen ze deze niet voltooien. Daarom raden wij u niet aan deze taken toe te wijzen.

  Voor informatie over de toegangsniveaus en hoe ze definiëren wat gebruikers met Workfront-objecten kunnen doen, raadpleegt u [Overzicht van toegangsniveaus](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

* Taken rollen
* Teams

Raadpleeg de artikelen in het dialoogvenster [Taken toewijzen](../../../manage-work/tasks/assign-tasks/assign-tasks-1.md) sectie.

## Bronnen beheren

Het Beheer van het middel in Workfront staat u toe om te bepalen of er voldoende personeel is om het project te voltooien. Wanneer de gebruikers aan een project worden toegevoegd, toont Workfront het gebruik van elke gebruiker. De Managers van het middel kunnen het totale aantal uren zien de persoon aan andere projecten tijdens het tijdkader van het project wordt toegewezen.

>[!NOTE]
>
>Zolang het project een status van Planning heeft, verschijnen de taken die aan gebruikers worden toegewezen niet in hun taaklijsten.

In het begin van een belastingjaar of een kwartaal, kunt u uw middelen op een hoger niveau, over veelvoudige projecten, zonder de kennis van een specifieke Structuur van de Onderverdeling van het Werk willen beheren.\
Raadpleeg het artikel voor informatie over het plannen van het gebruik van uw bronnen op een hoger niveau [Aan de slag met bronnenplanning](../../../resource-mgmt/resource-planning/get-started-resource-planning.md).

Wanneer u uw middelen in de context van de bouw van de Structuur van de Onderverdeling van het Werk van één project beheert, en ervoor zorgt dat elke taak aan het correcte middel wordt toegewezen, bent u bereid om uw middelen voor het werk te plannen dat moet worden gedaan.\
Raadpleeg de artikelen in het dialoogvenster [De werklastbalans](../../../resource-mgmt/workload-balancer/workload-balancer.md) sectie.

## Projectfinanciën schatten

Workfront zal de geplande kosten voor elke taak en de totale kosten voor een project berekenen. De geplande kosten voor een taak omvatten alle uitgaven van de taak plus de kosten van de werknemer of de rol die aan de taak wordt toegewezen. Uurtarieven voor de taak, de rol, en de werknemer worden toegewezen tijdens taak, rol, en gebruikersverwezenlijking.

Zie de sectie over de financiering van projecten voor meer informatie [Projectfinanciën](../../../manage-work/projects/project-finances/project-finances-overview.md) .

## Goedkeuringspunten voor het project bepalen

Door goedkeuringsprocessen in Workfront te maken, kunt u controlepunten voor het project instellen om de voortgang en mogelijke probleemgebieden te controleren. Door het goedkeuringsproces kunnen de Eigenaars van het Project ontdekken welke taken te laat en vroegtijdig zijn, controletrails bekijken die een lijst maken van die een taakstatus veranderden, en geschiedenissen van kwesties zien, met inbegrip van hoe de kwesties werden opgelost en toen zij werden gesloten. Bij het herzien van een project, kunnen de Eigenaars van het Project bepalen welke stappen om het projectplan te nemen en bij te werken, indien nodig.

Raadpleeg het artikel voor informatie over goedkeuringen [Een goedkeuringsproces voor werkitems maken](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

## WBS bekijken

Om WBS van een project te begrijpen, wilt u de volgende taakelementen bekijken:

* Taakvolgorde en tijdlijn (geplande begin- en einddatum en taakduur)
* Afhankelijkheden van voorgaande
* Kind- en ouderrelatie
* Toewijzingen

Zodra u uw WBS voltooit, kunt u het in een taaklijst op het projectniveau of in een rapport bekijken.

* [WBS in een takenlijst weergeven](#view-the-wbs-in-a-task-list)
* [WBS in een taakrapport weergeven](#view-the-wbs-in-a-task-report)

### WBS in een takenlijst weergeven {#view-the-wbs-in-a-task-list}

U kunt de taaklijst op projectniveau bekijken.

1. Ga naar het project waarvoor u de Structuur van de Onderverdeling van het Werk wilt zien.
1. Selecteer **Taken** tab.
1. (Optioneel) Selecteer **Niets** in de **Groepering** vervolgkeuzemenu.

   De structuur van de Onderverdeling van het Werk toont niet de inspringing van de taken in WBS.

1. Van de **Weergave** en selecteert u de **Werkverdeling** weergeven.

   De structuur Werkverdeling wordt weergegeven in de tweede kolom van de geselecteerde weergave.

   ![De Structuur van de Onderverdeling van het werk in een taaklijst](assets/work-breakdown-structure.png)

### WBS in een taakrapport weergeven {#view-the-wbs-in-a-task-report}

U kunt een taakrapport bouwen en WBS van de taken tonen door één van het volgende te doen:

* Pas de bestaande mening van de Structuur van de Onderverdeling van het Werk op het rapport toe.
* Voeg de kolom Structuur van de Onderverdeling van het Werk aan om het even welk douanerapport toe.

>[!TIP]
>
>Wij adviseren toevoegend een groepering van het Project, om duidelijkheid aan toe te voegen aan welke projecten de taken tot behoren. De inspringing van de taken wordt niet weergegeven in een taakrapport.

Zie het artikel voor informatie over het samenstellen van rapporten [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Sparen WBS van een Project als Malplaatje

Als u aan andere projecten werkt die werkprogramma&#39;s gelijkend op WBS volgen u enkel creeerde, kunt u het project als malplaatje willen bewaren. Een sjabloon bespaart tijd en moeite bij het maken van toekomstige gerelateerde projecten.

Als uw organisatie weinig omzet heeft, denk na wachtend tot na gebruikerstaken worden gemaakt om het malplaatje te bewaren. Ongeacht wanneer een project als malplaatje wordt bewaard, kunnen de gebruikerstaken of specifieke taken tijdens het vastmaken van het malplaatje aan een nieuw project worden verwijderd.

De volgende elementen van een Structuur van de Onderverdeling van het Werk kunnen in een malplaatje, voor toekomstig gebruik met een ander project worden bewaard:

* Afhankelijkheden van eerdere versies
* Toewijzingen (inclusief projecteigenaar, sponsor en beheer van bronnen)
* Goedkeuringsprocessen
* Taakbeperkingen
* Documenten
* Uitgaven en andere financiële informatie
* Doelen
* Uurtypen
* Wachtrijstructuur aanvragen
* Herinneringsmeldingen
* Risico&#39;s
* Factureringstarieven
* Informatie delen
* Aangepaste Forms

Voor informatie over het bewaren van projecten als malplaatjes, zie het artikel [Sjabloon maken van project](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md) .
