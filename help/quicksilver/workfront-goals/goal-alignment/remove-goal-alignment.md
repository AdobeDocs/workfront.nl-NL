---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Goal Alignment in Adobe Workfront Goals verwijderen
description: U kunt de uitlijning tussen twee doelen verwijderen als het niet langer logisch is dat ze met elkaar verbonden zijn.
author: Alina
feature: Workfront Goals
exl-id: a6196356-ca11-4759-9cff-64850a60208e
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# Doeluitlijning van Adobe Workfront-doelen verwijderen

<!--Audited P&P only: 4/2025-->

U kunt de uitlijning tussen twee doelen verwijderen als het niet langer logisch is dat ze met elkaar verbonden zijn.

Raadpleeg de volgende artikelen voor informatie over het uitlijnen van doelen:

* [&#x200B; richt doelstellingen door hen in de Doelen van Adobe Workfront te verbinden &#x200B;](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)
* [Richt doelstellingen door resultaten en activiteiten aan doelstellingen om te zetten](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md)

## Toegangsvereisten

>[!NOTE]
>
>Uw bedrijf zou kunnen verkiezen om de Doelen van Adobe Workfront verder te gebruiken als zij dit pakket in het verleden kochten. U moet voor meer informatie contact opnemen met uw accountvertegenwoordiger.
>
>Adobe Workfront Goals kan niet meer worden aangeschaft.

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront-pakket</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
 <tr>
 <td role="rowheader">Adobe Workfront-licentie</td>
 <td>
 <p>Medewerker of hoger</p>
 <p>Aanvraag of hoger</p> </td>
 </tr>
  <tr>
 <td role="rowheader">Toegangsniveau</td>
 <td> <p>Toegang tot doelen bewerken</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Objectmachtigingen</td>
 <td>
  <p>De toestemmingen van de mening of hoger aan het doel om het te bekijken</p>
  <p>Machtigingen beheren om het te bewerken</p>

</td>
 </tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> <p>Aan alle gebruikers, inclusief Systeembeheerders, moet een lay-outsjabloon worden toegewezen die het gebied Doelen in het hoofdmenu bevat. </p>  
</td>
  </tr>
</tbody>
</table>

Voor meer informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++
<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Adobe Workfront plan*</td>
 <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
 </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
   <p> New product requirement: Workfront</p>
   Or
   <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </td>
 </tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

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

   ![&#x200B; REmove doel groepering &#x200B;](assets/remove-goal-alignment-from-list-unshimmed.png)

1. In het **Type: Goal** groeperen, selecteer een doel, dan klik **losmaakt** pictogram ![&#x200B; los pictogram &#x200B;](assets/disconnect-goal-to-remove-alignment-icon-unshimmed.png) bij de bovenkant van de lijst los.

   Het vak Verbinding verbreken wordt weergegeven.

1. Klik **losmaken** om het geselecteerde doel van zijn ouder los te maken.

   Het doel wordt een zelfstandig doel en wordt niet meer vermeld als een voortgangsindicator van het oorspronkelijke doel. De voortgang van het ontkoppelde doel beïnvloedt niet langer de voortgang van het oorspronkelijke doel.

   Een succesbericht wordt in de rechterbovenhoek van de pagina weergegeven om te bevestigen dat het doel is losgekoppeld.
