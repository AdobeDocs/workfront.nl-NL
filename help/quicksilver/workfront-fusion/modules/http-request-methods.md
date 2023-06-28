---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]
description: Wanneer u een API vraag in een module vormt, moet u het gebied voor de HTTP- verzoekmethode invullen.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]

Wanneer u een API vraag in een module vormt, moet u het gebied voor de HTTP- verzoekmethode invullen.

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

## HTTP-methoden

Gebruik een van de volgende HTTP-methoden.

* **[!UICONTROL GET]**: Haalt gegevens op van een webserver op basis van uw parameters. [!UICONTROL GET] vraagt om een vertegenwoordiging van het gespecificeerde middel, en ontvangt een [!UICONTROL 200 OK] antwoordbericht met de gevraagde inhoud indien succesvol.
* **[!UICONTROL POST]**: Hiermee verzendt u gegevens naar een webserver op basis van uw parameters. [!UICONTROL POST] verzoeken bevatten handelingen zoals het uploaden van een bestand. Meerdere [!UICONTROL POST]Het resultaat kan verschillen van het resultaat [!UICONTROL POST]Wees daarom voorzichtig met het onbedoeld verzenden van meerdere [!UICONTROL POST]s. Indien een [!UICONTROL POST] is gelukt, ontvangt u een [!UICONTROL 200 OK] antwoordbericht.
* **[!UICONTROL PUT]**: Hiermee verzendt u gegevens naar een locatie op de webserver op basis van uw parameters. [!UICONTROL PUT] verzoeken bevatten handelingen zoals het uploaden van een bestand. Het verschil tussen een [!UICONTROL PUT] en [!UICONTROL POST] is dat de PUT epidemisch is, wat betekent dat het resultaat van één succesvolle [!UICONTROL PUT] is hetzelfde als veel identieke [!UICONTROL PUT]s. Als een PUT succesvol is, ontvangt u een 200 reactiebericht (gewoonlijk 201 of 204).
* **[!UICONTROL PATCH]**: (Niet beschikbaar voor sommige API-vraagmodules) Hiermee past u op basis van uw parameters gedeeltelijke wijzigingen toe op een bron op een webserver. [!UICONTROL PATCH] is niet epidemisch, wat betekent dat het resultaat van meerdere [!UICONTROL PATCH]Dat kan onbedoelde gevolgen hebben. Indien een [!UICONTROL PATCH] Als dit is gelukt, ontvangt u een antwoordbericht van 200 (meestal 204).
* **[!UICONTROL DELETE]**: Verwijdert de opgegeven bron van de webserver op basis van uw parameters (als de bron bestaat). Indien een [!UICONTROL DELETE] Als dit is gelukt, ontvangt u een 200 OK-antwoordbericht.
