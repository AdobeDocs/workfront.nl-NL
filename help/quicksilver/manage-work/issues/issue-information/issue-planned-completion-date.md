---
product-area: projects
navigation-topic: issue-information
title: Overzicht van de geplande afsluitdatum van de uitgave
description: De geplande afgiftedatum is de datum waarop de afgifte naar verwachting zal zijn voltooid.
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 0%

---

# Overzicht van de geplande afsluitdatum van de uitgave

De geplande afgiftedatum is de datum waarop de afgifte naar verwachting zal zijn voltooid.

U kunt de Geplande Voltooiingsdatum van een kwestie specificeren, of u kunt het aan Adobe Workfront verlaten om het te berekenen afhankelijk van bepaalde criteria. 

De geplande uitvoeringstermijnen hebben geen invloed op de geplande uitvoeringsdatum van het project. Alleen de geplande voltooiingsdatums van de taken zijn van invloed op de geplande uitvoeringsdatum van het project. Voor meer informatie over het project Geplande Datum van de Voltooiing, zie [ plaatsen het project Geplande Datum van de Voltooiing ](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>De geplande afsluitende datum van een uitgifte verschilt op de volgende manieren van de datum van afgifte van de uitgifte of de verwachte afsluitende datum van de uitgifte:
>
>* De Vastlegdatum is de datum waarop de persoon die aan de uitgifte is toegewezen, handmatig schat dat hij de uitgifte zal hebben voltooid. Zie de volgende artikelen voor meer informatie:
>
>   * [ het overzicht van de Datum van het Vastleggen ](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [ Interacties tussen de Vastlegdatum en de Geplande Datum van de Voltooiing ](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* De voorspelde afsluitdatum is een door Workfront berekende datum die rekening houdt met externe factoren om een datum in real-time vast te stellen waarop de uitgifte realistisch kan worden voltooid. Voor meer informatie, zie [ Overzicht van de Verwachte Datum van de Voltooiing voor projecten, taken, en kwesties ](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## Handmatig de geplande afsluitdatum van een uitgave instellen

U moet over Edit toegang tot Kwesties en Beheren toestemmingen op de kwestie hebben om de Geplande Datum van Voltooiing van de kwestie te kunnen bijwerken.

U kunt de Geplande Datum van Voltooiing van een kwestie in de volgende gebieden van Workfront manueel plaatsen:

* In het vak Uitgave bewerken of in het gebied Details van uitgave bij het maken of bewerken van een uitgave. Voor informatie, zie [ kwesties ](../../../manage-work/issues/manage-issues/edit-issues.md) uitgeven.
* In het gebied van het Huis als de Geplande Datum van de Voltooiing wanneer het bekijken van een kwestie verschijnt. Voor informatie, zie [ Update of geef een het werkpunt op het gebied van het Huis ](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md) uit.
* In de uitgiftekop. Voor informatie, zie [ Nieuwe objecten kopballen ](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* In een uitgiftenlijst of rapport wanneer het Geplande gebied van de Datum van de Voltooiing in de mening toont.

  Voor informatie, zie [ kwesties in een lijst ](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md) uitgeven.

## Hoe Workfront automatisch de geplande voltooiingsdatum voor een uitgave berekent

Wanneer Workfront automatisch de Geplande Voltooiingsdatum van een kwestie berekent, kan het volgende de datum beïnvloeden:

* Geplande begindatum

  De ingangsdatum en de geplande begindatum moeten overeenkomen met een uitgave wanneer u de uitgave voor het eerst maakt.

* De standaardduur zoals die in de sectie van de Details van de Rij van het project wordt gevormd. Voor informatie, zie [ een Rij van het Verzoek ](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.

  Als de standaardduur 0 dagen is, komt de geplande uitvoeringsdatum overeen met de geplande begindatum van de uitgave.

* Projectplanning

Wanneer deze optie automatisch wordt ingesteld, wordt de geplande datum van voltooiing bepaald op basis van de volgende berekening: 

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**Voorbeeld:** bijvoorbeeld, als uw taak een begindatum van Vrijdag, Januari 14 heeft en de StandaardDuur 5 Dagen is, is de Geplande Datum van de Voltooiing Vrijdag, Januari 21, als het Programma van het Project maandag-Vrijdag voor 8 uren per dag is.

De volgende situaties bestaan:

* Als het project geen Plan heeft, wordt het StandaardProgramma van uw systeem van Workfront in aanmerking genomen. Voor informatie, zie [ Overzicht van Programma&#39;s ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).
* Als het Programma maandag-vrijdag 9.00 tot 13.00 uur (4 uur per dag) is en de Normale uren van uw Workfront-systeem per werkdag 8 uur, is de Geplande Voltooiingsdatum 27 januari.

>[!TIP]
>
>Workfront houdt bij het berekenen van Geplande Voltooiingsdata rekening met uitzonderingen op het Plan, zoals feestdagen en weekends.

 
