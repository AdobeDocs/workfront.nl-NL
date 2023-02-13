---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: Overzicht van het Type van Duur en van de Duur van de Taak
description: De taakduur is het verschil tussen de Geplande Datum van Voltooiing en de Geplande Datum van het Begin van de taak. De Duur wijst op het tijdkader dat voor de taak beschikbaar is om te worden voltooid.
author: Alina
feature: Work Management
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1383'
ht-degree: 0%

---

# Overzicht van het Type van Duur en van de Duur van de Taak

De taakduur is het verschil tussen de Geplande Datum van Voltooiing en de Geplande Datum van het Begin van de taak. De Duur wijst op het tijdkader dat voor de taak beschikbaar is om te worden voltooid.

Het Type van Duur van een taak identificeert het verband tussen het aantal middelen die aan een taak, de totale inspanning, en de totale Duur van de taak worden toegewezen.

## Overzicht van taakduur

>[!NOTE]
>
>Wanneer rekening houdend met de tijd van de Primaire Ontvanger op een project, zouden de geplande data van de taak kunnen aanpassen, maar de Duur van de taak blijft het zelfde. Voor informatie over het in aanmerking nemen van de tijd van de Primaire Ontvanger wanneer het plannen van een project, zie  [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Als de Ware Datum van het Begin en van de Werkelijke Voltooiing van de taak buiten het programma van het project, primaire toegewezen, of StandaardProgramma vallen, is de taakDuur nul.

**Voorbeeld:** Als u een programma hebt dat bij 9:00 AM begint en bij 12:00 PM beëindigt en een taak die om bij 2:00 PM en eind bij 4:00 PM gepland is te beginnen, is de Duur van de taak nul.

Hieronder vindt u twee scenario&#39;s voor het berekenen van de duur in Adobe Workfront.

* Als de taak aan een gebruiker wordt toegewezen gebruikt Workfront één van de volgende programma&#39;s, in deze nauwkeurige orde om Duur te berekenen:

   1. Workfront houdt rekening met de planning van de gebruiker.
   1. Als de gebruiker niet met een programma wordt geassocieerd, houdt Workfront rekening met het programma van het project.
   1. Als het project niet aan een programma wordt geassocieerd, houdt Workfront rekening met het Standaard Programma van uw systeem. Voor informatie over programma&#39;s, zie [Een schema maken](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Als de taak aan meerdere gebruikers wordt toegewezen:

   Workfront houdt rekening met het projectschema of met dat van de primaire ontvanger.

   Uw Workfront-beheerder bepaalt welk schema Workfront gebruikt wanneer een taak aan meerdere gebruikers wordt toegewezen. Zie voor meer informatie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   De stappen zijn gelijkaardig aan het eerste scenario na begrip welk programma Workfront gebruikt om Duur te berekenen.

## Eenheden van tijd voor de Duur van de Taak

U kunt de duur van de taak aangeven in zowel de normale tijd als de verstreken tijd tussen de geplande begin- en de geplande voltooiingsdatum.

Wanneer u de duur van taken in een lijst bijwerkt, kunt u de volgende afkortingen gebruiken om de tijdeenheden in Workfront aan te geven:

| Tijdseenheid | Afkorting |
|---|---|
| Minuten | M |
| Uren | H |
| Dagen. Dit is de standaardinstelling. | D |
| Weken | W |
| Maanden | T |
| Verstreken minuten | EM |
| Verstreken uren | EH |
| Verstreken dagen | ED |
| Verstreken weken | EW |
| Verstreken maanden | ET |

{style=&quot;table-layout:auto&quot;}

**Voorbeeld:** Als u wilt erop wijzen dat de Duur van een taak 3 Verstreken Dag is, zou u &quot;3 ED&quot;op het gebied van de Duur in een taaklijst typen.  U kunt de aangewezen optie voor de Eenheid van de Duur van Tijd van het beschikbare drop-down menu ook selecteren wanneer het uitgeven van een taak of in de sectie van de Details van de Taak. Voor informatie over het bewerken van taken raadpleegt u [Taken bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

Denk aan het volgende wanneer u de duur van een taak opgeeft:

* De verstreken tijd is een eenheid van tijd voor de Duur van een taak. Dit is de tijd tussen de Geplande Datum van het Begin en de Geplande Datum van de Voltooiing van een taak die vakantie, weekends, en onderbreking omvat. Met andere woorden, de verstreken tijd is de doorloop van kalenderdagen.
* De regelmatige tijd houdt rekening met vakantie, weekends, en onderbreking en sluit hen van de Duur van de taak uit.

* Wanneer u op de Duur van een taak in weken wijst, berekent Workfront de Duur in dagen en uren gebaseerd op de Typische het werkdagen per week en Typische uren per de montages van de het werkdag die door uw beheerder van Workfront in het gebied van de Voorkeur van het Project van Opstelling worden geplaatst.
* Workfront gebruikt de standaardduur van 4 weken gedurende één maand bij het berekenen van de Duur in maanden.

## Overzicht van het type taakduur

Het beheren van het Type van Duur van een taak laat u toe om verenigbare middeltaken te plaatsen die op de behoeften van de taak worden gebaseerd.

Met het type Duur kunt u de volgende vragen beantwoorden:

* Hoe druk gaan we het hebben?
* Hoe groot is de baan?
* Hoe lang duurt het nog?

![duration_type_triangle.png](assets/duration-type-triangle-350x245.png)

## Definieer duurtypen

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row">Duur </th> 
   <th scope="col"> <p><strong>-functie</strong> </p> </th> 
   <th scope="col"> <p><strong>De invloed van bronnen hierop</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>Berekende toewijzing</strong> </p> </th> 
   <td scope="col"> <p>Berekent het toewijzingspercentage voor elke toegewezen persoon op een taak. </p> <p>Wanneer u dit Type van Duur kiest, kunt u individuele Duur en Geplande Uren voor de taak invoeren. Workfront deelt de geplande uren door het aantal uren binnen de Duur van de taak, dan door het aantal middelen die aan de taak worden toegewezen om de toewijzing voor elke toegewezen persoon te berekenen.</p> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">Overzicht van het type duur: Berekende toewijzing</a>.</p> </td> 
   <td scope="col">De duur en de Geplande Uren veranderen niet wanneer het toevoegen van of het verwijderen van toegewezen aan de taak. </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Berekend werk</strong> </p> </th> 
   <td scope="col"> <p>Bepaalt de Geplande Uren (hoeveelheid inspanning) die voor de te voltooien taak wordt vereist.</p> <p>Normaal gebruikt wanneer de middelen die aan de taak worden toegewezen voor de volledige Duur van de taak worden toegewezen.</p> <p>Wanneer u dit Type van Duur kiest, hebt u de capaciteit om een individuele Duur voor de taak in te voeren. Workfront berekent de Geplande Uren voor de taak door het aantal dagen in de Duur met het aantal werkuren in het programma en met het aantal wijzers aan de taak te vermenigvuldigen. </p> <p>U kunt het toewijzingspercentage van elke toegewezen persoon handmatig wijzigen in de taak, waardoor de hoeveelheid geplande uren wordt verkort.</p> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">Overzicht van het type duur: Berekend werk</a>.</p> </td> 
   <td scope="col"> <p>De geplande Uren stijgen wanneer de wijzers aan de taak worden toegevoegd. </p> <p>Geplande uren nemen af wanneer er toewijzingen uit de taak worden verwijderd.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p>Inzet gedreven</p> </th> 
   <td scope="col"> <p>Hiermee bepaalt u de geplande uren op basis van het aantal bronnen.</p> <p>Wanneer u dit Type van Duur kiest, hebt u de capaciteit om een individuele Duur voor de taak in te voeren. Workfront berekent de Geplande Uren voor de taak door het aantal dagen in de Duur met het aantal werkuren in het programma te vermenigvuldigen en dat te delen door het aantal wijzers aan de taak. </p> <p>U kunt het toewijzingspercentage van elke toegewezen persoon voor de taak handmatig wijzigen, maar het aantal geplande uren blijft ongewijzigd.</p> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">Overzicht van het type duur: Inzet gedreven</a>.</p> </td> 
   <td scope="col"> <p>De geplande uren stijgen wanneer de wijzers van de taak worden verwijderd.</p> <p>Geplande uren nemen af wanneer er toewijzingen aan de taak worden toegevoegd. </p> <p>De Duur verandert niet, ongeacht veranderingen in het aantal aangewezen personen of hun programma. </p> <p>De duur is gelijk aan de geplande uren. De geplande duur is gelijk aan de geplande uren gedeeld door het aantal toegewezen personen.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Eenvoudig</strong> </p> </th> 
   <td scope="col"> <p>Bepaalt de Geplande Uren en de Duur (die het zelfde, voor dit Type van Duur) zijn gebaseerd op het aantal uren elke toegewezen persoon voor. </p> <p>Workfront berekent de geplande uren door de geplande toegewezen uren voor elke ontvanger op te tellen. </p> <p>U kunt de hoeveelheid uren waarvoor elke toegewezen persoon is toegewezen handmatig wijzigen en het aantal geplande uren en de hoeveelheid tijdsduur worden dienovereenkomstig aangepast. Als u een totaal aantal toegewezen uren kiest voor alle toegewezen personen, wordt dat aantal gelijkelijk over elke toegewezen persoon verdeeld.</p> <p>Zie voor meer informatie <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">Overzicht van het type duur: Eenvoudig</a>.</p> </td> 
   <td scope="col"> <p>De uren worden gelijkmatig verdeeld over toegewezen uren als u een totaal aantal toegewezen uren kiest. Nochtans, als projectmanager, kunt u de uren voor elke toegewezen persoon manueel aanpassen. </p> <p>U kunt Geplande uren en Duur van een taak met het Eenvoudige Type van Duur inline of op het taakniveau uitgeven. </p> <p>Als een nieuw team aan een taak wordt toegewezen, wordt het Type van Duur automatisch geplaatst aan Eenvoudig en kan niet worden veranderd. De taakduur voor een flexibel team moet langer zijn dan 0 minuten.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Het type Duur van nieuwe taken

Het type van Duur van een nieuwe taak past het Type van Duur aan opstelling in uw systeem aan. Het standaardtype van Duur is Berekende Toewijzing. Uw beheerder van Workfront of een groepsbeheerder kan het Type van standaardDuur voor uw systeem of voor de groep bijwerken verbonden aan het project. Zie voor meer informatie [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Het type duur van een taak wijzigen

Voor informatie over het veranderen van het Type van Duur van een taak, zie [Werk het Type van Duur van een taak bij](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).
