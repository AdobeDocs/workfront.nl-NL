---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: bovenliggende taken tot 4 niveaus diep weergeven'
description: Deze taakmening toont de taaknaam in de eerste kolom en (als zij bestaan) tot 4 oudertaken in afzonderlijke kolommen in de zelfde lijst.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 66b45d64-794d-4adc-b208-2ded0dc9c5dc
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 0%

---

# Weergave: bovenliggende taken tot 4 niveaus diep weergeven

Deze taakmening toont de taaknaam in de eerste kolom en (als zij bestaan) tot 4 oudertaken in afzonderlijke kolommen in de zelfde lijst.

![ parent_tasks_4_levels_deep.png ](assets/parent-tasks-4-levels-deep-350x29.png)

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

## Bovenliggende taken tot 4 niveaus diep weergeven

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom, dan klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over het gebied van de tekstwijze, en klikt **klikt om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:

   ```
   column.0.descriptionkey=name
   ```

   <pre>column.0.link.linkproperty.0.name=ID <br> column.0.link.linkproperty.0.valueField=ID <br> column.0.link.linkproperty.0.valueFormat=int <br> column.0.link.lookup=link.view <br> column.0.link.valueField=objCode <br> column.0.link.valuefat=val <br> column.0.linkedname=direct <br> column.0.listsort=string (naam) <br> column.0.namekey=name.abbr <br> column.0.querysort=name <br> column.0.shortview=false <br> column.0.valueField=name <br> column.0.valueformat=HTML <br> 2} column.0.width=150 <br> column.1.descriptionkey=parent <br> column.1.link.linkproperty.0.name=ID <br> column.1.link.linkproperty.0.valueField=parent:ID <br> column.1.link.linkproperty.0.valueFormat=int <br> column.1.link.lookup=link.view <br> column.1.link.valueField=parent:objCode <br> column.1.link.valueformat=val <br> column.1.linkedname=parent <br> column.1.listsort=nested (ouder).string(naam) <br> column.1.namekey=parent <br> 3} column.1.querysort=parent:name <br> column.1.shortview=false <br> column.1.stretch=0 <br> column.1.valueField=parent:name <br> column.1.valueformat=HTML <br> column.1.width=150 <br> column.2.description=Parc De ouder <br> column.2.link.linkproperty.0.name=ID <br> column.2.link.linkproperty.0.valueField=parent :parent: identiteitskaart <br> column.2.link.linkproperty.0.valueformat=int <br> column.2.link.lookup=link.view <br> column.2.link valueField=parent :parent: objCode <br> column.2.link.valueformat=val <br> column.2.linkedname=parent <br> column.2.listsort=nested (ouder:ouder).string(naam) <br> column.2.name=Parent <br> column.2.querysort=parent 2} naam <br> column.2.shortview=false <br> column.2.stretch=0 <br> column.2.valueField=parent :parent: naam <br> column.2.valueformat=HTML <br> column.2.width=150 <br> column.3.description=Parent Bovenliggend Bovenliggend <br> column.3.link.linkproperty.0.name=ID <br> column.3.link.linkproperty.0.valueField=parent :parent: ouder:ID <br> column.3.link.linkproperty.0.valueformat=int <br> column.3.link.lookup=link.view <br> column.3.link.value field=parent :parent: ouder:objCode <br> column.3.link.valueformat=val <br> column.3.linkedname=parent <br> column.3.listsort=nested (ouder :parent: ouder).string(naam) <br> column.3.name=Parent <br> column.3.querysort=parent :parent: ouder:naam <br> column.3.shortview=false <br> column.3.stretch=0 <br> column.3.valueField=parent :parent: ouder:name <br> column.3.valueformat=HTML <br> column.3.width=150 <br>.4.description=Parent Bovenliggende Ouder <br> column.4.link.linkproperty.0.name=ID <br> column.4.link.linkproperty.0.valueField=parent :parent: ouder :parent: identiteitskaart <br> column.4.link.linkproperty.0.valueformat=int <br> column.4.link.link up=link.view :parent: column.4.link.valueField=parent :parent: ouder :parent: objCode <br> column.4.link.valueformat=val <br> column.4.linkedname=parent <br> column.4.listsort=nested (ouder :parent: ouder:parent).string(naam) <br> 4} column.4.name=Parent Parent Parent Parent <br> column.4.querysort=parent :parent: ouder :parent: naam 88} column.4.shortview=false <br> column.4.stretch=100 <br> column.4.valueField=parent :parent: ouder :parent: naam 93} column.4.valueformat=HTML <br> column.4.width=150<br><br><br></pre>

1. Klik **sparen Mening**.

   De naam van de taak wordt weergegeven in de eerste kolom en als de taak bovenliggende items heeft, worden maximaal vier bovenliggende items weergegeven in de resterende kolommen.
