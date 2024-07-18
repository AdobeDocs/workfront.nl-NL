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
source-git-commit: 033a9f4aa1f191e5e3cabd0c0f232128fa6bce5d
workflow-type: tm+mt
source-wordcount: '600'
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

## Functies

* [join](#join-array-separator)
* [length](#length-array)
* [toetsen](#keys-object)
* [segment](#slice-array-start-end)
* [samenvoegen](#merge-array1-array2)
* [contains](#contains-array-value)
* [remove](#remove-array-value1-value2)
* [toevoegen](#add-array-value1-value2)
* [map](#map-complex-array-keykey-for-filteringpossible-values-for-filtering)
* [ willekeurige volgorde ]
* [sorteren](#sort-array-order-key)
* [omkeren](#reverse-array)
* [afvlakken](#flatten-array)
* [onderscheiden](#distinct-array-key)
* [ toCollection ]
* [toArray](#toarray)
* [arrayDifference](#arraydifference-array1-array2-mode)
* [ deduplicate ]

### [!UICONTROL join (array; separator)]

Hiermee worden alle items van een array samengevoegd in een tekenreeks, waarbij het opgegeven scheidingsteken tussen elk item wordt gebruikt.

### [!UICONTROL length (array)]

Retourneert het aantal items in een array.

### [!UICONTROL keys (object)]

Retourneert een array van de eigenschappen van een bepaald object of een bepaalde array.

### [!UICONTROL slice (array; start; [end])]

Retourneert een nieuwe array die alleen geselecteerde items bevat.

### [!UICONTROL merge (array1; array2; ...)]

Voegt een of meer arrays samen tot één array.

### [!UICONTROL contains (array; value)]

Controleert of een array de waarde bevat.

### [!UICONTROL remove (array; value1; value2; ...)]

Verwijdert waarden die zijn opgegeven in de parameters van een array. Deze functie is alleen effectief op primitieve arrays met tekst of getallen.

### [!UICONTROL add (array; value1; value2; ...)]

Voegt waarden die in parameters zijn opgegeven toe aan een array en retourneert die array.

### [!UICONTROL map (complex array; key;[key for filtering];[possible values for filtering])]

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

Voor meer informatie, zie [ informatie van de Kaart van één module aan een andere in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)

### schudden

### [!UICONTROL sort (array; [order]; [key])]

Sorteert waarden van een array. De geldige waarden voor de parameter `order` zijn:

* `asc`

  (standaardwaarde) - oplopende volgorde: 1, 2, 3, ... voor het type Number. A, B, C, a, b, c... voor tekst

* `desc`

  Aflopende volgorde: ..., 3, 2, 1 voor type Number. ..., c, b, a, C, B, A voor tekst.

* `asc ci`

  niet-hoofdlettergevoelige oplopende volgorde: A, a, B, b, C, c, ... voor tekst.

* `desc ci`

  niet-hoofdlettergevoelige aflopende volgorde: ..., C, c, B, b, A, a voor tekst.

Gebruik de parameter `key` om eigenschappen binnen complexe objecten te benaderen.

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
>    Hiermee wordt een array van contactpersonen gesorteerd op de eigenschap &quot;name&quot; in hoofdlettergevoelige oplopende volgorde
>
>* `sort(Emails[];sender.name)`
>
>    Hiermee wordt een array met e-mailberichten gesorteerd op de eigenschap &quot;sender.name&quot;

### [!UICONTROL reverse (array)]

Het eerste element van de array wordt het laatste element, het tweede het op een na laatste element enzovoort.

### [!UICONTROL flatten (array)]

Hiermee wordt een nieuwe array gemaakt waarin alle elementen van de subarray recursief tot de opgegeven diepte zijn samengevoegd.

### [!UICONTROL distinct (array; [key])]

Hiermee worden duplicaten uit een array verwijderd. Gebruik het argument &quot;[!UICONTROL key]&quot; om toegang te krijgen tot eigenschappen binnen complexe objecten. Gebruik puntnotatie voor toegang tot geneste eigenschappen. Het eerste item in een array is index 1.

>[!INFO]
>
>**Voorbeeld:** `distinct(Contacts[];name)`
>
>Verwijdert duplicaten binnen een array van contactpersonen door de eigenschap &quot;name&quot; te vergelijken

### toCollection

### toArray

Deze functie converteert een verzameling naar een array van sleutelwaardeparen.

>[!INFO]
>
>**Voorbeelden:**
>
>Gezien de collectie
>
>`{ key1: "value1", key2: "value2:}`
>
>De functie
>
>`toArray({ key1: "value1", key2: "value2:})`
>
>Retourneert de array van sleutelwaardeparen
>
>`[{ key1: "value1"}, { key2: "value2"}]`

### [!UICONTROL arrayDifference [array1, array2, mode]]

Geeft het verschil tussen twee arrays.

Voer een van de volgende waarden in voor de parameter `mode` .

* `classic`: Geeft een nieuwe array met alle elementen van `array1` die niet bestaan in `array2` .

* `symmetric`: retourneert een array met elementen die niet voor beide arrays hetzelfde zijn.

  Met andere woorden, de functie retourneert een array die alle elementen van `array1` bevat die niet bestaan in `array2` , en alle elementen van `array2` die niet bestaan in `array1` .

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

### dedupliceren

## Trefwoorden

### emptyarray
