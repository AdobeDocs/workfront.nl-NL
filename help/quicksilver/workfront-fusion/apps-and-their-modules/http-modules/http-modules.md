---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: HTTP &gt; Overige modules
description: De [!DNL Adobe Workfront Fusion] De HTTP-toepassing biedt verschillende modules voor communicatie op basis van het HTTP-protocol (Hypertext Transfer Protocol). HTTP is de stichting van gegevensmededeling voor het World Wide Web. U kunt de modules gebruiken om Web-pagina's en dossiers te downloaden, Web-haken en API eindpunten te roepen, etc.
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---

# HTTP > Overige modules

>[!NOTE]
>
>[!UICONTROL Adobe Workfront Fusion] vereist een [!UICONTROL Adobe Workfront Fusion] naast een [!UICONTROL Adobe Workfront] licentie.

De [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] app biedt verschillende modules voor communicatie op basis van het HTTP-protocol (Hypertext Transfer Protocol). HTTP is de stichting van gegevensmededeling voor het World Wide Web. U kunt de modules gebruiken om Web-pagina&#39;s en dossiers te downloaden, Web-haken en API eindpunten te roepen, etc.

De juiste keuze van de module is afhankelijk van het verificatie-/verificatiemechanisme waartoe de bron waartoe u toegang wilt hebben, behoort. Hieronder volgen voorbeelden van modules

* Voer een verzoek in:universele module hoofdzakelijk bedoeld voor middelen die geen enkele vorm van authentificatie/vergunning gebruiken
* Voer een verzoek van de Auth van de Basis:voor middelen die [!DNL HTTP] Basisverificatie (BA)
* Voer een OAuth 2.0 verzoek in: voor middelen die OAuth 2.0 vergunningsprotocol gebruiken
* Voer een verzoek van de Auteur van het Certificaat van de Cliënt in: voor middelen die vergunningsprotocol gebruiken dat een cliënt-zijcertificaat vereist.
* Een aanvraag voor een API-sleutelautorisatie indienen: voor bronnen die gebruik maken van API-sleutels voor autorisatie.

## Aanvraagmodules

Zie de volgende artikelen voor specifieke instructies van de verzoekmodule:

* [[!UICONTROL HTTP] >[!UICONTROL Make a request] module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Make a Basic Authorization request] module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL Make an OAuth 2.0 request] module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL Make a Client Certificate Authorization request] module](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
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
   <td> <p>Voer de URL die u wilt omzetten in of wijs deze toe, zoals een [!DNL bit.ly] URL.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method] </td> 
   <td> <p>Selecteer of u de [!UICONTROL HEAD] of de [!UICONTROL GET] methode.</p> </td> 
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
