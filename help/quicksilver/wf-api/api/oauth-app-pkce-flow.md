---
content-type: api
navigation-topic: api-navigation-topic
title: PKCE-stroom gebruiken voor OAuth 2-toepassingen
description: PKCE-stroom gebruiken voor OAuth 2-toepassingen
author: Becky
feature: Workfront API
role: Developer
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# Configureer en gebruik de aangepaste OAuth 2-toepassingen van uw organisatie met PKCE-stroom

PKCE is een veilige autorisatiestroom die goed werkt bij dynamisch vernieuwende toepassingen zoals mobiele apps, maar waardevol is voor alle OAuth2-clients. In plaats van een statisch clientgeheim gebruikt PKCE een dynamisch gegenereerde tekenreeks, waardoor het risico van een gelekt clientgeheim wordt verwijderd.

## PKCE-overzicht

Een PKCE-stroom heeft de volgende stappen. De stappen in deze sectie worden alleen ter informatie weergegeven. Zie andere secties in dit artikel voor informatie over het uitvoeren van deze procedures.

1. De client maakt de `code_challenge` door de `code_verifier` using `S256` -codering te transformeren.

1. De client stuurt de browser samen met de gegenereerde `code_challenge` naar de aanmeldingspagina van OAuth2. U moet uw app (Client) registreren zodat OAuth2 de autorisatieaanvraag kan accepteren. Na registratie kan uw toepassing de browser omleiden naar OAuth2.

1. De OAuth2 Server van de Vergunning leidt de authentificatieherinnering aan de Gebruiker opnieuw.

1. De gebruiker verklaart zich gebruikend één van de gevormde login opties voor authentiek, en kan een toestemmingspagina zien die van de toestemmingen OAuth2 aan de toepassing een lijst maakt.

1. OAuth2 leidt terug naar uw toepassing met `authorization code`.

1. Uw toepassing verzendt deze code samen met de `code_verifier` naar OAuth2.

1. OAuth2 Authorization Server transformeert `code_verifier` gebruikend `code_challenge_method` van het aanvankelijke vergunningsverzoek, en controleert het resultaat tegen `code_challenge`. Als de waarde van beide tekenreeksen overeenkomt, heeft de server gecontroleerd of de aanvragen afkomstig zijn van dezelfde client en geeft deze een `access token` uit.

1. OAuth2 retourneert de `access token` en optioneel een `refresh token` .

1. Uw toepassing kan deze tokens nu gebruiken om de resourceserver, zoals een API, namens de gebruiker aan te roepen.

1. De bronserver valideert het token voordat wordt gereageerd op het verzoek.


## Uw toepassing configureren

Voordat u autorisatie kunt implementeren, moet u uw app registreren in OAuth2 door een app-integratie te maken vanuit Workfront.

Voor instructies bij het creëren van de toepassing OAuth2, zie [ een OAuth2 enig-pagina Webtoepassing gebruikend PKCE ](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) in [ creëren toepassingen OAuth2 voor de integratie van Workfront ](../../administration-and-setup/configure-integrations/create-oauth-application.md)

>[!NOTE]
>
>U kunt tot een totaal van tien Toepassingen OAuth2 in één keer hebben.


## Proefsleutel maken voor Codeuitwisseling

Net als bij de standaardstroom van de machtigingscode, begint de app met het doorsturen van de browser van de gebruiker naar het `/authorize` -eindpunt van de machtigingsserver. In deze instantie moet u echter ook een code-uitdaging doorgeven.

Uw eerste stap is het produceren van een code verificateur en uitdaging.

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">Code-verificateur</td>
        <td>
          <p>Willekeurige URL-veilige tekenreeks met een minimale lengte van 43 tekens</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Codeuitdaging</td>
        <td>
          <p>Base64 URL-gecodeerde SHA-256-hash van de codeverificateur</p>
        </td>
      </tr>
    </tbody>
</table>


U moet code toevoegen in uw clienttoepassing om de code-verificateur en de code-uitdaging te maken.

De PKCE-generatorcode maakt uitvoer die vergelijkbaar is met het volgende:

>[!INFO]
>
>**Voorbeeld:**
>
>```
>{
>  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>}
>```

Uw app slaat de `code_verifier` for later op en verzendt de `code_challenge` samen met de autorisatieaanvraag naar de URL `/authorize` van de machtigingsserver.

## Aanvragen van een machtigingscode

Als u de standaard Server van de Vergunning van de Douane gebruikt, dan zou uw verzoek URL aan het volgende gelijkaardig zijn:

>[!INFO]
>
>**Voorbeeld:**
>
>
>```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

Maak een notitie van de parameters die worden doorgegeven:

* `client_id` komt overeen met de client-id van de OAuth2-toepassing die u in de toepassing hebt gemaakt tijdens het configureren van de toepassing.

  Zie Een OAuth2-webtoepassing van één pagina maken met PKCE in OAuth2-toepassingen maken voor Workfront-integratie voor instructies.

* `response_type` is `code` omdat de toepassing het subsidietype voor machtigingscode gebruikt.

* `redirect_uri` is de callback plaats waaraan de gebruikersagent samen met `code` wordt geleid. Dit moet één van redirect URls aanpassen die u specificeerde toen u uw toepassing OAuth2 creeerde.

* `code_challenge_method` is de knoeiboelmethode die wordt gebruikt om de uitdaging te produceren, die altijd `S256` voor Workfront Oauth2 toepassingen is die PKCE gebruiken.

* `code_challenge` is de code die voor PKCE wordt gebruikt.


## De code voor tokens uitwisselen

Als u de machtigingscode voor een toegangstoken wilt uitwisselen, geeft u deze samen met `code_verifier` door aan het eindpunt van de machtigingsserver `/token` .

>[!INFO]
>
>**Voorbeeld:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> In tegenstelling tot de regelmatige stroom van de Code van de Vergunning, vereist deze vraag niet de kopbal van de Vergunning met identiteitskaart van de Cliënt en geheim. Daarom is deze versie van de machtigingscode-stroom geschikt voor systeemeigen toepassingen, zoals mobiele toepassingen of toepassingen van één pagina die geen back-end hebben.

Maak een notitie van de parameters die worden doorgegeven:

* `grant_type` is `authorization_code` , omdat de toepassing het subsidietype voor machtigingscode gebruikt.

* `redirect_uri` moet overeenkomen met de URI die is gebruikt om de machtigingscode op te halen.

* `code` is de vergunningscode die u van het /authorize eindpunt ontving.

* `code_verifier` is de PKCE codecontroleur die uw app in [ wordt geproduceerd creeert de Sleutel van het Bewijs voor de Uitwisseling van de Code ](#Create).

* `client_id` identificeert uw klant en moet overeenkomen met de waarde die vooraf is geregistreerd in OAuth2.


Als de code nog geldig is en de verificateur van de code aanpast, ontvangt uw toepassing een toegangstoken.

>[!INFO]
>
>**Voorbeeld:**
>
>```
>{
>    "access\_token": "eyJhd\[...\]Yozv",
>    "expires\_in": 3600,
>    "token\_type": "Bearer"
>}
>```

## Het toegangstoken valideren

Wanneer uw toepassing een verzoek met een toegangstoken overgaat, moet de middelserver het bevestigen.

U kunt uw toegangstoken met een API vraag bevestigen gelijkend op het volgende:

>[!INFO]
>
>**Voorbeeld:**
>
>```
>/attask/api/<api version>/proj/search \\
>  --header 'sessionID: <access\_token>' \\
>```

## Een vernieuwingstoken aanvragen

Als u een vernieuwingstoken wilt aanvragen, kunt u een POST-aanroep naar de API maken, vergelijkbaar met het volgende:

>[!INFO]
>
>**Voorbeeld:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
