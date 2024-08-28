---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Voorbeelden van query's voor Data Connect
description: Met voorbeeldquery's kunt u uzelf vertrouwd maken met de syntaxis en structuur van specifieke soorten query's.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 84f7f80314e4acafb0414b806f7b1e1e4b2845fc
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Voorbeelden van query&#39;s voor Workfront Data Connect

Om u te helpen beter gebruik te maken van uw Workfront Data Connect-gegevens, bevat deze pagina eenvoudige voorbeeldquery&#39;s waarmee u bekend kunt maken met de syntaxis en structuur van specifieke soorten query&#39;s.

## Aangepaste gegevensquery

In dit voorbeeld wordt getoond hoe u een query kunt samenstellen om aangepaste gegevens in Workfront, zoals aangepaste formulieren en aangepaste velden, te retourneren.

### Scenario:

Uw organisatie die een douaneformulier genoemd de Integratie van de Financiën gebruikt. Het formulier is gekoppeld aan elk project en bevat de volgende velden:

* **BedrijfsEenheid** - een douanegebied dat een koord bevat.
* **ProjectID** - een douanegebied dat een numeriek koord bevat.
* **Uitgebreide Naam van het Project** - een berekend gebied van douanegegevens dat de waarden van BedrijfsEenheid, ProjectID, en de inheemse het projectnaam van Workfront in één enkel koord aaneenschakelt.

U moet deze informatie opnemen in de reactie voor een query op Data Connect. De gegevenswaarden van de douane voor een verslag in het gegevensmeer zijn bevat in een kolom genoemd `parameterValues`. Deze kolom wordt opgeslagen als een JSON-object.

### Query:

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit" :: int as BusinessUnit,
    parametervalues:"DE:Project ID" :: int as ProjectID,
    parametervalues:"DE:Expanded Project Name" :: text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Antwoord

De bovenstaande query retourneert de volgende gegevens:

* `projectid` - de native Workfront-project-id
* `parametervalues` - een kolom waarin een JSON-object wordt opgeslagen
* `name` - de native Workfront-projectnaam
* `Business Unit` - een aangepaste gegevenswaarde die in het `parametervalues` -object wordt opgenomen
* `Project ID` - een aangepaste gegevenswaarde die in het `parametervalues` -object wordt opgenomen
* `Expanded Project Name` - een aangepaste gegevenswaarde die in het `parametervalues` -object wordt opgenomen

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
