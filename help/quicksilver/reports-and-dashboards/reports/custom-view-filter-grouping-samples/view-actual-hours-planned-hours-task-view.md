---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergeven: Werkelijke uren over geplande uren in dezelfde kolom van een taakweergave'
description: In deze taakweergave wordt het werkelijke aantal uren voor een taak weergegeven over de geplande uren voor elke taak.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Weergeven: Werkelijke uren over geplande uren in dezelfde kolom van een taakweergave

In deze taakmening, wordt de daadwerkelijke hoeveelheid uren die op een taak wordt geregistreerd getoond over de uren die voor elke taak worden gepland.

![ actual_vs_scheduled_in_task_report.png ](assets/actual-vs-planned-in-task-report-350x58.png)

## Vereisten voor toegang

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-lidmaatschap*</td> 
   <td> <p>Enig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Verzoek voor het wijzigen van een weergave </p>
   <p>Een rapport wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> <p><b>OPMERKING</b>

Als je nog steeds geen toegang hebt, vraag je je Workfront-beheerder of deze extra beperkingen instelt voor je toegangsniveau. Zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus</a> maken of wijzigen voor informatie over de wijze waarop een Workfront-beheerder je toegangsniveau kan wijzigen.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen voor een rapport beheren</p> <p>Zie Toegang aanvragen tot objecten </a>voor meer informatie over het aanvragen van aanvullende toegang<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met je Workfront-beheerder als je wilt kijken welk lidmaatschap, welk licentietype of welke toegang je hebt.

## Werkelijke uren over geplande uren weergeven in een taakweergave

Deze weergave toepassen:

1. Ga naar een lijst met taken.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik op de kop van de resterende kolom en klik vervolgens op Overschakelen naar **de tekstmodus**.
1. Plaats de muis boven het tekstmodusgebied en klik op **Klik om de tekst** te bewerken.
1. Verwijder de tekst die u vindt in het **vak Tekstmodus** en vervang deze door de volgende code:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID column.0.link.linkproperty.0.valuefield=ID<br>column.0.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.00.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch<br>=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.viewalias=assignments<br>column.1.displayname=<br>column.1.linkedname=direct<br>column.1.namekey=toewijzingen<br>column.1.valuefield=assignmentsListString<br>column.1.valueformat=HTML<br>column.1.tile.name=component.assignmentslist<br>column.2.displayname=Actual/Geplande uren<br>column.2.linkedname=direct<br>column.2.namekey=actualworkrequired<br>column.2.querysort=actualWork<br>column.2.textmode=true<br>column.2.valueexpression=CONCAT({actualWorkRequired}/60,' / ',{workRequired}/60)<br>column.2.valuefield =actualWorkRequired<br>column.2.valueformat=compound<br>column.2.viewalias=actualworkrequired<br>column.3.aggregator.function=SUM<br>column.3.aggregator.valueexpression=SUB({actualWork}, {workRequired})<br>column.3.aggregator.valueformat=compound<br>column.3.displayname=Hours Variance<br>column.3.linkedname=direct<br>column.3.textmode=true<br>column.3.valueexpression=SUB({actualWork}, {workRequired})/60<br>column.3.valueformat=customNumberAsString</pre>

1. Klik op **Weergave** opslaan.
