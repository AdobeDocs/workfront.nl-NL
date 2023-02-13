---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Weergave: bovenliggende taken tot 4 niveaus diep tonen'
description: Deze taakmening toont de taaknaam in de eerste kolom en (als zij bestaan) tot 4 oudertaken in afzonderlijke kolommen in de zelfde lijst.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 66b45d64-794d-4adc-b208-2ded0dc9c5dc
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 0%

---

# Weergave: bovenliggende taken tot 4 niveaus diep tonen

Deze taakmening toont de taaknaam in de eerste kolom en (als zij bestaan) tot 4 oudertaken in afzonderlijke kolommen in de zelfde lijst.

![parent_tasks_4_levels_deep.png](assets/parent-tasks-4-levels-deep-350x29.png)

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

## Bovenliggende taken tot 4 niveaus diep weergeven

1. Ga naar een takenlijst.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Nieuwe weergave**.

1. In de **Kolomvoorvertoning** gebied, alle kolommen behalve één verwijderen.
1. Klik op de koptekst van de resterende kolom en klik vervolgens op **Overschakelen naar tekstmodus**.
1. Plaats de muis boven het gebied in de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:

   ```
   column.0.descriptionkey=name
   ```

   <pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.lookup=link.view<br>column.0.link.valueField=objCode<br>column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=150<br>column.1.descriptionKey=parent<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valueField=parent:ID<br>column.1.link.linkproperty.0.valueFormat=int<br>column.1.link.lookup=link.view<br>column.1.link.valueField=parent:objCode<br>column.1.link.valueFormat=val<br>column.1.linkedname=parent<br>column.1.listsort=nested(parent).string(name)<br>column.1.namekey=parent<br>column.1.querysort=parent:name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valueField=parent:name<br>column.1.valueFormat=HTML<br>column.1.width=150<br>column.2.description=Parent<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valueField=parent:parent:ID<br>column.2.link.linkproperty.0.valueFormat=int<br>column.2.link.lookup=link.view<br>column.2.link.valueField=parent:parent:objCode<br>column.2.link.valueFormat=val<br>column.2.linkedname=parent<br>column.2.listsort=nested(parent:parent).string(name)<br>column.2.name=Parent Parent<br>column.2.querysort=parent:parent:name<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valueField=parent:parent:name<br>column.2.valueFormat=HTML<br>column.2.width=150<br>column.3.description=Parent Parent Parent<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valueField=parent:parent:parent:ID<br>column.3.link.linkproperty.0.valueFormat=int<br>column.3.link.lookup=link.view<br>column.3.link.valueField=parent:parent:parent:objCode<br>column.3.link.valueFormat=val<br>column.3.linkedname=parent<br>column.3.listsort=nested(parent:parent:parent).string(name)<br>column.3.name=Parent Parent Parent<br>column.3.querysort=parent:parent:parent:name<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valueField=parent:parent:parent:name<br>column.3.valueFormat=HTML<br>column.3.width=150<br>column.4.description=Parent Parent Parent Parent Parent<br>column.4.link.linkproperty.0.name=ID<br>column.4.link.linkproperty.0.valueField=parent:parent:parent:parent:ID<br>column.4.link.linkproperty.0.valueFormat=int<br>column.4.link.lookup=link.view<br>column.4.link.valueField=parent:parent:parent:parent:objCode<br>column.4.link.valueFormat=val<br>column.4.linkedname=parent<br>column.4.listsort=nested(parent:parent:parent:parent).string(name)<br>column.4.name=Parent Parent Parent Parent<br>column.4.querysort=parent:parent:parent:parent:name<br>column.4.shortview=false<br>column.4.stretch=100<br>column.4.valueField=parent:parent:parent:parent:name<br>column.4.valueFormat=HTML<br>column.4.width=150</pre>

1. Klikken **Weergave opslaan**.

   De naam van de taak wordt weergegeven in de eerste kolom en als de taak bovenliggende items heeft, worden maximaal vier bovenliggende items weergegeven in de resterende kolommen.
