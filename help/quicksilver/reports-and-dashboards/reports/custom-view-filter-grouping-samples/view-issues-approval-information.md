---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Weergave: kwesties met betrekking tot goedkeuringsinformatie"'
description: De volgende probleemweergave toont het goedkeuringsproces, de stap, de namen van de fiatteurs en de status van de kwestie voordat de goedkeuring werd verleend. Sommige van deze gebieden zijn niet toegankelijk door de standaardinterfacebouwer.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4e123844-a0d6-474b-87fb-d30ed391ad07
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# Weergave: kwesties met goedkeuringsinformatie

De volgende probleemweergave toont het goedkeuringsproces, de stap, de namen van de fiatteurs en de status van de kwestie voordat de goedkeuring werd verleend. Sommige van deze gebieden zijn niet toegankelijk door de standaardinterfacebouwer.

![custom_issue_view_with_approval_info.png](assets/custom-issue-view-with-approval-info-350x46.png)

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

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een rapport beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Problemen met goedkeuringsgegevens weergeven

1. Ga naar een lijst met problemen.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Nieuwe weergave**.

1. In de **Kolomvoorvertoning** gebied, alle kolommen behalve één verwijderen.
1. Klik op de koptekst van de resterende kolom en klik vervolgens op **Overschakelen naar tekstmodus**.
1. Plaats de muis boven het gebied in de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:
   <pre style="font-style: normal;">column.0.descriptionKey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.lookup=link.view<br>column.0.link.valueField=objCode<br>column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=40<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=220<br>column.1.descriptionkey=assigned to<br>column.1.linkedname=assignedTo<br>column.1.listsort=nested(assignedTo).string(name)<br>column.1.namekey=assigned to<br>column.1.querysort=assignedTo:name<br>column.1.shortview=true<br>column.1.stretch=0<br>column.1.valueField=assignedTo:name<br>column.1.valueFormat=HTML<br>column.1.width=150<br>column.2.descriptionkey=role<br>column.2.linkedname=role<br>column.2.listsort=nested(role).string(name)<br>column.2.namekey=role<br>column.2.querysort=role:name<br>column.2.shortview=false<br>column.2.stretch=25<br>column.2.valueField=role:name<br>column.2.valueFormat=HTML<br>column.2.width=150<br>column.3.description=Approval Process Name<br>column.3.linkedname=direct<br>column.3.listsort=string(name)<br>column.3.name=Approval Process Name<br>column.3.querysort=name<br>column.3.shortview=false<br>column.3.stretch=35<br>column.3.valueField=approvalProcess:name<br>column.3.valueFormat=HTML<br>column.3.width=220<br>column.4.description=Approval Step Name<br>column.4.linkedname=direct<br>column.4.listsort=string(name)<br>column.4.name=Approval Step Name<br>column.4.querysort=name<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valueField=currentApprovalStep:name<br>column.4.valueFormat=HTML<br>column.4.width=220<br>column.5.description=Previous Status<br>column.5.linkedname=direct<br>column.5.listsort=string(name)<br>column.5.name=Previous Status<br>column.5.querysort=name<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valueField=previousStatus<br>column.5.valueFormat=HTML<br>column.5.width=220<br>column.6.linkedname=direct<br>column.6.listsort=HTML(ApproversString)<br>column.6.namekey=fiatver.plural.abbr<br>column.6.querysort=ApproversString<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valueField=ApproversString<br>column.6.valueFormat=HTML<br>column.6.viewalias=Approver.plural<br>column.6.width=200<br></pre>

1. Klikken **Weergave opslaan**.
