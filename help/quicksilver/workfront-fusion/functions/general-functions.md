---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Algemene functies in Adobe Workfront Fusion
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# Algemene functies in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ Algemene functies ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/general-functions.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

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

Retourneert `value1` als de expressie wordt geëvalueerd op true; anders wordt de `value2` geretourneerd.

Als u een if-instructie wilt maken die alleen een waarde retourneert wanneer twee of meer expressies worden geëvalueerd op true, gebruikt u het trefwoord `and` .

Gebruik de operatoren `and` en `or` om `if` -instructies te combineren.

![ en exploitant ](/help/quicksilver/workfront-fusion/functions/assets/and-in-if-statement.png)

>[!INFO]
>
>**Voorbeelden:**
>
>* `if( 1 = 1 ; A ; B )`
>
>    Retourneert A
>
>* `if( 1 = 2 ; A ; B )`
>
>   Retourneert B
>
>* `if( 1 = 2 and 1 = 2 ; A ; B )`
>
>    Retourneert B
>   

## [!UICONTROL ifempty (value1; value2)]

Retourneert de waarde `value1` als deze waarde niet leeg is; anders wordt de waarde `value2` geretourneerd.

>[!INFO]
>
>**Voorbeelden:**
>
>* `ifempty(` `A` `;` `B`
>
>   Retourneert A
>
>* `ifempty(` `unknown` `;` `B`
>
>   Retourneert B
>
>* `ifempty(` `""` `;` `B`
>
>   Retourneert B

## [!UICONTROL switch (expression; value1; result1; [value2; result2; ...]; [else])]

Evalueert één waarde (de expressie genoemd) met een lijst van waarden; retourneert het resultaat dat overeenkomt met de eerste overeenkomende waarde. Als u een `else` -waarde wilt opnemen, voegt u deze waarde toe na de laatste expressie of waarde.

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
>   Retourneert 4
>   
>   In deze functie is 4 de waarde die moet worden geretourneerd als er geen expressies van toepassing zijn (de `else` waarde).

## [!UICONTROL omit(object; key1; [key2; ...])]

Hiermee worden de opgegeven sleutels van het object weggelaten en wordt de rest geretourneerd.

>[!INFO]
>
>**Voorbeeld:**
>
>`omit(` Gebruiker `;` password `)`
>
>Retourneert een verzameling van de gegevens van de gebruiker, exclusief het wachtwoord.

## [!UICONTROL pick(object; key1; [key2; ...])]

Hiermee worden alleen de opgegeven toetsen van het object geselecteerd.

>[!INFO]
>
>**Voorbeeld:**
>
>`pick(` E-mail met het `;` wachtwoord `;` van de gebruiker `)`
>
>Retourneert alleen een verzameling van het wachtwoord en het e-mailadres van de gebruiker.

## mergeCollections(collection1; collection2)

Voegt twee verzamelingen samen door hun sleutel-waarde paren te combineren. Als beide verzamelingen dezelfde sleutel bevatten, overschrijft de waarde van de tweede verzameling die waarde van de eerste verzameling.

