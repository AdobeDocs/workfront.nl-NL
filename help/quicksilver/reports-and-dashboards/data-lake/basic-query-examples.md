---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Voorbeelden van query's voor Data Connect
description: Met voorbeeldquery's kunt u uzelf vertrouwd maken met de syntaxis en structuur van specifieke soorten query's.
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: c8a25bcc8c9b56a649ca7764918c86f9cdd5b3e2
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Voorbeelden van query&#39;s voor Workfront Data Connect

Om u te helpen beter gebruik te maken van uw Workfront Data Connect-gegevens, bevat deze pagina eenvoudige voorbeeldquery&#39;s waarmee u bekend kunt maken met de syntaxis en structuur van specifieke soorten query&#39;s.

## Aangepaste gegevensquery

In dit voorbeeld wordt getoond hoe u een query kunt samenstellen om aangepaste gegevens in Workfront, zoals aangepaste formulieren en aangepaste velden, te retourneren.

### Scenario

Uw organisatie gebruikt een douanevorm genoemd de Integratie van de Financiën. Het formulier is gekoppeld aan elk project en bevat de volgende velden:

* **BedrijfsEenheid**: Een douanegebied dat een koord bevat.
* **ProjectID**: Een douanegebied dat een numeriek koord bevat.
* **Uitgebreide Naam van het Project**: Een berekend gebied van douanegegevens dat de waarden van BedrijfsEenheid, ProjectID, en de inheemse het projectnaam van Workfront in één enkel koord aaneenschakelt.

U moet deze informatie opnemen in de reactie voor een query op Data Connect. De gegevenswaarden van de douane voor een verslag in het gegevensmeer zijn bevat in een kolom genoemd `parametervalues`. Deze kolom wordt opgeslagen als een JSON-object.

### Query

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

### Antwoord

De bovenstaande query retourneert de volgende gegevens:

* `projectid`: De native Workfront-project-id.
* `parametervalues`: Een kolom waarin een JSON-object wordt opgeslagen.
* `name`: De native Workfront-projectnaam.
* `Business Unit`: Een aangepaste gegevenswaarde die in het `parametervalues` -object wordt opgenomen.
* `Project ID`: Een aangepaste gegevenswaarde die in het `parametervalues` -object wordt opgenomen.
* `Expanded Project Name`: Een aangepaste gegevenswaarde die in het `parametervalues` -object wordt opgenomen.

### Toelichting

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

## Tijd in statusquery

In dit voorbeeld wordt getoond hoe u de tijd meet die een project in eerder toegewezen statussen heeft doorgebracht. Het kan gemakkelijk worden aangepast om taak te meten of tijd uit te geven in een status, of het kan worden aangepast om te meten hoe lang een voorwerp om het even welk ander attribuut (met inbegrip van douanegegevenswaarden) had toegepast.

### Scenario

Uw leiderschap van uw organisatie gelooft dat u te veel tijd besteedt in elke fase van uw werklevenscyclus. Voordat u aanbevelingen doet om het proces te verbeteren, wilt u een basislijnmeting maken van hoe vaak een projectstatus verandert in de loop van de tijd en hoeveel dagen een project in een bepaalde status blijft.

U gaat de PROJECTS_EVENT gegevensmening gebruiken om in een lijst van elke statusverandering tegen het projectvoorwerp te trekken. U zult de nieuwe status met de vorige status vergelijken, zal de efficiënte tijdwaaier voor de eerder toegewezen status grijpen, en dan de dagen berekenen besteed in die status.

Gebruikend deze ruwe output van tijd die in elke status per project wordt doorgebracht, kunt u beginnen visualisaties te bouwen of de gegevens verder samen te voegen om de gemiddelden van de statusduur door status, projecttype, of tijd van jaar te bouwen. Deze basislijn wordt dan gebruikt om een benchmark te plaatsen u tegen kunt meten om aan de verwachtingen van uw leiderschap te voldoen.

De volgende query gebruikt de gegevensweergave Data Connect PROJECTS_EVENTS om elke gebeurtenis van de projectstatus te vergelijken en de tijd in status weer te geven.

### Query

```
-- Calculate the begin/end effective timestamp and duration in days 

SELECT 

    projectid, 
    name as project_name, 
    prev_status as previous_status, 
    status, 
    status_change_date as status_begin_effective_timestamp, 
    case 
        when status_change_date is null then NULL
        else
            nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp) 
    end as status_end_effective_timestamp, 
    datediff('DAYS',status_change_date, nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp)) as status_duration_days 

FROM 
    ( -- Filter to just the records that have changed 
     SELECT projectid, 
        name, 
        prev_status, 
        status, 
        begin_effective_timestamp as status_change_date    
     FROM 
        (  -- Calculate records where previous status is different 
          SELECT DISTINCT  
           pe.projectid, 
           pe.name AS name, 
           pe.STATUS, 
           nvl(lag(pe.STATUS) over (partition by pe.projectid order by pe.BEGIN_EFFECTIVE_TIMESTAMP), status) prev_status, 
           begin_effective_timestamp 

          FROM projects_event pe 
         -- Set any WHERE conditions to limit the results as needed 
         --WHERE 
            -- pe.PROJECTID = '5ebe…c1e1' 
        ) 
        WHERE prev_status != status 
    ) 
    order by status_change_date; 
```

### Antwoord

De bovenstaande query retourneert de volgende gegevens:

* `PROJECTID`: De Workfront-project-id die is gekoppeld aan de gebeurtenis status change.
* `PROJECT_NAME`: De Workfront-projectnaam.
* `PREVIOUS_STATUS`: De status van het project vlak voor de wijziging.
* `STATUS`: De status van het project na de wijziging.
* `STATUS_BEGIN_EFFECTIVE_TIMESTAMP`: De tijdstempel van de gebeurtenis change toen de vorige status werd ingesteld.
* `STATUS_END_EFFECTIVE_TIMESTAMP`: De tijdstempel van de gebeurtenis change wanneer de bijgewerkte statuswaarde is ingesteld.
* `STATUS_DURATION_DAYS`: Het verschil (in dagen) tussen de effectieve eindtijdstempel en de effectieve begintijdstempel.

### Toelichting

De query gebruikt de mogelijkheden voor het bijhouden van wijzigingsgebeurtenissen van Data Connect.  Hiermee wordt de datum bepaald waarop een gebeurtenis met een andere nieuwe statuswaarde dan de vorige gebeurtenis is geactiveerd. 

Het onderzoeken van de vraag van binnenuit: 

1. Records berekenen waarbij de vorige status anders is: 
   * Voor elke veranderingsgebeurtenis, gebruik de lag () functie om de vorige waarde van status te identificeren. 

2. Filteren naar alleen de records die zijn gewijzigd: 

   * Selecteer records uit berekening in stap 1 waar de vorige status zich bevindt!= huidige status. 

3. Bereken het effectieve begin/einde-tijdstempel en de duur in dagen: 

   * `<status_begin_effective_timestamp>`: Berekend in stap 2. 

   * `<status_end_effective_timestamp>`: Berekend op basis van de volgende instructie (lead()). `<status_begin_effective_timestamp>`: alleen de status weergeven als `<status_begin_effective_timestamp>` NIET NULL is. 
   * `<status_duration_days>`: gegevensverschil tussen `<status_begin_effective_timestamp>` en `<status_end_effective_timestamp>` . 

>[!NOTE]
>
>Het is raadzaam deze query als een eigen &quot;Weergave&quot; in PowerBI of Tableau te gebruiken.  Als u andere velden vanuit de `<object>_event view` wilt inbrengen, voegt u de uitvoer van deze query terug naar de `<object>_event view` .  De samenvoegvelden zijn als volgt: <br>
>>Voor project_event: 
>>`From projects_event p`
>>`Join <above query> c on c.projectid = p.projectid  `
>>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`



<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
