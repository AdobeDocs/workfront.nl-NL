---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Uur van gebruikers- en roltoewijzing beheren voor taken
description: Wanneer het toewijzen van gebruikers of rollen aan een taak, worden zij toegewezen om een bepaald aantal uren te werken om de taak te voltooien. U kunt de hoeveelheid uren manueel wijzigen dat elke gebruiker of baanrol wordt toegewezen wanneer zij aan een taak worden toegewezen, wanneer het Type van Duur van de taak Eenvoudig is.
author: Lisa
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: 6ded38ef130fbcdde8d680f77f6db38fbd81efb4
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Gebruikers- en roltoewijzingstijden beheren voor taken

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 
-->

De uren van de toewijzing vertegenwoordigen de totale hoeveelheid tijd een toegewezen middel om aan een taak te werken wordt gepland. De uren vertegenwoordigen de tijd dat een gebruiker op één bepaalde dag of weekdag, week, of maand door de duur van de taak wordt toegewezen.

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
   <p>Machtigingen bewerken om de toewijzingstijden bij te werken in het vak Taak bewerken</p></td>
  </tr>
 </tbody>
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Change this sentence in the table:
<p>Edit permissions to update allocation hours in the Edit Task box</p>
To this:
<p>Edit permissions to update allocation hours in the Edit Task box in the Production environment. <span class="preview">You can no longer manage allocation hours in the Edit task box in the Preview environment.</span></p>
-->

## Overwegingen bij het wijzigen van de toewijzingstijden voor een taak

>[!IMPORTANT]
>
>Nadat u handmatig de toewijzingen voor elke toewijzing voor taken hebt gewijzigd, kunnen de geplande uren van de taken dienovereenkomstig worden bijgewerkt. Voor meer informatie, zie de sectie [&#x200B; Geplande taak van de Update Uren wanneer het beheren van gebruikerstoewijzingen &#x200B;](../../../manage-work/tasks/task-information/planned-hours.md#update) in het artikel [&#x200B; Geplande overzicht van Uren &#x200B;](../../../manage-work/tasks/task-information/planned-hours.md).

* Het totaal aantal uren dat is toegewezen aan individuele bronnen die zijn toegewezen aan de taak, vertegenwoordigt de geplande uren van de taak.
* Als er één gebruiker of roltaak aan een taak is, past de hoeveelheid uren die aan de gebruiker of de rol wordt toegewezen de Geplande Uren van de taak aan.
* In het geval van veelvoudige taken, wordt elke gebruiker of baanrol toegewezen een gelijke hoeveelheid uren om aan de taak te werken, door gebrek, als het Type van Duur van de taak Eenvoudig is. Raadpleeg de volgende artikelen voor meer informatie:

   * [&#x200B; Overzicht van het Type van Duur en van de Duur van de Taak &#x200B;](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Overzicht van het type duur: Eenvoudig](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* Wanneer de taak een Eenvoudig Type van Duur heeft, kunt u de hoeveelheid toegewezen uren voor elke gebruiker of baanrol manueel veranderen om erop te wijzen dat sommige taaktoegewezen aanwezigen meer tijd zouden kunnen hebben om aan een taak te werken dan anderen.
* U kunt de hoeveelheid uren niet wijzigen die aan teams wordt toegewezen die aan taken worden toegewezen.
* U kunt de gebruikers- of taakroltoewijzing voor uitgaven niet handmatig wijzigen.
* U kunt ook dagelijkse, wekelijkse of maandelijkse toewijzingen van gebruikers aan taken of problemen beheren met de werklastverdeler. Voor meer informatie, zie [&#x200B; gebruikerstoewijzingen in de Balancer van de Werklast beheren &#x200B;](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## De gebruikers- of roltoewijzingsuren voor een taak wijzigen

1. Ga naar een taak waarvoor taken u de toewijzingstijden wilt veranderen.
1. Klik **Meer** menu ![](assets/qs-more-icon-on-an-object.png) naast de naam van de taak, dan klik **uitgeven**, dan **Taken**.

   of

   Klik het **gebied van Taken** in de taakkopbal, dan klik **Geavanceerd**.

1. Zorg ervoor dat het **Type van Duur** van de taak **Eenvoudig** is.
1. Wijzig **Verdelingen** voor elke taak toegewezen. Dit zijn algemene toewijzingen voor elke toewijzing aan deze taak, voor de volledige duur van de taak. Hierdoor kunnen ook de algemene geplande uren van de taak worden bijgewerkt.

   ![&#x200B; wijzigt toewijzingen &#x200B;](assets/advanced-assignments-duration-type-allocations.png)

1. Klik **sparen**.
