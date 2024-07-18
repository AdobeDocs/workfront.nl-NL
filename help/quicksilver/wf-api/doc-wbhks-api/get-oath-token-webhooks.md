---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: OAuth2-tokens ophalen
description: OAuth2-tokens ophalen
author: Becky
feature: Workfront API
role: Developer
exl-id: f3a2630d-d34e-4d36-b2bb-707ba0d3258e
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---


# OAuth2-tokens ophalen

## OAuth2-tokens ophalen

Keert OAuth2 terug verfrist teken en toegangstoken voor een voor authentiek verklaarde gebruiker. Dit wordt eenmaal aangeroepen wanneer de gebruiker een Document Provider levert. De verdere vraag wordt gemaakt om een bijgewerkt toegangstoken te krijgen.

**URL**

POST/alle URL&#39;s

URL is configureerbaar en beantwoordt aan de Symbolische waarde van URL van het Eindpunt op de pagina van de Opstelling van de douanevertegratie.

### Zoekparameters

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>Naam</th>
   <th>Vereist</th>
   <th>Beschrijving</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>subsidie_type</td>
   <td>ja</td>
   <td><p>Waarden zijn onder andere "authentication_code" of "refresh_token". De opgegeven waarde geeft aan welke van de twee parameters wordt doorgegeven aan deze API-aanroep: code of refresh_token.</p></td>
  </tr>
  <tr>
   <td>code</td>
   <td>afhankelijk</td>
   <td><p>De machtigingscode die naar Adobe Workfront wordt verzonden vlak nadat de gebruiker op de knop "Grant" klikt. Dit is alleen vereist wanneer het subsidietype "authentication_code" is. De toelatingscode moet van korte duur zijn, gewoonlijk aflopend binnen 10 minuten of minder.</p></td>
  </tr>
  <tr>
   <td>refresh_token</td>
   <td>afhankelijk</td>
   <td><p>Dit wordt slechts vereist wanneer het maken van verdere vraag om een nieuw access_token terug te winnen, gegeven dat vorige access_token als verlopen. Wanneer het verzenden van deze waarde plaats de subsidie_type parameter aan "verfrist_token".</p></td>
  </tr>
  <tr>
   <td>client_id</td>
   <td>ja</td>
   <td>De client-id die in Workfront is geconfigureerd voor deze aangepaste integratie.</td>
  </tr>
  <tr>
   <td>client_geheime</td>
   <td>ja</td>
   <td> Het clientgeheim dat in Workfront is geconfigureerd voor deze aangepaste integratie.</td>
  </tr>
 </tbody>
</table>

 

## Antwoord

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>Naam</th>
   <th>Type </th>
   <th>Beschrijving</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>access_token </td>
   <td>String</td>
   <td><p>Een token dat wordt gebruikt om geautoriseerde API-aanroepen uit te voeren in naam van de gebruiker. Dit zou moeten verlopen om onbevoegde API vraag te verhinderen.</p></td>
  </tr>
  <tr>
   <td>refresh_token </td>
   <td>String</td>
   <td><p>Een token van lange duur dat wordt gebruikt om een nieuw access_token op te halen door deze API-methode aan te roepen.</p></td>
  </tr>
  <tr>
   <td>verloopt_in </td>
   <td>lang</td>
   <td><p>(facultatief) de tijd (in seconden) alvorens access_token verloopt, over het algemeen 3.600.</p></td>
  </tr>
 </tbody>
</table>

**Voorbeeld**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```

## Antwoord

```
{
access_token:"ad8af5ad5ads759",
refresh_token:"9a0h5d87d808ads",
expires_id:3600
}
```
