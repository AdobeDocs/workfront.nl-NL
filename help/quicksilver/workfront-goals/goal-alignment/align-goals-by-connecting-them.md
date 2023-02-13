---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Richt doelstellingen door hen in de Doelen van Adobe Workfront te verbinden
description: Als u een individuele medewerker bent die een persoonlijk doel heeft, kunt u het aan de doelstellingen van uw team willen richten om de vooruitgang van uw eigen doel in de grotere context van de strategie van uw organisatie effectief te tonen.
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# Richt doelstellingen door hen in de Doelen van Adobe Workfront te verbinden


Als u een individuele medewerker bent die een persoonlijk doel heeft, kunt u het aan de doelstellingen van uw team willen richten om de vooruitgang van uw eigen doel in de grotere context van de strategie van uw organisatie effectief te tonen.

Wanneer iedereen in uw organisatie hun doelstellingen heeft die aan de doelstellingen van uw organisatie worden gericht, kunnen zij duidelijk zien hoe hun individuele bijdragen en teaminspanningen helpen om de naald op grotere, bedrijf-vlakke prioriteiten vooruit te bewegen. Voor meer informatie over de beste praktijken voor het richten van doelstellingen, zie [Overzicht van uitlijning van doelstellingen in Adobe Workfront](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

Er zijn twee manieren om doelen te verbinden in Adobe Workfront Goals:

* U kunt groepering tussen doelstellingen tot stand brengen door doelstellingen met elkaar te verbinden.

* U kunt twee doelstellingen manueel richten of u kunt resultaten en activiteiten van een bestaand doel in een ander doel omzetten. Het omgezette resultaat of de omgezette activiteit wordt het kinddoel van het originele doel.

>[!IMPORTANT]
>
>Een doel kan in totaal 1000 voortgangsindicatoren hebben.

In dit artikel wordt beschreven hoe u doelen kunt uitlijnen door ze met elkaar te verbinden. Voor informatie over het richten van doelstellingen door resultaten en activiteiten in doelstellingen om te zetten, zie [Richt doelstellingen door resultaten en activiteiten aan doelstellingen om te zetten](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

## Toegangsvereisten

<!--drfated for the P&P release: 

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
   <td> <p>Toegang tot doelen bewerken</p> <p><b>OPMERKING</b>

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

## Richt doelstellingen door hen met elkaar te verbinden

<!--
Aligning goals by connecting them differs depending on what environment you use. 

### Align goals by connecting them in the Production environment

1. Create two goals that you want to align. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Activate the goals that you want to align. You can align goals that have a Draft, Active, or Inactive status. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Go to the goal that you want to align (child goal) to another goal (parent goal) and click its name to open the **Goal Details** panel.

   For example, if you want Goal 2 to influence the progress of Goal 1, you must go to Goal 2. 

1. Click **Align to another goal** in the upper-right corner of the right panel.

   ![](assets/align-to-another-goal-link-highlighted-350x128.png)

1. Start typing the name of an existing goal or the name of an owner in the **Align to another goal** field, then select it when it appears in the list. Only goals that are from the same or future periods display in the list. 
1. Click **Save**.

   The goal you started with (Goal 2) is now the child goal of the goal you aligned it with (Goal 1).   
   The aligned goals display connected in the Goal Alignment section with Goal 2 as secondary to Goal 1.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) To view the goals in the Goal Alignment section, do one of the following:

   * Click the Goal Alignment section in the left panel and find the goals by applying the correct filter. For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).
   * Click the Goal List, Check-in, or Pulse sections in the left panel and find one of the goals, then click the **Alignment icon** ![](assets/align-icon.png) next to the goal name to go directly to the goal in the Goal Alignment section.

   For information about the Goal Alignment section, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md). 

1. (Optional) Add activities and results to either goal to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Remove the alignment between two goals, when you consider that no longer is relevant to your organization's overall strategy For information about removing alignment between goals, see [Remove goal alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

-->
1. Maak twee doelen die u wilt uitlijnen. Voor informatie over het creëren van doelstellingen, zie [Doelen maken voor Adobe Workfront-doelen](../../workfront-goals/goal-management/create-goals.md).
1. (Optioneel) Activeer de doelen die u wilt uitlijnen. U kunt doelstellingen richten die een Ontwerp, Actief, of Inactieve status hebben. Voor informatie over het activeren van doelstellingen, zie [Doelen in Adobe Workfront-doelen activeren](../../workfront-goals/goal-management/activate-goals.md).
1. Ga naar het doel dat u (kinddoel) aan een ander doel (ouderdoel) wilt richten en zijn naam klikken om de doelpagina te openen.

   >[!INFO]
   >
   >Als u bijvoorbeeld wilt dat doelstelling 2 de voortgang van doelstelling 1 beïnvloedt, moet u naar doelstelling 2 gaan.

1. Klikken **Goederendetails** in het linkerdeelvenster.

1. In de **Informatie over bovenliggende doelen** gebied, klikken **Toevoegen** in de **Bovenliggende doelstelling** veld indien er geen hoofddoel is;

   of

   Klik op de naam van het bovenliggende doel om een ander doel te kiezen.

1. Begin de naam van een bestaand doel in te typen **Bovenliggende doelstelling** en selecteert u deze wanneer deze in de lijst wordt weergegeven. Alleen doelen die afkomstig zijn van dezelfde of toekomstige perioden worden weergegeven in de lijst.

1. Klikken **Wijzigingen opslaan**.

   Het doel waarmee u bent begonnen (doelstelling 2) is nu het onderliggende doel van het bovenliggende doel waarmee u het hebt uitgelijnd (doelstelling 1).\
   De uitgelijnde doelweergave die is verbonden in de sectie Goal Alignment met doelstelling 2 als secundair aan doelstelling 1.
Het kinddoel toont in de de indicatorensectie van de Voortgang van het ouderdoel aangezien zijn vooruitgang de vooruitgang van het ouderdoel bijwerkt.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optioneel) Als u de doelen wilt weergeven in het gedeelte Doeluitlijning van Workfront, gaat u naar het gebied Doelen en klikt u op de knop **Goal Alignment** in het linkerdeelvenster. Voor informatie over de sectie van de Groepering van het Beleid, zie [Navigeren in de sectie Goal Alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. (Optioneel) Voeg activiteiten en resultaten toe aan beide doelen om de voortgang ervan aan te geven. Raadpleeg de volgende artikelen voor informatie over het toevoegen van activiteiten en resultaten:

   * [Activiteiten toevoegen aan doelen in Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Resultaten toevoegen aan doelen in Adobe Workfront-doelen](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optioneel) Verwijder de uitlijning tussen twee doelen wanneer u van mening bent dat deze niet langer relevant zijn voor de algemene strategie van uw organisatie. Voor informatie over het verwijderen van groepering tussen doelstellingen, zie [Doeluitlijning van Adobe Workfront-doelen verwijderen](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

