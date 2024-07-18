---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: voorganger-details'
description: Deze taakmening toont details van predecessors van de taken gebruikend een inzamelingsmening. In een verzamelingsweergave kunt u informatie weergeven over objecten die een 'een-op-veel'-relatie hebben. In dit geval kan elke taak (één) meerdere voordecessors (vele) hebben. De weergave bevat de naam van de taken, de namen van de voorgangers, de projectnamen van de voorgangers, de geplande afsluitdatums van de voorgangers en de statussen van de voorgangers.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Weergave: details van vorige versie

Deze taakmening toont details van predecessors van de taken gebruikend een inzamelingsmening. In een verzamelingsweergave kunt u informatie weergeven over objecten die een &#39;een-op-veel&#39;-relatie hebben. In dit geval kan elke taak (één) meerdere voordecessors (vele) hebben. De weergave bevat de naam van de taken, de namen van de voorgangers, de projectnamen van de voorgangers, de geplande afsluitdatums van de voorgangers en de statussen van de voorgangers.

Voor informatie over het van verwijzingen voorzien van inzamelingen in rapporten, zie [ inzamelingen van de Verwijzing in een rapport ](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![ predecessor_details_task_view.png ](assets/predecessor-details-task-view-350x34.png)

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

## Details voorganger weergeven

1. Ga naar een takenlijst.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom, dan klik **Schakelaar aan de Wijze van de Tekst**.
1. De muis over het gebied van de tekstwijze, en klikt **klikt om tekst** uit te geven.
1. Verwijder de tekst u in het **vakje van de Wijze van de Tekst** vindt, en vervang het met de volgende code:
   <pre>column.0.displayname= <br> column.0.linkedname=direct <br> column.0.namekey=name <br> column.0.querysort=name <br> column.0.valueField=name <br> column.0.valueformat=HTML <br> column.1.displayname=Predecessors Numbers &amp; Names <br> column.1.listimdelimdelimdeln iter= <br><br> column.1.listmethod=nested (predecessors).lists <br> column.1.textmode=true <br> column.1.type=iterate <br> column.1.valueexpression=CONCAT ({predecessor}.{taskNumber},' - ',{predecessor}.{name}) <br> column.1.valueformat=HTML <br> column.2.displayname=Predecessors de Namen van het Project <br> column.2.listdelimiter= <br><br> column.2.listmethod=nested (predecessors).lists <br> column.2.textmode=true <br> column.2.type=iterate <br> column.2.value={predecessor}.{project}.{name} <br> column.2.valueformat=HTML <br> column.3.displayname=PredecessorsVoltooiingsdata <br> column.3.listdelimiter= <br><br> column.3.listmethod=nested (predecessors).lists <br> column.3.textmode=true <br> column.3.type=iterate <br> column.3.valueexpression={predecessor}.{plannedCompletionDate} <br> column.3.valueformat=HTML <br> column.4.displayname=Predecessors Status <br> column.4.listdelimiter= <br><br> column.4.listmethod=nested (predecessors).lists <br> column.4.textmode=true <br> column.4.type=iterate <br> column.4.valueexpression= {predecessor}.{status} <br> column.4.valueformat=HTML</pre>

1. Klik **sparen Mening**.
