---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Arrayfuncties in Adobe Workfront Fusion
description: De volgende arrayfuncties zijn beschikbaar in het Adobe Workfront Fusion-toewijzingspaneel.
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 0%

---

# Arrayfuncties in Adobe Workfront Fusion

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

## [!UICONTROL add (array; value1; value2; ...)]

Voegt waarden die in parameters zijn opgegeven toe aan een array en retourneert die array.

## [!UICONTROL contains (array; value)]

Controleert of een array de waarde bevat.

## [!UICONTROL distinct (array; [key])]

Hiermee worden duplicaten uit een array verwijderd. Gebruik de &quot;[!UICONTROL key]&quot; argument om eigenschappen binnen complexe objecten te benaderen. Gebruik puntnotatie voor toegang tot geneste eigenschappen. Het eerste item in een array is index 1.

>[!INFO]
>
>**Voorbeeld:** `distinct(Contacts[];name)`
>
>Verwijdert duplicaten binnen een array van contactpersonen door de eigenschap &quot;name&quot; te vergelijken

## [!UICONTROL flatten (array)]

Hiermee wordt een nieuwe array gemaakt waarin alle elementen van de subarray recursief tot de opgegeven diepte zijn samengevoegd.


## [!UICONTROL join (array; separator)]

Hiermee worden alle items van een array samengevoegd in een tekenreeks, waarbij het opgegeven scheidingsteken tussen elk item wordt gebruikt.

## [!UICONTROL keys (object)]

Retourneert een array van de eigenschappen van een bepaald object of een bepaalde array.

## [!UICONTROL length (array)]

Retourneert het aantal items in een array.

## [!UICONTROL map (complex array; key;[key for filtering];[possible values for filtering])]

Retourneert een primitieve array met waarden van een complexe array. Deze functie staat het filtreren waarden toe. Gebruik namen van onbewerkte variabelen voor sleutels.

>[!INFO]
>
>**Voorbeelden:**
>
>* `map(Emails[];email)`
>
>  Retourneert een primitieve array met e-mails
>
>* `map(Emails[];email;label;work;home)`
>
>  Retourneert een primitieve array met e-mails met een label dat gelijk is aan werk of privé

Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)


## [!UICONTROL merge (array1; array2; ...)]

Voegt een of meer arrays samen tot één array.

## [!UICONTROL remove (array; value1; value2; ...)]

Verwijdert waarden die zijn opgegeven in de parameters van een array. Deze functie is alleen effectief op primitieve arrays met tekst of getallen.

## [!UICONTROL reverse (array)]

Het eerste element van de array wordt het laatste element, het tweede het op een na laatste element enzovoort.

## [!UICONTROL slice (array; start; [end])]

Retourneert een nieuwe array die alleen geselecteerde items bevat.

## [!UICONTROL sort (array; [order]; [key])]

Hiermee worden waarden van een array gesorteerd. De geldige waarden van de `order` parameter zijn:

* `asc`

  (standaard) - oplopende volgorde: 1, 2, 3, ... voor type Number. A, B, C, a, b, c, ... voor tekst

* `desc`

  aflopende volgorde: ..., 3, 2, 1 voor type Number. ..., c, b, a, C, B, A voor tekst.

* `asc ci`

  hoofdlettergevoelig, oplopende volgorde: A, a, B, b, C, c, ... voor tekst.

* `desc ci`

  niet-hoofdlettergevoelig, aflopende volgorde: ..., C, c, B, b, A, a voor tekst.

Gebruik de `key` parameter voor toegang tot eigenschappen in complexe objecten.

Gebruik namen van onbewerkte variabelen voor sleutels.

Gebruik puntnotatie voor toegang tot geneste eigenschappen.

Het eerste item in een array is index 1.

>[!INFO]
>
>**Voorbeelden:**
>
>* `sort(Contacts[];name)`
>
>    Hiermee wordt een array van contactpersonen gesorteerd op de eigenschap &quot;name&quot; in oplopende volgorde
>
>* `sort(Contacts[];desc;name)`
>
>   Hiermee wordt een array van contactpersonen gesorteerd op de eigenschap &quot;name&quot; in aflopende volgorde
>
>* `sort(Contacts[];asc ci;name)`
>
>    Hiermee wordt een array van contactpersonen gesorteerd op de eigenschap &quot;name&quot; in niet-hoofdlettergevoelige oplopende volgorde
>
>* `sort(Emails[];sender.name)`
>
>    Hiermee wordt een array met e-mailberichten gesorteerd op de eigenschap &quot;sender.name&quot;

## [!UICONTROL arrayDifference [array1, array2, mode]]

Geeft het verschil tussen twee arrays.

Voer een van de volgende waarden in voor de `mode` parameter.

* `classic`: Hiermee wordt een nieuwe array geretourneerd die alle elementen bevat van `array1` die niet bestaan in `array2`.

* `symmetric`: Retourneert een array met elementen die niet hetzelfde zijn voor beide arrays.

  Met andere woorden, de functie retourneert een array die alle elementen van `array1` die niet bestaan in `array2`en alle elementen van `array2` die niet bestaan in `array1`.

  >[!INFO]
  >
  >**Voorbeelden:**
  >
  >Op basis van de volgende arrays:
  >
  >```
  >myArray = [1,2,3,4,5]
  >```
  >
  >```
  >yourArray = [3,4,5,6,7]
  >```
  >
  >* `arrayDifference [myArray, yourArray, classic]`
  >
  >    Retourneert `[1,2]`
  >
  >* `arrayDifference [yourArray, myArray, classic]`
  >
  >    Retourneert `[6,7]`
  >
  >* `arrayDifference [myArray, yourArray, symmetric]`
  >
  >    Retourneert `[1,2,6,7]`
