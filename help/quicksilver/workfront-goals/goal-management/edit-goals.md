---
product-previous: workfront-goals
navigation-topic: goal-management
title: Doelen in Adobe Workfront-doelen bewerken
description: U kunt bestaande doelen op elk gewenst moment en in elke gewenste status bewerken.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# Doelen in Adobe Workfront-doelen bewerken

U kunt bestaande doelen op elk gewenst moment en in elke gewenste status bewerken.

## Toegangsvereisten

<!--drafted - for P&P releases: 

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

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Vereisten

U moet het volgende hebben voordat u kunt beginnen:

* Een lay-outsjabloon die het gebied Doelen in het hoofdmenu bevat.
* U hebt de doelen gemaakt die u wilt bewerken of u hebt beheermachtigingen voor deze doelen.

## Overwegingen bij het bewerken van doelen

* U kunt doelen met de status Gesloten niet bewerken.
* U kunt doelstellingen van om het even welke tijdspanne uitgeven.

   U kunt de volgende informatie voor een vorig doel uitgeven:

   * Naam
   * Tijdsperiode
   * Status

      >[!TIP]
      >
      >Als het doel is gesloten, wordt het percentage Voortgang opnieuw berekend als het opnieuw wordt geopend. U kunt een gesloten doel niet bewerken.

   * Beschrijving
   * Resultaten en activiteiten

## Doelstellingen bewerken

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![](assets/more-icon.png), then click **Edit**.

   ![](assets/edit-goal-highlighted.png)

1. Update the name of the goal in the **Goal** field. 
1. Select a time period when the goal should be completed.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a start and an end date for your goal, if you clicked **Define custom dates**.

   
   <p>(NOTE: these fields don't yet have a name) </p>
   

   >[!CAUTION]
   >
   >You cannot create a goal with custom dates in the past.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same time frames for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your larger organization-wide strategy.

1. Click the **Owner** field and select a new owner for the goal, if you want to indicate someone else as the owner of the goal. 
1. (Conditional) Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. Update the **Description** of the goal, then click **Save**.

-->

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png)en klik vervolgens op **Doelen**.\
   Er wordt een lijst met doelen weergegeven.
1. Klik op een doel.\
   De doelpagina wordt weergegeven.

   ![](assets/goal-page-unshimmed.png)

1. Voer een van de volgende handelingen uit om informatie voor het doel te bewerken:
   * Klik op velden die in de doelkoptekst worden weergegeven om deze bij te werken. Niet alle velden in de koptekst kunnen worden bewerkt.
   * Klik op de knop **Meer pictogram** ![](assets/more-icon.png) rechts van de doelnaam klikt u op **Bewerken**.
   * Klikken **Goederendetails** in het linkerdeelvenster en klik op de knop **Pictogram Bewerken** ![](assets/edit-icon.png) in de rechterbovenhoek klikt u op **Alles bewerken**. Start met het bijwerken van velden in de sectie Goal details.

      >[!IMPORTANT]
      >
      >Niet alle velden die in de hierboven vermelde gebieden worden weergegeven, kunnen worden bewerkt. Workfront berekent een aantal velden en deze zijn alleen-lezen.

1. (Voorwaardelijk) Afhankelijk van wat u in de vorige stap selecteerde, werk de volgende informatie over het doel bij:

   * Werk de volgende informatie in de doelkopbal bij, dan druk binnengaan om uw veranderingen te bewaren:
      * **Goederennaam**: Klik op de naam van het doel en typ een nieuwe naam.
      * **Eigenaar**: Klik de naam van de eigenaar, en begin de naam van een gebruiker, een team, een groep, of uw bedrijf te typen, dan selecteer het wanneer het in de lijst toont. U kunt slechts één eigenaar voor een doel hebben.
   * Werk de volgende informatie in het Edit vakje van het Doel bij, dan klik **Opslaan**:
      * **Goederennaam**
      * **Periode**: Klik om de periode voor het doel bij te werken\
         of\
         Selecteren **Aangepaste datums inschakelen** om data voor het doel te specificeren **Start** en **Einddata**.

         >[!TIP]
         >
         >Deselecteren **Aangepaste datums inschakelen** om terug te keren naar de oorspronkelijke periode voor het doel.

      * **Goedereneigenaar**
      * **Beschrijving**: Voeg of werk informatie over het doel bij.
   * Werk of herzie informatie in de sectie van de Details van het Doel bij. Zie voor meer informatie [Doelen bijwerken in de sectie Gooddetails in Adobe Workfront Goals](../goal-management/update-goals-in-goal-details-panel.md).

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Optioneel) Klik op **Voortgangsindicatoren** in het linkerpaneel om resultaten, activiteiten, of projecten aan het doel toe te voegen. Door voortgangsindicatoren toe te voegen, kunt u de voortgang van het doel volgen.
Raadpleeg de volgende artikelen voor meer informatie:
   * [Activiteiten toevoegen aan doelen in Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   * [Resultaten toevoegen aan doelen in Adobe Workfront-doelen](../results-and-activities/add-results-to-goals.md).
   * [Projecten toevoegen aan doelen in Adobe Workfront](../results-and-activities/connect-projects-to-goals-overview.md).

</div>
