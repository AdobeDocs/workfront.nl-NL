---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Wijs een serie in  [!DNL Adobe]  de Fusie van Workfront toe
description: U kunt een array toewijzen aan een moduleveld in Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Een array toewijzen in [!DNL Adobe Workfront Fusion]

Een array is een speciaal type item dat het volgende kan bevatten:

* Een of meer tekstwaarden (eenvoudige array)
* Een of meer verzamelingen van hetzelfde type (complexe array)

>[!INFO]
>
>**Voorbeeld:** de [!UICONTROL Watch emails] module keert een serie van gehechtheid voor elke e-mail terug. Elke bijlage vertegenwoordigt een verzameling die een naam, inhoud, grootte enzovoort kan bevatten.

Voor meer informatie, zie {de gegevenstypes van 0} Punt in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).[

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

## Een array toewijzen

1. Klik op de knop in het doelveld.

   >[!INFO]
   >
   >  **Voorbeeld:** Voor het bovenstaande voorbeeld, zou u de [!UICONTROL Add an attachment] knoop voor een e-mail klikken.
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. Voer het item in het vak dat wordt weergegeven.

   In het deelvenster kunt u velden op dezelfde manier toewijzen als bij elk ander type item. Als u niet elk item afzonderlijk wilt invullen, maar een andere array wilt toewijzen aan het doelveld, gebruikt u de knop [!UICONTROL Map] . In dit geval moet u ervoor zorgen dat beide arrays (de bronarray en de doelarray) dezelfde structuur hebben.

   U kunt elk gewenst aantal items aan een array toevoegen.

U kunt een array in afzonderlijke bundels verdelen met behulp van een iterator. Zie [[!UICONTROL Iterator] module in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) voor meer informatie.
