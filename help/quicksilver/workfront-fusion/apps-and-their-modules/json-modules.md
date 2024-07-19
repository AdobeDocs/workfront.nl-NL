---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JSON-modules
description: De Adobe Workfront Fusion JSON-app biedt modules voor het verwerken van gegevens in JSON-indeling, zodat Adobe Workfront Fusion verder kan werken met de gegevensinhoud of nieuwe JSON-inhoud kan maken.
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 0%

---

# [!UICONTROL JSON] modules

De app [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] biedt modules voor het verwerken van gegevens in JSON-indeling, zodat [!DNL Adobe Workfront Fusion] verder kan werken met de gegevensinhoud of nieuwe JSON-inhoud kan maken.

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] of hoger</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor verouderde licentie: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie], [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>
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

## Parse JSON

* [ de structuur van Gegevens ](#data-structure)
* [Verzameling versus array](#collection-vs-array)

### Gegevensstructuur

De gegevensstructuur beschrijft hoe de JSON-gegevens zijn georganiseerd en maakt het mogelijk om afzonderlijke JSON-items toe te wijzen aan andere modules in uw scenario. Als u de gegevensstructuur niet aanbiedt, kunt u de module handmatig uitvoeren en bouwt [!DNL Workfront Fusion] de structuur op basis van de beschikbare JSON:

1. Voeg de module [!UICONTROL Parse JSON] toe aan een scenario.
1. Voer in het veld **[!UICONTROL JSON String]** de JSON in waarvan u een gegevensstructuur wilt maken.
1. Sluit nog geen andere modules aan op de module [!UICONTROL Parse JSON] . Omdat [!DNL Workfront Fusion] nog niet de structuur van de JSON-gegevens kent, is het nog niet mogelijk om gegevens van de module [!UICONTROL Parse JSON] toe te wijzen aan andere modules in uw scenario.
1. Voer het scenario handmatig uit. Hierdoor kan de module [!UICONTROL Parse JSON] de JSON-structuur identificeren vanuit de JSON die u hebt opgegeven.
1. U kunt nu de volgende modules verbinden. De punten van de Parse JSON module zijn nu beschikbaar voor afbeelding.

Zie [ Gegevensstructuren in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md) voor meer informatie.

### Verzameling versus array

Als het JSON-tekenreeksveld een verzameling `{ ... }` bevat, bestaat de uitvoer uit één bundel die de items van de verzameling bevat.

>[!INFO]
>
>**Voorbeeld:**
>
>```
>{
>       "name" : "Peter",
>
>    
>   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

Als het JSON-tekenreeksveld een array `[ ... ]` bevat, bestaat de uitvoer uit een reeks bundels. elke bundel bevat één element van de array.

>[!INFO]
>
>**Voorbeeld:**
>
>```
>[
>   {
>       "name" : "Peter",
>       "ID" : 1
>   },
>
>  
> {
>       "name" : "Mike",
>       "ID" : 2
>   }
>]
>```
>
>![](assets/json-array.png)

## [!UICONTROL JSON] modules en hun velden

Wanneer u [!DNL JSON] modules configureert, geeft [!DNL Workfront Fusion] de onderstaande velden weer. Daarnaast kunnen aanvullende JSON-velden worden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Voor meer informatie, zie [ informatie van de Kaart van één module aan een andere in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [ Geaggregeerd aan JSON ](#aggregate-to-json)
* [ zet JSON in XML ](#convert-json-to-xml) om
* [ ontleed JSON ](#parse-json)
* [ creeer JSON ](#create-json)
* [Transform JSON](#transform-json)

### [!UICONTROL Aggregate to JSON]

Deze aggregatormodule aggregeert de uitvoer van een vorige module naar JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source module] </td> 
   <td> <p>Selecteer de module die de gegevens uitvoert die u aan JSON wilt samenvoegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data structure]</td> 
   <td> <p>Selecteer de gegevensstructuur die u wilt gebruiken om JSON te maken. De gegevensstructuur bepaalt welke andere velden beschikbaar zijn in deze module. Voor meer informatie, zie <a href="#data-structure" class="MCXref xref"> de structuur van Gegevens </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Indentation]</td> 
   <td> <p> Selecteer of u de JSON wilt laten inspringen met tabs, twee spaties of vier spaties.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by]</td> 
   <td>Definieer een expressie waarop u de geaggregeerde uitvoer wilt groeperen. Deze expressie kan een of meer toegewezen items bevatten. De geaggregeerde gegevens worden vervolgens in groepen verdeeld op basis van de waarde van deze expressie. Elke groep voert als een afzonderlijke bundel met een sleutel (de geëvalueerde uitdrukking) en een waarde (de samengevoegde tekst) uit. U kunt de sleutel als filter in verdere modules gebruiken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Schakel deze optie in om het scenario te stoppen als er geen resultaten zijn.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convert JSON to XML]

Deze actiemodule converteert een JSON-tekenreeks naar XML.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON string] </td> 
   <td> <p>Typ of wijs de JSON toe die u in XML wilt omzetten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Parse JSON]

Deze actiemodule parseert een JSON-tekenreeks in een gegevensstructuur, waarmee u toegang hebt tot de gegevens in de JSON-tekenreeks.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data structure]</td> 
   <td> <p>Selecteer de gegevensstructuur die u wilt gebruiken om JSON te maken. Voor meer informatie, zie <a href="#data-structure" class="MCXref xref"> de structuur van Gegevens </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON string] </td> 
   <td> <p>Typ of wijs de JSON toe die u wilt parseren.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Create JSON]

Deze actiemodule maakt JSON op basis van een gegevensstructuur.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">Gegevensstructuur</td> 
   <td> <p>Selecteer de gegevensstructuur die u wilt gebruiken om JSON te maken. Voor meer informatie, zie <a href="#data-structure" class="MCXref xref"> de structuur van Gegevens </a> in dit artikel.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Transform JSON]

Deze actiemodule transformeert een object naar een json-tekenreeks.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object]</td> 
   <td> <p>Typ of wijs het object toe dat u in JSON wilt transformeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Gegevensrecords omzetten in JSON

>[!INFO]
>
>**Voorbeeld:** het volgende voorbeeld toont hoe te om gegevensverslagen van [!DNL Google Sheets] aan formaat te transformeren JSON:
>
>1. Plaats de module [!DNL Google Sheets] > [!UICONTROL Select rows] in uw scenario om de gegevens op te halen. Stel de module in om rijen op te halen uit de [!DNL Google] -spreadsheet. Plaats de &#x200B; **[!UICONTROL Maximum number of returned rows]** aan een klein aantal, maar groter dan één voor het testen doeleinden (Voorbeeld, drie). Voer de module [!DNL Google Sheets] uit door er met de rechtermuisknop op te klikken en &quot;**[!UICONTROL Run this module only]**&quot; te kiezen. Controleer de uitvoer van de module.
>
1. Sluit de module [!UICONTROL Array Aggregator] aan na de module [!DNL Google Sheets] . Kies in de installatie van de module de module [!DNL Google Sheets] in het veld **[!UICONTROL Source node]** . Laat de andere velden op dit moment ongewijzigd.
>
1. Verbind [!UICONTROL JSON] > [!UICONTROL Create JSON] module na de [!UICONTROL Array Aggregator] module. De opstelling van de module vereist een structuur van Gegevens die het formaat JSON beschrijft. Klik op **[!UICONTROL Add]** om de gegevensstructuurinstellingen te openen. De eenvoudigste manier om deze gegevensstructuur te maken, is deze automatisch te genereren op basis van een JSON-voorbeeld. Klik op **[!UICONTROL Generator]** en plak uw JSON-voorbeeld in het veld **[!UICONTROL Sample data]** :
>
**Voorbeeld:**
>   
>```
>{
>
>"books": [
>
>{
>
>"id": "ID",
>
>"title": "Title",
>
>"author": "Author"
>
>}
>
>]
>
>}
>```
>
1. Klik op **[!UICONTROL Save]**. Het veld [!UICONTROL Specification] in de gegevensstructuur bevat nu de gegenereerde structuur.
1. Wijzig de naam van de gegevensstructuur in een specifiekere naam en klik op **[!UICONTROL Save]** . Een veld dat overeenkomt met het kenmerk van de hoofdarray wordt als een toewijzingsveld weergegeven in de instellingen van de JSON-module.
>
1. Klik op de knop **[!UICONTROL Map]** naast het veld en wijs het `Array[]` -item vanuit de uitvoer van de Array-aggregator naar het veld toe.
>
1. Klik op **[!UICONTROL OK]** om de installatie van de module [!UICONTROL JSON] te sluiten.
>
1. Open de instelling van de module [!UICONTROL Array Aggregator] . Wijzig **[!UICONTROL Target structure]** van [!UICONTROL Custom] in het veld van de module [!UICONTROL JSON] dat overeenkomt met het kenmerk van de hoofdarray. Wijs items van de module [!DNL Google Sheets] toe aan de desbetreffende velden.
>
1. Klik op **[!UICONTROL OK]** om de installatie van de module [!UICONTROL Array Aggregator] te sluiten.
>
1. Voer het scenario uit.
>
De module [!UICONTROL JSON] geeft de juiste JSON-indeling.
>
1. Open de instelling van de module [!DNL Google Sheets] en verhoog het getal [!UICONTROL Maximum number of returned rows] om groter te zijn dan het aantal rijen in het werkblad om alle gegevens te verwerken.

## Problemen oplossen

### Kan geen gegevens toewijzen uit de module [!UICONTROL Parse JSON]

Controleer of de JSON-inhoud correct is toegewezen aan de module [!UICONTROL Parse JSON] en of de gegevensstructuur correct is gedefinieerd. Voor meer informatie, zie [ het Transformeren gegevensverslagen aan JSON ](#transforming-data-records-to-json) in dit artikel.

### De module mislukt wanneer voorwaardelijke instructies in JSON worden gebruikt

Wanneer u voorwaardelijke instructies gebruikt, zoals `if` in uw JSON, plaatst u de aanhalingstekens buiten de voorwaardelijke instructie.

>[!INFO]
>
**Voorbeeld:**
>
![](assets/quotes-in-json-350x120.png)
