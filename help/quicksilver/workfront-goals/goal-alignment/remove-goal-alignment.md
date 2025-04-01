---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Goal Alignment in Adobe Workfront Goals verwijderen
description: U kunt de uitlijning tussen twee doelen verwijderen als het niet langer logisch is dat ze met elkaar verbonden zijn.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Doeluitlijning van Adobe Workfront-doelen verwijderen

<!--Audited P&P only: 4/2025-->

U kunt de uitlijning tussen twee doelen verwijderen als het niet langer logisch is dat ze met elkaar verbonden zijn.

Raadpleeg de volgende artikelen voor informatie over het uitlijnen van doelen:

* [ richt doelstellingen door hen in de Doelen van Adobe Workfront te verbinden ](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [Richt doelstellingen door resultaten en activiteiten aan doelstellingen om te zetten](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
  <ul><li>Een Ultimate-abonnement </li></ul>
   </p>
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
   <p> Nieuwe productvereisten: Workfront</p>
   of
   <p>Huidige productvereiste: Naast een Workfront-licentie moet u een licentie aanschaffen voor Adobe Workfront Goals. </p> <p>Voor informatie, zie <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref"> Vereisten om de Doelen van Workfront </a> te gebruiken. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Toegangsniveau</td>
 <td> <p>Toegang tot doelen bewerken</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objectmachtigingen</td>
 <td>
  <p>De toestemmingen van de mening of hoger aan het doel om het te bekijken</p>
  <p>Machtigingen beheren om het te bewerken</p>
  <p>Voor informatie over het delen van doelstellingen, zie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref"> een doel in de Doelen van Workfront delen </a>. </p>
  </td>
 </tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het gebied Doelen in het hoofdmenu bevat. </p>  
</td>
  </tr>
</tbody>
</table>

*Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

U moet het volgende hebben voordat u kunt beginnen:

* Een bovenliggend doel waaraan minstens één onderliggend doel is gekoppeld. Kinderdoelen zijn de voortgangsindicatoren van het doel.

## Overwegingen bij het verwijderen van doeluitlijning

Overweeg het volgende wanneer het verwijderen van groepering tussen twee doelstellingen:

* Het ouderdoel moet een ander doel, een activiteit, of een resultaat verbonden aan het hebben om Actief te kunnen blijven.
* U kunt een uitgelijnd onderliggend doel niet verwijderen uit een bovenliggend doel als dit de enige voortgangsindicator van het bovenliggende doel is.
* Het kinddoel wordt een standalone doel wanneer u zijn groepering aan het ouderdoel verwijdert.

## Doeluitlijning verwijderen

<!--
Removing goal alignment differs depending on which environment you use.

### Remove goal alignment in the Production environment


1. Go to a child goal aligned to a parent goal. 
1. Click the goal name to open the **Goal Details** panel. 
1. Click the **gear icon** ![Gear icon](assets/gear-icon-settings.png) next to the parent goal, then click **Remove alignment**.

   ![Reove alignment](assets/edit-remove-alignment-350x88.png)

   The goal becomes a standalone goal and its progress no longer influences the progress of the original parent goal. 

1. (Optional) Click **Undo** in the lower-left corner of the screen if you want to revert this change and keep the goals aligned. 
1. (Optional) Add activities and results to either goals to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
-->

1. Heb toegang tot het **gebied van Doelen** in Workfront en klik de naam van een doel om de pagina van het doel te openen.
1. Van de pagina van het doel van een ouderdoel, klik **Indicatoren van de Voortgang** in het linkerpaneel.

   ![ REmove doel groepering ](assets/remove-goal-alignment-from-list-unshimmed.png)

1. In het **Type: Goal** groeperen, selecteer een doel, dan klik **losmaakt** pictogram ![ los pictogram ](assets/disconnect-goal-to-remove-alignment-icon-unshimmed.png) bij de bovenkant van de lijst los.

   Het vak Verbinding verbreken wordt weergegeven.

1. Klik **losmaken** om het geselecteerde doel van zijn ouder los te maken.

   Het doel wordt een zelfstandig doel en wordt niet meer vermeld als een voortgangsindicator van het oorspronkelijke doel. De voortgang van het ontkoppelde doel beïnvloedt niet langer de voortgang van het oorspronkelijke doel.

   Een succesbericht wordt in de rechterbovenhoek van de pagina weergegeven om te bevestigen dat het doel is losgekoppeld.