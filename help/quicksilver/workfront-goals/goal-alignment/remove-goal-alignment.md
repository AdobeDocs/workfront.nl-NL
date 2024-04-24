---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Doeluitlijning van Adobe Workfront-doelen verwijderen
description: U kunt de uitlijning tussen twee doelen verwijderen als het niet langer logisch is dat ze met elkaar verbonden zijn.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: 2f8a5b2d2183090029966a13c7af37f20eb44fd0
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Doeluitlijning van Adobe Workfront-doelen verwijderen

U kunt de uitlijning tussen twee doelen verwijderen als het niet langer logisch is dat ze met elkaar verbonden zijn.

Raadpleeg de volgende artikelen voor informatie over het uitlijnen van doelen:

* [Richt doelstellingen door hen in de Doelen van Adobe Workfront te verbinden](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [Richt doelstellingen door resultaten en activiteiten aan doelstellingen om te zetten](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

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
   <p>Nieuw abonnement: Selecteren of hoger</p>
   of
   <p>Huidig abonnement: Pro of hoger</p>
   
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
   <p>Huidige productvereiste: een Workfront-plan en een extra licentie voor Adobe Workfront Goals. </p> <p>Zie voor meer informatie <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Vereisten voor het gebruik van Workfront-doelen</a>. </p> </td>
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
     <p>Voor informatie over het delen van doelstellingen, zie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Een doel delen in Workfront-doelen</a>. </p>
    </td>
  </tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het gebied Doelen in het hoofdmenu bevat. </p>  
</td>
  </tr>
 </tbody>
</table>

*Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
1. Click the **gear icon** ![](assets/gear-icon-settings.png) next to the parent goal, then click **Remove alignment**.

   ![](assets/edit-remove-alignment-350x88.png)

   The goal becomes a standalone goal and its progress no longer influences the progress of the original parent goal. 

1. (Optional) Click **Undo** in the lower-left corner of the screen if you want to revert this change and keep the goals aligned. 
1. (Optional) Add activities and results to either goals to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)
-->

1. Toegang krijgen tot de **Doelen** in Workfront en klik op de naam van een doel om de doelpagina te openen.
1. Van de pagina van het doel van een ouderdoel, klik **Voortgangsindicatoren** in het linkerdeelvenster.

   ![](assets/remove-goal-alignment-from-list-unshimmed.png)

1. In de **Type: Doel** groeperen, een doel selecteren en vervolgens op de knop **Verbinding verbreken** pictogram ![](assets/disconnect-goal-to-remove-alignment-icon-unshimmed.png) boven aan de lijst.

   Het vak Verbinding verbreken wordt weergegeven.

1. Klikken **Verbinding verbreken** om het geselecteerde doel van zijn ouder los te maken.

   Het doel wordt een zelfstandig doel en wordt niet meer vermeld als een voortgangsindicator van het oorspronkelijke doel. De voortgang van het ontkoppelde doel beïnvloedt niet langer de voortgang van het oorspronkelijke doel.

   Een succesbericht wordt in de rechterbovenhoek van de pagina weergegeven om te bevestigen dat het doel is losgekoppeld.