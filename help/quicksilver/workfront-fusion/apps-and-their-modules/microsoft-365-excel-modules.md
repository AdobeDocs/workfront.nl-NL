---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 Excel-modules
description: In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema's automatiseren die Microsoft 365 Excel gebruiken, evenals het verbinden met veelvoudige derdetoepassingen en de diensten.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 9aa3739d-6800-4eb1-a17f-32fdfd8ed0f2
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2194'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Excel] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!DNL Microsoft 365 Excel]en deze verbinding maken met meerdere toepassingen en services van derden.

Als u instructies bij het creëren van een scenario nodig hebt, zie [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Voor informatie over modules, zie [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Vereisten

Te gebruiken [!DNL Microsoft office 365 Excel], je moet een Microsoft-account hebben.

## [!DNL Microsoft Office 365 Excel] modules en hun velden

Wanneer u [!DNL Microsoft 365 Excel] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Microsoft 365 Excel] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Werkboek](#workbook)
* [Werkblad](#worksheet)
* [Tabel](#table)
* [Overige](#other)

### Werkboek

* [Werkboeken controleren](#watch-workbooks)
* [Werkboeken zoeken](#search-workbooks)
* [Een werkboek downloaden](#download-a-workbook)

#### [!UICONTROL Watch Workbooks]

Deze trekkermodule begint een scenario wanneer een werkboek wordt gecreeerd.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p>Selecteer de map die u wilt controleren voor nieuwe werkboeken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>U kunt een filter instellen om alleen te controleren op werkboeken die voldoen aan de criteria die u selecteert.</p> <p>Voer voor elk filter het veld in dat door het filter moet worden geëvalueerd, de operator en de waarde die door het filter moet worden toegestaan. U kunt meer dan één filter gebruiken door EN of OF regels toe te voegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal werkboeken in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search Workbooks]

In deze actiemodule wordt gezocht naar [!DNL Excel] werkboeken.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p>Selecteer de map die u wilt zoeken naar werkboeken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>U kunt een filter plaatsen om naar slechts werkboeken te zoeken die aan criteria voldoen u selecteert.</p> <p>Voer voor elk filter het veld in dat door het filter moet worden geëvalueerd, de operator en de waarde die door het filter moet worden toegestaan. U kunt meer dan één filter gebruiken door EN of OF regels toe te voegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ga of kaart het maximumaantal aantekenvellen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download a Workbook]

Deze actiemodule downloadt de inhoud van het gespecificeerde werkboek van Excel.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Download a workbook]</td> 
   <td> <p>Selecteer hoe u het werkboek voor de module wilt identificeren om te downloaden.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL By entering an ID manually]</strong> </p> <p>In de [!UICONTROL Workbook ID] gebied, ga of kaart identiteitskaart van het specifieke werkboek in dat u de module wilt downloaden.</p> </li> 
     <li> <p><strong>[!UICONTROL By selecting from the path]</strong> </p> <p>In de [!UICONTROL Workbook] gebied, selecteer het werkboek dat u de module wilt downloaden.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Werkblad

* [[!UICONTROL Watch Worksheet Rows]](#watch-worksheet-rows)
* [[!UICONTROL List Worksheets]](#list-worksheets)
* [[!UICONTROL List Worksheet Rows]](#list-worksheet-rows)
* [[!UICONTROL Add a Worksheet]](#add-a-worksheet)
* [[!UICONTROL Add a Worksheet Row]](#add-a-worksheet-row)
* [[!UICONTROL Update a Worksheet Row]](#update-a-worksheet-row)
* [[!UICONTROL Delete a Worksheet Row]](#delete-a-worksheet-row)

#### [!UICONTROL Watch Worksheet Rows]

Deze triggermodule start een scenario wanneer een nieuwe rij aan het werkblad wordt toegevoegd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Selecteer het werkboek dat het aantekenvel bevat u op nieuwe rijen wilt letten.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Selecteer het Excel-werkblad waarop u nieuwe rijen wilt controleren.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Ga of kaart het maximumaantal aantekenvelrijen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Worksheets]

Deze actiemodule wint een lijst van aantekenvellen in het gespecificeerde werkboek terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Selecteer het werkboek dat de aantekenvellen bevat die u de module aan lijst wilt.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Ga of kaart het maximumaantal aantekenvellen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Worksheet Rows]

Deze actiemodule wint een lijst van rijen in het gespecificeerde aantekenvel terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Selecteer het werkboek dat het aantekenvel bevat dat de rijen omvat u wilt een lijst maken.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Selecteer het werkblad met de rijen die u wilt weergeven.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Ga of kaart het maximumaantal aantekenvelrijen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add a Worksheet]

Deze actiemodule leidt tot een nieuw aantekenvel binnen het geselecteerde werkboek.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Selecteer het werkboek waar u een aantekenvel wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Name] </td>
   <td> <p>Voer een naam voor het nieuwe werkblad in of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add a Worksheet Row]

Deze actiemodule voegt een nieuwe rij toe aan het geselecteerde werkblad.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Selecteer het werkboek dat het aantekenvel bevat waar u een rij wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Selecteer het werkblad waaraan u een rij wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type of values being entered]</p> </td> 
   <td> <p>Selecteer het type waarde dat u in het werkblad wilt invoeren. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formulas]</strong> </p> <p> Excel probeert de opgegeven expressie te evalueren. De namen van functies in een formule zijn in het Engels. Voorbeeld: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formulas local]</strong> </p> <p>Excel probeert de opgegeven expressie te evalueren. De functienamen zijn in de taal van uw toepassing van Excel. Voorbeeld: <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Excel evalueert de waarde niet. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>Voer voor elke kolom de waarde in die de kolom in de nieuwe rij moet hebben.</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a Worksheet Row]

Deze actiemodule werkt een bestaande werkbladrij bij.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Selecteer het werkboek dat het aantekenvel bevat dat de rij omvat u wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Selecteer het werkblad dat de rij bevat die u wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type of values being entered]</p> </td> 
   <td> <p>Selecteer het type waarde dat u in het werkblad wilt invoeren. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formulas]</strong> </p> <p> Excel probeert de opgegeven expressie te evalueren. De namen van functies in een formule zijn in het Engels. Voorbeeld: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formulas local]</strong> </p> <p>Excel probeert de opgegeven expressie te evalueren. De functienamen zijn in de taal van uw toepassing van Excel. Voorbeeld: <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Excel evalueert de waarde niet. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Row ID]</td> 
   <td>Selecteer het nummer van de rij dat u wilt bijwerken.</td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>Voer voor elke kolom de waarde in die de kolom in de nieuwe rij moet hebben.</td>
   --&gt; 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Worksheet Row]

Met deze actiemodule verwijdert u een rij uit een werkblad.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Selecteer het werkboek dat het aantekenvel bevat dat de rij omvat u wilt schrappen.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet]</td>
   <td> <p> Selecteer het werkblad dat de rij bevat die u wilt verwijderen.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row ID]</td>
   <td>Voer de id in van de rij die u wilt verwijderen of wijs deze toe.</td> 
  </tr> 
 </tbody> 
</table>

### Tabel

* [[!UICONTROL Watch table rows]](#watch-table-rows)
* [[!UICONTROL List tables]](#list-tables)
* [[!UICONTROL List table rows]](#list-table-rows)
* [[!UICONTROL Get a Table]](#get-a-table)
* [[!UICONTROL Add a table]](#add-a-table)
* [[!UICONTROL Add a table row]](#add-a-table-row)
* [[!UICONTROL Update a table]](#update-a-table)
* [[!UICONTROL Delete a table]](#delete-a-table)

#### [!UICONTROL Watch table rows]

Deze trigger start een scenario wanneer een nieuwe rij aan een tabel wordt toegevoegd.

>[!NOTE]
>
>De tabel verwijst hier naar het ingesloten tabelelement in het werkboek. Niet de volledige tabel (werkboek/werkblad).

![](assets/embedded-table-350x420.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Workbook]</p> </td> 
   <td> <p>Selecteer het werkboek dat de lijst bevat u wilt letten op.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p> Selecteer het werkblad dat de tabel bevat die u wilt bekijken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Table]</p> </td> 
   <td> <p>Selecteer de tabel die u wilt bekijken.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Ga of kaart het maximumaantal rijen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List tables]

Deze zoekmodule haalt een lijst met alle tabelobjecten op.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Selecteer het werkboek dat de lijsten bevat u wilt een lijst maken.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Selecteer het werkblad dat de tabellen bevat die u wilt weergeven</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Ga of kaart het maximumaantal lijsten in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List table rows]

Deze onderzoeksmodule wint een lijst van alle lijstrijen in een werkboek terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Selecteer het werkboek dat de lijst bevat die de rijen omvat u wilt een lijst maken.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Selecteer het werkblad dat de tabel bevat met de rijen die u wilt weergeven</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Table] </td>
   <td> <p>Selecteer de tabel die de rijen bevat die u wilt weergeven.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Ga of kaart het maximumaantal lijstrijen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Table]

Deze actiemodule wint meta-gegevens voor de gespecificeerde lijst terug.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
     <p >[!UICONTROL Connection]</p>
   </td> 
   <td> 
     <p>Voor instructies over het aansluiten van uw Office 365-account op [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p>
    --&gt; </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get a table]</td> 
   <td> <p>Selecteer hoe u de tabel wilt identificeren die u wilt ophalen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>In de [!UICONTROL Workbook ID] gebied, ga of kaart identiteitskaart van het werkboek in dat de lijst bevat u wilt terugwinnen.</p> <p>In de [!UICONTROL Table Name] Voer de naam in van de tabel die u wilt ophalen.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Selecteer het werkboek en het aantekenvel die de lijst bevatten u wilt terugwinnen, dan de lijst selecteren.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add a table]

Deze actiemodule leidt tot een lijstelement binnen het aantekenvel van Excel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workbook] </td> 
   <td> <p>Selecteer het werkboek dat het aantekenvel bevat waar u een lijst wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Worksheet] </td> 
   <td> <p>Selecteer het werkblad waaraan u een tabel wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Has headers]</td> 
   <td> <p>Schakel deze optie in om de eerste rij als tabelkoppen te definiëren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Address]</p> </td> 
   <td> <p>Stel de grootte van de tabel in door de cellen linksboven en rechtsonder aan te geven. Voorbeeld: <code>A1:C10</code> Hiermee maakt u een tabel met 3 kolommen en 10 rijen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add a table row]

Deze actiemodule wijzigt een bestaande tabel.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Selecteer het werkboek dat de lijst bevat waar u een rij wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Selecteer het werkblad dat de tabel bevat waarin u een rij wilt toevoegen.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Table]</td>
   <td>Selecteer de tabel waaraan u een rij wilt toevoegen.</td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>Voer voor elke kolom de waarde in die de kolom in de nieuwe rij moet hebben.</td>
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Row ID]</p> </td> 
   <td> <p>Als u een rij wilt toevoegen op een specifieke locatie in de tabel, voert u een rijnummer in of wijst u dit toe. De module neemt de nieuwe rij na deze rij op.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a table]

Deze actiemodule werkt een bestaande tabel bij.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Update a table]</td> 
   <td> <p>Selecteer hoe u de tabel wilt identificeren die u wilt bijwerken.</p> 
    <ul> 
     <li> <p><strong>Handmatig invoeren</strong> </p> <p>In de [!UICONTROL Workbook ID] gebied, ga identiteitskaart van het werkboek in of kaart die de lijst bevat u wilt bijwerken.</p> <p>In de [!UICONTROL Table Name] voert u de naam in van de tabel die u wilt bijwerken.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Selecteer het werkboek en het aantekenvel die de lijst bevatten u wilt bijwerken, dan de lijst selecteren.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table] </td> 
   <td> <p>Selecteer de tabel die u wilt bijwerken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td> <p>Als u de naam van de tabel wilt wijzigen, voert u een nieuwe naam voor de tabel in of wijst u deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show Headers]</td> 
   <td> <p>Schakel deze optie in om de koppen van de bijgewerkte tabel weer te geven.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show totals]</td> 
   <td>Schakel deze optie in om de totale waarden van de tabel weer te geven.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Style]</td> 
   <td>Kies een stijl voor de nieuwe tabel.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a table]

Met deze actiemodule verwijdert u de opgegeven tabel uit een [!DNL Excel] werkblad.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get a table]</td> 
   <td> <p>Selecteer hoe u de tabel wilt identificeren die u wilt verwijderen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>In de [!UICONTROL Workbook ID] gebied, ga identiteitskaart van het werkboek in of kaart die de lijst bevat u wilt schrappen.</p> <p>In de [!UICONTROL Table Name] Voer de naam in van de tabel die u wilt verwijderen.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Selecteer het werkboek en het aantekenvel die de lijst bevatten u wilt schrappen, dan de lijst selecteren.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Overige

* [[!UICONTROL Retrieve data]](#retrieve-data)
* [[!UICONTROL Make an API Call]](#make-an-api-call)

#### [!UICONTROL Retrieve data]

Deze actie wint gegevens van de bepaalde aantekenvelwaaier terug, en keert een bundel voor elke rij terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workbook] </td> 
   <td> <p>Selecteer het werkboek dat de gegevens bevat u wilt terugwinnen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Worksheet] </td> 
   <td> <p>Selecteer het werkblad met de gegevens die u wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Range] </td> 
   <td> <p>Geef het gebied van het blad op waarvan u de gegevens wilt ophalen door de cellen linksboven en rechtsonder aan te geven. Voorbeeld: <code>A1:D10</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Make an API Call]

Met deze actiemodule kunt u een aangepaste API-aanroep maken.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Office 365] account aan [!DNL Workfront Fusion], zie <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Sluit de app of webservice van de module aan op [!DNL Workfront Fusion]</a> in het artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Een scenario maken in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Een pad invoeren ten opzichte van <code>https://graph.microsoft.com</code>. Voorbeeld:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion voegt de machtigingsheaders voor u toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Voeg de query voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"name":"something-urgent"}</code></p> </td> 
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
