---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: details voorganger'
description: Deze taakmening toont details van predecessors van de taken gebruikend een inzamelingsmening. In een verzamelingsweergave kunt u informatie weergeven over objecten die een 'een-op-veel'-relatie hebben. In dit geval kan elke taak (één) meerdere voordecessors (vele) hebben. De weergave bevat de naam van de taken, de namen van de voorgangers, de projectnamen van de voorgangers, de geplande afsluitdatums van de voorgangers en de statussen van de voorgangers.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# Weergave: details voorganger

Deze taakmening toont details van predecessors van de taken gebruikend een inzamelingsmening. In een verzamelingsweergave kunt u informatie weergeven over objecten die een &#39;een-op-veel&#39;-relatie hebben. In dit geval kan elke taak (één) meerdere voordecessors (vele) hebben. De weergave bevat de naam van de taken, de namen van de voorgangers, de projectnamen van de voorgangers, de geplande afsluitdatums van de voorgangers en de statussen van de voorgangers.

Voor informatie over het van verwijzingen voorzien van inzamelingen in rapporten, zie [Referentieverzamelingen in een rapport](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![predecessor_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

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

## Details voorganger weergeven

1. Ga naar een takenlijst.
1. Van de **Weergave** vervolgkeuzelijst, selecteert u **Nieuwe weergave**.

1. In de **Kolomvoorvertoning** gebied, alle kolommen behalve één verwijderen.
1. Klik op de koptekst van de resterende kolom en klik vervolgens op **Overschakelen naar tekstmodus**.
1. Plaats de muis boven het gebied in de tekstmodus en klik op **Klik om tekst te bewerken**.
1. Verwijder de tekst die u vindt in het dialoogvenster **Tekstmodus** en vervang deze door de volgende code:
   <pre>column.0.displayName=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.1.displayName=Predecessors Nummers &amp; Names<br>column.1.listdelimiter=<br><br>column.1.listmethod=nested(predecessors).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression=CONCAT({predecessor}.{taskNumber},' - ',{predecessor}.{name})<br>column.1.valueFormat=HTML<br>column.2.displayName=Predecessors Projectnamen<br>column.2.listdelimiter=<br><br>column.2.listmethod=nested(predecessors).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={predecessor}.{project}.{name}<br>column.2.valueFormat=HTML<br>column.3.displayName=Predecessors Voltooiingsdatums<br>column.3.listdelimiter=<br><br>column.3.listmethod=nested(predecessors).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={predecessor}.{scheduledCompletionDate}<br>column.3.valueFormat=HTML<br>column.4.displayName=Predecessors Status<br>column.4.listdelimiter=<br><br>column.4.listmethod=nested(predecessors).lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.valueexpression={predecessor}.{status}<br>column.4.valueFormat=HTML</pre>

1. Klikken **Weergave opslaan**.
