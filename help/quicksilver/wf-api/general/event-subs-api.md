---
content-type: api
navigation-topic: general-api
title: API voor abonnementen voor gebeurtenissen
description: API voor abonnementen voor gebeurtenissen
author: Becky
feature: Workfront API
role: Developer
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: c08bd3311892d24a9bd40af138169957f5ea2ca4
workflow-type: tm+mt
source-wordcount: '2126'
ht-degree: 0%

---


# API voor abonnementen voor gebeurtenissen

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

Wanneer een actie op een voorwerp van Adobe Workfront voorkomt dat door gebeurtenisabonnementen wordt gesteund, kunt u Workfront vormen om een reactie naar uw gewenste eindpunt te verzenden. Dit betekent dat toepassingen van derden updates van Workfront-interacties kunnen ontvangen via de Workfront API kort nadat ze zich voordoen. Over het algemeen kunt u verwachten dat u binnen 5 seconden vanaf het moment dat de gegevenswijziging wordt geregistreerd, webhaakmeldingen ontvangt. Gemiddeld ontvangen klanten binnen minder dan 1 seconde berichten via een webhaak vanaf de gegevenswijziging die wordt geregistreerd.  

Als u via uw firewall gebeurtenisabonnementen wilt ontvangen, moet u de volgende IP-adressen aan uw lijst van gewenste personen toevoegen:

**Voor klanten in Europa:**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**Voor klanten op andere locaties dan Europa:**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

De volgende onderwerpen ondersteunen de API voor abonnementen op gebeurtenissen:

## Objecten ondersteund door gebeurtenisabonnementen

De volgende Workfront-objecten worden ondersteund door gebeurtenisabonnementen.

* Toewijzing
* Bedrijf
* Dashboard
* Document
* Kosten
* Veld
* Uur
* Probleem
* Opmerking
* Portfolio
* Programma
* Project
* Opnemen
* Recordtype
* Rapport
* Taak
* Sjabloon
* Tijdschema
* Gebruiker
* Werkruimte

Zie voor een lijst met velden die worden ondersteund door gebeurtenisabonnementsobjecten [Bronvelden voor abonnementen](../../wf-api/api/event-sub-resource-fields.md).

## Verificatie van abonnement op gebeurtenis

Uw Workfront-gebruiker heeft het volgende nodig om een gebeurtenissenabonnement te maken, te vragen of te verwijderen:

* Een toegangsniveau van &quot;Beheerder van het Systeem&quot;wordt vereist om de Abonnementen van de Gebeurtenis te gebruiken.
* A `sessionID`  header is vereist om de API voor abonnementen op gebeurtenissen te gebruiken

  Zie voor meer informatie [Verificatie](api-basics.md#authentication) in [API-basisbeginselen](api-basics.md).

## Het vormen van het Middel van het Abonnement

De abonnementsbron bevat de volgende velden.

* objId (optioneel)

   * **String** - De id van het object van de opgegeven objCode waarvoor gebeurtenissen worden geactiveerd. Als dit veld niet is opgegeven, ontvangt de gebruiker gebeurtenissen voor alle objecten van het opgegeven type.

* objCode (vereist)

   * **String** - De objCode van het voorwerp dat aan veranderingen wordt geabonneerd. De mogelijke waarden voor objCode worden in de onderstaande tabel weergegeven.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <thead> 
       <tr> 
        <th><p>Object</p></th> 
        <th><p>objCode</p></th> 
       </tr> 
      </thead> 
      <tbody> 
       <tr> 
        <td scope="col">Toewijzing</td> 
        <td scope="col"><p>ASSGN</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Bedrijf </td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Dashboard</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Document</p></td> 
        <td scope="col">DOCU </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Kosten</p></td> 
        <td scope="col">EXPNS</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Veld</p></td> 
        <td scope="col"><p>VELD</p></td> 
       </tr> 
      <tr> 
        <td scope="col"><p>Uur</p></td> 
        <td scope="col">UUR</td> 
       </tr> 
       <tr> 
        <td scope="col">Probleem</td> 
        <td scope="col"><p>OPTASK</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Opmerking</td> 
        <td scope="col">OPMERKING</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Portfolio</p></td> 
        <td scope="col"><p>POORT</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Programma</p></td> 
        <td scope="col"><p>PRGM</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Project</p></td> 
        <td scope="col"><p>PROJ</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Opnemen</p></td> 
        <td scope="col"><p>RECORD</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Recordtype</p></td> 
        <td scope="col"><p>RECORD_TYPE</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Rapport</p></td> 
        <td scope="col"><p>PTLSEC</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Taak</p></td> 
        <td scope="col"><p>TAAK</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Sjabloon</p></td> 
        <td scope="col"><p>TMPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Tijdschema</td> 
        <td scope="col">TSHET</td> 
       </tr> 
       <tr> 
        <td scope="col">Gebruiker</td> 
        <td scope="col">GEBRUIKER</td> 
       </tr> 
       <tr> 
        <td scope="col">Werkruimte</td> 
        <td scope="col">WERKRUIMTE</td> 
       </tr> 
      </tbody> 
     </table>

* eventType (vereist)

   * **String** - Een waarde die het type gebeurtenis vertegenwoordigt waarop het object is geabonneerd. De beschikbare gebeurtenistypen zijn:

      * MAKEN
      * DELETE 
      * BIJWERKEN

* url (vereist)

   * **String** - De URL van het eindpunt waarnaar abonnementsgebeurtenistaken via HTTP worden verzonden.

* authToken (vereist)

   * **String** - Het token OAuth2 dat wordt gebruikt voor verificatie met de URL die is opgegeven in het veld URL. 

## API-aanvragen voor abonnementen voor gebeurtenissen maken

Nadat u ervoor hebt gezorgd dat de gebruiker beheerderstoegang heeft en de abonneebron vormt, bent u klaar om gebeurtenisabonnementen te maken.

Gebruik de volgende syntaxis om de URL samen te stellen.

**Aanvraag-URL:**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Aanvraagkoppen:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Naam koptekst</p> </th> 
   <th> <p>Waarde koptekst</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Inhoudstype</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID, waarde</p> </td> 
  </tr> 
 </tbody> 
</table>

**Voorbeeld hoofdtekst aanvraag:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua",
                "authToken": "EauthTokenWorkfrontRocks1234_"
            }
```

| Antwoordcode | Beschrijving |
|---|---|
| 201 | Het gebeurtenisabonnement is gemaakt. |
| 400 (Ongeldige aanvraag) | Het URL-veld van de abonnementsbron werd als ongeldig beschouwd. |
| 401 (Niet-geautoriseerd) | De opgegeven sessionID is leeg of wordt als ongeldig beschouwd. |
| 403 (verboden) | De gebruiker die de verstrekte sessionID aanpast heeft beheerdertoegang niet. |

Als u een abonnementsbron doorgeeft als de hoofdtekst van een aanvraag (waarbij het inhoudstype &#39;application/json&#39; is), wordt een gebeurtenisabonnement gemaakt voor het opgegeven object. Een antwoordcode van 201 (Gemaakt) geeft aan dat het abonnement is gemaakt. Een andere antwoordcode dan 201 betekent dat het abonnement **NOT** gemaakt.

>[!NOTE]
>
> De responsheader &#39;Locatie&#39; bevat de URI van het zojuist gemaakte gebeurtenisabonnement.

**Voorbeeld van responsheaders:**

| Antwoordheaders | Voorbeeld |
|---|---|
| Content-Length | `→0` |
| Datum | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| Locatie | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| Server | `→Apache-Coyote/1.1` |

## Abonnementen voor opvragen van gebeurtenissen

Bij het opvragen van Workfront HTTP gebruikt u de methode GET. Er zijn twee manieren om te zoeken naar gebeurtenisabonnementen: query op abonnement-id (zie hieronder) of vraag naar alle gebeurtenisabonnementen.

### Query uitvoeren op alle abonnementen voor gebeurtenissen

U kunt alle gebeurtenissenabonnementen voor een klant vragen, of het volgende gebruiken om de reactie te beheren. U kunt ook de volgende opties gebruiken om de reactie te beheren:

* **page**: optie voor queryparameter om op te geven hoeveel pagina&#39;s moeten worden geretourneerd. De standaardwaarde is 1.
* **limiet**: optie voor queryparameter om het aantal resultaten op te geven dat per pagina moet worden geretourneerd. De standaardwaarde is 100 met een maximum van 1000.

De aanvraagsyntaxis voor het aanbieden van alle gebeurtenisabonnementen voor een specifieke klant is als volgt:

**Aanvraag-URL:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Aanvraagkoppen:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Naam koptekst</p> </th> 
   <th> <p>Waarde koptekst</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID, waarde</p> </td> 
  </tr> 
 </tbody> 
</table>

**Responscodes:**

| Antwoordcode | Beschrijving |
|---|---|
| 200 | Het verzoek is geretourneerd met alle gebeurtenisabonnementen die zijn gevonden voor de klant die overeenkomt met de opgegeven sessionID. |
| 401 (Niet-geautoriseerd) | De opgegeven sessionID is leeg. |
| 403 (verboden) | De gebruiker, die verstrekte sessionID aanpast, heeft beheerdertoegang niet. |


**Voorbeeld van responsheaders:**

| Reactiekoptekst | Voorbeeld |
|---|---|
| Inhoudstype | `→application/json;charset=UTF-8` |
| Datum | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| Server | `→Apache-Coyote/1.1` |
| Overdrachtscodering | `→chunked` |


**Voorbeeld van reactiebody:**

<!-- [Copy](javascript:void(0);) -->

```
                {
                "subscriptions":                
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": "ObjId1234",
                "objCode": "TASK",
                "url": "http://test.test.net/test/1234",
                "eventType": "UPDATE",
                "authToken": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
                ],
                "meta":
                {
                "page": 1,
                "page_count": 2,
                "limit": 100,
                "total_count": 150
                }
                }            
```

Wanneer

* **page** en **limiet** zijn de waarden die in het verzoek worden vermeld of de standaardwaarde als er geen waarden worden opgegeven.
* **page_count** is het totale aantal pagina&#39;s waarop een query kan worden uitgevoerd.
* **total_count** is het totale aantal abonnementen dat de vraag aanpast.

### Query uitvoeren op de abonnements-id

U kunt zoeken naar gebeurtenisabonnementen op basis van de id van het abonnement op de gebeurtenis. De aanvraagsyntaxis voor abonnementen op gebeurtenissen ziet er als volgt uit:

**Aanvraag-URL:**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Aanvraagkoppen:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Naam koptekst</p> </th> 
   <th> <p>Waarde koptekst</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID, waarde</p> </td> 
  </tr> 
 </tbody> 
</table>

**Responscodes:**

| Antwoordcode | Beschrijving |
|---|---|
| 200 | Het verzoek is geretourneerd met het gebeurtenisabonnement dat overeenkomt met de opgegeven abonnement-id. |
| 401 (Niet-geautoriseerd) | De opgegeven sessionID is leeg. |
| 403 (verboden) | De gebruiker, die verstrekte sessionID aanpast, heeft beheerdertoegang niet. |


**Voorbeeld van reactiebody:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
```

## Filteren op abonnementen voor gebeurtenissen

Filteren met gebeurtenisabonnementen kan worden gebruikt om ervoor te zorgen dat u alleen relevante berichten ontvangt. Het creëren van filters voor uw abonnementen kan het aantal berichten beduidend verminderen dat uw eindpunt moet verbruiken.

Een **BIJWERKEN - TAAK** gebeurtenisabonnement kan alleen worden geactiveerd wanneer de **newState** van een gebeurtenislading bepaalt **taskStatus** als **huidig**.

>[!IMPORTANT]
>
De volgende kenmerken zijn van toepassing op het filteren van gebeurtenisabonnementen

* Wanneer een filterveld een niet-lege waarde heeft, alleen berichten met een **newState** met de filtersleutels en -waarden worden naar de geabonneerde URL verzonden
* U kunt filteren op aangepaste gegevens die zijn opgenomen in het dialoogvenster **newState** EN/OF **oldState** van het object
* Filters worden alleen beoordeeld op het feit of ze al dan niet gelijk zijn aan een specifieke waarde
* Als de filtersyntaxis onjuist is of niet overeenkomt met de gegevens in het dialoogvenster **newState** van de lading, zal een bevestigingsbericht niet zijn teruggekeerd om erop te wijzen dat een fout is voorgekomen
* Filters kunnen niet worden bijgewerkt op een abonnement dat momenteel bestaat. Een nieuw abonnement moet worden gemaakt met nieuwe filterparameters.
* Er kunnen meerdere filters worden toegepast op één abonnement en het abonnement wordt alleen geleverd als aan alle filtervoorwaarden is voldaan.
* Het toepassen van meerdere filters op één abonnement staat gelijk aan het gebruik van een **EN** logische operator.
* Meerdere gebeurtenisabonnementen kunnen op één object worden toegepast zolang er een of meer parameters voor het abonnementsveld voor gebeurtenissen verschillen tussen de abonnementen voor elke gebeurtenis.
* Wanneer meerdere gebeurtenisabonnementen worden toegewezen aan één object, kunnen alle gebeurtenisabonnementen die aan dat object zijn gekoppeld, worden geretourneerd naar één eindpunt. Deze praktijk kan worden gebruikt als equivalent substituut voor logische operator **OF** die niet kunnen worden ingesteld met filterparameters.

### Vergelijkingsoperatoren gebruiken

U kunt samen met het filterveld een vergelijkingsveld opgeven. Gebruik een vergelijkingsoperator in dit veld om te filteren op vergelijkende resultaten. U kunt bijvoorbeeld een UPDATE - TASK-abonnement maken dat alleen een lading verzendt als de taakstatus NIET gelijk is aan de huidige status. U kunt de volgende vergelijkingsoperatoren gebruiken:

#### eq: gelijk

Met dit filter kunnen berichten worden doorlopen als de wijziging die is opgetreden overeenkomt met `fieldValue` in het filter. De `fieldValue` waarde is hoofdlettergevoelig.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "eq"
        }
    ]
}
```

#### ne: niet gelijk

Met dit filter kunnen berichten worden weergegeven als de wijziging die is opgetreden niet overeenkomt `fieldValue` in het filter. De `fieldValue` waarde is hoofdlettergevoelig.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "ne"
        }
    ]
}
```

#### gt: groter dan

Met dit filter kunnen berichten worden weergegeven als de update van de opgegeven `fieldName` is groter dan de waarde voor `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gt"
        }
    ]
}
```

#### gte: groter dan of gelijk aan

Met dit filter kunnen berichten worden weergegeven als de update van de opgegeven `fieldName` is groter dan of gelijk aan de waarde voor `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gte"
        }
    ]
}
```

#### lt: minder dan

Met dit filter kunnen berichten worden weergegeven als de update van de opgegeven `fieldName` is kleiner dan de waarde voor `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lt"
        }
    ]
}
```

#### lte: kleiner dan of gelijk aan

Met dit filter kunnen berichten worden weergegeven als de update van de opgegeven `fieldName` is kleiner dan of gelijk aan de waarde voor `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lte"
        }
    ]
}
```

#### contains

Met dit filter kunnen berichten doorkomen als de wijziging die zich heeft voorgedaan, de `fieldValue` in het filter. De `fieldValue` waarde is hoofdlettergevoelig

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        }
    ]
}
```

#### wijzigen

Met dit filter kunnen alleen berichten worden weergegeven als het opgegeven veld (`fieldName`) heeft een andere waarde in de oude en de nieuwe staat. Andere velden bijwerken naast het opgegeven veld (`fieldName`) retourneert deze wijziging niet.

>[!NOTE]
>
`fieldValue` in de array filters hieronder heeft geen effect.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "",
            "comparison": "changed"
        }
    ]
}
```

#### state

Met deze connector wordt het filter toegepast op de nieuwe status of oude status van het object dat is gemaakt of bijgewerkt. Dit is handig als u wilt weten waar een wijziging van de ene naar de andere wijziging heeft plaatsgevonden.
`oldState` is niet mogelijk op CREATE `eventTypes`.

>[!NOTE]
>
Het abonnement hieronder met het opgegeven filter retourneert alleen berichten waarin de naam van de taak `again` op de `oldState`, wat het was voordat er een update van de taak werd uitgevoerd.
Een gebruiksgeval voor dit zou zijn om de objCode- berichten te vinden die van één ding aan een ander veranderden. Bijvoorbeeld om alle taken te weten te komen die van &quot;Onderzoek één of andere naam&quot;in &quot;Onderzoek TeamName Één of andere naam&quot;veranderde

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains",
            "state": "oldState"
        }
    ]
}
```

### Verbindingsvelden gebruiken

De `filterConnector` in het veld voor de abonnementspayload kunt u kiezen hoe de filters moeten worden toegepast. De standaardwaarde is &quot;AND&quot;, waarbij alle filters moeten zijn ingesteld op `true` voor het abonnementsbericht om door te komen. Als &quot;OR&quot; is opgegeven, moet slechts één filter overeenkomen voor het abonnementsbericht dat wordt doorgestuurd.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        },
        {
            "fieldName": "name",
            "fieldValue": "also",
            "comparison": "contains"
        }
    ],
    "filterConnector": "AND"
}
```

## Gebeurtenisabonnementen verwijderen

Bij het verwijderen van Workfront HTTP gebruikt u de methode DELETE. De aanvraagsyntaxis voor het verwijderen van één gebeurtenisabonnement op basis van abonnement-id ziet er als volgt uit:

**Aanvraag-URL:**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Aanvraagkoppen:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Naam koptekst</p> </th> 
   <th> <p>Waarde koptekst</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> sessionID, waarde </p> </td> 
  </tr> 
 </tbody> 
</table>

**Responscodes:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Antwoordcode</p> </th> 
   <th> Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (geen inhoud)</td> 
   <td>De server heeft het gebeurtenisabonnement verwijderd dat overeenkomt met de opgegeven abonnement-id.</td> 
  </tr> 
  <tr> 
   <td>401 (Niet-geautoriseerd)</td> 
   <td>De opgegeven sessionID is leeg.</td> 
  </tr> 
  <tr> 
   <td>403 (verboden)</td> 
   <td>De gebruiker die de verstrekte sessionID aanpast heeft beheerdertoegang niet.</td> 
  </tr> 
  <tr> 
   <td>404</td> 
   <td>De server kan geen gebeurtenisabonnement vinden dat overeenkomt met de abonnement-id die is opgegeven voor verwijdering.</td> 
  </tr> 
 </tbody> 
</table>

**Voorbeeld van responsheaders:**

| Reactiekoptekst | Voorbeeld |
|---|---|
| Datum | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| Server | `→Apache-Coyote/1.1` |


**Voorbeeld van reactiebody:** NVT

## Voorbeelden van gebeurtenistaken

De lading die een gebruiker ontvangt varieert afhankelijk van het objecttype, maar er is een verenigbare formaat waarvoor die variërende ladingen worden geleverd.

De volgende eigenschappen blijven bijvoorbeeld consistent voor alle gebeurtenisladingen:

* eventType
* subscriptionId
* oldState
* newState
* eventTime

Hoewel de indeling consistent is, variëren de waarden in de eigenschappen tussen de verschillende objecten en objecttypen.

Hieronder ziet u voorbeelden van ladingen voor een UPDATE-gebeurtenis en een CREATE-gebeurtenis. In het voorbeeld UPDATE zijn de objecten oldState en newState hetzelfde, terwijl in het voorbeeld CREATE het object oldState leeg is (niet NULL).

Hieronder ziet u een voorbeeld van een payload voor een UPDATE-gebeurtenis:

<!-- [Copy](javascript:void(0);) -->

```
{
                  "eventType": "UPDATE",
                   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                   "eventTime": {
                       "nano": 998000000,
                       "epochSecond": 1507319336
                   },
                   "newState": {
                "ID": "59d7ddf7000002322d791eb08bafddfb", 
                       "name": "EventSub Test updated",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:56.980-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,       "categoryID": null,
                      "status": "CUR",
                      "parameterValues": {}
                   },
                   "oldState": {
                       "ID": "59d7ddf7000002322d791eb08bafddfb",
                       "name": "EventSub Test 180fd595-63fb-4fa9-bd47-58bf6e53d964",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:07.792-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,<
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,
                       "categoryID": null,
                       "status": "CUR",
                       "parameterValues": {}
                   }
                }
```

Hier volgt een voorbeeld van een payload voor een CREATE-gebeurtenis:

<!-- [Copy](javascript:void(0);) -->

```
{
                "eventType": "CREATE",
                "subscriptionId": "4028e3815ebf03a7015ebfa53b6d0002",
                "eventTime": {
                "nano": 232000000,
                "epochSecond": 1506453831
                },
                "newState": {
                "ID": "59caa946000000e07b0afc3383230c67",
                "name": "EventSub Test fe16d470-0a40-4290-92f4-6a0389fb536c",
                "objCode": "PROJ",
                "entryDate": "2017-09-26T13:23:50.746-0600",
                "accessorIDs": ["544820df0000142362741fc0c368de19"],
                "lastUpdateDate": "2017-09-26T13:23:50.927-0600",
                "groupID": "544820df0000140f6a9c1faa7cacadd3",
                "sponsorID": null,
                "description": null,
                "plannedCompletionDate": "2017-09-26T09:00:00.000-0600",
                "enteredByID": "544820df0000142362741fc0c368de19",
                "ownerID": "544820df0000142362741fc0c368de19",
                "templateID": null,
                "priority": 0,
                "companyID": null,
                "portfolioID": null,
                "referenceNumber": 1750,
                "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                "customerID": "544820df0000135b7719dcca654391f6",
                "currency": null,
                "categoryID": null,
                "status": "CUR",
                "parameterValues": {}
                },
                "oldState": {}
            }
```

## Basis 64-codering

Als een gebeurtenisabonnement wegens een conflict tussen speciale karakters in uw gebeurtenisabonnementen en uw netwerkmontages wordt verworpen, dan kunt u het coderen Base64 gebruiken om uw gebeurtenisabonnementen over te gaan. Base64 is een reeks coderingsregelingen die om het even welke willekeurige gegevens in een formaat van het koord van ASCII kunnen omzetten. Het is belangrijk om op te merken dat Base64 geen vorm van veiligheidsencryptie is.

### Base 64 Encoding Field

Het base64Encoding-veld is een optioneel veld dat wordt gebruikt om Base64-codering van gebeurtenisabonnementsladingen in te schakelen. De standaardwaarde is false en de mogelijke waarden zijn: true, false en &quot; &quot; (leeg).

### Voorbeeld van een aanvraag met het base64Encoding-veld

Als een verzoek wordt ingediend gebruikend base64Encoding gebied dat aan waar wordt geplaatst, dan **newState** en **oldState** objecten in de payload worden geleverd als basis 64-coderingstekenreeksen. Als het base64Encoding-veld is ingesteld op false, leeg wordt gelaten of niet is opgenomen in de aanvraag, wordt de geretourneerde payload niet gecodeerd in basis 64.

Hieronder ziet u een voorbeeld van een aanvraag die het veld base64Encoding gebruikt:

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua"",
                "authToken": "EauthTokenWorkfrontRocks1234_",
                "base64Encoding": "true"
            }
```

### Voorbeelden van antwoordladingen in basis 64-codering

<!-- [Copy](javascript:void(0);) -->

```
                {
                "eventType": "UPDATE",
                "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                "eventTime": {
                "nano": 998000000,
                "epochSecond": 1507319336
                },
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## Verouderde methode voor het opvragen van alle abonnementen op gebeurtenissen

Het volgende API eindpunt is afgekeurd en zou niet voor nieuwe implementaties moeten worden gebruikt. Wij adviseren ook overgangen oude implementaties aan de methode in **Abonnementen voor opvragen van gebeurtenissen** hierboven beschreven.

U kunt alle gebeurtenisabonnementen voor een klant zoals die door de sessionID waarde wordt gespecificeerd vragen. De aanvraagsyntaxis voor het aanbieden van alle gebeurtenisabonnementen voor een specifieke klant is de volgende URL:

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**Aanvraagkoppen:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Naam koptekst</p> </th> 
   <th> <p>Waarde koptekst</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> sessionID, waarde </p> </td> 
  </tr> 
 </tbody> 
</table>

**Responscodes:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Antwoordcode</p> </th> 
   <th> Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (geen inhoud)</td> 
   <td>De aanvraag heeft alle voor de gebruiker gevonden gebeurtenisabonnementen geretourneerd.</td> 
  </tr> 
  <tr> 
   <td>401 (Niet-geautoriseerd)</td> 
   <td>De opgegeven sessionID is leeg.</td> 
  </tr> 
  <tr> 
   <td>403 (verboden)</td> 
   <td>De gebruiker die de verstrekte sessionID aanpast heeft beheerdertoegang niet.</td> 
  </tr> 
 </tbody> 
</table>

 

### Voorbeeld van reactieorgaan

<!-- [Copy](javascript:void(0);) -->

```
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customer_id": "504f9640000013401be513579fbebffa",
                "obj_id": "ObjId1234",
                "obj_code": "TASK",
                "url": "http://test.test.net/test/1234",
                "event_type": "UPDATE",
                "auth_token": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customer_d": "504f9640000013401be513579fbebffa",
                "obj_id": null,
                "obj_code": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "event_type": "UPDATE",
                "auth_token": "authTokenWorkfrontRocks1234_"
                }                
                ]
```
