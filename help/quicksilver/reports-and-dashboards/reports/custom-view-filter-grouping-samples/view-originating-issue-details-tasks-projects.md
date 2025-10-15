---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: details van oorsprong van uitgave voor taken en projecten'
description: Wanneer een kwestie in een taak of een project wordt omgezet wordt een het oplossen van objecten verhouding gevestigd tussen de taak of het project en de kwestie. In deze weergave worden de velden van de uitgave weergegeven die automatisch worden voltooid wanneer de taak of het project is voltooid.
author: Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Weergave: details over de oorsprong van taken en projecten

<!--Audited: 11/2024-->

Wanneer een kwestie in een taak of een project wordt omgezet wordt een het oplossen van objecten verhouding gevestigd tussen de taak of het project en de kwestie. In deze weergave worden de volgende velden van de uitgave weergegeven die automatisch worden voltooid wanneer de taak of het project is voltooid:

* Naam
* Invoerdatum
* Geplande afsluitdatum
* Werkelijke afsluitdatum
* Type aanvraag
* Naam van maker
* Toegewezen aan gebruiker

![ task_with_resolving_issue_fields.png ](assets/task-with-resolving-issue-fields-350x38.png)

Voor meer informatie, zie ook [ Mening: toon originele uitgifteinformatie over taak of projectlijsten ](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Medewerker of verzoek om een weergave te wijzigen </p>
   <p>Standaard of Plan om een rapport te wijzigen</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Uitstekende details voor taken en projecten weergeven

1. Ga naar een lijst met taken of een lijst met projecten.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.
1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom en klik **Schakelaar aan de Wijze van de Tekst**, dan **geeft de Wijze van de Tekst** uit.
1. Verwijder de tekst u in **vindt geef de Wijze van de Tekst** vakje uit, en vervang het met de volgende code:

   ```
   column.0.textmode=false
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.descriptionkey=name
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.width=150
   column.1.displayname=Resolvables (Issues)
   column.1.listdelimiter=
   column.1.listmethod=nested(resolvables).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression={name}
   column.1.valueformat=HTML
   column.2.displayname=Resolvables Entry Date
   column.2.listdelimiter=
   column.2.listmethod=nested(resolvables).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={entryDate}
   column.2.valueformat=HTML
   column.3.displayname=Resolvables Due Date
   column.3.listdelimiter=
   column.3.listmethod=nested(resolvables).lists
   column.3.textmode=true
   column.3.type=iterate
   column.3.valueexpression={plannedCompletionDate}
   column.3.valueformat=HTML
   column.4.displayname=Resolvables Actual Completion Date
   column.4.listdelimiter=
   column.4.listmethod=nested(resolvables).lists
   column.4.textmode=true
   column.4.type=iterate
   column.4.valueexpression={actualCompletionDate}
   column.4.valueformat=HTML
   column.5.displayname=Resolvables Request Type
   column.5.listdelimiter=
   column.5.listmethod=nested(resolvables).lists
   column.5.textmode=true
   column.5.type=iterate
   column.5.valueexpression={opTaskType}
   column.5.valueformat=HTML
   column.6.displayname=Resolvables Originator
   column.6.listdelimiter=
   column.6.listmethod=nested(resolvables).lists
   column.6.textmode=true
   column.6.type=iterate
   column.6.valueexpression={owner}.{name}
   column.6.valueformat=HTML
   column.7.descriptionkey=assignedto
   column.7.linkedname=assignedTo
   column.7.listsort=nested(assignedTo).string(name)
   column.7.namekey=assignedto
   column.7.querysort=assignedTo:name
   column.7.shortview=false
   column.7.stretch=0
   column.7.textmode=true
   column.7.valuefield=assignedTo:name
   column.7.valueformat=HTML
   column.7.width=150
   ```

1. Klik **Gedaan** > **sparen Mening**.
