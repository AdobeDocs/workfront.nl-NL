---
product-area: resource-management
navigation-topic: resource-pools
title: Brongroepen koppelen aan projecten en sjablonen
description: Brongroepen zijn verzamelingen gebruikers die u helpen bij het beheren van bronnen in Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: 36599722aafadcbbc630650a94005fd73b3e517e
workflow-type: tm+mt
source-wordcount: '644'
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
   <td> <p>Toegang tot bronnenbeheer bewerken, inclusief toegang tot Brongroepen beheren</p> <p>Toegang tot projecten, sjablonen en gebruikers bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de projecten, sjablonen en gebruikers beheren waaraan u de bronnengroepen koppelt</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

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
