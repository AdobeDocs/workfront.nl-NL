---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Een webhaak ontvangen van een webservice
description: Als een webservice momenteel niet is geïmplementeerd als een app in [!DNL Adobe Workfront Fusion], maar het steunt het verzenden van webhooks, kunt u de dienst aan een scenario toevoegen gebruikend de Webhaak van de Douane module als onmiddellijke trekker.
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Een webhaak ontvangen van een webservice

Als een webservice momenteel niet is geïmplementeerd als een app in [!DNL Adobe Workfront Fusion], maar het steunt het verzenden van webhooks, kunt u de dienst aan een scenario toevoegen gebruikend de Webhaak van de Douane module als onmiddellijke trekker.

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
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereisten: Als u de [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Oudere productvereisten: Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Een webhaak ontvangen

1. Voeg de **[!UICONTROL Webhooks]>[!UICONTROL Custom webhook]** aan uw scenario.
1. Klikken **[!UICONTROL Add]**, typt u een **[!UICONTROL Webhook name]** in het vak dat wordt weergegeven, klikt u op **[!UICONTROL Save]**.

1. Klikken **[!UICONTROL Copy address to clipboard]** en klik vervolgens op **[!UICONTROL OK]**.

1. Meld u aan bij de webservice en voer de volgende handelingen uit:

   1. In de [!UICONTROL Settings] voor de webservice maakt u een webhaak.
   1. Plak het adres dat u in stap 3 naar het klembord hebt gekopieerd.
   1. Selecteer de gebeurtenis die de webhaak activeert.

1. In de [!DNL Workfront Fusion] scenario, specificeer de gebeurtenis of de gebeurtenissen die u wilt teweegbrengen [!UICONTROL Custom webhook] module.
1. Voer het scenario uit.

   Wanneer de gebeurtenis of gebeurtenissen plaatsvinden, [!UICONTROL Custom webhook] de moduletrekkers en de scenario looppas.
