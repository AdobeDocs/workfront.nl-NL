---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Overzicht van de geplande voltooiing van de taak
description: De geplande Voltooiingsdatum van een taak is de datum waarop de taak wordt geplaatst om te voltooien.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 0%

---

# Overzicht van de geplande voltooiing van de taak

De geplande Voltooiingsdatum van een taak is de datum waarop de taak wordt geplaatst om te voltooien.

U kunt de Geplande Voltooiingsdatum van een taak specificeren, of u kunt het aan Adobe Workfront verlaten om het te berekenen afhankelijk van bepaalde criteria. 

De geplande voltooiingsdata van taken op een project bepalen de Geplande Voltooiingsdatum van een project wanneer het project van de Datum van het Begin wordt gepland. Voor meer informatie over het Geplande Project Datum van Voltooiing, zie [Geplande afsluitdatum van project instellen](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>De geplande voltooiing van een taak verschilt op de volgende manieren van de Vastlegdatum van de taak of de Verwachte Voltooiingsdatum van de taak:
>
>* De datum van de Vastlegging is de datum waardoor de persoon die aan de taak wordt toegewezen manueel schat dat zij de taak zullen voltooien. Zie de volgende artikelen voor meer informatie:
   * [Overzicht van datum vastleggen](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
   * [Interacties tussen de Vastlegdatum en de Geplande Voltooiingsdatum](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
* De voorspelde datum van voltooiing is een datum die door Workfront wordt berekend en houdt rekening met de vertraging van de taak, de tijdlijnen van de taak of de voorgangers ervan en andere factoren om een datum in real-time vast te stellen waarop de taak op realistische wijze kan worden voltooid. Zie voor meer informatie [Overzicht van de geplande afsluitdatum voor projecten, taken en problemen](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>


## De geplande voltooiingsdatum van een taak handmatig instellen

U moet over Edit toegang tot Taken en beheertoestemmingen op de taak hebben om de Geplande Datum van Voltooiing van de taak bij te werken.

Het plaatsen van de Geplande Datum van de Voltooiing van een taak hangt van het type van de Beperking van de Taak af u aan de taak toewijst. 

U kunt de Geplande Datum van de Voltooiing in de volgende gebieden van Workfront manueel plaatsen:

* Selecteer in het vak Taak bewerken wanneer u een taak maakt of bewerkt. Zie voor meer informatie [Taken bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* In het gebied van de Details van de Taak. Zie voor meer informatie [Taakgegevens beheren in het gebied Overzicht van taakdetails](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* In het gebied Home als de Geplande Datum van Voltooiing wanneer het bekijken van een taak toont. Zie voor meer informatie [Een tijdelijk onderdeel bijwerken of bewerken in het gebied Home](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* In de taakkoptekst. Zie voor meer informatie [Nieuwe objectkoppen](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* In een taaklijst of rapport wanneer het Geplande gebied van de Datum van de Voltooiing in de mening toont.

   Zie voor meer informatie [Taken in een lijst bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

U kunt de Geplande Datum van de Voltooiing manueel specificeren wanneer u om het even welke volgende Beperkingen van de Taak selecteert: 

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Type taakbeperking</strong> </p> </th> 
   <th> <p><strong>Effect van het manueel wijzigen van de Geplande VoltooiingsDatum</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Moet worden voltooid op</p> <p>Niet later voltooien dan</p> <p>Niet eerder voltooien dan</p> </td> 
   <td> <p><span class="s1">De geplande begindatum wordt aangepast om de duur gelijk te houden.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Vaste datums</p> </td> 
   <td> <p>De duur wordt aangepast om de geplande begindatum gelijk te houden.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Hoe Workfront automatisch de geplande voltooiingsdatum voor een taak berekent

Wanneer het automatisch door het systeem wordt berekend, kan het volgende de Geplande Datum van de Voltooiing van een Taak beïnvloeden:

* Taakbeperking

   Voor meer informatie over de Beperkingen van de Taak, zie het artikel [Overzicht van taakbeperking](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Taak voorgangerrelatie

   Raadpleeg het artikel voor meer informatie over voorlanders voor taken [Overzicht van voorgangers van taken](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Voltooiingsdatum van het project, wanneer het project van de Afsluitingsdatum wordt gepland.
* Het tijdschema voor de primaire ontvanger van de taak.

   Wanneer de Primaire Ontvanger tijd van gepland tijdens de duur van de taak heeft, passen de geplande data van de taak dienovereenkomstig aan wanneer **Overweeg de gebruikerstijd in taakduur** instelling is geselecteerd voor de **Gebruikerstijd uit** veld. De nieuwe projecten erven dit het plaatsen van het gebied van de Voorkeur van het Project, maar u kunt het plaatsen op het projectniveau uitgeven.

   Als bijvoorbeeld een taak met een beperking van Zo snel mogelijk op 1 juni begint en op 3 juni wordt voltooid, en de primaire ontvanger op 2 juni is gemarkeerd voor time-off, wordt de geplande afsluitende datum van de taak 4 juni.

   Voor informatie over de **Gebruikerstijd uit** voorkeuren, zie de artikelen [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) of [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

* De hoeveelheid tijd die aan goedkeuringsinstellingen is gekoppeld als de taak aan een goedkeuring is gekoppeld. Zie voor meer informatie [Algemene goedkeuringsinstellingen configureren](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

Wanneer deze optie automatisch wordt ingesteld, wordt de geplande datum van voltooiing bepaald op basis van de volgende berekening: 

```
Planned Completion Date = Planned Start Date + Duration
```

Als uw taak bijvoorbeeld een startdatum van 16 september en een duur van 10 dagen heeft, is de geplande voltooiingsdatum 26 september.

>[!NOTE]
 Het Type van Update voor het project moet aan Automatisch en bij Verandering of automatisch worden geplaatst om de Geplande Uren en Duur automatisch aan te passen.\
Raadpleeg het artikel voor meer informatie over het updatetype [Selecteer het Type van projectupdate](../../../manage-work/projects/manage-projects/select-project-update-type.md).
