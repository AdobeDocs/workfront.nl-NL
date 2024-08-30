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
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Projecten toevoegen aan doelen in Adobe Workfront-doelen

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

U kunt projecten met doelstellingen verbinden om erop te wijzen hoe het doel vordert, die op de daadwerkelijke vooruitgang van het project wordt gebaseerd. Het project wordt een voortgangsindicator voor het doel.

Door projecten aan doelstellingen te verbinden kunt u de strategische planning (doelstellingen) van uw organisatie aan het daadwerkelijke werk verbinden uw mensen uitvoeren en voltooien elke dag (projecten).

>[!IMPORTANT]
>
>Projectniveaudoelstellingen die in het gebied Bedrijfs van het Geval van een project worden gecreeerd worden niet verbonden met strategische doelstellingen die in de Doelen van Workfront worden gecreeerd. Voor informatie over de doelstellingen van het BedrijfsGeval project, zie [ BedrijfsGevallendoelstellingen ](../../manage-work/projects/define-a-business-case/create-business-case-goals.md) creëren.


## Toegangsvereisten

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
  <ul><li>Een ultiem plan </li></ul>
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
 <p> Nieuwe productbehoefte, één van het volgende: </p>
<ul>
<li>Een Select- of Prime Adobe Workfront-abonnement en een extra Adobe Workfront Goals-licentie.</li>
<li>Een Ultimate Workfront-plan dat standaard Workfront Goals bevat. </li></ul>
 <p>of</p>
 <p>Huidige productvereiste: een Workfront-plan en een extra licentie voor Adobe Workfront Goals. </p> <p>Voor informatie, zie <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref"> Vereisten om de Doelen van Workfront </a> te gebruiken. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Toegangsniveau</td>
 <td> <p>Toegang tot doelen bewerken</p> </td>
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

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* Wanneer u een project schrapt in bijlage aan een doel, wordt het project ook geschrapt van het doel.

  >[!CAUTION]
  >
  >Als het doel actief was alvorens u het project schrapte en er geen andere vooruitgangsindicatoren op het doel zijn, wordt het doel Inactief.


## Projecten toevoegen aan doelen

1. Klik het **Belangrijkste Menu** ![](assets/main-menu-icon.png) (ontwerp dit voor Shell: of klik het **Belangrijkste Menu** ![](assets/three-line-main-menu-icon.png) in de upper-left hoek, als het beschikbaar is.), toen **Doelen**.
1. Klik in de lijst met doelen op de naam van een doel om de doelpagina te openen.
1. Klik **indicatoren van de Voortgang** in het linkerpaneel.
1. Van de **Nieuwe voortgangsindicator** drop-down menu, klik **toevoegen bestaand project**.

   De Add projecten aan de vertoningen van het doelvakje.
1. (Facultatief) werk de **Mening** bij, **Filter**, of **Groepering** door de respectieve pictogrammen in de hoger-juiste hoek van de lijst te klikken om de manier te wijzigen de lijst van projectvertoningen.
1. (Facultatief) klik het **pictogram van het 1} Onderzoek ![](assets/search-icon.png) en begin de naam van een project te typen om het in de lijst snel te vinden.**
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
