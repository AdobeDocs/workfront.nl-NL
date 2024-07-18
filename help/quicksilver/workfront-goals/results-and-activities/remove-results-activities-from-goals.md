---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Voortgangsindicatoren verwijderen uit doelen van Adobe Workfront
description: U kunt resultaten, activiteiten, en projecten van doelstellingen in de Doelen van Adobe Workfront verwijderen, wanneer zij niet meer relevant zijn.
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# Voortgangsindicatoren verwijderen uit doelen van Adobe Workfront

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

U kunt resultaten, activiteiten, en projecten uit doelstellingen verwijderen als zij niet meer relevant zijn.

Raadpleeg de volgende artikelen voor informatie over het maken van doelen en het toevoegen van resultaten en activiteiten aan deze doelen:

* [ creeer doelstellingen in de Doelen van Adobe Workfront ](../../workfront-goals/goal-management/create-goals.md)
* [ voeg activiteiten aan doelstellingen in de Doelen van Adobe Workfront toe ](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [ voeg resultaten aan doelstellingen in de Doelen van Adobe Workfront toe ](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Resultaten en activiteiten bewerken in Adobe Workfront Goals](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

De doelstellingen kunnen ook aan ouderdoelstellingen worden gericht, die kinddoelstellingen worden. Kinderdoelen zijn ook voortgangsindicatoren van de bovenliggende doelen.

U kunt de groepering tussen doelstellingen verwijderen door de verbinding tussen hen te verwijderen. Voor informatie, zie [ doelgroepering in de Doelen van Adobe Workfront verwijderen ](../goal-alignment/remove-goal-alignment.md).

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> 
   <p>Voor het nieuwe plan en de nieuwe licentiestructuur:
  <ul><li>Een ultiem plan </li>
  of
  <li>Een extra licentie voor Adobe Workfront Goals voor de Adobe Workfront-plannen voor de Premier of Select. </li></ul> </p>
<p>Voor het huidige plan en de licentiestructuur: 
<ul><li> Een Pro of hoger </li>
  <li>Een Adobe Workfront Goals-licentie in aanvulling op een Workfront-licentie.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-licentie*</td>
 <td>
 <p>Nieuwe licentie: Medewerker of hoger</p>
 of
 <p>Huidige licentie: aanvragen of hoger</p> <p>Voor meer informatie, zie <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref"> het vergunningsoverzicht van Adobe Workfront </a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> Nieuwe productbehoefte, één van het volgende: </p>
<ul>
<li>Een Select- of Prime Adobe Workfront-abonnement en een extra Adobe Workfront Goals-licentie.</li>
<li>Een Ultimate Workfront-plan dat standaard Workfront Goals bevat. </li></ul>
 <p>of</p>
 <p>Huidige productvereiste: een Workfront-plan en een extra licentie voor Adobe Workfront Goals. </p> <p>Voor informatie, zie <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref"> Vereisten om de Doelen van Workfront </a> te gebruiken. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Toegangsniveau</td>
 <td> <p>Toegang tot doelen bewerken</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objectmachtigingen</td>
 <td>
  <div>
  <p>De toestemmingen van de mening of hoger aan het doel om het te bekijken</p>
  <p>Machtigingen beheren om het te bewerken</p>
  <p>Voor informatie over het delen van doelstellingen, zie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref"> een doel in de Doelen van Workfront delen </a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het gebied Doelen in het hoofdmenu bevat. </p>  
</td>
  </tr>
</tbody>
</table>

*Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

U moet een doel hebben verbonden aan resultaten, activiteiten, of projecten.

## Overwegingen voor het verwijderen van resultaten, activiteiten, en het losmaken van projecten van doelstellingen

* U kunt resultaten en activiteiten slechts uit actieve doelstellingen verwijderen.
* U kunt resultaten en activiteiten uit een doel verwijderen door hen te schrappen. Verwijderde resultaten en activiteiten kunnen niet worden hersteld.
* Wanneer u het resultaat of de activiteit uit een doel verwijdert, beïnvloedt de vooruitgang van het verwijderde resultaat of de activiteit de algemene vooruitgang van het doel.
* U kunt geen project van een doel schrappen, maar u kunt het van het doel losmaken. Door het project van het doel los te maken beïnvloedt het percentage voltooide van het project niet meer de vooruitgang van het doel.

  Voor informatie over hoe de projecten doelvooruitgang beïnvloeden, zie [ projecten aan doelstellingen in de Doelen van Adobe Workfront ](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md) toevoegen.

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

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek, dan klik **Doelen**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   Dit opent het gebied van de Doelstellingen van Workfront en de vertoningen van de Lijst van het Gol door gebrek.

1. Klik op de naam van een doel waaruit u resultaten en activiteiten wilt verwijderen.

   Hierdoor wordt de doelpagina geopend.

1. Klik **indicatoren van de Voortgang** in het linkerpaneel.

1. Selecteer een resultaat of een activiteit, dan klik **Schrapping** pictogram ![](assets/delete-icon.png) bij de bovenkant van de lijst.

1. Klik **Schrapping** om de schrapping te bevestigen. Het resultaat of de activiteit wordt verwijderd en kan niet worden hersteld. Het percentage voltooide van het doel werkt bij om de verwijderde activiteit of het resultaat uit te sluiten.


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


1. Klik het **Belangrijkste pictogram van het Menu** in de hoger-juiste hoek, dan klik **Doelen**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Dit opent het gebied van de Doelstellingen van Workfront en de vertoningen van de Lijst van het Gol door gebrek.

1. Klik op de naam van een doel waaruit u resultaten en activiteiten wilt verwijderen.

   Hierdoor wordt de doelpagina geopend.
1. Klik **indicatoren van de Voortgang** in het linkerpaneel.
1. Selecteer een project, dan klik **losmaken** pictogram ![](assets/disconnect-icon.png) bij de bovenkant van de lijst.
1. Klik **losmaken** om te bevestigen.

   Het project is niet meer verbonden met het doel. Het percentage voltooide van het doel werkt bij om het losgemaakte project uit te sluiten.

