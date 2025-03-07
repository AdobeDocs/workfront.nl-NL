---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: KPI-vragen
description: Uitgebreide query's voor Analytics
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
source-git-commit: eccecaece64b78aa19444407b182ea80b2115a63
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# KPI-vragen

U kunt de vragen in dit artikel gebruiken om gegevensvisualisaties tot stand te brengen gelijkend op die in Verbeterde Analytics.

>[!IMPORTANT]
>
>Zoekopdrachten leveren vergelijkbare resultaten op als in Verbeterde analyse, maar deze komen mogelijk niet exact overeen.


## Vereisten

Voordat u begint, moet u

1. Een verbinding tot stand brengen met uw Business Intelligence-tool (BI):
   1. [Een reader-account of -verbinding maken voor Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)
   1. [Verbinding maken met Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)

Zodra u een verbinding vestigt, kunt u de vragen in dit artikel gebruiken om gegevens te halen en te visualiseren.

## Voltooide projecten

Uit de voltooide KPI-projecten blijkt hoeveel projecten binnen de gefilterde periode zijn voltooid en hoe het percentage is gestegen of gedaald sinds de vorige periode. Onder deze aantallen, kunt u het aantal projecten zien die in de vorige tijdspanne, evenals het aantal dagen in de vorige tijdspanne werden voltooid.

![ voltooide projecten KPI ](assets/kpi-projects-completed-350x182.png)

### Query

```
WITH completedProjectsInRange as ( 
SELECT COUNT(t0.PROJECTID) as PROJECT_COUNT FROM PROJECTS_CURRENT t0 
WHERE t0.ACTUALCOMPLETIONDATE >= '2025-01-01' 
AND t0.ACTUALCOMPLETIONDATE <= '2025-01-31' 
), completedProjectsPreviousRange as ( 
SELECT COUNT(t0.PROJECTID) as PROJECT_COUNT FROM PROJECTS_CURRENT t0 
WHERE t0.ACTUALCOMPLETIONDATE >= '2024-12-01' 
AND t0.ACTUALCOMPLETIONDATE <= '2024-12-31' 
), rawChange as ( 
SELECT (a.PROJECT_COUNT - b.PROJECT_COUNT) as CHANGE_FROM_PREVIOUS_PERIOD FROM completedProjectsInRange a, completedProjectsPreviousRange b 
), percentChange as ( 
SELECT  
CASE 
WHEN a.PROJECT_COUNT = b.PROJECT_COUNT THEN 0.00 
WHEN b.PROJECT_COUNT > 0 THEN ((a.PROJECT_COUNT - b.PROJECT_COUNT) / b.PROJECT_COUNT * 100) 
END AS PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b 
) 
SELECT 
a.PROJECT_COUNT, 
b.PROJECT_COUNT as PREVIOUS_PROJECT_COUNT, 
c.CHANGE_FROM_PREVIOUS_PERIOD, 
d.PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b, rawChange c, 
percentChange d
```

## Projecten tijdig voltooid

De projecten die tijdig zijn voltooid, geven het percentage van de projecten binnen de gefilterde periode aan die op tijd zijn voltooid, en de mate waarin het percentage is gestegen of gedaald sinds de vorige periode. Onder deze aantallen, kunt u het percentage projecten zien die op tijd in de vorige tijdspanne, evenals het aantal dagen in de vorige tijdspanne werden voltooid.

![ KPI projecten die op tijd worden voltooid ](assets/kpi-projects-completed-on-time-350x180.png)

## Gem. projectduur

Het Gem. De projectduur KPI toont de gemiddelde hoeveelheid voltooiingstijd-in dagen, weken, of jaar-voor projecten met daadwerkelijke einddata binnen de gefilterde tijdspanne, evenals hoe het percentage sinds de vorige tijdspanne steeg of daalde. Onder deze aantallen, kunt u de gemiddelde hoeveelheid voltooiingstijd voor projecten met daadwerkelijke einddata in de vorige tijdspanne zien, evenals het aantal dagen in de vorige tijdspanne.

![ KPI gemiddelde projectduur ](assets/kpi-avg.-project-duration-350x168.png)

## Gemiddelde taken per project

Het gemiddelde, de taken per project KPI toont het gemiddelde aantal taken die aan projecten binnen de gefilterde tijdspanne worden toegewezen, evenals hoe het percentage sinds de vorige tijdspanne steeg of daalde. Onder deze aantallen, kunt u het gemiddelde aantal taken zien die aan projecten in de vorige tijdspanne worden toegewezen, evenals het aantal dagen in de vorige tijdspanne.

![ KPI gemiddelde taken per project ](assets/kpi-average-tasks-per-project-350x179.png)