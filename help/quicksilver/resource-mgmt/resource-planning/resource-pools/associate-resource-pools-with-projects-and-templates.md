---
product-area: resource-management
navigation-topic: resource-pools
title: Brongroepen koppelen aan projecten en sjablonen
description: Brongroepen zijn verzamelingen gebruikers die u helpen bij het beheren van bronnen in Adobe Workfront.
author: Alina
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: 23257f11b0795aa1f1e422923f6d596017c58126
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# Brongroepen koppelen aan projecten en sjablonen


<!-- drafted for bulk editing projects: keep this in yellow till this releases to ALL customers - May 1, 2023

Also - take out all the references to Preview and Prod at prod final
-->

<span class="preview">De gemarkeerde informatie op deze pagina verwijst naar functionaliteit die nog niet algemeen beschikbaar is. Deze optie is alleen beschikbaar in de voorvertoningsomgeving.</span>


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
</div>
-->

Brongroepen zijn verzamelingen gebruikers die u helpen bij het beheren van bronnen in Adobe Workfront.

Nadat u middelpools creeert, kunt u hen met projecten of malplaatjes associëren zodat kunt u uw middelen op de projecten later begroten.

Wij adviseren dat u uw middelgroepen vooraf creeert, hen associeert met projecten, en uw middelen begroot alvorens het project begint.

Voor informatie over bronnenpools raadpleegt u [Overzicht van bronnenpools](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

Voor informatie over het maken van bronnenpools raadpleegt u [Brongroepen maken](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

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
   <td> <p>Toegang tot bronnenbeheer bewerken, inclusief toegang tot Brongroepen beheren</p> <p>Toegang tot projecten, sjablonen en gebruikers bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor de projecten, sjablonen en gebruikers beheren waaraan u de bronnengroepen koppelt</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Brongroepen koppelen aan één project of sjabloon

U kunt middelpools met een malplaatje op de zelfde manier associëren u middelpools met een project. Dit artikel beschrijft hoe u middelgroepen met projecten kunt associëren.

1. Ga naar een project en klik op de knop **Meer** pictogram ![](assets/more-icon.png)naast de projectnaam klikt u op **Bewerken**.

1. Klikken **Projectinstellingen**.

1. Begin de naam van een middelpool in te typen **Brongroepen** en selecteert u deze in de lijst wanneer deze wordt weergegeven.\
   U kunt veelvoudige middelpools met één project of malplaatje associëren.

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. Klikken **Opslaan**.

Voor meer informatie over hoe te om een project uit te geven en het te associëren met middelpools, zie [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

Voor meer informatie over hoe te om een malplaatje uit te geven en het te associëren met middelpools, zie [Projectsjablonen bewerken](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Brongroepen koppelen aan meerdere projecten of sjablonen in bulk

U kunt veelvoudige projecten of malplaatjes in bulk uitgeven en de zelfde middelgroepen met elk van hen tezelfdertijd associëren.

U kunt middelpools met malplaatjes op de zelfde manier associëren u middelpools met projecten.

Om middelgroepen met verscheidene projecten in bulk te associëren:

1. Ga naar een lijst met projecten.
1. Selecteer meerdere projecten en klik op de knop **Bewerken** pictogram ![](assets/edit-icon.png) boven aan de lijst.

1. Klikken **Instellingen**.
1. Begin de naam van een middelpool in te typen **Brongroepen** en selecteert u deze in de lijst wanneer deze wordt weergegeven.\
   U kunt veelvoudige middelgroepen met de projecten of de malplaatjes associëren.

   >[!NOTE]
   >
   >* In het milieu van de Productie, wanneer u projecten of malplaatjes in bulk uitgeeft, slechts verschijnen de middelgroepen die voor alle geselecteerde projecten of malplaatjes gemeenschappelijk zijn op dit gebied. Als de geselecteerde projecten geen gedeelde bronnenpools hebben, is dit veld leeg. De middelpools u hier specificeert zullen de individuele middelpools van de projecten of de malplaatjes beschrijven.
   >
   >* <span class="preview">In het milieu van de Voorproef, wanneer u projecten in bulk uitgeeft, is er een &quot;Veelvoudige waarde&quot;indicator als de geselecteerde projecten verschillende middelgroepen hebben. Als u bronnenpools bulksgewijs toevoegt, worden alle pools toegevoegd aan het geselecteerde project en worden de oorspronkelijke bronnenpools overschreven.</span>


   <span class="preview">![add_resource_pools_to_multiple_projects.png](assets/add-resource-pools-to-multiple-projects-350x358.png)</span>

1. Klikken **Wijzigingen opslaan**.\
   Wanneer uw middelpools met uw projecten of uw malplaatjes worden geassocieerd, kunt u gebruikerstoewijzingen voor uw projecten binnen de Planner van het Middel begroten.\
   Voor meer informatie over de Planner van het Middel, zie [Overzicht van de bronnenplanner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Voor meer informatie over hoe te om projecten in bulk uit te geven, zie de &quot;projecten in bulk&quot;sectie in [Projecten bewerken](../../../manage-work/projects/manage-projects/edit-projects.md).

Voor meer informatie over het bulksgewijs bewerken van sjablonen raadpleegt u de sectie &#39;Sjablonen bulksgewijs bewerken&#39; in [Projectsjablonen bewerken](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
