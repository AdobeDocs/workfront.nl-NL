---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Rendement op investering berekenen (ROI)
description: Rendement op Investering (ROI) is de metrische factor van Adobe Workfront die portefeuillebeheerders toestaat om snel te zien hoe het project tegen het oorspronkelijke Geplande Voordeel en de Gefabriceerde Kosten van het project presteert.
author: Alina
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Rendement op investering berekenen (ROI)

Rendement op Investering (ROI) is de metrische factor van Adobe Workfront die portefeuillebeheerders toestaat om snel te zien hoe het project tegen het oorspronkelijke Geplande Voordeel en de Gefabriceerde Kosten van het project presteert.

## Overzicht van het investeringsrendement van het project

Workfront berekent ROI met de volgende formule:

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

De volgende gebieden beïnvloeden ROI van een project:

* **Gepland projectvoordeel**: Dit is een handmatige vermelding die door de projecteigenaar is opgegeven bij het invullen van het gebied Projectinfo van de bedrijfscase. Dit is een schatting van wat u, als de Eigenaar van het Project, denkt dat het voordeel van het project zou kunnen zijn als u het project voltooit. Dit is een specifiek bedrag aan valuta en het moet een positieve waarde zijn.\
   Voor meer informatie over het Geplande Voordeel van een project, zie de sectie &quot;Info van het Project&quot;in het artikel [Een bedrijfscase maken voor een project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **Geraamde projectkosten**: Dit zijn de totale kosten verbonden aan het project zoals geschat wanneer u het project eerst lanceert.

   De **Geraamde kosten** gebruikt de **begrote arbeidskosten** Waarde die wordt berekend in het gebied van de Begroting van het Middel van het BedrijfsGeval en het houdt rekening met de uren die voor uw baanrollen in de Planner van het Middel worden begroot en het tarief van Kosten per Uur van elke baanrol.\
   Zie voor meer informatie [Geraamde kosten berekenen](../../../manage-work/projects/project-finances/budgeted-cost.md).

## Zoek het investeringsrendement van het project

U kunt de ROI-waarde voor een project in de volgende gebieden in Workfront weergeven:

* In Portfolio optimizer als het project met een portefeuille wordt geassocieerd

   >[!NOTE]
   >
   >Het totaal van alle ROI-waarden van het project is het investeringsrendement van de portefeuille.

   Raadpleeg het artikel voor informatie over de Portfolio Optimizer [Overzicht van Portfolio optimaliseren](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* Op het gebied van het ROI van het Project in de volgende lijsten en rapporten: 

   * Project
   * Taak
   * Probleem
   * Project (financiële gegevens)
   Raadpleeg het artikel voor meer informatie over het samenstellen van rapporten in Workfront [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
