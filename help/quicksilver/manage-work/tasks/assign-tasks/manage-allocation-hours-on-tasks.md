---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Gebruikers- en roltoewijzingstijden beheren voor taken
description: Wanneer het toewijzen van gebruikers of rollen aan een taak, worden zij toegewezen om een bepaald aantal uren te werken om de taak te voltooien. U kunt de hoeveelheid uren manueel wijzigen dat elke gebruiker of baanrol wordt toegewezen wanneer zij aan een taak worden toegewezen, wanneer het Type van Duur van de taak Eenvoudig is.
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: 830ad0411084844ace1e1e543c3ebefcb558af80
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---

# Gebruikers- en roltoewijzingstijden beheren voor taken

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuw: Standaard </p>
   <p>Huidig: Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot taken bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute- of hogere machtigingen voor de taak</p> <p>Machtigingen bewerken om de toewijzingstijden bij te werken in het vak Taak bewerken</p> </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
1. Klik **Meer** menu ![](assets/qs-more-icon-on-an-object.png) naast de naam van de taak, dan klik **uitgeven**, dan **Taken**.

   of

   Klik het **gebied van Taken** in de taakkopbal, dan klik **Geavanceerd**.

1. Zorg ervoor dat het **Type van Duur** van de taak **Eenvoudig** is.
1. Wijzig **Verdelingen** voor elke taak toegewezen. Dit zijn algemene toewijzingen voor elke toewijzing aan deze taak, voor de volledige duur van de taak. Hierdoor kunnen ook de algemene geplande uren van de taak worden bijgewerkt.

   ![ wijzigt toewijzingen ](assets/advanced-assignments-duration-type-allocations.png)

1. Klik **sparen**.
