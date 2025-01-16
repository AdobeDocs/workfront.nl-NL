---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: HTTP&gt; Overige modules
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# HTTP > Overige modules

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ HTTP > Andere modules ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/universal-connectors/http-modules.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

>[!NOTE]
>
>[!UICONTROL Adobe Workfront Fusion] vereist een [!UICONTROL Adobe Workfront Fusion] licentie naast een [!UICONTROL Adobe Workfront] licentie.

De app [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] biedt verschillende modules voor communicatie op basis van het HTTP-protocol (Hypertext Transfer Protocol). HTTP is de stichting van gegevensmededeling voor het World Wide Web. U kunt de modules gebruiken om Web-pagina&#39;s en dossiers te downloaden, Web-haken en API eindpunten te roepen, etc.

De juiste keuze van de module is afhankelijk van het verificatie-/verificatiemechanisme waartoe de bron waartoe u toegang wilt hebben, behoort. Hieronder volgen voorbeelden van modules

* Voer een verzoek in:universele module hoofdzakelijk bedoeld voor middelen die geen enkele vorm van authentificatie/vergunning gebruiken
* Voer een Basic Auth-verzoek uit:voor bronnen die gebruikmaken van [!DNL HTTP] Basic authentication (BA)
* Maak een OAuth 2.0 verzoek: voor middelen die OAuth 2.0 vergunningsprotocol gebruiken
* Maak een verzoek van de Auteur van het Certificaat van de Cliënt: voor middelen die vergunningsprotocol gebruiken dat een cliënt-zijcertificaat vereist.
* Maak een aanvraag voor een API-sleutelautorisatie: voor bronnen die API-sleutels gebruiken voor autorisatie.

>[!NOTE]
>
>Als u verbinding maakt met een product van de Adobe dat momenteel geen speciale aansluiting heeft, raden we u aan de Adobe Authenticator-module te gebruiken.
>
>Voor meer informatie, zie [ module van Adobe Authenticator ](/help/quicksilver/workfront-fusion/apps-and-their-modules/adobe-authenticator-modules.md).

## Aanvraagmodules

Zie de volgende artikelen voor specifieke instructies van de verzoekmodule:

* [[!UICONTROL HTTP] > [!UICONTROL Make a request] module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL Make a Basic Authorization request] module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL Make a Client Certificate Authorization request] module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Make an API Key Authorization request]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

## Overige actiemodules

* [[!UICONTROL Get a File]](#get-a-file)
* [[!UICONTROL Resolve a target URL]](#resolve-a-target-url)

### [!UICONTROL Get a File]

Deze actiemodule downloadt een bestand van de opgegeven URL. Nadat het bestand is gedownload, kunt u het bestand verder verwerken (de bestandsgegevens toewijzen) met behulp van andere modules in het scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Voer de URL in van het bestand dat u wilt downloaden of wijs deze toe. </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Resolve a target URL]

Deze actiemodule verhelpt een keten van HTTP-omleidingen en retourneert een doel-URL.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>Voer de URL die u wilt omzetten in of wijs deze toe, bijvoorbeeld een [!DNL bit.ly] URL.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method] </td> 
   <td> <p>Selecteer of u de methode [!UICONTROL HEAD] of [!UICONTROL GET] wilt gebruiken.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Iteratormodules

### [!UICONTROL Retrieve headers]

Deze module retourneert elke header (naam en waarde) van de opgegeven HTTP-module in een aparte bundel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Selecteer de module waarvan u kopteksten wilt terugwinnen.</p> </td> 
  </tr> 
 </tbody> 
</table>

## JSON-webtokens genereren (JWT)

Het is mogelijk om een token JWT te genereren met behulp van ingebouwde functies:

Koptekst:

![](assets/jwt-header-350x19.png)

Code voor kopiëren en plakken:

```
{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Payload:

![](assets/jwt-payload-350x17.png)

Code voor kopiëren en plakken:

```
{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

Token:

![](assets/jwt-token-350x15.png)

Code voor kopiëren en plakken:

```
{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```
