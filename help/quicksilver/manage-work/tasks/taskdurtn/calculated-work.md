---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Overzicht van het type Duur: Berekend werk'''
description: Berekend werk is een Duur Type dat u voor een taak in Adobe Workfront kunt plaatsen. Voor algemene informatie over de Types van Duur in Workfront, zie Overzicht van het Type van Duur en van de Duur van de Taak.
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Overzicht van het type duur: Berekend werk

Berekend werk is een Duur Type dat u voor een taak in Adobe Workfront kunt plaatsen. Voor algemene informatie over de Types van Duur in Workfront, zie [Overzicht van het Type van Duur en van de Duur van de Taak](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Overzicht van het berekende type van de Duur van het Werk

Het Berekende Werk bepaalt de hoeveelheid inspanning (Geplande Uren) nodig voor de te voltooien taak. Wij adviseren dat u het Berekende Type van Duur van het Werk gebruikt wanneer de middelen die aan de taak worden toegewezen voor de volledige duur van de taak worden toegewezen.

Uw Workfront of een groepsbeheerder kan het standaard Duur Type van uw systeem of groep als Berekend Werk plaatsen. In dit geval, zullen alle nieuwe taken met dit Type van Duur worden gecreeerd. Voor informatie over het wijzigen van uw taak en het uitgeven voorkeur als deel van uw systeem-vlakke of groep-vlakke projectvoorkeur, zie [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Aangezien de middelen aan een taak worden toegevoegd, kan een projectmanager verwachten om de geplande inspanningsverhoging te zien. Om te illustreren, vertegenwoordigt een één-uur planningsvergadering met drie middelen drie totale vereiste uren van het werk, en een één-uurplanning vergadering met tien middelen vertegenwoordigt tien vereiste uren van werk. Hierbij wordt ervan uitgegaan dat elke bron met 100% toewijzing aan de taak wordt toegewezen.

## Herzie de formule voor het berekenen van het Vereiste Werk wanneer het gebruiken van het Berekende Type van Duur van het Werk

Wanneer u het Berekende Type van Duur van het Werk op een taak gebruikt, berekent Workfront de hoeveelheid Werk voor elke taak gebruikend de volgende twee formules. De formules verschillen afhankelijk van welk percentage van tijd elk middel aan de taak wordt toegewezen en hoeveel middelen u aan elke taak hebt toegewezen:

* Vereenvoudigde formule: Ervan uitgaande dat u één bron aan de taak hebt toegewezen en dat deze voor 100% van de beschikbare tijd aan de taak is toegewezen, wordt de waarde voor Vereiste werkzaamheden voor elke taak berekend aan de hand van de volgende formule:

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* Complexe formule: Als u elk middel met diverse toewijzingen toewijst, houdt de formule rekening met deze toewijzingen en verklaart deze variaties:

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## Herzie het effect van het toevoegen van of het verwijderen van middelen uit de taak

Wanneer het toevoegen van of het verwijderen van toegewezen aan een taak met het Berekende type van de Duur van het Werk, kan de Duur manueel worden uitgegeven. Als er toewijzingen worden toegevoegd aan of verwijderd uit de taak, veranderen de geplande uren.

In het volgende voorbeeld is de instelling voor de typische uren per werkdag 8 in de projectvoorkeuren in Setup. Elke taak heeft een Duur van 1 dag. Als het aantal toewijzingen verandert, veranderen de geplande uren op basis van het aantal toewijzingen voor een bepaalde taak:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Aantal Toewijzers (elk 100% toegewezen)</strong> </p> </th> 
   <th> <p><strong>Duur</strong> </p> </th> 
   <th> <p><strong>Geplande uren</strong> </p> </th> 
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

![](assets/calcwork-350x71.png)

## Verander het Type van Duur van een taak in Berekend Werk

Voor informatie over het veranderen van het Type van Duur van een taak, zie [Werk het Type van Duur van een taak bij](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

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
