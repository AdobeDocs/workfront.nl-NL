---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Berekende aangepaste velden versus berekende kolommen
description: Meer informatie over aangepaste gegevens in rapporten en dashboards
author: Nolan
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# Berekende aangepaste velden versus berekende kolommen

Als u meerdere velden in Adobe Workfront wilt samenvoegen en die geaggregeerde waarde wilt weergeven in een nieuw veld, kunt u het volgende doen:

* Een berekend aangepast veld in een aangepast formulier\
  Zie de sectie voor meer informatie over het toevoegen van een berekend aangepast veld aan een aangepast formulier [Een berekend veld toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#creating-calculated-custom-fields) in het artikel [Berekende gegevens toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* Een berekende kolom in een weergave\
  Zie de sectie voor meer informatie over het gebruik van berekeningen in een weergave [Tekstmodus gebruiken in weergaven](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#using-text-mode-in-views) in het artikel [Overzicht van veelvoorkomende toepassingen voor de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Hoewel u de tekstmodus gebruikt om zowel berekende velden als berekende kolommen samen te stellen, verschilt de syntaxis voor het samenstellen van deze velden. Raadpleeg de bovenstaande artikelen voor meer informatie over het bouwen van berekende velden en berekende kolommen. Zie de sectie voor informatie over de verschillende syntaxis die wordt gebruikt in berekende gegevensexpressies, zoals berekende aangepaste velden en kolommen [Syntaxis van berekende aangepaste velden versus berekende aangepaste kolommen](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns-syntax) in dit artikel.

U kunt dezelfde berekeningen gebruiken in beide berekende velden en in een berekende kolom. Afhankelijk van wat uw doel voor deze berekeningen is, kunt u echter overwegen om het ene versus het andere te bouwen.

## Syntaxis van berekende aangepaste velden versus berekende aangepaste kolommen

Hoewel de functies die u gebruikt hetzelfde zijn, kan de syntaxis voor het bouwen van een expressie in een berekend aangepast veld anders zijn dan voor het bouwen van een berekende aangepaste kolom.

Bijvoorbeeld:

* In een aangepast veld gebruikt u op een aangepast formulier voor taken de volgende opties om de naam te genereren van het bovenliggende project van de taak waaraan het aangepaste formulier is gekoppeld:

  ```
  {project}.{name}
  ```

* In een douanekolom in een rapport, zou u het volgende gebruiken om een de douanekolom van de Naam van het Project op een taakrapport toe te voegen:

  ```
  valuefield=project:name
  ```

  of

  ```
  valueexpression={project}.{name}
  ```

  >[!TIP]
  >
  >Dezelfde syntaxis is van toepassing op alle rapportelementen in de tekstmodus waarvoor berekende expressies worden gebruikt: weergaven, filters, groepen en aanwijzingen.

De verschillen tussen de twee syntaxis zijn als volgt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Berekend aangepast veld</td> 
   <td>Berekend aangepast rapporteringselement</td> 
  </tr> 
  <tr> 
   <td> <p>Gebruik de naam van de velden zoals deze worden weergegeven in de Workfront-interface.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span>Voorbeeld van een veldnaam die in een berekend aangepast veld wordt gebruikt: <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Gebruik de naam van de objecten of velden zoals deze worden weergegeven in de Workfront-database. De namen van objecten en velden worden in kleine letters of hoofdletters gespeld, als het samengestelde namen betreft. </p> <p>Voor een overzicht van alle Workfront-objecten en -velden die in de database worden weergegeven, raadpleegt u <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Voorbeeld: </b></span></span>Voorbeeld van een veldnaam die wordt gebruikt in een berekend aangepast rapporteringselement: <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Veldnamen tussen haakjes of accolades plaatsen</td> 
   <td> <p>Veldnamen tussen haakjes of haakjes plaatsen wanneer u ze in een <code>valuefield </code>lijn.</p> <p>Veldnamen tussen accolades plaatsen wanneer ze worden gebruikt in een <code>valueexpression</code> lijn.</p> </td> 
  </tr> 
  <tr> 
   <td>De velden scheiden met punten</td> 
   <td> <p>De velden scheiden met dubbele punten wanneer u ze in een <code>valuefield </code>line</p> <p>De velden van elkaar scheiden op punten wanneer u ze in een <code>valueexpression </code>lijn. </p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie over de syntaxis moet u in een berekende douanekolom gebruiken, zie [Overzicht van de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Wanneer moeten berekende aangepaste velden worden gebruikt

* Wanneer u de samengevoegde resultaten in een rapport wilt groeperen of u wilt deze informatie in een grafiek tonen
* Wanneer u de gegevens buiten de aggregatie wilt samenvoegen die in het veld wordt berekend
* Wanneer u niet bezorgd bent over de tijdigheid van de gegevens, aangezien de gegevens niet worden bijgewerkt en het in tijd kan veranderen

## Handelingen die de update van een berekend aangepast veld activeren

* Klik op het pictogram Meer op de hoofdpagina van een object ![](assets/more-icon.png)en klik vervolgens op **Expressies opnieuw berekenen**

* Bulk die meerdere objecten bewerkt wanneer **Aangepaste expressies opnieuw berekenen** is ingeschakeld
* Een aangepast formulier bewerken wanneer **Vorige berekeningen bijwerken** is ingeschakeld voor het berekende aangepaste veld

## Wanneer gebruikt u Berekende kolommen in een weergave

* Wanneer u gegevens in real time op een rapport beschikbaar wilt zijn.

  De berekende meningen zijn altijd vers omdat de berekening wordt gemaakt wanneer het rapport in werking wordt gesteld of de mening wordt toegepast.

* Wanneer u geen plannen hebt om door samengevoegde resultaten te groeperen noch deze informatie in een grafiek te gebruiken.
* Wanneer u niet van plan bent om de gegevens voorbij de samenvoeging samen te voegen die in de kolom wordt berekend (de gegevens kunnen slechts eenmaal worden samengevoegd).
* Als u wilt dat de berekening een verwijzing naar de huidige datum bevat met de jokertekens $$TODAY of $$NOW.

  >[!TIP]
  >
  >Gebruik deze verwijzing niet in berekende aangepaste velden omdat deze alleen opnieuw wordt berekend wanneer het gekoppelde object wordt bewerkt. Deze typen berekeningen zijn achterhaald.

## Voorbeelden van berekende aangepaste velden en kolommen

Zie voor voorbeelden van berekende aangepaste velden [Berekende aangepaste gegevens in rapporten](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Zie de volgende artikelen voor voorbeelden van berekende aangepaste kolommen in weergaven:

* [Overzicht van veelvoorkomende toepassingen voor de tekstmodus](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [Voorbeelden van aangepaste weergaven, filters en groeperingen](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
