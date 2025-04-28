---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Vragen over projectmanagement
description: Uitgebreide query's voor Analytics
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 3943703a-0d0b-46d3-a708-52987d330523
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 0%

---

# Vragen over projectmanagement

U kunt de vragen in dit artikel gebruiken om gegevensvisualisaties tot stand te brengen gelijkend op die in Verbeterde Analytics.

>[!IMPORTANT]
>
>Zoekopdrachten leveren vergelijkbare resultaten op als in Verbeterde analyse, maar deze komen mogelijk niet exact overeen.


## Vereisten

Voordat u begint, moet u

1. Een verbinding tot stand brengen met uw Business Intelligence-tool (BI):
   1. [Een reader-account of -verbinding maken voor Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)
   1. [Verbinding maken met Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)

Nadat u een verbinding hebt gemaakt, kunt u de query&#39;s in dit artikel gebruiken om gegevens te extraheren en visualiseren.

## Geplande gepensioneerde projecten

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        workrequired, 
        percentcomplete, 
        calendardate, 
        (workrequired - (workrequired * percentcomplete)) as remainingMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.workrequired) as projectTotalWork, 
    sum(tdw.remainingMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

### Geplande gepensioneerde projecten: opsluiting

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        workrequired, 
        percentcomplete, 
        calendardate, 
        (workrequired - (workrequired * percentcomplete)) as remainingMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.workrequired) as projectTotalWork, 
    sum(tdw.remainingMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

## Geplande looptijd van projecten 

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        planneddurationminutes, 
        percentcomplete, 
        calendardate, 
        (planneddurationminutes - (planneddurationminutes * percentcomplete)) as remainingDurationMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.planneddurationminutes) as projectTotalWork, 
    sum(tdw.remainingDurationMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

### Geplande duur van de projecten: afboeking

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        planneddurationminutes, 
        percentcomplete, 
        calendardate, 
        (planneddurationminutes - (planneddurationminutes * percentcomplete)) as remainingDurationMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.planneddurationminutes) as projectTotalWork, 
    sum(tdw.remainingDurationMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```
