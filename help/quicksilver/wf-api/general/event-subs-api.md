---
content-type: api
navigation-topic: general-api
title: API voor abonnementen voor gebeurtenissen
description: API voor abonnementen voor gebeurtenissen
author: Becky
feature: Workfront API
role: Developer
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: 1c6a1238e9ea1ca843dcb296db7a552ff354c50a
workflow-type: tm+mt
source-wordcount: '2666'
ht-degree: 0%

---


# API voor abonnementen voor gebeurtenissen

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

Wanneer een actie op een voorwerp van Adobe Workfront voorkomt dat door gebeurtenisabonnementen wordt gesteund, kunt u Workfront vormen om een reactie naar uw gewenste eindpunt te verzenden. Dit betekent dat toepassingen van derden updates van Workfront-interacties kunnen ontvangen via de Workfront API kort nadat ze zich voordoen. Over het algemeen kunt u verwachten dat u binnen 5 seconden vanaf het moment dat de gegevenswijziging wordt geregistreerd, webhaakmeldingen ontvangt. Gemiddeld ontvangen klanten binnen minder dan 1 seconde berichten via een webhaak vanaf de gegevenswijziging die wordt geregistreerd.

Aangezien gebeurtenisabonnementen gegevens naar een andere service verzenden, worden ze beheerd via opdrachten in plaats van via de Workfront-toepassing.

Als u via uw firewall gebeurtenisabonnementen wilt ontvangen, moet u de volgende IP-adressen aan uw lijst van gewenste personen toevoegen:

**voor klanten in Europa:**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**voor klanten in plaatsen buiten Europa:**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

De volgende onderwerpen ondersteunen de API voor abonnementen op gebeurtenissen:

## Objecten ondersteund door gebeurtenisabonnementen

De volgende Workfront-objecten worden ondersteund door gebeurtenisabonnementen.

* Goedkeuring
* Goedkeuringsfase
* Deelnemer goedkeuringswerkgebied
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
* Workspace

>[!NOTE]
>
>Voor een lijst van gebieden die door de voorwerpen van het gebeurtenisabonnement worden gesteund, zie &lbrace;de gebieden van het het abonnementsmiddel van de Gebeurtenis [.](../../wf-api/api/event-sub-resource-fields.md)

## Verificatie van abonnement op gebeurtenis

Uw Workfront-gebruiker heeft het volgende nodig om een gebeurtenissenabonnement te maken, te vragen of te verwijderen:

* Een toegangsniveau van &quot;Beheerder van het Systeem&quot;wordt vereist om de Abonnementen van de Gebeurtenis te gebruiken.
* Een header `sessionID` is vereist om de API voor abonnementen op gebeurtenissen te gebruiken

  Voor meer informatie, zie [ Authentificatie ](api-basics.md#authentication) in [ API Grondbeginselen ](api-basics.md).

## De abonnementsbron opmaken

De abonnementsbron bevat de volgende velden.

* objId (optioneel)

   * **Koord** - identiteitskaart van het voorwerp van gespecificeerde objCode waarvoor de gebeurtenissen in brand worden gestoken. Als dit veld niet is opgegeven, ontvangt de gebruiker gebeurtenissen voor alle objecten van het opgegeven type.

* objCode (vereist)

   * **Koord** - objCode van het voorwerp dat aan veranderingen wordt ingetekend. De mogelijke waarden voor objCode worden in de onderstaande tabel weergegeven.

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
        <td scope="col">Goedkeuring</td> 
        <td scope="col"><p>goedkeuring</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Goedkeuringsfase</td> 
        <td scope="col"><p>approval_stage</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Deelnemer goedkeuringswerkgebied</td> 
        <td scope="col"><p>approval_stage_participant</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Toewijzing</td> 
        <td scope="col"><p>ASSGN</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Bedrijf </td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Dashboard</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Document</p></td> 
        <td scope="col">DOCU </td> 
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
        <td scope="col">Workspace</td> 
        <td scope="col">WORKSPACE</td> 
       </tr> 
      </tbody> 
     </table>

* eventType (vereist)

   * **Koord** - een waarde die het type van gebeurtenis vertegenwoordigt waarop het voorwerp wordt ingetekend. De beschikbare gebeurtenistypen zijn:

      * MAKEN
      * DELETE
      * BIJWERKEN

* url (vereist)

   * **Koord** - URL van het eindpunt waaraan de nuttige ladingen van de abonnementsgebeurtenis via HTTP worden verzonden.

* authToken (vereist)

   * **Koord** - het token OAuth2 dat wordt gebruikt om met URL voor authentiek te verklaren die op het &quot;URL&quot;gebied wordt gespecificeerd.

## API-aanvragen voor abonnementen voor gebeurtenissen maken

Nadat u ervoor hebt gezorgd dat de gebruiker beheerderstoegang heeft en de abonneebron vormt, bent u klaar om gebeurtenisabonnementen te maken.

Gebruik de volgende syntaxis om de URL samen te stellen.

**Verzoek URL**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**de kopballen van het Verzoek**

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

**Voorbeeld van het Lichaam van het Verzoek:**

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua",
                "authToken": "EauthTokenWorkfrontRocks1234_"
            }
```

**het lichaamshoofdvoorbeeld van de Reactie**

```
{
    "id": <NEW SUBSCRIPTION ID>,
    "version": <NEW SUBSCRIPTION VERSION>
}
```

| Antwoordcode | Beschrijving |
|---|---|
| 201 | Het gebeurtenisabonnement is gemaakt. |
| 400 (Ongeldige aanvraag) | Het URL-veld van de abonnementsbron werd als ongeldig beschouwd. |
| 401 (Niet-geautoriseerd) | De opgegeven sessionID is leeg of wordt als ongeldig beschouwd. |
| 403 (verboden) | De gebruiker die de verstrekte sessionID aanpast heeft beheerdertoegang niet. |

Als u een abonnementsbron doorgeeft als de hoofdtekst van een aanvraag (waarbij het inhoudstype &#39;application/json&#39; is), wordt een gebeurtenisabonnement gemaakt voor het opgegeven object. Een antwoordcode van 201 (Gemaakt) geeft aan dat het abonnement is gemaakt. Een antwoordcode buiten 201 betekent het abonnement **NIET** werd gecreeerd.

>[!NOTE]
>
> De responsheader &#39;Locatie&#39; bevat de URI van het zojuist gemaakte gebeurtenisabonnement.

**Voorbeeld van de Kopballen van de Reactie:**

| Antwoordheaders | Voorbeeld |
|---|---|
| Content-Length | `→0` |
| Datum | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| Locatie | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| Server | `→Apache-Coyote/1.1` |

## Abonnementen voor opvragen van gebeurtenissen

Gebruik de GET-methode wanneer u Workfront HTTP opvraagt. Er zijn twee manieren om te zoeken naar gebeurtenisabonnementen: query op abonnement-id (zie hieronder) of vraag naar alle gebeurtenisabonnementen.

### Query uitvoeren op alle abonnementen voor gebeurtenissen

U kunt alle gebeurtenissenabonnementen voor een klant vragen, of het volgende gebruiken om de reactie te beheren. U kunt ook de volgende opties gebruiken om de reactie te beheren:

* **pagina**: de optie van de vraagparameter om het aantal pagina&#39;s te specificeren om terug te keren. De standaardwaarde is 1.
* **grens**: de optie van de vraagparameter om het aantal resultaten te specificeren per pagina terug te keren. De standaardwaarde is 100 met een maximum van 1000.

De aanvraagsyntaxis voor het aanbieden van alle gebeurtenisabonnementen voor een specifieke klant is als volgt:

**Verzoek URL**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**Kopballen van het Verzoek:**

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

**Codes van de Reactie**

| Antwoordcode | Beschrijving |
|---|---|
| 200 | Het verzoek is geretourneerd met alle gebeurtenisabonnementen die zijn gevonden voor de klant die overeenkomt met de opgegeven sessionID. |
| 401 (Niet-geautoriseerd) | De opgegeven sessionID is leeg. |
| 403 (verboden) | De gebruiker, die verstrekte sessionID aanpast, heeft beheerdertoegang niet. |


**Voorbeeld van de Kopballen van de Reactie**

| Reactiekoptekst | Voorbeeld |
|---|---|
| Inhoudstype | `→application/json;charset=UTF-8` |
| Datum | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| Server | `→Apache-Coyote/1.1` |
| Overdrachtscodering | `→chunked` |


**Voorbeeld van het Lichaam van de Reactie**

```
{
    "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
    "date_created": "2024-04-11T17:10:10.305981",
    "date_modified": "2024-04-11T17:10:10.305981",
    "version": "v2",
    "dateVersionUpdated": "2025-01-15T04:04:04.407945"
    "customerId": "504f9640000013401be513579fbebffa",
    "objId": null,
    "objCode": "PROJ",
    "url": "http://requestb.in/ua5hi2ua",
    "eventType": "UPDATE",
    "authToken": "authTokenWorkfrontRocks1234_"
    "subscription_url": {
        "url": "http://requestb.in/ua5hi2ua",
        "date_created": "2024-04-11T15:56:14.169489",
        "successes": 11,
        "failures": 2,
        "disabled_at": null,
        "frozen_at": null
   }
}
```

Wanneer

* **pagina** en **grens** zijn de waarden die in het verzoek of het gebrek worden verstrekt als geen waarden worden verstrekt
* **page_count** is het totale aantal pagina&#39;s die kunnen worden gevraagd.
* **total_count** is het totale aantal abonnementen die de vraag aanpassen.

### Query uitvoeren op de abonnements-id

U kunt zoeken naar gebeurtenisabonnementen op basis van de id van het abonnement op de gebeurtenis. De aanvraagsyntaxis voor abonnementen op gebeurtenissen ziet er als volgt uit:

**Verzoek URL**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Kopballen van het Verzoek**

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

**Codes van de Reactie**

| Antwoordcode | Beschrijving |
|---|---|
| 200 | Het verzoek is geretourneerd met het gebeurtenisabonnement dat overeenkomt met de opgegeven abonnement-id. |
| 401 (Niet-geautoriseerd) | De opgegeven sessionID is leeg. |
| 403 (verboden) | De gebruiker, die verstrekte sessionID aanpast, heeft beheerdertoegang niet. |


**Voorbeeld van het Lichaam van de Reactie**



```
{
    "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
    "date_created": "2024-04-11T17:10:10.305981",
    "date_modified": "2024-04-11T17:10:10.305981",
    "version": "v2",
    "dateVersionUpdated": "2025-01-15T04:04:04.407945"
    "customerId": "504f9640000013401be513579fbebffa",
    "objId": null,
    "objCode": "PROJ",
    "url": "http://requestb.in/ua5hi2ua",
    "eventType": "UPDATE",
    "authToken": "authTokenWorkfrontRocks1234_"
    "subscription_url": {
        "url": "http://requestb.in/ua5hi2ua",
        "date_created": "2024-04-11T15:56:14.169489",
        "successes": 11,
        "failures": 2,
        "disabled_at": null,
        "frozen_at": null
   }
}
```


## Abonnementsversie voor gebeurtenissen

Workfront heeft twee versies van gebeurtenisabonnementen.

De capaciteit om gebeurtenisabonnementen te bevorderen of te degraderen zorgt ervoor dat wanneer de veranderingen in de structuur van gebeurtenissen worden aangebracht, de bestaande abonnementen niet breken, toestaand u om aan de nieuwe versie zonder een hiaat in uw gebeurtenisabonnement te testen en te bevorderen.

Voor meer informatie over gebeurtenisabonnement versioning, met inbegrip van specifieke verschillen tussen de versie en belangrijke data, zie [ het abonnement van de Gebeurtenis versioning ](/help/quicksilver/wf-api/general/event-subs-versioning.md).

>[!NOTE]
>
>Wanneer u uw gebeurtenissenabonnement upgradet of downloadt naar een andere versie, ontvangt u dubbele gebeurtenissen voor elke gebeurtenislevering gedurende een venster van vijf minuten na de versiewijziging. De duplicaten bevatten een van de versies 1 en 2 van het gebeurtenisabonnement. Dit zorgt ervoor dat u geen gebeurtenissen mist toe te schrijven aan het veranderen van de versie van het gebeurtenisabonnement.

### Versie van één abonnement wijzigen

De aanvraagsyntaxis voor het wijzigen van de versie voor één abonnement is:

**Verzoek URL**

```
PUT https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>/version 
```

**het verzoeklichaam van het Voorbeeld**

```
{
    "version": "v2" 
}
```


**het reactielichaam van het Voorbeeld (200)**

```
{
    "id": <SUBSCRIPTION ID>,
    "version": "v2" 
}
```

**Mogelijke antwoordcodes**

* 200
* 400
* 404


### Meerdere versies met abonnement wijzigen

Dit eindpunt verandert de versie van veelvoudige abonnementen, door lijst van abonnementen of de abonnementenvlag van alle klant.

De aanvraagsyntaxis voor het wijzigen van de versie voor één abonnement is:

**Verzoek URL**

```
PUT https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/version
```

**de organen van het de verzoekverzoek van het Voorbeeld**

* Instantie van het verzoek voor lijst van abonnementen

  ```
  {
      "subscriptionIds": [<SUBSCRIPTION ID 1>, <SUBSCRIPTION ID 2>],
      "version": "v2" 
  }
  ```

* Instantie aanvragen voor alle abonnementen van de klant

  ```
  {
      "allCustomerSubscriptions": true,
      "version": "v2" 
  }
  ```

**het reactielichaam van het Voorbeeld (200)**

```
{
    "subscription_ids": [<SUBSCRIPTION ID 1>, <SUBSCRIPTION ID 2>, ...],
    "version": "v2" 
}
```

**Mogelijke antwoordcodes**

* 200
* 400

## Filteren op abonnementen voor gebeurtenissen

Filteren met gebeurtenisabonnementen kan worden gebruikt om ervoor te zorgen dat u alleen relevante berichten ontvangt. Het creëren van filters voor uw abonnementen kan het aantal berichten beduidend verminderen dat uw eindpunt moet verbruiken.

Bijvoorbeeld, kan een **UPDATE - TASK** gebeurtenisabonnement worden geplaatst om slechts teweeg te brengen wanneer **newState** van een gebeurtenislading **taskStatus** als **huidig** bepaalt.

>[!IMPORTANT]
>
>De volgende kenmerken zijn van toepassing op het filteren van gebeurtenisabonnementen

* Wanneer een filtergebied een niet lege waarde slechts berichten met a **newState** heeft die de filtersleutels bevatten en de waarden worden verzonden naar geabonneerde URL
* U kunt door douanegegevens filtreren inbegrepen in **newState** EN/OF **oldState** van het voorwerp
* Filters worden alleen beoordeeld op het feit of ze al dan niet gelijk zijn aan een specifieke waarde
* Als uw filtersyntaxis onjuist is of geen gegevens aanpast in **newState** van de nuttige lading, zal een bevestigingsbericht niet zijn teruggekeerd om op te wijzen een fout is voorgekomen
* Filters kunnen niet worden bijgewerkt op een abonnement dat momenteel bestaat. Een nieuw abonnement moet worden gemaakt met nieuwe filterparameters.
* Er kunnen meerdere filters worden toegepast op één abonnement en het abonnement wordt alleen geleverd als aan alle filtervoorwaarden is voldaan.
* Het toepassen van veelvoudige filters op één enkel abonnement is een praktijk gelijkwaardig aan het gebruiken van een **EN** logische exploitant.
* Meerdere gebeurtenisabonnementen kunnen op één object worden toegepast zolang er een of meer parameters voor het abonnementsveld voor gebeurtenissen verschillen tussen de abonnementen voor elke gebeurtenis.
* Wanneer meerdere gebeurtenisabonnementen worden toegewezen aan één object, kunnen alle gebeurtenisabonnementen die aan dat object zijn gekoppeld, worden geretourneerd naar één eindpunt. Deze praktijk kan als gelijkwaardig substituut voor logische exploitant **worden gebruikt OF** die niet kan worden geplaatst gebruikend filterparameters.
* De volgende velden kunnen niet worden gefilterd:

   * DOCU.groups
   * RECORD.data
   * RECORD_TYPE.data
   * RECORD_TYPE.fields

### Vergelijkingsoperatoren gebruiken

U kunt samen met het filterveld een vergelijkingsveld opgeven. Gebruik een vergelijkingsoperator in dit veld om te filteren op vergelijkende resultaten. U kunt bijvoorbeeld een UPDATE - TASK-abonnement maken dat alleen een lading verzendt als de taakstatus NIET gelijk is aan de huidige status. U kunt de volgende vergelijkingsoperatoren gebruiken:

#### eq: gelijk

Met dit filter kunnen berichten worden doorlopen als de wijziging die zich heeft voorgedaan precies overeenkomt met `fieldValue` in het filter. De waarde `fieldValue` is hoofdlettergevoelig.

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

Met dit filter kunnen berichten worden doorlopen als de wijziging die zich heeft voorgedaan niet exact overeenkomt met `fieldValue` in het filter. De waarde `fieldValue` is hoofdlettergevoelig.

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

Met dit filter kunnen berichten worden weergegeven als de update voor de opgegeven `fieldName` groter is dan de waarde voor `fieldValue` .

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

Met dit filter kunnen berichten worden weergegeven als de update voor de opgegeven `fieldName` groter is dan of gelijk is aan de waarde voor `fieldValue` .

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

Met dit filter kunnen berichten worden weergegeven als de update van de opgegeven `fieldName` kleiner is dan de waarde voor `fieldValue` .

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

Met dit filter kunnen berichten worden weergegeven als de update voor de opgegeven `fieldName` kleiner is dan of gelijk is aan de waarde voor `fieldValue` .

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

Met dit filter kunnen berichten worden doorlopen als de wijziging die zich heeft voorgedaan de `fieldValue` in het filter bevat. De waarde `fieldValue` is hoofdlettergevoelig

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

#### containsOnly

Met dit filter kunnen alleen berichten worden weergegeven wanneer de volledige set geselecteerde waarden exact overeenkomt met de fieldValue in het filter, ongeacht de volgorde. Er mogen geen extra of ontbrekende waarden zijn.

>[!NOTE]
>
>Dit wordt gebruikt voor (multi-select) velden van het arraytype. In dit voorbeeldabonnement kunnen berichten alleen worden weergegeven wanneer het veld `groups` exact &quot;Keuze 3&quot; en &quot;Keuze 4&quot; bevat, zonder extra of ontbrekende waarden en ongeacht de volgorde. Als een tekenreeks of een geheel getal wordt opgegeven in `fieldValue` in plaats van een array, staat het abonnement toe dat berichten alleen worden doorgestuurd wanneer het veld `groups` exact één optie bevat en die optie exact overeenkomt met de tekenreeks of het gehele getal dat is opgegeven in `fieldValue` .&quot;


```
{
    "objCode": "PROJ",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedProjects",
    "filters": [
        {
            "fieldName": "groups",
            "fieldValue": [
                "Choice 3",
                "Choice 4"
            ],
            "state": "newState",
            "comparison": "containsOnly"
        }
    ]
}
```

#### notContains

Met dit filter kunnen alleen berichten worden weergegeven wanneer het opgegeven veld (`fieldName`) niet de opgegeven waarde (`fieldValue` ) bevat.

>[!NOTE]
>
>Dit wordt gebruikt voor array-type (multi-select) of tekenreeksvelden. Als het veld een tekenreeks is, controleren we of de opgegeven waarde niet in de tekenreeks staat (de tekenreeks &quot;Nieuw&quot; staat bijvoorbeeld niet in de tekenreeks &quot;Project - Bijgewerkt&quot;). Als het gebied een serie is en de gespecificeerde gebiedswaarde een koord of een geheel is, zullen wij controleren als de serie niet de gespecificeerde waarde bevat (bijvoorbeeld, &quot;Keus 1&quot;niet in [ &quot;Keus 2&quot;, &quot;Keus 3&quot;]). Met het onderstaande voorbeeldabonnement kunnen berichten alleen worden doorgestuurd wanneer de velden `groups` niet de tekenreeks &quot;Groep 2&quot; bevatten.

```
{
    "objCode": "PROJ",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedProjects",
    "filters": [
        {
            "fieldName": "groups",
            "fieldValue": "Group 2",
            "state": "newState",
            "comparison": "notContains"
        }
    ]
}
```

#### wijzigen

Dit filter staat berichten toe om door te komen slechts als het gespecificeerde gebied (`fieldName`) een verschillende waarde in oldstate en newstate heeft. Het bijwerken van andere gebieden naast gespecificeerd (`fieldName`) zal niet die verandering terugkeren.

>[!NOTE]
>
>`fieldValue` in de array filters eronder heeft geen effect.

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
`oldState` is niet mogelijk op CREATE `eventTypes` .

>[!NOTE]
>
>Het abonnement hieronder met het opgegeven filter retourneert alleen berichten waarin de naam van de taak `again` bevat op de `oldState` -taak, wat deze was voordat een update op de taak werd uitgevoerd.
>&#x200B;>Een gebruiksgeval voor dit zou zijn om de objCode- berichten te vinden die van één ding aan een ander veranderden. Bijvoorbeeld om alle taken te weten te komen die van &quot;Onderzoek één of andere naam&quot;in &quot;Onderzoek TeamName Één of andere naam&quot;veranderde

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

### Geneste filters gebruiken

Met Gebeurtenisabonnement kunt u filteren op geneste velden van gebeurtenissen met behulp van de geneste veldnamen. Als u bijvoorbeeld een bericht wilt filteren waarin `newState.data.customField1 = 'myCustomeFieldValue'` , kunt u het volgende abonnement met filter maken:

```
{
    "objCode": "RECORD",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedRecords",
    "filters": [
        {
            "fieldName": "data",
            "fieldValue": {
                    "customField1": "myCustomFieldValue"
            },
            "comparison": "eq",
            "state": "newState"
        }
    ]
}
```

Dubbel geneste filters kunnen ook worden benaderd.

```
"filters": [
    {
        "fieldName": "data",
        "fieldValue": {
            "fields": {
                "children": {
                    "customerId":"customer1234",
                    "name":"New Campaign"
                }
            }
        },
        "comparison": "eq",
        "state": "newState"
    }
],
"filterConnector": 'AND'
```

### Verbindingsvelden gebruiken

In het veld `filterConnector` op de payload van het abonnement kunt u kiezen hoe de filters moeten worden toegepast. De standaardwaarde is &quot;AND&quot;, waarbij de filters `true` moeten zijn voordat het abonnementsbericht wordt weergegeven. Als &quot;OR&quot; is opgegeven, moet slechts één filter overeenkomen voor het abonnementsbericht dat wordt doorgestuurd.

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

Gebruik de DELETE-methode wanneer u Workfront HTTP verwijdert. De aanvraagsyntaxis voor het verwijderen van één gebeurtenisabonnement op basis van abonnement-id ziet er als volgt uit:

**Verzoek URL:**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**Kopballen van het Verzoek:**

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

**Codes van de Reactie:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Antwoordcode</p> </th> 
   <th> Beschrijving</th> 
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

**Voorbeeld van de Kopballen van de Reactie:**

| Reactiekoptekst | Voorbeeld |
|---|---|
| Datum | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| Server | `→Apache-Coyote/1.1` |


**Voorbeeld van het Lichaam van de Reactie:** nvt

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
                   "eventVersion": "v2",
                   "subscriptionVersion": "v2",
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
                "eventVersion": "v2",
                "subscriptionVersion": "v2",
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

Als een verzoek wordt gemaakt gebruikend het base64Encoding gebied dat aan waar wordt geplaatst, dan worden de **newState** en **oldState** voorwerpen in de nuttige lading geleverd als basis 64 coderende koorden. Als het base64Encoding-veld is ingesteld op false, leeg wordt gelaten of niet is opgenomen in de aanvraag, wordt de geretourneerde payload niet gecodeerd in basis 64.

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
                "eventVersion": "v2",
                "subscriptionVersion": "v2",
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## Verouderde methode voor het opvragen van alle abonnementen op gebeurtenissen

Het volgende API eindpunt is afgekeurd en zou niet voor nieuwe implementaties moeten worden gebruikt. Wij adviseren ook overbrengend oude implementaties aan de methode in de **het Vragen van de Abonnementen van de Gebeurtenis** hierboven beschreven sectie.

U kunt alle gebeurtenisabonnementen voor een klant zoals die door de sessionID waarde wordt gespecificeerd vragen. De aanvraagsyntaxis voor het aanbieden van alle gebeurtenisabonnementen voor een specifieke klant is de volgende URL:

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**Kopballen van het Verzoek:**

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

**Codes van de Reactie:**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Antwoordcode</p> </th> 
   <th> Beschrijving</th> 
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
