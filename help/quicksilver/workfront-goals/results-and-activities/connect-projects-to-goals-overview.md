---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Projecten toevoegen aan doelen in Adobe Workfront
description: U kunt projecten met doelstellingen verbinden om erop te wijzen hoe het doel vordert, gebaseerd op de daadwerkelijke vooruitgang van het project. Het project wordt een voortgangsindicator voor het doel.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 0%

---

# Projecten toevoegen aan doelen in Adobe Workfront

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

U kunt projecten met doelstellingen verbinden om erop te wijzen hoe het doel vordert, gebaseerd op de daadwerkelijke vooruitgang van het project. Het project wordt een voortgangsindicator voor het doel.

Door projecten aan doelstellingen te verbinden kunt u de strategische planning (doelstellingen) van uw organisatie aan het daadwerkelijke werk verbinden uw mensen uitvoeren en voltooien elke dag (projecten).

>[!IMPORTANT]
>
>Projectniveaudoelstellingen die in het gebied Bedrijfs van het Geval van een project worden gecreeerd worden niet verbonden met strategische doelstellingen die in de Doelen van Workfront worden gecreeerd. Voor informatie over de projectdoelstellingen van het BedrijfsGeval, zie [Zakelijke hoofddoelen maken](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## Toegangsvereisten

<!--drafted for P&P release: replace the table below with this: 

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

Voor meer informatie over toegang tot Workfront Goals raadpleegt u [Vereisten voor het gebruik van Workfront-doelen](../goal-management/access-needed-for-wf-goals.md).

## Overwegingen over het verbinden van projecten met doelstellingen

* U kunt een project toevoegen dat aan de volgende criteria aan een doel voldoet:

   * U moet ten minste over machtigingen beschikken om deze weer te geven.

      >[!NOTE]
      >
      >Als u uw toestemmingen verliest om het project te bekijken nadat u het project aan het doel hebt vastgemaakt, kunt u projectinformatie over het doel nog zien, maar u kunt niet meer tot het project toegang hebben.

   * Het project mag niet in de status Dode verkeren.

* U kunt veelvoudige projecten met een doel associëren.
* U kunt het zelfde project met veelvoudige doelstellingen associëren.
* U kunt niet manueel de vooruitgang van een project van het doel bijwerken dat het project aan in bijlage is. In plaats daarvan berekent Workfront het percentage van voltooiing van het project en Workfront Goals berekent de voortgang van het doel met dit percentage voltooid. Dit werkt het doel in echt bij - tijd na de updates van het projectpercentage.
* De projectduur kan buiten de tijdsperiode van een doel zijn. Als een project langer duurt dan de deadline van het doel, kunt u nog steeds uw doel sluiten en overwegen het te voltooien, maar het doel zal niet 100% zijn voltooid. Het percentage voltooide van het project wordt niet meer bijgewerkt op het doel.

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* Wanneer u een project schrapt in bijlage aan een doel, wordt het project ook geschrapt van het doel.

   >[!CAUTION]
   >
   >Als het doel actief was alvorens u het project schrapte en er geen andere vooruitgangsindicatoren op het doel zijn, wordt het doel Inactief.


## Projecten toevoegen aan doelen

1. Klik op de knop **Hoofdmenu** ![](assets/main-menu-icon.png) (stel dit voor Shell voor: of klik op **Hoofdmenu** ![](assets/three-line-main-menu-icon.png) in de linkerbovenhoek, als het beschikbaar is.) **Doelen**.
1. Klik in de lijst met doelen op de naam van een doel om de doelpagina te openen.
1. Klikken **Voortgangsindicatoren** in het linkerdeelvenster.
1. Van de **Nieuwe voortgangsindicator** vervolgkeuzelijst, klikt u op **Bestaand project toevoegen**.

   De Add projecten aan de vertoningen van het doelvakje.
1. (Optioneel) Werk de **Weergave**, **Filter**, of **Groepering** door op de respectieve pictogrammen in de rechterbovenhoek van de lijst te klikken om de manier te wijzigen waarop de lijst met projecten wordt weergegeven.
1. (Optioneel) Klik op de knop **Zoeken** pictogram ![](assets/search-icon.png) en typ de naam van een project om het snel in de lijst te vinden.
1. Selecteer de projecten die u aan het doel wilt toevoegen, dan klik **Toevoegen**.

   De geselecteerde projecten worden toegevoegd aan het doel en worden weergegeven in de sectie Voortgangsindicatoren van de doelpagina, onder **Project** groeperen.

   Nadat u het doel hebt geactiveerd, wordt de voortgang van het doel automatisch bijgewerkt wanneer de voortgang van een project wordt bijgewerkt. Voor informatie over het activeren van een doel raadpleegt u [Doelen in Adobe Workfront-doelen activeren](../goal-management/activate-goals.md).

## Projectinformatie zoeken over doelen

<p>
De volgende projectinformatie is zichtbaar op het doelniveau in de sectie van de indicatoren van de Voortgang van een doelpagina:

</p>

<table>
  <tr>
   <td>Projectnaam
   </td>
   <td>Om het even welke veranderingen in de projectnaam weerspiegelen ook in het verbonden project.
   </td>
  </tr>
  <tr>
   <td>Projecteigenaar
   </td>
   <td>Eventuele wijzigingen in de eigenaar van het project weerspiegelen ook in het verbonden project.
   </td>
  </tr>
    <tr>
   <td>Werkelijke voortgang
   </td>
   <td> <p>Het percentage voltooide van het project. U kunt het projectpercentage niet manueel bijwerken volledig van het doel. Workfront berekent deze automatisch op basis van het percentage voltooide taken. </p>
   </td>
  </tr>
  <tr>
   <td>Voortgang
   </td>
   <td>Het percentage voltooide van het project dat door een bar wordt vertegenwoordigd. Om het even welke verandering in het percentage voltooide van het project werkt automatisch de doelvooruitgang bij tenzij het doel wordt gesloten.
   </td>
  </tr>

</table>

## Doelinformatie over projecten zoeken

De volgende doelinformatie is zichtbaar in een projectlijst of een rapport:

| Goedereninformatie | Beschrijving |
|---|---|
| Doelen | Een lijst van alle doelstellingen die een project verbonden aan hen hebben. |
| Goal Hierarchy | De hiërarchie waartoe een doel behoort. Alleen de ouders van het doel en het doel tonen op dit gebied. Onderliggende doelen worden niet weergegeven. |
| Aantal gekoppelde doelen | Het aantal doelen dat aan één project is gekoppeld. |
