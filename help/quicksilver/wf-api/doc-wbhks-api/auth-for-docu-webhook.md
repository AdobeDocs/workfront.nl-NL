---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Verificatie voor documentwebhooks
description: Verificatie voor documentwebhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Verificatie voor documentwebhooks

## Verificatie

Websites van Adobe Workfront-documenten ondersteunen twee verschillende verificatievormen: OAuth2 en ApiKey. In beide gevallen geeft Workfront verificatietokens door in de header wanneer een API-aanroep wordt uitgevoerd.

### OAuth2

OAuth2 staat Workfront toe om erkende API vraag aan een websiteleverancier namens een gebruiker te maken. Voordat de gebruiker dit doet, moet hij zijn externe account voor de documentprovider verbinden met Workfront en Workfront verlenen

toegang om namens hen te handelen. Dit handshaking proces gebeurt slechts eenmaal voor elke gebruiker. Zo werkt het:

1. De gebruiker begint de integratie met de webhaak aan te sluiten op zijn of haar account. Dit gebeurt momenteel door te klikken op het vervolgkeuzemenu Document toevoegen > Service toevoegen > Aangepaste integratienaam.
1. Workfront navigeert door de gebruiker naar de verificatie-URL, die de gebruiker kan vragen zich aan te melden bij de externe documentprovider. Deze pagina wordt gehost door de websiteprovider of het externe documentbeheersysteem. Als u dit doet, voegt Workfront een parameter &quot;state&quot; toe aan de URL van de verificatie. Deze waarde moet worden doorgegeven aan Workfront door dezelfde waarde toe te voegen aan de Workfront Return URI in de onderstaande stap.
1. Na het registreren aan het externe systeem (of als de gebruiker reeds het programma wordt geopend), wordt de gebruiker genomen aan een pagina van de &quot;Authentificatie&quot;, die verklaart dat Workfront toegang aanvraagt om een reeks acties namens de gebruiker uit te voeren.
1. Als de gebruiker &quot;toestaat&quot;knoop klikt, zal browser aan Workfront Redirect URI opnieuw richten, toevoegend &quot;code= `<code>`&quot;aan het querystring. Conform de OAuth2-specificatie is dit token van korte duur. Het querystring moet ook het volgende hebben, &quot;state= `<sent_by_workfront>`&quot;.
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

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of "username:password". See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
