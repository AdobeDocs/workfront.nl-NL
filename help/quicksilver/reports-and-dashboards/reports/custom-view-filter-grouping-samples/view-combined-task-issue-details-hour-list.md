---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: gecombineerde taak- en uitgavedetails in een overzicht van uren'
description: In deze uurweergave worden de kolommen Taak en Naam van uitgave gecombineerd, evenals de taken en Geplande uren uitgeven met de arceroltag. Omdat een uuringang slechts tot of een taak of kwestie kan behoren, kunnen beide voorwerpen niet in de zelfde kolom tezelfdertijd verschijnen. Elke lijn van de mening bevolkt met de informatie van of een Taak of een Kwestie.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cf1137fd-c26a-4907-afe9-2373d3434631
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# Weergave: gecombineerde taak- en uitgavedetails in een overzicht van uren

Deze uurmening combineert de kolommen van de Naam van de Taak en van de Kwestie, evenals de Taak en Geplande Uren gebruikend de

```
sharecol
```

-tag. Omdat een uuringang slechts tot of een taak of kwestie kan behoren, kunnen beide voorwerpen niet in de zelfde kolom tezelfdertijd verschijnen. Elke lijn van de mening bevolkt met de informatie van of een Taak of een Kwestie.

Meer informatie over de

```
sharecol
```

markering, zie [ Mening: fusie informatie van veelvoudige kolommen in één gedeelde kolom ](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).\
![ custom_view_hours_with_task_and_issue_information.png ](assets/custom-view-hours-with-350x48.png)

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

## Gecombineerde taak en uitgiftedetails in een lijst van het Uur bekijken

Deze weergave toepassen:

1. Ga naar een lijst met uren.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom, dan klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over het gebied van de tekstwijze, en klikt **klikt om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:
   <pre>column.1.querysort=project:name <br> column.1.shortview=false <br> column.1.stretch=0 <br> column.1.valueField=project:name <br> column.1.valueformat=HTML <br> column.1.width=100 <br> column.2.description=Task of Issue <br> column.2.link.linkproperty.0.name=ID <br> column.2.link.linkproperty.0.valueField=task:ID <br> column.2.link.linkproperty.0.valueformat=int <br> column.2.link.lookup=link.view <br> column.2.link.valueField=task:objCode <br> column.2.link.valueformat val <br> column.2.linkedname=task <br> column.2.listsort=nested (taak).string(naam) <br> column.2.name=Task of Issue <br> column.2.querysort=task:name <br> column.2.sharecol=true <br> column.2.shortview=false <br>.2.stretch=0 <br> column.2.valueField=task:name <br> column.2.valueformat=HTML <br> column.2.width=100 <br> column.3.descriptionkey=optask <br> column.3.link.linkproperty.0.name=ID <br> column.3.link.linkproperty.0.valueField=opTask:ID <br> column.3.link.linkproperty.0.valueformat=int <br> column.3.link.lookup=link.view <br> column.3.link.valueField=opTask:objCode <br> column.3.link.valueformat=val <br>} column.3.linkedname=optask <br> column.3.listsort=nested (opTask).string(naam) <br> column.3.namekey=opTask <br> column.3.querysort=opTask:name <br> column.3.shortview=false <br> column.3.stretch=0 <br>.3.valueField=opTask:name <br> column.3.valueformat=HTML <br> column.3.width=1 <br> column.4.valueField=task:werk <br> column.4.sharecol=true <br> column.4.linkedname=task <br> column.4.valueformat doubleAsInt <br> column.4.namekey=view.relatedcolumn <br> column.4.querysort=task:het werk <br> column.4.textmode=true <br> column.4.namekeyargkey.0=task <br> column.4.namekeyargkey.1=work <br> column.4.yk name=Planned inspanning <br> column.5.displayname=Planned inspanning <br> column.5.viewalias=opTask:werk vereiste <br> column.5.linkedname=opTask <br> column.5.valuefield=opTask:workRequired <br> column.5.valueformat=compound <br> 3} column.5.querysort=opTask:workRequired <br> column.5.namekeyargkey.0=opTask <br> column.5.namekeyargkey.1=workrequired <br> column.5.namekey=view.relatedcolumn <br> column.5.textmode=true <br> column.6.description uren <br> column.6.linkedname=direct <br> column.6.listsort=doubleAsDouble (uren) <br> column.6.namekey=hours.abbr <br> column.6.querysort=hours <br> column.6.shortview=false <br> column.6.stretch=0 <br> column.6.valueField=hours <br> column.6.valueformat=doubleAsString <br> column.6.width=75 <br> column.7.descriptionkey=entrydate <br> column.7.linkedname=direct <br> column.7.listsort=atDateAsAtDate(entryDate) <br> column.7.namekey=entrydate.abbr <br> column.7.querysort=entryDate <br> column.7.shortview=false <br> column.7.stretch=0 <br> column.7.valueField=entryDate <br> column.7.valueFormat=atDate <br> column.7 width=75 <br> column.8.descriptionkey=description <br> column.8.linkedname=direct <br> column.8.listsort=string(beschrijving) <br> column.8.namekey=description.abbr <br> column.8.querysort=description <br> column.8.shortview=false <br> 8.stretch=0 <br> column.8.valueField=description <br> column.8.valueformat=HTML <br> column.8.width=150</pre>

1. Klik **sparen Mening**.
