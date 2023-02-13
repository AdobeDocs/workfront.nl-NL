---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Weergave: gecombineerde taak en uitgiftedetails in een lijst van het Uur"'
description: In deze uurweergave worden de kolommen Taak en Naam van uitgave gecombineerd, evenals de taken en Geplande uren uitgeven met de arceroltag. Omdat een uuringang slechts tot of een taak of kwestie kan behoren, kunnen beide voorwerpen niet in de zelfde kolom tezelfdertijd verschijnen. Elke lijn van de mening bevolkt met de informatie van of een Taak of een Kwestie.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cf1137fd-c26a-4907-afe9-2373d3434631
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# Weergave: gecombineerde taak en uitgiftedetails in een lijst van het Uur

Deze uurmening combineert de kolommen van de Naam van de Taak en van de Kwestie, evenals de Taak en Geplande Uren gebruikend de

```
sharecol
```

tag. Omdat een uuringang slechts tot of een taak of kwestie kan behoren, kunnen beide voorwerpen niet in de zelfde kolom tezelfdertijd verschijnen. Elke lijn van de mening bevolkt met de informatie van of een Taak of een Kwestie.

Meer informatie over de

```
sharecol
```

tag, zie [Weergave: gegevens uit meerdere kolommen samenvoegen in één gedeelde kolom](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).\
![custom_view_hours_with_task_and_issue_information.png](assets/custom-view-hours-with-350x48.png)

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

## Gecombineerde taak en uitgiftedetails in een lijst van het Uur bekijken

Deze weergave toepassen:

1. Ga naar een lijst met uren.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Nieuwe weergave**.

1. In de **Kolomvoorvertoning** gebied, alle kolommen behalve één verwijderen.
1. Klik op de koptekst van de resterende kolom en klik vervolgens op **Overschakelen naar tekstmodus**.
1. Plaats de muis boven het gebied in de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:
   <pre>column.1.querysort=project:name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valueField=project:name<br>column.1.valueFormat=HTML<br>column.1.width=100<br>column.2.description=Task or Issue<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valueField=task:ID<br>column.2.link.linkproperty.0.valueFormat=int<br>column.2.link.lookup=link.view<br>column.2.link.valueField=task:objCode<br>column.2.link.valueFormat=val<br>column.2.linkedname=task<br>column.2.listsort=nested(task).string(name)<br>column.2.name=Task or Issue<br>column.2.querysort=task:name<br>column.2.sharecol=true<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valueField=task:name<br>column.2.valueFormat=HTML<br>column.2.width=100<br>column.3.descriptionKey=optask<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valueField=opTask:ID<br>column.3.link.linkproperty.0.valueFormat=int<br>column.3.link.lookup=link.view<br>column.3.link.valueField=opTask:objCode<br>column.3.link.valueFormat=val<br>column.3.linkedname=optask<br>column.3.listsort=nested(opTask).string(name)<br>column.3.namekey=opTask<br>column.3.querysort=opTask:name<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valueField=opTask:name<br>column.3.valueFormat=HTML<br>column.3.width=1<br>column.4.valueField=task:work<br>column.4.sharecol=true<br>column.4.linkedname=task<br>column.4.valueFormat=doubleAsInt<br>column.4.namekey=view.related column<br>column.4.querysort=task:work<br>column.4.textmode=true<br>column.4.namekeyargkey.0=task<br>column.4.namekeyargkey.1=work<br>column.4.displayName=Planned inspanning<br>column.5.displayName=Planned inspanning<br>column.5.viewalias=opTask:workrequired<br>column.5.linkedname=opTask<br>column.5.valueField=opTask:workRequired<br>column.5.valueFormat=compound<br>column.5.querysort=opTask:workRequired<br>column.5.namekeyargkey.0=opTask<br>column.5.namekeyargkey.1=workrequired<br>column.5.namekey=view.related column<br>column.5.textmode=true<br>column.6.descriptionKey=hours<br>column.6.linkedname=direct<br>column.6.listsort=doubleAsDouble(hours)<br>column.6.namekey=hours.abbr<br>column.6.querysort=hours<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valueField=hours<br>column.6.valueFormat=doubleAsString<br>column.6.width=75<br>column.7.descriptionkey=entrydate<br>column.7.linkedname=direct<br>column.7.listsort=atDateAsAtDate(entryDate)<br>column.7.namekey=entrydate.abbr<br>column.7.querysort=entryDate<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.valueField=entryDate<br>column.7.valueFormat=atDate<br>column.7.width=75<br>column.8.descriptionkey=description<br>column.8.linkedname=direct<br>column.8.listsort=string(description)<br>column.8.namekey=description.abbr<br>column.8.querysort=description<br>column.8.shortview=false<br>column.8.stretch=0<br>column.8.valueField=description<br>column.8.valueFormat=HTML<br>column.8.width=150</pre>

1. Klikken **Weergave opslaan**.
