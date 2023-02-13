---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Weergave: taken die door planningsuitzonderingen worden beïnvloed"'
description: Deze taakmening identificeert taken die wegens weekends, Persoonlijke Tijd weg, of andere planningsuitzonderingen moeten te voltooien.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d7c77fa-d9a7-4e91-8dae-ad3aaca6f1da
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Weergave: taken die door planningsuitzonderingen worden beïnvloed

Deze taakmening identificeert taken die wegens weekends, Persoonlijke Tijd weg, of andere planningsuitzonderingen moeten te voltooien.

In deze weergave wordt het volgende weergegeven:

* De duur van de taken
* De geplande begin- en einddatum van de taken
* De duur van de taken op basis van het aantal dagen tussen de geplande aanvangsdatum en de geplande einddatum van de taken (kalenderduur)
* Het aantal van de dag in het programma van het project wanneer de taak (de Datum van het Begin van de Kalender) begint
* De duur van de weekdagen van de taken volgens het aantal weekdagen tussen de geplande aanvangs- en geplande einddatum van de taken (duur weekdag)
* Als de Duur van de Dag van de Week groter is dan de duur van de taken, die erop wijst dat er uitzonderingsdagen in de duur van de taken zijn, zijn de taken duidelijk als &quot;Uitzondering&quot;.\
   ![tasks_with_Kalender_Exc.png](assets/tasks-with-calendar-exceptions-350x51.png)

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

## Taken weergeven die door planningsuitzonderingen worden beïnvloed

1. Ga naar een takenlijst.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Nieuwe weergave**.

1. In de **Kolomvoorvertoning** gebied, alle kolommen behalve één verwijderen.
1. Klik op de koptekst van de resterende kolom en klik vervolgens op **Overschakelen naar tekstmodus**.
1. Plaats de muis boven het gebied in de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:
   <pre>column.0.descriptionKey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.lookup=link.view<br>column.0.link.valueField=objCode<br>column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=150<br>column.1.descriptionKey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAsInt(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valueField=durationFieldLong<br>column.1.valueFormat=compound<br>column.1.viewalias=duration<br>column.1.width=80<br>column.2.descriptionKey=planningStartDate<br>column.2.linkedname=direct<br>column.2.listsort=atDateAsAtDate(scheduledStartDate)<br>column.2.namekey=planedstartdate.abbr<br>column.2.querysort=SchedulStartDate<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valueField=SchedulStartDate<br>column.2.valueFormat=atDate<br>column.2.width=80<br>column.3.descriptionKey=planningComplementationDate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(scheduledCompletionDate)<br>column.3.namekey=planningComplementationDate.abbr<br>column.3.querysort=SchedulCompletionDate<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valueField=SchedulCompletionDate<br>column.3.valueFormat=atDate<br>column.3.width=80<br>column.4.aggregator.displayformat=int<br>column.4.aggregator.function=SUM<br>column.4.aggregator.namekey=id<br>column.4.aggregator.valueexpression=DATEDIFF({scheduledCompletionDate},<br>{SchedulStartDate})+1<br>column.4.aggregator.valueFormat=intAsInt<br>column.4.descriptionkey=id<br>column.4.linkedname=direct<br>column.4.listsort=intAsInt(ID)<br>column.4.name=Calendar Duration<br>column.4.querysort=ID<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valueexpression=DATEDIFF({scheduledCompletionDate},{scheduledStartDate})+1<br>column.4.valueFormat=int<br>column.4.width=80<br>column.5.aggregator.displayformat=int<br>column.5.aggregator.function=SUM<br>column.5.aggregator.namekey=id<br>column.5.aggregator.valueexpression=DATEDIFF({scheduledStartDate},{project}.<br>{SchedulStartDate})+0<br>column.5.aggregator.valueFormat=intAsInt<br>column.5.descriptionkey=id<br>column.5.linkedname=direct<br>column.5.listsort=intAsInt(ID)<br>column.5.name=Calendar Start Date<br>column.5.querysort=ID<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valueexpression=DATEDIFF({scheduledStartDate},{project}.{SchedulStartDate})+0<br>column.5.valueFormat=int<br>column.5.width=80<br>column.6.aggregator.displayformat=int<br>column.6.aggregator.function=SUM<br>column.6.aggregator.namekey=id<br>column.6.aggregator.valueexpression=WEEKDAYDIFF({SchedulStartDate},<br>{scheduledCompletionDate})+0<br>column.6.aggregator.valueFormat=HTML<br>column.6.descriptionkey=id<br>column.6.linkedname=direct<br>column.6.listsort=intAsInt(ID)<br>column.6.name=Week Day Duration<br>column.6.querysort=ID<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valueexpression=WEEKDAYDIFF({SchedulStartDate},{scheduledCompletionDate})+0<br>column.6.valueFormat=int<br>column.6.width=80<br>column.7.aggregator.display.format=int<br>column.7.aggregator.expression=IF((WEEKDAYDIFF({scheduledStartDate},{scheduledCompletionDate}))&gt;({duration}/480), "Exception",")<br>column.7.aggregator.function=SUM<br>column.7.aggregator.namekey=id<br>column.7.aggregator.valueFormat=HTML<br>column.7.linkedname=direct<br>column.7.listsort=intAsInt(ID)<br>column.7.name=Schedule<br>column.7.querysort=ID<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.valueexpression=IF((WEEKDAYDIFF({scheduledStartDate},{scheduledCompletionDate}))&gt;({duration}/480),"Exception",")<br>column.7.valueFormat=HTML<br>column.7.width=80</pre>

1. Klikken **Weergave opslaan**.
