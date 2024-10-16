---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Werk handmatig toewijzen met de werklastverdeling
description: Met de Adobe Workfront Workload Balancer kunt u handmatig werkitems toewijzen aan gebruikers.
author: Lisa
feature: Resource Management
role: User
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 0%

---

# Handmatig werk toewijzen met Workload Balancer

Met de Adobe Workfront Workload Balancer kunt u handmatig werkitems toewijzen aan gebruikers.

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
       <p>Huidig: Plan, wanneer het gebruiken van de Balancer van de Werkbelasting in het gebied van de Middelen;</br>
       Het werk, wanneer het gebruiken van de Balancer van de Werkbelasting van een team of een project</p></td>
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

## Handmatig werk toewijzen in Workload Balancer

U kunt werkitems toewijzen die nog niet aan een gebruiker zijn toegewezen of items die aan gebruikers in de werklastbalans zijn toegewezen, opnieuw toewijzen.

1. Ga naar Werklastverdeling waar u werk wilt toewijzen.

   U kunt werk aan gebruikers toewijzen gebruikend de Balancer van de Werkbelasting in het gebied van het Middelen, op het project, of op het teamniveau. Voor meer informatie over waar de Balancer van de Werkbelasting in Workfront wordt gevestigd, zie [ plaats van de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Facultatief) ga naar het **Niet toegewezen gebied van het Werk** en pas een filter op meningstaken of kwesties toe

   of

   Ga naar het **Toegewezen gebied van het Werk** en breid de naam van een gebruiker uit om de het werkpunten te bekijken die aan hen worden toegewezen, als u hun punten opnieuw wilt toewijzen.

1. Klik het **Meer menu** ![](assets/qs-more-menu.png) aan de linkerzijde van de naam van het het werkpunt, dan klik **toewijzen dit aan**.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >U kunt ook de volgende sneltoetsen gebruiken om taken of problemen toe te wijzen:
   >
   >* In Windows: CTRL + klik de taak of de uitgiftebar.
   >* In Mac: CMD + klik op de taak of de uitgiftebalk.

1. Voer een van de volgende handelingen uit:

   * Begin het typen van de naam van een gebruiker, baanrol, of team dat u aan het punt in het **gebied van het Onderzoek wilt toewijzen mensen, rol of teams**, het selecteren wanneer het in de lijst toont, dan **sparen** klikken.

   >[!TIP]
   >
   >Wanneer u een gebruiker toevoegt, ziet u de avatar, de primaire rol van de gebruiker en hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen.
   >
   >Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt.
   >
   > De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Voor informatie, zie [ toegang van de Verlening tot gebruikers ](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Als uw Workfront- of groepsbeheerder delegaties in uw omgeving heeft ingeschakeld, gebruikt u het tabblad Toewijzingen om gebruikers toe te wijzen aan de taak of uitgave. Gebruik het tabblad Delegaties om gebruikers weer te geven die zijn gedelegeerd aan het werkitem. Voor informatie over het delegeren van het werk, zie [ de taken en kwesties van de Afgevaardigde ](../../manage-work/delegate-work/how-to-delegate-work.md).


   Hiermee wijst u het werkitem toe aan of wijst u het toe aan de opgegeven toewijzingen.

   Als u een punt aan enkel een team of een baanrol toewijst, toont het punt slechts in het Niet toegewezen gebied van het Werk. U moet werkitems toewijzen aan gebruikers om deze weer te geven in het gedeelte Toegewezen werk van Workload Balancer.

   >[!TIP]
   >
   >U kunt meerdere gebruikers, taakrollen of teams toewijzen. U kunt alleen actieve gebruikers, taakrollen en teams toewijzen.
   >
   >
   >Als een gebruiker, een baanrol, of een team werd toegewezen alvorens zij werden gedeactiveerd, blijven zij toegewezen aan het het werkpunt. In dit geval raden we het volgende aan:
   >
   >   
   >   
   >   * Wijs het werkitem opnieuw toe aan actieve bronnen.
   >   * Koppel de gebruikers in een gedeactiveerd team aan een actief team en wijs het het werkpunt aan het actieve team opnieuw toe.
   >   
   >

   * Klik **Geavanceerd** om tot Geavanceerde Toewijzingen toegang te hebben.

     Voor meer informatie over het maken van Geavanceerde Taken, zie [ Geavanceerde taken ](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md) creëren.

1. (Facultatief) klik het **pictogram van de Toon toewijzingen** ![](assets/show-allocations-icon-small.png), dan klik het **Meer menu** ![](assets/qs-more-menu.png) > **geeft toewijzingen** uit.

   of

   Dubbelklik op een dagelijkse of wekelijkse toewijzing om de hoeveelheid tijd aan te passen die de gebruiker aan het werkitem heeft toegewezen.

   Voor informatie over het wijzigen van gebruikerstoewijzingen in de Balancer van de Werkbelasting, zie de &quot;wijzig gebruikerstoewijzingen&quot;sectie in artikel [ gebruikerstoewijzingen in de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md) beheren.

   Voor informatie over het verwijderen van taken uit een het werkpunt gebruikend de Balancer van de Werklast, zie [ werk in de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md) unassign.

    
