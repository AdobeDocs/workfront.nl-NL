---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: http-modules
title: Wederzijdse TLS gebruiken in HTTP-modules in Adobe Workfront Fusion
description: U kunt Wederzijdse TLS gebruiken in uw Adobe Workfront Fusion HTTP-modules, zodat beide zijden van de informatietransactie de identiteit van de ander kunnen verifiëren.
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
source-git-commit: d2baef04d0a02a2a73dbe1dd4c46cb49a75a0d5e
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---

# Gebruik wederzijds TLS in HTTP-modules in [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>Adobe Workfront Fusion vereist een [!DNL Adobe Workfront Fusion] naast een Adobe Workfront-licentie.

## Overzicht van wederzijdse TLS

Wanneer u gegevens via internet verzendt, is het belangrijk ervoor te zorgen dat deze naar de juiste locatie worden verzonden en dat alleen de beoogde ontvanger deze kan lezen. Als TLS is ingeschakeld, gebruikt de client (computer die om informatie vraagt) certificaten om de identiteit van de server (computer die informatie verschaft) te verifiëren. Hierdoor worden veilige HTTP-verbindingen gemaakt.

Met wederzijdse TLS kan deze identiteitsbevestiging op beide manieren verlopen. Wanneer de server zijn certificaat verzendt om zijn identiteit aan de cliënt te verifiëren, vraagt het ook het certificaat van de cliënt. Dit zorgt ervoor dat de server geen informatie naar een plaats of een gebruiker verzendt die het zou misbruiken.

>[!INFO]
>
>**Voorbeeld:**
>
>* **TLS**: Wanneer iemand &quot;MyGreatBank.com&quot; in een browser typt, willen ze er zeker van zijn dat ze naar Mijn Grote Bank gaan, niet een website die hun bankgegevens kan misbruiken of verkopen. Ze willen ook zeker weten dat hun bankrekeninggegevens gecodeerd zijn.
>
>   Wanneer de browser (de client) verbinding maakt met MyGreatBank.com (de server), vereist TLS een certificaat van MyGreatBank.com om de identiteit ervan te verifiëren. Het certificaat wordt geleverd door een certificeringsinstantie, zoals [!DNL DigiCert] of [!DNL Thawte]. Omdat de browser de certificeringsinstantie vertrouwt, is de verbinding mogelijk.
>
>* **Wederzijdse TLS**: MySoftware.com is een softwareclient die informatie nodig heeft van de MyGreatBank.com API. MyGreatBank staat alleen vertrouwde clients toe verbinding te maken met hun servers. Naast de regelmatige controle van het TLS op de identiteit van MyGreatBank.com, verifieert het proces van de TLS/Certificate Authority dus ook het verzoek van MySoftware.com.

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
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
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

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

&#42;&#42;Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Uw [!DNL Workfront Fusion] public certificate


Wanneer u verbinding maakt met een webservice met een HTTP-aanvraag, vereist de webservice meestal een [!DNL Workfront Fusion] openbare keuringsverklaring. Hierdoor kan de webservice het certificaat dat in de HTTP-aanvraag wordt aangeboden, vergelijken met het certificaat in het bestand, zodat u zeker weet dat het certificaat zich op de lijst van gewenste personen van de webservice bevindt.

Voor instructies over het uploaden van de [!DNL Adobe Workfront Fusion] raadpleeg de documentatie van de webservice voor een openbaar certificaat voor een webservice.

>[!NOTE]
>
>U moet mogelijk andere informatie opgeven naast het certificaat. Raadpleeg de API-documentatie van de webservice voor informatie over wat een webservice nodig heeft.

U kunt de volgende koppelingen gebruiken om de openbare certificaten van Workfront Fusion te downloaden:

### Certificaten voor 23 april 2023-7 mei 2024

>[!IMPORTANT]
>
>* Deze [!DNL Workfront Fusion] openbare certificaten verlopen op 7 mei 2025. Nadat uw certificaat is verlopen, moet u een nieuw certificaat uploaden naar de webservice. We raden u aan:
>
>   * Noteer de vervaldatum en stel een herinnering voor uzelf in om het certificaat te uploaden naar uw webservice.
>   * Bladwijzer deze pagina om de nieuwe certificaten gemakkelijk te vinden.
>
>* Dit zijn mTLS-certificaten die geen jokertekens bevatten.

* [Downloaden [!DNL Workfront Fusion] Certificaat 2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-us-mtls-certificate.pem)
* [Downloaden [!DNL Workfront Fusion] EU-certificaat 2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-eu-mtls-certificate.pem)

  Voor gebruik in de EU

<!--

### Certificates for November 14, 2022 - July 15, 2023

>[!IMPORTANT]
>
>* These [!DNL Workfront Fusion] public certificates expire on July 15, 2023.
>* These are wildcard mTLS certificates.

* [Download [!DNL Workfront Fusion] Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [Download [!DNL Workfront Fusion] EU Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   For use in the EU 

   -->

## Wederzijdse TLS inschakelen in [!DNL Workfront Fusion] HTTP-modules

Alles [!DNL Workfront Fusion] [!UICONTROL HTTP] aanvraagmodules hebben de optie om wederzijdse TLS in te schakelen.

Wederzijdse TLS inschakelen in een [!UICONTROL HTTP] aanvraagmodule:

1. Een [!UICONTROL HTTP] verzoek module aan uw scenario.
1. Beginnen met het configureren van de module.

   Voor instructies over het configureren van een [!UICONTROL HTTP] verzoek module, zie het aangewezen artikel onder [[!UICONTROL HTTP] modules](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. Inschakelen **[!UICONTROL Show advanced settings]** onder aan de module.
1. Inschakelen **[!UICONTROL Use Mutual TLS]**.
