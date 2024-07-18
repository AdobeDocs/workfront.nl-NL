---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Een webhaak ontvangen van een webservice
description: Als een Webdienst momenteel niet als app in  [!DNL Adobe Workfront Fusion] wordt uitgevoerd, maar het steunt het verzenden van webhooks, kunt u de dienst aan een scenario toevoegen gebruikend de module van de Webhaak van de Douane als onmiddellijke trekker.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Een webhaak ontvangen van een webservice

Als een webservice momenteel niet als een app in [!DNL Adobe Workfront Fusion] is geïmplementeerd, maar het verzenden van webhooks ondersteunt, kunt u de service aan een scenario toevoegen met de module Aangepaste webhaak als instant trigger.

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
   <p>Huidige productvereiste: als u het [!UICONTROL Select] - of [!UICONTROL Prime] [!DNL Adobe Workfront] -abonnement hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Een webhaak ontvangen

1. Voeg de module **[!UICONTROL Webhooks]>[!UICONTROL Custom webhook]** aan uw scenario toe.
1. Klik op **[!UICONTROL Add]** , typ een **[!UICONTROL Webhook name]** in het vak dat wordt weergegeven en klik op **[!UICONTROL Save]** .

1. Klik op **[!UICONTROL Copy address to clipboard]** en vervolgens op **[!UICONTROL OK]** .

1. Meld u aan bij de webservice en voer de volgende handelingen uit:

   1. Maak een webhaak in het gebied [!UICONTROL Settings] voor de webservice.
   1. Plak het adres dat u in stap 3 naar het klembord hebt gekopieerd.
   1. Selecteer de gebeurtenis die de webhaak activeert.

1. Geef in het [!DNL Workfront Fusion] -scenario de gebeurtenis of gebeurtenissen op die u de module [!UICONTROL Custom webhook] wilt activeren.
1. Voer het scenario uit.

   Wanneer de gebeurtenis of gebeurtenissen plaatsvinden, wordt de module [!UICONTROL Custom webhook] geactiveerd en wordt het scenario uitgevoerd.
