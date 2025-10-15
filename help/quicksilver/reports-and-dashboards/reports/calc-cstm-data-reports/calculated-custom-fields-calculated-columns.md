---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Berekende aangepaste velden versus berekende kolommen
description: Als u meerdere velden in Adobe Workfront wilt samenvoegen en die geaggregeerde waarde wilt weergeven in een nieuw veld, kunt u een berekend aangepast veld maken in een aangepast formulier of een berekende kolom in een weergave.
author: Jenny
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Berekende aangepaste velden versus berekende kolommen

Als u meerdere velden in Adobe Workfront wilt samenvoegen en die geaggregeerde waarde wilt weergeven in een nieuw veld, kunt u het volgende maken:

* Een berekend aangepast veld in een aangepast formulier\
  Voor meer informatie over het toevoegen van een berekend douanegebied aan een douanevorm, zie [ berekende gebieden aan een vorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) toevoegen.

* Een berekende kolom in een weergave\
  Voor meer informatie over het gebruiken van berekeningen in een mening, zie de sectie [ Wijze van de Tekst van het Gebruik in meningen ](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#use-text-mode-in-views) in het artikel [ Overzicht van gemeenschappelijk gebruik voor de Wijze van de Tekst ](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

Hoewel u de tekstmodus gebruikt om zowel berekende velden als berekende kolommen samen te stellen, verschilt de syntaxis voor het samenstellen van deze velden. Raadpleeg de bovenstaande artikelen voor meer informatie over het bouwen van berekende velden en berekende kolommen. Voor informatie over de verschillende syntaxis die in berekende gegevensuitdrukkingen zoals berekende douanegebieden en kolommen wordt gebruikt, zie de sectie [ Syntaxis van berekende douanegebieden vs. berekende douanekolommen ](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) in dit artikel.

U kunt dezelfde berekeningen gebruiken in beide berekende velden en in een berekende kolom. Afhankelijk van wat uw doel is voor deze berekeningen, kunt u echter overwegen om een voor een te bouwen.

## Syntaxis van berekende aangepaste velden versus berekende aangepaste kolommen

Hoewel de functies die u gebruikt hetzelfde zijn, kan de syntaxis voor het bouwen van een expressie in een berekend aangepast veld anders zijn dan voor het bouwen van een berekende aangepaste kolom.

Bijvoorbeeld:

* In een aangepast veld gebruikt u op een aangepast formulier voor taken de volgende opties om de naam te genereren van het bovenliggende project van de taak waaraan het aangepaste formulier is gekoppeld:

  `{project}.{name}`

* In een douanekolom in een rapport, zou u het volgende gebruiken om een de douanekolom van de Naam van het Project op een taakrapport toe te voegen:

  `valuefield=project:name`

  of

  `valueexpression={project}.{name}`

  >[!TIP]
  >
  >Dezelfde syntaxis is van toepassing op alle rapportelementen in de tekstmodus waarvoor berekende expressies worden gebruikt: weergaven, filters, groeperingen en aanwijzingen.

De verschillen tussen de twee syntaxis zijn als volgt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Berekend aangepast veld</strong></td>
   <td><strong>Berekend aangepast rapporteringselement</strong></td> 
  </tr> 
  <tr> 
   <td> <p>Gebruik de naam van de velden zoals deze worden weergegeven in de Workfront-interface.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b> Voorbeeld: </b></span></span> Voorbeeld van gebiedsnaam die op een berekend douanegebied wordt gebruikt: <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>Gebruik de naam van de objecten of velden zoals deze worden weergegeven in de Workfront-database. De namen van objecten en velden worden in kleine letters of hoofdletters gespeld, als het samengestelde namen betreft. </p> <p>Voor een inventaris van alle voorwerpen en gebieden van Workfront aangezien zij in het gegevensbestand verschijnen, zie <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref"> API Ontdekkingsreiziger </a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b> Voorbeeld: </b></span></span> Voorbeeld van gebiedsnaam die in een berekend douanerapporteringselement wordt gebruikt: <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Veldnamen tussen haakjes of accolades plaatsen</td> 
   <td> <p>Sluit geen gebiedsnamen in steunen of haakjes in wanneer het gebruiken van hen in a <code>valuefield </code> lijn.</p> <p>Plaats veldnamen tussen accolades wanneer u ze op een <code>valueexpression</code> -regel gebruikt.</p> </td> 
  </tr> 
  <tr> 
   <td>De velden scheiden met punten</td> 
   <td> <p>Scheid de gebieden door dubbelepunten wanneer het gebruiken van hen in a <code>valuefield</code> lijn.</p> <p>Scheid de gebieden door periodes wanneer het gebruiken van hen in a <code>valueexpression</code> lijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie over de syntaxis moet u in een berekende douanekolom gebruiken, zie [ Overzicht van de Wijze van de Tekst ](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Wanneer moeten berekende aangepaste velden worden gebruikt

* Wanneer u de samengevoegde resultaten in een rapport wilt groeperen of u wilt deze informatie in een grafiek tonen
* Wanneer u de gegevens buiten de aggregatie wilt samenvoegen die in het veld wordt berekend
* Wanneer u niet bezorgd bent over de tijdigheid van de gegevens, aangezien de gegevens niet worden bijgewerkt en het in tijd kan veranderen

## Handelingen die de update van een berekend aangepast veld activeren

* Op de belangrijkste pagina van een voorwerp, klikkend het Meer pictogram ![ Meer pictogram ](assets/more-icon.png), dan klikkend **Uitdrukkingen** opnieuw berekenen

* Onk die veelvoudige voorwerpen uitgeven wanneer **de Uitdrukkingen van de Douane** opnieuw berekenen wordt toegelaten
* Het uitgeven van een douaneformulier wanneer **vorige berekeningen** bijwerken wordt toegelaten voor het berekende douanegebied

## Wanneer moeten berekende kolommen in een weergave worden gebruikt

* Wanneer u gegevens in real time op een rapport beschikbaar wilt zijn.

  De berekende meningen zijn altijd vers omdat de berekening wordt gemaakt wanneer het rapport in werking wordt gesteld of de mening wordt toegepast.

* Wanneer u geen plannen hebt om door samengevoegde resultaten te groeperen noch deze informatie in een grafiek te gebruiken.
* Wanneer u niet van plan bent om de gegevens voorbij de samenvoeging samen te voegen die in de kolom wordt berekend (de gegevens kunnen slechts eenmaal worden samengevoegd).
* Als u wilt dat de berekening een verwijzing naar de huidige datum bevat met de jokertekens $$TODAY of $$NOW.

  >[!TIP]
  >
  >Gebruik deze verwijzing niet in berekende aangepaste velden omdat deze alleen opnieuw wordt berekend wanneer het gekoppelde object wordt bewerkt. Deze typen berekeningen zijn achterhaald.

## Voorbeelden van berekende aangepaste velden en kolommen

Voor voorbeelden van berekende douanegebieden, zie [ Berekende douanegegevens in rapporten ](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

Raadpleeg de volgende artikelen voor voorbeelden van berekende aangepaste kolommen in weergaven:

* [ Overzicht van gemeenschappelijk gebruik voor de Wijze van de Tekst ](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [Voorbeelden van aangepaste weergaven, filters en groepen: artikelindex](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
