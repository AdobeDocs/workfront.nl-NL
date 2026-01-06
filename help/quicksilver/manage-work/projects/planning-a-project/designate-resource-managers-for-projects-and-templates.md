---
product-area: projects;templates
navigation-topic: plan-a-project
title: Bronbeheerders aanwijzen voor een project of sjabloon
description: U kunt de Managers van het Middel voor een project aanwijzen om erop te wijzen wie voor het beheren van middelen op het project verantwoordelijk is.
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 0%

---

# Bronbeheerders aanwijzen voor een project of sjabloon

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

U kunt de Managers van het Middel voor een project aanwijzen om erop te wijzen wie voor het beheren van middelen op het project verantwoordelijk is. Dit is een informatieveld en het is niet verbonden met om het even welke hulpmiddelen van het middelbeheer.

<!-- drafted for res scheduling deprecation blurb for preview release
Designating Resource Managers for a project is a prerequisite for using the Scheduling tools in Adobe Workfront, in the Production environment.
  
>[!CAUTION]  
>  
>  
> <span class="preview">Some of the information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span>  
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span>  
>  
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../../resource-mgmt/workload-balancer/workload-balancer.md).</span>  
>  
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten en sjablonen bewerken</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het project of de sjabloon beheren</p>

</td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Templates</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project or template</p> 
   
   <p><b>NOTE</b>
   
   Users who are added as Resource Managers to a project or a template immediately gain Manage permissions on the project or the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Overwegingen over Resource Managers

>[!NOTE]
>
>De Manager van het middel is geen baanrol; het is een gebied beschikbaar op een project of een malplaatje dat u manueel kunt bijwerken.

* U kunt tot 30 gebruikers als Managers van het Middel voor een individueel project of een malplaatje aanwijzen.

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Workload Balancer overview](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* U kunt geen teams of groepen als middelmanagers aanwijzen. U kunt gebruikers alleen aanwijzen als bronmanagers.

* De gebruikers die u als Beheerders van het Middel op een project of een malplaatje aanwijst worden automatisch geen deel van het Team van het Project.

  Voor informatie over projectteams, zie [&#x200B; het Team van het Project beheren &#x200B;](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* U kunt de Managers van het Middel voor projecten of voor projectmalplaatjes aanwijzen. Wanneer u de Managers van het Middel op een projectmalplaatje aanwijst, om het even welke gebruikers u als Managers van het Middel op het malplaatje aanwijst worden automatisch de Managers van het Middel op om het even welke projecten die gebruikend dat malplaatje worden gecreeerd.
* U kunt het gebied van de Manager van het Middel op de volgende gebieden bekijken:

   * Tijdens het bewerken van een project, zoals beschreven in dit artikel.
   * Tijdens het bewerken van een sjabloon, zoals beschreven in dit artikel.
   * Tijdens het samenstellen van project- of sjabloonrapporten. Voor informatie over de bouw van rapporten, zie [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.
   * Bij het maken of aanpassen van een project- of sjabloonweergave voor een lijst. Voor meer informatie, zie [&#x200B; Overzicht van Meningen in Adobe Workfront &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* U kunt de Managers van het Middel op veelvoudige projecten of malplaatjes snel toevoegen of verwijderen door het gebied van de Manager van het Middel aan een mening van een lijst of een project toe te voegen en dit gebied uit te geven gebruikend in-line geef uit.

## Bronbeheerders aanwijzen voor een project

1. Voer een van de volgende handelingen uit:

   * Om de Managers van het Middel aan één enkel project toe te voegen, ga naar het project waar u één of meerdere middelmanagers wilt aanwijzen, dan klik het **Meer menu** naast de projectnaam, dan **geeft uit.**

   * Om de Managers van het Middel aan veelvoudige projecten gelijktijdig toe te voegen, navigeer aan een lijst van projecten, selecteer de projecten waar u één of meerdere middelmanagers wilt aanwijzen, dan klik **uitgeven**.

     De bestaande Managers van het Middel worden niet verwijderd uit de projecten u uitgeeft; om het even welke gebruikers u op deze manier toevoegt worden toegevoegd als Managers van Middelen op het project naast om het even welke bestaande Managers van het Middel.

   * Om de Managers van het Middel aan een nieuw project toe te voegen, begin creërend een nieuw project.

     Voor informatie over het creëren van een project, zie [&#x200B; een project &#x200B;](../../../manage-work/projects/create-projects/create-project.md) creëren.

1. In de **sectie van het Overzicht** op het Edit de dialoogvakje van het Project, klik op het **gebied van de Manager van het Middel**.
1. Typ de naam van de gebruiker die u als middelmanager voor het project wilt toevoegen, dan klik de naam wanneer het in de lijst verschijnt.

   Herhaal deze stap om veelvoudige middelmanagers voor het project toe te voegen.

1. Klik **sparen Veranderingen**.

## Bronbeheer toewijzen voor een sjabloon

{{step1-to-templates}}

1. Voer een van de volgende handelingen uit:

   * Om de Managers van het Middel aan één enkel malplaatje toe te voegen, ga naar het malplaatje waar u één of meerdere middelmanagers wilt aanwijzen, dan klik het **Meer menu** naast de malplaatjenaam, dan **geeft uit.**

   * Om de Managers van het Middel aan veelvoudige malplaatjes gelijktijdig toe te voegen, ga naar een lijst van malplaatjes en selecteer de malplaatjes waar u één of meerdere Managers van het Middel wilt aanwijzen, dan klik **uitgeven**.

     De bestaande Managers van het Middel worden niet verwijderd uit de malplaatjes u uitgeeft; om het even welke gebruikers u op deze manier toevoegt worden toegevoegd als Managers van Middelen op het malplaatje naast om het even welke bestaande Managers van het Middel.

   * Om de Managers van het Middel aan een nieuw malplaatje toe te voegen, klik **Nieuw Malplaatje**, dan klik het **Meer menu** naast de malplaatjenaam, dan **geeft uit.**

1. In de **sectie van het Overzicht**, klik op het **gebied van de Manager van het Middel**.
1. Typ de naam van de gebruiker die u als middelmanager voor het malplaatje wilt toevoegen, dan klik de naam wanneer het in de lijst verschijnt.

   Herhaal deze stap om veelvoudige middelmanagers aan het malplaatje toe te voegen.

1. Klik **sparen Veranderingen**.
