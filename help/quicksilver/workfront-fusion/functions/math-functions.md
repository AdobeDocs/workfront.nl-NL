---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Wiskundige functies in Adobe Workfront Fusion
description: De volgende rekenkundige functies zijn beschikbaar in het Adobe Workfront Fusion mapping panel.
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# Wiskundige functies in [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p><p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL average ([array of values]) average(value1; [value2], ...)]

Retourneert de gemiddelde waarde van de numerieke waarden in een specifieke array, of de gemiddelde waarde van numerieke waarden die afzonderlijk zijn ingevoerd.

## [!UICONTROL ceil (number)]

Retourneert het kleinste gehele getal dat groter dan of gelijk is aan een opgegeven getal.

>[!INFO]
>
>**Voorbeelden:**
>
>* `ceil(` `1.2` `)`
   >
   >   Retourneert 2
>
>* `ceil(` `4` `)`
   >
   >   Retourneert 4


## [!UICONTROL floor (number)]

Retourneert het grootste gehele getal dat kleiner dan of gelijk is aan een opgegeven getal.

>[!INFO]
>
>**Voorbeelden:**
>
>* `floor(` `1.2` `)`
   >
   >   Retourneert 1
>
>* `floor(` `1.9` `)`
   >
   >   Retourneert 1
>
>* `floor(` `4` `)`
   >
   >   Retourneert 4


## [!UICONTROL formatNumber (number; decimalPOINTS; [decimalSeparator]; [thousandsSeparator])]

Retourneert een getal in de gewenste notatie. Het decimale punt is standaard een komma (,) en het scheidingsteken voor duizendtallen is een punt (.).

>[!INFO]
>
>**Voorbeeld:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Retourneert 123.456.789.000

## [!UICONTROL max ([array of values]), max(value1;value2; ...)]

Retourneert het grootste getal in een opgegeven array of het grootste getal onder getallen die afzonderlijk zijn ingevoerd.

## [!UICONTROL min ([array of values]), min(value1; value2; ...)]

Retourneert het kleinste getal in een opgegeven array of het kleinste getal onder getallen die afzonderlijk zijn ingevoerd.

## [!UICONTROL parseNumber (number; decimal separator)]

Parseert een tekenreeks met een getal en retourneert het getal. Bijvoorbeeld, parseNumber(1 756,456;,)

## [!UICONTROL round (number)]

Rondt een numerieke waarde af op het dichtstbijzijnde gehele getal.

>[!INFO]
>
>**Voorbeelden:**
>
>* `round(` `1.2` `)`
   >
   >   Retourneert 1
>
>* `round(` `1.5` `)`
   >
   >   Retourneert 2
>
>* `round(` `1.7` `)`
   >
   >   Retourneert 2
> 
>* `round(` `2` `)`
   >
   >   Retourneert 2


## [!UICONTROL sum ([array of values]), sum(value1; value2; ...)]

Retourneert de som van de waarden in een opgegeven array of de som van de getallen die afzonderlijk zijn ingevoerd.
