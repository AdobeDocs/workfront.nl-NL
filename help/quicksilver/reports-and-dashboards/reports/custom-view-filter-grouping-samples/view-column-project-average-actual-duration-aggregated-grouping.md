---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergeven en groeperen: De werkelijke duur van het project weergeven, samengevoegd met het gemiddelde in een groep'
description: U kunt de volgende kolom in een projectrapport toevoegen om de Ware Duur te tonen die als gemiddelde in een groepering wordt bijeengevoegd.
author: Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Weergeven en groeperen: werkelijke duur van project weergeven geaggregeerd door gemiddelde in een groep

<!--Audited: 11/2024-->

U kunt de volgende kolom in een projectmening toevoegen om de Ware Duur te tonen die als gemiddelde in een groepering wordt bijeengevoegd.

![ project_with_aggregate_actual_duration_in_grouping_view.png ](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Medewerker of verzoek om een filter te wijzigen </p>
   <p>Standaard of Plan om een rapport te wijzigen</p>
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

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Werkelijke duur van project weergeven geaggregeerd door gemiddelde in een groep

Deze kolom toevoegen aan een projectweergave:

1. Ga naar een projectlijst.
1. (Vereist) om de samengevoegde gemiddelde waarde van de Ware Duur van het project te zien, moet u een groepering hebben die aan uw projectlijst wordt toegevoegd.\
   Voor meer informatie over het creëren van groeperingen, zie het artikel [ overzicht van Groepen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
1. Vouw het **drop-down menu van de Mening** uit, en selecteer **aanpassen Mening**.
1. Klik **toevoegen Kolom**.
1. Klik **Schakelaar aan de Wijze van de Tekst**, dan klik **uitgeven de Wijze van de Tekst**.
1. Verwijder alle tekst in **uitgeeft de Wijze van de Tekst** vakje, en vervang het met de volgende code:

   ```
   aggregator.displayformat=compound 
   aggregator.function=AVG 
   aggregator.namekey=view.relatedcolumn 
   aggregator.namekeyargkey=actualduration 
   aggregator.valuefield=actualDurationMinutes 
   aggregator.valueformat=val 
   displayname=Project Actual Duration 
   durationunitfield=durationUnit.value 
   linkedname=project 
   namekey=actualduration 
   namekeyargkey=actualduration 
   querysort=actualDurationMinutes 
   textmode=true 
   valuefield=actualDurationMinutes 
   valueformat=compound#M:D 
   viewalias=actualduration
   ```

1. Klik **Gedaan**, dan **sparen Mening**.
1. (Facultatief) werk de meningsnaam bij, dan klik **sparen Mening**.
