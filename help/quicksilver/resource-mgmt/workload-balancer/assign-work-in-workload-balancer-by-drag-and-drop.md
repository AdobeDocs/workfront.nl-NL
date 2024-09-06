---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Werk toewijzen in de werklastverdeler door slepen en neerzetten
description: U kunt werkitems toewijzen met de Adobe Workfront Workload Balancer door werkitems naar de juiste gebruikers te slepen en neer te zetten.
author: Lisa
feature: Resource Management
exl-id: caffcde8-3953-44a4-b945-76f2de84f4c6
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 0%

---

# Werk toewijzen in Workload Balancer door slepen en neerzetten

U kunt werkitems toewijzen met de Adobe Workfront Workload Balancer door werkitems naar de juiste gebruikers te slepen en neer te zetten.

Voor algemene informatie over het toewijzen van het werk aan gebruikers die de Balancer van de Werklast gebruiken, zie [ Overzicht van het toewijzen van het werk in de Balancer van de Werklast ](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan, om het werk in de Balancer van de Werkbelasting op het gebied van de Middelen toe te wijzen;</br>
       Het werk, om het werk in de Balancer van de Werkbelasting van een team of een project toe te wijzen</p></td>
  </tr>
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot het volgende bewerken:</p> 
    <ul> 
     <li>Bronbeheer</li> 
     <li>Projecten</li> 
     <li>Taken</li> 
     <li>Problemen</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>Contribute-machtigingen of hoger voor de projecten, taken en problemen die Toewijzingen maken bevatten</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een item toewijzen door het te slepen en neer te zetten

U kunt een item uit het gebied Niet toegewezen werk toewijzen aan een gebruiker of u kunt een reeds toegewezen item opnieuw toewijzen aan een andere gebruiker in het gebied Toegewezen werk.

1. Ga naar Werklastverdeling waar u werk wilt toewijzen.

   U kunt werk aan gebruikers toewijzen gebruikend de Balancer van de Werkbelasting in het gebied van het Middelen, op het project, of op het teamniveau. Voor meer informatie over waar de Balancer van de Werkbelasting in Workfront wordt gevestigd, zie [ plaats van de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Facultatief) ga naar het **Niet toegewezen gebied van het Werk** en pas een filter op meningstaken en kwesties toe die niet aan gebruikers worden toegewezen

   of

   Ga naar het **Toegewezen gebied van het Werk** en breid de naam van een gebruiker uit om de het werkpunten te bekijken die aan hen worden toegewezen, als u hun punten opnieuw wilt toewijzen.

1. (Voorwaardelijk) in de Balancer van de Werklast van een project, klik **toon alle gebruikers** pictogram ![](assets/show-all-users-icon-project-workload-balancer.png) om alle gebruikers van Workfront te tonen.

   Alle gebruikers die toegang hebben tot de weergave worden dan weergegeven.

   De gebruikers die ook deel uitmaken van het projectteam en reeds aan punten op het project worden toegewezen hebben het projectpictogram rechts van hun naam in het Toegewezen gebied van het Werk.

   ![](assets/user-on-the-project-indicator-highlighted-project-workload-balancer.png)


   >[!TIP]
   >
   >* De optie Alle gebruikers weergeven is alleen beschikbaar in Workload Balancer van een project.
   >* Gebruik filters om alleen de gebruikers weer te geven die voor u van belang zijn. Gebruik bijvoorbeeld een filter om alleen gebruikers van uw teams of groepen weer te geven.



1. Klik de bar van een het werkpunt dat of op de geplande of geprojecteerde chronologie wijst en het over de naam van een gebruiker in het **Toegewezen** gebied sleept.

   De gebruiker waarop u de muisaanwijzer plaatst om het werkitem naar te zetten, wordt gemarkeerd.

   >[!TIP]
   >
   >De Geplande Uren voor de gebruiker u over update in echt - tijd met het aantal dagelijkse Geplande Uren van het het werkpunt beweegt, om erop te wijzen wat het effect van het toevoegen van een nieuw punt aan hun algemene toewijzing zou kunnen zijn.

   ![](assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png)

1. Als u klaar bent, zet u het geselecteerde werkitem neer op dezelfde regel als de naam van de gebruiker in het Toegewezen gebied. Het punt wordt toegewezen en de toegewezen Geplande Uren worden bijgewerkt voor de gebruiker met de nieuwe uren van het het werkpunt.

   Als het punt aan een baanrol werd toegewezen die de gebruiker niet kan vervullen, toont het punt onder de naam van de gebruiker in het Toegewezen gebied van het Werk en het blijft ook in het Niet toegewezen gebied van het Werk om erop te wijzen dat de baanrol verbonden aan het nog niet door een gebruiker is vervangen.

   >[!TIP]
   >
   >* Als u Groep door Project op het gebied van Montages toeliet, toont de toegewezen taak onder het overeenkomstige project. Als de instelling is uitgeschakeld, wordt de toegewezen taak weergegeven in het gebruikersgebied.
   >
   >
   >     Het item wordt weergegeven volgens de criteria voor werklastbalans voor het sorteren van werkitems. Voor meer informatie, zie [ de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) navigeren.
   >
   >
   >* Als u toeliet toon alle gebruikers in de Balancer van de Werkbelasting van een project en toewees punten aan gebruikers die niet eerder aan punten op het project werden toegewezen, worden de gebruikers toegevoegd aan het Team van het Project. Voor meer informatie, zie [ projectteam ](../../manage-work/projects/planning-a-project/manage-project-team.md) leiden.


1. (Optioneel) Klik op de balk van een tijdelijk item onder de naam van een gebruiker in het gebied Toegewezen werk en sleep het item vervolgens over het gebied Niet toegewezen werk om de toewijzing ongedaan te maken. Het punt is unassigned van de gebruiker, maar het zou nog aan een baanrol kunnen worden toegewezen waarin het in het Unassigned gebied van het Werk toont. Als het punt aan een andere gebruiker wordt toegewezen, blijft het in het Toegewezen gebied van het Werk onder de naam van de gebruiker die nog wordt toegewezen.
1. (Facultatief) klik het **pictogram van de Toon toewijzingen** ![](assets/show-allocations-icon-small.png), dan klik het **Meer menu** ![](assets/qs-more-menu.png) > **geeft toewijzingen** uit.

   <!--
   (make sure these are still called this, and that the icon has not changed)
   -->
   of

   Dubbelklik op een dagelijkse of wekelijkse toewijzing om de hoeveelheid tijd aan te passen die de gebruiker aan het werkitem heeft toegewezen.

   Voor informatie over het wijzigen van gebruikerstoewijzingen in de Balancer van de Werkbelasting, zie de &quot;wijzig gebruikerstoewijzingen&quot;sectie in artikel [ gebruikerstoewijzingen in de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md) beheren.

   Voor informatie over het verwijderen van taken uit een het werkpunt gebruikend de Balancer van de Werklast, zie [ werk in de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md) unassign.

