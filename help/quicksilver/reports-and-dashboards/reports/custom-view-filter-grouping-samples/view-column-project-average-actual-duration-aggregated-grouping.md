---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergeven en groeperen: weergaveproject Werkelijke duur geaggregeerd door gemiddelde in een groepering'
description: U kunt de volgende kolom in een projectrapport toevoegen om de Ware Duur te tonen die als gemiddelde in een groepering wordt bijeengevoegd.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# Weergeven en groeperen: weergaveproject Werkelijke duur geaggregeerd door gemiddelde in een groep

U kunt de volgende kolom in een projectrapport toevoegen om de Ware Duur te tonen die als gemiddelde in een groepering wordt bijeengevoegd.

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Werkelijke duur van project weergeven geaggregeerd door gemiddelde in een groep

Deze kolom toevoegen aan een projectweergave:

1. (Aanbevolen) Voor beste resultaten en om de samengevoegde gemiddelde waarde van de Ware Duur te zien, moet u een Groepering hebben die aan uw projectlijst of rapport wordt toegevoegd.\
   Zie het artikel voor meer informatie over het maken van groepen [Overzicht van groepen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Ga naar een bestaande projectweergave.
1. Vouw het vervolgkeuzemenu Weergave uit en selecteer **Weergave aanpassen**.
1. Klikken **Kolom toevoegen**.
1. Klikken **Overschakelen naar tekstmodus**.
1. Muis over de **Tonen in deze kolom** en klik op **Klik om tekst te bewerken**.

1. Verwijder alle tekst in het vak Tekstmodus en vervang deze door de volgende code:

   <pre>aggregator.displayFormat=compound <br>aggregator.function=AVG <br>aggregator.namekey=view.related column <br>aggregator.namekeyargkey=actualduration <br>aggregator.valueField=actualDurationMinutes <br>aggregator.valueformat=val <br>displayname=Project Ware Duur <br>durationunitfield=durationUnit.value <br>linkedname=project <br>namekey=actualduration <br>namekeyargkey=actualduration <br>querysort=actualDurationMinutes <br>textmode=true <br>valueField=actualDurationMinutes <br>valueFormat=compound#M:D <br>viewalias=actualduration</pre>

1. Klikken **Weergave opslaan**.
