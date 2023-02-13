---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Weergave: het resultaat weergeven van een berekening tussen twee velden in een kolom"'
description: U kunt de tekstmodus in een kolom gebruiken om een berekening tussen twee velden weer te geven.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Weergave: het resultaat weergeven van een berekening tussen twee velden in een kolom

U kunt de tekstmodus in een kolom gebruiken om een berekening tussen twee velden weer te geven.

Als u bijvoorbeeld wilt weten hoeveel weken er zijn verstreken tussen twee datums, kunt u dit verschil berekenen met de syntaxis van de tekstmodus en gegevensexpressies.\
U kunt bijvoorbeeld het weekdagverschil berekenen tussen de Geplande Voltooiingsdatum en de Werkelijke Voltooiingsdatum van een taak en het resultaat weergeven in een kolom.

U kunt andere twee datums gebruiken in deze berekening (Werkelijk begin, Werkelijke voltooiing, Geprojecteerd begin, Geprojecteerde voltooiing, enz.).\
Zie voor meer informatie over berekende gegevensexpressies [Berekende gegevensexpressies](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

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

## Het resultaat weergeven van een berekening tussen twee velden in een kolom

Deze kolom toevoegen aan een taakweergave:

1. Ga naar een takenlijst.
1. Van de **Weergave** vervolgkeuzelijst, klikt u op **Nieuwe weergave**.

1. Klikken **Kolom toevoegen** vervolgens **Overschakelen naar tekstmodus**.

1. Houd de cursor boven het gebied van de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:
   <pre>displayname=Week Day Difference<br>textmode=true<br>valueexpression=WEEKDAYDIFF({scheduledCompletionDate},{actualCompletionDate})<br>valueformat=HTML</pre>

1. (Optioneel) Als u de waarden die in de weergave in een groep worden weergegeven, wilt samenvoegen, voert u de stappen uit die worden beschreven in [Groeperen: het resultaat weergeven van het samenvoegen van meerdere berekende waarden in een groep](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Klikken **Opslaan** vervolgens **Weergave opslaan**.
