---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Overzicht van Portfolio Optimizer
description: '[!UICONTROL Portfolio Optimizer] is het hulpmiddel dat voor projectevaluatie en vergelijking wordt gebruikt. Het proces om de waarden van BedrijfsGeval voor projecten te herzien en te vergelijken die aan een portefeuille worden toegewezen is hoe een portefeuillemanager projecten kan voorrang geven en de meeste waarde voor een organisatie produceert.'
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: c53e7d2229032c59710a8f955de53cfbd7fc6df4
workflow-type: tm+mt
source-wordcount: '1326'
ht-degree: 0%

---

# [!UICONTROL Portfolio Optimizer] overzicht

<!-- Audited: 01/2024 -->

[!UICONTROL Portfolio Optimizer] is het hulpmiddel dat voor projectevaluatie en vergelijking wordt gebruikt. Bij het evalueren en vergelijken van [!UICONTROL Business Case] -waarden voor projecten die zijn toegewezen aan een portfolio, kan een portfoliobeheerder prioriteit geven aan projecten en de meeste waarde voor een organisatie genereren.

![ Portfolio optimizer met projecten ](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

Het doel van [!UICONTROL portfolio optimizer] is een interface te verstrekken waarmee een portefeuillebeheerder, stuurcomité, of het bureau van het productbeheer summiere informatie over het bedrijfscase van elk project kan bekijken. De projecten kunnen dan worden geprioriteerd volgens strategische waarden en doelstellingen, of volgens hun algemene score.

[!UICONTROL Portfolio Optimizer] kan u alleen helpen als u aan de volgende voorwaarden hebt voldaan:

* [!UICONTROL Business Cases] is voltooid voor de projecten. Voor informatie, zie de artikelen in [ een BedrijfsGeval bepalen: artikelindex ](../../projects/define-a-business-case/define-business-case.md).
* Een portefeuille wordt bepaald in het gebied van het Overzicht van het Project van de sectie van de Details van het Project voor de projecten u wilt herzien.
* U hebt de projectbegroting en het geplande voordeel voor de projecten aangegeven u wilt herzien. Vaste kosten en Vaste inkomsten zijn optioneel, maar geven een extra waarde. Voor informatie, zie [ de financiert gebieden van het Project ](../../projects/project-finances/project-finances-overview-1.md).

Voor informatie over de plaats bepalen van [!UICONTROL Portfolio Optimizer], zie [ plaats [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## Financiën in de [!UICONTROL Portfolio Optimizer]

U kunt de financiële status van uw portfolio op elk gewenst moment tijdens de levensduur van uw projecten zien wanneer u de [!UICONTROL Portfolio Optimizer] gebruikt.

Houd rekening met het volgende wanneer u werkt met financiën in de [!UICONTROL Portfolio Optimizer] :

* Projecten krijgen elk een score wanneer hun [!UICONTROL Business Cases] voltooid zijn volgens de criteria die ze in [!UICONTROL Portfolio Optimizer] hebben. Lage kosten of uitlijningsprojecten krijgen bijvoorbeeld een hogere score.

  Voor meer informatie over het berekenen van de portefeuille optimizer score van een project, zie [ Overzicht van de [!UICONTROL Portfolio Optimizer] Score ](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* De financiële berekeningen voor de [!UICONTROL Portfolio Optimizer] gebruiken [!UICONTROL Budgeted Cost] in [!UICONTROL Business Case] van het project.
* U kunt handmatig prioriteiten stellen aan uw projecten in de [!UICONTROL Portfolio Optimizer] , rekening houdend met alle informatie over de projecten. Dit omvat financiële gegevens, aanpassing aan hun scorecards, en ROI, bijvoorbeeld.

### De financiële gebieden in de [!UICONTROL Portfolio Optimizer] {#the-financial-areas-in-the-portfolio-optimizer}

U kunt financiële informatie in de volgende gebieden van [!UICONTROL Portfolio Optimizer] bekijken:

* **[!UICONTROL Portfolio Header]**: Dit gebied bevat financiële informatie die is verzameld voor alle projecten in het portfolio. Deze wordt weergegeven op elk tabblad van het Portfolio-object.
* **[!UICONTROL Portfolio Finances for Selected Projects]**: In dit gebied wordt financiële informatie weergegeven die is verzameld voor de projecten die zijn geselecteerd in [!UICONTROL Portfolio Optimizer] . U kunt projecten toevoegen of verwijderen en begrijpen hoe dit de financiën van de portefeuille door de informatie op dit gebied te bekijken zal beïnvloeden.
* **[!UICONTROL Projects Finances]**: In dit gebied worden de financiële gegevens van elk project weergegeven dat in de [!UICONTROL Portfolio Optimizer] wordt weergegeven.

### De financiële velden in de [!UICONTROL Portfolio Optimizer] {#the-financial-fields-in-the-portfolio-optimizer}

De volgende financiële velden worden weergegeven in de [!UICONTROL Portfolio Optimizer] :

* [Portfolio header](#portfolio-header)
* [Portfolio financiert geselecteerde projecten](#portfolio-finances-for-selected-projects)

#### Portfolio header {#portfolio-header}

![ de kopbal van Portfolio ](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] berekent de financiële velden in de portfoliokop met behulp van gegevens uit projecten met statussen die alleen overeenkomen met [!UICONTROL Approved] of [!UICONTROL Current] .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Naam van Gebied </strong> </th> 
   <th><strong> Beschrijving </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL On Time]</td> 
   <td> <p>Het percentage projecten in de portfolio dat als [!UICONTROL On Time] wordt beschouwd. Dit is zichtbaar vanaf elk tabblad in een portfolio.</p> <p>Een project wordt beschouwd als [!UICONTROL On Time] wanneer het project <strong>[!UICONTROL Condition]</strong> <strong>[!UICONTROL On Target]</strong> is. <br> voor meer informatie over [!UICONTROL Project Conditions], zie het artikel <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref"> Overzicht van het Type van de Voorwaarde en van de Voorwaarde van het Project </a>.</p> <p>Het percentage <strong>[!UICONTROL On Time]</strong> wordt berekend met de volgende formule:</p> <p><em>[!UICONTROL On Time Portfolio Percentage] = Aantal [!UICONTROL On Time] Projecten/Totaal aantal Projecten in a [!UICONTROL Current] of [!UICONTROL Approved] status </em> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL On Budget]</td> 
   <td> <p>Het percentage projecten in de portfolio dat als [!UICONTROL On Budget] wordt beschouwd. Dit is zichtbaar vanaf elke tab in een [!UICONTROL portfolio] .</p> <p>Projecten zijn <strong>[!UICONTROL On Budget]</strong> wanneer ze hun vooraf gedefinieerde budget niet hebben overschreden. <br> voor meer informatie over het budget van een project, zie de artikel <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">[!UICONTROL Manage] informatie in het gebied van de Financiën van het project </a>.</p> <p>Het percentage [!UICONTROL On Budget] wordt berekend met de volgende formule:</p> <p><em>[!UICONTROL On Budget Portfolio Percentage] = Aantal [!UICONTROL On Budget] Projecten/Totaal Aantal Projecten </em> <em> in a [!UICONTROL Current] of [!UICONTROL Approved] status </em> </p> </td> 
  </tr> 
  <tr> 
   <td>ROI (voor portefeuille)</td> 
   <td> <p>Het [!UICONTROL Return on Investment] (ROI) voor het portfolio wordt berekend met inachtneming van het totaal [!UICONTROL Benefit] van de [!UICONTROL Portfolio] en het totaal van de [!UICONTROL Budgeted Costs] van de projecten. Dit is zichtbaar vanaf elk tabblad in een portfolio.</p> <p>De ROI-waarde van Portfolio wordt berekend met behulp van de volgende formule:</p> <p><em> Portfolio ROI = ([!UICONTROL Total Benefit] - [!UICONTROL Total Budgeted Cost])/ [!UICONTROL Total Cost] * 100 </em> </p> <p>Voor meer informatie over hoe ROI voor een project wordt berekend, zie het artikel <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref"> Rendement van Investering (ROI) berekenen </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aligned] of [!UICONTROL Alignment Score] </td> 
   <td> <p>Een gemiddelde van alle [!UICONTROL Project Alignment Score] waarden, die worden berekend na voltooiing van [!UICONTROL Scorecard] in [!UICONTROL Business Case] van het project. De uitlijningsscore van elk project wordt vermeld in de kolom [!UICONTROL Alignment] van [!UICONTROL Portfolio Optimizer] . Dit is zichtbaar vanaf elk tabblad in een portfolio.</p> <p>Voor meer informatie over het produceren van een groeperingsscore voor een project, zie het artikel <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref"> een scorecard op een project toepassen en een Score van de Uitlijning </a> produceren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Net Value]</td> 
   <td> <p>De som van alle [!UICONTROL Net Values] projecten in het portfolio. Dit is zichtbaar vanaf elk tabblad in een portfolio.</p> <p>Voor meer informatie over hoe [!UICONTROL Net Value] voor een project wordt berekend, zie het artikel <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref"> Netto Waarde </a> berekenen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Portfolio financiert geselecteerde projecten {#portfolio-finances-for-selected-projects}

![ Portfolio financiert ](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Naam van Gebied </strong> </th> 
   <th><strong>Beschrijving</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Number of projects]</td> 
   <td> <p>Het totale aantal actieve projecten in de portefeuille. Projecten die in een portfolio als actief worden beschouwd, kunnen zich in een van de volgende statussen bevinden:</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL Planning]</li> 
     <li>[!UICONTROL Approved]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budget]</td> 
   <td>U kunt dit veld handmatig bijwerken om aan te geven wat het totale budget voor de gehele portfolio is. Dit budget wordt gebruikt voor alle projecten binnen de portefeuille. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Remaining]</td> 
   <td> <p>Het resterende budget na [!UICONTROL Total Cost] voor alle projecten binnen de portefeuille is afgetrokken van de begroting van de portefeuille.</p> <p>[!UICONTROL Remaining Portfolio Budget] wordt berekend met behulp van de volgende formule:</p> <p><em>[!UICONTROL Remaining Portfolio Budget] = [!UICONTROL Total Portfolio Budget] - Totaal [!UICONTROL Budgeted Cost] van alle Portfolio-projecten </em> </p> <p>Het portfoliobudget is een handmatige vermelding in het veld Begroting van Portfolio Optimizer. </p> <p>Voor meer informatie over het volgen van kosten op een project, zie <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref"> Kosten van het Spoor </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total Cost]</td> 
   <td> <p>De som van de kosten van alle projecten die in [!UICONTROL Portfolio Optimizer] worden weergegeven. De kosten van elk project zijn gelijk aan de [!UICONTROL Budgeted Cost] van het project die wordt weergegeven in [!UICONTROL Business Case Summary] . </p> <p>Voor meer informatie over de financiële gebieden van projecten in [!UICONTROL Business Case], zie de sectie "Begrijpend Financiële Gebieden in het BedrijfsGeval"in het artikel <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref"> een BedrijfsGeval voor een project </a> creëren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risk] </td> 
   <td> <p>De som van alle [!UICONTROL Potential Risk Costs] projecten in het portfolio. De [!UICONTROL Potential Risk Cost] van elk project wordt vermeld in de [!UICONTROL Risk] kolom van [!UICONTROL Portfolio Optimizer]. </p> <p>Voor meer informatie over het berekenen van risico's voor projecten, zie het artikel <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref"> Mogelijke Kosten van het Risico </a> berekenen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benefit]</td> 
   <td> <p>De som van alle [!UICONTROL Planned Benefit] waarden van alle projecten in het portfolio. De waarde voor Gepland voordeel van elk project wordt vermeld in de kolom [!UICONTROL Benefit] van [!UICONTROL Portfolio Optimizer] . </p> <p>Voor meer informatie over [!UICONTROL Planned Benefit] van een project, zie het artikel <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref"> Overzicht van project Gepland Voordeel </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risk to Net Value] indicator</td> 
   <td> <p>Hiermee wordt de [!UICONTROL Potential Risk] -waarde gemeten, rekening houdend met de [!UICONTROL Net Value] -waarde die door alle projecten in het portfolio wordt geboden. Om de meest efficiënte oplossing in het portfolio te bereiken, moet u controleren of de indicator [!UICONTROL Risk] laag is en de indicator [!UICONTROL Net Value] hoog. </p> <p>Voor meer informatie over het berekenen van Risico aan [!UICONTROL Net Value], zie het artikel <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref"> het Risico aan Netto Waarde in een portefeuille </a> berekenen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## De [!UICONTROL Portfolio Optimizer] aanpassen

U kunt alleen het gebied van de projectlijst van de [!UICONTROL Portfolio Optimizer] aanpassen door instellingen te gebruiken om de informatie in de lijst te wijzigen.

De volgende pictogrammen en opties zijn beschikbaar voor [!UICONTROL Portfolio Optimizer]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Pictogram in de Portfolio Optimizer</strong></td> 
   <td><strong>Naam</strong></td> 
   <td><strong>Functie</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[!UICONTROL Set project priority]</td> 
   <td><p>Gebruik dit pictogram wanneer u de projectorde wilt bewaren, die op hun prioriteit wordt gebaseerd.</p>
   <p>U moet hebben leiden toestemmingen aan alle projecten in de lijst om <b> te kunnen gebruiken Vastgestelde projectprioriteit </b></p>.
    </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-optimize-icon-in-optimizer.png"> </td> 
   <td>[!UICONTROL Optimize portfolio]</td> 
   <td>Gebruik dit pictogram om het portfolio te optimaliseren op basis van de volgende financiële waarden van de projecten:
    <ul>
     <li>[!UICONTROL Cost]</li>
     <li>[!UICONTROL Alignment]</li>
     <li>[!UICONTROL Value]</li>
     <li>[!UICONTROL Risk to Benefit]</li>
     <li>[!UICONTROL ROI]</li>
    </ul><p>Voor meer informatie over het optimaliseren van uw portefeuille, zie het artikel <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref"> projecten in [!UICONTROL Portfolio Optimizer]</a> optimaliseren.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>[!UICONTROL Undo]/ [!UICONTROL Redo] pictogrammen</td> 
   <td>Gebruik deze pictogrammen om de wijzigingen die u in de [!UICONTROL Portfolio Optimizer] hebt aangebracht, te annuleren of opnieuw uit te voeren voordat u ze opslaat.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portfolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>[!UICONTROL Show]/[!UICONTROL Hide] ongecontroleerde projecten</td> 
   <td>Gebruik deze pictogrammen om de ongecontroleerde projecten in het portfolio weer te geven of te verbergen.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[!UICONTROL Export] </td> 
   <td> <p>Gebruik dit pictogram om de gegevens in het [!UICONTROL Project Prioritization] -gebied van [!UICONTROL Portfolio Optimizer] te exporteren. U kunt het naar de volgende formaten uitvoeren:</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>[!UICONTROL Tab] Gescheiden</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferences_portfolio_optimizer.png"> </td> 
   <td>[!UICONTROL Preferences]</td> 
   <td> <p>Gebruik dit pictogram om de projectgebieden te wijzigen die in de kolommen van [!UICONTROL Portfolio Optimizer] worden getoond, of om te wijzigen welke projecten u in [!UICONTROL Optimizer] toont, die op hun status wordt gebaseerd. </p> <p>Tip:  
     <ul> 
      <li> <p>Niet alle standaardvelden van [!DNL Workfront] zijn beschikbaar om toe te voegen in de kolommen. </p> </li> 
     </ul> 
     <ul> 
      <li> <p>U kunt alleen aangepaste velden toevoegen die een andere waarde dan nul hebben in een van de projecten in het portfolio.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
