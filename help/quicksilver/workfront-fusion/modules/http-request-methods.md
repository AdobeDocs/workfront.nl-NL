---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Methoden voor HTTP-aanvragen in  [!DNL Adobe Workfront Fusion]
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Methoden voor HTTP-aanvragen in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ HTTP- verzoekmethodes ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/http-request-methods.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

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

## HTTP-methoden

Gebruik een van de volgende HTTP-methoden.

* **[!UICONTROL GET]**: haalt gegevens op van een webserver op basis van uw parameters. [!UICONTROL GET] vraagt om een representatie van de opgegeven bron en ontvangt een [!UICONTROL 200 OK] -antwoordbericht met de aangevraagde inhoud als dit gelukt is.
* **[!UICONTROL POST]**: verzendt gegevens naar een webserver op basis van uw parameters. [!UICONTROL POST] -aanvragen bevatten handelingen zoals het uploaden van een bestand. Meerdere [!UICONTROL POST]&#39;s kunnen resulteren in een ander resultaat dan één [!UICONTROL POST] . Wees daarom voorzichtig met het onbedoeld verzenden van meerdere [!UICONTROL POST] s. Als een [!UICONTROL POST] is gelukt, ontvangt u een [!UICONTROL 200 OK] antwoordbericht.
* **[!UICONTROL PUT]**: verzendt gegevens naar een locatie op de webserver op basis van uw parameters. [!UICONTROL PUT] -aanvragen bevatten handelingen zoals het uploaden van een bestand. Het verschil tussen a [!UICONTROL PUT] en [!UICONTROL POST] is dat PUT epidemisch is, wat betekent dat het resultaat van één succesvolle [!UICONTROL PUT] hetzelfde is als veel identieke [!UICONTROL PUT] s. Als een PUT succesvol is, ontvangt u een 200 reactiebericht (gewoonlijk 201 of 204).
* **[!UICONTROL PATCH]**: (Niet beschikbaar voor sommige API-callmodules) Hiermee past u op basis van uw parameters gedeeltelijke wijzigingen toe op een bron op een webserver. [!UICONTROL PATCH] is niet dekkend, wat betekent dat het resultaat van meerdere [!UICONTROL PATCH] &#39;&#39;s onbedoelde gevolgen kan hebben. Als een [!UICONTROL PATCH] is gelukt, ontvangt u een 200-antwoordbericht (meestal 204).
* **[!UICONTROL DELETE]**: verwijdert de opgegeven bron van de webserver op basis van uw parameters (als de bron bestaat). Als een [!UICONTROL DELETE] is gelukt, ontvangt u een 200 OK-antwoordbericht.
