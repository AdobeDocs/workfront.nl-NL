---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Overzicht van de geplande startdatum van de taak
description: De geplande begindatum van een taak is de datum waarop u, als taakmaker, besluit dat het werk aan de taak moet worden gestart. De geplande taakdata beïnvloeden de data en de chronologie op het project. Voor informatie over het project Geplande Datum van het Begin, zie Overzicht van de geplande Datum van het Begin van het project.
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# Overzicht van de geplande startdatum van de taak

De geplande begindatum van een taak is de datum waarop u, als taakmaker, besluit dat het werk aan de taak moet worden gestart. De geplande taakdata beïnvloeden de data en de chronologie op het project. Voor informatie over de Geplande Datum van het Begin van het project, zie [Overzicht van de geplande begindatum van het project](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## De geplande begindatum van een taak

U kunt de geplande begindatum van een taak opgeven of deze aan Adobe Workfront overlaten om de taak te berekenen op basis van bepaalde criteria. 

* [De geplande begindatum van een taak handmatig instellen](#manually-set-the-planned-start-date-of-a-task)
* [Hoe de Geplande Datum van het Begin voor een taak wordt berekend](#how-the-planned-start-date-is-calculated-for-a-task)

### De geplande begindatum van een taak handmatig instellen {#manually-set-the-planned-start-date-of-a-task}

Het plaatsen van de Geplande Datum van het Begin van een taak hangt van het type van de Beperking van de Taak af u aan de taak toewijst. 

U kunt de geplande begindatum handmatig instellen wanneer u een taak maakt, zoals wordt beschreven in het artikel [Taken maken in een project](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

U kunt de Geplande Datum van het Begin manueel specificeren wanneer u om het even welke volgende Beperkingen van de Taak selecteert: 

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
   <td> <p>Moet beginnen op</p> <p>Niet eerder starten dan</p> <p>Niet later starten dan</p> </td> 
   <td> <p><span class="s1">De geplande datum van voltooiing wordt aangepast om de Duur het zelfde te houden.</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Vaste datums</p> </td> 
   <td> <p>De Duur wordt aangepast om de Geplande Datum van Voltooiing te handhaven.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Hoe de Geplande Datum van het Begin voor een taak wordt berekend {#how-the-planned-start-date-is-calculated-for-a-task}

Wanneer het automatisch door het systeem wordt berekend, kan het volgende de Geplande Datum van het Begin van een taak beïnvloeden:

* De voorkeursinstelling Begindatum in het gedeelte Taken en problemen in Setup

   Uw Workfront of groepsbeheerder kan bepalen of een nieuwe taak op de zelfde datum begint zoals de Geplande Datum van het Begin van het project of op de dag u creeert de taak.

   Voor informatie over de voorkeuren voor Taken en problemen raadpleegt u [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Taakbeperking

   Voor meer informatie over de Beperkingen van de Taak, zie het artikel [Overzicht van taakbeperking](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)

* Taak voorgangerrelatie

   Raadpleeg het artikel voor meer informatie over voorlanders voor taken [Overzicht van voorgangers van taken](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* De Datum van het Begin van het project, wanneer het project van de Datum van het Begin gepland is.
* Het tijdschema voor de primaire ontvanger van de taak.

   Wanneer de Primaire Ontvanger tijd van gepland tijdens de duur van de taak heeft, passen de geplande data van de taak dienovereenkomstig aan wanneer **Overweeg de gebruikerstijd in taakduur** instelling is geselecteerd voor de **Gebruikerstijd uit** veld. De nieuwe projecten erven dit het plaatsen van het gebied van de Voorkeur van het Project, maar u kunt het plaatsen op het projectniveau uitgeven.

   Als bijvoorbeeld een taak met een beperking van Zo snel mogelijk op 1 juni moet beginnen en op 3 juni moet worden voltooid, en de primaire ontvanger op 1 juni moet zijn gemarkeerd voor een time-off, wordt de geplande begindatum van de taak 2 juni.

   Voor informatie over de **Gebruikerstijd uit** voorkeuren, zie de artikelen  [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) of [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

Wanneer deze optie automatisch wordt ingesteld, wordt de geplande begindatum bepaald op basis van de volgende berekening: 

```
Planned Start Date = Planned Completion Date - Task Duration
```

Als uw taak bijvoorbeeld een Voltooiingsdatum van 16 september en een duur van 10 dagen heeft, is de Geplande Begindatum 6 september.

>[!NOTE]
>
> Het updatetype voor het project moet ook aan &quot;Automatisch en bij Verandering&quot;of &quot;automatisch&quot;worden geplaatst opdat de Geplande Uren en Duur automatisch worden aangepast.\
Raadpleeg het artikel voor meer informatie over het updatetype [Selecteer het Type van projectupdate](../../../manage-work/projects/manage-projects/select-project-update-type.md).
