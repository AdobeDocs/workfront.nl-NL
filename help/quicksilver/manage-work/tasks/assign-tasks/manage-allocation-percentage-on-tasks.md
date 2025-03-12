---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Percentage gebruikers- of roltoewijzing beheren voor taken
description: Het percentage van de toewijzing vertegenwoordigt de hoeveelheid tijd een toegewezen middel wordt gepland om aan een taak in een dag te werken. Het is het percentage van een het werkdag (volgens het gebruikers of projectprogramma) waarbij een middel door de duur van de taak wordt toegewezen.
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 1211a441b542df49480d933d4c25b0c31ef0883d
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Het percentage gebruikers- of roltoewijzingen beheren voor taken

Het percentage van de toewijzing vertegenwoordigt de hoeveelheid tijd een toegewezen middel wordt gepland om aan een taak in een dag te werken. Het is het percentage van een het werkdag (volgens het gebruikers of projectprogramma) waarbij een middel door de duur van de taak wordt toegewezen.

>[!NOTE]
>
>Wanneer gebruikers aan het werk worden toegewezen, heeft hun beschikbaarheid volgens hun programma&#39;s invloed op de geplande en verwachte datum van taken en problemen. Voor informatie over programma&#39;s, zie [ een programma ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Nieuw: Standaard</p> 
   <p>Huidig: Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute of hoger machtigingen voor de taak</p> <p>Machtigingen bewerken om het toewijzingspercentage bij te werken in het vak Taak bewerken</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang voor de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het wijzigen van percentagetoewijzingen voor taken

* De gebruikers worden toegewezen een gelijk percentage van tijd aan taken zij worden toegewezen, door gebrek.
* U kunt het toewijzingspercentage voor gebruikers en baanrollen manueel wijzigen die aan taken slechts worden toegewezen wanneer het Type van Duur van de taak Berekend Werk of Gedreven Inspanning is.

  Voor informatie, zie [ Overzicht van het Type van Duur en van de Duur van de Taak ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* U kunt niet de percententoewijzing voor teams wijzigen die aan taken worden toegewezen.
* U kunt niet de percentaletoewijzing voor gebruikers en baanrollen wijzigen die aan kwesties worden toegewezen.

## Wijzig de gebruiker of rolpercenten toewijzing voor een taak

1. Ga naar een taak waarvoor de middelen u de percententoewijzing veranderen.
1. Klik **Meer** menu ![](assets/qs-more-icon-on-an-object.png) naast de naam van de taak, dan klik **uitgeven**.

   of

   Klik het **gebied van Taken** in de taakkopbal, dan klik **Geavanceerd**.

1. Zorg ervoor dat het **Type van Duur** van de taak één van het volgende is:

   * Berekend werk
   * Inzet gedreven

   >[!TIP]
   >
   >* Voor het Berekende Type van Duur van de Toewijzing, gebruikt Workfront de volgende formule om het toewijzingspercentage van elke toegewezen persoon te berekenen: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Voor het Eenvoudige Type van Duur, kunt u de uren schatten die aan elk middel worden toegewezen, niet het toewijzingspercentage.

1. Klik **Taken**, dan wijzigen de **Toewijzingen** voor elke taak toegewezen persoon.

   U kunt het toewijzingspercentage voor gebruikers en taakroltoewijzingen alleen wijzigen.

   U kunt niet het toewijzingspercentage voor een team wijzigen dat aan een taak wordt toegewezen.

   ![ wijzigen toewijzingspercentage ](assets/advanced-assignments-allocation-percentage.png)

1. Klik **sparen**.
