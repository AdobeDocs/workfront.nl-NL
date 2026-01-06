---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Doelen verwijderen en deactiveren in Adobe Workfront-doelen
description: Wanneer u aan een doel begint te werken en het in uw organisatie irrelevant wordt, adviseren wij deactivering het, in plaats van het te schrappen. Als u een doel deactiveert, blijft de historische informatie behouden en hebt u de kans om het later opnieuw te activeren. Wanneer u een doel verwijdert, kan het echter logisch zijn dat u uw doellijst nauwkeurig houdt.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Doelen verwijderen en deactiveren in Adobe Workfront-doelen

<!--Audited for P&P only: 10/2025-->

Wanneer u aan een doel begint te werken en het in uw organisatie irrelevant wordt, adviseren wij deactivering het, in plaats van het te schrappen. Als u een doel deactiveert, blijft de historische informatie behouden en hebt u de kans om het later opnieuw te activeren. Wanneer u een doel verwijdert, kan het echter logisch zijn dat u uw doellijst nauwkeurig houdt.

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
<p>Aanvraag of hoger</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configuratie op toegangsniveau</td>
 <td> <p>Toegang tot doelen bewerken</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objectmachtigingen</td>
 <td>
  <div>
  <p>De toestemmingen van de mening of hoger aan het doel om het te bekijken</p>
  <p>Machtigingen beheren om het te bewerken</p>
  </div> </td>
 </tr>
<tr>
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
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
  <p> New product requirement: Workfront</p>
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
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
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Doelen deactiveren

U kunt een doel deactiveren dat niet meer relevant is en dat u in de toekomst wellicht opnieuw wilt activeren.

* [&#x200B; Overwegingen wanneer het deactiveren van doelstellingen &#x200B;](#considerations-when-deactivating-goals)
* [Doelen deactiveren](#deactivate-goals)

### Overwegingen bij het deactiveren van doelen

Herinner het volgende wanneer het deactiveren van doelstellingen:

* U kunt doelen alleen deactiveren in een actieve status. Voor informatie over het activeren van een doel, zie [&#x200B; doelstellingen in de Doelen van Adobe Workfront &#x200B;](../../workfront-goals/goal-management/activate-goals.md) activeren.

  >[!TIP]
  >
  >U kunt doelen in een conceptstatus niet deactiveren.

* Workfront berekent niet langer de voortgang van gedeactiveerde doelen.
* Niet-actieve doelen worden niet meer weergegeven in het gedeelte Grafieken van Workfront Goals, of er wordt hiermee rekening mee gehouden. Voor informatie over de grafieken van de Doelen van Workfront, zie [&#x200B; grafieken van het Overzicht om de tendensen van de doelvooruitgang in de Doelen van Adobe Workfront te begrijpen &#x200B;](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

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

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Deactivate**.

   ![Deactivate goal](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

{{step1-to-goals}}

De vertoningen van de doellijst.


1. (Optioneel) Wijzig de filters om alleen actieve doelen weer te geven.

   Voor informatie over het filtreren van informatie in de Doelen van Workfront, zie [&#x200B; informatie van de Filter in de Doelen van Adobe Workfront &#x200B;](../goal-management/filter-information-wf-goals.md).

1. Klik op een actief doel.

   De doelpagina wordt geopend.

   ![&#x200B; Goal pagina &#x200B;](assets/goal-page-unshimmed.png)

1. Klik het **Meer** menu ![&#x200B; Meer pictogram &#x200B;](assets/more-icon.png) aan het recht van de doelnaam, dan klik **Deactivate**.

1. Het doel wordt gedeactiveerd en zijn status wordt Inactief.

## Doelstellingen verwijderen

U kunt doelstellingen schrappen die niet meer of zou nooit relevant kunnen zijn.

* [&#x200B; Overwegingen wanneer het schrappen van doelstellingen &#x200B;](#considerations-when-deleting-goals)
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

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Delete**.

   ![Delete goal](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

{{step1-to-goals}}

De vertoningen van de doellijst.

1. Klik op de naam van een doel. Hierdoor wordt de doelpagina geopend.
1. Klik het **Meer** menu ![&#x200B; Meer pictogram &#x200B;](assets/more-icon.png) aan het recht van de doelnaam, dan klik **Goal van de Schrapping**, toen **Schrapping**.

   Het doel en de activiteiten en resultaten ervan worden eveneens geschrapt en kunnen niet worden teruggevorderd. De projecten die met het doel of de kinddoelstellingen werden geassocieerd worden niet geschrapt.


