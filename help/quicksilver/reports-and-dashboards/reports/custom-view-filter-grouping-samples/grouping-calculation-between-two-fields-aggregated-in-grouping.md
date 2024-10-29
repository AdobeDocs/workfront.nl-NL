---
content-type: reference
product-area: reporting;projects
keywords: berekend,geaggregeerde,geavanceerde,weergaven
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groeperen: het resultaat weergeven van het samenvoegen van meerdere berekende waarden in een groepering'
description: U kunt de tekstmodus in een kolom gebruiken om een berekening weer te geven tussen twee velden in de weergave van een rapport of lijst. Op elke regel wordt de berekening voor elk object in het rapport of de lijst weergegeven.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Groeperen: het resultaat weergeven van het samenvoegen van meerdere berekende waarden in een groep

<!--Audited: 10/2024-->

U kunt de tekstmodus in een kolom gebruiken om een berekening weer te geven tussen twee velden in de weergave van een rapport of lijst. Op elke regel wordt de berekening voor elk object in het rapport of de lijst weergegeven.

U kunt bijvoorbeeld het verschil tussen Werkelijke uren en Geplande uren weergeven in een derde kolom met de naam Werkbalans voor elke taak in een taakrapport. Voor meer informatie over berekende gegevensuitdrukkingen, zie [ Overzicht van berekende gegevensuitdrukkingen ](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

U kunt de geaggregeerde waarde van meerdere berekende weergave-items in dezelfde kolom in een groep weergeven door een berekening toe te voegen aan de `aggregator` regel van de kolom die de berekende waarde bevat. U kunt bijvoorbeeld de hoeveelheid werkbalansuren van alle taken in de groep van het rapport of de lijst voor de kolom Werkbalans samenvoegen (weergeven). In dit artikel wordt beschreven hoe u dit doet.

## Toegangsvereisten

+++ Vouw uit om de toegangsvereisten voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-lidmaatschap</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> 
    <p>Nieuw:</p>
   <ul><li><p>Medewerker om een filter te wijzigen </p></li>
   <li><p>Standaard voor het wijzigen van een rapport</p></li> </ul>

<p>Huidig:</p>
   <ul><li><p>Verzoek om een filter te wijzigen </p></li>
   <li><p>Overgaan tot wijziging van een rapport</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards en kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen voor een rapport beheren</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Het resultaat weergeven van het samenvoegen van meerdere berekende waarden in een groep

1. Ga naar een taakrapport, klik **Acties van het Rapport** > **geef** uit.
1. In het **lusje van Groeperingen**, klik **groepering** toevoegen, en begin typend **Naam van het Project** in de **Groep door** gebied, dan selecteer **Project > Naam** het wanneer het in de lijst toont.

1. In de **Kolommen (Mening)** lusje, klik **Kolom** toevoegen, dan begin typend **Geplande Uren** in **tonen in dit kolom** gebied, dan selecteer het wanneer het in de lijst toont.

   >[!TIP]
   >
   >Begin altijd met het toevoegen van zoveel informatie via de Standaardinterface voordat u informatie bewerkt in de tekstmodus. Voeg velden toe die het dichtst bij de meeste informatie liggen of die de meeste informatie bevatten die u wilt gebruiken voor de berekening die u wilt maken.

1. In **vat deze kolom door** gebied samen, uitgezochte **Som**.
1. Klik **Schakelaar aan de Wijze van de Tekst** in de kolom u toevoegde, dan klik **geef de Wijze van de Tekst** uit.
1. Vervang de tekst in het vak door het volgende voorbeeld voor de tekstmodus:

   ```
   valueformat=compound
   aggregator.displayformat=minutesAsHoursString
   aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2)
   aggregator.function=SUM
   aggregator.valueformat=val
   aggregator.namekey=workrequired
   linkedname=direct
   textmode=true
   valuefield=workRequired
   namekey=workrequired
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") 
   viewalias=workrequired 
   displayname=Work Balance
   ```

   >[!TIP]
   >
   >Als u de geaggregeerde waarde in de groep wilt ophalen om het geaggregeerde verschil tussen de velden Geplande uren en Werkelijke uren weer te geven, voert u dezelfde vergelijking in de `aggregator.valuefield` -regel in. De `aggregator.displayformat` die voor de kolom Geplande uren wordt gebruikt, zet minuten om in uren. Omdat het veld Geplande uren is gebruikt als plaatsaanduiding, hoeft deze regel niet te worden aangepast.
   >
   >
   >De `minutesAsHoursString` -definitie van de `aggregator.displayformat` -regel betekent dat u niet elk veld met 60 hoeft te delen, zoals op de `valueexpression` -regel voor de resultaten gebeurt. In deze lus `aggregator.valuefield=workRequired` wordt: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2` .
1. Klik **Gedaan**.
1. Klik **sparen+Sluiten**.
