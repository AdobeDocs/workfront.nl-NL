---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Doelen verwijderen en deactiveren in Adobe Workfront-doelen
description: Wanneer u aan een doel begint te werken en het in uw organisatie irrelevant wordt, adviseren wij deactivering het, in plaats van het te schrappen. Als u een doel deactiveert, blijft de historische informatie behouden en hebt u de kans om het later opnieuw te activeren. Wanneer u een doel verwijdert, kan het echter logisch zijn dat u uw doellijst nauwkeurig houdt.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# Doelen verwijderen en deactiveren in Adobe Workfront-doelen

Wanneer u aan een doel begint te werken en het in uw organisatie irrelevant wordt, adviseren wij deactivering het, in plaats van het te schrappen. Als u een doel deactiveert, blijft de historische informatie behouden en hebt u de kans om het later opnieuw te activeren. Wanneer u een doel verwijdert, kan het echter logisch zijn dat u uw doellijst nauwkeurig houdt.

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
 <p>Huidige licentie: aanvragen of hoger</p> </td>
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
 <td role="rowheader"><p>Toegangsniveau</p></td>
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

## Doelen deactiveren

U kunt een doel deactiveren dat niet meer relevant is en dat u in de toekomst wellicht opnieuw wilt activeren.

* [ Overwegingen wanneer het deactiveren van doelstellingen ](#considerations-when-deactivating-goals)
* [Doelen deactiveren](#deactivate-goals)

### Overwegingen bij het deactiveren van doelen

Herinner het volgende wanneer het deactiveren van doelstellingen:

* U kunt doelen alleen deactiveren in een actieve status. Voor informatie over het activeren van een doel, zie [ doelstellingen in de Doelen van Adobe Workfront ](../../workfront-goals/goal-management/activate-goals.md) activeren.

  >[!TIP]
  >
  >U kunt doelen in een conceptstatus niet deactiveren.

* Workfront berekent niet langer de voortgang van gedeactiveerde doelen.
* Niet-actieve doelen worden niet meer weergegeven in het gedeelte Grafieken van Workfront Goals, of er wordt hiermee rekening mee gehouden. Voor informatie over de grafieken van de Doelen van Workfront, zie [ grafieken van het Overzicht om de tendensen van de doelvooruitgang in de Doelen van Adobe Workfront te begrijpen ](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

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

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hogere juiste hoek, dan klik **Doelen**.

   De vertoningen van de doellijst.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. (Optioneel) Wijzig de filters om alleen actieve doelen weer te geven.

   Voor informatie over het filtreren van informatie in de Doelen van Workfront, zie [ informatie van de Filter in de Doelen van Adobe Workfront ](../goal-management/filter-information-wf-goals.md).

1. Klik op een actief doel.

   De doelpagina wordt geopend.

   ![](assets/goal-page-unshimmed.png)

1. Klik **Meer** menu ![](assets/more-icon.png) aan het recht van de doelnaam, dan klik **Deactivate**.

1. Het doel wordt gedeactiveerd en zijn status wordt Inactief.

## Doelstellingen verwijderen

U kunt doelstellingen schrappen die niet meer of zou nooit relevant kunnen zijn.

* [ Overwegingen wanneer het schrappen van doelstellingen ](#considerations-when-deleting-goals)
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

1. Klik het Belangrijkste pictogram van het Menu ![](assets/main-menu-icon.png) in de hogere juiste hoek, dan klik **Doelen**.

   De vertoningen van de doellijst.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Klik op de naam van een doel. Hierdoor wordt de doelpagina geopend.
1. Klik het **Meer** menu ![](assets/more-icon.png) aan het recht van de doelnaam, dan klik **Goal van de Schrapping**, dan **Schrapping**.

   Het doel en de activiteiten en resultaten ervan worden eveneens geschrapt en kunnen niet worden teruggevorderd. De projecten die met het doel of de kinddoelstellingen werden geassocieerd worden niet geschrapt.


