---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Overzicht duur: berekend werk'
description: Berekend werk is een Duur Type dat u voor een taak in Adobe Workfront kunt plaatsen. Voor algemene informatie over de Types van Duur in Workfront, zie Overzicht van het Type van Duur en van de Duur van de Taak.
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 0%

---

# Overzicht duur: berekend werk

Berekend werk is een Duur Type dat u voor een taak in Adobe Workfront kunt plaatsen. Voor algemene informatie over de Types van Duur in Workfront, zie [ Overzicht van het Type van Duur en van de Duur van de Taak ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Overzicht van het berekende type van de Duur van het Werk

Het Berekende Werk bepaalt de hoeveelheid inspanning (Geplande Uren) nodig voor de te voltooien taak. Wij adviseren dat u het Berekende Type van Duur van het Werk gebruikt wanneer de middelen die aan de taak worden toegewezen voor de volledige duur van de taak worden toegewezen.

Uw Workfront of een groepsbeheerder kan het standaard Duur Type van uw systeem of groep als Berekend Werk plaatsen. In dit geval, zullen alle nieuwe taken met dit Type van Duur worden gecreeerd. Voor informatie over het veranderen van uw taak en geef voorkeur uit als deel van uw systeem-niveau of groep-vlakke projectvoorkeur uit, zie [ systeembrede taak en uitgiftevoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) vormen.

Aangezien de middelen aan een taak worden toegevoegd, kan een projectmanager verwachten om de geplande inspanningsverhoging te zien. Om te illustreren, vertegenwoordigt een één-uur planningsvergadering met drie middelen drie totale vereiste uren van het werk, en een één-uurplanning vergadering met tien middelen vertegenwoordigt tien vereiste uren van werk. Hierbij wordt ervan uitgegaan dat elke bron met 100% toewijzing aan de taak wordt toegewezen.

## Herzie de formule voor het berekenen van het Vereiste Werk wanneer het gebruiken van het Berekende Type van Duur van het Werk

Wanneer u het Berekende Type van Duur van het Werk op een taak gebruikt, berekent Workfront de hoeveelheid Werk voor elke taak gebruikend de volgende twee formules. De formules verschillen afhankelijk van welk percentage van tijd elk middel aan de taak wordt toegewezen en hoeveel middelen u aan elke taak hebt toegewezen:

* Vereenvoudigde formule: Ervan uitgaande dat u één middel aan de taak hebt toegewezen en zij aan de taak voor 100% van hun beschikbare tijd worden toegewezen, wordt de Vereiste waarde van het Werk voor elke taak berekend gebruikend de volgende formule:

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* Complexe formule: als u elke bron met verschillende toewijzingen toewijst, wordt met deze toewijzingen rekening gehouden en worden deze variaties verwerkt:

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## Herzie het effect van het toevoegen van of het verwijderen van middelen uit de taak

Wanneer u toewijzingen toevoegt of verwijdert aan een taak met het type Berekende werkduur, kan Duur handmatig worden bewerkt. Als er toewijzingen worden toegevoegd aan of verwijderd uit de taak, veranderen de geplande uren.

In het volgende voorbeeld is de instelling voor de typische uren per werkdag 8 in de projectvoorkeuren in Setup. Elke taak heeft een Duur van 1 dag. Als het aantal toewijzingen verandert, veranderen de geplande uren op basis van het aantal toewijzingen voor een bepaalde taak:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong> Aantal Toegewezen Wijzen (elk 100%) </strong> </p> </th> 
   <th> <p><strong> Duur </strong> </p> </th> 
   <th> <p><strong> Geplande Uren </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>1</p> </td> 
   <td> <p>1 dag</p> </td> 
   <td> <p>8 uur</p> <p>(1 dag x 8 uur per werkdag x 1 ontvanger = 8 geplande uren)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>2</p> </td> 
   <td> <p>1 dag</p> </td> 
   <td> <p>16 uur</p> <p>(1 dag x 8 uur per werkdag x 2 toewijzingen = 16 geplande uren)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1 dag</p> </td> 
   <td> <p>24 uur</p> <p>(1 dag x 8 uur per werkdag x 3 toewijzingen = 24 geplande uren)</p> </td> 
  </tr> 
 </tbody> 
</table>

In dit geval wordt elke toegewezen persoon voor 100% toegewezen aan de taak Berekend werk.

![ Berekend type van de werkduur ](assets/calcwork-350x71.png)

## Verander het Type van Duur van een taak in Berekend Werk

Voor informatie over het veranderen van het Type van Duur van een taak, zie [ het Type van Duur van een taak ](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md) bijwerken.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Work</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
