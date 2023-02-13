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
source-wordcount: '589'
ht-degree: 0%

---

# Brongroepen maken

Brongroepen zijn verzamelingen gebruikers die u helpen bronnen gemakkelijker te beheren in Adobe Workfront. Voor meer informatie over middelpools, zie [Overzicht van bronnenpools](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

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
   <td> <p>Toegang tot bronnenbeheer bewerken, inclusief toegang tot Brongroepen beheren</p> <p>Toegang tot gebruikers, projecten en sjablonen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Beheren toestemmingen voor de projecten en de malplaatjes die u de Groepen van het Middel met wilt associëren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Een bronnenpool maken {#create-a-resource-pool}

1. Meld u aan als een gebruiker die toegang heeft tot het bewerken van bronnenpools.\
   Zie voor meer informatie [Een bronnenpool maken](#create-a-resource-pool).

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront.

1. Klikken **Bronnen**.
1. Klikken **Brongroepen** in het linkerdeelvenster.\
   ![resource_pools_tab.png](assets/resource-pools-tab-350x198.png)

1. Klikken **Nieuwe bronnenpool**.
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
      <td><p> Voeg gebruikers afzonderlijk toe aan de bronnenpool.<br>of <br>Een grote hoeveelheid gebruikers tegelijk toevoegen aan de bronnenpool. U kunt een van de volgende entiteiten toevoegen die aan gebruikers of verzamelingen gebruikers zijn gekoppeld:
        <ul>
         <li><strong>Teams</strong>: alle leden van het team worden toegevoegd aan de Groep van het Middel.</li>
         <li><strong>Groepen</strong>: alle leden van de groep worden toegevoegd aan de Groep van het Middel.</li>
         <li><strong>Rollen</strong>: alle gebruikers verbonden aan die rol worden toegevoegd aan de Pool van het Middel.</li>
         <li><strong>Bedrijven</strong>: alle gebruikers in het bedrijf worden toegevoegd aan de Groep van het Middel.</li>
        </ul><p>Tip: U kunt alleen actieve gebruikers, teams, <span>rollen,</span> of ondernemingen.</p><p>Opmerking: Als een gebruiker een lid van een groep, een team, een bedrijf wordt of met een baanrol verbonden nadat de groep, het team, het bedrijf of de baanrol aan de Pool van het Middel zijn toegevoegd, wordt het nieuwe lid niet automatisch toegevoegd aan de Pool van het Middel. <br>Als een gebruiker tot het team, de groep, het bedrijf, en de baanrol behoort u, tezelfdertijd toevoegt, wordt de gebruiker slechts eenmaal toegevoegd aan de Pool van het Middel.<br>Gebruikers die zijn gedeactiveerd nadat ze aan de bronnenpool zijn toegevoegd, worden grijs weergegeven in de lijst met gebruikers en worden gemarkeerd als gedeactiveerd.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (Optioneel) Gebruik de opdracht **Ongedaan maken** koppeling om de gebruikers te verwijderen die via een groep, team, bedrijf of taakrol zijn toegevoegd.

   >[!NOTE]
   >
   >Er is geen limiet voor het aantal gebruikers dat u in een bronnenpool kunt hebben. Nochtans, adviseren wij niet teveel gebruikers aan een Pool van het Middel toe te voegen, aangezien het Beheer van het Middel een uitdaging anders zou kunnen worden. In de lijst met gebruikers worden alleen de eerste 2000 gebruikers in de bronnenpool weergegeven. Deze gebruikers worden in alfabetische volgorde weergegeven.

   ![Resource_pools_NEW__UNDO_button_for_teams_groups_etc.png](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)

1. (Optioneel) Klik op het X-pictogram rechts van de naam van een gebruiker om een gebruiker te verwijderen. Voor meer informatie over het verwijderen van gebruikers uit een middelpool, zie [Gebruikers verwijderen uit bronnenpools](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md).
1. (Optioneel) Gebruik de opdracht **Zoeken** om een gebruiker te zoeken in de Resource Pool.
1. Klikken **Maken**.
