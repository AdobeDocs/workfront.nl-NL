---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergeven en groeperen: werkelijke duur van project weergeven geaggregeerd door gemiddelde in een groep'
description: U kunt de volgende kolom in een projectrapport toevoegen om de Ware Duur te tonen die als gemiddelde in een groepering wordt bijeengevoegd.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Weergeven en groeperen: werkelijke duur van project weergeven geaggregeerd door gemiddelde in een groep

U kunt de volgende kolom in een projectrapport toevoegen om de Ware Duur te tonen die als gemiddelde in een groepering wordt bijeengevoegd.

![ project_with_aggregate_actual_duration_in_grouping_view.png ](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

## Werkelijke duur van project weergeven geaggregeerd door gemiddelde in een groep

Deze kolom toevoegen aan een projectweergave:

1. (Aanbevolen) Voor beste resultaten en om de samengevoegde gemiddelde waarde van de Ware Duur te zien, moet u een Groepering hebben die aan uw projectlijst of rapport wordt toegevoegd.\
   Voor meer informatie over het creëren van Groepen, zie het artikel [ overzicht van Groepen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Ga naar een bestaande projectweergave.
1. Breid het drop-down menu van de Mening uit, en selecteer **Mening** aanpassen.
1. Klik **toevoegen Kolom**.
1. Klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over **toont in dit kolom** gebied, en klikt **om tekst** uit te geven.

1. Verwijder alle tekst in het vak Tekstmodus en vervang deze door de volgende code:
   <pre>aggregator.displayformat=compound <br> aggregator.function=AVG <br> aggregator.namekey=view.relatedcolumn <br> aggregator.namekeyargkey=actualduration <br> aggregator.valuefield=actualDurationMinutes <br> aggregator.valueformat=val <br> displayname=Project Werkelijke Duur <br> duur <br> linkedname=project <br> namekey=actualduration <br> namekeyargkey=actualduration <br> querysort=actualDurationMinutes <br> textmode=true <br> valueField=actualDurationMinutes <br> valueFormat=compound#M:D <br> viewmode=actualduration</pre>

1. Klik **sparen Mening**.
