---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Een array toewijzen in [!DNL Adobe] Workfront Fusion
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
>**Voorbeeld:** De [!UICONTROL Watch emails] retourneert een array met bijlagen voor elke e-mail. Elke bijlage vertegenwoordigt een verzameling die een naam, inhoud, grootte enzovoort kan bevatten.

Zie voor meer informatie [Gegevenstypen item in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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

## Een array toewijzen

1. Klik op de knop in het doelveld.

   >[!INFO]
   >
   >  **Voorbeeld:** In het bovenstaande voorbeeld klikt u op de knop [!UICONTROL Add an attachment] voor een e-mailbericht.
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. Voer het item in het vak dat wordt weergegeven.

   In het deelvenster kunt u velden op dezelfde manier toewijzen als bij elk ander type item. Als u niet elk punt afzonderlijk wilt invullen, maar een andere serie in het doelgebied wilt in kaart brengen, gebruik [!UICONTROL Map] knop. In dit geval moet u ervoor zorgen dat beide arrays (de bronarray en de doelarray) dezelfde structuur hebben.

   U kunt elk gewenst aantal items aan een array toevoegen.

U kunt een array in afzonderlijke bundels verdelen met behulp van een iterator. Zie voor meer informatie [[!UICONTROL Iterator] module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
