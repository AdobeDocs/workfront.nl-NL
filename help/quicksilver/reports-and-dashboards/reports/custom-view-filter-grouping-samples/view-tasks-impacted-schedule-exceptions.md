---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: taken die worden beïnvloed door uitzonderingen van schema'
description: Deze taakmening identificeert taken die wegens weekends, Persoonlijke Tijd weg, of andere planningsuitzonderingen moeten te voltooien.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d7c77fa-d9a7-4e91-8dae-ad3aaca6f1da
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 0%

---

# Weergave: taken die worden beïnvloed door planningsuitzonderingen

Deze taakmening identificeert taken die wegens weekends, Persoonlijke Tijd weg, of andere planningsuitzonderingen moeten te voltooien.

In deze weergave wordt het volgende weergegeven:

* De duur van de taken
* De geplande begin- en einddatum van de taken
* De duur van de taken op basis van het aantal dagen tussen de geplande aanvangsdatum en de geplande einddatum van de taken (kalenderduur)
* Het aantal van de dag in het programma van het project wanneer de taak (de Datum van het Begin van de Kalender) begint
* De duur van de weekdagen van de taken volgens het aantal weekdagen tussen de geplande aanvangs- en geplande einddatum van de taken (duur weekdag)
* Als de Duur van de Dag van de Week groter is dan de duur van de taken, die erop wijst dat er uitzonderingsdagen in de duur van de taken zijn, zijn de taken duidelijk als &quot;Uitzondering&quot;.\
  ![ tasks_with_agenda_exception.png ](assets/tasks-with-calendar-exceptions-350x51.png)

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

## Taken weergeven die door planningsuitzonderingen worden beïnvloed

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom, dan klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over het gebied van de tekstwijze en klikt **om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:
   <pre>column.0.descriptionkey=name <br> column.0.link.linkproperty.0.name=ID <br> column.0.link.linkproperty.0.valueField=ID <br> column.0.link.linkproperty.0.valueformat=int <br> column.0.link.lookup=link.view <br> column.0.link.valueField=objCode 5} column.0.link.valueformat=val <br> column.0.linkedname=direct <br> column.0.listsort=string(naam) <br> column.0.namekey=name.abbr <br> column.0.querysort=name <br> column.0.shortview=false <br> column.0.stretch=100 {1 2} column.0.valueField=name <br> column.0.valueformat=HTML <br> column.0.width=150 <br> column.1.descriptionkey=duration <br> column.1.linkedname=direct <br> column.1.listsort=intAsInt (durationMinutes) <br> column.1.namekey=duration.abbr <br> column.1.querysort=durationMinutes <br> column.1.shortview=false <br> column.1.stretch=0 <br> column.1.valueField=durationFieldLong <br> column.1.valueformat=compound <br> column.1.viewalias duur <br> column.1.width=80 <br> column.2.descriptionkey=planedstartdate <br> column.2.linkedname=direct <br> column.2.listsort=atDateAsAtDate (scheduledStartDate) <br> column.2.namekey=planedstartdate.abbr <br> column.2.querysort=scheduledStartDate <br> column.2.shortview=false <br> column.2.stretch=0 <br> column.2.valueField=SchedulStartDate <br> column.2.valueformat=atDate <br> column.2.width=80 <br> column.3.description=planedcompltiondate <br> column.3.linkedname=direct <br> column.3.listsort=atDateAsAtDate (scheduledCompletionDate) <br> column.3.namekey=planedcompltiondate.abbr <br> column.3.querysort=scheduledCompletionDate <br> column.3.3 shortview=false <br> column.3.stretch=0 <br> column.3.valuefield=scheduledCompletionDate <br> column.3.valueformat=atDate <br> column.3.width=80 <br> column.4.aggregator.displayformat=int <br> column.4.aggregator.function SUM <br> column.4.aggregator.namekey=id <br> column.4.aggregator.valueexpression=DATEDIFF ({plannedCompletionDate}, <br> {plannedStartDate})+1 <br> column.4.aggregator.valueformat=intAsInt <br> column.4.descriptionkey=id <br> column.4.linkedname=direct <br> column.4.listsort=intAsInt (identiteitskaart) <br> column.4.name=Calendar Duur <br> column.4.querysort=ID <br> column.4.shortview=false <br> column.4.stretch=0 <br> column.4.value expression=DATETETEST DIFF ({plannedCompletionDate},{plannedStartDate}) + 1 <br> column.4.valueformat=int <br> column.4.width=80 <br> column.5.aggregator.displayformat=int <br> column.5.aggregator.function=SUM <br> column.5.aggregator.namekey=id <br> column.5.aggregator.valueexpression=DATEDIFF ({plannedStartDate}, {project}.<br><br><br> {plannedStartDate})+0 <br> column.5.aggregator.valueformat=intAsInt <br> column.5.descriptionkey=id <br> column.5.linkedname=direct <br> column.5.listsort=intAsInt (identiteitskaart) <br> column.5.name=Calendar Datum <br> column.5.querysort=ID <br> column.5.shortview=false <br> column.5.stretch=0 <br> column.5.valueexpression=DATEDIFF ({plannedStartDate}, {project}.{plannedStartDate})+0 <br> column.5.valueformat=int <br> column.5.width=80 <br> column.6.aggregator.displayformat=int <br> column.6.aggregator.function=SUM <br> column.6.aggregator.namekey=id <br> column.6.aggregator.valueexpression=WEEKDAYDIFF ({plannedStartDate},<br> {plannedCompletionDate})+0 <br> column.6.aggregator.valueformat=HTML <br> column.6.descriptionkey=id <br> column.6.linkedname=direct <br> column.6.listsort=intAsInt (identiteitskaart) <br> column.6.name=Week Duur van de Dag <br>.6.querysort=ID <br> column.6.shortview=false <br> column.6.stretch=0 <br> column.6.valueexpression=WEEKDAYDIFF ({plannedStartDate}, {plannedCompletionDate}) + 0 <br> column.6.valueFormat=int <br> column.6.width=80 <br> 3} column.7.aggregator.displayformat=int <br> column.7.aggregator.expression=IF ((WEEKDAYDIFF ({plannedStartDate}, {plannedCompletionDate}))&gt; ({duration}/480), "Uitzondering",") <br> column.7.aggregator.function=SUM <br> column.7 aggregator.namekey=id <br> column.7.aggregator.valueformat=HTML <br> column.7.linkedname=direct <br> column.7.listsort=intAsInt (identiteitskaart) <br> column.7.name=Schedule <br> column.7.querysort=ID <br> column.7.shortview=false <br> column.7.stretch=0 <br> column.7.valueexpression=IF ((WEEKDAYDIFF ({plannedStartDate}, {plannedCompletionDate}))&gt; ({duration}/480), "Uitzondering",") <br> column.7.valueformat=HTML <br> column.7.width 80</pre>

1. Klik **sparen Mening**.
