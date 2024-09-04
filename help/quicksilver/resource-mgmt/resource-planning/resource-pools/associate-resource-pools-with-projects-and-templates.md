---
product-area: resource-management
navigation-topic: resource-pools
title: Brongroepen koppelen aan projecten en sjablonen
description: Brongroepen zijn verzamelingen gebruikers die u helpen bij het beheren van bronnen in Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# Brongroepen koppelen aan projecten en sjablonen


<!-- drafted for bulk editing projects: keep this in yellow till this releases to ALL customers - May 1, 2023

Also - take out all the references to Preview and Prod at prod final
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->


<!--
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
-->

Brongroepen zijn verzamelingen gebruikers die u helpen bij het beheren van bronnen in Adobe Workfront.

Nadat u middelpools creeert, kunt u hen met projecten of malplaatjes associëren zodat kunt u uw middelen op de projecten later begroten.

Wij adviseren dat u uw middelgroepen vooraf creeert, hen associeert met projecten, en uw middelen begroot alvorens het project begint.

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

## Brongroepen koppelen aan één project of sjabloon

U kunt middelpools met een malplaatje op de zelfde manier associëren u middelpools met een project. Dit artikel beschrijft hoe u middelgroepen met projecten kunt associëren.

1. Ga naar een project en klik **Meer** pictogram ![](assets/more-icon.png) naast de projectnaam, dan klik **uitgeven**.

1. Klik **Montages van het Project**.

1. Begin de naam van een middelpool op het **gebied van de Pools van het Middel 0} te typen, dan het van de lijst te selecteren wanneer het verschijnt.**\
   U kunt veelvoudige middelpools met één project of malplaatje associëren.

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. Klik **sparen**.

Voor meer informatie over hoe te om een project uit te geven en het te associëren met middelpools, zie [ projecten ](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

Voor meer informatie over hoe te om een malplaatje uit te geven en het te associëren met middelpools, zie [ projectmalplaatjes ](../../../manage-work/projects/create-and-manage-templates/edit-templates.md) uitgeven.

## Brongroepen koppelen aan meerdere projecten of sjablonen in bulk

U kunt veelvoudige projecten of malplaatjes in bulk uitgeven en de zelfde middelgroepen met elk van hen tezelfdertijd associëren.

U kunt middelpools met malplaatjes op de zelfde manier associëren u middelpools met projecten.

Om middelgroepen met verscheidene projecten in bulk te associëren:

1. Ga naar een lijst met projecten.
1. Selecteer veelvoudige projecten, dan klik **uitgeven** pictogram ![](assets/edit-icon.png) bij de bovenkant van de lijst.

1. Klik **Montages**.
1. Begin de naam van een middelpool op het **gebied van de Pools van het Middel 0} te typen, dan het van de lijst te selecteren wanneer het verschijnt.**\
   U kunt veelvoudige middelgroepen met de projecten of de malplaatjes associëren.

   >[!NOTE]
   >
   >* Wanneer u malplaatjes in massa uitgeeft, slechts verschijnen de middelgroepen die voor alle geselecteerde malplaatjes gemeenschappelijk zijn op dit gebied. Als de geselecteerde sjablonen geen gedeelde bronnenpools hebben, is dit veld leeg. De middelpools u specificeert hier beschrijven de individuele middelpools van de projecten of de malplaatjes.
   >
   >* Wanneer u projecten in bulk uitgeeft, is er een &quot;Veelvoudige waarde&quot;indicator als de geselecteerde projecten verschillende middelgroepen hebben. Als u bronnenpools bulksgewijs toevoegt voor projecten, worden alle pools toegevoegd aan het geselecteerde project en worden de oorspronkelijke bronnenpools overschreven.

   ![ add_resource_pools_to_multiple_projects.png ](assets/add-resource-pools-to-multiple-projects-350x358.png)

1. Klik **sparen Veranderingen**.\
   Wanneer uw middelpools met uw projecten of uw malplaatjes worden geassocieerd, kunt u gebruikerstoewijzingen voor uw projecten binnen de Planner van het Middel begroten.\
   Voor meer informatie over de Planner van het Middel, zie [ Overzicht van de Planner van het Middel ](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Voor meer informatie over hoe te om projecten in bulk uit te geven, zie &quot;projecten in bulk&quot;sectie in [ projecten ](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

Voor meer informatie over hoe te om malplaatjes in massa uit te geven, zie de &quot;malplaatjes in bulk&quot;sectie in [ projectmalplaatjes ](../../../manage-work/projects/create-and-manage-templates/edit-templates.md) uitgeven.
