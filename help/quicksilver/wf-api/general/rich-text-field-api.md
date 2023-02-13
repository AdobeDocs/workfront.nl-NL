---
content-type: api
navigation-topic: general-api
title: Rijke tekstvelden in de Adobe Workfront API
description: Rijke tekstvelden in de Adobe Workfront API
author: John
feature: Workfront API
exl-id: 67fc34dc-0722-4419-8254-0371ad5abfc3
source-git-commit: 40698643b0fa530b38da465f3bc1e4d841fcc190
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---


# Rijke tekstvelden in de Adobe Workfront API

Sommige objecten in Adobe Workfront maken het mogelijk tekst met opmaak op te slaan. In de rijke tekst van de Workfront API wordt opgeslagen als JSON met behulp van het open-sourceframework Draft.js.

## Voorbeeld van overzicht

Een aangepast veld met opmaak in RTF-indeling wordt **Veld met RTF-tekst** en kan de volgende waarden hebben verbonden aan het:

![](assets/rich-text-example-350x158.png)

**Voorbeeld:** Een basisverzoek voor GET om de waarde van het aangepaste formulierveld op te halen **Veld met RTF-tekst**:

<!-- [Copy](javascript:void(0);) -->
<pre><OBJ Code><OBJ ID><OBJ Code><OBJ ID></pre>

**Voorbeeld:** Dit verzoek retourneert de waarde van **Veld met RTF-tekst** in JSON opgeslagen in de **parameterValue** **DE:Veld met RTF-tekst**

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

**Voorbeeld:** Dit is een geformatteerde versie van de reactie die in de figuur direct boven wordt getoond

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

## Blokken

De JSON-objecten die de RTF-inhoud opslaan, bestaan uit twee hoofdonderdelen: **blokken** en **entiteitMaps**.

Een blok is een JSON-object dat een enkele regel opgemaakte tekst vertegenwoordigt. Aangezien één aangepast veld meerdere tekstregels kan bevatten, heeft elke tekstregel een eigen blok en wordt elk blok vertegenwoordigd als een element in een bovenliggende array met de naam **blokken**.

**Voorbeeld:** Hier wordt elke tekstregel van een aangepast veld toegewezen aan een blokelement in de arrayblokken

![](assets/copy-of-rich-text-mapping-350x159.png)

Aangezien elk blokelement ook een JSON-object is, bestaat elk blok uit de elementen: **key**, **text**, **type**, **diepte**, **inlineStyleRanges**, **entiteitRanges**, en **data**. Elk van deze elementen werkt als volgt:

* **Sleutel** is de unieke id voor dat blok. De sleutel wordt gebruikt om een tekstregel via entityMaps in kaart te brengen. Meer informatie over entiteitskaarten vindt u in de sectie entityMaps van dit document.
* **Tekst** Dit is de regel tekstinhoud die wordt opgeslagen vanuit het aangepaste veld.
* **Type** beschrijft het type tekst dat wordt vertegenwoordigd. Een tekstregel die bijvoorbeeld in een blok wordt opgeslagen, kan onderdeel zijn van een lijst. Als die tekstregel onderdeel was van een niet-geordende lijst, zou het type als volgt worden gedefinieerd: ongeordend-list-item.
* Lijsten worden momenteel niet ondersteund, maar moeten binnenkort beschikbaar zijn.
* **Diepte** Deze parameter bepaalt de diepte van de lijn wanneer de lijn een genesteld deel van een geordende of ongeordende lijst is.
* **inlineStyleRanges** Is een array die de opmaaktypen beschrijft die zijn toegepast op de tekstregel die wordt vertegenwoordigd door het huidige blok.

**Voorbeeld:** Hier volgt een inlineStyleRanges-array die elke stijl op tekenniveau beschrijft. In dit geval: 9 tekens (lengte: 9) vanaf index 0 (verschuiving: 0) had de stijl **Vet** toegepast:

![](assets/copy-of-rich-text-mapping-2-350x136.png)

Wanneer meerdere typen opmaak zijn toegepast op één regel, worden stijlen toegewezen aan extra elementen in de** inlineStyleRanges**-array.

**Voorbeeld:** Zo ziet een blok eruit wanneer u een tekstregel opslaat die de gemengde opmaak bevat: **Vette tekst en cursief**

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

>[!NOTE]
>
>Alle versies na de release 20.3 bieden ondersteuning voor opties voor vet, cursief en onderstrepen.

## entiteitMaps en entiteitRanges

Een gegevensblok kan entiteiten bevatten zoals hyperlinks of andere typen gestileerde opmaak die zijn verbonden met gegevensbronnen buiten het aangepaste tekstveld.

## Voorbeelden

### Onbewerkte tekst ophalen van JSON

Wanneer een aangepast veld met RTF-opmaak wordt verzonden, wordt alle tekst opgeslagen in de array **blokken**. Elke regel van de volledige tekst wordt echter opgeslagen in de **text, parameter** binnen elk van de afzonderlijke blokelementen die de bovenliggende array vormen **blokken**. Om de volledige tekst op te halen, moet elke afzonderlijke tekstregel worden opgehaald en samen worden geparkeerd. Dit kan worden bereikt door alle elementen in blokken te herhalen en elke tekstparameter samen met een regelscheidingsteken (\n) te koppelen.

**Voorbeeld:** Zo ziet uw JS er mogelijk uit:

<!-- [Copy](javascript:void(0);) -->
<pre></pre>

### Een RTF-waarde opslaan met de Workfront API

De volgende waarden van een RTF-veld opslaan met de Workfront API:
<pre>
		Hallo <strong>Wereld</strong>!!!
		Dit is mijn eerste <strong>RTF</strong></pre>

1. Construeer JSON die de waarde van het rijke-tekstgebied vertegenwoordigt u probeert te vangen door elke lijn van tekst in een blokelement, in de serie te organiseren **blokken**

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Leg de RTF-opmaak vast met de opdracht **inlineStyleRanges** parameter

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Als u de tweede regel wilt vastleggen, moet de tekst &#39;RTF&#39; zowel vet als cursief worden opgemaakt.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

   >[!NOTE]
   >
   >Hoewel de functionaliteit entityMap niet tijdens de aanvankelijke versie wordt gesteund, is het nog een vereist gebied om deze JSON in een verzoek over te gaan

1. Gebruik de **aanscherpen** op de hierboven beschreven JSON-methode om een **PUT** aanvragen en updates verzenden

   <!-- [Copy](javascript:void(0);) -->
   <pre><OBJ Code><OBJ ID></pre>
