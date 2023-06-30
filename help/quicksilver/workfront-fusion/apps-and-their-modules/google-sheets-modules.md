---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Google Sheets-modules
description: Voor gebruik [!DNL Google Sheets] with [!DNL Adobe Workfront Fusion],you need the [!UICONTROL Workfront Fusion Google Sheets] extensie (optioneel, maar vereist voor instant-triggers).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 11d62222-df34-472d-93d7-f0d53eb95c9b
source-git-commit: 6f4e5042054f3936fa0e387bfbebaa1775d16573
workflow-type: tm+mt
source-wordcount: '3439'
ht-degree: 0%

---

# [!DNL Google Sheets] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Google Sheets]en deze verbinding maken met meerdere toepassingen en services van derden.

Voor instructies over het aansluiten van uw [!DNL Google Sheets] account aan [!DNL Workfront Fusion], zie [Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies](../../workfront-fusion/connections/connect-to-fusion-general.md)

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

## Vereisten

Te gebruiken [!UICONTROL Google Sheets] modules, moet u een [!UICONTROL Google] account.

## Triggers

### [!UICONTROL Watch Rows]

Haalt waarden op van elke nieuwe rij die is toegevoegd aan het werkblad.

De module wint slechts nieuwe rijen terug die niet eerder zijn ingevuld. De trigger verwerkt geen overschreven rij.

>[!IMPORTANT]
>
>Als het werkblad een lege rij bevat, worden er geen rijen na de lege rij verwerkt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Sheets] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Spreadsheet] </td> 
   <td> <p>Selecteer het werkblad dat het werkblad bevat dat u wilt bekijken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sheet] </td> 
   <td> <p>Selecteer het werkblad dat u wilt controleren voor een nieuwe rij.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table contains headers]</td> 
   <td> <p> Selecteer of het spreadsheet de kopbalrij bevat.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Yes]</strong> </p> <p>De module haalt de koptekstrij niet op als uitvoergegevens. </p> <p>De namen van variabelen in de uitvoer worden aangeroepen door de kopteksten.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>De module wint ook de eerste lijstrij terug</p> <p>De namen van variabelen in de uitvoer worden A, B, C, D enzovoort genoemd.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Row with headers] </td> 
   <td> <p>Voer het bereik van de koptekstrij in. Bijvoorbeeld, <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL First table row]</td> 
   <td> <p>Voer het bereik van de eerste rij van de tabel in. Bijvoorbeeld, <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Value render option]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Formatted value]</p> <p>De waarden worden berekend en opgemaakt in de reactie volgens de opmaak van de cel. Opmaak is gebaseerd op de landinstelling van het werkblad, niet op de landinstelling van de gebruiker die het verzoek indient. Als <code>A1</code> is <code>1.23</code> en <code>A2</code> is <code>=A1</code> en worden opgemaakt als valuta, en vervolgens <code>A2</code> zou terugkeren <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Unformatted value]</p> <p>De waarden worden berekend, maar niet opgemaakt in de reactie. Als <code>A1</code> is <code>1.23</code> en <code>A2</code> is <code>=A1</code> en worden opgemaakt als valuta, en vervolgens <code>A2</code> retourneert het getal <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formula]</p> <p>De waarden worden niet berekend. Het antwoord zal ook de formules bevatten. Als <code>A1</code> is <code>1.23</code> en <code>A2</code> is <code>=A1</code> en worden opgemaakt als valuta, en vervolgens <code>A2</code> zou terugkeren <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Date and time render option]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Serial number]</p> <p>Geeft velden voor datum, tijd, datumtijd en tijdsduur de opdracht om te worden uitgevoerd als dubbele gegevens in de indeling "serienummer", zoals deze worden gevuld door Lotus 1-2-3. Het gehele getalgedeelte van de waarde (links van het decimaalteken) telt de dagen sinds 30 december 1899. Het fractionele gedeelte (rechts van het decimaalteken) telt de tijd als een fractie van de dag. Bijvoorbeeld, zou 1 januari 1900 om 12.00 uur 2.5 zijn, 2 omdat het 2 dagen na 30 december 1899 is, en 0.5 omdat 12.00 uur een halve dag is. 1 februari 1900 om 15.00 uur is 33.625 uur. Dit is een goede manier om het jaar 1900 te beschouwen als geen schrikkeljaar.</p> <p style="font-weight: bold;">[!UICONTROL Formatted string]</p> <p>Hiermee worden datum-, tijd-, datum- en duurvelden geïnstrueerd als tekenreeksen in de opgegeven getalnotatie (die afhankelijk is van de landinstelling van het werkblad).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Stel het maximale aantal resultaten in dat [!DNL Workfront Fusion] zal met tijdens één uitvoeringscyclus werken.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Handelingen

* [[!UICONTROL Add a Row]](#add-a-row)
* [[!UICONTROL Update a Row]](#update-a-row)
* [[!UICONTROL Clear a Row]](#clear-a-row)
* [[!UICONTROL Delete a Row]](#delete-a-row)
* [[!UICONTROL Get a Cell]](#get-a-cell)
* [[!UICONTROL Update a Cell]](#update-a-cell)
* [[!UICONTROL Clear a Cell]](#clear-a-cell)
* [[!UICONTROL Add a Sheet]](#add-a-sheet)
* [[!UICONTROL Create a Spreadsheet]](#create-a-spreadsheet)
* [[!UICONTROL Delete a Sheet]](#delete-a-sheet)
* [[!UICONTROL Make an API Call]](#make-an-api-call)

### [!UICONTROL Add a Row]

Met deze module voegt u een rij toe aan een vel.

Wanneer u [!DNL Google Sheets] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Google Sheets] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Sheets] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mode]</td> 
   <td> <p>Selecteer of u de spreadsheet en het blad handmatig of door toewijzing wilt selecteren.</p> <p>Opmerking: Handmatige toewijzing is bijvoorbeeld handig wanneer een nieuw spreadsheet wordt gemaakt in een [!DNL Workfront Fusion] scenario en u wilt gegevens in nieuw gecreeerd spreadsheet direct in het scenario toevoegen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Selecteer [!DNL Google] spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Selecteer het blad waaraan u een rij wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Column Range]</td> 
   <td>Selecteer het kolombereik waarmee u wilt werken.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Table contains headers]</td> 
   <td> <p> Selecteer of het spreadsheet de kopbalrij bevat.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Yes]</strong> </p> <p>De module haalt de koptekstrij niet op als uitvoergegevens. </p> <p>De namen van variabelen in de uitvoer worden aangeroepen door de kopteksten.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>De module wint ook de eerste lijstrij terug</p> <p>De namen van variabelen in de uitvoer worden A, B, C, D enzovoort genoemd.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Values] </td> 
   <td> <p>Voer de gewenste cellen in van de rij die u wilt toevoegen of wijs deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value input option]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL User entered]</strong></p> <p>De waarden worden geparseerd alsof de gebruiker hen in UI typt. Getallen blijven getallen, maar tekenreeksen kunnen in getallen, datums of andere indelingen worden omgezet volgens dezelfde regels die gelden wanneer u tekst in een cel invoert via de [!DNL Google Sheets] UI.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> De waarden die de gebruiker invoert, worden niet geparseerd en worden als zodanig opgeslagen. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Insert data option]</td> 
   <td> <p>Geef op hoe bestaande gegevens moeten worden gewijzigd wanneer nieuwe gegevens worden ingevoerd. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Insert rows]</strong></p> <p>De rijen worden opgenomen voor de nieuwe gegevens.</p> </li> 
     <li> <p><strong>[!UICONTROL Overwrite]</strong> </p> <p>De nieuwe gegevens overschrijven bestaande gegevens in de gebieden waar ze zijn geschreven. Als u gegevens toevoegt aan het einde van het blad, worden nieuwe rijen of kolommen ingevoegd, zodat de gegevens kunnen worden geschreven.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Update a Row]

In deze module kunt u de celinhoud in een geselecteerde rij wijzigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Sheets] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mode]</td> 
   <td> <p>Selecteer of u de spreadsheet en het blad handmatig of door toewijzing wilt selecteren.</p> <p>Opmerking: Handmatige toewijzing is bijvoorbeeld handig wanneer een nieuw spreadsheet wordt gemaakt in het dialoogvenster [!UICONTROL Workfront Fusion] scenario en u wilt gegevens aan pas gecreeerd spreadsheet direct in het scenario toevoegen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Selecteer [!DNL Google] spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Selecteer het blad waarin u een rij wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Row number]</td> 
   <td> <p> Voer het nummer in van de rij die u wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Table contains headers]</td> 
   <td> <p> Selecteer of het spreadsheet de kopbalrij bevat.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Yes]</strong> </p> <p>De module haalt de koptekstrij niet op als uitvoergegevens. </p> <p>De namen van variabelen in de uitvoer worden aangeroepen door de kopteksten.</p> </li> 
     <li> <p><strong>[!UICONTROL No]</strong> </p> <p>De module wint ook de eerste lijstrij terug</p> <p>De namen van variabelen in de uitvoer worden A, B, C, D enzovoort genoemd.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Values] </td> 
   <td> <p>Voer de waarden in of wijs deze toe aan de gewenste cellen van de rij die u wilt wijzigen (bijwerken).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value input option]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL User entered]</strong></p> <p>De waarden worden geparseerd alsof de gebruiker hen in UI typt. Getallen blijven getallen, maar tekenreeksen kunnen in getallen, datums of andere indelingen worden omgezet volgens dezelfde regels die gelden wanneer u tekst in een cel invoert via de [!DNL Google Sheets] UI.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> De waarden die de gebruiker invoert, worden niet geparseerd en worden als zodanig opgeslagen. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Clear a Row]

Hiermee verwijdert u waarden uit een opgegeven rij.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Sheets] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Selecteer [!DNL Google] spreadsheet die het blad bevat u een rij van wilt ontruimen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p> Selecteer het blad waarvan u gegevens wilt wissen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Row number]</td> 
   <td> <p>Voer het nummer in van de rij waaruit u gegevens wilt wissen. Bijvoorbeeld, <code> 23</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Delete a Row]

Hiermee verwijdert u een opgegeven rij.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Sheets] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Selecteer de Google-spreadsheet met het blad waaruit u een rij wilt verwijderen.</p> </td> 
  </tr> 
  <tr> 
   <td>Werkblad </td> 
   <td> <p>Selecteer het blad waarvan u een rij wilt verwijderen.</p> </td> 
  </tr> 
  <tr> 
   <td>Rijnummer</td> 
   <td> <p>Voer het nummer in van de rij die u wilt verwijderen. Voorbeeld: <code>23</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Get a Cell]

Hiermee wordt een waarde uit een geselecteerde cel opgehaald.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Sheets] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Selecteer [!DNL Google] spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Selecteer het werkblad met de cel waaruit u de gegevens wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Voer de id in van de cel waarvan u de gegevens wilt ophalen. Voorbeeld: <code>A6</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Formatted value]</p> <p>De waarden worden berekend en opgemaakt in de reactie volgens de opmaak van de cel. Opmaak is gebaseerd op de landinstelling van het werkblad, niet op de landinstelling van de gebruiker die het verzoek indient. Als <code>A1</code> is <code>1.23</code> en <code>A2</code> is <code>=A1</code> en worden opgemaakt als valuta, en vervolgens <code>A2</code> zou terugkeren <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Unformatted value]</p> <p>De waarden worden berekend, maar niet opgemaakt in de reactie. Als <code>A1</code> is <code>1.23</code> en <code>A2</code> is <code>=A1</code> en worden opgemaakt als valuta, en vervolgens <code>A2</code> retourneert het getal <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Formula]</p> <p>De waarden worden niet berekend. Het antwoord zal ook de formules bevatten. Als <code>A1</code> is <code>1.23</code> en <code>A2</code> is <code>=A1</code> en worden opgemaakt als valuta, en vervolgens <code>A2</code> zou terugkeren <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!DNL Serial number]</p> <p>Geeft velden voor datum, tijd, datumtijd en tijdsduur de opdracht om te worden uitgevoerd als dubbele gegevens in de indeling "serienummer", zoals deze worden gevuld door Lotus 1-2-3. Het gehele getalgedeelte van de waarde (links van het decimaalteken) telt de dagen sinds 30 december 1899. Het fractionele gedeelte (rechts van het decimaalteken) telt de tijd als een fractie van de dag. Bijvoorbeeld, zou 1 januari 1900 om 12.00 uur 2.5 zijn, 2 omdat het 2 dagen na 30 december 1899 is, en 0.5 omdat 12.00 uur een halve dag is. 1 februari 1900 om 15.00 uur is 33.625 uur. Dit is een goede manier om het jaar 1900 te beschouwen als geen schrikkeljaar.</p> <p style="font-weight: bold;">[!DNL Formatted string]</p> <p>Hiermee worden datum-, tijd-, datum- en duurvelden geïnstrueerd als tekenreeksen in de opgegeven getalnotatie (die afhankelijk is van de landinstelling van het werkblad).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Update a Cell]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Sheets] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Selecteer [!DNL Google] spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Voer de id in van de cel die u wilt bijwerken. Voorbeeld: <code>A5</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value]</td> 
   <td> <p>Voer de nieuwe waarde voor de cel in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value input option]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL User entered]</strong></p> <p>De waarden worden geparseerd alsof de gebruiker hen in UI typt. Getallen blijven getallen, maar tekenreeksen kunnen in getallen, datums of andere indelingen worden omgezet volgens dezelfde regels die gelden wanneer u tekst in een cel invoert via de [!DNL Google Sheets] UI.</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> De waarden die de gebruiker invoert, worden niet geparseerd en worden als zodanig opgeslagen. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Clear a Cell]

Hiermee wordt een waarde uit een opgegeven cel verwijderd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Sheets] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Selecteer de Google-spreadsheet met het vel waaruit u een cel wilt wissen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Selecteer het blad waarvan u een cel wilt wissen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cell] </td> 
   <td> <p>Voer de id in van de cel die u wilt wissen. Voorbeeld: <code>A5</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Add a Sheet]

Hiermee maakt u een nieuw blad in een geselecteerde spreadsheet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Sheets] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Selecteer de Google-spreadsheet waar u een vel wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Properties]</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">[!UICONTROL Title]</p> <p>Voer de naam van het nieuwe blad in.</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL Index]</p> <p>Voer de positie van het blad in. De standaardwaarde is 0 (het blad wordt op de eerste plaats geplaatst)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Create a Spreadsheet]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Sheets] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title] </td> 
   <td> <p>Voer de naam van een nieuw spreadsheet in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Locale]</td> 
   <td> <p>Voer de landinstelling van het werkblad in een van de volgende notaties in:</p> 
    <ul> 
     <li>een ISO 639-1 taalcode zoals <code>en</code></li> 
     <li>een ISO 639-2 taalcode zoals <code>haw</code>, als er geen 639-1 code bestaat</li> 
     <li>een combinatie van de ISO-taalcode en de landcode, zoals <code>en_US</code></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recalculation interval]</td> 
   <td> <p>De hoeveelheid tijd die moet worden gewacht voordat vluchtige functies opnieuw worden berekend:</p> <p style="font-weight: bold;">[!UICONTROL On change]</p> <p>Vluchtige functies worden bij elke wijziging bijgewerkt.</p> <p style="font-weight: bold;">[!UICONTROL On change and every minute]</p> <p>Vluchtige functies worden bij elke wijziging en elke minuut bijgewerkt.</p> <p style="font-weight: bold;">[!UICONTROL On change and hourly]</p> <p>Vluchtige functies worden bij elke verandering en per uur bijgewerkt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time zone]</td> 
   <td> <p> Selecteer de tijdzone van het spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Number format]</td> 
   <td> <p>Selecteer de standaardindeling van alle cellen in het werkblad.</p> <p><strong>[!UICONTROL Text]</strong>: Tekstopmaak. Voorbeeld: <code>1000. 12</code></p> <p><strong>[!UICONTROL Number]</strong>: Getalopmaak. Voorbeeld: <code>1,000.12</code></p> <p><strong>[!UICONTROL Percent]</strong>: Percentage van opmaak. Voorbeeld: <code>10. 12%</code></p> <p><strong>[!UICONTROL Currency]</strong>: Opmaak van valuta. Voorbeeld: <code>$1,000.12</code></p> <p><strong>[!UICONTROL Date]</strong>: Opmaak datum. Voorbeeld: <code>9/26/2008</code></p> <p><strong>[!UICONTROL Time]</strong>: Tijdnotatie. Voorbeeld: <code>3:59:00 PM</code></p> <p><strong>[!UICONTROL Date time]</strong>: Opmaak datum en tijd. Voorbeeld: <code>9/26/08 15:59:00</code> </p> <p><strong>[!UICONTROL Scientific]</strong>Wetenschappelijke getalnotatie. Voorbeeld: <code>1. 01E+03</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheets] </td> 
   <td> <p>Klikken <strong>[!UICONTROL Add]</strong> om een werkblad aan het werkblad toe te voegen. Voer voor elk blad een titel voor het blad en de index van het blad in of wijs deze toe. Een index van 0 staat voor het eerste blad.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Delete a Sheet]

Hiermee verwijdert u een specifiek blad.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Sheets] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Selecteer [!DNL Google] spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Selecteer het blad dat u wilt verwijderen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Make an API Call]

Met deze actiemodule kunt u een aangepaste API-aanroep uitvoeren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Voor instructies over het aansluiten van uw [Fusion App]-account op [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Een pad invoeren ten opzichte van <code>https://sheets.googleapis.com/v4/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van de aanvraag toe in de vorm van een standaard JSON-object. Bijvoorbeeld: <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] Hiermee voegt u de machtigingsheaders voor u toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Voeg de query voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:   <p>Bij het gebruik van voorwaardelijke instructies zoals <code>if</code> in uw JSON, plaats de aanhalingstekens buiten de voorwaardelijke verklaring.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Zoekopdrachten

* [[!UICONTROL Search Rows]](#search-rows)
* [[!UICONTROL Search Rows (Advanced)]](#search-rows-advanced)
* [[!UICONTROL Get Range Values]](#get-range-values)
* [[!UICONTROL List Sheets]](#list-sheets)

### [!UICONTROL Search Rows]

Hiermee doorzoekt u rijen met de filteropties.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [Fusion App]-account op [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Verbinding maken met [!DNL Adobe Workfront Fusion] - Basisinstructies</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Selecteer [!DNL Google] spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Selecteer het blad waarin u de rijen wilt doorzoeken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Table contains headers]</td> 
   <td> <p> Selecteer of het spreadsheet de kopbalrij bevat. Als de [!UICONTROL Yes] Als deze optie is geselecteerd, haalt de module de koptekstrij niet op als uitvoergegevens en worden de namen van variabelen in de uitvoer vervolgens aangeroepen door de koppen. Als de [!UICONTROL No] wordt geselecteerd, dan wint de module ook de eerste lijstrij terug en de veranderlijke namen in de output worden dan geroepen enkel A, B, C, D, etc.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Column range]</td> 
   <td>Selecteer het kolombereik waarmee u wilt werken. Voorbeeld: <code>A-F</code></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>Stel het filter in voor de rij waarop moet worden gezocht.</p> <p>Zie voor meer informatie over filters <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Een filter toevoegen aan een scenario in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sort order]</td> 
   <td>Selecteer of u oplopend of aflopend wilt sorteren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Order by]</td> 
   <td>Kies de kolom waarop u wilt sorteren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Formatted value]</p> <p>De waarden worden berekend en opgemaakt in de reactie volgens de opmaak van de cel. Opmaak is gebaseerd op de landinstelling van het werkblad, niet op de landinstelling van de gebruiker die het verzoek indient. Als <code>A1</code> is <code>1.23</code> en <code>A2</code> is <code>=A1</code> en worden opgemaakt als valuta, en vervolgens <code>A2</code> zou terugkeren <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Unformatted value]</p> <p>De waarden worden berekend, maar niet opgemaakt in de reactie. Als <code>A1</code> is <code>1.23</code> en <code>A2</code> is <code>=A1</code> en worden opgemaakt als valuta, en vervolgens <code>A2</code> retourneert het getal <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formula]</p> <p>De waarden worden niet berekend. Het antwoord zal ook de formules bevatten. Als <code>A1</code> is <code>1.23</code> en <code>A2</code> is <code>=A1</code> en worden opgemaakt als valuta, en vervolgens <code>A2</code> zou terugkeren <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Serial number]</p> <p>Geeft velden voor datum, tijd, datum en tijd de opdracht om te worden uitgevoerd als dubbele cijfers in de notatie "serienummer", zoals gevuld door Lotus 1-2-3. Het gehele getalgedeelte van de waarde (links van het decimaalteken) telt de dagen sinds 30 december 1899. Het fractionele gedeelte (rechts van het decimaalteken) telt de tijd als een fractie van de dag. Bijvoorbeeld, zou 1 januari 1900 om 12.00 uur 2.5 zijn, 2 omdat het 2 dagen na 30 december 1899 is, en 0.5 omdat 12.00 uur een halve dag is. 1 februari 1900 om 15.00 uur is 33.625 uur. Dit is een goede manier om het jaar 1900 te beschouwen als geen schrikkeljaar.</p> <p style="font-weight: bold;">[!UICONTROL Formatted string]</p> <p>Hiermee worden datum-, tijd-, datum- en duurvelden geïnstrueerd als tekenreeksen in de opgegeven getalnotatie (die afhankelijk is van de landinstelling van het werkblad).</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned rows]</td> 
   <td>Het maximum aantal rijen instellen [!DNL Workfront Fusion] wordt tijdens één uitvoeringscyclus geretourneerd.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Search Rows (Advanced)]

Geeft resultaten die overeenkomen met de opgegeven criteria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Sheets] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Selecteer de Google-spreadsheet die het vel bevat dat u wilt zoeken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Selecteer het blad met de rijen die u wilt doorzoeken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query]</td> 
   <td> <p>Gebruik de [!DNL Google Charts Query Language]. Voorbeeld: <code>select * where B = "John"</code></p> <p>Voor meer informatie over [!DNL Google Charts Query Language], zie <a href="https://developers.google.com/chart/interactive/docs/querylanguage">Zoektaalnaslag</a> in de [!DNL Google] documentatie.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Get Range Values]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Sheets] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Selecteer [!DNL Google] spreadsheet.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sheet] </td> 
   <td> <p>Selecteer het blad waarvan u de bereikinhoud wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Range] </td> 
   <td> <p>Voer het bereik in dat u wilt ophalen. Voorbeeld: <code>A1:D25</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Table contains headers]</td> 
   <td> <p>Schakel dit vakje in als het blad een koptekstrij heeft</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Row with headers]</td> 
   <td>Voer het bereik van de tabelkoppen in. Voorbeeld <code>A1:F1</code>. Als u het veld leeg laat, [!DNL Workfront Fusion] zal veronderstellen dat de kopbal in de eerste rij van de gespecificeerde waaier is.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Value render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Formatted value]</p> <p>De waarden worden berekend en opgemaakt in de reactie volgens de opmaak van de cel. Opmaak is gebaseerd op de landinstelling van het werkblad, niet op de landinstelling van de gebruiker die het verzoek indient. Als <code>A1</code> is <code>1.23</code> en <code>A2</code> is <code>=A1</code> en worden opgemaakt als valuta, en vervolgens <code>A2</code> zou terugkeren <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Unformatted value]</p> <p>De waarden worden berekend, maar niet opgemaakt in de reactie. Als <code>A1</code> is <code>1.23</code> en <code>A2</code> is <code>=A1</code> en worden opgemaakt als valuta, en vervolgens <code>A2</code> retourneert het getal <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL Formula]</p> <p>De waarden worden niet berekend. Het antwoord zal ook de formules bevatten. Als <code>A1</code> is <code>1.23</code> en <code>A2</code> is <code>=A1</code> en worden opgemaakt als valuta, en vervolgens <code>A2</code> zou terugkeren <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL Serial number]</p> <p>Geeft velden voor datum, tijd, datum en tijd de opdracht om te worden uitgevoerd als dubbele cijfers in de notatie "serienummer", zoals gevuld door Lotus 1-2-3. Het gehele getalgedeelte van de waarde (links van het decimaalteken) telt de dagen sinds 30 december 1899. Het fractionele gedeelte (rechts van het decimaalteken) telt de tijd als een fractie van de dag. Bijvoorbeeld, zou 1 januari 1900 om 12.00 uur 2.5 zijn, 2 omdat het 2 dagen na 30 december 1899 is, en 0.5 omdat 12.00 uur een halve dag is. 1 februari 1900 om 15.00 uur is 33.625 uur. Dit is een goede manier om het jaar 1900 te beschouwen als geen schrikkeljaar.</p> <p style="font-weight: bold;">[!UICONTROL Formatted string]</p> <p>Hiermee worden datum-, tijd-, datum- en duurvelden geïnstrueerd als tekenreeksen in de opgegeven getalnotatie (die afhankelijk is van de landinstelling van het werkblad).</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL List Sheets]

Deze module retourneert een lijst met alle bladen in een spreadsheet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Google Sheets] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Spreadsheet] </td> 
   <td> <p>Selecteer [!DNL Google] werkblad dat de bladen bevat die u wilt weergeven.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Gebruiksbeperkingen

Als de fout `429: RESOURCE_EXHAUSTED` voorkomt, hebt u de limiet van de API-snelheid overschreden.

De [!DNL Google Sheets] API heeft een grens van 500 verzoeken per 100 seconden per project, en 100 verzoeken per 100 seconden per gebruiker. Limieten voor lezen en schrijven worden afzonderlijk bijgehouden. Er is geen dagelijkse gebruikslimiet.

Meer informatie vindt u op [developers.google.com/sheets/api/limits](https://developers.google.com/sheets/api/limits).

## Tips en trucs

* [Lege cellen ophalen van een [!DNL Google] Werkblad](#how-to-get-empty-cells-from-a-google-sheet)
* [Voeg een knoop in een blad toe om een scenario in werking te stellen](#add-a-button-in-a-sheet-to-run-a-scenario)

### Lege cellen ophalen van een [!DNL Google Sheet]

Gebruik de [!UICONTROL Search Rows (Advanced)] en gebruik deze formule om de kolommen op te halen die leeg zijn.
<pre>select * waarbij E null is</pre>Hier is "E"de kolom &amp; "is ongeldig"de voorwaarde. U kunt een geavanceerdere query maken met [Google Query Lang] (https://developers.google.com/chart/interactive/docs/querylanguage).

### Voeg een knoop in een blad toe om een scenario in werking te stellen

1. In [!DNL Workfront Fusion], voegt de **[!UICONTROL Webhook]** > **[!UICONTROL Custom webhooks]** module/trekker in het scenario en vorm het (zie [Webhaken](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)).

1. Kopieer de URL van de webhaak.
1. Voer het scenario uit.
1. Kies in Google-bladen de optie **[!UICONTROL Insert]** > **[!UICONTROL Drawing]**... in de hoofdmenubalk.

1. In de [!UICONTROL Drawing] venster, klik op **[!UICONTROL Text box]** pictogram ![](assets/text-box.png) boven in het venster.
1. Een knop ontwerpen en op de knop klikken **[!UICONTROL Save and Close]** in de rechterbovenhoek:
1. De knop wordt in uw werkblad geplaatst. Klik op de drie verticale stippen in de rechterbovenhoek van de knop:
1. Kies **[!UICONTROL Assign script..].** in het menu.
1. Voer de naam van het script (functie) in, bijvoorbeeld `runScenario` en klik op **[!UICONTROL OK]**:
1. Kies **[!UICONTROL Tools]** > **[!UICONTROL Script editor]** in de hoofdmenubalk.

1. Voeg de volgende code in:

   * De naam van de functie moet overeenkomen met de naam die u in stap 9 hebt opgegeven.
   * Vervang de URL door de URL van de webhaak die u in stap 2 hebt gekopieerd.

     <pre>function runScenario() {</pre><pre>UrlFetchApp.fetch("<webhook you copied>");</pre><pre>}</pre>

1. Druk **[!UICONTROL Ctrl+S]** om het manuscriptdossier te bewaren, ga een projectnaam in en klik **[!UICONTROL OK]**.

1. Terug naar [!DNL Google Sheets] en klik op de nieuwe knop.
1. Verleen de vereiste toestemming aan het manuscript:
1. In [!DNL Workfront Fusion]controleert u of het scenario met succes is uitgevoerd.

## Datums opslaan in een spreadsheet

Als u een Date-waarde opslaat in een spreadsheet zonder opmaak, wordt deze waarde in de spreadsheet weergegeven als tekst in de ISO 8601-indeling. Maar [!DNL Google Sheets] formules of functies die werken met datums die deze tekst niet begrijpen (voorbeeld: formule `=A1+10`) wordt de volgende fout weergegeven:

![](assets/mceclip6-350x87.png)

Help toestaan [!DNL Google Sheets] om de datum te begrijpen, formatteer het met [[!UICONTROL formatDate] (datum; formaat; [tijdzone])](../../workfront-fusion/functions/date-and-time-functions.md#formatda) functie. De juiste indeling die als het tweede argument aan de functie wordt doorgegeven, is afhankelijk van de landinstellingen van het werkblad.

U kunt als volgt de juiste indeling bepalen:

1. Kies **[!UICONTROL File]** > **[!UICONTROL Spreadsheet]** instellingen in het hoofdmenu om de landinstelling te controleren of in te stellen.

1. Nadat u de juiste landinstelling hebt gecontroleerd of ingesteld, bepaalt u de corresponderende datum- en tijdnotatie door **[!UICONTROL Format]** > **[!UICONTROL Number]** in het hoofdmenu. De notatie wordt weergegeven naast de menuoptie Datum en tijd:

1. Om het correcte formaat samen te stellen dat tot zou moeten worden overgegaan [!UICONTROL formatDate()] functie, verwijs naar de lijst van [Tokens voor datum- en tijdnotaties in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md).

**Voorbeeld:** Het gebruik van `MM/DD/YYYY HH:mm:ss` notatie voor de landinstelling Verenigde Staten:

![](assets/locale-time-350x83.png)

## Exploderen [!DNL Google Sheets] functies

Als u een ingebouwde functie mist, maar het wordt voorzien van door [!DNL Google Sheets], kunt u er misbruik van maken. Zie voor meer informatie [Gebruiken [!DNL Google Sheets] functies](../../workfront-fusion/functions/map-using-functions.md#exploiti) in [Items toewijzen met behulp van functies in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md) .

## Behouden [!DNL Google Sheets] van het wijzigen van getallen in datums

U zult merken dat een reeks getallen die u als tekst gebruikt, wordt geïnterpreteerd als een datum in een [!DNL Google] werkblad. U typt bijvoorbeeld 1-2019, waarbij u het als tekst wilt gebruiken, maar Google interpreteert het als een datum. U kunt het nummer vooraf opmaken als normale tekst om dit te voorkomen.

1. In [!DNL Google Sheets]markeert u de kolom of cel met het nummer of de nummers.
1. Klik op **[!UICONTROL Format]** > **[!UICONTROL Number]** > **[!UICONTROL Plain text]**.

Een andere oplossing in [!DNL Workfront Fusion] moet een apostrof (&#39;) vóór een getal typen, bijvoorbeeld &#39;1-2019 of &#39;1/47. De apostrof wordt niet weergegeven in de cel nadat de gegevens zijn verzonden vanuit [!DNL Workfront Fusion].
