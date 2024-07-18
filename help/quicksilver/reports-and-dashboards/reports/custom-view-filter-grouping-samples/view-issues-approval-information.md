---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergeven: problemen met goedkeuringsinformatie'
description: De volgende probleemweergave toont het goedkeuringsproces, de stap, de namen van de fiatteurs en de status van de kwestie voordat de goedkeuring werd verleend. Sommige van deze gebieden zijn niet toegankelijk door de standaardinterfacebouwer.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4e123844-a0d6-474b-87fb-d30ed391ad07
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Weergeven: problemen met goedkeuringsinformatie

De volgende probleemweergave toont het goedkeuringsproces, de stap, de namen van de fiatteurs en de status van de kwestie voordat de goedkeuring werd verleend. Sommige van deze gebieden zijn niet toegankelijk door de standaardinterfacebouwer.

![ custom_issue_view_with_approval_info.png ](assets/custom-issue-view-with-approval-info-350x46.png)

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

## Problemen met goedkeuringsgegevens weergeven

1. Ga naar een lijst met problemen.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom, dan klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over het gebied van de tekstwijze, en klikt **klikt om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:
   <pre style="font-style: normal;">column.0.descriptionkey=name <br> column.0.link.linkproperty.0.name=ID <br> column.0.link.linkproperty.0.valueField=ID <br> column.0.link.linkproperty.0.valueformat=int <br> column.0.link.lookup=link.view <br> column.0.link.valueField=objCode 5} column.0.link.valueformat=val <br> column.0.linkedname=direct <br> column.0.listsort=string(name) <br> column.0.namekey=name.abbr <br> column.0.querysort=name <br> column.0.shortview=false <br> column.0.stretch=40 <br> column.0.valueField=name <br> column.0.valueformat=HTML <br> column.0.width=220 <br> column.1.descriptionkey=assigned to <br> column.1.linkedname=assignedTo <br> column.1.listsort=nested(assignedTo).string(name) 18} column.1.namekey=assigned to <br> column.1.querysort=assignedTo:name <br> column.1.shortview=true <br> column.1.stretch=0 <br> column.1.valueField=assignedTo:name <br> column.1.valueformat=HTML <br>.1.width=150 <br> column.2.descriptionkey=rol <br> column.2.linkedname=rol <br> column.2.listsort=nested (rol).string(naam) <br> column.2.namekey=rol <br> column.2.querysort=role:name <br> column.2.shortview=false <br> column.2.stretch=25 <br> column.2.valuefield=rol:name <br> column.2.valueformat=HTML <br> column.2.width=150 <br> column.3.description=Approval Naam van het Proces <br> column.3.linkedname=direct <br> 3.listsort=string (naam) <br> column.3.name=Approval Naam van het Proces <br> column.3.querysort=name <br> column.3.shortview=false <br> column.3.stretch=35 <br> column.3.valueField=approvalProcess:name <br> column.3.valueformat=HTML <br> column.3.width=220 <br> column.4.description=Approval Step Name <br> column.4.linkedname=direct <br> column.4.listsort=string(name) <br> column.4.name=Approval Naam van de Stap van de Stap <br> column.4.querysort=name <br> column.4.shortview=false <br> column.4.stretch=0 <br> column.4.valueField=currentApprovalStep:name <br> column.4.valueFormat=HTML <br> column.4.width=220 <br> column.5.description=Previous Status <br> column.5.linkedname=direct <br>.5.listsort=string (naam) <br> column.5.name=Previous Status <br> column.5.querysort=name <br> column.5.shortview=false <br> column.5.stretch=0 <br> column.5.valuefield=previousStatus <br> column.5.valueformat=HTML <br> column.5.width=220 <br> column.6.linkedname=direct <br> column.6.listsort=HTML (ApproversString) <br> column.6.namekey=fiver.plural.abbr <br> column.6.querysort=ApproversString <br> column.6.shortview=false <br> 0} column.6.stretch=0 <br> column.6.valueField=ApproversString <br> column.6.valueformat=HTML <br> column.6.viewalias=Approver.plural <br> column.6.width=200<br><br><br></pre>

1. Klik **sparen Mening**.
