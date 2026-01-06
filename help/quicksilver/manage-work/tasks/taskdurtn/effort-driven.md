---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Type duur overzicht: inspanning voortbewogen'
description: Geforceerde inspanning is een duurtype dat u voor een taak in Adobe Workfront kunt plaatsen. Voor algemene informatie over de Types van Duur in Workfront, zie Overzicht van het Type van Duur en van de Duur van de Taak.
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 0%

---

# Overzicht van het Duur Type: Door de inspanning gestuurde

Geforceerde inspanning is een duurtype dat u voor een taak in Adobe Workfront kunt plaatsen. Voor algemene informatie over de Types van Duur in Workfront, zie [ Overzicht van het Type van Duur en van de Duur van de Taak ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Overzicht van het type door de inspanning bepaalde duur

Uw Workfront of een groepsbeheerder kan het standaardtype Duur van uw systeem of groep instellen als Gedreven inspanning. In dit geval, zullen alle nieuwe taken met dit Type van Duur worden gecreeerd. Voor informatie over het veranderen van uw taak en geef voorkeur uit als deel van uw systeem-niveau of groep-vlakke projectvoorkeur uit, zie [ systeembrede taak en uitgiftevoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) vormen.

In dit scenario, is er een risico om het projectplan willekeurig te verkorten, tenzij u, als projectleider, de tijd neemt om te overwegen of de taak eigenlijk een Efort Gedreven taak is.

Gebruik de functie Gedreven inspanning om:

* Bepaal de Geplande Duur die op het aantal middelen beschikbaar wordt gebaseerd om aan de taak te werken. De duur is gelijk aan de geplande uren. De geplande duur is gelijk aan de geplande uren gedeeld door het aantal toegewezen personen.

  De omvang van de inspanning die op de taak wordt toegepast bepaalt de verdeling van arbeid en Duur.

* Traceer het totale aantal uren dat aan een taak wordt besteed wanneer de veelvoudige middelen worden toegewezen.

  Aangezien de middelen worden toegevoegd, vermindert de Geplande Duur van de taak. (Het beginsel van &quot;vele handen maakt licht werk&quot;illustreert het effect dat dit Type van Duur op de Geplande Duur van een taak heeft.)

De volgende secties verstrekken meer gedetailleerde informatie over hoe Workfront de Geplande Duur van een Geplande Taak van de Inspanning en het effect berekent dat het toevoegen van middelen aan de taak met dit Type van Duur moet.

## Overzicht van de formule Door de inspanning bepaalde duur

De formule voor berekening de Geplande Duur voor een taak met een Type van Duur van Gedreven inspanning hangt van het toewijzingspercentage van elk middel af dat aan de taak wordt toegewezen. In het geval van een door de inspanning gestuurde taak berekent Workfront de geplande uren van de taak en zijn deze altijd gelijk aan de duur van de taak:

```
Planned Hours (in hours) = Duration (in days)
```

U kunt de duur van de taak handmatig aanpassen.

Workfront gaat ervan uit dat er 8 werkuren per werkdag zijn. Uw Workfront- of groepsbeheerder bepaalt de uren per werkdag met de instelling Meestvoorkomende uren per werkdag in de projectvoorkeuren in Setup. Voor meer informatie over het veranderen van uw taak en geef voorkeur als deel van uw systeem-vlakke projectvoorkeur uit, zie [ de taak van het hele systeem vormen en geven voorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) uit.

>[!TIP]
>
>Workfront beschouwt het Programma voor elke die middel aan de taak wordt toegewezen om het percentage van toewijzing voor elke middel voor de taak te bepalen. Voor informatie over het creëren van en het toewijzen van programma&#39;s aan gebruikers, zie [ een programma ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

Overweeg de volgende scenario&#39;s:

* [ de Middelen worden toegewezen 100% aan de taak ](#resources-are-allocated-100-to-the-task)
* [De middelen worden toegewezen voor diverse percentages van tijd aan de taak](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### De middelen worden 100% toegewezen aan de taak {#resources-are-allocated-100-to-the-task}

In deze formule wordt ervan uitgegaan dat alle middelen volledig aan de taak worden toegewezen.

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

Bij deze berekening wordt ervan uitgegaan dat het aantal uren op een normale werkdag 8 is. De vergelijking omvat deze waarde zodat toont de Geplande Duur in dagen.

### De middelen worden toegewezen voor diverse percentages van tijd aan de taak {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

Omdat elke toegewezen bron een uniek toewijzingsniveau kan hebben, houdt de daadwerkelijke formule rekening met deze toewijzingswaarden:

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

Bij deze berekening wordt ervan uitgegaan dat het aantal uren op een normale werkdag 8 is. De vergelijking omvat deze waarde zodat toont de Geplande Duur in dagen.

## Het effect van het toevoegen van meer middelen aan een taak

Wanneer u toewijzingen toevoegt aan of verwijdert uit een taak met het type Duur (afhankelijk van de inspanning), veranderen Duur en Geplande uren niet. De geplande duur verandert echter wel.

In het volgende voorbeeld is de instelling voor de typische uren per werkdag ingesteld op 8 in de projectvoorkeuren in de systeeminstellingen. Aangezien de duur 3 dagen bedraagt, wordt de geplande uren ingesteld op 24 (3 dagen x 8 uur per werkdag = 24 geplande uren).

>[!NOTE]
>
>Wanneer het gebruiken van de Vaste Beperking van de Taak van Datums, blijft de Geplande Duur het zelfde wanneer u toevoegt of toevoegt toewijzingen verwijdert, en in plaats daarvan worden de Duur en Geplande Uren aangepast. Wanneer het gebruiken van om het even welke Beperking van de Taak buiten Vaste Datums, wordt de Geplande Duur aangepast.

In de volgende tabel ziet u hoe de geplande duur verandert door bronnen aan de taak toe te voegen:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong> Aantal Toegewezen Wijzen (elk 100%) </strong> </p> </th> 
   <th> <p><strong> Duur </strong> </p> </th> 
   <th> <p><strong> Geplande Uren </strong> </p> </th> 
   <th><strong> Geplande Duur </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3 dagen</p> </td> 
   <td> <p>24 uur</p> <p>(3 dagen x 8 uur per werkdag = 24 geplande uren)</p> </td> 
   <td> <p>3 dagen</p> <p>(24 geplande uren / 1 ontvanger = 3 dagen)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3 dagen</p> </td> 
   <td> <p>24 uur</p> <p>(3 dagen x 8 uur per werkdag = 24 geplande uren)</p> </td> 
   <td> <p>1,5 dagen</p> <p>(24 geplande uren / 2 Toewijzers = 12 uur, of 1,5 dagen)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3 dagen</p> </td> 
   <td> <p>24 uur</p> <p>(3 dagen x 8 uur per werkdag = 24 geplande uren)</p> </td> 
   <td> <p>1 dag</p> <p>(24 geplande uren / 3 toewijzingen = 8 uur, of 1 dag)</p> </td> 
  </tr> 
 </tbody> 
</table>

## Verander het Type van Duur van een taak in Gedreven Inspanning

Voor informatie over het veranderen van het Type van Duur van een taak, zie [ het Type van Duur van een taak ](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md) bijwerken.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Effort Driven</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong><strong>Changes</strong>.</li>
</ol>
-->
