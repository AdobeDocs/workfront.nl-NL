---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Percentage gebruikers- of roltoewijzing beheren voor taken
description: Het percentage van de toewijzing vertegenwoordigt de hoeveelheid tijd een toegewezen middel wordt gepland om aan een taak in een dag te werken. Het is het percentage van een het werkdag (volgens het gebruikers of projectprogramma) waarbij een middel door de duur van de taak wordt toegewezen.
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 798e9ee9862b34653730c07acc9c48b901b98e63
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# Het percentage gebruikers- of roltoewijzingen beheren voor taken

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->

<div class="preview">

De gemarkeerde informatie op deze pagina verwijst naar functionaliteit die nog niet algemeen beschikbaar is. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Dezelfde functies zijn ook beschikbaar in de productieomgeving voor alle klanten vanaf een week na de release Preview.

Voor meer informatie, zie [&#x200B; modernisering van de Interface &#x200B;](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>


Het percentage van de toewijzing vertegenwoordigt de hoeveelheid tijd een toegewezen middel wordt gepland om aan een taak in een dag te werken. Het is het percentage van een het werkdag (volgens het gebruikers of projectprogramma) waarbij een middel door de duur van de taak wordt toegewezen.

U kunt het toewijzingspercentage wijzigen wanneer u geavanceerde toewijzingen voor een taak uitvoert.

>[!NOTE]
>
>Wanneer gebruikers aan het werk worden toegewezen, heeft hun beschikbaarheid volgens hun programma&#39;s invloed op de geplande en verwachte datum van taken en problemen. Voor informatie over programma&#39;s, zie [&#x200B; een programma &#x200B;](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td> <p>Standard</p>
   <p>Werk of hoger</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>Toegang tot taken bewerken</td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td>
   <td><p>Contribute of hoger machtigingen voor de taak</p>
   <p>Bewerk machtigingen om het toewijzingspercentage bij te werken in het vak Taak bewerken wanneer <span class="preview"> taken bewerkt met de oude ervaring. U kunt toewijzingspercentage in het Edit taakvakje niet meer beheren wanneer het uitgeven van taken in de nieuwe ervaring.</span></p> <p>Voor informatie, zie <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md"> taken </a> uitgeven</p>.</td>
  </tr>
 </tbody>
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Take this piece out of the table above when we remove the new experience/ after production release in the task box: 

<p>Edit permissions to update allocation percentage in the Edit Task box when editing tasks using the old experience. <span class="preview">You can no longer manage allocation percentage in the Edit task box when editing tasks in the new experience.</span></p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a></p>.
-->

## Overwegingen bij het wijzigen van percentagetoewijzingen voor taken

* De gebruikers worden toegewezen een gelijk percentage van tijd aan taken zij worden toegewezen, door gebrek.
* U kunt het toewijzingspercentage voor gebruikers en baanrollen manueel wijzigen die aan taken slechts worden toegewezen wanneer het Type van Duur van de taak Berekend Werk of Gedreven Inspanning is.

  Voor informatie, zie [&#x200B; Overzicht van het Type van Duur en van de Duur van de Taak &#x200B;](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* U kunt niet de percententoewijzing voor teams wijzigen die aan taken worden toegewezen.
* U kunt niet de percentaletoewijzing voor gebruikers en baanrollen wijzigen die aan kwesties worden toegewezen.

## Wijzig de gebruiker of rolpercenten toewijzing voor een taak

1. Ga naar een taak waarvoor de middelen u de percententoewijzing veranderen.
1. Klik het **gebied van Taken** in de taakkopbal, dan klik **Geavanceerd**.

1. Zorg ervoor dat het **Type van Duur** van de taak één van het volgende is:

   * Berekend werk
   * Inzet gedreven

   >[!TIP]
   >
   >* Voor het Berekende Type van Duur van de Toewijzing, gebruikt Workfront de volgende formule om het toewijzingspercentage van elke toegewezen persoon te berekenen: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Voor het Eenvoudige Type van Duur, kunt u de uren schatten die aan elk middel worden toegewezen, niet het toewijzingspercentage.

1. Wijzig het **gebied van Toewijzingen** voor elke taak toegewezen.

   U kunt het toewijzingspercentage voor gebruikers en taakroltoewijzingen alleen wijzigen.

   U kunt niet het toewijzingspercentage voor een team wijzigen dat aan een taak wordt toegewezen.

   ![&#x200B; wijzigen toewijzingspercentage &#x200B;](assets/advanced-assignments-allocation-percentage.png)

1. Klik **sparen**.
