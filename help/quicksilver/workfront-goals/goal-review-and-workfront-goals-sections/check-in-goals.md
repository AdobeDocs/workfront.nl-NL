---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Voortgang van Adobe Workfront-doelen bijwerken
description: U moet uw doelstellingen periodiek herzien en hun vooruitgang bijwerken om ervoor te zorgen dat zij niet achterblijven of het risico lopen niet te worden bereikt.
author: Alina
feature: Workfront Goals
exl-id: 5092f508-e52c-4934-a8c1-d0be04ecce13
source-git-commit: a64f6e507d74201cba1455fbbc6af77c2b7ba058
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# Voortgang van Adobe Workfront-doelen bijwerken

<!-- Audited for P&P only: 4/2025-->

U moet uw doelstellingen periodiek herzien en hun vooruitgang bijwerken om ervoor te zorgen dat zij niet achterblijven of het risico lopen niet te worden bereikt.

<!--And: take this last sentence ^^ out when you update this for goal redesign production.-->

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
 <p>Huidige licentie: aanvragen of hoger</p> <p>Voor meer informatie, zie <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref"> het vergunningsoverzicht van Adobe Workfront </a>.</p> </td>
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
 <td> <p>Toegang tot doelen bewerken</p></td>
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

+++

## Vereisten

U moet een actief doel hebben alvorens u kunt beginnen.

U kunt geen vooruitgang op doelstellingen bijwerken die concepten, inactief, of gesloten zijn.

## Overwegingen voor het bijwerken van doelstellingen

Houd rekening met het volgende wanneer u de voortgang op het gebied van doelstellingen bijwerkt:

* Met Workfront-doelen wordt automatisch de voortgang van een doel berekend wanneer u de voortgang van de voortgangsindicatoren bijwerkt.

  >[!TIP]
  >
  >U kunt de voortgang van een doel niet rechtstreeks bijwerken. U moet de vooruitgang van de voortgangsindicatoren van het doel (activiteiten, resultaten, verwante projecten) bijwerken die op hun beurt de voortgang van het doel bijwerken. Als u de voortgang van projecten wilt bijwerken, moet u de taken voor het project bijwerken.

  Zie ook de volgende artikelen:

   * Voor informatie over het toevoegen van activiteiten aan doelstellingen, zie [ activiteiten aan doelstellingen in de Doelen van Adobe Workfront ](../../workfront-goals/results-and-activities/add-activities-to-goals.md) toevoegen.
   * Voor informatie over het toevoegen van resultaten aan doelstellingen, zie [ resultaten aan doelstellingen in de Doelen van Adobe Workfront ](../../workfront-goals/results-and-activities/add-results-to-goals.md) toevoegen.
   * Voor informatie over hoe de Doelen van Workfront de vooruitgang op een doel berekent, zie [ Overzicht van doelvooruitgang en voorwaarde in de Doelen van Adobe Workfront ](../../workfront-goals/goal-management/calculate-goal-progress.md).

* U moet doelen maken en deze activeren voordat u de voortgang kunt bijwerken.

  Zie ook de volgende artikelen:

   * Voor informatie over het creëren van doelstellingen, zie [ doelstellingen in de Doelen van Adobe Workfront ](../../workfront-goals/goal-management/create-goals.md) creëren.
   * Voor informatie over het activeren van doelstellingen, zie [ doelstellingen in de Doelen van Adobe Workfront ](../../workfront-goals/goal-management/activate-goals.md) activeren.

  >[!IMPORTANT]
  >
  >U kunt de vooruitgang van doelstellingen niet bijwerken die worden opgesteld, gesloten, of inactief.

* De eerste keer dat u of iemand anders de voortgang van een resultaat of activiteit op een doel bijwerkt, worden de wijzigingen in de voortgang van het doel ten opzichte van New en Workfront Goals gestart met het vastleggen van de voortgang en updates van de voortgangsstatus op het doel.

<!--

## Update goal progress by using Check-in in the Production environment

>[!IMPORTANT]
>
> <span class="preview"> The Check-in functionality has been removed from the Preview environment and will be removed from Workfront Goals with the 23.1 release. See the [Update goal progress in the Preview environment](#update-goal-progress-in-the-preview-environment) section in this article to update goal progress in Preview. </span>


You can check in on goals at the individual goal level, or you can check in on multiple goals from the Check-in section of Workfront Goals.

* [Update individual goals](#update-individual-goals) 
* [Update goals in the Check-in section](#update-goals-in-the-check-in-section)

### Update individual goals {#update-individual-goals}

When you check in on a goal at the goal level, you can update the progress of the results and activities that are assigned to you or other users.

For information about how to update additional information about results and activities, see [Edit results and activities in Adobe Workfront Goals](../../workfront-goals/results-and-activities/edit-results-and-activities.md).

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area.

   All goals display by default. 

1. (Optional) Click any of the following sections in the left panel to access a list of goals:

   * Goal Alignment 
   * Pulse 
   * Check-in

   Or

   From the Goal List, click the name of a goal to open the **Goal Details** panel on the right.

   >[!TIP]
   >
   >You must have Edit access to Goals in your Access Level to view the Check-in section or the Check in button.

1. Click **Check in**.

   ![Check in link](assets/check-in-link-inside-goal-details-highlighted-350x156.png)

   The progress of results and activities becomes editable.

1. Update the current progress on each of the results. Depending on what type of result you selected, you can do one of the following:

   * Update the quantity 
   * Update the currency amount
   * Update the percent complete

1. Update the percent complete on the Manual progress bar activity.

   >[!TIP]
   >
   >When you add projects as activities to your goals, you cannot manually update projects at the goal level. Workfront automatically updates project progress based on the project of their tasks. When the project percent complete updates in Workfront, the goal progress associated with the project also updates automatically.

1. Click **Back to Summary** to return to the Goal Details panel.

   Your goal progress updates as you update the results and activities of your goal. 

1. Click the **X icon** in the upper-right corner of the Goal Details panel to close it.

### Update goals in the Check-in section {#update-goals-in-the-check-in-section}

You can use the Check-in section to check in on goals when you want to quickly provide updates for several goals at the same time.

>[!TIP]
>
>You can access the Check-in section from any of the following sections:
>
>* Goal List 
>* Goal Alignment 
>* Pulse 
>

When you check in on a goal in the Check-in section, you can update the progress of the results and activities that are assigned only to you. You cannot update the progress of results and activities that are assigned to other users in this section.

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List section displays by default. 

1. Click Check-in in the left panel.

   Or

   (Conditional) If you are in the Goal List, Goal Alignment, or Pulse sections, click the **Check in** button in the upper-right of the screen. This opens the Check-in section.

   ![Check in button](assets/check-in-button-highlighted-350x102.png)

   Goals display in a list and results and activities are listed under each goal.

   ![Check in page](assets/check-in-page-with-show-all-aligned-goals-link-350x178.png)

1. (Optional) Click **Show all results**, **Show all activities**, or **Show all aligned goals** to the far right of the goal name to display all results, activities, and aligned goals of a goal whose progress you want to update.

   >[!CAUTION]
   >
   >You cannot directly update aligned goals, but you can update their results and activities.

1. Update the current progress on each of the results assigned to you. Depending on what type of result you selected, you can do one of the following:

   * Update the quantity 
   * Update the currency amount
   * Update the percent complete

   The result and the goal progress updated automatically and you receive a confirmation of your changes.

1. Update the percent complete on your Manual progress bar activity.

   >[!TIP]
   >
   >When you add projects as activities to your goals, you cannot manually update projects at the goal level. Workfront automatically updates project progress based on the project of their tasks. When the project percent complete updates in Workfront, the goal progress associated with the project also updates automatically.

   The activity and the goal progress updated automatically and you receive a confirmation of your changes.

1. (Optional) Add a comment for your goal, then click **Post** to save your comment.

-->

Voortgang van doelen bijwerken:

1. Klik het **pictogram van het 1} pictogram van het Belangrijkste Menu ![ ](assets/main-menu-icon.png) >** Doelen **in de hoger-juiste hoek.**

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Hierdoor wordt de lijst met doelen geopend. Alle doelstellingen die u toegang tot meningsvertoning door gebrek hebt.

   U kunt ook in het linkerdeelvenster op Uitlijning van doel klikken.

1. Klik in de lijst met doelen op de naam van een doel om de doelpagina te openen.
1. Klik **indicatoren van de Voortgang** in het linkerpaneel.

   In de lijst Voortgangsindicatoren worden alle voortgangsindicatoren weergegeven voor het doel dat u hebt geselecteerd.

   >[!NOTE]
   >
   >  * U kunt alleen resultaten en activiteiten bijwerken.
   >  * U moet de voortgangsindicatoren van de doelstellingen van kinderen bijwerken om vooruitgang op de doelstellingen van de kinderen te tonen.
   >  * U moet de taken op de verbonden projecten bijwerken om vooruitgang op de projecten te tonen.
   >   
   >    De vooruitgang van de kinderdoelen en de voortgang van de projecten leiden op hun beurt tot de voortgang van het geselecteerde doel.


1. Om de vooruitgang van een resultaat of een activiteit bij te werken, klik de waarde binnen de **Ware kolom van de Voortgang** van het resultaat of de activiteit en typ een aantal om zijn waarde bij te werken, dan druk binnengaan.

   ![ Ware vooruitgang ](assets/actual-progress-result-updating-highlighted-unshimmed.png)

   De voortgangsbalk voor de voortgangsindicator in de kolom Voortgang en de voortgang van het doel in de doelkoptekst worden direct bijgewerkt.

