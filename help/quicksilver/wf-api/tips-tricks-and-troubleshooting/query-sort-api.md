---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Zoekresultaten sorteren in de API
description: Zoekresultaten sorteren in de API
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: 5936982217adc6cfcaf9e400bfff67a1496d3a78
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# Zoekresultaten sorteren in de API

U kunt de resultaten op elk veld sorteren als u het volgende aan uw API-aanroep toevoegt:

```
&entryDate_Sort=asc
```

Als u bijvoorbeeld wilt sorteren op taak Geplande Voltooiingsdatum, verwijdert u `entryDate` en vervangt u deze door `plannedCompletionDate` .

```
&plannedCompletionDate_Sort=asc
```

Dit werkt voor de meeste velden in Adobe Workfront.
