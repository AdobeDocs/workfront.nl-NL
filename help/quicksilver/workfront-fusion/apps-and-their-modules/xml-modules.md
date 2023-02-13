---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: XML
description: Met de XML-toepassing kunt u tekst met XML-indeling parseren via de XML-&gt. Parseer de module van XML en zet het in een bundel om om de gegevens ter beschikking te stellen aan andere modules. U kunt een bundel via de XML-&gt ook omzetten in tekst met XML-indeling; XML-module maken
author: Becky
feature: Workfront Fusion
exl-id: 3459e930-8156-4171-8920-34f4e07bc530
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 2%

---

# XML

De [!UICONTROL XML] kunt u een tekst met XML-opmaak parseren via de [!UICONTROL XML] > [!UICONTROL Parse XML] en zet deze om in een bundel om de gegevens beschikbaar te maken voor andere modules. U kunt een bundel via de [!UICONTROL XML] > [!UICONTROL Create XML] module

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Parse XML]

De [!UICONTROL XML] > [!UICONTROL Parse XML] parseert een XML-tekst en voert een enkele bundel uit die alle informatie bevat die uit de XML is geëxtraheerd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Data structure]</p> </td> 
   <td> <p>De gegevensstructuur beschrijft de structuur van XML om de output van de module beschikbaar te maken in het toewijzingspaneel voor de volgende modules.</p> <p>Als u een voorbeeld hebt van de XML die u wilt parseren, kunt u deze gebruiken om de gegevensstructuur te genereren:</p> 
    <ol> 
     <li value="1">Klik op de knop <strong>[!UICONTROL Add]</strong> knop.</li> 
     <li value="2">Klik op de knop <strong>[!UICONTROL Generator]</strong> knop.</li> 
     <li value="3">Het XML-voorbeeld kopiëren en in het deelvenster <strong>[!UICONTROL Sample data]</strong> veld.</li> 
     <li value="4">Klik op <strong>[!UICONTROL Save]</strong>.</li> 
     <li value="5">Controleer of de gegevensstructuur is gegenereerd.</li> 
     <li value="6"> <p>Klik op de knop <strong>[!UICONTROL Save]</strong> om de gegevensstructuur op te slaan.</p> <p>U kunt de stappen 2 tot en met 5 overslaan om een lege gegevensstructuur op te geven. Als de gegevensstructuur leeg is, is de uitvoer van de module niet beschikbaar in het deelvenster Toewijzing totdat de module ten minste één keer is uitgevoerd.</p> </li> 
    </ol> <p>Zie voor meer informatie <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Gegevensstructuren in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Preserve numbers as text]</td> 
   <td>Schakel deze optie in om ervoor te zorgen dat getallen behouden blijven als tekst (tekenreeks). Anders worden getallen naar getalwaarden gecast.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL XML]</p> </td> 
   <td> <p>Typ of wijs de XML-opgemaakte tekst toe die u wilt parseren.</p> <p>Als u een formule gebruikt, zorg ervoor zijn resultaatwaardetype (of kan automatisch tot worden gedwongen) is [!UICONTROL Text] gegevenstype. </p> <p> <img src="assets/if-you-use-a-formula-350x164.png" style="width: 350;height: 164;"> </p> <p>Als het type resultaatwaarde [!UICONTROL Buffer] (binaire gegevens) gebruikt u vervolgens de <code>toString()</code> om deze om te zetten in het gegevenstype Text. Zie voor meer informatie <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Afgedwongen typegebruik in [!DNL Adobe Workfront Fusion]</a> en <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Gegevenstypen item in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Voorbeeld:** Een XML-bestand downloaden van een URL en de inhoud ervan parseren:
>
>1. Maak een nieuw scenario.
>1. Invoegen [!UICONTROL HTTP] > [!UICONTROL Get a file] module
>1. Open de configuratie van de module en vorm het als volgt:

>
>   **URL**: URL van het XML-bestand (bijvoorbeeld `https://siftrss.com/f/rqLy05ayMBJ`)
>
>   ![](assets/url-of-xml-file-350x184.png)
>
>1. Klikken **[!UICONTROL OK]**&#x200B; om de configuratie van de module te bewaren en te sluiten.
1. Toevoegen [!UICONTROL XML] > [!UICONTROL Parse XML] -module, sluit deze aan na de [!UICONTROL HTTP] > [!UICONTROL Get a file] en deze als volgt configureren:
<table style="table-layout:auto"> 
&gt;    <col> 
&gt;    <col> 
&gt;    <tbody> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL Data structure]</td> 
&gt;      <td> 
&gt;       <ol> 
&gt;        <li value="1">Klik op de knop <strong>[!UICONTROL Add]</strong> knop.</li> 
&gt;        <li value="2">Klik op de knop <strong>[!UICONTROL Generator]</strong> knop.</li> 
&gt;        <li value="3">Open een nieuw tabblad of venster in uw webbrowser.</li> 
&gt;        <li value="4">Plaats URL u in de derde stap in de adresbar gebruikte en haal het dossier van XML.</li> 
&gt;        <li value="5">Selecteer alle XML-tekst en kopieer deze naar het klembord.</li> 
&gt;        <li value="6">Sluit de tab of het venster en ga terug naar het scenario.</li> 
&gt;        <li value="7">Plak de gekopieerde XML-tekst in het veld Voorbeeldgegevens.</li> 
&gt;        <li value="8">Klik op <strong>[!UICONTROL Save]</strong>.</li> 
&gt;        <li value="9">Controleer of de gegevensstructuur is gegenereerd.</li> 
&gt;        <li value="10">Klikken <strong>[!UICONTROL Save]</strong> om de gegevensstructuur op te slaan.</li> 
&gt;       </ol> <p>U kunt stap 2 tot en met 9 overslaan om een lege gegevensstructuur op te geven. Als de gegevensstructuur leeg is, is de uitvoer van de module niet beschikbaar in het deelvenster Toewijzing totdat de module ten minste één keer is uitgevoerd.</p> </td> 
&gt;     </tr> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL XML]</td> 
&gt;      <td> <p>Wijs de <code>Data </code>item uit de uitvoer van het [!UICONTROL HTTP] &gt; [!UICONTROL Get a file] in het veld. Gebruik de <code>toString()</code> functie om zijn waarde van om te zetten [!UICONTROL Buffer] (binaire gegevens) type to [!UICONTROL Text] gegevenstype.</p> <p>U kunt de code van de formule kopiëren en in het gebied kleven: <code>&#123;&#123;toString(1.data)&#125;&#125;</code></p> <p>Zie voor meer informatie over de gegevenstypen Buffer en Text <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Gegevenstypen item in Adobe Workfront Fusion</a>.</p> <p> <img src="assets/paste-formula-code-350x99.png" style="width: 350;height: 99;"> </p> </td> 
&gt;     </tr> 
&gt;    </tbody> 
&gt;   </table>


## [!UICONTROL Parsing XML attributes]

Standaard worden de [!UICONTROL XML] > [!UICONTROL Parse XML] module plaatst attributen in een speciale inzameling `_attributes` als een onderliggend element van het knooppunt dat deze kenmerken heeft. Als het knooppunt een tekstknooppunt is en kenmerken heeft, worden twee speciale eigenschappen toegevoegd: `_attributes` voor kenmerken en `_value` voor de tekstinhoud van het knooppunt.

>[!INFO]
**Voorbeeld:** Deze XML:

```
<root attr="1">
<node attr="ABC">Hello, World</node>
</root>
```

wordt omgezet in deze bundel:

![](assets/xml-converted-to-bundle.png)

## XML maken

De [!UICONTROL XML] > [!UICONTROL Create XML] converteert een bundel naar tekst met XML-indeling.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Data structure]</p> </td> 
   <td> <p>De gegevensstructuur beschrijft de structuur van de resulterende XML. Als u een voorbeeld hebt van de XML die u wilt maken, kunt u deze gebruiken om de gegevensstructuur te genereren:</p> 
    <ol> 
     <li value="1">Klik op de knop <strong>[!UICONTROL Add]</strong> knop.</li> 
     <li value="2">Klik op de knop <strong>[!UICONTROL Generator]</strong> knop.</li> 
     <li value="3">Kopieer en plak het XML-voorbeeld in het veld Voorbeeldgegevens.</li> 
     <li value="4">Klik op de knop <strong>[!UICONTROL Save]</strong> knop.</li> 
     <li value="5">Controleer of de gegevensstructuur is gegenereerd.</li> 
     <li value="6">Klikken <strong>[!UICONTROL Save]</strong> om de gegevensstructuur op te slaan.</li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Root element name]</td> 
   <td>Voer de naam van het hoofdelement van de XML in. De standaardwaarde is <code>root</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype SYSTEM ID]</td> 
   <td>Voer de bestandsnaam in die u wilt gebruiken in het dialoogvenster<code> !DOCTYPE SYSTEM</code> declaratie</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype PUBLIC ID]</td> 
   <td>Voer de bestandsnaam in die u wilt gebruiken in het dialoogvenster<code> !DOCTYPE PUBLIC</code> declaratie</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Strip Xml Declaration]</td> 
   <td>Schakel deze optie in om de XML-declaratie te verwijderen <code>&lt;?xml ... ?&gt;</code> en <code>&lt;!DOCTYPE ... &gt;</code>en laat alleen het XML-hoofdelement en de inhoud ervan ongewijzigd.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
**Voorbeeld:**
Doorgaans worden gegevens getransformeerd van een [!DNL Google] >spreadsheet in XML.
1. Plaats de [!DNL Google Sheets] > [!UICONTROL Select rows] in uw scenario om de gegevens op te halen. Stel de module in om rijen op te halen uit uw [!DNL Google] spreadsheet. De &#x200B; instellen **[!UICONTROL Maximum number of returned rows]** tot een klein aantal, maar groter dan één voor testdoeleinden (bijvoorbeeld drie). Voer de [!DNL Google Sheets] door er met de rechtermuisknop op te klikken en &quot;**[!UICONTROL Run this module only]**.&quot; Controleer de uitvoer van de module.
1. Verbind de [!UICONTROL Array Aggregator] module na de [!DNL Google Sheets] module. In de opstelling van de module kiest u [!DNL Google Sheets] in de **[!UICONTROL Source node]** veld. Laat de andere velden op dit moment ongewijzigd.
1. Verbind de [!UICONTROL XML] > [!UICONTROL Create XML] module na de [!UICONTROL Array Aggregator] module.
   De opstelling van de module vereist een gegevensstructuur die de structuur van de output van XML beschrijft. Klik op de knop **[!UICONTROL Add]** om de gegevensstructuurinstellingen te openen. De eenvoudigste manier om deze gegevensstructuur te maken, is deze automatisch te genereren op basis van een XML-voorbeeld.
1. Klik op de knop **[!UICONTROL Generator]** en plak uw XML-voorbeeld in de [!UICONTROL Sample data] veld:

![](assets/sample-data-field-350x146.png)
1. Klik op **[!UICONTROL Save]**. Het veld Specificatie in de gegevensstructuur bevat nu de gegenereerde structuur.
1. Wijzig de naam van de gegevensstructuur in een specifiekere naam en klik op **[!UICONTROL Save]**. Een veld dat overeenkomt met het kenmerk van de hoofdarray wordt als een toewijzingsveld weergegeven in de instellingen van de JSON-module.
1. Klik op de knop **[!UICONTROL Map]** naast het veld en wijs de `Array[]` item van [!UICONTROL Array aggregator] uitvoer naar:
1. Klikken **[!UICONTROL OK]** om de instelling van de XML-module te sluiten.
1. Open de instelling van het dialoogvenster [!UICONTROL Array Aggregator] module. Wijzig de **[!UICONTROL Target structure]** van Aangepast naar het veld van een XML-module dat overeenkomt met de bovenliggende items XML element.Map van het [!DNL Google Sheets] aan de aangewezen gebieden.
1. Klikken **[!UICONTROL OK]** om de installatie van de Array Aggregator-module te sluiten.
1. Voer het scenario uit.

   De module XML geeft het juiste XML-bestand als uitvoer.
1. Open de instelling van het dialoogvenster [!DNL Google Sheets] en verhoogt u de [!UICONTROL Maximum number of returned rows] getal dat groter is dan het aantal rijen in het werkblad om alle gegevens te verwerken.
   De resulterende XML kan worden opgeslagen naar [!DNL Dropbox], verzonden als bijlage via e-mail, geüpload via FTP naar een server, enzovoort.


## XML-kenmerken toevoegen

Als u attributen aan een complexe knoop (een knoop wilt toevoegen die andere knopen zal bevatten), moet u een inzameling met de naam toevoegen `_attributes` voor de complexe notitie in uw aangepaste gegevensstructuur. Deze verzameling wordt toegewezen aan knooppuntkenmerken. Als u kenmerken wilt toevoegen aan een tekstknooppunt (bijvoorbeeld: `<node attr="1">abc</node>`), moet u een verzameling toevoegen `_attributes` voor kenmerken en een teksteigenschap `_value` voor de knoopwaarde voor dit knooppunt in uw aangepaste gegevensstructuur.

```
{
   "name": "node",
   "type": "collection",
   "spec": [
      {
         "name": "_attributes",
         "type": "collection"
         "spec": [
            {
               "name": "attr1",
               "type": "text"
            }
         ]
      },
      {
         "name": "_value",
         "type": "text"
      }
   ]
}
```

## Problemen oplossen: Kan geen gegevens toewijzen uit de [!UICONTROL Parse XML] module

Zorg ervoor dat de gegevensstructuur correct is gedefinieerd. U kunt ook een lege gegevensstructuur gebruiken en de module ten minste één keer uitvoeren om een XML-invoer te verwerken.
