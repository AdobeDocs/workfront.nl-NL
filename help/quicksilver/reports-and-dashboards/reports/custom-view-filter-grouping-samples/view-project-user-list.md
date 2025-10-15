---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: Lijst met projectgebruikers met taakrollen'
description: U kunt deze mening in een projectlijst of een rapport toepassen om een lijst van gebruikers te tonen die met het project, evenals een lijst van de baanrollen worden geassocieerd zij op het project uitvoeren.
author: Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Weergave: lijst met projectgebruikers met taakrollen

<!--Audited: 11/2024-->

U kunt deze mening in een projectlijst of een rapport toepassen om een lijst van gebruikers te tonen die met het project, evenals een lijst van de baanrollen worden geassocieerd zij op het project uitvoeren.

De informatie in dit verslag is ook te vinden in het gebied Mensen van het project.

>[!TIP]
>
>Als geen baanrollen voor de gebruikers maar u weten dat zij met baanrollen in hun gebruikersprofielen worden geassocieerd, zou dit kunnen betekenen zij aan taken en kwesties worden toegewezen maar zij zouden niet met een baanrol op de taak of de kwestie kunnen worden geassocieerd, of de gebruikers die in het rapport worden vermeld zijn niet de toegewezen taken en kwesties, maar vervullen andere rollen op het project (bijvoorbeeld, Eigenaar of Sponsor.)

![ project_with_user_and_role_information_report.png ](assets/project-with-user-and-role-information-report-350x100.png)

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


## Een lijst met projectgebruikers met taakrollen weergeven

1. Ga naar een lijst met projecten.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.
1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom, dan klik **Schakelaar aan de Wijze van de Tekst** > **geeft de Wijze van de Tekst** uit.
1. Verwijder de tekst u in **vindt geef de Wijze van de Tekst** vakje uit, en vervang het met de volgende code:

   ```
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.section=0
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=200
   column.1.displayname=Project Users
   column.1.listdelimiter=<br>
   column.1.listmethod=nested(projectUsers).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression={user}.{name}
   column.1.valueformat=HTML
   column.2.displayname=Project Roles
   column.2.listdelimiter=<br>
   column.2.listmethod=nested(projectUserRoles).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={role}.{name}
   column.2.valueformat=HTML
   ```

1. Klik **Gedaan** > **sparen Mening**.
