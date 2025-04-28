---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Vragen over projectactiviteiten
description: Uitgebreide query's voor Analytics
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: b7155160-4537-4919-bebf-72056b181bb6
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Vragen over projectactiviteiten

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

## Aanmeldingsgebeurtenissen van gebruikers van projecten

Toont de aantalmensen die aan het project worden toegewezen die op een bepaalde dag het programma opende.

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT 
    tds.projectid, 
    ads.calendardate, 
    count(1) 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN userlogins ul ON ads.assignedtoid = ul.userid and TO_DATE(ul.lastlogindate) = ads.calendardate 
GROUP BY tds.projectid, ads.calendardate
```

### Aanmeldingsgebeurtenissen van gebruikers van projecten: uitvouwen

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 

SELECT 
    tds.projectid, 
    ul.userid, 
    ads.calendardate, 
    count(1) 
FROM assignments_daily_history ads 
INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
INNER JOIN userlogins ul ON ads.assignedtoid = ul.userid AND TO_DATE(ul.lastlogindate) = ads.calendardate 
group by tds.projectid, ul.userid, ads.calendardate
 
```

## De gebeurtenissen van de de taakstatusverandering van projecten de gebruikers

Toont het aantal mensen die de status van een taak voor het project op een bepaalde dag veranderden.

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event 
        WHERE status != 'CPL' 
    )  
    WHERE status != previous_status  
)  
 
SELECT 
    tds.projectid, 
    count(tds.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid AND tsc.taskid = tds.taskid and TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, ads.calendardate
```

### De gebeurtenissen van de de taakstatusverandering van projecten de gebruikers: boor neer

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        lastupdatedbyid, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lastupdatedbyid, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status != 'CPL'  
    )  
    WHERE status != previous_status  
)  
 
SELECT 
    tds.projectid, 
    tsc.lastupdatedbyid, 
    count(tsc.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid AND tsc.taskid = tds.taskid AND TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, tsc.lastupdatedbyid, ads.calendardate
```

## Projecten van de taakvoltooiing van gebruikers

Het aantal personen tonen dat een taak voor het project op een bepaalde dag heeft voltooid.

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status = 'CPL'  
    )  
    WHERE status != previous_status  
) 
 
SELECT 
    tds.projectid, 
    count(tds.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid and tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid and tsc.taskid = tds.taskid and TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, ads.calendardate
```

### De gebeurtenissen van de de taakvoltooiing van projecten van gebruikers: boor neer

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        lastupdatedbyid, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lastupdatedbyid, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status = 'CPL'  
    )  
    WHERE status != previous_status  
)  
 
SELECT 
    tds.projectid, 
    tsc.lastupdatedbyid, 
    count(tsc.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid AND tsc.taskid = tds.taskid AND TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, tsc.lastupdatedbyid, ads.calendardate
```
