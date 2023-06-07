---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: Tekstparser
description: Met het gereedschap Tekstparser kunt u tekst parseren voor gebruik in andere [!DNL Adobe Workfront Fusion] scenario-modules. Voor de tekstparser is geen verbinding vereist.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 54d1753b9062b6d4910e4478c1f072b7fedc87eb
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# [!UICONTROL Text parser]

U kunt de [!UICONTROL Text parser tool] tekst parseren voor gebruik in andere [!DNL Adobe Workfront Fusion] scenario-modules. De [!UICONTROL Text parser] geen verbinding vereist.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Text parser] modules en hun velden

Wanneer u [!UICONTROL Text parser] modules, [!DNL Adobe Workfront Fusion] geeft de onderstaande velden weer. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Transformatoren

* [[!UICONTROL Get Elements from HTML]](#get-elements-from-html)
* [[!UICONTROL Get Elements from text]](#get-elements-from-text)
* [[!UICONTROL HTML to Text]](#html-to-text)
* [[!UICONTROL Match Pattern]](#match-pattern)
* [[!UICONTROL Replace]](#replace)

#### [!UICONTROL Get Elements from HTML]

Hiermee worden de gewenste elementen opgehaald uit de HTML-code.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module finds no matches]</td> 
   <td> <p>Schakel deze optie in om ervoor te zorgen dat de module het scenario niet stopt als er geen resultaten worden geretourneerd.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Element type]</td> 
   <td> <p> Selecteer het elementtype dat u wilt ophalen uit de HTML-code. </p> 
    <ul> 
     <li>[!UICONTROL Image]</li> 
     <li>[!UICONTROL Link]</li> 
     <li>[!UICONTROL iFrame element(s)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Voer de HTML-code in of wijs deze toe waaruit u de opgegeven elementtypen wilt ophalen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Elements from text]

Hiermee parseert u elementen van tekst op basis van het opgegeven patroon.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Input text]</td> 
   <td> <p>Typ of wijs de tekst toe die u wilt parseren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pattern]</td> 
   <td> <p>Selecteer het patroon dat de elementen weerspiegelt die u in de tekst wilt parseren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ignore Duplicate Occurrences]</td> 
   <td> <p>Schakel dit vakje in om dubbele instanties van een tekstelement te negeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL HTML to Text]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>Voer de HTML-code in die u wilt omzetten in onbewerkte tekst.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Line break] </td> 
   <td> <p>Selecteer het type nieuwe regel (regeleinde).</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Uppercase headings]</p> </td> 
   <td> <p>Schakel deze optie in om tekst die in kopcodes staat, om te zetten (zoals &lt;h2&gt; &lt;/h2&gt;) in hoofdletters.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Match Pattern]

De [!UICONTROL Match pattern] kunt u tekenreekselementen zoeken en extraheren die overeenkomen met een zoekpatroon in een bepaalde tekst. Deze module gebruikt reguliere expressies (ook wel regex of regexp genoemd).

Een reguliere expressie is een reeks tekens waarin elk teken een metateken is met een speciale betekenis of een regulier teken met een letterlijke betekenis. Met deze teken- en metatekens wordt een patroon geïdentificeerd dat kan worden gebruikt voor het zoeken naar tekst. Als u bijvoorbeeld naar namen wilt zoeken, kunt u een reguliere expressie instellen om te zoeken naar een patroon dat bestaat uit twee opeenvolgende woorden die beginnen met hoofdletters. Reguliere expressies zijn een krachtig gereedschap voor het zoeken en bewerken van tekst.

Een discussie over reguliere expressies valt buiten het toepassingsgebied van dit artikel. Wij adviseren de volgende middelen:

* Voor de volledige lijst met metatekens raadpleegt u [Reguliere expressies](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) in MDN-webdocumenten.
* Voor een zelfstudie over het maken van reguliere expressies raden we aan [RegexOne](https://regexone.com/).
* Voor het experimenteren met reguliere expressies raden we de [Gewone uitdrukkingen 101](https://regex101.com/) website. Selecteer de ECMAScript-FLAVOR (JavaScript) in het linkerdeelvenster.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>Voer het reguliere-expressiepatroon in. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> Extraheert alle cijfers in de opgegeven tekst.</p> <p>Opmerking:  <p>Het patroon moet ten minste één vastleggroep tussen haakjes bevatten <code>()</code>. Als het patroon geen vastleggingsgroepen bevat, is de uitvoerbundel leeg.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global match]</td> 
   <td> <p>Schakel deze optie in om alle overeenkomsten in de tekst op te halen. Elke overeenkomst wordt uitgevoerd in een afzonderlijke bundel. Als deze optie is uitgeschakeld, haalt de module alleen het eerste item op.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Case sensitive]</td> 
   <td> <p> Schakel deze optie voor deze module in om tekst als hoofdlettergevoelig te behandelen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Schakel deze optie in om ervoor te zorgen dat metatekens aan het begin en einde (<code>^</code> en <code>$</code>) komt overeen met het begin of einde van elke regel, niet alleen het uiterste begin of einde van de gehele invoertekenreeks.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Schakel deze optie in om ervoor te zorgen dat de periode (.) komt overeen met nieuwe-regeltekens (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module returns no results]</td> 
   <td> <p>Schakel deze optie in om ervoor te zorgen dat de module het scenario niet stopt als er geen resultaten worden geretourneerd.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>Typ of wijs de tekst toe die u aan het patroon wilt aanpassen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Replace]

Zoekt de ingevoerde tekst naar een opgegeven waarde of reguliere expressie en vervangt het resultaat door de nieuwe waarde.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>Voer de zoekterm in. U kunt ook een reguliere expressie gebruiken. Voor meer informatie over de reguliere expressie raadpleegt u de <a href="#match-pattern" class="MCXref xref">[!UICONTROL Match Pattern]</a> module.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL New value]</td> 
   <td> <p> Voer een waarde in die de zoekterm vervangt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global match]</td> 
   <td> <p>Schakel deze optie in om alle overeenkomsten in de tekst op te halen. Elke overeenkomst wordt uitgevoerd in een afzonderlijke bundel. Als deze optie is uitgeschakeld, haalt de module alleen het eerste item op.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Case sensitive]</td> 
   <td> <p> Schakel deze optie voor deze module in om tekst als hoofdlettergevoelig te behandelen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>Schakel deze optie in om ervoor te zorgen dat metatekens aan het begin en einde (<code>^</code> en <code>$</code>) komt overeen met het begin of einde van elke regel, niet alleen het uiterste begin of einde van de gehele invoertekenreeks.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>Schakel deze optie in om ervoor te zorgen dat de periode (.) komt overeen met nieuwe-regeltekens (<code>\n</code>).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>Voer de tekst in die u wilt doorzoeken.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Gegevensovervulling

Het schrapen van gegevens, soms genoemd Webschrapping, gegevensextractie, of Web het oogsten, is het proces om gegevens van websites te verzamelen en het op te slaan in uw lokale gegevensbestand of spreadsheets. Als u gegevens van een website wilt verwijderen en u niet bekend bent met reguliere expressies, kunt u een gereedschap voor het verwijderen van gegevens gebruiken.

Als het hulpprogramma voor het plakken van gegevens een REST API biedt, kunt u er verbinding mee maken via onze universele [[!UICONTROL HTTP] modules](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) en [Webhaken](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) modules.
