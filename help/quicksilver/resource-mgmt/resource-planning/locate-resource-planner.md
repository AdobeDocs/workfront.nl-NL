---
product-area: resource-management
navigation-topic: resource-planning
title: Bronnen zoeken
description: '''(Dit artikel is van toepassing: concept dat inhoud in het artikel bevat wanneer dit live gaat : /Content/Resource Management/Resource Planning/get-started-resource-planner.html)"'
author: Alina
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Bronnen zoeken

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

U kunt de Planner van het Middel gebruiken om de toewijzing van uw middelen aan projecten te beheren. U kunt tot de Planner van het Middel voor veelvoudige projecten tezelfdertijd of voor één project, van het Van Bedrijfs project gebied toegang hebben.

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
   <td> <p>Controleren of hoger<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> <p>Plan of hoger om van de Planner van het Middel in het globale gebied de plaats te bepalen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot of hoger weergeven voor bronnenbeheer</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toestemmingen voor projecten en gebruikers weergeven </p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

Zorg ervoor dat aan alle voorwaarden voor toegang tot en het werken met de Planner van het Middel wordt voldaan alvorens het te beginnen te gebruiken. Op deze manier zorgt u ervoor dat de functie Bronnen de juiste gegevens weergeeft voordat u begint met het budgetteren van uw bronnen.

Voor informatie over de voorwaarden van de Planner van het Middel, zie [Aan de slag met bronnenplanning](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Bronnen zoeken

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

U kunt van de Planner van het Middel in twee gebieden van Workfront de plaats bepalen, afhankelijk van of u uw middelen voor veelvoudige projecten, of voor enkel één project wilt begroten.

* [Gebruik de Planner van het Middel voor veelvoudige projecten](#use-the-resource-planner-for-multiple-projects)
* [Gebruik de Planner van het Middel voor één project](#use-the-resource-planner-for-one-project)

### Gebruik de Planner van het Middel voor veelvoudige projecten {#use-the-resource-planner-for-multiple-projects}

Wanneer het gebruiken van de Planner van het Middel voor veelvoudige projecten, vertegenwoordigen de toewijzingsaantallen voor uw middelen aantallen over veelvoudige projecten.

De sectie Planner openen in het gebied Bronnen:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront.

1. Klikken **Bronnen**. Standaard wordt de Planner weergegeven.  Zie het artikel voor informatie over budgettering van bronnen in de functie voor middelenbeheer [De middelen van de begroting in de Planner van het Middel gebruikend de meningen van het Project en van de Rol](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   ![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. Houd de cursor boven het linkerdeelvenster en klik op **Brongroepen**.\
   Voor informatie over het maken van bronnenpools raadpleegt u [Brongroepen maken](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### Gebruik de Planner van het Middel voor één project {#use-the-resource-planner-for-one-project}

Wanneer het gebruiken van de Planner van het Middel voor één project, vertegenwoordigen de toewijzingsaantallen voor uw middelen aantallen voor het geselecteerde project.

1. Ga naar een project waarvoor u middelen wilt begroten.
1. Klikken **Bedrijfs-case** in het linkerdeelvenster.
1. Naar de **Bronnen begroten** van de Business Case.
1. Klikken **Resource Budgeting bewerken** om bronnenpools aan uw project toe te voegen en uw bronnen in de begroting op te nemen.

   >[!TIP]
   >
   >U kunt een middelpool in het het Lagen van het Middel gebied van het BedrijfsGeval slechts toevoegen wanneer het project geen middelgroepen verbonden aan het heeft. Wanneer het project reeds een Pool van het Middel heeft, tonen de gebruikers in de pool en hun baanrollen in het het Leiden van het Middel gebied door gebrek.

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   Zie het artikel voor informatie over het budgetteren van middelen voor één project [Begrotingsmiddelen in het bedrijfscase](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
