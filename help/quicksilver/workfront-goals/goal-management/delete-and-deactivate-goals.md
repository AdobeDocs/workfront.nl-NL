---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Doelen verwijderen en deactiveren in Adobe Workfront-doelen
description: Wanneer u aan een doel begint te werken en het in uw organisatie irrelevant wordt, adviseren wij deactivering het, in plaats van het te schrappen. Als u een doel deactiveert, blijft de historische informatie behouden en hebt u de kans om het later opnieuw te activeren. Wanneer u een doel verwijdert, kan het echter logisch zijn dat u uw doellijst nauwkeurig houdt.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Doelen verwijderen en deactiveren in Adobe Workfront-doelen

Wanneer u aan een doel begint te werken en het in uw organisatie irrelevant wordt, adviseren wij deactivering het, in plaats van het te schrappen. Als u een doel deactiveert, blijft de historische informatie behouden en hebt u de kans om het later opnieuw te activeren. Wanneer u een doel verwijdert, kan het echter logisch zijn dat u uw doellijst nauwkeurig houdt.

## Toegangsvereisten

<!--drafted for P&P release: 

You must have the following:

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
   <td> <p>Toegang tot doelen of hoger bewerken</p> <p><b>OPMERKING</b>

<p>Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie:</p> 
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

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

U moet het volgende hebben voordat u kunt beginnen:

* Een lay-outsjabloon die het gebied Doelen in het hoofdmenu bevat.

## Doelen deactiveren

U kunt een doel deactiveren dat niet meer relevant is en dat u in de toekomst wellicht opnieuw wilt activeren.

* [Overwegingen bij het deactiveren van doelen](#considerations-when-deactivating-goals)
* [Doelen deactiveren](#deactivate-goals)

### Overwegingen bij het deactiveren van doelen

Herinner het volgende wanneer het deactiveren van doelstellingen:

* U kunt doelen alleen deactiveren in een actieve status. Voor informatie over het activeren van een doel raadpleegt u [Doelen in Adobe Workfront-doelen activeren](../../workfront-goals/goal-management/activate-goals.md).

   >[!TIP]
   >
   >U kunt doelen in een conceptstatus niet deactiveren.

* Workfront berekent niet langer de voortgang van gedeactiveerde doelen.
* Niet-actieve doelen worden niet meer weergegeven in het gedeelte Grafieken van Workfront Goals, of er wordt hiermee rekening mee gehouden. Zie voor meer informatie over Workfront Goals grafieken [Grafieken bekijken om trends in de voortgang van het doel in Adobe Workfront-doelen te begrijpen](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

   <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* U kunt geen updates meer maken van gedeactiveerde doelen.
* U kunt informatie over het doel en zijn groepering uitgeven.
* U kunt een eerder gedeactiveerd doel opnieuw activeren.

### Doelen deactiveren

<!--
Deactivating goals differs depending on which environment you use.

### Deactivate goals in the Production environment


1. Go to the goal that you want to deactivate.

   For example, go to the Goal List and click the name of a goal.

   The Goal Details panel opens on the right.

   >[!TIP]
   >
   >You can open goals from any sections of Workfront Goals.

1. Click the **More icon** ![](assets/more-icon.png), then click **Deactivate**.

   ![](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek klikt u op **Doelen**.

   De vertoningen van de doellijst.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Optioneel) Wijzig de filters om alleen actieve doelen weer te geven.

   Voor informatie over het filtreren van informatie in de Doelen van Workfront, zie [Gegevens filteren in Adobe Workfront Goals](../goal-management/filter-information-wf-goals.md).

1. Klik op een actief doel.

   De doelpagina wordt geopend.

   ![](assets/goal-page-unshimmed.png)

1. Klik op de knop **Meer** menu ![](assets/more-icon.png) rechts van de doelnaam klikt u op **Deactiveren**.

1. Het doel wordt gedeactiveerd en zijn status wordt Inactief.

## Doelstellingen verwijderen

U kunt doelstellingen schrappen die niet meer of zou nooit relevant kunnen zijn.

* [Overwegingen bij het verwijderen van doelen](#considerations-when-deleting-goals)
* [Doelstellingen verwijderen](#delete-goals)

### Overwegingen bij het verwijderen van doelen {#considerations-when-deleting-goals}

* U kunt doelstellingen in om het even welke status, met inbegrip van gesloten doelstellingen schrappen.
* U kunt verwijderde doelen niet herstellen.
* De resultaten en de activiteiten van de handmatige voortgangsbalk die aan het doel zijn gekoppeld, worden ook verwijderd.
* De projecten verbonden aan doelstellingen worden niet geschrapt, maar hun verband met het doel wordt verwijderd.

### Doelstellingen verwijderen

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![](assets/more-icon.png), then click **Delete**.

   ![](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. Klik op het pictogram Hoofdmenu ![](assets/main-menu-icon.png) in de rechterbovenhoek klikt u op **Doelen**.

   De vertoningen van de doellijst.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Klik op de naam van een doel. Hierdoor wordt de doelpagina geopend.
1. Klik op de knop **Meer** menu ![](assets/more-icon.png) rechts van de doelnaam klikt u op **Doel verwijderen** vervolgens **Verwijderen**.

   Het doel en de activiteiten en resultaten ervan worden eveneens geschrapt en kunnen niet worden teruggevorderd. De projecten die met het doel of de kinddoelstellingen werden geassocieerd worden niet geschrapt.


