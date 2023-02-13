---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Document Webhooks-API
description: Document Webhooks-API
author: John
feature: Workfront API
exl-id: 7ac2c6c8-1cb8-49df-8d63-a6b47ad02a13
source-git-commit: a2f340122b22ccc57af1afffd82093e458219648
workflow-type: tm+mt
source-wordcount: '3661'
ht-degree: 0%

---


# Document Webhooks-API

Adobe Workfront Document Webhooks definieert een set API-eindpunten waarmee Workfront geoorloofde API-aanroepen uitvoert naar een externe documentprovider. Hierdoor kan iedereen een middleware-insteekmodule maken voor elke leverancier van documentopslag.

De gebruikerservaring voor integratie op basis van een webhaak is vergelijkbaar met die van bestaande documentintegratie, zoals Google Drive, Box en Dropbox. Een Workfront-gebruiker kan bijvoorbeeld de volgende handelingen uitvoeren:

* Navigeren door de mapstructuur van de externe documentprovider
* Bestanden zoeken
* Bestanden koppelen naar Workfront
* Bestanden uploaden naar de externe documentprovider
* Een miniatuur voor het document weergeven

## Referentie-implementatie

Workfront biedt een voorbeeldimplementatie om de ontwikkeling van een nieuwe webhooks-implementatie te versnellen. Code hiervoor is te vinden op [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Deze implementatie is gebaseerd op Java en maakt het Workfront mogelijk om verbinding te maken met documenten op een netwerkbestandssysteem.

## Registreren van een Integratie Webhaak

Workfront-beheerders kunnen een aangepaste webshintegratie voor hun bedrijf toevoegen door te navigeren naar Setup > Documenten > Aangepaste integratie in Workfront. Van de pagina van de Integratie van de Douane binnen Opstelling, kunnen de beheerders een lijst van bestaande integratie van documentWebHaak bekijken. Vanaf deze pagina kunnen integraties worden toegevoegd, bewerkt, ingeschakeld en uitgeschakeld. Als u een integratie wilt toevoegen, klikt u op de knop Integratie toevoegen.

### Beschikbare velden

Wanneer de beheerder een integratie toevoegt, zal hij waarden voor de volgende gebieden ingaan:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Veldnaam</th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Naam</td> 
   <td>De naam van deze integratie.</td> 
  </tr> 
  <tr> 
   <td>Basis-API-URL</td> 
   <td> <p>De locatie van de callback-API. Wanneer het maken van vraag aan het externe systeem, zal Workfront eenvoudig de eindpuntnaam aan dit adres toevoegen. Als de beheerder bijvoorbeeld de URL van de basis-API, " https://www.mycompany.com/api/v1 " invoert, gebruikt Workfront de volgende URL om de metagegevens van een document op te halen: https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
  </tr> 
  <tr> 
   <td>Parameters aanvragen</td> 
   <td> <p>Optionele waarden die aan de querytekenreeks van elke API-aanroep moeten worden toegevoegd. Bijvoorbeeld access_type=offline.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Type verificatie</td> 
   <td>OAuth2 of ApiKey</td> 
  </tr> 
  <tr> 
   <td>Verificatie-URL</td> 
   <td> <p>(Alleen OAuth2) De volledige URL die wordt gebruikt voor gebruikersverificatie. Workfront navigeert gebruikers naar dit adres als onderdeel van het OAuth-inrichtingsproces. Opmerking: Workfront voegt een parameter "state" toe aan de queryreeks. De provider moet dit bestand teruggeven aan Workfront door het toe te voegen aan de Workfront Redirect URI.</p> </td> 
  </tr> 
  <tr> 
   <td>URL van token-eindpunt</td> 
   <td> <p>(Alleen OAuth2) De volledige API-URL waarmee OAuth2-tokens worden opgehaald. Dit wordt gehost door de websiteprovider of externe documentprovider</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Client-id</td> 
   <td>(Alleen OAuth2) De OAuth2 Client ID voor deze integratie</td> 
  </tr> 
  <tr> 
   <td>Clientgeheim</td> 
   <td> <p>(Alleen OAuth2) Het OAuth2-clientgeheim voor deze integratie</p> </td> 
  </tr> 
  <tr> 
   <td>Workfront Redirect URI</td> 
   <td>  <p>(Alleen OAuth2) Dit is een alleen-lezen veld en wordt gegenereerd door Workfront. Deze waarde wordt gebruikt om deze integratie bij de externe documentprovider te registreren. Opmerking: Zoals hierboven voor Authentificatie URL wordt beschreven, moet de leverancier de "staat"parameter en zijn waarde aan het querystring toevoegen wanneer het uitvoeren van redirect.</p></td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td>  <p>(Alleen ApiKey) Wordt gebruikt om geoorloofde API-aanroepen uit te voeren naar de websiteprovider. De API-sleutel die door de websiteprovider is uitgegeven.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Verificatie

Websites van Workfront-documenten ondersteunen twee verschillende verificatievormen: OAuth2 en ApiKey. In beide gevallen geeft Workfront verificatietokens door in de header wanneer een API-aanroep wordt uitgevoerd.

### OAuth2

OAuth2 staat Workfront toe om erkende API vraag aan een websiteleverancier namens een gebruiker te maken. Voordat de gebruiker dit doet, moet hij zijn externe account voor de documentprovider verbinden met Workfront en Workfront verlenen

toegang om namens hen te handelen. Dit handshaking proces gebeurt slechts eenmaal voor elke gebruiker. Zo werkt het:

1. De gebruiker begint de integratie met de webhaak aan te sluiten op zijn of haar account. Dit gebeurt momenteel door te klikken op het vervolgkeuzemenu Document toevoegen > Service toevoegen > Aangepaste integratienaam.
1. Workfront navigeert door de gebruiker naar de verificatie-URL, die de gebruiker kan vragen zich aan te melden bij de externe documentprovider. Deze pagina wordt gehost door de websiteprovider of het externe documentbeheersysteem. Als u dit doet, voegt Workfront een parameter &quot;state&quot; toe aan de URL van de verificatie. Deze waarde moet worden doorgegeven aan Workfront door dezelfde waarde toe te voegen aan de Workfront Return URI in de onderstaande stap.
1. Na het registreren aan het externe systeem (of als de gebruiker reeds het programma wordt geopend), wordt de gebruiker genomen aan een pagina van de &quot;Authentificatie&quot;, die verklaart dat Workfront toegang aanvraagt om een reeks acties namens de gebruiker uit te voeren.
1. Als de gebruiker op de knop Toestaan klikt, wordt de browser omgeleid naar de Workfront Redirect URI en wordt &quot;code=&quot; toegevoegd`<code>`&quot; aan het querystring. Conform de OAuth2-specificatie is dit token van korte duur. De querystring moet ook het volgende hebben: &quot;state=`<sent_by_workfront>`&quot;.
1. Workfront verwerkt dit verzoek en doet een API vraag aan het Symbolische Eindpunt URL met de vergunningscode.
1. De Symbolische URL van het Eindpunt keert vernieuwt teken en toegangstoken terug.
1. Workfront slaat deze tokens op en past de integratie van de webhaak volledig toe op deze gebruiker.
1. Vanaf dat moment kan Workfront geoorloofde API-aanroepen uitvoeren naar de websiteprovider. Wanneer het maken van deze vraag, zal Workfront het toegangstoken in de HTTP- verzoekkopbal zoals hieronder getoond verzenden:

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. Als het toegangstoken is verlopen, zal Workfront een vraag aan het Symbolische Eindpunt URL maken om een nieuw toegangstoken terug te winnen dan de geautoriseerde API vraag met het nieuwe toegangstoken opnieuw proberen.

### ApiKey

Het maken van geautoriseerde API-aanroepen naar een webhakprovider met behulp van een ApiKey is veel eenvoudiger dan OAuth2. Wanneer Workfront een API-aanroep maakt, geeft het gewoon de gebruikersnaam van ApiKey en Workfront door in de HTTP-aanvraagheader:

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

De leverancier Webhaak kan de gebruikersbenaming gebruiken om gebruiker-specifieke toestemmingen toe te passen. Dit werkt het beste wanneer beide systemen verbinding maken met LDAP via Single Sign On (SSO).

### Aanvraagheaders toevoegen (optioneel)

Naast het gebruiken van of OAuth2 tokens of een ApiKey voor authentificatie, kan Workfront een vooraf bepaalde reeks kopballen naar de webhaleverancier voor elke API vraag verzenden. Een Workfront-beheerder kan dit instellen bij het registreren of bewerken van een Webook-integratie, zoals beschreven in de bovenstaande sectie. Zie Registreren van een Integratie Webhaak.

Dit kan bijvoorbeeld worden gebruikt voor Basic Authentication. Hiervoor voegt de Workfront-beheerder de volgende informatie over Aanvraagkoptekst toe in het dialoogvenster Aangepaste integratie:

   Autorisatie standaard QWxhZGRpbjpvcGVuIHNlc2FtZQ==

waarbij QWxhZGRpbjpvcGVuIHNlc2FtZQ== een base-64-gecodeerde tekenreeks is van &quot;username:password&quot;. Zie Basisverificatie. Op voorwaarde dat dit is toegevoegd, geeft Workfront dit in de HTTP-aanvraagheader door, naast andere aanvraagheaders:

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## API-specificatie

Hieronder vindt u een lijst met API&#39;s die de webhakprovider moet implementeren om documentwebhooks te laten werken.

### Het krijgen OAuth2 Tokens (nodig slechts authentificatie OAuth2)

Keert OAuth2 terug verfrist teken en toegangstoken voor een voor authentiek verklaarde gebruiker. Dit wordt eenmaal aangeroepen wanneer de gebruiker een Document Provider levert. De verdere vraag wordt gemaakt om een bijgewerkt toegangstoken te krijgen.

HTTP-aanvraagPOST /any/url

URL is configureerbaar en beantwoordt aan de Symbolische waarde van URL van het Eindpunt op de pagina van de Opstelling van de douanevertegratie.

**Zoekparameters**

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
   <td> <p>Waarden zijn onder andere "authentication_code" of "refresh_token". De opgegeven waarde geeft aan welke van de twee parameters wordt doorgegeven aan deze API-aanroep: code of refresh_token.</p> </td> 
  </tr> 
  <tr> 
   <td>code</td> 
   <td>afhankelijk</td> 
   <td> <p>De machtigingscode die naar Workfront wordt verzonden vlak nadat de gebruiker op de knop "Grant" klikt. Dit is alleen vereist wanneer het subsidietype "authentication_code" is. De toelatingscode moet van korte duur zijn, die gewoonlijk over 10 minuten of minder afloopt.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>afhankelijk</td> 
   <td> <p>Dit wordt slechts vereist wanneer het maken van verdere vraag om een nieuw access_token terug te winnen, gegeven dat vorige access_token als verlopen. Wanneer het verzenden van deze waarde plaats de subsidie_type parameter aan "verfrist_token".</p> </td> 
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

 

**Antwoord**

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
   <td> <p>Een token dat wordt gebruikt om geautoriseerde API-aanroepen uit te voeren in naam van de gebruiker. Dit zou moeten verlopen om onbevoegde API vraag te verhinderen.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token </td> 
   <td>String</td> 
   <td> <p>Een token van lange duur dat wordt gebruikt om een nieuw access_token op te halen door deze API-methode aan te roepen.</p> </td> 
  </tr> 
  <tr> 
   <td>verloopt_in </td> 
   <td>lang</td> 
   <td>  <p>(facultatief) de tijd (in seconden) alvorens access_token verloopt, over het algemeen 3.600.</p></td> 
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


**Antwoord**

```
{
"access_token":"ad8af5ad5ads759", 
"refresh_token":"9a0h5d87d808ads", 
"expires_id":"3600" 
}
```

### Metagegevens ophalen voor bestand of map

Retourneert metagegevens voor het opgegeven bestand of de opgegeven map.

**URL**

GET /metadata?id=[document- of map-id]

**Zoekparameters**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Naam </th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>id</td> 
   <td>  <p>De id van het bestand of de map, waarnaar wordt verwezen door de websiteprovider. Dit is anders dan de Workfront-document-id. Gebruik de waarde '/' om de metagegevens van de hoofdmap op te halen.</p><p>Opmerking: De maximale lengte voor de id is 255 tekens.</p></td> 
  </tr> 
 </tbody> 
</table>

 

**Antwoord**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Naam </th> 
   <th>Type </th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>titel </td> 
   <td>String </td> 
   <td>De naam van het document of de map</td> 
  </tr> 
  <tr> 
   <td>aardig </td> 
   <td>String </td> 
   <td>Hiermee wordt opgegeven of dit item een bestand of map ('bestand' of 'map') is</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>String </td> 
   <td>De id van het bestand of de map.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>String </td> 
   <td> <p>Het URL-pad dat door een gebruiker wordt gebruikt om het document in een browservenster weer te geven. De URL kan worden gehost door de documentprovider of de native externe opslagprovider.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>String </td> 
   <td> <p>Het URL-pad dat door een gebruiker wordt gebruikt om het document in een browservenster te downloaden. De URL kan worden gehost door de documentprovider of de native externe opslagprovider.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>String </td> 
   <td>Het MIME-type voor het bestand. (optioneel)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>String </td> 
   <td>De laatste keer dat dit bestand is gewijzigd (RFC 339-tijdstempel opgemaakt)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
   <td>Lang</td> 
   <td>  De grootte van het bestand in bytes. (optioneel)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Boolean</td> 
   <td>  <p> Hiermee wordt aangegeven of dit bestand of deze map alleen-lezen is voor de geverifieerde gebruiker.(optioneel)</p><p> </p></td> 
  </tr> 
 </tbody> 
</table>

**Voorbeeld:** `https://www.acme.com/api/metadata?id=12345`

**Antwoord**

```
{
"title":"My Document", 
"kind":"file"
"id":"12345", 
"viewLink":"https://www.acme.com/viewDocument?id=12345", 
"downloadLink":"https://www.acme.com/downloadDocument?id=12345",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size": "32554694"
}
```

>[!NOTE]
>
>Foutafhandeling moet consistent zijn voor alle API-aanroepen. Zie de sectie &quot;Foutverwerking&quot; hieronder voor meer informatie.

### Een lijst met items in een map ophalen

Retourneert metagegevens voor de bestanden en mappen voor een bepaalde map.

**URL**

GET/bestanden

**Zoekparameters**

| Naam  | Beschrijving |
|---|---|
| parentId  | De map-id. Gebruik de waarde &#39;/&#39; om de metagegevens van de hoofdmap op te halen. |

{style=&quot;table-layout:auto&quot;}

De API voor documentwebhooks biedt momenteel geen ondersteuning voor paginering.

**Antwoord**

JSON bevat een lijst met bestanden en mappen. De meta-gegevens voor elk punt zijn het zelfde dat door het /metadata eindpunt is teruggekeerd.

**Voorbeeld:** `https://www.acme.com/api/files?parentId=123456`

**Antwoord**

```
[
{
"title":"Folder A",
"kind":"folder",
"id":"2lj23lkj",
"viewLink":"https://www.acme.com/viewDocument?id=2lj23lkj",
"downloadLink":"https://www.acme.com/downloadDocument?id=2lj23lkj",
"mimeType":"",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"" 
},
{
"title":"My Document",
"kind":"file",
"id":"da8cj234"
"viewLink":"https://www.acme.com/viewDocument?id=da8cj234",
"downloadLink":"https://www.acme.com/downloadDocument?id=da8cj234",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"32554694"
},
]
```

### Een zoekopdracht uitvoeren

Retourneert metagegevens voor de bestanden en mappen die door een zoekopdracht worden geretourneerd. Dit kan als full-text onderzoek of als regelmatige gegevensbestandvraag worden uitgevoerd. Workfront roept het /search eindpunt wanneer de gebruiker een onderzoek van externe dossierbrowser uitvoert.

**URL**

GET/zoekopdracht

**Zoekparameters**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Naam </th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>query</td> 
   <td>De zoekterm of uitdrukking.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(optioneel) De map-id waaruit de zoekopdracht is uitgevoerd. Opmerking: Dit is een tijdelijke aanduiding voor een toekomstige functie in Workfront. Workfront geeft deze parameter momenteel niet door. </p> </td> 
  </tr> 
  </tbody> 
</table>

De API voor documentwebhooks biedt momenteel geen ondersteuning voor paginering.

 

**Antwoord**

JSON bevat een lijst met metagegevens voor bestanden en mappen die overeenkomen met de query. Wat een &quot;gelijke&quot;is wordt bepaald door de websiteleverancier. In het ideale geval wordt een zoekopdracht in volledige tekst uitgevoerd. Het uitvoeren van een op bestandsnaam gebaseerde zoekopdracht werkt ook.

**Voorbeeld:** `https://www.acme.com/api/search?query=test-query`

**Antwoord**

```
[
{ File/Folder Metadata },
{ File/Folder Metadata }
]
```

### De inhoud van een document ophalen

Hiermee worden de onbewerkte bytes van een document geretourneerd

**URL**

GET/download

**Zoekparameters**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Naam </th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td> De document-id.</td> 
  </tr> 
 </tbody> 
</table>

 

**Antwoord**

De onbewerkte bytes van het document.

**Voorbeeld:** `https://www.acme.com/api/download?id=123456`

### Een miniatuur voor een document ophalen

Retourneert de onbewerkte miniatuurbytes voor een document.

**URL**

GET /miniatuur

**Zoekparameters**

| Naam  | Beschrijving |
|---|---|
| id  | De document-id. |
| size  |  De breedte van de miniatuur |

{style=&quot;table-layout:auto&quot;}

 

**Antwoord**

De onbewerkte miniatuurbytes.

**Voorbeeld:** `https://www.acme.com/api/thumbnail?id=123456`

### Een bestand uploaden - Deel 1 van 2

Het uploaden van een dossier aan een leverancier van de documentopslag is een proces in twee stappen dat twee afzonderlijke API eindpunt vereist. Workfront begint het uploadproces door /uploadInit te roepen. Dit eindpunt keert een document identiteitskaart terug die dan tot /upload wordt overgegaan wanneer het uploaden van de documentbytes. Afhankelijk van het onderliggende documentopslagsysteem kan het nodig zijn om een document met een lengte van nul te maken en de inhoud van het document later bij te werken.

De document-id en de document-versie-id zijn toegevoegd aan versie 1.1 van deze specificatie en kunnen worden gebruikt om extra informatie van Workfront op te halen. Als het documentbeheersysteem bijvoorbeeld extra informatie over het document wil, kan de webhimplementatiecode de document-id gebruiken om die informatie op te halen met behulp van de Workfront RESTful-API. Als goede praktijk, kon deze informatie uit de gebieden van douanegegevens op het document komen en het bevat taak, kwestie, of project.

**URL**

POST /uploadInit

**Zoekparameters**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Naam </th> 
   <th>Beschrijving</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId </td> 
   <td>De bovenliggende map-id, waarnaar wordt verwezen door de websiteprovider.</td> 
  </tr> 
  <tr> 
   <td>filename </td> 
   <td>De naam van het document</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>De Workfront-document-id (toegevoegd in versie 1.1)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>De Workfront-document versie-id (toegevoegd in versie 1.1)</td> 
  </tr> 
 </tbody> 
</table>

 

**Antwoord**

De meta-gegevens voor het dossier, zoals die door het /metadata eindpunt wordt bepaald.

**Voorbeeld:** `https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**Antwoord**

`[file_metadata]` bevat de nieuwe document-id die door de documentprovider wordt gebruikt.

### Een bestand uploaden - Deel 2 van 2

Hiermee uploadt u de bytes van een document naar de websiteprovider.

**URL**

PUT /upload

**Zoekparameters**

| Naam  | Beschrijving |
|---|---|
| id  |  De document-id, die zojuist is gemaakt. |


 

**Verzoek**

De onbewerkte inhoudbytes voor het document.

**Antwoord**

```
{
"result": "success"
}
```

of

```
{
"result": "fail"
}
```

**Voorbeeld:** `https://www.acme.com/api/upload?id=1234` *[documentbytes die zijn opgenomen in updatestroom]*

**Antwoord**

```
{
"result":"success"
}
```

### Informatie ophalen over de service 

(Releasedatum - TBD) Retourneert informatie over de service, zoals functies en mogelijkheden. Workfront gebruikt deze informatie om de gebruikersinterface in Workfront aan te passen. Als de implementatie van de webhaak bijvoorbeeld aangepaste handelingen bevat, moet de JSON deze bewerkingen in de JSON opnemen. Gebruikers kunnen deze acties dan aanroepen vanuit Workfront.

**URL**

GET/serviceInfo

Zoekparameters

Geen. Bovendien zouden de vraag aan dit eindpunt geen authentificatie moeten vereisen.

**Antwoord**

JSON met informatie over deze service

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
   <td>webhaakversie </td> 
   <td>String </td> 
   <td>De webhaakversie die door deze service is geïmplementeerd. Dit is het versienummer dat boven aan deze specificatie staat.</td> 
  </tr> 
  <tr> 
   <td>versie </td> 
   <td>String </td> 
   <td>Het interne versienummer voor deze service. Dit nummer wordt bepaald door de webshservice provider en wordt alleen ter informatie gebruikt.<br><br></td> 
  </tr> 
  <tr> 
   <td>uitgever </td> 
   <td>String </td> 
   <td>De naam van het bedrijf dat de implementatie van de website verstrekt.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>String </td> 
   <td>Een lijst die de API Eindpunten bevat die door deze dienst worden uitgevoerd. Dit kan worden gebruikt om ervoor te zorgen dat de gebruikersinterface in Workfront de mogelijkheden weerspiegelt die door de websiteprovider worden aangeboden. Elk punt in de lijst moet de naam van het eindpunt (zoals "onderzoek") omvatten.</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>String</td> 
   <td>  <p>Een lijst met de aangepaste bewerkingen die door deze webhaak worden uitgevoerd. Elk lijstitem bevat een naam en een weergavenaam. De weergavenaam wordt weergegeven in het vervolgkeuzemenu "Documenthandelingen" in Workfront. Het klikken op het punt in dropdown zal de actie in webhaak aanhalen door het /customAction eindpunt te roepen.</p></td> 
  </tr> 
 </tbody> 
</table>

**Voorbeeld:** https://www.acme.com/api/serviceInfo

**Retourneert**

```
{
"webhook version": "1.2", "version": "1.0", "publisher": "Acme, LLC", "availableEndpoints": ["files", "metadata", "search", "download"

"thumbnail", "uploadInit", "upload" ], "customActions" [
{
"name": "archive", "displayName": "Archive" }, {

"name": "doSomethingElse", "displayName": "Do Something" }, ] }
```

### Een map maken

(Toegevoegd in versie 1.2) Hiermee maakt u een map in een bepaalde map.
URL

POST /createFolder

**Zoekparameters**

| Naam  | Beschrijving |
|---|---|
| parentId  | De map-id waarin de map moet worden gemaakt |
| name  | De naam van de nieuwe map |

{style=&quot;table-layout:auto&quot;}

 

**Antwoord**

De meta-gegevens voor de pas gecreëerde omslag, zoals die door het /metadata eindpunt wordt bepaald.

**Voorbeeld:** `POST https://www.acme.com/api/createFolder`

```
-------------------------------

parentId=1234

name=New Folder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

retourneert

```
{"title":"New Folder", 
 "kind":"folder""id":"5678",
 "viewLink":"",
 "downloadLink":"",
 "mimeType":"",
 "dateModified":"2014­06­05T17:39:45.251Z" 
 "size": "" 
 }
```

### Een document of map verwijderen

(Releasedatum - TBD) Hiermee verwijdert u een document of map met de opgegeven id in het externe systeem. Als u een map verwijdert, wordt ook de inhoud van de map verwijderd.

URL

PUT /delete

**Zoekparameters**

| Naam  | Beschrijving |
|---|---|
| documentId  | Te verwijderen document-id |
| folderId  |  De te verwijderen map-id |

{style=&quot;table-layout:auto&quot;}

Antwoord Een JSON-tekenreeks die aangeeft of de functie is gelukt of mislukt, zoals is opgegeven in de sectie Foutafhandeling hieronder.

**Voorbeeld:** PUT https://www.acme.com/api/delete

retourneert

```
{
"status": "success" 
}
```

retourneert

```
{
"status": "failure", "error": "File not found"
}
```


### De naam van een document of map wijzigen

(Releasedatum - TBD) Hiermee wijzigt u de naam van een document of map met de opgegeven id in het externe systeem.

URL

PUT /naam wijzigen

**Zoekparameters**

| Naam  | Beschrijving |
|---|---|
| id | De document- of map-id waarvan de naam moet worden gewijzigd |
| name  | De nieuwe naam van het document of de map |

{style=&quot;table-layout:auto&quot;}

 

Antwoord

Een JSON-tekenreeks die aangeeft of de functie is gelukt of mislukt, zoals is opgegeven in de sectie Foutafhandeling hieronder.

**Voorbeeld:**

`PUT https://www.acme.com/api/rename`

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

```
{
"status": "success" 
}returns
{
"status": "failure", error: "Folder cannot be renamed because a folder with that name already exists." 
}
```

### Een aangepaste handeling uitvoeren

(Releasedatum - TBD) Met dit eindpunt kan een Workfront-gebruiker (of misschien een geautomatiseerde workflowgebeurtenis) een actie uitvoeren in het externe systeem. Het /customAction eindpunt keurt een &quot;naam&quot;parameter goed, die de websiteleverancier toestaat om veelvoudige douaneverrichtingen uit te voeren.

De websiteleverancier registreert douaneacties met Workfront door de acties in de /serviceInfo reactie onder customActions te omvatten. Workfront laadt deze lijst bij het instellen of vernieuwen van de websiteprovider onder Instellen > Documenten > Aangepaste integratie.\
![](assets/mceclip0-350x262.png)

Gebruikers kunnen de aangepaste handeling activeren door de sectie onder &quot;Documenthandelingen&quot; te selecteren\
![](assets/mceclip1-350x95.png)

**URL**

GET /customAction

**Zoekparameters**

<table style="table-layout:auto">
 <col>
 <col>
 <thead>
  <tr>
   <th>Naam </th>
   <th>Beschrijving</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><p>name</p></td>
   <td><p>De id die het type handeling aangeeft dat moet worden uitgevoerd. Deze waarde beantwoordt aan één van de waarden customAction die door het /serviceInfo eindpunt zijn teruggekeerd.</p></td>
  </tr>
  <tr>
   <td>documentId </td>
   <td>De werkfront document-id waarvoor de handeling wordt uitgevoerd.</td>
  </tr>
  <tr>
   <td>documentVersionId </td>
   <td> De werkfront document versie-id waarvoor de handeling wordt uitgevoerd.</td>
  </tr>
 </tbody>
</table>

 

**Antwoord**

Een JSON-tekenreeks die aangeeft of de functie is gelukt of mislukt, zoals is opgegeven in de sectie Foutafhandeling hieronder. Bij een fout (d.w.z. status = &quot;mislukking&quot;) geeft Workfront het aangeboden foutbericht aan de gebruiker weer.

**Voorbeeld:** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30 ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

reactie

```
{
"status": "success" 
}
```


## Foutafhandeling

Er kunnen zich problemen voordoen bij het verwerken van API-aanvragen. Dit zou op een verenigbare manier over alle API eindpunten moeten worden behandeld. Wanneer er een fout optreedt, doet de websiteprovider het volgende:

* Neem een foutcode op in de antwoordkop. Foutcodes zijn:

   * 403 - Verboden. Geeft aan dat de aanvraagtokens ontbreken of ongeldig zijn of dat referenties die aan de tokens zijn gekoppeld, geen toegang hebben tot de opgegeven bron. Workfront probeert nieuwe toegangstokens op te halen voor webhaken die op OAuth zijn gebaseerd.
   * 404 - Niet gevonden. Geeft aan dat het opgegeven bestand of de map niet bestaat.
   * 500 - Interne serverfout. Een ander type fout.

* Beschrijf de fout in het reactievermogen gebruikend het volgende formaat:


```
{
"status": "error"
"error": "Sample error message" 
}
```


## Testen

Voer de volgende tests uit om te controleren of de implementatie van uw documentwebhaak correct werkt. Dit zijn handtests die de Workfront-webinterface doorlopen en indirect de eindpunten voor uw webhaakimplementatie raken.

### Vereisten

Voor het uitvoeren van deze tests hebt u het volgende nodig:

* Een Workfront-account met ADM (Advanced Document Management) ingeschakeld
* Een Workfront-gebruiker voor dit account met System Admin Rights
* Een WebHaakinstantie van het Document, die de eindpunten van HTTP voor Workfront toegankelijk zijn

Bij deze tests wordt er ook van uitgegaan dat u de instantie WebHaak van document al in Workfront hebt geregistreerd onder Instellen > Documenten > Aangepaste integratie.

### Test 1: Verstrek de dienst van Webhaak van het Document voor een gebruiker

Test URL van de Authentificatie en Symbolische Eindpunt URL voor op OAuth-Gebaseerde Leveranciers van Webhaken.

1. Ga in Workfront naar de hoofdpagina Documenten door op de koppeling Documenten in de bovenste navigatiebalk te klikken.
1. Klik op Add dropdown Documenten en selecteer uw dienst van Webhaak van het Document onder Add de Dienst.
1. (Alleen OAuth-services) Nadat u de vorige stap hebt uitgevoerd, wordt de pagina voor OAuth2-verificatie van uw service geladen in een pop-upvenster. (Opmerking: u wordt mogelijk eerst gevraagd zich aan te melden bij uw service.) Via de verificatiepagina geeft u Workfront toegang tot de account van de gebruiker door op de knop Vertrouwd of Toestaan te klikken.
1. Controleer of uw service is toegevoegd aan het vervolgkeuzemenu Documenten toevoegen. Vernieuw de browser als deze standaard niet wordt weergegeven.

### Test 2: Een document koppelen aan Workfront Test de volgende eindpunten: /bestanden, /metadata

1. Ga in Workfront naar de hoofdpagina Documenten door op de koppeling Documenten in de bovenste navigatiebalk te klikken.
1. Selecteer de documentservice Webhaak onder Documenten toevoegen.
1. Navigeer in het modaal door de mappenstructuur.
1. Controleer of u de mapstructuur correct kunt navigeren.
1. Een document selecteren en koppelen naar Workfront

### Test 3: Naar een document navigeren in het inhoudsbeheersysteem

Test de volgende eindpunten: /metadata (in het bijzonder viewLink)

1. Een document koppelen aan Workfront
1. Selecteer het document en klik op de koppeling Openen.
1. Controleer of het document op een nieuw tabblad wordt geopend.

### Test 4: Naar een document in het inhoudsbeheersysteem navigeren (met aanmelding)

Test de volgende eindpunten: /metadata (in het bijzonder viewLink)

1. Zorg ervoor dat u bent afgemeld bij het inhoudsbeheersysteem.
1. Koppel een document aan Workfront.
1. Selecteer het document en klik op de koppeling Openen.
1. Controleer of het aanmeldingsscherm van het inhoudsbeheersysteem op een nieuw tabblad wordt geladen.
1. Aanmelden en controleren of u naar het document bent gegaan

### Test 5: Het document downloaden van het contentbeheersysteem

Test de volgende eindpunten: /metadata (in het bijzonder de downloadLink)

1. Koppel een document aan Workfront.
1. Selecteer het document en klik op de koppeling Downloaden.
1. Controleer of het downloaden begint.

### Test 6: Inhoud zoeken

Test de volgende eindpunten: /search

1. Ga in Workfront naar de hoofdpagina Documenten door op de koppeling Documenten in de bovenste navigatiebalk te klikken.
1. Selecteer de documentservice Webhaak onder Documenten toevoegen.
1. Voer een zoekopdracht uit vanuit het modaal.
1. Controleer of de zoekresultaten correct zijn.

### Test 7: Document van Workfront naar inhoudsbeheersysteem verzenden

Test de volgende eindpunten: /files, /uploadInit, /upload

1. Ga in Workfront naar de hoofdpagina Documenten door op de koppeling Documenten in de bovenste navigatiebalk te klikken.
1. Een document vanaf uw computer uploaden naar Workfront
1. Ga naar de pagina met documentdetails
1. Selecteer in het vervolgkeuzemenu Documenthandelingen de documentservice onder Verzenden naar...
1. Ga naar de gewenste doelmap en klik op de knop Opslaan.
1. Controleer of het document naar de juiste locatie in het inhoudsbeheersysteem is geüpload.

### Test 8: Miniaturen weergeven in Workfront

Test de volgende eindpunten: /miniatuur

1. Koppel een document aan Workfront.
1. Selecteer het document in de lijst.
1. Controleer of de miniatuur in het rechterdeelvenster wordt weergegeven.

### Test 9: De inhoudbytes ophalen

Test de volgende eindpunten: /download

1. Koppel een document aan Workfront.
1. Ga naar de pagina met documentdetails.
1. Het document naar Workfront verzenden door Documenthandelingen > Verzenden naar te selecteren.. > Workfront. Hiermee wordt een nieuwe documentversie in Workfront gemaakt.
1. Download het document vanuit Workfront door op de koppeling Downloaden te klikken.

### Test 10: Toegangstoken vernieuwen (alleen OAuth2 Webhaak-providers)

Test de volgende eindpunten: URL van token-eindpunt

1. Verricht de dienst van Webhaak van het Document voor een gebruiker
1. Maak het toegangstoken van de gebruiker ongeldig door 1 te wachten op time-out, of 2) het manueel ongeldig te maken in het externe systeem.
1. Vernieuw het toegangstoken in Workfront. U kunt dit bijvoorbeeld doen door een document aan Workfront te koppelen. Het toegangstoken is vernieuwd als u naar een document kunt navigeren en er een koppeling naar kunt maken.

>[!NOTE]
>
>De optie Verzenden naar.. is niet beschikbaar voor gekoppelde documenten. Dit wordt door Workfront toegevoegd. U kunt het /download eindpunt testen door het eindpunt manueel te raken gebruikend een cliënt REST, zoals Postman. Alternatief, kan het /download eindpunt worden getest door een digitaal bewijs te produceren. Neem contact op met Workfront om digitale proefdrukken in te schakelen.

## Versies

* Versie 1.0 (Releasedatum - mei 2015)

   * Oorspronkelijke specificatie

* Versie 1.1 (Releasedatum - juni 2015)

   * Bijgewerkt /uploadInit - Toegevoegde documentId en documentVersionId

* Versie 1.2 (Releasedatum - oktober 2015)

   * Toegevoegde /createFolder

