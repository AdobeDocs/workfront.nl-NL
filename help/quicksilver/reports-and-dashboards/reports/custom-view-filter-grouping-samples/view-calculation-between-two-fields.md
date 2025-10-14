---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergeven: het resultaat weergeven van een berekening tussen twee velden in een kolom'
description: U kunt de tekstmodus in een kolom gebruiken om een berekening tussen twee velden weer te geven.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Weergeven: het resultaat weergeven van een berekening tussen twee velden in een kolom

<!--Audited: 11/2024-->

U kunt de tekstmodus in een kolom gebruiken om een berekening tussen twee velden weer te geven.

Als u bijvoorbeeld wilt weten hoeveel weken er zijn verstreken tussen twee datums, kunt u dit verschil berekenen met de syntaxis van de tekstmodus en gegevensexpressies.\
U kunt bijvoorbeeld het weekdagverschil berekenen tussen de Geplande Voltooiingsdatum en de Werkelijke Voltooiingsdatum van een taak en het resultaat weergeven in een kolom.

U kunt andere twee datums gebruiken in deze berekening (Werkelijk begin, Werkelijke Voltooiing, Geprojecteerd Begin, Geprojecteerde Voltooiing, enz.).\
Voor meer informatie over berekende gegevensuitdrukkingen, zie [&#x200B; Overzicht van berekende gegevensuitdrukkingen &#x200B;](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> 
    <p>Nieuw:</p>
   <ul><li><p>Medewerker om een filter te wijzigen </p></li>
   <li><p>Standaard voor het wijzigen van een rapport</p></li> </ul>

<p>Huidige:</p>
   <ul><li><p>Verzoek om een filter te wijzigen </p></li>
   <li><p>Plan om een rapport te wijzigen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Het resultaat weergeven van een berekening tussen twee velden in een kolom

Deze kolom toevoegen aan een taakweergave:

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Mening**, klik **Nieuwe Mening**.

1. Klik **toevoegen Kolom**, dan **Schakelaar aan de Wijze van de Tekst** > **geeft de Wijze van de Tekst** uit.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:

   ```
   displayname=Week Day Difference
   textmode=true
   valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})
   valueformat=HTML
   ```

1. (Facultatief) om de waarden samen te voegen die in de mening in een groepering worden getoond, volg de stappen die in [&#x200B; worden beschreven Groepering: toon het resultaat van het samenvoegen van veelvoudige berekende waarden in een groepering &#x200B;](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Klik **Gedaan**, dan **sparen Mening**.
