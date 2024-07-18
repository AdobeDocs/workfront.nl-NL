---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Kies waar een triggermodule begint in Adobe Workfront Fusion
description: Met bepaalde triggermodules kunt u de eerste bundel selecteren waaruit u het ophalen van bundels wilt laten starten.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Kies waar een triggermodule begint in [!DNL Adobe Workfront Fusion]

Met bepaalde triggermodules kunt u de eerste bundel selecteren waaruit u het ophalen van bundels wilt laten starten.

U kunt ook opgeven of u alle bundels wilt ophalen of alleen de bundels vanaf een bepaalde datum.

Voor meer informatie over trekkermodules, zie de sectie [ modules van de Trekker ](../../workfront-fusion/modules/module-types.md#triggers) in het artikel [ Types van modules ](../../workfront-fusion/modules/module-types.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] of hoger</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licentie**</td> 
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

## Kiezen waar een triggermodule begint

1. Sla een triggermodule op.

   of

   Verander de montages van de trekkermodule zoals die in [ worden beschreven vormen de montages van een module in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   of

   Klik het pictogram voor de trekkermodule in [!UICONTROL Scenario editor] met de rechtermuisknop aan, zoals die in [ wordt beschreven creeer een scenario in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Selecteer een optie in het vak **[!UICONTROL Choose where to start]** dat wordt weergegeven.

   ![](assets/choose-where-to-start-350x346.jpg)

   Welke opties worden weergegeven, is afhankelijk van de mogelijkheden van een bepaalde service. Zij kunnen het volgende omvatten:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL From now on] (standaard)</td>
            <td>Hiermee worden alle toegevoegde of bijgewerkte bundels (afhankelijk van de instellingen) opgehaald vanaf nu</td>
        </tr>
        <tr>
            <td>[!UICONTROL From after a specific date]</td>
            <td>Hiermee worden alle bundels opgehaald die na een opgegeven datum of tijd zijn toegevoegd of bijgewerkt (afhankelijk van de instellingen)</td>
        </tr>
        <tr>
            <td>[!UICONTROL With ID greater than or equal to a specific value]</td>
            <td>Hiermee worden alle bundels opgehaald met een id die groter is dan of gelijk is aan een opgegeven id</td> 
        </tr>
        <tr>
            <td>[!UICONTROL All bundles]</td>
            <td>Hiermee worden alle beschikbare bundels opgehaald</td>
        </tr>
        <tr>
            <td>[!UICONTROL Select the first bundle]</td>
            <td>Hiermee kunt u de eerste bundel selecteren waaruit het ophalen van bundels moet beginnen</td>
        </tr>
   </table>
