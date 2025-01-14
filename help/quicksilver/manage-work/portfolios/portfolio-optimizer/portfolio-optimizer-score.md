---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Overzicht van de Portfolio Optimizer Score
description: U kunt de score van de Optimizer van het Portfolio in de Optimizer van het Portfolio vinden. Deze wordt in de kolom [!UICONTROL Score] voor elk project weergegeven. Dit vertegenwoordigt een score voor elk project in de portefeuille.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 4451b1a3-57ae-4c66-a6a1-a85bd51a1648
source-git-commit: 00e58ea9a207037b701e1be010c2c4c2995d60e0
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Overzicht van de [!UICONTROL Portfolio Optimizer] score

<!--Audited: 01/2025-->

U kunt de [!UICONTROL Portfolio Optimizer] score vinden in [!UICONTROL Portfolio Optimizer] . Deze wordt in de kolom **[!UICONTROL Score]** voor elk project weergegeven. Dit vertegenwoordigt een score voor elk project in de portefeuille.

Voor informatie over de plaats bepalen van [!UICONTROL Portfolio Optimizer], zie het artikel [[!UICONTROL Portfolio Optimizer] overzicht ](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

Voor informatie over hoe [!DNL Adobe Workfront] de Score van het project en andere projectinformatie gebruikt om projecten in [!UICONTROL Portfolio Optimizer] te optimaliseren, zie [ projecten in Portfolio optimaliseren ](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

## Verschil tussen de [!UICONTROL Alignment Score] en de [!UICONTROL Portfolio Optimizer Score]

Er is een verschil tussen de uitlijningsscore en de optimaliseringsscore van een project voor het portfolio.

De groeperingsscore van een project wordt berekend gebaseerd op de punten die na de voltooiing van scorecard worden verkregen. Deze score wordt vervolgens gebruikt om de uitlijningsscore van het portfolio te bepalen. De uitlijningsscore wordt weergegeven als een percentage.

De uitlijningsscore van een project wordt weergegeven in de kolom **[!UICONTROL Alignment]** van het [!UICONTROL Portfolio Optimizer] -veld of in het [!UICONTROL Alignment] -veld van het [!UICONTROL Business Case Summary] -project.

![](assets/business-case-summary-aligned-field-highlighted.png)

![](assets/project-alignment-score-portfolio-optimizer-highlighted-350x174.png)

Voor meer informatie over het produceren van de groeperingsscore van een project, zie het artikel [ een scorecard op een project toepassen en een Score van de Uitlijning ](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md) produceren.

De [!UICONTROL portfolio optimizer] score is een positie die automatisch wordt berekend in de [!UICONTROL Portfolio Optimizer] aan de hand waarvan aan projecten prioriteiten kunnen worden toegewezen. De score voor het optimaliseren van het portfolio wordt weergegeven als een indicatorpictogram met een getal en wordt weergegeven in de kolom **[!UICONTROL Score]** van [!UICONTROL Portfolio Optimizer] .

>[!NOTE]
>
>Een project kan in [!UICONTROL Portfolio Optimizer] slechts worden gescoord als zijn BedrijfsGeval is voltooid. Voor meer informatie over de voltooiing van een Bedrijfs Geval, zie het artikel [[!UICONTROL Create a Business Case] voor een project ](../../../manage-work/projects/define-a-business-case/create-business-case.md).

![](assets/portfolio-optimizer-project-score-highlighted-350x132.png)

De score voor elk project wordt berekend op basis van het belang van de volgende categorieën:

* [!UICONTROL Cost]
* [!UICONTROL Alignment]
* [!UICONTROL Net Value]
* [!UICONTROL Risk to Benefit]
* [!UICONTROL ROI]

## De [!UICONTROL Portfolio Optimizer] score berekenen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This was edited based on this issue, per Anna: https://hub.workfront.com/issue/603d0c58000095ea0bc00ce5e2110693/overview)</p>
-->

[!DNL Workfront] levert een score op met behulp van de [!UICONTROL Portfolio Optimizer] . Dit is een classificatie die u helpt bij het bepalen van prioriteiten voor projecten. De waarden in de portefeuille zijn gebaseerd op waarden die in de bedrijfsgevallen van de projecten zijn ingevoerd en worden gebruikt om een score voor het project te berekenen. Projecten met een hogere score kunnen als belangrijker worden beschouwd en er kan prioriteit aan worden gegeven om ze eerst af te ronden.

Ga als volgt te werk om de positie van een project te bepalen:

1. Ga naar de [!UICONTROL Portfolio Optimizer] .
1. Houd de muisaanwijzer boven het ranking-pictogram om de score voor het optimaliseren van een portfolio voor een project weer te geven.

![ ranking_icon_in_portfolio_optimizer_new.png ](assets/ranking-icon-in-portfolio-optimizer-new-350x160.png)

Bij het algoritme voor de berekening van de scores wordt rekening gehouden met de waarden die in de zakelijke gevallen van de projecten worden geschetst en met de gewichten die zij dragen. Het geeft elk project in optimizer een score en normaliseert die score zodat is er altijd een project met een score van 100. Dit geeft een hoge score aan het beste project.

>[!BEGINSHADEBOX]

**VOORBEELD**

Als u bijvoorbeeld [!UICONTROL higher alignment] als enige factor in overweging neemt, krijgt het project met de hoogste uitlijning de score 100.

>[!ENDSHADEBOX]

Hieronder volgt een overzicht van de criteria waaraan u een project kunt voldoen:

* [!UICONTROL Cost]
* [!UICONTROL Alignment]
* [!UICONTROL Value]
* [!UICONTROL Risk to Benefit]
* [!UICONTROL ROI]

![](assets/optimizer-sliding-value-options-350x77.png)

Voor informatie over hoe te om projecten in de portefeuille te optimaliseren, zie [ projecten in [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md) optimaliseren.

Aan alle criteria in het configuratiescherm ([!UICONTROL Cost], [!UICONTROL Alignment], [!UICONTROL ROI], [!UICONTROL Net Value], [!UICONTROL Risk to Benefit]) wordt het gewicht gegeven in het bereik 0-100 op basis van wat u hebt geselecteerd.

Voor elk project met een volledig bedrijfscase wordt een score per criteria geproduceerd gebruikend de volgende formule:

```
Score Per Criteria = (Project Value For The Criteria - AVG(all the project values for this criteria)) / Standard Deviation of that value for that project
```

**Voorbeeld:** voor [!UICONTROL Alignment Score] voor Project A, zult u het volgende hebben:

```
Alignment Score = (Project A Alignment Score - AVG (of all the project Alignments)) / Standard Deviation of alignment score for that project
```

Wanneer u alle berekeningen van [!UICONTROL Score Per Criteria] hebt uitgevoerd, kunt u deze toevoegen met inachtneming van hun gewichten om de volledige score per project te halen. De score van het project wordt berekend met behulp van de volgende formule:

```
Score = Cost Score * Cost Weight + Alignment Score * Alignment Weight + ROI Score * ROI Weight + Net Value Score * Net Value Weight + Risk Score * Risk Weight
```

Voor de projectkosten en [!UICONTROL risk] werkt de logica omgekeerd van de manier waarop de andere criteria werken: als u wilt dat de [!UICONTROL Low Cost] voor u belangrijk is, zal de algemene score van het project niet met `Cost Score * Cost Weight` toenemen maar afnemen.

Nadat u voor elk project scores hebt berekend, wordt [!UICONTROL Optimization Score] voor de projecten als volgt bepaald:

1. [!UICONTROL Minimum] en [!UICONTROL Maximum] scores zijn gedefinieerd.
1. Het bereik tussen deze waarden wordt berekend.
1. Voor elk project wordt [!UICONTROL Optimization Score] berekend met behulp van de volgende formule:

   ```
   Optimization Score = Rounded ((Score - Minimum / Range)*100)
   ```
