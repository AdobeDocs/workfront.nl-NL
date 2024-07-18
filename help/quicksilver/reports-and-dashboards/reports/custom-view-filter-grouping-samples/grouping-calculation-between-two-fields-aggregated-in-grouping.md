---
content-type: reference
product-area: reporting;projects
keywords: berekend,aggregaten,geavanceerd,weergaven
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groeperen: het resultaat weergeven van het samenvoegen van meerdere berekende waarden in een groep'
description: U kunt tekstmodus in een kolom gebruiken om een berekening weer te geven tussen twee velden in de weergave van een rapport of lijst. Elke lijn toont de berekening voor elk voorwerp in het rapport of de lijst.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Groeperen: het resultaat weergeven van het samenvoegen van meerdere berekende waarden in een groep

U kunt tekstmodus in een kolom gebruiken om een berekening weer te geven tussen twee velden in de weergave van een rapport of lijst. Elke lijn toont de berekening voor elk voorwerp in het rapport of de lijst.

Bijvoorbeeld, kunt u het verschil tussen Ware Uren en Geplande Uren in een derde kolom tonen genoemd het Saldo van het Werk voor elke taak in een taakrapport. Voor meer informatie over berekende gegevensuitdrukkingen, zie [ Overzicht van berekende gegevensuitdrukkingen ](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

U kunt de geaggregeerde waarde van meerdere berekende weergave-items in dezelfde kolom in een groep weergeven door een berekening toe te voegen aan de `aggregator` -regel van de kolom die de berekende waarde bevat. Bijvoorbeeld, kunt u (som van) de hoeveelheid uren van het Saldo van het Werk van alle taken in de groepering van het rapport of de lijst voor de kolom van het Saldo van het Werk samenvoegen. In dit artikel wordt beschreven hoe u dit kunt doen.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Verzoek om een groepering te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een groep te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Het resultaat weergeven van het samenvoegen van meerdere berekende waarden in een groep

1. Ga naar een taakrapport, klik **de Acties van het Rapport** > **uitgeven**.
1. In het **lusje van Groepen**, klik **Groepering** toevoegen, en begin **Naam van het Project** in de **Groep uw Rapport** > **eerst door** gebied te typen, dan het te selecteren wanneer het in de lijst toont.

1. In de **Kolommen (Mening)** tabel, klik **Kolom** toevoegen, dan begin **Geplande Uren** in **tonen in dit kolom** gebied, dan selecteren het wanneer het in de lijst toont.

   >[!TIP]
   >
   >Begin altijd met het toevoegen van zoveel informatie gebruikend de Standaardinterface alvorens u informatie op tekstwijze uitgeeft. Voeg velden toe die het dichtst bij de meeste informatie liggen of die de meeste informatie bevatten die u wilt maken voor de berekening.

1. In **vat deze kolom door** gebied samen, uitgezochte **Som**, dan klik **Gedaan**.
1. Klik **Schakelaar aan de Wijze van de Tekst** in de kolom u toevoegde.
1. Beweeg over het gebied van de tekstwijze, en klik **Klik om tekst** uit te geven.
1. Vervang de regels `valuefield ` en `aggregator.valuefield` door de regels die zijn gemarkeerd in het volgende voorbeeld in de tekstmodus:

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
   >Als u de geaggregeerde waarde in de groep wilt ophalen om het geaggregeerde verschil tussen de velden Geplande uren en Werkelijke uren weer te geven, voert u dezelfde vergelijking in de regel `aggregator.valuefield` in. De `aggregator.displayformat` die voor de kolom Geplande uren wordt gebruikt, zet minuten om in uren. Aangezien het veld Geplande uren is gebruikt als tijdelijke aanduiding, hoeft deze regel niet te worden aangepast.
   >
   >
   >De `minutesAsHoursString` -definitie van de `aggregator.displayformat` -regel houdt in dat u elk veld niet met 60 hoeft te delen, zoals op de `valueexpression` -regel is gebeurd. In deze `aggregator.valuefield=workRequired` wordt: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2` .

1. Klik **sparen+Sluiten**.
