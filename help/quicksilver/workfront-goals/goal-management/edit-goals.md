---
product-previous: workfront-goals
navigation-topic: goal-management
title: Doelen in Adobe Workfront-doelen bewerken
description: U kunt bestaande doelen op elk gewenst moment en in elke gewenste status bewerken.
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Doelen in Adobe Workfront-doelen bewerken

<!--Audited for P&P only: 10/2025-->

U kunt bestaande doelen op elk gewenst moment en in elke gewenste status bewerken.

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

## Overwegingen bij het bewerken van doelen

* U kunt doelen met de status Gesloten niet bewerken.
* U kunt doelstellingen op elk gewenst moment bewerken.

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
1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Edit**.

   ![Edit goal](assets/edit-goal-highlighted.png)

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

{{step1-to-goals}}

Er wordt een lijst met doelen weergegeven.

1. Klik op een doel.\
   De doelpagina wordt weergegeven.

   ![&#x200B; Goal pagina &#x200B;](assets/goal-page-unshimmed.png)

1. Voer een van de volgende handelingen uit om informatie voor het doel te bewerken:
   * Klik op velden die in de doelkoptekst worden weergegeven om deze bij te werken. Niet alle velden in de koptekst kunnen worden bewerkt.
   * Klik het **Meer pictogram** ![&#x200B; Meer pictogram &#x200B;](assets/more-icon.png) aan het recht van de doelnaam, dan klik **uitgeven**.
   * Klik **Goele details** in het linkerpaneel en klik **uitgeven pictogram** ![&#x200B; uitgeven pictogram &#x200B;](assets/edit-icon.png) in de hoger-juiste hoek, dan klik **allen** uitgeven. Start met het bijwerken van velden in de sectie Goal details.

     >[!IMPORTANT]
     >
     >Niet alle velden die in de hierboven vermelde gebieden worden weergegeven, kunnen worden bewerkt. Workfront berekent een aantal velden en deze zijn alleen-lezen.

1. (Voorwaardelijk) Afhankelijk van wat u in de vorige stap selecteerde, werk de volgende informatie over het doel bij:

   * Werk de volgende informatie in de doelkopbal bij, dan druk binnengaan om uw veranderingen te bewaren:
      * **Goal naam**: Klik de naam van het doel en begin een nieuwe naam te typen.
      * **Eigenaar**: Klik de naam van de eigenaar, en begin de naam van een gebruiker, een team, een groep, of uw bedrijf te typen, dan het te selecteren wanneer het in de lijst toont. U kunt slechts één eigenaar voor een doel hebben.
   * Werk de volgende informatie in het Edit vakje van het Doel bij, dan klik **sparen**:
      * **Goal name**
      * **Periode**: Klik om de tijdspanne voor het doel bij te werken\
        of\
        Selecteer **douanedata** toelaten om data voor het 2&rbrace; Begin van het doel **en** Eind data **te specificeren.**

        >[!TIP]
        >
        >Deselecteer **douanedata** toelaten om op de originele tijdspanne voor het doel terug te keren.

      * **Goal owner**
      * **Beschrijving**: Voeg of werk informatie over het doel toe bij.
   * Werk of herzie informatie in de sectie van de Details van het Doel bij. Voor meer informatie, zie [&#x200B; doelstellingen van de Update in de sectie van de Details van het Doel in de Doelen van Adobe Workfront &#x200B;](../goal-management/update-goals-in-goal-details-panel.md).

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. (Facultatief) klik **Indicatoren van de Voortgang** in het linkerpaneel om resultaten, activiteiten, of projecten aan het doel toe te voegen. Door voortgangsindicatoren toe te voegen, kunt u de voortgang van het doel volgen.
Raadpleeg de volgende artikelen voor meer informatie:
   * [Activiteiten toevoegen aan doelen in Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   * [&#x200B; voeg resultaten aan doelstellingen in de Doelen van Adobe Workfront toe &#x200B;](../results-and-activities/add-results-to-goals.md).
   * [&#x200B; voeg projecten aan doelstellingen in de Doelen van Adobe Workfront &#x200B;](../results-and-activities/connect-projects-to-goals-overview.md) toe.

</div>
