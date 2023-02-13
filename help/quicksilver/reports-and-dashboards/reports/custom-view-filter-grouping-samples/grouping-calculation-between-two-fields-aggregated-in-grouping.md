---
content-type: reference
product-area: reporting;projects
keywords: berekend,aggregaten,geavanceerd,weergaven
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Groeperen: het resultaat weergeven van het samenvoegen van meerdere berekende waarden in een groep.'
description: U kunt tekstmodus in een kolom gebruiken om een berekening weer te geven tussen twee velden in de weergave van een rapport of lijst. Elke lijn toont de berekening voor elk voorwerp in het rapport of de lijst.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# Groeperen: het resultaat weergeven van het samenvoegen van meerdere berekende waarden in een groep

U kunt tekstmodus in een kolom gebruiken om een berekening weer te geven tussen twee velden in de weergave van een rapport of lijst. Elke lijn toont de berekening voor elk voorwerp in het rapport of de lijst.

Bijvoorbeeld, kunt u het verschil tussen Ware Uren en Geplande Uren in een derde kolom tonen genoemd het Saldo van het Werk voor elke taak in een taakrapport. Zie voor meer informatie over berekende gegevensexpressies [Berekende gegevensexpressies](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

U kunt de geaggregeerde waarde van meerdere berekende weergaveitems in dezelfde kolom in een groep weergeven door een berekening toe te voegen aan de `aggregator` lijn van de kolom die de berekende waarde bevat. Bijvoorbeeld, kunt u (som van) de hoeveelheid uren van het Saldo van het Werk van alle taken in de groepering van het rapport of de lijst voor de kolom van het Saldo van het Werk samenvoegen. In dit artikel wordt beschreven hoe u dit kunt doen.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken</p> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Het resultaat weergeven van het samenvoegen van meerdere berekende waarden in een groep

1. Ga naar een taakrapport, klik **Handelingen rapporteren** > **Bewerken**.
1. In de **Groepen** tabblad, klikt u op **Groepering toevoegen** en begint te typen **Projectnaam** in de **Uw rapport groeperen** > **Eerst** en selecteert u deze wanneer deze in de lijst wordt weergegeven.

1. In de **Kolommen (weergave)** tabblad, klikt u op **Kolom toevoegen** en begint vervolgens met typen **Geplande uren** in de **Tonen in deze kolom** en selecteert u deze wanneer deze in de lijst wordt weergegeven.

   >[!TIP]
   >
   >Begin altijd met het toevoegen van zoveel informatie gebruikend de Standaardinterface alvorens u informatie op tekstwijze uitgeeft. Voeg velden toe die het dichtst bij de meeste informatie liggen of die de meeste informatie bevatten die u wilt maken voor de berekening.

1. In de **Deze kolom samenvatten met** veld, selecteren **Som** en klik vervolgens op **Gereed**.
1. Klikken **Overschakelen naar tekstmodus** in de kolom die u hebt toegevoegd.
1. Houd de cursor boven het gebied van de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Vervang de `valuefield ` en de `aggregator.valuefield` regels met de regels die zijn gemarkeerd in het volgende voorbeeld voor de tekstmodus:

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
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") viewalias=workrequired displayname=Work Balance
   ```

   >[!TIP]
   >
   >Als u de geaggregeerde waarde in de groep wilt ophalen om het geaggregeerde verschil tussen de velden Geplande uren en Werkelijke uren weer te geven, voert u dezelfde vergelijking in de `aggregator.valuefield` lijn. De `aggregator.displayformat` gebruikt voor de Geplande kolom van Uren zet notulen in uren om. Aangezien het veld Geplande uren is gebruikt als tijdelijke aanduiding, hoeft deze regel niet te worden aangepast.
   >
   >
   >De `minutesAsHoursString` definitie van de `aggregator.displayformat` regel betekent dat elk veld niet met 60 hoeft te worden gedeeld, zoals op het tabblad `valueexpression` voor de resultaten. In dit `aggregator.valuefield=workRequired` wordt: `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. Klikken **Opslaan en sluiten**.
