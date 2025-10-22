---
title: Grondbeginselen van Adobe Workfront Planning API
description: Het doel voor de Planning API van Adobe Workfront is het vereenvoudigen van de bouwintegratie met Planning door een REST-ful architectuur in te voeren die over HTTP werkt. In dit document wordt ervan uitgegaan dat u bekend bent met REST- en JSON-reacties en wordt de aanpak beschreven die door de API voor planning wordt gevolgd.
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1009'
ht-degree: 1%

---


# Basisbeginselen van de API voor Adobe Workfront-planning

{{planning-important-intro}}

Het doel voor de Planning API van Adobe Workfront is het vereenvoudigen van de bouwintegratie met Planning door een REST-ful architectuur in te voeren die over HTTP werkt. In dit document wordt ervan uitgegaan dat u bekend bent met REST- en JSON-reacties en wordt de aanpak beschreven die door de API voor planning wordt gevolgd.

Een vertrouwdheid met het schema van de Planning van Workfront zal u in het begrip van de gegevensbestandverhoudingen helpen die kunnen worden gebruikt om gegevens uit de Planning van Workfront voor integratiedoeleinden te trekken.

U kunt de API voor planning oproepen vanuit een extern opzoekveld in een aangepast Workfront-formulier.

Voor meer informatie over Externe raadplegingsgebieden, zie [&#x200B; Voorbeelden van het Externe raadplegingsgebied in een douanevorm &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>Wanneer u de plannings-API gebruikt, wordt alle informatie over de gebruiker geretourneerd met de gebruikers-id van Adobe Identity Management System (IMS) en niet met de gebruikers-id van Workfront.
>
>Voor informatie, zie [&#x200B; gebruikers in Adobe Admin Console &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md) leiden.

## URL Workfront-plannings-API

<!--For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

### Bewerkingen

Objecten worden gemanipuleerd door een HTTP-aanvraag naar hun unieke URI te verzenden. De uit te voeren bewerking wordt opgegeven door de HTTP-methode.

De standaard HTTP-methoden komen overeen met de volgende bewerkingen:

* **GET** - wint een voorwerp door identiteitskaart terug, onderzoeken naar alle voorwerpen door een vraag
* **POST** - neemt een nieuw voorwerp op
* **PUT** - geeft een bestaand voorwerp uit
* **DELETE** - schrapt een voorwerp

Voor meer details en voorbeelden van elke verrichting, zie de [&#x200B; de ontwikkelaarsdocumentatie van de Planning API van Workfront &#x200B;](https://developer.adobe.com/wf-planning/).

### Veldtypen en zoekopties die hiermee worden gebruikt

Met wijzigingstoetsen en filters kunt u bepalen welke gegevens in de resultaten worden geretourneerd.

<!--For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

#### Zoekopties gebruiken

Workfront Planning ondersteunt de volgende zoekopties:

<table>
    <tr>
        <td><b>Modifier</b></td>
        <td><b>Voorbeeld</b></td>
        <td><b>Beschrijving</b></td>
        <td><b>Mogelijke waarden</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Retourneert records waarvan de veldwaarde het filter bevat  </td>
        <td>"Nieuwe productlancering"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Hiermee worden records geretourneerd waarin de veldwaarde het filter niet bevat  </td>
        <td>"New Launch"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Hiermee worden records geretourneerd waarvan de veldwaarde exact overeenkomt met het filter  </td>
        <td>"Nieuwe productlancering"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Hiermee worden records geretourneerd waarvan de veldwaarde exact overeenkomt met het filter  </td>
        <td>"Nieuwe productlancering"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Retourneert records waarvan de veldwaarde niet leeg is  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Retourneert records waarvan de veldwaarde niet leeg is  </td>
        <td>"Nieuwe productlancering"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Hiermee worden records geretourneerd waarvan de veldwaarde groter is dan het filter  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Hiermee worden records geretourneerd waarvan de veldwaarde groter is dan of gelijk is aan het filter  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Hiermee worden records geretourneerd waarvan de veldwaarde kleiner is dan het filter  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Hiermee worden records geretourneerd waarvan de veldwaarde kleiner dan of gelijk is aan het filter </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Hiermee worden records geretourneerd waarvan de veldwaarde na het filter ligt  </td>
        <td>"2024-05-15T20 :00: 00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Hiermee worden records geretourneerd waarvan de veldwaarde vóór het filter ligt </td>
        <td>"2024-05-12T20 :00: 00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Hiermee worden records geretourneerd waarvan de veldwaarde zich tussen de filters bevindt  </td>
        <td><ul><li>"2024-05-12T20 :00: 00.000Z" </li><li>"2024-05-14T20 :00: 00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Hiermee worden records geretourneerd waarvan de veldwaarde zich niet tussen het filter bevindt  </td>
        <td><ul><li>"2024-05-09T20 :00: 00.000Z"  </li><li>"2024-05-17T20 :00: 00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Hiermee worden records geretourneerd waarvan de veldwaarde een van de filters is  </td>
        <td><ul><li>"active" </li><li>"completed" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Hiermee worden records geretourneerd waarvan de veldwaarde geen van de filters is </td>
        <td><ul><li>"voltooid"  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Hiermee worden records geretourneerd waarvan de veldwaarde een filter heeft  </td>
        <td><ul><li>["actief", "vast"]  </li><li>["fixed", "completed", "completed"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Hiermee worden records geretourneerd waarvan de veldwaarde alle filters bevat  </td>
        <td><ul><li>["actief", "voltooid"]   </li><li>["actief", "voltooid", "voltooid"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Hiermee worden records geretourneerd waarvan de veldwaarde geen filter heeft </td>
        <td>["fixed", "completed"]  </td>
    </tr>
    <tr>
        <td>$isPrecies </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Hiermee worden records geretourneerd waarvan de veldwaarde exact het filter is  </td>
        <td>["actief", "voltooid"]  </td>
    </tr>
</table>

#### Veldtypen

Hieronder ziet u de lijst met ondersteunde veldtypen en de zoekopties die u kunt gebruiken voor elk van deze veldtypen

| Veldtype | Ondersteunde zoekopties |
|---|---|
| text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| met lange tekst | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| getal | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| percentage | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| valuta | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| date | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| eenmalig | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| multi-select | $hasAnyOf, $hasAllOf, $isPrecies, $hasNoneOf, $isEmpty, $isNotEmpty |
| boolean | $is |
| user | $hasAnyOf, $hasAllOf, $isPrecies, $hasNoneOf, $isEmpty, $isNotEmpty |
| formule | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| gemaakt door | $is, $isNot, $isAnyOf, $isNoneOf |
| gemaakt op | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| bijgewerkt | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| bijgewerkt op | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| referentie | $hasAnyOf, $hasAllOf, $isPrecies, $hasNoneOf, $isEmpty, $isNotEmpty |
| opzoeken | Afhankelijk van het gekoppelde veld |

### Instructies &quot;And&quot; en &quot;Or&quot; gebruiken

In de API-aanroep kunt u filters hebben die zijn gebaseerd op verschillende criteria gecombineerd met instructies $and&quot; en &quot;$or&quot;

```
{
  "recordTypeId": "recordTypeId",
  "offset": "integer",
  "limit": "integer",
  "filters": [
    {
      "$or": [
        {
          "launch_date": {
            "$isBetween": [
              "2024-03-31T20:00:00.000Z",
              "2024-04-01T20:00:00.000Z"
            ]
          }
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-03-31T20:00:00.000Z",
                  "2024-04-01T20:00:00.000Z"
                ]
              }
            },
            {
              "status": "active"
            }
          ]
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-04-15T00:00:00.000Z",
                  "2024-04-16T00:00:00.000Z"
                ]
              }
            },
            {
              "status": "planned"
            }
          ]
        }
      ]
    }
  ]
}
```

### De parameter voor veldaanvragen gebruiken

U kunt de parameter van het gebiedsverzoek gebruiken om een komma-gescheiden lijst van specifieke gebieden te specificeren die zouden moeten worden teruggekeerd. Deze veldnamen zijn hoofdlettergevoelig.

De aanvraag

`/v1/records/search?attributes=data,createdBy`

```
{
    "records": [
        {
            "id": "Rc6527ecb35df57c441d92ba00",
            "createdBy": "61a9cc0500002f9fdaa7a6f824f557e1",
            "createdAt": null,
            "updatedBy": null,
            "updatedAt": null,
            "customerId": null,
            "imsOrgId": null,
            "recordTypeId": null,
            "data": {
                "F666c0b58b6fee61a2ea6ea81": [
                    {
                        "externalId": null,
                        "id": "Rc665728ff95730b58bc757b13",
                        "value": null
                    },
..
```

retourneert een reactie die lijkt op het volgende:


```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Zoekresultaten sorteren in de API

U kunt de resultaten op elk veld sorteren als u het volgende aan uw API-aanroep toevoegt:


`/v1/records/search`

Instantie van aanvraag:

```
{
    "recordTypeId": "Rt6527ecb25df57c441d92b9fa",
    "filters": [],
    "sorting": [
        {
            "fieldId": "F6527ecb25df57c441d92b9fc",
            "direction": "asc"
        },
        {
            "fieldId": "F658afcbd4a0273c67c346fd5",
            "direction": "desc"
        }
    ],
    "limit": 500,
    "offset": 0,
    "rowOrderViewId": "V6527ecb75df57c441d92ba03",
    "groupingFieldIds": []
}
```

### Zoeklimieten en gepagineerde reacties

Standaard retourneren API-aanvragen 500 resultaten, vanaf het begin van de lijst. Als u de standaardbeperking voor het aantal resultaten wilt overschrijven, gebruikt u de parameter `limit` in uw aanvragen en stelt u deze in op een ander getal, met maximaal 2000 resultaten.

We raden u aan gepagineerde reacties voor grote gegevenssets te gebruiken door de parameter `offset` aan uw aanvragen toe te voegen. Met gepagineerde reacties kunt u de locatie opgeven van het eerste resultaat dat moet worden geretourneerd.

Als u bijvoorbeeld de resultaten 2001-4000 wilt retourneren, kunt u de volgende aanvraag gebruiken. Dit voorbeeld keert 2000 verslagen terug die in actieve status zijn, die van het resultaat van 2001st beginnen:

`POST /v1/records/search`



Instantie van aanvraag:

```
{ 
    "recordTypeId": "recordTypeId", 
    "offset": "2001", 
    "limit": "2000", 
    "filters": [ 
        { "status": "active" } 
    ] 
} 
```

Gebruik een sorteerparameter om ervoor te zorgen dat de resultaten correct worden gepagineerd. Hierdoor kunnen de resultaten in dezelfde volgorde worden geretourneerd, zodat de paginering de resultaten niet herhaalt of overslaat.

Voor meer informatie bij het sorteren, zie [&#x200B; Sorterend vraagresultaten in API &#x200B;](#sorting-query-results-in-the-api) in dit artikel.
