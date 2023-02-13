---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Weergave: de informatie van het programma en van de Portfolio van de vertoning in een taakmening"'
description: Deze taakmening toont het Programma en de Portfolio die met het project van de taak worden geassocieerd. Deze informatie is niet beschikbaar in de rapportaannemer wanneer het bouwen van een taakmening. Deze informatie is alleen beschikbaar in de tekstmodus.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cdd5a1e9-3cbf-4951-b803-fca544b2519a
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---

# Weergave: programma- en Portfolio-informatie weergeven in een taakweergave

Deze taakmening toont het Programma en de Portfolio die met het project van de taak worden geassocieerd. Deze informatie is niet beschikbaar in de rapportaannemer wanneer het bouwen van een taakmening. Deze informatie is alleen beschikbaar in de tekstmodus.

De weergave bevat ook koppelingen naar het project, het programma en de Portfolio vanuit een takenlijst.

![](assets/view--program-and-portfolio-350x116.png)

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

## Programma- en Portfolio-informatie weergeven in een taakweergave

Deze weergave toepassen op een takenlijst:

1. Ga naar een takenlijst.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Nieuwe weergave**.

1. In de **Kolomvoorvertoning** gebied, alle kolommen behalve één verwijderen.
1. Klik op de koptekst van de resterende kolom en klik vervolgens op **Overschakelen naar tekstmodus**.
1. Plaats de muis boven het gebied in de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:
   <pre>column.0.descriptionKey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.lookup=link.view<br>column.0.link.valueField=objCode<br>column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=150<br>column.1.descriptionkey=project<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valueField=project:ID<br>column.1.link.linkproperty.0.valueFormat=int<br>column.1.link.lookup=link.view<br>column.1.link.valueField=project:objCode<br>column.1.link.valueFormat=val<br>column.1.linkedname=project<br>column.1.listsort=nested(project).string(name)<br>column.1.namekey=project<br>column.1.querysort=project:name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valueField=project:name<br>column.1.valueFormat=HTML<br>column.1.width=150<br>column.2.descriptionkey=program<br>column.2.displayName=Program<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valueField=project:program:ID<br>column.2.link.linkproperty.0.valueFormat=int<br>column.2.link.lookup=link.view<br>column.2.link.valueField=project:program:objCode<br>column.2.link.valueFormat=val<br>column.2.linkedname=project<br>column.2.listsort=nested(project:program).string(name)<br>column.2.namekey=project<br>column.2.querysort=project:program:name<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valueField=project:program:name<br>column.2.valueFormat=HTML<br>column.2.width=150<br>column.3.descriptionKey=portfolio<br>column.3.displayName=Portfolio<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valueField=project:portfolio:ID<br>column.3.link.linkproperty.0.valueFormat=int<br>column.3.link.lookup=link.view<br>column.3.link.valueField=project:portfolio:objCode<br>column.3.link.valueFormat=val<br>column.3.linkedname=project<br>column.3.listsort=nested(project:portfolio).string(name)<br>column.3.namekey=project<br>column.3.querysort=project:portfolio:name<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valueField=project:portfolio:name<br>column.3.valueFormat=HTML<br>column.3.width=150 </pre>

1. Klikken **Weergave opslaan**.
