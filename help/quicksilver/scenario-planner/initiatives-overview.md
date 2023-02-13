---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Overzicht van initiatieven in het scenario Planner
description: De Scenario Planner is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring en vereist een aanvullende licentie. Zie het overzicht Scenario Planner voor meer informatie over de Workfront Scenario Planner.
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Overzicht van initiatieven in het [!DNL Scenario Planner]

De [!DNL Scenario Planner] is alleen beschikbaar in de nieuwe [!DNL Adobe Workfront] ervaring hebben opgedaan en een aanvullende vergunning nodig hebben. Voor informatie over de [!DNL Workfront Scenario Planner], zie [De [!DNL Scenario Planner] overzicht](../scenario-planner/scenario-planner-overview.md).
Als bedrijfsmanager kunt u initiatieven voor plannen in [!DNL Adobe Workfront Scenario Planner]. Raadpleeg het artikel voor informatie over het maken van plannen [Plannen maken en bewerken in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Overzicht van initiatieven

Met de [!DNL Workfront Scenario Planner], kunt u de volgende informatie voor elk initiatief schatten en herzien:

* Schatting van het soort en het aantal functies die nodig kunnen zijn om het initiatief te voltooien. Dit verhoogt het vereiste aantal functies voor het abonnement en berekent de Personeelskosten die u voor een initiatief kunt beoordelen.
* Schatting van de vaste kosten in verband met de werkzaamheden die nodig zijn om het initiatief te voltooien.
* Schatting van het Geplande Voordeel dat uw bedrijf zou kunnen winnen wanneer het initiatief wordt voltooid.

Om informatie over uw initiatieven te bekijken, kunt u tot individuele initiatieven binnen een plan toegang hebben. Raadpleeg het artikel voor informatie over het maken van en het openen van initiatieven [Initiatieven maken en bewerken in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Overwegingen bij initiatieven

Houd rekening met het volgende wanneer u initiatieven maakt:

* U moet een plan maken voordat u een initiatief kunt maken.
* U kunt geheel nieuwe initiatieven maken of projecten importeren in een plan. De projecten worden initiatieven binnen het plan.

   Ga voor meer informatie over het geheel nieuwe initiatief naar [Initiatieven maken en bewerken in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   Voor informatie over het invoeren van projecten in een plan om initiatieven van projecten tot stand te brengen, zie [Projecten importeren naar plannen in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Initiatieven zijn kleinere planningseenheden dan plannen en worden alleen als onderdeel van een plan gemaakt.
* Het kortste initiatief kan een duur van één maand hebben. Het langste initiatief kan een looptijd van vijf jaar hebben.
* U kunt niet echt aan een initiatief werken. Op het initiatiefniveau kunt u bepalen welke middelen nodig zijn en welke kosten deze middelen zullen maken zodat u kunt beginnen één van de eisen van het plan uit te voeren. Bijvoorbeeld, als uw bedrijf een plan heeft om een nieuw bureau in een nieuwe plaats uit te breiden en te verwerven, zou uw afdeling een initiatief kunnen hebben om de netwerkinfrastructuur voor die nieuwe plaats te installeren.
* U kunt meerdere initiatieven maken in een plan. Met elk initiatief, kunt u een strategie op hoog niveau schetsen om het werk in uw afdeling te verwezenlijken.
* U kunt binnen een plan prioriteit geven aan initiatieven om ervoor te zorgen dat het belangrijkste initiatief de meeste begroting en de meeste middelen krijgt.
* Wanneer u initiatieven binnen een plan creeert kan iedereen die dat plan bekijkt alle initiatieven binnen het plan ook bekijken.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change when we add to the access levels granularity)</p>
  -->

* U kunt initiatieven publiceren om projecten tot stand te brengen of de projecten bij te werken die met hen verbonden zijn. Voor informatie over publicatieinitiatieven raadpleegt u [Werk of creeer projecten bij door initiatieven in te publiceren [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## Financiële informatie over initiatieven

U kunt financiële informatie over individuele initiatieven herzien om te begrijpen hoe de initiatieven binnen het plan passen. Raadpleeg het artikel voor informatie over het benaderen van een initiatief [Initiatieven maken en bewerken in het dialoogvenster [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

U kunt de volgende financiële indicatoren over een initiatief bekijken door tot het binnen een plan toegang te hebben:

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costs total amount]</td> 
   <td> <p style="font-weight: normal;">Dit is een berekening van de totale kosten van een initiatief. </p> <p style="font-weight: normal;">[!DNL Workfront] berekent de totale kostenwaarde van een initiatief aan de hand van deze formule:</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fixed Costs]</td> 
   <td> <p><span style="font-weight: normal;">Dit is een handmatige invoer waarop u kunt schatten <span>een maandelijks bedrag aan vaste kosten voor elke maand van het initiatief.</span> Hieronder vallen niet de kosten in verband met de aan het initiatief toegevoegde taken die in de [!UICONTROL People Cost] veld.</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL People Costs]</td> 
   <td> <p style="font-weight: normal;">Dit is een totale berekening van de kosten in verband met de functie van het initiatief gedurende de looptijd van het initiatief. Dit aantal hangt af van het aantal VTE's of uren dat u voor elke maand van het initiatief inschat voor een functie. </p> 
     <p><b>TIPS</b>  
     <ul> 
      <li> <p>Het aantal maandelijkse VTE's voor dezelfde functie kan per maand verschillen.</p> </li> 
      <li> <p>[!DNL Workfront] is van mening dat er 160 werkuren zijn in één maand. </p> </li> 
     </ul> 
     <p>[!DNL Workfront] berekent de [!UICONTROL People Costs] van een initiatief met behulp van de volgende formule:</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] berekent de maandelijkse Personeelskosten voor elke maand tijdens de duur van het Initiatief met behulp van de volgende formule:</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>VOORBEELD</b></p>
      <p>Als u een initiatief hebt met een duur van 6 maanden waarvoor 1 Designer vereist is met een frequentie van 50 dollar per maand voor 1 FTE en een webontwerper met een uurtarief van 100 dollar voor 2 maanden van het initiatief, worden de kosten voor het initiatief als volgt berekend:</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planned Benefit]</td> 
   <td>Dit is een handmatige vermelding waarin u het totale voordeel kunt inschatten dat uw afdeling zou behalen door dit initiatief te voltooien. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Net Value amount]</td> 
   <td> <p style="font-weight: normal;">Dit is de waarde van uw initiatief, rekening houdend met de totale kosten en het op het initiatief geraamde voordeel. [!DNL Workfront] berekent de nettowaarde van een initiatief met behulp van de volgende formule:</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--drafted content from People Costs:
(NOTE: drafted below)</p> 
       <p>Depending on whether the plan is set up to use FTEs or hours, Workfront uses the following formulas to calculate People Cost:</p> 
       <ul> 
        <li> <p>When using FTEs: </p> <p><code>People Costs = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, where 160 is the total number of working hours in a month. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span style="font-weight: normal;"> When estimating resources using FTEs,(NOTE: drafted and yellow and fix the rest of the sentence)
      <p>When using hours:</p> 
      <p><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> 
      <p>For information about setting up the plan to use hours or FTE, see <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Scenario Planner</a>.</p>-->

## Informatie over initiatieven in verslagen

U kunt informatie over initiatieven weergeven in rapporten, zoals wordt beschreven in de onderstaande tabel. Deze informatie is alleen beschikbaar in uw Workfront-exemplaar als uw bedrijf een Workfront Scenario Planner-licentie heeft aangeschaft.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Type rapport</b></td> 
   <td><b>Initiatiefinformatie</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative] </td> 
   <td>Naam, duur, begin- en einddatum, ingevoerd door, id, datum van laatste publicatie*, alle projectvelden inclusief aangepaste velden*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role]</td> 
   <td>Alle informatie over het initiatief zoals hierboven vermeld, (Functie-id), Project*, Geplande uren projecttoewijzing*, Taken initiëren, Aantal taken (Functie-rol), Alle projectvelden inclusief aangepaste velden*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL Project]*</p></td> 
   <td> <p>Alle bovenstaande informatie over het initiatief*</p> </td> 
  </tr> 
 </tbody> 
</table>

*Deze velden vullen alleen informatie in uit het project dat verband houdt met het initiatief, wanneer het initiatief is gemaakt op basis van een project of minstens eenmaal is gepubliceerd naar een project. Voor informatie over publicatieinitiatieven raadpleegt u [Werk of creeer projecten bij door initiatieven in te publiceren [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
