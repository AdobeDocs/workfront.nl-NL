---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Voorbeelden van query's voor Data Connect
description: Met voorbeeldquery's kunt u uzelf vertrouwd maken met de syntaxis en structuur van specifieke soorten query's.
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Voorbeelden van query&#39;s voor Workfront Data Connect

Om u te helpen beter gebruik te maken van uw Workfront Data Connect-gegevens, bevat deze pagina eenvoudige voorbeeldquery&#39;s waarmee u bekend kunt maken met de syntaxis en structuur van specifieke soorten query&#39;s.

## Aangepaste gegevensquery

In dit voorbeeld wordt getoond hoe u een query kunt samenstellen om aangepaste gegevens in Workfront, zoals aangepaste formulieren en aangepaste velden, te retourneren.

### Scenario:

Uw organisatie gebruikt een douanevorm genoemd de Integratie van de Financiën. Het formulier is gekoppeld aan elk project en bevat de volgende velden:

* **BedrijfsEenheid** - een douanegebied dat een koord bevat.
* **ProjectID** - een douanegebied dat een numeriek koord bevat.
* **Uitgebreide Naam van het Project** - een berekend gebied van douanegegevens dat de waarden van BedrijfsEenheid, ProjectID, en de inheemse het projectnaam van Workfront in één enkel koord aaneenschakelt.

U moet deze informatie opnemen in de reactie voor een query op Data Connect. De gegevenswaarden van de douane voor een verslag in het gegevensmeer zijn bevat in een kolom genoemd `parametervalues`. Deze kolom wordt opgeslagen als een JSON-object.

### Query:

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit"::int as BusinessUnit,
    parametervalues:"DE:Project ID"::int as ProjectID,
    parametervalues:"DE:Expanded Project Name"::text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Reactie:

De bovenstaande query retourneert de volgende gegevens:

* `projectid` - de native Workfront-project-id
* `parametervalues` - een kolom waarin een JSON-object wordt opgeslagen
* `name` - de native Workfront-projectnaam
* `Business Unit` - een aangepaste gegevenswaarde die in het `parametervalues` -object wordt opgenomen
* `Project ID` - een aangepaste gegevenswaarde die in het `parametervalues` -object wordt opgenomen
* `Expanded Project Name` - een aangepaste gegevenswaarde die in het `parametervalues` -object wordt opgenomen

### Uitleg:

Wanneer u het JSON-object `parametervalues` opvraagt, kunt u elk aangepast gegevensveld benaderen als een kolom met behulp van de volgende code:

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>` is de naam van het JSON-object in de tabel die wordt opgevraagd. In het geval van aangepaste gegevens is dit altijd `parametervalues` .
* `<parameter_name>` is de `parametername` -tekenreeks die wordt gevonden in het gereedschap Formulierconfiguratie, hoewel deze mogelijk niet altijd overeenkomt met deze waarde.

>[!NOTE]
>
>Als de naam van de parameter wordt gewijzigd in het Workfront-formulierconfiguratieprogramma, wordt deze weergegeven als een nieuwe kolom in het JSON-object. Daarom raden we u aan de naam van een kolom niet te wijzigen als deze eenmaal is gemaakt met het gereedschap Formulierconfiguratie. Het label kan echter worden gewijzigd zonder dat dit van invloed is op het JSON-object.
>
>Als de tekstreeks voor de parameternaam onjuist is, retourneert de kolom de waarde NULL in plaats van een fout.

* `<data_type>` converteert de waarde die wordt geretourneerd van het JSON-object naar een gegevenstype dat geschikt is voor het veld. Als u een niet-compatibel gegevenstype kiest voor de waarde die wordt geretourneerd, treedt er een fout op bij een datatype dat niet overeenkomt. Mogelijke gegevenstypen zijn:

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)` (`Number(32,4)` retourneert bijvoorbeeld 1234.0987)
   * `date`
   * `timestamp`

* `<column_name>` is het label dat u voor elke kolom met aangepaste gegevens maakt.

>[!NOTE]
>
>Alleen parameters waaraan waarden in het formulier zijn toegewezen, worden opgenomen in het JSON-object. Als een aangepast gegevensveld leeg is op het formulier, wordt het niet weergegeven.

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
