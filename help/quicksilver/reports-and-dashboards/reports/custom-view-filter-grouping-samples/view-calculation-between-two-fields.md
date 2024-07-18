---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: het resultaat weergeven van een berekening tussen twee velden in een kolom'
description: U kunt de tekstmodus in een kolom gebruiken om een berekening tussen twee velden weer te geven.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# Weergeven: het resultaat weergeven van een berekening tussen twee velden in een kolom

U kunt de tekstmodus in een kolom gebruiken om een berekening tussen twee velden weer te geven.

Als u bijvoorbeeld wilt weten hoeveel weken er zijn verstreken tussen twee datums, kunt u dit verschil berekenen met de syntaxis van de tekstmodus en gegevensexpressies.\
U kunt bijvoorbeeld het weekdagverschil berekenen tussen de Geplande Voltooiingsdatum en de Werkelijke Voltooiingsdatum van een taak en het resultaat weergeven in een kolom.

U kunt andere twee datums gebruiken in deze berekening (Werkelijk begin, Werkelijke Voltooiing, Geprojecteerd Begin, Geprojecteerde Voltooiing, enz.).\
Voor meer informatie over berekende gegevensuitdrukkingen, zie [ Overzicht van berekende gegevensuitdrukkingen ](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

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
   <td> <p>Verzoek om een weergave te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Het resultaat weergeven van een berekening tussen twee velden in een kolom

Deze kolom toevoegen aan een taakweergave:

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Mening**, klik **Nieuwe Mening**.

1. Klik **toevoegen Kolom**, toen **Schakelaar aan de Wijze van de Tekst**.

1. Beweeg over het gebied van de tekstwijze, en klik **Klik om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:
   <pre>displayname=Week het Verschil van de Dag van de Dag <br> textmode=true <br> valueexpression=WEEKDAYDIFF ({plannedCompletionDate}, {actualCompletionDate}) <br> valueformat=HTML</pre>

1. (Facultatief) om de waarden samen te voegen die in de mening in een groepering worden getoond, volg de stappen die in [ worden beschreven Groepering: toon het resultaat van het samenvoegen van veelvoudige berekende waarden in een groepering ](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Klik **sparen**, dan **sparen Mening**.
