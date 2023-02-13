---
product-previous: workfront-goals
navigation-topic: goal-management
title: Herzie in-probleem doelstellingen in de Doelen van Adobe Workfront
description: Olijven met een Progress of In Trouble dreigen niet te worden bereikt en worden in Adobe Workfront Goals weergegeven door een rode voortgangsbalk. U moet uw doelstellingen vaak herzien en begrijpen waarom de vooruitgang achterloopt.
author: Alina
feature: Workfront Goals
exl-id: df2cdc12-9102-4759-9daa-1f8ae68f110b
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Herzie in-probleem doelstellingen in de Doelen van Adobe Workfront

<!--
<p>(NOTE: the status of goals in "red" used to be called At Risk. Now, it is "in trouble") </p>
-->

Doelen met een vooruitgang in de problemen dreigen niet te worden verwezenlijkt en worden in de doelstellingen van Adobe Workfront weergegeven door een rode voortgangsbalk. U moet uw doelstellingen vaak herzien en begrijpen waarom de vooruitgang achterloopt. Voor informatie over de voortgang van het doel raadpleegt u [Overzicht van de voortgang en conditie van het doel in de Adobe Workfront-doelstellingen](../../workfront-goals/goal-management/calculate-goal-progress.md).

## Toegangsvereisten

<!--drafted for P&P release: replace the existing requirements with this:

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
   <td> <p>Toegang tot doelen of hoger bewerken</p> <p><b>OPMERKING</b><p>Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie:</p> 
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

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

U moet het volgende hebben voordat u kunt beginnen:

* Een lay-outsjabloon die het gebied Doelen in het hoofdmenu bevat.

## Recommendations voor het voorkomen van doelen om vooruitgang te boeken in Problemen

Voordat de doelstellingen een stap voorwaarts in Problemen bereiken, kunt u ze vaak volgen en de voortgang ervan aanpassen wanneer ze een voortgang in Bij risico bereiken. Doelen die gevaar lopen, dreigen in de problemen te raken. Zie voor meer informatie over de voortgang van het doel [Overzicht van de voortgang en conditie van het doel in de Adobe Workfront-doelstellingen](../../workfront-goals/goal-management/calculate-goal-progress.md)

Voordat uw doelstellingen een stap verder gaan in Problemen, raden we het volgende aan:

* De doelstellingen van het overzicht die een voorwaarde van Op Risico vaak zijn die aan u evenals organisatorische doelstellingen worden toegewezen die aan uw teams, groepen, of aan uw organisatie worden toegewezen die door de vooruitgang van uw doelstellingen zouden kunnen worden beïnvloed. Risicodoelen dreigen in de problemen te raken. De risicodoelstellingen worden gemarkeerd met een gele voortgangsbalk. Gebruik de Lijst van het Doel om doelstellingen te bekijken die tot u, uw teams, groepen, of uw organisatie behoren.


## Herzie in-probleemdoelstellingen in de Lijst van het Doel

U kunt doelstellingen in om het even welk gedeelte van de Doelen van Workfront herzien. Zie voor meer informatie over de secties Workfront Goals [Overzicht van de secties Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

Dit artikel beschrijft hoe te om doelstellingen in de Lijst van het Beleid te herzien.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) > **Doelen** in de rechterbovenhoek.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Hiermee opent u standaard het gebied Workfront Goals en de sectie Goal List.

1. (Aanbevolen) Pas de volgende filters voor het gebied van de Lijst van het Beleid aan overzicht bij risicodoelstellingen:

   * Klikken **Bedrijf** vervolgens **Mijn teams** vervolgens **Mijn groepen** vervolgens **Persoonlijk** doelstellingen in deze orde om doelstellingen te bekijken die tot uw organisatie, uw teams, groepen, en toen uw eigen doelstellingen behoren.

      >[!TIP]
      >
      >In de Doelen van Adobe Workfront, toont de filter van het Bedrijf de doelstellingen waarvoor uw organisatie als eigenaar wordt geselecteerd.
      >
      >
      >U kunt niet zoeken naar bedrijven die dit veld gebruiken. Alleen uw organisatie die eigenaar is van uw Workfront-exemplaar is standaard geselecteerd.

   * Voor elk van de organisatorische eenheden die u hierboven selecteert, klikt u op **Nieuw filter** > **Voortgang** > **In problemen** >**Toepassen.**
   * (Optioneel) Selecteer de periode waarvoor u de doelen wilt weergeven.

      De indicator van de vooruitgangsbar toont in rood voor elk doel in de doellijst.

      Voor meer informatie over het filtreren van doelstellingen die alle andere criteria in het juiste paneel gebruiken, zie [Gegevens filteren in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. Houd de cursor boven de voortgangsbalkindicator om te zien wat het werkelijke voortgangspercentage is en wat de verwachte waarde voor de huidige dag is.

   ![](assets/goal-progress-hover-over-detail-unshimmed.png)

1. (Optioneel) Gebruik de filters om doelen te zoeken die bij een specifieke eigenaar horen.

   De doelstellingen van in-probleem voor de geselecteerde gebruikers tonen in de doellijst.

1. Klik op de naam van een doel om de doelpagina te openen en klik vervolgens op **Voortgangsindicatoren** in het linkerdeelvenster. Bekijk welke voortgangsindicator ervoor zorgt dat het doel achterblijft en werk de voortgang van de indicator inline bij in het dialoogvenster **Werkelijke vooruitgang** kolom van de lijst van voortgangsindicatoren.

   Voor informatie over het bijwerken van resultaten en activiteiten raadpleegt u [Voortgang van Adobe Workfront-doelen bijwerken](../goal-review-and-workfront-goals-sections/check-in-goals.md)

   ![](assets/actual-progress-editable-column-in-indicator-list-unshimmed.png)

   >[!NOTE]
   >
   >U kunt alleen resultaten en activiteiten bijwerken in de lijst Voortgangsindicatoren. U moet de voortgangsindicatoren van kinddoelstellingen bijwerken door tot de doelstellingen toegang te hebben en u moet de taken op de verbonden projecten bijwerken om de vooruitgang van de projecten bij te werken.


