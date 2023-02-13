---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Zoekresultaten sorteren in de API
description: Zoekresultaten sorteren in de API
author: John
feature: Workfront API
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# Zoekresultaten sorteren in de API

U kunt de resultaten op elk veld sorteren als u het volgende aan uw API-aanroep toevoegt:

```
&entryDate_Sort=asc
```

Als u bijvoorbeeld wilt sorteren op taak Geplande begindatum, verwijdert u `entryDate` en vervangen door `plannedCompletionDate`.

Dit werkt voor de meeste velden in Adobe Workfront.
