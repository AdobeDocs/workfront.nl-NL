---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: geef Program- en Portfolio-informatie weer in een taakweergave.'
description: Deze taakmening toont het Programma en het Portfolio die met het project van de taak worden geassocieerd. Deze informatie is niet beschikbaar in de rapportaannemer wanneer het bouwen van een taakmening. Deze informatie is alleen beschikbaar in de tekstmodus.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cdd5a1e9-3cbf-4951-b803-fca544b2519a
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Weergave: informatie over programma en Portfolio weergeven in een taakweergave

Deze taakmening toont het Programma en het Portfolio die met het project van de taak worden geassocieerd. Deze informatie is niet beschikbaar in de rapportaannemer wanneer het bouwen van een taakmening. Deze informatie is alleen beschikbaar in de tekstmodus.

De weergave bevat ook koppelingen naar het project, het programma en het Portfolio in een takenlijst.

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

## Programma- en Portfolio-informatie weergeven in een taakweergave

Deze weergave toepassen op een takenlijst:

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom, dan klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over het gebied van de tekstwijze, en klikt **klikt om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:
   <pre>column.0.descriptionkey=name <br> column.0.link.linkproperty.0.name=ID <br> column.0.link.linkproperty.0.valueField=ID <br> column.0.link.linkproperty.0.valueformat=int <br> column.0.link.lookup=link.view <br> column.0.link.valueField=objCode 5} column.0.link.valueformat=val <br> column.0.linkedname=direct <br> column.0.listsort=string(naam) <br> column.0.namekey=name.abbr <br> column.0.querysort=name <br> column.0.shortview=false <br> column.0.stretch=100 {1 2} column.0.valueField=name <br> column.0.valueformat=HTML <br> column.0.width=150 <br> column.1.descriptionkey=project <br> column.1.link.linkproperty.0.name=ID <br> column.1.link.linkproperty.0.valuefield=project ID <br> column.1.link.linkproperty.0.valueformat=int <br> column.1.link.lookup=link.view <br> column.1.link.valuefield=project:objCode <br> column.1.link.valueformat=val <br> column.1.linkedname=project <br> 1.listsort=nested (project).string(naam) <br> column.1.namekey=project <br> column.1.querysort=project:name <br> column.1.shortview=false <br> column.1.stretch=0 <br> column.1.valueField=project:name <br> column.1.valuefat=HTML <br> column.1.width=150 <br> column.2.descriptionkey=program <br> column.2.displayname=Program <br> column.2.link.linkproperty.0.name=ID <br> column.2.link.linkproperty.0.valueField=project :program: identiteitskaart <br>.2.link.linkproperty.0.valueformat=int <br> column.2.link.lookup=link.view <br> column.2.link.valuefield=project :program: objCode <br> column.2.link.valueformat=val <br> column.2.linkedname=project <br> column.2.2. sort=nested (project:programma).string(naam) <br> column.2.namekey=project <br> column.2.querysort=project :program: naam <br> column.2.shortview=false <br> column.2.stretch=0 <br> column.2.valueField=project :program: naam <br>.2.valueformat=HTML <br> column.2.width=150 <br> column.3.descriptionkey=portfolio <br> column.3.displayname=Portfolio <br> column.3.link.linkproperty.0.name=ID <br> column.3.link.linkproperty.0.valueField=project :portfolio: Identiteitskaart <br> column.3.link.linkproperty.0.valueformat=int <br> column.3.link.lookup=link.view <br> column.3.link.valuefield=project :portfolio: objCode <br> column.3.link.valueformat=val <br> column.3.linkedname=project {6 3} column.3.listsort=nested (project:portefeuille).string(naam) <br> column.3.namekey=project <br> column.3.querysort=project :portfolio: naam 67} column.3.shortview=false <br> column.3.stretch=0 <br> column.3.valueField=project :portfolio: <br> column.3.valueformat=HTML <br> column.3.width=150 <br><br><br><br></pre>

1. Klik **sparen Mening**.
