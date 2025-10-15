---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Overzicht van de geplande voltooiingsdatum van de taak
description: De geplande voltooiingsdatum van een taak is de datum waarop de taak wordt voltooid.
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 0%

---

# Overzicht van de geplande voltooiing van de taak

De geplande voltooiingsdatum van een taak is de datum waarop de taak wordt voltooid.

U kunt de Geplande Voltooiingsdatum van een taak specificeren, of u kunt het aan Adobe Workfront verlaten om het te berekenen afhankelijk van bepaalde criteria.

De geplande voltooiingsdata van taken op een project bepalen de Geplande Voltooiingsdatum van een project wanneer het project van de Datum van het Begin wordt gepland. Voor meer informatie over het project Geplande Datum van de Voltooiing, zie [&#x200B; plaatsen het project Geplande Datum van de Voltooiing &#x200B;](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>De geplande voltooiing van een taak verschilt op de volgende manieren van de Vastlegdatum van de taak of de Verwachte Voltooiingsdatum van de taak:
>
>* De datum van de Vastlegging is de datum waardoor de persoon die aan de taak wordt toegewezen manueel schat dat zij de taak zullen voltooien. Zie de volgende artikelen voor meer informatie:
>
>   * [&#x200B; het overzicht van de Datum van het Vastleggen &#x200B;](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [&#x200B; Interacties tussen de Vastlegdatum en de Geplande Datum van de Voltooiing &#x200B;](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
>
>* De voorspelde datum van voltooiing is een datum die door Workfront wordt berekend en houdt rekening met de vertraging van de taak, de tijdlijnen van de taak of de voorgangers ervan en andere factoren om een datum in real-time vast te stellen waarop de taak op realistische wijze kan worden voltooid. Voor meer informatie, zie [&#x200B; Overzicht van de Verwachte Datum van de Voltooiing voor projecten, taken, en kwesties &#x200B;](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>

## De geplande voltooiingsdatum van een taak handmatig instellen

U moet over Edit toegang tot Taken en beheertoestemmingen op de taak hebben om de Geplande Datum van Voltooiing van de taak bij te werken.

Het plaatsen van de Geplande Datum van de Voltooiing van een taak hangt van het type van de Beperking van de Taak af u aan de taak toewijst.

U kunt de Geplande Datum van de Voltooiing in de volgende gebieden van Workfront manueel plaatsen:

* Selecteer in het vak Taak bewerken wanneer u een taak maakt of bewerkt. Voor informatie, zie [&#x200B; taken &#x200B;](../../../manage-work/tasks/manage-tasks/edit-tasks.md) uitgeven.
* In het gebied van de Details van de Taak. Voor informatie, zie [&#x200B; taakinformatie in het gebied van het Overzicht van de Details van de Taak beheren &#x200B;](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* In het gebied Home als de Geplande Datum van Voltooiing wanneer het bekijken van een taak in het Summiere paneel toont. Voor informatie, zie [&#x200B; Update of geef een het werkpunt op het gebied van het Huis &#x200B;](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md) uit.
* In de taakkoptekst. Voor informatie, zie [&#x200B; Nieuwe objecten kopballen &#x200B;](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* In een taaklijst of rapport wanneer het Geplande gebied van de Datum van de Voltooiing in de mening toont.

  Voor informatie, zie [&#x200B; taken in een lijst &#x200B;](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) uitgeven.

U kunt de Geplande Datum van de Voltooiing manueel specificeren wanneer u om het even welke volgende Beperkingen van de Taak selecteert:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong> Type van de Beperking van de Taak </strong> </p> </th> 
   <th> <p><strong> Effect van manueel het Veranderen van de Geplande Datum van de Voltooiing </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Moet worden voltooid op</p> <p>Uiterlijk op</p> <p>Niet eerder voltooien dan</p> </td> 
   <td> <p><span class="s1"> de Geplande Datum van het Begin wordt aangepast om het zelfde Duur te houden.</span> </p> </td> 
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

  Voor meer informatie over de Beperkingen van de Taak, zie het overzicht van de artikel [&#x200B; Beperking van de Taak &#x200B;](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* Taak-voorgangerrelatie

  Voor meer informatie over taakvoordecessors, zie het artikel [&#x200B; Overzicht van taakvoordecessors &#x200B;](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Voltooiingsdatum van het project, wanneer het project van de Afsluitingsdatum wordt gepland.
* Het tijdschema voor de primaire ontvanger van de taak.

  Wanneer de Primaire Ontvanger tijd van gepland tijdens de duur van de taak heeft, passen de geplande data van de taak dienovereenkomstig aan wanneer **gebruikerstijd van in taakduur** het plaatsen wordt geselecteerd voor de **Tijd van de Gebruiker van** gebied overweegt. De nieuwe projecten erven dit het plaatsen van het gebied van de Voorkeur van het Project, maar u kunt het plaatsen op het projectniveau uitgeven.

  Als bijvoorbeeld een taak met een beperking van Zo snel mogelijk op 1 juni begint en op 3 juni wordt voltooid, en de primaire ontvanger op 2 juni is gemarkeerd voor time-off, wordt de geplande afsluitende datum van de taak 4 juni.

  Voor informatie over de **Tijd van de Gebruiker van** voorkeur, zie de artikelen [&#x200B; systeem-brede projectvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen of [&#x200B; projecten &#x200B;](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

* De hoeveelheid tijd die aan goedkeuringsinstellingen is gekoppeld als de taak aan een goedkeuring is gekoppeld. Voor meer informatie, zie [&#x200B; globale goedkeuringsmontages &#x200B;](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md) vormen.

Wanneer deze optie automatisch wordt ingesteld, wordt de geplande datum van voltooiing bepaald op basis van de volgende berekening:

```
Planned Completion Date = Planned Start Date + Duration
```

Als uw taak bijvoorbeeld een startdatum van 16 september en een duur van 10 dagen heeft, is de geplande voltooiingsdatum 26 september.

>[!NOTE]
>
> Het Type van Update voor het project moet aan Automatisch en bij Verandering of automatisch worden geplaatst om de Geplande Uren en Duur automatisch aan te passen.\
>Voor meer informatie over het Type van Update, zie het artikel [&#x200B; het Type van projectupdate &#x200B;](../../../manage-work/projects/manage-projects/select-project-update-type.md) selecteren.
