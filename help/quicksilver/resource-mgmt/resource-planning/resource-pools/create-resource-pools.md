---
product-area: resource-management
navigation-topic: resource-pools
title: Brongroepen maken
description: Brongroepen zijn verzamelingen gebruikers die u helpen bronnen gemakkelijker te beheren in Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: f18bf59202ba524173774a0215f4071bd6e77432
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Brongroepen maken

{{preview-and-fast-release-Q424}}

Brongroepen zijn verzamelingen gebruikers die u helpen bronnen gemakkelijker te beheren in Adobe Workfront. Voor meer informatie over middelpools, zie [ overzicht van de pools van het Middel ](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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

+++

## Een bronnenpool maken {#create-a-resource-pool}

{{step1-to-resourcing}}

1. Klik **Pools van het Middel** in het linkerpaneel.

   <span class="preview"> beeld van de Steekproef in het milieu van de Voorproef:</span>
   <span class="preview">![ Pools van het Middel ](assets/list-of-resource-pools.png)</span>

   Voorbeeldafbeelding in de productieomgeving:
   ![ Pools van het Middel ](assets/resource-pools-tab-350x198.png)

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
        </ul><p>Tip: U kunt actieve gebruikers, teams, <span> rollen, </span> of bedrijven slechts toevoegen.</p><br> u zou neer in de dialoog kunnen moeten scrollen om alle gebruikers in de Pool van het Middel te zien.
        <p>Nota: Als een gebruiker een lid van een groep, een team, een bedrijf wordt of met een baanrol verbonden nadat de groep, het team, het bedrijf of de baanrol aan de Pool van het Middel zijn toegevoegd, wordt het nieuwe lid niet automatisch toegevoegd aan de Pool van het Middel. <br> als een gebruiker tot het team, de groep, het bedrijf, en de baanrol behoort u, tezelfdertijd toevoegt, wordt de gebruiker slechts eenmaal toegevoegd aan de Pool van het Middel.<br> de Gebruikers die na het zijn toegevoegd aan de Pool van het Middel worden gedeactiveerd verschijnen in de lijst van gebruikers en duidelijk als worden gedeactiveerd.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (Facultatief) gebruik **maak** verbinding ongedaan om de gebruikers te verwijderen die door een groep, een team, een bedrijf of een baanrol worden toegevoegd.

   >[!NOTE]
   >
   >Er is geen limiet voor het aantal gebruikers dat u in een bronnenpool kunt hebben. Nochtans, adviseren wij niet teveel gebruikers aan een Pool van het Middel toe te voegen, aangezien het Beheer van het Middel een uitdaging anders zou kunnen worden. In de lijst met gebruikers worden alleen de eerste 2000 gebruikers in de bronnenpool weergegeven. Deze gebruikers worden in alfabetische volgorde weergegeven.

   <span class="preview"> beeld van de Steekproef in het milieu van de Voorproef:</span>
   <span class="preview">![ Gebruikers die aan de Pool van het Middel ](assets/users-in-resource-pool2.png)</span> worden toegevoegd

   Voorbeeldafbeelding in de productieomgeving:
   ![ Gebruikers die aan de Pool van het Middel ](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png) worden toegevoegd

1. (Optioneel) Klik op het X-pictogram rechts van de naam van een gebruiker om een gebruiker te verwijderen. Voor meer informatie over het verwijderen van gebruikers uit een middelpool, zie [ gebruikers uit middelpools ](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md) verwijderen.
1. (Facultatief) gebruik de **optie van het Onderzoek** om een gebruiker in de Pool van het Middel te vinden.
1. Klik **creëren**.
