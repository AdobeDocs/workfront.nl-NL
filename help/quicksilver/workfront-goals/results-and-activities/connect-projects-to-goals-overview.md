---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Projecten toevoegen aan doelen in Adobe Workfront-doelen
description: U kunt projecten met doelstellingen verbinden om erop te wijzen hoe het doel vordert, die op de daadwerkelijke vooruitgang van het project wordt gebaseerd. Het project wordt een voortgangsindicator voor het doel.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 0%

---

# Projecten toevoegen aan doelen in Adobe Workfront-doelen

<!--Audited for P&P only: 10/2025-->

U kunt projecten met doelstellingen verbinden om erop te wijzen hoe het doel vordert, die op de daadwerkelijke vooruitgang van het project wordt gebaseerd. Het project wordt een voortgangsindicator voor het doel.

Door projecten aan doelstellingen te verbinden kunt u de strategische planning (doelstellingen) van uw organisatie aan het daadwerkelijke werk verbinden uw mensen uitvoeren en voltooien elke dag (projecten).

>[!IMPORTANT]
>
>Projectniveaudoelstellingen die in het gebied Bedrijfs van het Geval van een project worden gecreeerd worden niet verbonden met strategische doelstellingen die in de Doelen van Workfront worden gecreeerd. Voor informatie over de doelstellingen van het BedrijfsGeval project, zie [ BedrijfsGevallendoelstellingen ](../../manage-work/projects/define-a-business-case/create-business-case-goals.md) creëren.


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

Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
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

## Overwegingen over het verbinden van projecten met doelstellingen

* U kunt een project toevoegen dat aan de volgende criteria aan een doel voldoet:

   * U moet ten minste beschikken over de juiste machtigingen om deze weer te geven.

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

  ![Goal closed](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* Wanneer u een project schrapt in bijlage aan een doel, wordt het project ook geschrapt van het doel.

  >[!CAUTION]
  >
  >Als het doel actief was alvorens u het project schrapte en er geen andere vooruitgangsindicatoren op het doel zijn, wordt het doel Inactief.


## Projecten toevoegen aan doelen

1. Klik het **Belangrijkste pictogram van het Menu** ![ Belangrijkste pictogram van het Menu ](assets/main-menu-icon.png) (ontwerp dit voor Shell: of klik de **Belangrijkste lijnen van het Menu** ![ HoofdMenu ](assets/three-line-main-menu-icon.png) in de upper-left hoek, als het beschikbaar is.), toen **Doelen**.
1. Klik in de lijst met doelen op de naam van een doel om de doelpagina te openen.
1. Klik **indicatoren van de Voortgang** in het linkerpaneel.
1. Van de **Nieuwe voortgangsindicator** drop-down menu, klik **toevoegen bestaand project**.

   De Add projecten aan de vertoningen van het doelvakje.
1. (Facultatief) werk de **Mening** bij, **Filter**, of **Groepering** door de respectieve pictogrammen in de hoger-juiste hoek van de lijst te klikken om de manier te wijzigen de lijst van projectvertoningen.
1. (Facultatief) klik het **pictogram van het Onderzoek** pictogram van het Onderzoek ![ en begin de naam van een project te typen om het in de lijst snel te vinden.](assets/search-icon.png)
1. Selecteer de projecten die u aan het doel wilt toevoegen, dan klik **toevoegen**.

   De geselecteerde projecten worden toegevoegd aan het doel en zij tonen in de Voortgangsindicatorensectie van de doelpagina, onder de **** groepering van het Project.

   Nadat u het doel hebt geactiveerd, wordt de voortgang van het doel automatisch bijgewerkt wanneer de voortgang van een project wordt bijgewerkt. Voor informatie over het activeren van een doel, zie [ doelstellingen in de Doelen van Adobe Workfront ](../goal-management/activate-goals.md) activeren.

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
   <td> <p>Het percentage van de voltooiing van het project. U kunt het projectpercentage niet manueel bijwerken volledig van het doel. Workfront berekent deze automatisch op basis van het percentage voltooide taken. </p>
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
