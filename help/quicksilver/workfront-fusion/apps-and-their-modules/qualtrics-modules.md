---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Qualtriciteitsmodules
description: In een  [!DNL Adobe Workfront Fusion]  scenario, kunt u werkschema's automatiseren die Qualtrics gebruiken, evenals het met veelvoudige derdetoepassingen en de diensten verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 146802cd-b863-4c93-b767-50e05892c4de
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Qualtriciteitsmodules

In een [!DNL Adobe Workfront Fusion] -scenario kunt u workflows automatiseren die [!DNL Qualtrics] gebruiken en deze koppelen aan meerdere toepassingen en services van derden.

Als u instructies bij het creëren van een scenario nodig hebt, zie [ een scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) creëren.

Voor informatie over modules, zie [ Modules in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het abonnement [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Als u [!DNL Qualtrics] -modules wilt gebruiken, moet u een [!UICONTROL Qualtrics] -account hebben.

## API-informatie voor kwaliteitscontrole

De schakelaar van Qualtrics gebruikt het volgende:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td> https://&lbrace;&lbrace;connection.dataCenterCode&rbrace;&rbrace;.qualtrics.com/API/v3 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-versie</td> 
   <td> v3 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-tag</td> 
   <td>v1.1.1</td> 
  </tr>
 </tbody> 
 </table>

## Verbinding maken [!DNL Qualtrics] met [!DNL Workfront Fusion]

U kunt rechtstreeks vanuit een [!UICONTROL Qualtrics] -module verbinding maken met uw [!DNL Qualtrics] -account.

1. Klik in een willekeurige [!UICONTROL Qualtrics] -module op **[!UICONTROL Add]** naast het [!UICONTROL Connection] -veld.
1. Voer de volgende gegevens in:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>Voer een naam in voor de nieuwe verbinding.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Data Center ID] </td> 
      <td>Gebruik de indeling <code>&lt;Data Center ID>.qualtrics.com</code> .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API Key]</td> 
      <td>Raadpleeg de documentatie van [!DNL Qualtrics] om de API-sleutel te zoeken.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Continue]** om de verbinding te maken en terug te gaan naar de module.

## [!DNL Qualtrics] modules en hun velden

De volgende modules zijn beschikbaar voor de [!DNL Qualtrics] schakelaar:

* [!UICONTROL Watch New Survey Response]
* [!UICONTROL Create a Directory Contact]
* [!UICONTROL Delete a Directory Contact]
* [!UICONTROL Get a Directory Contact]
* [!UICONTROL Update a Directory Contact]
* [!UICONTROL Create a New Survey Distribution via SMS]
* [!UICONTROL Distribute a Survey via Email]
* [!UICONTROL Make an API call]
* [!UICONTROL List Directory Contacts]
