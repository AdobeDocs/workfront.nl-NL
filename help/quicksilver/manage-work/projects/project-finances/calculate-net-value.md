---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Nettowaarde berekenen
description: De nettowaarde van een project is de totale verwachte waarde van het project na berekening van het voordeel en verwijdering van de kosten.
author: Alina
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# Nettowaarde berekenen

De nettowaarde van een project is de totale verwachte waarde van het project na berekening van het voordeel en verwijdering van de kosten. 

## Overzicht van de netto-waarde van het project

Adobe Workfront berekent de Netto Waarde van een project gebruikend de volgende formule: 

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

De volgende gebieden kunnen de Netto Waarde van een project beïnvloeden:

* **Gepland voordeel**: Dit is een handmatige invoer die door de eigenaar van het project wordt opgegeven bij het voltooien van de **Projectinfo** in de Business Case.\
   Voor meer informatie over het Geplande Voordeel van een project, zie [Projectinfo](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) sectie in artikel [Overzicht van de gebieden van de bedrijfscase](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* **Geraamde kosten**: Dit zijn de totale kosten verbonden aan het project zoals geschat wanneer u het project eerst lanceert.

   De **Geraamde kosten** gebruikt de **begrote arbeidskosten** Waarde die wordt berekend in het gebied van de Begroting van het Middel van het BedrijfsGeval en het houdt rekening met de uren die voor uw baanrollen in de Planner van het Middel worden begroot en het tarief van Kosten per Uur van elke baanrol.\
   De begrote kosten beïnvloeden de **Nettowaarde** van het project. Voor meer informatie over hoe de begrote Kosten wordt berekend, zie [Geraamde kosten berekenen](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **Potentiële risicokosten**: Dit zijn de kosten verbonden aan om het even welke risico&#39;s op het project, zoals zij in het BedrijfsGeval, of het lusje van Risks van het project worden bepaald.\
   Raadpleeg het artikel voor meer informatie over het berekenen van de potentiële risicokosten van een project [Mogelijke risicokosten berekenen](../../../manage-work/projects/project-finances/potential-risk-cost.md).

    

## De netto-waarde van het project zoeken

U kunt de Netto Waarde voor een project in de volgende gebieden in Workfront vinden:

* In bedrijfscase - Samenvatting van de bedrijfscase \
   Raadpleeg voor meer informatie over het gedeelte Overzicht van bedrijfscase de sectie &quot;Understanding the Business Case Summary&quot; in het artikel [Een bedrijfscase maken voor een project](../../../manage-work/projects/define-a-business-case/create-business-case.md) [Een bedrijfscase maken voor een project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

   ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* In Portfolio optimizer als het project met een portefeuille wordt geassocieerd

   >[!TIP]
   >
   >Het totaal van alle netto waarden van het project is de Netto Waarde van de portefeuille.

   Voor meer informatie over de Portfolio Optimizer, zie [Overzicht van Portfolio optimaliseren](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* In het gebied van de Waarde van het Project Netto van de volgende lijsten en rapporten:

   * Project
   * Taak
   * Probleem
   * Project (financiële gegevens)
   Raadpleeg het artikel voor meer informatie over het maken van een rapport [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
