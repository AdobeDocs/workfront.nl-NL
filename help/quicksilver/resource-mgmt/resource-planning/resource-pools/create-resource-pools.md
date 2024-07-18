---
product-area: resource-management
navigation-topic: resource-pools
title: Brongroepen maken
description: Brongroepen zijn verzamelingen gebruikers die u helpen bronnen gemakkelijker te beheren in Adobe Workfront. Zie Overzicht van bronnenpools voor meer informatie over bronnenpools.
author: Alina
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Brongroepen maken

Brongroepen zijn verzamelingen gebruikers die u helpen bronnen gemakkelijker te beheren in Adobe Workfront. Voor meer informatie over middelpools, zie [ overzicht van de pools van het Middel ](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Pro en hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot bronnenbeheer bewerken, inclusief toegang tot Brongroepen beheren</p> <p>Toegang tot gebruikers, projecten en sjablonen bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Beheren toestemmingen voor de projecten en de malplaatjes die u de Groepen van het Middel met wilt associëren</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Een bronnenpool maken {#create-a-resource-pool}

1. Meld u aan als een gebruiker die toegang heeft tot het bewerken van bronnenpools.\
   Voor meer informatie, zie [ een Pool van het Middel ](#create-a-resource-pool) creëren.

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront.

1. Klik **Middelen**.
1. Klik **Pools van het Middel** in het linkerpaneel.\
   ![ resource_pools_tab.png ](assets/resource-pools-tab-350x198.png)

1. Klik **Nieuwe Pool van het Middel**.
1. Geef het volgende op:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Naam</strong></td>
      <td>Dit is de naam van de Bronpool.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Beschrijving</strong></td>
      <td>Dit is een korte beschrijving van deze Resource Pool. U kunt bijvoorbeeld opgeven voor welk doel het moet worden gebruikt.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Pool Leden</strong></td>
      <td><p> Voeg gebruikers afzonderlijk toe aan de bronnenpool.<br> of <br> om een grote hoeveelheid gebruikers aan de Pool van het Middel tegelijkertijd toe te voegen. U kunt een van de volgende entiteiten toevoegen die aan gebruikers of verzamelingen gebruikers zijn gekoppeld:
        <ul>
         <li><strong> Teams </strong>: alle leden van het team worden toegevoegd aan de Pool van het Middel.</li>
         <li><strong> Groepen </strong>: alle leden van de groep worden toegevoegd aan de Pool van het Middel.</li>
         <li><strong> Rollen </strong>: alle gebruikers verbonden aan die rol worden toegevoegd aan de Pool van het Middel.</li>
         <li><strong> Bedrijven </strong>: alle gebruikers in het bedrijf worden toegevoegd aan de Pool van het Middel.</li>
        </ul><p>Tip: U kunt actieve gebruikers, teams, <span> rollen, </span> of bedrijven slechts toevoegen.</p><p>Nota: Als een gebruiker een lid van een groep, een team, een bedrijf wordt of met een baanrol verbonden nadat de groep, het team, het bedrijf of de baanrol aan de Pool van het Middel zijn toegevoegd, wordt het nieuwe lid niet automatisch toegevoegd aan de Pool van het Middel. <br> als een gebruiker tot het team, de groep, het bedrijf, en de baanrol behoort u, tezelfdertijd toevoegt, wordt de gebruiker slechts eenmaal toegevoegd aan de Pool van het Middel.<br> de Gebruikers die na het zijn toegevoegd aan de Pool van het Middel worden gedeactiveerd verschijnen in de lijst van gebruikers en duidelijk als worden gedeactiveerd.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (Facultatief) gebruik **maak** verbinding ongedaan om de gebruikers te verwijderen die door een groep, een team, een bedrijf of een baanrol worden toegevoegd.

   >[!NOTE]
   >
   >Er is geen limiet voor het aantal gebruikers dat u in een bronnenpool kunt hebben. Nochtans, adviseren wij niet teveel gebruikers aan een Pool van het Middel toe te voegen, aangezien het Beheer van het Middel een uitdaging anders zou kunnen worden. In de lijst met gebruikers worden alleen de eerste 2000 gebruikers in de bronnenpool weergegeven. Deze gebruikers worden in alfabetische volgorde weergegeven.

   ![ Resource_pools_NEW__UNDO_button_for_teams_groups_etc.png ](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)

1. (Optioneel) Klik op het X-pictogram rechts van de naam van een gebruiker om een gebruiker te verwijderen. Voor meer informatie over het verwijderen van gebruikers uit een middelpool, zie [ gebruikers uit middelpools ](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md) verwijderen.
1. (Facultatief) gebruik de **optie van het Onderzoek** om een gebruiker in de Pool van het Middel te vinden.
1. Klik **creëren**.
