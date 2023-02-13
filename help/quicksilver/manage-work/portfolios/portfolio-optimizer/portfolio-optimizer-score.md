---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Overzicht van de Portfolio Optimizer Score
description: U kunt de Portfolio Optimizer score in de Optimizer van de Portfolio vinden. Deze wordt weergegeven in het dialoogvenster [!UICONTROL Score] kolom voor elk project. Dit vertegenwoordigt een score voor elk project in de portefeuille.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 4451b1a3-57ae-4c66-a6a1-a85bd51a1648
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---

# Overzicht van de [!UICONTROL Portfolio Optimizer] Score

U kunt de [!UICONTROL Portfolio Optimizer] score in de [!UICONTROL Portfolio Optimizer]. Deze wordt weergegeven in het dialoogvenster **[!UICONTROL Score]** kolom voor elk project. Dit vertegenwoordigt een score voor elk project in de portefeuille.

Voor informatie over de locatie van de [!UICONTROL Portfolio Optimizer], zie het artikel [[!UICONTROL Portfolio Optimizer] overzicht](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

Voor informatie over hoe [!DNL Adobe Workfront] gebruikt de Score van het project en andere projectinformatie om projecten in te optimaliseren [!UICONTROL Portfolio Optimizer], zie [Projecten optimaliseren in Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

## Verschil tussen de [!UICONTROL Alignment Score] en de [!UICONTROL Portfolio Optimizer Score]

Er is een verschil tussen de uitlijningsscore en de optimaliseringsscore van een project voor het portfolio.

De groeperingsscore van een project wordt berekend gebaseerd op de punten die na de voltooiing van scorecard worden verkregen. Deze score wordt vervolgens gebruikt om de uitlijningsscore van het portfolio te bepalen. De uitlijningsscore wordt weergegeven als een percentage.\
De uitlijningsscore van een project wordt weergegeven in het deelvenster **[!UICONTROL Alignment]** kolom van de [!UICONTROL Portfolio Optimizer] of in de [!UICONTROL Alignment] van het [!UICONTROL Business Case Summary].

![](assets/business-case-summary-aligned-field-highlighted.png)

![](assets/project-alignment-score-portfolio-optimizer-highlighted-350x174.png)

Zie het artikel voor meer informatie over het genereren van de uitlijningsscore van een project [Pas een scorecard op een project toe en produceer een Score van de Uitlijning](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

De [!UICONTROL portfolio optimizer] de score is een automatisch berekende positie in de [!UICONTROL Portfolio Optimizer] aan de hand van welke projecten prioriteit kan worden toegekend. De score voor het optimaliseren van het portfolio wordt weergegeven als een indicatiepictogram, vergezeld van een nummer en wordt weergegeven in het dialoogvenster **[!UICONTROL Score]** kolom van de [!UICONTROL Portfolio Optimizer].

>[!NOTE]
>
>Een project kan in [!UICONTROL Portfolio Optimizer] alleen als de Business Case is voltooid. Raadpleeg het artikel voor meer informatie over het voltooien van een kwestie-Business [[!UICONTROL Create a Business Case] voor een project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

![](assets/portfolio-optimizer-project-score-highlighted-350x132.png)

De score voor elk project wordt berekend op basis van het belang van de volgende categorieën:

* [!UICONTROL Cost]
* [!UICONTROL Alignment]
* [!UICONTROL Net Value]
* [!UICONTROL Risk to Benefit]
* [!UICONTROL ROI]

## De [!UICONTROL Portfolio Optimizer] Score

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This was edited based on this issue, per Anna: https://hub.workfront.com/issue/603d0c58000095ea0bc00ce5e2110693/overview)</p>
-->

[!DNL Workfront] Hiermee maakt u een score met de [!UICONTROL Portfolio Optimizer] die een rangorde is om bij te dragen tot de prioritering van projecten. De waarden in de portefeuille zijn gebaseerd op waarden die in de bedrijfsgevallen van de projecten zijn ingevoerd en worden gebruikt om een score voor het project te berekenen. Projecten met een hogere score kunnen als belangrijker worden beschouwd en er kan prioriteit aan worden gegeven om ze eerst af te ronden.

Ga als volgt te werk om de positie van een project te bepalen:

1. Ga naar de [!UICONTROL Portfolio Optimizer].
1. Houd de muisaanwijzer boven het ranking-pictogram om de score voor het optimaliseren van een portfolio voor een project weer te geven.

![ranking_icon_in_portfolio_optimizer_new.png](assets/ranking-icon-in-portfolio-optimizer-new-350x160.png)

Bij het algoritme voor de berekening van de scores wordt rekening gehouden met de waarden die in de zakelijke gevallen van de projecten worden geschetst en met de gewichten die zij dragen. Het geeft elk project in optimizer een score en normaliseert die score zodat is er altijd een project met een score van 100. Dit geeft een hoge score aan het beste project.

**Voorbeeld:** Als u bijvoorbeeld [!UICONTROL higher alignment] de enige factor die in overweging moet worden genomen, is dat het project met de hoogste uitlijning de score 100 krijgt.

Hieronder volgt een overzicht van de criteria waaraan u een project kunt voldoen:

* [!UICONTROL Cost]
* [!UICONTROL Alignment]
* [!UICONTROL Value]
* [!UICONTROL Risk to Benefit]
* [!UICONTROL ROI]

![](assets/optimizer-sliding-value-options-350x77.png)

Voor informatie over hoe te om projecten in de portefeuille te optimaliseren, zie [Projecten optimaliseren in het dialoogvenster [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

Elk criterium op het configuratiescherm ([!UICONTROL Cost], [!UICONTROL Alignment], [!UICONTROL ROI], [!UICONTROL Net Value], [!UICONTROL Risk to Benefit]) krijgen hun gewichten in het bereik 0-100, gebaseerd op wat u hebt geselecteerd.

Voor elk project met een volledig bedrijfscase wordt een score per criteria geproduceerd gebruikend de volgende formule:

```
Score Per Criteria = (Project Value For The Criteria - AVG(all the project values for this criteria)) / Standard Deviation of that value for that project
```

**Voorbeeld:** Voor de [!UICONTROL Alignment Score] voor Project A, zult u het volgende hebben:

```
Alignment Score = (Project A Alignment Score - AVG (of all the project Alignments)) / Standard Deviation of alignment score for that project
```

Als u alle [!UICONTROL Score Per Criteria] berekend, kunt u hen toevoegen rekening houdend met hun gewichten om de volledige score per project te krijgen. De score van het project wordt berekend met behulp van de volgende formule:

```
Score = Cost Score * Cost Weight + Alignment Score * Alignment Weight + ROI Score * ROI Weight + Net Value Score * Net Value Weight + Risk Score * Risk Weight
```

Voor de projectkosten en [!UICONTROL risk] de logica is omgekeerd van de manier waarop de andere criteria werken : als u de [!UICONTROL Low Cost] om belangrijk voor u te zijn, zal het niet de algemene score van het project verhogen maar verminderen door `Cost Score * Cost Weight`.

Nadat u voor elk project scores hebt berekend, [!UICONTROL Optimization Score] wordt voor de projecten als volgt gedefinieerd:

1. [!UICONTROL Minimum] en [!UICONTROL Maximum] scores zijn gedefinieerd.
1. Het bereik tussen deze waarden wordt berekend.
1. Voor elk project [!UICONTROL Optimization Score] wordt berekend met behulp van de volgende formule:

   ```
   Optimization Score = Rounded ((Score - Minimum / Range)*100)
   ```
