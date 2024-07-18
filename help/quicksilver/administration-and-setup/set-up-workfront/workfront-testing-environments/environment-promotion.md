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
recommendations: noDisplay, noCatalog
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
source-git-commit: 6f5da5ede6bb8c98b26d7d37366670c89ded6c49
workflow-type: tm+mt
source-wordcount: '2093'
ht-degree: 0%

---

# Objecten tussen [!DNL Workfront] -omgevingen verplaatsen met de [!DNL Workfront] Environment Promotion API

Met de mogelijkheid Omgevingsbevordering kunt u configuratiegerelateerde objecten van de ene omgeving naar de andere verplaatsen. U kunt deze objecten verplaatsen met de Workfront API, zoals beschreven in dit artikel.

Voor instructies over het verplaatsen van objecten tussen omgevingen met de Workfront-toepassing raadpleegt u:

* [Een pakket voor milieubescherming maken of bewerken](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
* [Een pakket voor milieubescherming installeren](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)


## Toegangsvereisten

U moet het volgende hebben:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan </strong>
   </td>
   <td> Premier of Ultimate (alleen nieuwe plannen)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenties </strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Configuraties op toegangsniveau
   </td>
   <td>U moet een [!DNL Workfront] beheerder zijn.
   </td>
  </tr>
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

Het Create eindpunt van het Pakket van de Bevordering veronderstelt dat u reeds het bronmilieu hebt gevormd. Voor deze API-aanroep moet handmatig een objectkaart van [!DNL Workfront] objCodes en object GUIDs worden gemaakt. De specifieke structuur van deze kaart wordt hieronder beschreven.

## Ondersteunde objecten voor milieubescherming

Het vermogen van de Bevordering van het Milieu is bedoeld om de capaciteit te verstrekken om op configuratie betrekking hebbende voorwerpen van één milieu aan een andere te bewegen. Het ondersteunt niet de mogelijkheid om transactieobjecten te verplaatsen (met beperkte uitzonderingen).

Voor een lijst van promotable voorwerpen en hun inbegrepen promotable subobjects, zie [ Gesteunde voorwerpen voor milieubevordering ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) in het artikel [ Overzicht van het bewegen van voorwerpen tussen de milieu&#39;s van Workfront ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).

## Verificatie

De API verifieert elke aanvraag om ervoor te zorgen dat de client toegang heeft om een aangevraagd object te bekijken of te wijzigen.

Verificatie wordt uitgevoerd door een sessie-id of API-sleutel door te geven. Deze kan met de volgende methode worden gegeven:

### Koptekstverificatie aanvragen

De aangewezen methode van authentificatie is een verzoekkopbal over te gaan genoemd SessionID die het zittingsteken bevat. Dit heeft het voordeel om tegen [ Cross-site van het Verzoek Smederij (CSRF) ](https://en.wikipedia.org/wiki/Cross-site_request_forgery) aanvallen veilig te zijn en zich niet met URI voor caching doeleinden te mengen.

Hieronder ziet u een voorbeeld van een aanvraagkoptekst:

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## API-eindpunten

* [Een pakket maken](#create-a-package)
* [Een lijst met pakketten ophalen](#get-a-list-of-packages)
* [Pakket ophalen op id](#get-a-package-by-id)
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

In de tweede stap wordt de array `objectCollections` in de hoofdtekst van de POST gebruikt om de gevraagde records van Workfront samen te stellen. Deze stap kan enkele minuten duren, afhankelijk van het aantal opgevraagde records en uw Workfront-configuratie. Aan het einde van dit proces wordt het lege promotiepakket bijgewerkt met `packageEntities` en wordt de status automatisch ingesteld op &quot;DRAFT&quot;.


>[!NOTE]
>
>Noteer de structuur van de array `objectCollections` .
>
>Elk item in de array bevat een `objCode` -sleutel die overeenkomt met de objectcode die in de Workfront API Explorer is gedocumenteerd.
>
>Elk item bevat ook een `entities` -verzameling. Hiermee wordt het veld `ID` verwacht. Het kan ook een optioneel `name` -kenmerk accepteren, zodat u gemakkelijker kunt zien wat de `ID` vertegenwoordigt.
>
>Voor de lijst van toegestane objecten codes die in de `objectCollections` lijst moeten worden gevraagd, zie de [ Gesteunde voorwerpen voor milieu bevordering ](#supported-objects-for-environment-promotion) sectie in dit artikel.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### Kopteksten

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

of

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Lichaam

```json
{
    "name": "Agency Onboarding - 2023-06-06",
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
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ASSEMBLING",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
    }
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
    "apikey": "**********"
}
```

of

```json
{
    "sessionID": "*****************"
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
            "createdAt": "2023-06-06T17:29:21.600Z",
            "deletedAt": null
},
        {...}
    ]
}
```

&lt;!—Schakel hierboven &quot;status&quot; in—is deze toegevoegd?—>

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
    "apikey": "**********"
}
```

of

```json
{
    "sessionID": "*****************"
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
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "DRAFT",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
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
1. status (tekenreeks met validatie van waarden)

Voor een gedetailleerde beschrijving van beschikbare statussen, zie [ de bevorderingsstatussen van het Milieu ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) in het artikel [ Overzicht van het bewegen van voorwerpen tussen de milieu&#39;s van Workfront ](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).


#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### Kopteksten

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

of

```json
{
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
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ACTIVE",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
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
    "apikey": "**********"
}
```

of

```json
{
    "sessionID": "*****************"
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

>[!IMPORTANT]
>
>Voordat u een installatie kunt uitvoeren, moet u deze uitvoering uitvoeren. U zult identiteitskaart gebruiken die van deze vraag wordt geproduceerd wanneer u de installatie uitvoert.

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

Voor elk promotieobject wordt een van de volgende opties ingesteld: `actions`

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>MAKEN</td> 
   <td><p>Wanneer een corresponderende record niet kan worden gevonden in de doelomgeving, wordt de actie ingesteld op CREATE.</p><p>Wanneer deze handeling wordt ingesteld in het <code>translationmap</code> -bestand dat aan het <code>/install</code> -eindpunt wordt geleverd, maakt de installatieservice de record.</p></td> 
  </tr> 
  <tr> 
   <td>GEBRUIKELIJK</td> 
   <td><p>Wanneer een corresponderende record wordt gevonden in de doelomgeving, wordt de actie ingesteld op USEEXISTING en wordt een <code>targetId</code> ook vastgelegd in <code>translationmap</code> .</p><p>Wanneer deze handeling wordt ingesteld in het <code>translationmap</code> -bestand dat aan het <code>/install</code> -eindpunt wordt geleverd, maakt de installatieservice de record niet. De code gebruikt echter de <code>targetId</code> die is opgenomen in de kaartvermelding voor andere objecten die een verwijzing naar deze record kunnen bevatten.</p><p>Een standaardgroep kan bijvoorbeeld worden gevonden in de doelomgeving waarin een pakket wordt geïmplementeerd. Het is niet mogelijk om twee "Standaard verslagen van de Groep"te hebben, zodat zal de installatieservice GUID voor de bestaande groep in een andere acties van de objecten tot stand brengen die een verwijzing naar de "StandaardGroep"omvatten, zoals een project, een vorm, of een andere entiteit die met deze groep verwant is.</p><p><b> Nota:</b> <ul><li><p>Wanneer de USEEXISTING-actie wordt toegewezen, wordt de bestaande record in de doelomgeving niet gewijzigd. </p><p>Als de beschrijving van de standaardgroep bijvoorbeeld is gewijzigd in de sandbox waarin het pakket is gemaakt en de beschrijvingswaarde in de doelomgeving afwijkt, blijft de waarde na een installatie met deze <code>translationmap</code> ongewijzigd.</li></ul></td> 
  </tr> 
  <tr> 
   <td>OVERSCHRIJVEN</td> 
   <td><p>Deze handeling wordt niet automatisch ingesteld.</p><p>Met deze actie kunt u een object bijwerken dat in de doelomgeving bestaat. Het biedt de mogelijkheid om een handmatige overschrijving uit te voeren van een toegewezen CREATE- of USEEXISTING-actie voordat de <code>/install</code> -aanroep wordt uitgevoerd.<ul><li>Een gebruiker kan een object bijwerken in de testomgeving en vervolgens de actie OVERSCHRIJVEN gebruiken om dat object bij te werken in de doelomgeving.</p></li><li><p>Als de gebruiker eerst één promotiepakket installeert en vervolgens een nieuw (of bijgewerkt) pakket in de toekomst wijzigingen bevat in objecten in het eerste pakket, kan de gebruiker met OVERSCHRIJVEN eerder geïnstalleerde objecten vervangen (overschrijven). </p><p>Zie de sectie [Overschrijven](#overschrijven) in dit artikel voor meer informatie over overschrijven.</li><ul></td> 
  </tr> 
  <tr> 
   <td>IGNORE</td> 
   <td><p>Deze handeling wordt niet automatisch ingesteld.</p><p>Het biedt de mogelijkheid om een handmatige overschrijving uit te voeren van een toegewezen CREATE- of USEEXISTING-actie voordat de <code>/install</code> -aanroep wordt uitgevoerd.</p><p><b>Opmerkingen: </b><ul><li><p>Als een verslag dat oorspronkelijk aan CREATE werd geplaatst aan IGNORE wordt geplaatst, dan zouden om het even welke kindverslagen ook aan IGNORE moeten worden geplaatst.</p><p>Bijvoorbeeld, als een verslag van het Malplaatje met CREATE actie in kaart werd gebracht, en de installerende gebruiker het van de plaatsing wenst uit te sluiten, kunnen zij de actie van het Malplaatje aan IGNORE plaatsen.</p><p>In dit geval, als de installerende gebruiker niet ook de Taken van het Malplaatje, de Toewijzingen van de Taak van het Malplaatje, Predecessors van de Taak van het Malplaatje, de Definitie van de Rij, de Onderwerpen van de Rij, het Verpletteren van Regels, enz. plaatst, zal de plaatsing in een ontbroken installatiepoging resulteren.</p></li><li><p>Als een record die oorspronkelijk op USEEXISTING was ingesteld, op IGNORE is ingesteld, kunnen er enkele negatieve effecten optreden tijdens het installatieproces.</p><p>Bijvoorbeeld, als een verslag van de Groep met de USEEXISTING actie in kaart is gebracht, en de installerende gebruiker de actie in IGNORE, voor voorwerpen verandert die een groep vereisen (b.v., kan een Project niet bestaan zonder een toegewezen groep), zal de systeem standaardgroep aan dat project worden toegewezen.</p></li><li><p>Als een record die oorspronkelijk op USEEXISTING was ingesteld, is ingesteld op CREATE, kunnen er enkele negatieve effecten optreden tijdens het installatieproces omdat veel Workfront-entiteiten unieke naambeperkingen hebben.</p><p>Als bijvoorbeeld een standaardrapport van de groep is toegewezen aan de USEEXISTING-actie en de installerende gebruiker de actie wijzigt in CREATE, omdat er al een "Standaardgroep" is, zal de installatiepoging niet alle stappen voltooien. Groepsnamen moeten uniek zijn.</p><p>Sommige entiteiten hebben geen unieke naambeperking. Als u deze wijziging aanbrengt voor deze objecten, worden twee records met dezelfde naam gemaakt. Sjablonen, projecten, weergaven, filters, groepen, rapporten en dashboards vereisen bijvoorbeeld geen unieke naambeperkingen. Het is aan te raden unieke namen voor deze records te hebben, maar dit wordt niet afgedwongen.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

Er is momenteel geen ondersteuning voor een UPDATE `action` in de alfamogelijkheden van deze service. De optie om een UPDATE `action` toe te staan, is iets waar we naar zoeken.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/:id/prepare-installation
```

#### Kopteksten

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

of

```json
{
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
{
    "environmentPromotionPackageId": "45f2ae94-76c0-4b13-8f3b-f688de83043d",
    "environmentPromotionPackageVersion": 1,
    "id": "c0bc79bd-c9c1-4b5b-b118-b1241392de0e",
    "userId": "5ba38da500b752fd66439d4f6a9999a1",
    "customerId": "5ba38d9d00b74f0c7a38b1b487fc9710",
    "status": "PREPARING",
    "environment": "mmi.my.workfront.com",
    "registeredAt": "2023-10-19T20:00:16.697Z",
    "updatedAt": "2023-10-19T20:00:16.701Z",
    "translationMap": {
        "CTGY": {
            "62d9c9a0000013aeeefe7242a0a5fdb2": {
                "name": "Example Document Form",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9a0000013aeeefe7242a0a5fdb2"
            }
        },
        "PGRP": {
            "62d1eee4001c6618e6b9f9a588ba1598": {
                "name": "Asset Detail",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee4001c6618e6b9f9a588ba1598"
            }
        },
        "GROUP": {
            "5ba38da500b752b0f46d13186030b7ad": {
                "name": "Default Group",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "5ba38da500b752b0f46d13186030b7ad"
            }
        },
        "PARAM": {
            "62d1eee400f8578895166ee91a83f97a": {
                "name": "Asset Type",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee400f8578895166ee91a83f97a"
            },
            "62d1eee50001407c713514a8970b58e4": {
                "name": "Keywords",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee50001407c713514a8970b58e4"
            },
            "62d1eee5000333ac3981ea4f3df6d88e": {
                "name": "Permitted Uses",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000333ac3981ea4f3df6d88e"
            },
            "62d1eee5000b188e9ec8039a097fc7ab": {
                "name": "File Format",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000b188e9ec8039a097fc7ab"
            },
            "62d1eee500100c159fd5f838ce560507": {
                "name": "CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee500100c159fd5f838ce560507"
            },
            "62d9c988001c1f23954dbb9d646335b5": {
                "name": "Other CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c988001c1f23954dbb9d646335b5"
            },
            "62d9c9880070f546cf4c798ea6c3eaa4": {
                "name": "Other Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9880070f546cf4c798ea6c3eaa4"
            },
            "62d9c990006258baf1b40f2569c3eab7": {
                "name": "Target Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c990006258baf1b40f2569c3eab7"
            }
        }
    }
}
```

>[!NOTE]
>
>De id die u nodig hebt om de installatie uit te voeren, is het veld `id` . In dit voorbeeld bevindt het veld `id` zich op het derde punt van de bovenkant en heeft een waarde die begint met `c0bc79bd` .

### Een installatie uitvoeren

>[!IMPORTANT]
>
>Voordat u een installatie kunt uitvoeren, moet u een voorvertoning uitvoeren. Wanneer u de installatie uitvoert, gebruikt u de id die bij de uitvoering is gegenereerd.
>
>Als om het even welke veranderingen in het bestemmingsmilieu (het milieu zijn aangebracht dat het pakket wordt opgesteld) na het uitvoeren van pre-looppas, adviseren wij nogmaals uitvoering pre-run. Als u de voorvertoning niet opnieuw uitvoert, is de uitvoering mogelijk niet correct voltooid of mislukt de installatie mogelijk.
>
>Voor instructies bij het uitvoeren van een pre-looppas, zie [ prerun ](#execute-a-pre-run) uitvoeren.

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

Deze vraag stelt een installatiepoging van een bevorderingspakket in het doelmilieu in werking dat in de POST URL wordt geïdentificeerd.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}/install
```

#### Kopteksten

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

of

```json
{
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
202
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
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
```

#### Kopteksten

```json
{
    "apikey": "**********"
}
```

of

```json
{
    "sessionID": "*****************"
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
        "status": "INSTALLED",
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

Deze aanroep retourneert de laatste `translationMap` die door de installatieservice voor een specifieke installatie is gemaakt.

In elke record wordt aangegeven wat de voorgeschreven `action` was en of die actie succesvol was of niet.

Voor records met een CREATE `action` wordt het veld `targetId` ingesteld met de waarde van de nieuwe record in het doelsysteem. Daarnaast wordt het veld `installationStatus` ingesteld op INSTALLED.

Voor records met USEEXISTING `action` wordt het veld `targetId` ook ingesteld en wordt het veld `installationStatus` ingesteld op REGISTERED. Dit betekent dat het kaartproces volledig was en de installatieservice erkent dat het het verslag heeft geëvalueerd en er niets om te handelen is.

Als de record een CREATE `action` heeft maar er geen record kan worden gemaakt, wordt de `installationStatus` ingesteld op FAILED en wordt ook de reden voor de fout opgegeven.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}
```

#### Kopteksten

```json
{
    "apikey": "**********"
}
```

of

```json
{
    "sessionID": "*****************"
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
    "status": "INSTALLED",
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

## Overschrijven

Dit is een proces in drie stappen.

1. Een vertaalkaart maken (dit is te vergelijken met de installatiefase &quot;De installatie voorbereiden&quot;)
1. Bewerk de gegenereerde vertaalkaart en stel de velden `action` en `targetId` in voor elk object dat ze willen overschrijven. De handeling moet `OVERWRITING` zijn en de `targetId` moet de uuid zijn van het object dat moet worden overschreven
1. Voer de installatie uit.

* [Stap 1 - Een vertaalkaart maken](#step-1---create-a-translation-map)
* [Stap 2 - Wijzig de Omzettingskaart](#step-2---modify-the-translation-map)
* [Stap 3 - Installeren](#step-3---install)

### **Stap 1 - creeer een Omzetkaart**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/translation-map
```

#### Lichaam

Geen

#### Antwoord

Een vertaalkaart, met een `202 - OK` -status

```json
{
    {objcode}: {
        {object uuid}: {
            "targetId": {uuid of object in destination},
            "action": {installation action},
            "name": {name of the object},
            "isValid": true
        },
        {...more objects}
    },
    {...more objcodes}
}
```


#### Voorbeeld

```json
{
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "CREATE",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
```

### Stap 2 - Wijzig de Omzettingskaart

Er is geen eindpunt voor deze stap.

1. In de vertaalkaart die in [ Stap 1 is teruggekeerd - creeer een Vertaal Kaart ](#step-1---create-a-translation-map), inspecteer de lijst van voorwerpen die zullen worden geïnstalleerd.
1. Werk het actieveld op elk voorwerp aan de gewenste installatieactie bij.
1. Valideer de `targetId` voor elk object. Als de actie set `USEEXISTING` of `OVERWRITING` is, moet de `targetId` worden ingesteld op de UUID van het doelobject in de doelomgeving. Voor elke andere actie moet targetId een lege tekenreeks zijn.

   >[!NOTE]
   >
   >`targetId` is reeds bevolkt als een botsing werd ontdekt.

### **Stap 3 - installeer**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/install
```

#### Lichaam

Dit is een voorwerp met één enkel gebied `translationMap`, dat de gewijzigde vertaalkaart van [ Stap 2 zou moeten evenaren - wijzig de Omzettingskaart ](#step-2---modify-the-translation-map).

```json
{
    "translationMap": {
        {objcode}: {
            {object uuid}: {
                "targetId": {uuid of object in destination},
                "action": {installation action},
                "name": {name of the object},
                "isValid": true
            },
            {...more objects}
        },
        {...more objcodes}
    }
}
```


#### Voorbeeld

```json
{
    "translationMap": {
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "OVERWRITING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
}
```

#### Antwoord

Het antwoord bevat de status `{uuid of the created installation}` en `202 - ACCEPTED` .

Voorbeeld: `b6aa0af8-3520-4b25-aca3-86793dff44a6`

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
