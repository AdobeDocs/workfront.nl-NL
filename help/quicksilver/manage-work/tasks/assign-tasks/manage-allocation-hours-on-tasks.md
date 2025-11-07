---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Uur van gebruikers- en roltoewijzing beheren voor taken
description: Wanneer het toewijzen van gebruikers of rollen aan een taak, worden zij toegewezen om een bepaald aantal uren te werken om de taak te voltooien. U kunt de hoeveelheid uren manueel wijzigen dat elke gebruiker of baanrol wordt toegewezen wanneer zij aan een taak worden toegewezen, wanneer het Type van Duur van de taak Eenvoudig is.
author: Lisa
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---

# Gebruikers- en roltoewijzingstijden beheren voor taken

<!--Audited: 10/2025-->

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->


<div class="preview">

De gemarkeerde informatie op deze pagina verwijst naar functionaliteit die nog niet algemeen beschikbaar is. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Dezelfde functies zijn ook beschikbaar in de productieomgeving voor alle klanten vanaf een week na de release Preview.

Voor meer informatie, zie [ modernisering van de Interface ](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

De uren van de toewijzing vertegenwoordigen de totale hoeveelheid tijd een toegewezen middel om aan een taak te werken wordt gepland. De uren vertegenwoordigen de tijd dat een gebruiker op één bepaalde dag of weekdag, week, of maand door de duur van de taak wordt toegewezen.

U kunt de toewijzingstijden wijzigen wanneer u geavanceerde toewijzingen voor een taak maakt.

>[!NOTE]
>
>Wanneer gebruikers aan het werk worden toegewezen, heeft hun beschikbaarheid volgens hun programma&#39;s invloed op de geplande en verwachte datum van taken en problemen. Voor informatie over programma&#39;s, zie [ een programma ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

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
   <p>Bewerk toestemmingen om toewijzingsuren in het vak Taak bewerken bij te werken wanneer u taken bewerkt <span class="preview"> met behulp van de oude ervaring. U kunt toewijzingsuren in het Edit taakvakje niet meer beheren wanneer het uitgeven van taken in de nieuwe ervaring.</span></p> <p>Voor informatie, zie <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md"> taken </a> uitgeven.</p></td>
  </tr>
 </tbody>
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Take this piece out of the table above when we remove the new experience/ after production release in the task box: 

<p>Edit permissions to update allocation hours in the Edit Task box when editing tasks using the old experience. <span class="preview">You can no longer manage allocation hours in the Edit task box when editing tasks in the new experience.</span></p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a></p>.-->


## Overwegingen bij het wijzigen van de toewijzingstijden voor een taak

>[!IMPORTANT]
>
>Nadat u handmatig de toewijzingen voor elke toewijzing voor taken hebt gewijzigd, kunnen de geplande uren van de taken dienovereenkomstig worden bijgewerkt. Voor meer informatie, zie de sectie [ Geplande taak van de Update Uren wanneer het beheren van gebruikerstoewijzingen ](../../../manage-work/tasks/task-information/planned-hours.md#update) in het artikel [ Geplande overzicht van Uren ](../../../manage-work/tasks/task-information/planned-hours.md).

* Het totaal aantal uren dat is toegewezen aan individuele bronnen die zijn toegewezen aan de taak, vertegenwoordigt de geplande uren van de taak.
* Als er één gebruiker of roltaak aan een taak is, past de hoeveelheid uren die aan de gebruiker of de rol wordt toegewezen de Geplande Uren van de taak aan.
* In het geval van veelvoudige taken, wordt elke gebruiker of baanrol toegewezen een gelijke hoeveelheid uren om aan de taak te werken, door gebrek, als het Type van Duur van de taak Eenvoudig is. Raadpleeg de volgende artikelen voor meer informatie:

   * [ Overzicht van het Type van Duur en van de Duur van de Taak ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Overzicht van het type duur: Eenvoudig](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* Wanneer de taak een Eenvoudig Type van Duur heeft, kunt u de hoeveelheid toegewezen uren voor elke gebruiker of baanrol manueel veranderen om erop te wijzen dat sommige taaktoegewezen aanwezigen meer tijd zouden kunnen hebben om aan een taak te werken dan anderen.
* U kunt de hoeveelheid uren niet wijzigen die aan teams wordt toegewezen die aan taken worden toegewezen.
* U kunt de gebruikers- of taakroltoewijzing voor uitgaven niet handmatig wijzigen.
* U kunt ook dagelijkse, wekelijkse of maandelijkse toewijzingen van gebruikers aan taken of problemen beheren met de werklastverdeler. Voor meer informatie, zie [ gebruikerstoewijzingen in de Balancer van de Werklast beheren ](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## De gebruikers- of roltoewijzingsuren voor een taak wijzigen

1. Ga naar een taak waarvoor taken u de toewijzingstijden wilt veranderen.
1. Klik het **gebied van Taken** in de taakkopbal, dan klik **Geavanceerd**.
1. Zorg ervoor dat het **Type van Duur** van de taak **Eenvoudig** is.
1. Wijzig het **gebied van Toewijzingen** voor elke taak toegewezen. Dit zijn algemene toewijzingen voor elke toewijzing aan deze taak, voor de volledige duur van de taak. Dit zou de algemene **Geplande Uren** van de taak ook kunnen bijwerken.

   ![ wijzigt toewijzingen ](assets/advanced-assignments-duration-type-allocations.png)

1. Klik **sparen**.
