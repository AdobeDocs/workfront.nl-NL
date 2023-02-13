---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Grafieken bekijken om trends in de voortgang van het doel in Adobe Workfront-doelen te begrijpen
description: U kunt de algemene gezondheid van uw doelstellingen en hun vooruitgangstendens in tijd in de sectie van Grafieken van de Doelen van Adobe Workfront bekijken. De grafieken in deze sectie breken niet de vooruitgang van elk doel af, maar geven u in plaats daarvan een holistische momentopname van de de vooruitgangsstatus van alle doelstellingen evenals hun vooruitgangstendens in tijd tijdens een gespecificeerde periode.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 3989903687f2ea64ebd5ad754119ce1a9d70b9f3
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# Grafieken bekijken om trends in de voortgang van het doel in Adobe Workfront-doelen te begrijpen

<!-- drafted mostly for P&P release-->

U kunt de algemene gezondheid van uw doelstellingen en hun vooruitgangstendens in tijd in de sectie van Grafieken van de Doelen van Adobe Workfront bekijken. De grafieken in deze sectie breken niet de vooruitgang van elk doel af, maar geven u in plaats daarvan een holistische momentopname van de de vooruitgangsstatus van alle doelstellingen evenals hun vooruitgangstendens in tijd tijdens een gespecificeerde periode.

>[!IMPORTANT]
>
>U kunt een totaal aantal voor uw doelstellingen in de sectie van Grafieken voor een geselecteerde periode zien. Nochtans, neemt de Doelen van Workfront slechts doelstellingen met een status van Actief en Gesloten in aanmerking wanneer het berekenen van de algemene status van de doelvooruitgang en het percentage voltooide.

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

U moet de volgende toegang hebben om de handelingen uit te voeren die in dit artikel worden beschreven:

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
   <td role="rowheader">Toegangsniveau*</td> 
   <td> <p>Toegang tot doelen weergeven of vergroten</p> <p><b>OPMERKING</b><p>Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Toegang tot Adobe Workfront-doelen verlenen</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> 
    <div> 
     <p>De toestemmingen van de mening of hoger op doelstellingen</p> 
     <p>Voor informatie over het delen van doelstellingen, zie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Een doel delen in Workfront-doelen</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Vereisten

U moet het volgende hebben voordat u kunt beginnen:

* Een lay-outsjabloon die het gebied Doelen in het hoofdmenu bevat.

## Typen grafieken in Workfront-doelen

De volgende grafieken zijn beschikbaar in de sectie Grafieken of de Doelen van Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">The Goal Health Chart</td> 
   <td> <p>Een diagram dat het volgende weergeeft:</p> 
    <ul> 
     <li>Een totaal aantal doelstellingen voor de geselecteerde periode. Er wordt rekening gehouden met doelstellingen met elke status. </li> 
     <li>De voortgangsstatus van doelen met de status Actief en Gesloten.</li> 
    </ul> <p>Ga voor informatie over hoe Workfront Goals de status van progress berekent naar <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Overzicht van de voortgang en conditie van het doel in de Adobe Workfront-doelstellingen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">The Goal Progress Chart</td> 
   <td> <p>Een lijngrafiek die updates toont die aan doelstellingen in wekelijkse toename tijdens de duur van het doel worden gemaakt. In het voortgangsdiagram voor het doel wordt het volgende weergegeven:</p> 
    <ul> 
     <li>Een gemiddeld verwacht en werkelijk percentage volledig van alle actieve en gesloten doelstellingen in de geselecteerde periode. Het percentage van de volledige voortgang wordt opgesplitst in wekelijkse stappen gemarkeerd door knooppunten. </li> 
     <li>Het totale gemiddelde percentage vorderingen voor actieve en afgeronde doelstellingen sinds de vorige week. </li> 
    </ul> <p>Tip: Het overzicht van de doelvooruitgang zou geen informatie kunnen tonen wanneer de updates over de doelstellingen buiten de geselecteerde tijdspanne worden gemaakt. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Voortgang van doel van grafieken controleren

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) > **Doelen** in de rechterbovenhoek.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Dit opent het gebied van de Doelen van Workfront.

1. Klikken **Grafieken** in het linkerdeelvenster.

   ![](assets/graphs-in-left-panel.png)

   De sectie Grafieken wordt weergegeven.

   Standaard worden de doelstellingen in de sectie Grafieken beperkt door de volgende criteria:

   * De filters die op het gebied van Grafieken worden toegepast.
   * De doelstellingen die in een status van Actief en Ontwerp zijn.

1. (Optioneel) Selecteer het type informatie dat u wilt weergeven door de filters in de rechterbovenhoek van de sectie Grafieken bij te werken.

   Voor meer informatie over het filtreren van doelstellingen, zie [Gegevens filteren in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   Als u ervoor hebt gekozen om meer dan één tijdsperiode weer te geven, wordt voor elke tijdsperiode een gezondheidgrafiek (gauge) en een voortgangsgrafiek (lijn) weergegeven.

1. Bekijk de informatie in de onderstaande tabel wanneer u de Goal Health Chart bekijkt.

   ![](assets/gauge-graph-wf-align-350x230.png)

   | Totaal aantal doelstellingen | Het getal onder aan het diagram geeft het aantal doelen in de geselecteerde periode aan, in alle statussen die u hebt geselecteerd. |
   |---|---|
   | Gemiddeld percentage voltooid | Bij de bovenkant van de grafiek, wijst dit aantal op het gemiddelde percentage volledige van actieve en gesloten doelstellingen in de geselecteerde tijdspanne. |
   | Doelstellingen en vorderingen | Het aantal doelstellingen voor elk segment van de vooruitgangsstatus, wanneer u over de segmenten van de grafiek beweegt. Alleen doelen in een status Actief of Gesloten worden geteld in de segmenten. |


1. Bekijk de informatie in de onderstaande tabel wanneer u de grafiek van de voortgang van het beleid bekijkt.

   ![](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Voortgang van basislijn</td> 
      <td>De groene hellingslijn wijst op het verwachte algemene percentage volledige gemiddelde van actieve en gesloten doelstellingen voor de geselecteerde tijdspanne. Alle doelstellingen binnen een periode worden verwacht te voltooien, zodat is de basisvooruitgang altijd 100% aan het eind van de periode. </td> 
     </tr> 
     <tr> 
      <td>Werkelijke vooruitgang</td> 
      <td> <p>De blauwe lijn geeft het daadwerkelijke totale percentage aan van het volledige gemiddelde van actieve en gesloten doelen voor de geselecteerde tijdsperiode in wekelijkse stappen. Elke week tijdens de duur van het doel wordt duidelijk door een knoop in de lijn. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Houd een weekknooppunt boven in het voortgangsdiagram voor het doel en bekijk het volgende:

   * **Weekdatum**: De maand, de dag en het jaar van de geselecteerde week.
   * **Voortgang**: Een gemiddelde van het daadwerkelijke percentage voltooide van alle doelstellingen voor de geselecteerde week.
   * **Basislijn**: Een gemiddelde van het verwachte percentage voltooide van alle doelstellingen voor de geselecteerde week.

1. (Optioneel) Klik op **Voortgang** onder aan het voortgangsdiagram om de huidige algemene voortgangslijn te verwijderen

   of

   Klikken **Basislijn** onder aan het voortgangsdiagram om de verwachte voortgang uit het diagram te verwijderen.

 
