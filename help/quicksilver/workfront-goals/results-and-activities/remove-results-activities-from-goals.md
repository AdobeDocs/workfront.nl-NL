---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Resultaten, activiteiten en projecten verwijderen uit doelen in Adobe Workfront Goals
description: U kunt resultaten, activiteiten, en projecten van doelstellingen in de Doelen van Adobe Workfront verwijderen, wanneer zij niet meer relevant zijn.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---

# Resultaten, activiteiten en projecten verwijderen uit doelen in Adobe Workfront Goals

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

U kunt resultaten, activiteiten, en projecten uit doelstellingen verwijderen als zij niet meer relevant zijn.

Raadpleeg de volgende artikelen voor informatie over het maken van doelen en het toevoegen van resultaten en activiteiten aan deze doelen:

* [Doelen maken voor Adobe Workfront-doelen](../../workfront-goals/goal-management/create-goals.md)
* [Activiteiten toevoegen aan doelen in Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Resultaten toevoegen aan doelen in Adobe Workfront-doelen](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Resultaten en activiteiten bewerken in Adobe Workfront Goals](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

De doelstellingen kunnen ook aan ouderdoelstellingen worden gericht, die kinddoelstellingen worden. Kinderdoelen zijn ook voortgangsindicatoren van de bovenliggende doelen.

U kunt de groepering tussen doelstellingen verwijderen door de verbinding tussen hen te verwijderen. Zie voor meer informatie [Doeluitlijning van Adobe Workfront-doelen verwijderen](../goal-alignment/remove-goal-alignment.md).

## Toegangsvereisten

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>
-->

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Pro of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Aanvraag of hoger</p> <p>Zie voor meer informatie <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Overzicht van Adobe Workfront-licenties</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>U moet een extra licentie voor de Adobe Workfront Goals aanschaffen om toegang te krijgen tot de functionaliteit die in dit artikel wordt beschreven. </p> <p>Zie voor meer informatie <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Vereisten voor het gebruik van Workfront-doelen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot doelen of hoger bewerken</p> <p><b>OPMERKING</b><p>Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Toegang tot Adobe Workfront-doelen verlenen</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> 
    <div> 
     <p>Rechten voor het doel beheren</p> 
     <p>Voor informatie over het delen van doelstellingen, zie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Een doel delen in Workfront-doelen</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Vereisten

U moet het volgende hebben voordat u kunt beginnen:

* Een lay-outsjabloon die het gebied Doelen in het hoofdmenu bevat.
* Een doel met resultaten, activiteiten of projecten.

## Overwegingen voor het verwijderen van resultaten, activiteiten, en het losmaken van projecten van doelstellingen

* U kunt resultaten en activiteiten slechts uit actieve doelstellingen verwijderen.
* U kunt resultaten en activiteiten uit een doel verwijderen door hen te schrappen. Verwijderde resultaten en activiteiten kunnen niet worden hersteld.
* Wanneer u het resultaat of de activiteit uit een doel verwijdert, beïnvloedt de vooruitgang van het verwijderde resultaat of de activiteit de algemene vooruitgang van het doel.
* U kunt geen project van een doel schrappen, maar u kunt het van het doel losmaken. Door het project van het doel los te maken beïnvloedt het percentage voltooide van het project niet meer de vooruitgang van het doel.

   Voor informatie over hoe de projecten doelvooruitgang beïnvloeden, zie [Projecten toevoegen aan doelen in Adobe Workfront](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* U kunt geen resultaat of een activiteit uit een doel verwijderen, en u kunt geen kinddoel of een project losmaken, als zij de laatste vooruitgangsindicator voor het doel zijn.
* Als een project van het gebied van Projecten wordt geschrapt en het de laatste vooruitgangsindicator van een doel is, wordt het doel Inactief.

## Resultaten en activiteiten van doelen verwijderen

U verwijdert resultaten en activiteiten uit een doel door hen te schrappen. Het verwijderen van resultaten en activiteiten uit een doel is identiek.

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek klikt u op **Doelen**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   Dit opent het gebied van de Doelstellingen van Workfront en de vertoningen van de Lijst van het Gol door gebrek.

1. Klik op de naam van een doel waaruit u resultaten en activiteiten wilt verwijderen.

   Hierdoor wordt de doelpagina geopend.

1. Klikken **Voortgangsindicatoren** in het linkerdeelvenster.

1. Selecteer een resultaat of activiteit en klik op de knop **Verwijderen** pictogram ![](assets/delete-icon.png) boven aan de lijst.

1. Klikken **Verwijderen** om de schrapping te bevestigen. Het resultaat of de activiteit wordt verwijderd en kan niet worden hersteld. Het percentage voltooide van het doel werkt bij om de verwijderde activiteit of het resultaat uit te sluiten.


## Projecten van doelstellingen verwijderen

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


1. Klik op de knop **Hoofdmenu** in de rechterbovenhoek, en klik vervolgens op **Doelen**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Dit opent het gebied van de Doelstellingen van Workfront en de vertoningen van de Lijst van het Gol door gebrek.

1. Klik op de naam van een doel waaruit u resultaten en activiteiten wilt verwijderen.

   Hierdoor wordt de doelpagina geopend.
1. Klikken **Voortgangsindicatoren** in het linkerdeelvenster.
1. Selecteer een project en klik op de knop **Verbinding verbreken** pictogram ![](assets/disconnect-icon.png) boven aan de lijst.
1. Klikken **Verbinding verbreken** ter bevestiging.

   Het project is niet meer verbonden met het doel. Het percentage voltooide van het doel werkt bij om het losgemaakte project uit te sluiten.

