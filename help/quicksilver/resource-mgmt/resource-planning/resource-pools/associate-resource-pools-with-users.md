---
product-area: resource-management
navigation-topic: resource-pools
title: Bronnenpools koppelen aan gebruikers
description: U moet een bronnenpool maken voordat u deze aan gebruikers kunt koppelen. U kunt gebruikers aan middelpools associëren wanneer u uw middelpools creeert.
author: Lisa
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Brongroepen koppelen aan gebruikers

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

Brongroepen zijn verzamelingen gebruikers die u helpen bij het beheren van bronnen in Adobe Workfront.

U moet een bronnenpool maken voordat u deze aan gebruikers kunt koppelen.

U kunt gebruikers aan middelpools associëren wanneer u uw middelpools creeert.

Als u bronnenpools maakt zonder deze te vullen met gebruikers, kunt u deze later koppelen aan gebruikers terwijl u nieuwe gebruikers bewerkt of maakt.

Voor informatie over middelpools, zie [ overzicht van de pools van het Middel ](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Voor informatie over het creëren van middelpools, zie [ middelpools ](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md) creëren.

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

## Brongroepen koppelen aan één gebruiker

{{step-1-to-users}}

1. Controleer de doos naast de naam van een gebruiker van de lijst, dan klik **uitgeven**.
1. Klik **Planning van het Middel**.
1. Begin de naam van een middelpool te typen die u met de gebruiker in het **gebied van de Pools van 0} Middel wilt associëren {, dan het van de lijst selecteren, wanneer het verschijnt.**\
   U kunt meerdere bronnenpools aan één gebruiker koppelen.\
   ![ add_resource_pool_to_user.png ](assets/add-resource-pool-to-user-350x307.png)

1. Klik **sparen Veranderingen**.

Voor meer informatie over het uitgeven van gebruikers, zie [ het profiel van een gebruiker ](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

Voor meer informatie over het creëren van nieuwe gebruikers, zie [ gebruikers ](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md) toevoegen.

## Brongroepen koppelen aan gebruikers in bulk

U kunt meerdere gebruikers bulksgewijs bewerken en dezelfde bronnenpools aan alle gebruikers tegelijk koppelen.

Brongroepen koppelen aan meerdere gebruikers in bulk:

{{step-1-to-users}}

1. Selecteer verscheidene gebruikers op de lijst, en klik **uitgeven**.
1. Klik **Planning van het Middel**.
1. Begin de naam van een middelpool te typen die u met de gebruikers in het **gebied van de Pools van 0} Middel wilt associëren {, dan het van de lijst selecteren, wanneer het verschijnt.**\
   U kunt meerdere bronnenpools koppelen aan meerdere gebruikers.

   >[!NOTE]
   >
   >Alleen de bronnenpools die alle geselecteerde gebruikers gemeen hebben, worden in dit veld weergegeven. Als de geselecteerde gebruikers geen gedeelde bronnenpools hebben, is dit veld leeg. Als dit veld leeg is, overschrijven de hier opgegeven bronnenpools hun afzonderlijke bronnenpools.

1. Klik **sparen Veranderingen**.

Voor meer informatie over hoe te om gebruikers in bulk uit te geven, zie [ gebruikersprofielen in bulk ](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md) uitgeven.
