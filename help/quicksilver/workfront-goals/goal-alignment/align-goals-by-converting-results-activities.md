---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Richt doelstellingen door resultaten en activiteiten aan doelstellingen om te zetten
description: U kunt twee doelstellingen manueel richten of u kunt de resultaten en de activiteiten van een bestaand doel in een ander doel omzetten. Het omgezette resultaat of de omgezette activiteit wordt het kinddoel van het originele doel. Voor informatie over het manueel richten van twee doelstellingen, zie richten doelstellingen door hen in de Doelen van Adobe Workfront aan te sluiten.
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Richt doelstellingen door resultaten en activiteiten aan doelstellingen om te zetten

U kunt twee doelstellingen manueel richten of u kunt de resultaten en de activiteiten van een bestaand doel in een ander doel omzetten. Het omgezette resultaat of de omgezette activiteit wordt het kinddoel van het originele doel.
Voor informatie over het manueel richten van twee doelstellingen, zie [Richt doelstellingen door hen in de Doelen van Adobe Workfront te verbinden](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Toegangsvereisten


<!--drafted for P&P release: 

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
* Een bestaand doel met bestaande resultaten en activiteiten.

   Voor informatie over het creëren van doelstellingen, zie [Doelen maken voor Adobe Workfront-doelen](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Een doel kan tot 1000 voortgangsindicatoren hebben.

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## Overwegingen bij het omzetten van resultaten en activiteiten in doelen

Soms kan een resultaat of een activiteit een grotere reikwijdte hebben dan verwacht en het zou meer zin hebben dat ze doelstellingen worden. U kunt resultaten en activiteiten van een bestaand doel omzetten in een nieuw doel. Dit is een bottom-up benadering van het richten van doelstellingen.

Overweeg het volgende wanneer het omzetten van resultaten en activiteiten in doelstellingen:

* Het omgezette resultaat of de omgezette activiteit wordt het kinddoel van het oorspronkelijke doel, en de twee doelstellingen worden gericht.
* Het nieuwe doel wordt de enige voortgangsindicator voor het oorspronkelijke doel, als er geen extra resultaten of activiteiten op het oorspronkelijke doel zijn. U moet resultaten en activiteiten aan het kinddoel toevoegen om vooruitgang op het te kunnen volgen.
* Het omzetten van een resultaat of activiteit in een doel is onomkeerbaar. Na omgezette, kan het nieuwe kinddoel nooit een resultaat of activiteit voor het ouderdoel opnieuw worden.

## Een resultaat of activiteit omzetten in een doel

<!--
<span class="preview">Converting results and activities differs depending on what environment you use. </span>

### Convert a result or activity to a goal in the Production environment

1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the **Goal Details** panel.
1. Expand the **Results** or **Activities** right-pointing arrows to see a list of results or activities for the goal. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. Ga naar een doel dat een resultaat of een activiteit heeft die u in een doel wilt omzetten.
1. Klik op de doelpagina op **Voortgangsindicatoren** in het linkerdeelvenster.
1. Selecteer een resultaat of activiteit in de lijst met voortgangsindicatoren en klik op de knop **Omzetten in doel** pictogram ![](assets/convert-to-goal-icon-unshimmed.png) boven aan de lijst van voortgangsindicatoren. Het vak Omzetten in doel wordt geopend.

   ![](assets/convert-to-goal-box-unshimmed.png)
1. Werk de volgende gegevens bij:
   * **Goederennaam**: Standaard heeft het nieuwe doel dezelfde naam als het oorspronkelijke resultaat of de oorspronkelijke activiteit.
   * **Periode**: Standaard is de periode van het nieuwe doel het huidige kwartaal. U kunt de **Aangepaste datums inschakelen** het plaatsen om een periode van de douanetijd voor het nieuwe doel te bepalen.
   * **Goedereneigenaar**: Door gebrek, is de nieuwe doeleigenaar de eigenaar van het originele resultaat of de activiteit.
   * **Beschrijving**: Meer informatie over het nieuwe doel toevoegen.
1. Klikken **Opslaan**

   Het resultaat of de activiteit wordt nu omgezet in een kinddoel van het originele doel. Het wordt vermeld als doel in de lijst van voortgangsindicatoren van het oorspronkelijke doel.



