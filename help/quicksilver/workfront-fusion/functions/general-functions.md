---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Algemene functies in Adobe Workfront Fusion
description: De volgende algemene functies zijn beschikbaar in het Adobe Workfront Fusion mapping panel.
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Algemene functies in [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL get (object or array; path)]

Retourneert het waardepad van een object of array. Gebruik puntnotatie om geneste objecten te openen. Het eerste item in een array is index 1.

>[!INFO]
>
>**Voorbeelden:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`

## [!UICONTROL if (expression; value1; value2)]

Hiermee wordt het `value1` als de expressie wordt geëvalueerd op true; anders retourneert het `value2`.

>[!INFO]
>
>**Voorbeelden:**
>
>* `if( 1 = 1 ; A ; B )`
>
>    Retourneert A
>
>* `if( = 2 ; A ; B )`
>
>   Retourneert B

## [!UICONTROL ifempty (value1; value2)]

Hiermee wordt het `value1` als deze waarde niet leeg is; anders retourneert het `value2`.

>[!INFO]
>
>**Voorbeelden:**
>
>* `ifempty(` `A` `;` `B` )
>
>   Retourneert A
>
>* `ifempty(` `unknown` `;` `B` )
>
>   Retourneert B
>
>* `ifempty(` `""` `;` `B` )
>
>   Retourneert B

## [!UICONTROL switch (expression; value1; result1; [value2; result2; ...]; [else])]

Evalueert één waarde (de expressie genoemd) ten opzichte van een lijst met waarden; retourneert het resultaat dat overeenkomt met de eerste overeenkomende waarde.

>[!INFO]
>
>**Voorbeelden:**
>
>* `switch( B ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   Retourneert 2
>
>* `switch( C ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   Retourneert 3
>
>* `switch( X ; A ; 1 ; B ; 2 ; C ; 3 ; 4 )`
>
>  Retourneert 4

## [!UICONTROL omit(object; key1; [key2; ...])]

Hiermee worden de opgegeven sleutels van het object weggelaten en wordt de rest geretourneerd.

>[!INFO]
>
>**Voorbeeld:**
>
>`omit(` Gebruiker `;` password `)`
>
>Retourneert een verzameling van de gegevens van de gebruiker, exclusief >het wachtwoord.

## [!UICONTROL pick(object; key1; [key2; ...])]

Hiermee worden alleen de opgegeven toetsen van het object geselecteerd.

>[!INFO]
>
>**Voorbeeld:**
>
>`pick(` Gebruiker `;` password `;` email `)`
>
>Retourneert alleen een verzameling van het wachtwoord en het e-mailadres van de gebruiker.
