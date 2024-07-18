---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "View: assigned user's Company and Home Group"
description: Deze taakmening toont het Bedrijf en de Groep van het Huis van de Primaire Eigenaar van de taak. Dit zijn waarden die niet beschikbaar zijn in de standaardinterface, maar die wel toegankelijk zijn via de tekstmodus.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Weergave: bedrijf en thuisgroep van toegewezen gebruiker

Deze taakmening toont het Bedrijf en de Groep van het Huis van de Primaire Eigenaar van de taak. Dit zijn waarden die niet beschikbaar zijn in de standaardinterface, maar die wel toegankelijk zijn via de tekstmodus.

![](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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

## Bedrijf en thuisgroep van toegewezen gebruiker weergeven

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom, dan klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over het gebied van de tekstwijze, en klikt **klikt om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:
   <pre>column.0.descriptionkey=name <br> column.0.link.linkproperty.0.name=ID <br> column.0.link.linkproperty.0.valueField=ID <br> column.0.link.linkproperty.0.valueFormat=int <br> column.0.link.lookup=link.view <br> column.0.link.valueField=objCode 5} column.0.link.valueFormat=val <br> column.0.linkedname=direct <br> column.0.listsort=string(name) <br> column.0.namekey=name.abbr <br> column.0.querysort=name <br> column.0.shortview=false <br> column.0.stretch=100 <br> 2} column.0.valueField=name <br> column.0.valueFormat=HTML <br> column.0.width=150 <br> column.1.descriptionKey=assigned to <br> column.1.link.linkproperty.0.name=ID <br> column.1.link.linkproperty.0.valueField=assignedTo:ID <br> column.1.link.linkproperty.0.valueformat=int <br> column.1.link.lookup=link.view <br> column.1.link.valueField=assignedTo:objCode <br> column.1.link.valueFormat=val <br> toegewezen column.1.linkedname=Aan <br> column.1.listsort=nested(assignedTo).string(name) <br> column.1.namekey=assigned to <br> column.1.querysort=assignedTo:name <br> column.1.shortview=false <br> column.1.stretch=0 <br> column.1.valueField assignedTo:name <br> column.1.valueformat=HTML <br> column.1.width=150 <br> column.2.description=Assigned to Company <br> column.2.displayname=Assigned to Company <br> column.2.linkedname=assignedTo:company <br> column.2.listsort=neto sted (assignedTo:company).string(name) <br> column.2.namekey=assigned to <br> column.2.querysort=assignedTo :company: name <br> column.2.shortview=false <br> column.2.stretch=0 <br> column.2.valueField=assignedTo :company: <br> column.2.valueformat=HTML <br> column.2.width=150 <br> column.3.description=Assigned to Home Group <br> column.3.displayname=Assigned to Home Group <br> column.3.linkedname=assignedTo:homeGroup <br> column.3.listsort=nested (assignedTo:homeGroup).string(naam) <br> column.3.namekey=assigned to <br> column.3.querysort=assignedTo :homeGroup: naam <br> column.3.shortview=false <br> column.3.stretch=0 <br> column.3.valueField=assignedTo :homeGroup: name<br> column.3.valueFormat=HTML <br> column.3.width=150<br></pre>

1. Klik **sparen Veranderingen**.
