---
product-area: resource-management
navigation-topic: resource-pools
title: Brongroepen maken
description: Brongroepen zijn verzamelingen gebruikers die u helpen bronnen gemakkelijker te beheren in Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: 2f5e0b8ba4ec4f32ae0457a6a901a43d03389773
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# Brongroepen maken {#create-resource-pools}

>[!CONTEXTUALHELP]
>id="wf_resource_pools"
>title="Brongroepen"
>abstract="Een pool van het Middel is een inzameling van gebruikers die tezelfdertijd voor de voltooiing van een project nodig zijn. Nadat u een middelpool creeert, kunt u het met projecten en malplaatjes associëren."

{{preview-and-fast-release-Q424}}

Brongroepen zijn verzamelingen gebruikers die u helpen bronnen gemakkelijker te beheren in Adobe Workfront. Voor meer informatie over middelpools, zie [ overzicht van de pools van het Middel ](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td><p>Nieuw: alle</p>
       <p>of</p>
       <p>Huidig: Pro of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot bronnenbeheer bewerken, inclusief toegang tot Brongroepen beheren</p> <p>Toegang tot projecten, sjablonen en gebruikers bewerken</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td>Beheren toestemmingen voor de projecten, de malplaatjes, en de gebruikers die u de Groepen van het Middel met wilt associëren</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
