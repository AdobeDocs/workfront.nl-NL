---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Variabelen wissen in  [!DNL Adobe Workfront Fusion]
description: De volgende wiskundige variabelen zijn beschikbaar in het  [!DNL Adobe Workfront Fusion mapping]  paneel.
author: Becky
feature: Workfront Fusion
exl-id: 2fb561d2-0780-4fd6-87b3-5360a02df177
source-git-commit: c325e16ba0cde4cd48fc3e40358a9ea9ed310659
workflow-type: tm+mt
source-wordcount: '120'
ht-degree: 0%

---

# Variabelen wissen in [!DNL Adobe Workfront Fusion]

<!--Audited: 4/2024-->

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>  
   <td> <p>Alle</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td>  
   <td> <p>Nieuw: [!UICONTROL Standard]</p><p>of</p><p>Huidig: [!UICONTROL Work] of hoger</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td>  
   <td> 
   <p>Huidig: Geen [!DNL Workfront Fusion] vereiste licentie.</p> 
   <p>of</p> 
   <p>Verouderd: alle </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Product</td>  
   <td> 
   <p>Nieuw:</p> <ul><li>[!UICONTROL Select] of [!UICONTROL Prime] [!DNL Workfront] Plan: Uw organisatie moet het abonnement aanschaffen [!DNL Adobe Workfront Fusion] .</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Overzicht: [!DNL Workfront Fusion] is opgenomen.</li></ul> 
   <p>of</p> 
   <p>Huidig: Uw organisatie moet [!DNL Adobe Workfront Fusion] aanschaffen.</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## pi

Vertegenwoordigt het wiskundige symbool $\pi$.

## [!UICONTROL random]

Retourneert een pseudo-willekeurig getal met drijvende komma in het bereik [`0` , `1`] (inclusief `0` , maar niet `1` ).

Gebruik de volgende formule om een geheel pseudo-willekeurig aantal in de waaier [`min`, `max`] (met inbegrip van zowel `min` als `max`) te produceren:

![](assets/math-variable-random-350x61.png)

```
floor(random * (1.max - 1.min + 1)) + 1.min
```
