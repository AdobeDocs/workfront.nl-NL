---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Objecten van de ene omgeving naar de andere verplaatsen
description: Het vermogen van de Bevordering van het Milieu is bedoeld om de capaciteit te verstrekken om op configuratie betrekking hebbende voorwerpen van één milieu aan een andere te bewegen. Het ondersteunt niet de mogelijkheid om transactieobjecten te verplaatsen (met beperkte uitzonderingen).
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
source-git-commit: 5d3c8e3626dabf88394bd6b3c2dd48e6168b56c4
workflow-type: tm+mt
source-wordcount: '2317'
ht-degree: 0%

---

# Objecten van de ene verplaatsen [!DNL Workfront] milieu aan een andere

<!-- 
TO DO

Overview of value
Check for any code changes
Fix {}
Add to tocs
-->

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] plan</td> 
   <td> <p>Enterprise, Prime of Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] licentie</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>U moet een [!DNL Workfront] beheerder. Voor informatie over [!DNL Workfront] beheerders, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Objectmachtigingen</p> </td> 
   <td> <p>Alles</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ondersteuningspakket</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred], of [!UICONTROL Enterprise]</p> <p>Het standaard ondersteuningspakket heeft geen toegang tot de aangepaste sandbox Vernieuwen, maar heeft wel toegang tot de voorvertoningssandbox.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Vereisten

Het Create eindpunt van het Pakket van de Bevordering veronderstelt dat u reeds het bronmilieu hebt gevormd. Voor deze API-aanroep moet handmatig een objectkaart worden gemaakt van [!DNL Workfront] objCodes en object GUIDs. De specifieke structuur van deze kaart wordt hieronder beschreven.

## Ondersteunde objecten voor milieubescherming

Het vermogen van de Bevordering van het Milieu is bedoeld om de capaciteit te verstrekken om op configuratie betrekking hebbende voorwerpen van één milieu aan een andere te bewegen. Het ondersteunt niet de mogelijkheid om transactieobjecten te verplaatsen (met beperkte uitzonderingen).

* [Werkobjecten](#work-objects)
* [Objecten rapporteren](#reporting-objects)
* [Aangepaste gegevensobjecten](#custom-data-objects)
* [Organisatie-objecten](#organization-objects)
* [Andere configuratieobjecten](#other-configuration-objects)


### Werkobjecten

| Promoteerbaar object | Opgenomen promoteerbare subobjecten |
| --- | --- |
| Project (PROJ) | Project<br>Taak<br>Toewijzing<br>Voorganger<br>Bedrijf<br>Overschrijvingssnelheid<br>Groep<br>Rol<br>Team<br>Goedkeuringsproces<br>Goedkeuringspad<br>Goedkeuringsstap<br>Stap fiatteur<br>Schema<br>Onwerkdag<br>Wachtrijdefinitie<br>Onderwerpgroep wachtrij<br>Onderwerp van wachtrij<br>Routeringsregel<br>Mijlpad<br>Mijlsteen<br>Uurtype<br>Bronpool<br>Categorie<br>Categorieparameter<br>Parameter<br>Parametergroep<br>Parameteroptie<br>Categorieweergavelogica |
| Sjabloon (TMPL) | Sjabloon<br>Sjabloontaak<br>Toewijzing sjabloontaak<br>Sjabloontaakvoorganger<br>Bedrijf<br>Overschrijvingssnelheid<br>Groep<br>Rol<br>Team<br>Goedkeuringsproces<br>Goedkeuringspad<br>Goedkeuringsstap<br>Stap fiatteur<br>Schema<br>Onwerkdag<br>Wachtrijdefinitie<br>Onderwerpgroep wachtrij<br>Onderwerp van wachtrij<br>Routeringsregel<br>Mijlpad<br>Mijlsteen<br>Uurtype<br>Bronpool<br>Categorie<br>Categorieparameter<br>Parameter<br>Parametergroep<br>Parameteroptie<br>Categorieweergavelogica |

### Objecten rapporteren

| Promoteerbaar object | Opgenomen promoteerbare subobjecten |
| --- | --- |
| Lay-outsjabloon (UITMPL) | Lay-outsjabloon<br>Dashboard<br>Kalender<br>Kalender, sectie<br>Externe pagina<br>Rapport<br>Filter<br>Groepering<br>Weergave<br>Parameter |
| Dashboard (PTLTAB) | Dashboard<br>Kalender<br>Kalender, sectie<br>Externe pagina<br>Rapport<br>Filter<br>Groepering<br>Weergave<br>Parameter |
| Kalender (CALEND) | Kalender<br>Kalender, sectie |
| Externe pagina (EXTSEC) | Externe pagina |
| Rapport (PTLSEC) | Rapport<br>Filter<br>Groepering<br>Weergave<br>Parameter |
| Filter (UIFT) | Filter<br>Parameter |
| Groeperen (UIGB) | Groepering<br>Parameter |
| Weergave (UIVW) | Weergave<br>Parameter |

### Aangepaste gegevensobjecten

| Promoteerbaar object | Opgenomen promoteerbare subobjecten |
| --- | --- |
| Categorie (CTGY) | Categorie<br>Categorieparameter<br>Parameter<br>Parametergroep<br>Parameteroptie<br>Categorieweergavelogica<br>Groep |
| Parameter (PARAM) | Parameter<br>Parameteroptie |
| Parametergroep (PGRP) | Parametergroep |

### Organisatie-objecten

| Promoteerbaar object | Opgenomen promoteerbare subobjecten |
| --- | --- |
| Groep (GROEP) | Groep <br>Subgroepen (maximaal 5 niveaus)<br>Categorie<br>Categorieparameter<br>Parameter<br>Parametergroep<br>Parameteroptie<br>Categorieweergavelogica |
| Rol (ROLE) | Rol |
| Team (TEAM) | Team<br>Groep |
| Bedrijf (CMPY) | Bedrijf<br>Overschrijvingssnelheid<br>Categorie<br>Categorieparameter<br>Parameter<br>Parametergroep<br>Parameter <br>Categorieweergavelogica<br>Groep |
| Portfolio (HAVEN) | Portfolio<br>Programma<br>Groep<br>Categorie<br>Categorieparameter<br>Parameter<br>Parametergroep<br>Parameteroptie<br>Categorieweergavelogica |
| Programma (PRGM) | Programma<br>Portfolio<br>Groep<br>Categorie<br>Categorieparameter<br>Parameter<br>Parametergroep<br>Parameteroptie<br>Categorieweergavelogica |

### Andere configuratieobjecten

| Promoteerbaar object | Opgenomen promoteerbare subobjecten |
| --- | --- |
| Goedkeuringsproces (ARVPRC) | Goedkeuringsproces<br>Goedkeuringspad<br>Goedkeuringsstap<br>Stap fiatteur<br>Rol<br>Team<br>Groep |
| Schema (SCHED) | Schema<br>Onwerkdag<br>Groep |
| Mijlpad (MPATH) | Mijlpad<br>Mijlsteen |
| Tijdbladprofiel (TSPRO) | Tijdbladprofiel<br>Uurtype |
| Uurtype (URT) | Uurtype |
| Type kosten (EXPTYP) | Type uitgave |
| Type risico (RSKTYP) | Type risico |
| Bronpool (RSPL) | Bronpool |

## Verificatie

De API verifieert elke aanvraag om ervoor te zorgen dat de client toegang heeft om een aangevraagd object te bekijken of te wijzigen.

Verificatie wordt uitgevoerd door een sessie-id of API-sleutel door te geven. Deze kan op een van de volgende manieren worden gegeven:

### Koptekstverificatie aanvragen

De aangewezen methode van authentificatie is een verzoekkopbal over te gaan genoemd SessionID die het zittingsteken bevat. Dit heeft het voordeel dat u veilig bent tegen [Cross-site Request-vervalsing (CSRF)](http://en.wikipedia.org/wiki/Cross-site_request_forgery) aanvallen en niet interfererend met URI voor caching doeleinden.

Hieronder ziet u een voorbeeld van een aanvraagkoptekst:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## API-eindpunten

* [Een pakket maken](#create-a-package)
* [Een lijst met pakketten ophalen](#get-a-list-of-packages)
* [Pakket ophalen op id](#get-a-package-by-id)
* [De configuratiedefinitie van een pakket ophalen](#get-a-packages-configuration-definition)
* [Details en definitie van pakket vervangen](#replace-package-details-and-definition)
* [Specifieke eigenschappen van een pakket bijwerken](#update-specific-properties-of-a-package)
* [Een pakket verwijderen](#delete-a-package)
* [Een prerun uitvoeren](#execute-a-pre-run)
* [Een installatie uitvoeren](#execute-an-installation)
* [Een lijst met installaties voor een specifiek pakket ophalen](#get-a-list-of-installations-for-a-specific-package)
* [Haal de installatiegegevens voor een installatie op](#get-the-installation-details-for-an-installation)

### Een pakket maken

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Deze vraag voert een multi-step proces uit.

De eerste stap resulteert in de creatie van een leeg promotiepakket in de status &quot;ASSEMBLING&quot;.

In de tweede stap worden de `objectCollections` -array in de POST-instantie om de gevraagde gegevens van Workfront samen te stellen. Deze stap kan enkele minuten duren, afhankelijk van het aantal opgevraagde records en uw Workfront-configuratie. Aan het einde van dit proces wordt het lege promotiepakket bijgewerkt met de `packageEntities` en de status wordt automatisch ingesteld op &quot;DRAFT&quot;.


>[!NOTE]
>
>Noteer de structuur van de `objectCollections`  array.
>
>Elk item in de array bevat een `objCode` sleutel die overeenkomt met de objectcode die wordt gedocumenteerd in de Workfront API Explorer.
>
>Elk item bevat ook een `entities` verzameling. Dit verwacht `ID` en `name` toetsen om aanwezig te zijn.
>
>Voor de lijst met toegestane objectcodes die moet worden aangevraagd in het dialoogvenster `objectCollections` lijst, zie [Ondersteunde objecten voor milieubescherming](#supported-objects-for-environment-promotion) in dit artikel.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### Kopteksten

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Lichaam

```json
{
    "packageName": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes...",
    "source": "https://{domain}.{environment}.workfront.com",
    "objectCollections": [
        {
            "objCode": "PROJ",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597ba1",
                    "name": "Agency Request"
                }
            ]
        },
        {
            "objCode": "TMPL",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597bb2",
                    "name": "New Agency Onboarding"
                },
                {
                    "ID": "6419b8b9001151ee258921a4f7597bc3",
                    "name": "New Agency Offboarding"
                }
            ]
        },
        {
            "objCode": "PTLTAB",
            "entities": [
                {
                    "ID": "645e6435000b4aaebe4776f4a42ed5ad",
                    "name": "Agency Performance and Readiness"
                }
            ]
        }
    ]
}
```

#### Antwoord

```json
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "ASSEMBLING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
}
```

### Een lijst met pakketten ophalen

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Deze vraag keert een ongefilterde lijst van bevorderingspakketten terug die tot de klant behoren.

De reactie omvat alle pakketten die zijn gemaakt op basis van een sandbox, voorvertoning of productie-instantie van Workfront van de klant.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### Kopteksten

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### Lichaam

_Leeg_

#### Antwoord

```
200
```

```json
{
    "data": [
        {
            "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
            "name": "Agency Onboarding - 2023-06-06",
            "description": "This promotion package contains configuration to support the agency onboarding processes...",
            "status": "ASSEMBLING",
            "version": 1,
            "installationCounts": {},
            "createdAt": "2023-06-06T17:29:21.600Z",
            "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
            "publishedAt": null,
            "customerId": "61aa9d090005fa42152c1cb66659f38d"
        },
        {...}
    ]
}
```

### Pakket ophalen op id

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Deze oproep retourneert de details van een aangevraagd promotiepakket.

Het verzoek kan worden gedaan door om het even welke milieu ongeacht de originele bron van het bevorderingspakket.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Kopteksten

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### Lichaam

_Leeg_

#### Antwoord

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "DRAFT",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "null"
                   - or -
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### De configuratiedefinitie van een pakket ophalen

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}/definition</code></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/definition
```

#### Kopteksten

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### Lichaam

_Leeg_

#### Antwoord

```
200
```

```json
{
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID": null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
}
```

### Details en definitie van pakket vervangen

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PUT /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Deze oproep vervangt alle inhoud van het promotiepakket.

De aanvraag verwacht dat alle bewerkbare velden worden opgegeven.

De bewerkbare kenmerken zijn:

1. name (string)
1. description (string)
1. bron (tekenreeks met URL-validatie)
1. status (tekenreeks met validatie van waarden)
1. version (geheel getal)
1. packageEntities (collectie)

De statusopties zijn:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>VERZAMELING</td> 
   <td><p>Deze status wordt automatisch toegewezen tijdens het samenstellen van objecten.</p><p>Deze status kan niet rechtstreeks door een klant worden ingesteld.</p></td> 
  </tr> 
  <tr> 
   <td>CONCEPT</td> 
   <td><p>Deze status wordt toegewezen aan het einde van een assemblageproces of bij het maken van een leeg promotiepakket.</p><p>Het is mogelijk dat een klant het promotiepakket terugbrengt naar deze status.</p><p>In deze status kan het promotiepakket niet in een omgeving worden geïnstalleerd.</p></td> 
  </tr> 
  <tr> 
   <td>TESTS</td> 
   <td><p>Met deze status kan een promotiepakket worden geïnstalleerd in elke voorvertoning of aangepaste vernieuwingssandbox. In deze status kan het pakket niet in Production worden geïnstalleerd.</p></td> 
  </tr> 
  <tr> 
   <td>ACTIEF</td> 
   <td><p>Met deze status kan een promotiepakket worden geïnstalleerd in elke omgeving, inclusief Productie.</p><p>Wanneer de pakketstatus is ingesteld op ACTIEF, wordt de instelling <code>publishedAt</code> De datum wordt automatisch ingesteld op de huidige tijdstempel van de aanvraag.</p></td> 
  </tr> 
  <tr> 
   <td>UITGESCHAKELD</td> 
   <td><p>Deze status wordt gebruikt om eerder gebruikte promotiepakketten te verbergen die in de toekomst niet in een omgeving worden geïnstalleerd.</p><p>Wanneer een pakket zich in deze status bevindt, kan het niet in een omgeving worden geïnstalleerd.</p><p>Wanneer een pakketstatus wordt ingesteld op DISABLED, wordt de <code>retiredAt</code> De datum wordt automatisch ingesteld op de huidige tijdstempel van de aanvraag.</p><p>Het gebruik van deze status wordt aanbevolen tijdens het gebruik van de<code>DELETE /package</code> eindpunt omdat het terugwinnbaar is en de installatiegeschiedenis voor om het even welke plaatsingen wordt behouden die met dit pakket worden gemaakt.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>Het promotiepakket wordt automatisch in deze status geplaatst als de ASSEMBLING-fase mislukt.</p><p>Als u het pakket wilt terugplaatsen naar het ASSEMBLING-stadium, moet u het extractieproces opnieuw starten.</p></td> 
  </tr> 
  </tbody> 
</table>

#### URL

```
PUT https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Kopteksten

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Lichaam

```json
{
    "packageName": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes... with a description change",
    "source": "https://{domain}.{environment}.workfront.com",
    "status": "TESTING",
    "version": 1,
    "metadata": {
        "displayOrder": ["GROUP","ROLE","TMPL","PROJ","PTLTAB"],
        "historyOrder": ["GROUP","ROLE","TMPL","TTSK","PROJ","PTLTAB"], 
        "installOrder": ["GROUP","ROLE","TMPL","TTSK","TPRED","TASSGN","PROJ","QUED","RRUL","QUET","UIFT","UIGB","UIVW","PTLTAB"], 
        "summaryOrder": ["GROUP","ROLE","TMPL"], 
        "shapeVersion": 2
    },
    "packageEntities": {
        "GROUP": [
           {
               "id": "52aa9d0e0005fcee8f212835bdaa2691",
               "name": "Default Group",
               "businessLeaderID": "...",
               "categoryID": "...",
               "defaultInterface": 1,
               "description": "...",
               "extRefID": null,
               "isActive": true,
               "isGroupPublic": true,
               "isPublic": true,
               "parentID": null,
               "rootID": null,
               "rootName": null,
               "uiTemplateID": null
           }
        ],
        "ROLE": [
           {...}
        ],
        ...
    }
}
```

#### Antwoord

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "TESTING",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Specifieke eigenschappen van een pakket bijwerken

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PATCH /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Deze oproep werkt de inhoud van het promotiepakket bij die in de PATCH-instantie wordt geleverd.

De bewerkbare kenmerken zijn:

1. name (string)
1. description (string)
1. bron (tekenreeks met URL-validatie)
1. status (tekenreeks met validatie van waarden)
1. version (geheel getal)
1. packageEntities (collectie)

   of

   objectCollections (array)

De `packageEntities` werkt het promotiepakket bij met de gegeven configuratiedefinitie.

De `objectCollections` een herwinning uit de `source` milieu in verband met het afzetbevorderingspakket. De `source` moet worden vermeld wanneer de `objectCollections` wordt opgegeven.

#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### Kopteksten

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Lichaam

```json
{
    "status": "ACTIVE"
}
```

#### Antwoord

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "status": "ACTIVE",
        "version": 1,
        "installationCounts": {},
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "displayEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Een pakket verwijderen

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>DELETE /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Met deze aanroep wordt de record voor het promotiepakket verwijderd. Deze actie is onomkeerbaar.

>[!NOTE]
>
>In tegenstelling tot het schrappen van een promotiepakket, is de aanbeveling om de status van het pakket te veranderen in DISABLED. Hierdoor kan het pakket worden opgehaald en blijft de installatiegeschiedenis van de locatie van het pakket behouden.

#### URL

```
DELETE https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### Kopteksten

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### Lichaam

_Leeg_

#### Antwoord

```
200
```

```
Deleted
```

### Een prerun uitvoeren

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST  {customer-domain}/environment-promotion/api/v1/packages/{id}/prepare-installation</code></td> 
  </tr> 
  </tbody> 
</table>

Met deze aanroep wordt een vergelijking gemaakt tussen de pakketdefinitie en de doelomgeving die in de URL is aangegeven.

Het resultaat is een JSON-instantie die aangeeft of een promotieobject al dan niet wordt gevonden in de doelomgeving.

Voor elk promotieobject een van de volgende `actions`  wordt ingesteld:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>MAKEN</td> 
   <td><p>Wanneer een corresponderende record niet kan worden gevonden in de doelomgeving, wordt de actie ingesteld op CREATE.</p><p>Wanneer deze handeling is ingesteld in het dialoogvenster <code>translationmap</code> die aan de <code>/install</code> eindpunt, zal de installatieservice het verslag tot stand brengen.</p></td> 
  </tr> 
  <tr> 
   <td>GEBRUIKELIJK</td> 
   <td><p>Wanneer een corresponderende record wordt gevonden in de doelomgeving, wordt de actie ingesteld op USEEXISTING en een <code>targetId</code> wordt ook vastgelegd in de <code>translationmap</code>.</p><p>Wanneer deze handeling is ingesteld in het dialoogvenster <code>translationmap</code> die aan de <code>/install</code> eindpunt, zal de installatieservice niet het verslag tot stand brengen. Het zal echter gebruikmaken van de <code>targetId</code> opgenomen in het kaartitem voor andere objecten die mogelijk een verwijzing naar deze record bevatten.</p><p>Een standaardgroep kan bijvoorbeeld worden gevonden in de doelomgeving waarin een pakket wordt geïmplementeerd. Het is niet mogelijk om twee "Standaard verslagen van de Groep"te hebben, zodat zal de installatieservice GUID voor de bestaande groep in een andere acties van de objecten tot stand brengen die een verwijzing naar de "StandaardGroep"omvatten, zoals een project, een vorm, of een andere entiteit die met deze groep verwant is.</p><p><b>Opmerking:</b> <ul><li><p>Wanneer de USEEXISTING-actie wordt toegewezen, wordt de bestaande record in de doelomgeving niet gewijzigd. </p><p>Als bijvoorbeeld de beschrijving van de standaardgroep is gewijzigd in de sandbox waarin het pakket is gemaakt en de beschrijvingswaarde in de doelomgeving afwijkt, blijft de waarde ongewijzigd na een installatie met deze <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>IGNORE</td> 
   <td><p>Deze handeling wordt niet automatisch ingesteld.</p><p>Het biedt de mogelijkheid om een handmatige overschrijving uit te voeren van een toegewezen CREATE- of USEEXISTING-handeling voordat de handeling wordt uitgevoerd <code>/install</code> vraag.</p><p><b>Opmerkingen: </b><ul><li><p>Als een verslag dat oorspronkelijk aan CREATE werd geplaatst aan IGNORE wordt geplaatst, dan zouden om het even welke kindverslagen ook aan IGNORE moeten worden geplaatst.</p><p>Bijvoorbeeld, als een verslag van het Malplaatje met CREATE actie in kaart werd gebracht, en de installerende gebruiker het van de plaatsing wenst uit te sluiten, kunnen zij de actie van het Malplaatje aan IGNORE plaatsen.</p><p>In dit geval, als de installerende gebruiker niet ook de Taken van het Malplaatje, de Toewijzingen van de Taak van het Malplaatje, Predecessors van de Taak van het Malplaatje, de Definitie van de Rij, de Onderwerpen van de Rij, het Verpletteren van Regels, enz. plaatst, zal de plaatsing in een ontbroken installatiepoging resulteren.</p></li><li><p>Als een record die oorspronkelijk op USEEXISTING was ingesteld, op IGNORE is ingesteld, kunnen er enkele negatieve effecten optreden tijdens het installatieproces.</p><p>Bijvoorbeeld, als een verslag van de Groep met de USEEXISTING actie in kaart is gebracht, en de installerende gebruiker de actie in IGNORE, voor voorwerpen verandert die een groep vereisen (b.v., kan een Project niet bestaan zonder een toegewezen groep), zal de systeem standaardgroep aan dat project worden toegewezen.</p></li><li><p>Als een record die oorspronkelijk op USEEXISTING was ingesteld, is ingesteld op CREATE, kunnen er enkele negatieve effecten optreden tijdens het installatieproces omdat veel Workfront-entiteiten unieke naambeperkingen hebben.</p><p>Als bijvoorbeeld een standaardrapport van de groep is toegewezen aan de USEEXISTING-actie en de installerende gebruiker de actie wijzigt in CREATE, omdat er al een "Standaardgroep" is, zal de installatiepoging niet alle stappen voltooien. Groepsnamen moeten uniek zijn.</p><p>Sommige entiteiten hebben geen unieke naambeperking. Als u deze wijziging aanbrengt voor deze objecten, worden twee records met dezelfde naam gemaakt. Sjablonen, projecten, weergaven, filters, groepen, rapporten en dashboards vereisen bijvoorbeeld geen unieke naambeperkingen. Het is aan te raden unieke namen voor deze records te hebben, maar dit wordt niet afgedwongen.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

Er is momenteel geen ondersteuning voor een UPDATE `action` in de alfamogelijkheden van deze service. De optie voor een UPDATE `action` is iets wat wij onderzoeken.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/translationmap
```

#### Kopteksten

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Lichaam

```json
{}
```

#### Antwoord

```
200
```

```json
{}
```

### Een installatie uitvoeren

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

Deze vraag stelt een installatiepoging van een bevorderingspakket in het doelmilieu in werking dat in de POST URL wordt geïdentificeerd.

#### Opties

Indien een `translationmap` niet in het lichaam van de POST wordt verstrekt, zal het proces automatisch `/translationmap` vraag. De `translationmap` het teruggegeven bedrag zal worden gebruikt zoals het is , zonder mogelijkheid om het te herzien of aan te passen .

Indien een `translationmap` wordt verstrekt in het lichaam van de POST, zal het installatieproces de verstrekte afbeelding gebruiken. Dit biedt een installerende gebruiker de gelegenheid om aanpassingen te herzien en aan te brengen zoals nodig alvorens een installatiepoging uit te voeren.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/install
```

#### Kopteksten

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Lichaam

```json
{
}
```

#### Antwoord

```
200
```


```json
{}
```

### Een lijst met installaties voor een specifiek pakket ophalen

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
</code></td> 
  </tr> 
  </tbody> 
</table>

De resultaten omvatten installatiegebeurtenissen van alle milieu&#39;s het pakket is opgesteld aan. Zij zijn niet beperkt tot de installaties voor het milieu waarmee het verzoek wordt gedaan. Zo kunt u bepalen welke omgevingen dit pakket hebben ontvangen.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
```

#### Kopteksten

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### Lichaam

_Leeg_

#### Antwoord

```
200
```

```json
[
    {
        "id": "2892b936-e09e-455a-935f-e1462ab9753c",
        "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
        "environmentPromotionPackageVersion": 1,
        "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
        "customerId": "54286d78b064451096752b99bf968481",
        "status": "COMPLETED",
        "environment": "https://{domain}.{environment}.workfront.com",
        "registeredAt": "2021-03-16T02:21:31.908Z",
        "updatedAt": null,
        "translationMap": {
            "ROLE": {
                "5f6d114f006883209828ddd9088e63b3": {
                    "name": "DAM Curator",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f4bed00028a718599f29575840053"
                },
                "ad535a9ebe647361e053a7656a0a1575": {
                    "name": "Copywriter",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f162700001ca051081c06667b14a4"
                },
                ...
            },
            "TMPL": {
                "5f9b317c00b3db5af69abcd1ed5f82aa": {
                    "name": "Digital Asset Production (Integrated)",
                    "action": "CREATE",
                    "isValid": true,
                    "targetId": "6054cda40000d5af63dc811d9c2b3a07"
                },
                ...
            },
            ...
        }
    },
    {...}
]
```

### Haal de installatiegegevens voor een installatie op

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /installations/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Deze vraag zal definitief terugkeren `translationMap` geproduceerd door de installatieservice voor een specifieke installatie.

In elke record wordt vermeld wat de voorgeschreven gegevens zijn `action` was en of die actie succesvol was of niet.

Voor records met een CREATE `action` de `targetId` het veld wordt ingesteld met de waarde van de nieuwe record in het doelsysteem. Daarnaast worden de `installationStatus` wordt ingesteld op INSTALLED.

Voor records met het USEEXIST `action` de `targetId` wordt ook het veld ingesteld en `installationStatus` wordt ingesteld op GEREGISTREERD. Dit betekent dat het kaartproces volledig was en de installatieservice erkent dat het het verslag heeft geëvalueerd en er niets om te handelen is.

Als de record een CREATE heeft `action` maar de record kan niet worden gemaakt. `installationStatus` wordt ingesteld op MISLUKT en de reden voor de fout wordt ook opgegeven.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}
```

#### Kopteksten

```json
{
    "apikey": "**********",
    - or -
    "sessionID": "*****************", 
}
```

#### Lichaam

_Leeg_

#### Antwoord

```
200
```

```json
{
    "id": "2892b936-e09e-455a-935f-e1462ab9753c",
    "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
    "environmentPromotionPackageVersion": 1,
    "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
    "customerId": "54286d78b064451096752b99bf968481",
    "status": "COMPLETED",
    "environment": "https://{domain}.{environment}.workfront.com",
    "registeredAt": "2021-03-16T02:21:31.908Z",
    "updatedAt": null,
    "translationMap": {
        "ROLE": {
            "5f6d114f006883209828ddd9088e63b3": {
                "name": "DAM Curator",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "600f4bed00028a718599f29575840053"
            },
            ...
        },
        "TMPL": {
            "5f9b317c00b3db5af69abcd1ed5f82aa": {
                "name": "Digital Asset Production (Integrated)",
                "action": "CREATE",
                "isValid": true,
                "targetId": "6054cda40000d5af63dc811d9c2b3a07"
            },
            ...
        },
        ...
    }
}
```



<!--table templates

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

<table style="table-layout:fixed"> 
 <col> 
 <tbody> 
  <tr> 
   <td><b></b></td> 
  </tr> 
  <tr> 
   <td><pre></pre></td> 
  </tr> 
  </tbody> 
</table>
-->