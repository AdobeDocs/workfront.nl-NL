---
content-type: api
navigation-topic: api-navigation-topic
title: JWT-stroom gebruiken voor aangepaste OAuth 2-toepassingen
description: JWT-stroom gebruiken voor aangepaste OAuth 2-toepassingen
author: Becky
feature: Workfront API
role: Developer
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Configureer en gebruik de aangepaste OAuth 2-toepassingen van uw organisatie met behulp van JWT-flow

Als u wilt integreren met Workfront en uw clienttoepassing in staat wilt stellen namens de gebruiker te communiceren met Workfront, moet u:

* Een OAuth2-toepassing maken
* Een certificaat met openbare sleutel maken
* Een JSON-webtoken (JWT) maken

## Een OAuth2-toepassing maken

Voor instructies over het maken van de OAuth2-toepassing raadpleegt u [Een OAuth2-toepassing maken met serververificatie (JWT-stroom)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) in [OAuth2-toepassingen maken voor Workfront-integratie](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Een certificaat met openbare sleutel maken

JWT moet worden ondertekend en basis-64 worden gecodeerd voor opneming in het toegangsverzoek. De JWT-bibliotheken bieden functies om deze taken uit te voeren.

Het token moet worden ondertekend met de persoonlijke sleutel voor een digitaal ondertekeningscertificaat. Als u dat doet, kunt u de persoonlijke sleutel van elk gekoppeld certificaat gebruiken om uw JWT te ondertekenen.

Het gebruikte algoritme is RS256 (RSA-handtekening met SHA-256). Dit is een asymmetrisch algoritme, en het gebruikt een openbare/privé zeer belangrijke paar. De identiteitsprovider heeft een persoonlijke (geheime) sleutel die wordt gebruikt om de handtekening te genereren en de consument van de JWT krijgt een openbare sleutel om de handtekening te valideren.

Als u de openbare sleutel wilt genereren, gaat u **één** van de volgende punten.

* Open uw MacOS/Linux-terminal en voer de volgende opdracht uit. Upload vervolgens `certificate_pub.crt` met de **Openbare sleutel toevoegen** in de OAuth2-toepassingsinstellingen in Workfront.

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* Gebruik de **Een openbaar/privé-sleutelpaar genereren** in de OAuth2 toepassingsopstelling in Workfront om RSA te produceren.

## Een JSON-webtoken maken

Een JSON-webtoken voor verificatie van serviceaccount vereist een bepaalde set claims en moet worden ondertekend met een geldig digitaal ondertekeningscertificaat. Wij adviseren dat u één van de openbaar beschikbare bibliotheken of hulpmiddelen gebruikt om uw JWT te bouwen.

De volgende lijst bevat informatie over gebieden die kunnen worden vereist wanneer u het teken JWT vormt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">exp</td> 
   <td> <p>Vereist. De vervalparameter is een vereiste parameter die de absolute tijd vanaf 01/01/1970 GMT meet. U moet ervoor zorgen dat de vervaltijd later is dan het tijdstip van uitgifte. Na deze tijd is de JWT niet meer geldig. </p> <p>Opmerking: we raden u aan een token met een korte levensduur (enkele minuten) te gebruiken, zodat het kort na de ruil verloopt voor een toegangstoken. Telkens wanneer een nieuw toegangstoken wordt vereist, wordt één JWT ondertekend en geruild. Dit is een veiligere aanpak. We raden niet langer gebruikte tokens aan die opnieuw worden gebruikt om zo nodig toegangstokens te verkrijgen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">is</td> 
   <td>Vereist. De uitgever is uw klant-id uit de OAuth2-toepassingsgegevens.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>Vereist. Het onderwerp is uw Gebruiker - identiteitskaart die de openbare sleutel in opstelling creeerde.</td> 
  </tr> 
 </tbody> 
</table>

## Uitwisseling JWT om een toegangstoken terug te winnen

1. Verzend een verzoek van de POST naar:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. De hoofdtekst van de aanvraag moet URL-gecodeerde parameters bevatten met uw client-id, clientgeheim en JWT:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
