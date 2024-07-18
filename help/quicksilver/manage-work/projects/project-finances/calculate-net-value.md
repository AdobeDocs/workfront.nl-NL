---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Nettowaarde berekenen
description: De nettowaarde van een project is de totale verwachte waarde van het project na de berekening van het voordeel en de verwijdering van de kosten.
author: Alina
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# Nettowaarde berekenen

De nettowaarde van een project is de totale verwachte waarde van het project na de berekening van het voordeel en de verwijdering van de kosten. 

## Overzicht van de netto-waarde van het project

Adobe Workfront berekent de nettowaarde van een project aan de hand van de volgende formule: 

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

De volgende velden kunnen van invloed zijn op de nettowaarde van een project:

* **Gepland Voordeel**: Dit is een handingang die door de Eigenaar van het Project wordt gespecificeerd wanneer het voltooien van het **gebied van Info van het Project** van het BedrijfsGeval.\
  Voor meer informatie over het Geplande Voordeel van een project, zie de ](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) sectie van Info van het 0} Project {in artikel [ Overzicht van de Gebieden van het BedrijfsGeval ](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).[

* **Voorspelde Kosten**: Dit is de totale kosten verbonden aan het project zoals geschat wanneer u eerst het project lanceert.

  De **Begrappte Kosten** gebruikt de **Begrappte waarde van de Kosten van de Arbeid** die in het gebied van de Begroting van het Middel van het BedrijfsGeval wordt berekend en het houdt rekening met de uren die voor uw baanrollen in de Planner van het Middel worden begroot en de Kosten per tarief van het Uur van elke baanrol.\
  De begrote Kosten beïnvloedt de **Netto Waarde** van het project. Voor meer informatie over hoe de Begrappte Kosten wordt berekend, zie [ Berekende Begrappte Kosten ](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **Potentiële Kosten van het Risico**: Dit is de kosten verbonden aan om het even welke risico&#39;s op het project, aangezien zij in het BedrijfsGeval, of het lusje van Risico&#39;s van het project worden bepaald.\
  Voor meer informatie over het berekenen van de Potentiële Kosten van het Risico van een project, zie het artikel [ Mogelijke Kosten van het Risico berekenen ](../../../manage-work/projects/project-finances/potential-risk-cost.md).

   

## De netto-waarde van het project zoeken

U kunt de Nettowaarde voor een project in de volgende gebieden in Workfront vinden:

* In Business Case Summary-gebied van de business case \
  Voor meer informatie over het Samenvattingsgebied van het BedrijfsGeval, zie de &quot;Begrijpende Samenvatting van het BedrijfsGeval&quot;sectie in het artikel [ een BedrijfsGeval voor een project ](../../../manage-work/projects/define-a-business-case/create-business-case.md) [ creëren een BedrijfsGeval voor een project ](../../../manage-work/projects/define-a-business-case/create-business-case.md).

  ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* In de Optimizer van het Portfolio als het project met een portefeuille wordt geassocieerd

  >[!TIP]
  >
  >Het totaal van alle netto waarden van het project is de Nettowaarde van de portefeuille.

  Voor meer informatie over Portfolio Optimizer, zie [ overzicht van Optimizer van het Portfolio ](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* Op het gebied van de Netto Waarde van het Project van de volgende lijsten en rapporten:

   * Project
   * Taak
   * Probleem
   * Project (financiële gegevens)

  Voor meer informatie over het creëren van een rapport, zie het artikel [ een douanerapport ](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.
