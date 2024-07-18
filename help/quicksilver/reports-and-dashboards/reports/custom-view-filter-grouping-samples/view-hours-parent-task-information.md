---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: hours with parent task information'
description: In deze uurweergave ziet u de naam van de taak waarin de uren zijn vastgelegd, plus de naam van de bovenliggende taak.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c24555fc-3bae-451b-8a44-28a8158199d1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Weergeven: uren met bovenliggende taakgegevens

In deze uurweergave ziet u de naam van de taak waarin de uren zijn vastgelegd, plus de naam van de bovenliggende taak.

![ custom_hour_view_with_task_and_parent_task_info.png ](assets/custom-hour-view-with-task-and-parent-task-info-350x55.png)

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

## Uren weergeven met informatie over bovenliggende taken

1. Ga naar een lijst met uren.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom, dan klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over het gebied van de tekstwijze, en klikt **klikt om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:
   <pre>column.0.aggregator.displayformat=doubleAsString <br> column.0.aggregator.function=SUM <br> column.0.aggregator.namekey=hours <br> column.0.aggregator.valueField=hours <br> column.0.aggregator.valueFormat=doubleAsDouble <br> column.0.descriptionkey=hours <br> column.0.0 link.linkproperty.0.name=ID <br> column.0.link.linkproperty.0.valueField=ID <br> column.0.link.linkproperty.0.valueformat=int <br> column.0.link.lookup=link.view <br> column.0.link.valueField=objCode <br> column.0.link.valueformat=<br> column.0.linkedname=direct <br> column.0.listsort=doubleAsDouble (uren) <br> column.0.namekey=hours.abbr <br> column.0.querysort=hours <br> column.0.shortview=false <br> column.0.stretch=100 <br> column.0.valueField=hours <br> column.0.valueformat=doubleAsString <br> column.0.width=150 <br> column.1.descriptionkey=task <br> column.1.link.linkproperty.0.name=ID <br> column.1.link.linkproperty.0.value=task:ID <br> column.1.link.linkproperty.0.valueformat=int <br> column.1.link.lookup=link.view <br> column.1.link.valuefield=task:objCode <br> column.1.link.valueformat=val <br> column.1.linkedname=task <br>.1.listsort=nested (taak).string(naam) <br> column.1.namekey=task <br> column.1.querysort=task:name <br> column.1.shortview=false <br> column.1.stretch=0 <br> column.1.valuefield=task:name <br> column.1.valuefefefefefex at=HTML <br> column.1.width=150 <br> column.2.description=Parent Naam van de Taak <br> column.2.link.linkproperty.0.name=ID <br> column.2.link.linkproperty.0.valueField=task :parent: identiteitskaart <br> column.2.link.linkproperty.0.valuFormat=int <br> column.2.link.lookup=link.view <br> column.2.link.valueField=task:objCode <br> column.2.link.valueformat=val <br> column.2.linkedname=task <br> column.2.listsort=nested (taak:ouder).string) <br> 6} column.2.name=Parent Naam van de Taak <br> column.2.querysort=task :parent: naam <br> column.2.shortview=false <br> column.2.stretch=0 <br> column.2.valueField=task :parent: naam <br> column.2.valueformat=HTML <br> column.2.width=150</pre>

1. Klik **sparen Mening**.
