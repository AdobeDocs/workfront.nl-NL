---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JWT-modules
description: De [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] app biedt een module die JWT-tokens maakt op basis van het opgegeven algoritme.
author: Becky
feature: Workfront Fusion
source-git-commit: d4f6f5d4919120e37fb94a23ac834a3896019584
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# [!UICONTROL JWT] module

De [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] app biedt een module die JWT-tokens maakt op basis van het opgegeven algoritme.

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] of hoger</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige vergunningsvereiste: Neen [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor arbeidsautomatisering en -integratie],  [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u beschikt over [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Vereisten voor verouderd product: uw organisatie moet het product kopen [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## JWT-module en de bijbehorende velden

### JWT genereren

Deze module produceert JWT die op het geselecteerde algoritme wordt gebaseerd.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Algorithm]</td> 
   <td> <p>Selecteer het algoritme waarmee u de JWT wilt genereren.</p> <ul>
   <li><b>HS256</b>: HMAC met SHA-256-hash-algoritme</li>
   <li><b>HS384</b>: HMAC met SHA-384-hash-algoritme</li>
   <li><b>HS512</b>: HMAC met SHA-512-hash-algoritme</li>
   <li><b>RS256</b>: RSASSA-PKCS1-v1_5 met SHA-256-hash-algoritme</li>
   <li><b>RS384</b>: RSASSA-PKCS1-v1_5 met SHA-384-hash-algoritme</li>
   <li><b>RS512</b>: RSASSA-PKCS1-v1_5 met SHA-512-hash-algoritme</li>
   <li><b>PS256</b>: RSASSA-PSS met SHA-256-hash-algoritme (alleen knooppunt ^6.12.0 OF &gt;=8.0.0)</li>
   <li><b>PS384</b>: RSASSA-PSS met SHA-384-hash-algoritme (alleen knooppunt ^6.12.0 OF &gt;=8.0.0)</li>
   <li><b>PS512</b>: RSASSA-PSS met SHA-512-hash-algoritme (alleen knooppunt ^6.12.0 OF &gt;=8.0.0)</li>
   <li><b>ES256</b>: ECDSA gebruikt P-256 curve en SHA-256 hash algoritme</li>
   <li><b>ES384</b>: ECDSA gebruikt P-384 curve en SHA-384 hash algoritme</li>
   <li><b>ES512</b>: ECDSA met P-521-curve en SHA-512-hash-algoritme</li>
   </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Payload] </td> 
   <td> <p>Voor elk ladingitem dat u wilt toevoegen, klikt u <b>Item toevoegen</b> en voer de sleutel en waarde van het item in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Options] </td> 
   <td> <p>Klik voor elk optie-item dat u wilt toevoegen op <b>Item toevoegen</b> en voer de sleutel en waarde van het item in.</p> <p>De volgende toetsen zijn beschikbaar:
   <ul>
   <li><b>algoritme</b>: (standaard: RS256)</li>
   <li><b>expiredIn</b>: Wordt uitgedrukt in seconden of een tekenreeks die een tijdbereik beschrijft (bijvoorbeeld 2 dagen, 10u, 7d). Een numerieke waarde wordt geïnterpreteerd als een aantal seconden. Als u een tekenreeks gebruikt, moet u de tijdseenheden (dagen, uren, enz.) opgeven, anders wordt de eenheid voor milliseconden standaard gebruikt (120 is gelijk aan 120 ms).</li>
   <li><b>notBefore</b>: Wordt uitgedrukt in seconden of een tekenreeks die een tijdbereik beschrijft (bijvoorbeeld 2 dagen, 10u, 7d). Een numerieke waarde wordt geïnterpreteerd als een aantal seconden. Als u een tekenreeks gebruikt, moet u de tijdseenheden (dagen, uren, enz.) opgeven, anders wordt de eenheid voor milliseconden standaard gebruikt (120 is gelijk aan 120 ms).
</li>
   <li><b>publiek</b></li>
   <li><b>uitgever</b></li>
   <li><b>jwtid</b></li>
   <li><b>onderwerp</b></li>
   <li><b>noTimestamp</b></li>
   <li><b>header</b></li>
   <li><b>sleutelid</b></li>
   <li><b>mutatePayload</b>: if <code>true</code>, wijzigt de functie sign het ladingsvoorwerp direct. Dit is handig als u een ruwe verwijzing naar de lading nodig hebt nadat de eisen op het zijn toegepast maar alvorens het in een teken is gecodeerd.</li>
   <li><b>allowInsecureKeySizes</b>: if <code>true</code>, maakt het gebruik van persoonlijke sleutels met een modulus lager dan 2048 voor RSA mogelijk.</li>
   <li><b>allowInvalidAsymmetricKeyTypes</b>: if <code>true</code>, staat asymmetrische sleutels toe die niet het gespecificeerde algoritme aanpassen. Deze optie is alleen bedoeld voor achterwaartse compatibiliteit en moet worden vermeden.</li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

