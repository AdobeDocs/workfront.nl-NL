---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergeven: uitgebreide gebruikersgegevens'
description: In deze gebruikersweergave wordt informatie over uw gebruikers weergegeven. Naast hun naam, toegangsniveaus, en Bedrijf, toont het ook lijsten van hun Groepen, Teams, en de Rollen van de Baan.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a978b43-4718-43fb-80b8-844b35e09d06
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%

---

# Weergeven: uitgebreide gebruikersgegevens

<!--Audited: 11/2024-->

In deze gebruikersweergave wordt informatie over uw gebruikers weergegeven. Naast hun naam, toegangsniveaus, en Bedrijf, toont het ook lijsten van hun Groepen, Teams, en de Rollen van de Baan.

![ extended_user_view.png ](assets/expanded-user-view-350x75.png)

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

## Uitgebreide gebruikersgegevens weergeven

Deze weergave toepassen:

1. Ga naar een lijst met gebruikers.
1. Van het **drop-down menu van de Mening**, uitgezochte **Nieuwe Mening**.

1. In het **gebied van de Voorproef van de Kolom**, elimineer alle kolommen behalve één.
1. Klik de kopbal van de resterende kolom, dan klik **Schakelaar aan de Wijze van de Tekst** > **geeft de Wijze van de Tekst** uit.
1. Verwijder de tekst u in het **vindt dit vakje van de Wijze van de Tekst**, en vervang het met de volgende code:

   ```
   column.0.descriptionkey=name 
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=0
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=accesslevel
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=accessLevel:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=accessLevel:objCode
   column.1.link.valueformat=val
   column.1.linkedname=accessLevel
   column.1.listsort=string(displayName)
   column.1.namekey=accesslevel
   column.1.querysort=name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=accessLevel:displayName
   column.1.valueformat=HTML
   column.1.viewalias=accessLevel:displayName
   column.1.width=100
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.value=val(objCode)
   column.2.listdelimiter=
   column.2.listmethod=nested(userGroups).lists
   column.2.namekey=group.plural
   column.2.stretch=50
   column.2.type=iterate
   column.2.valuefield=group:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.displayname=Teams
   column.3.listdelimiter=
   column.3.listmethod=nested(teams).lists
   column.3.textmode=true
   column.3.type=iterate
   column.3.valueexpression={name}
   column.3.valueformat=HTML
   column.4.link.linkproperty.0.name=ID
   column.4.link.linkproperty.0.valuefield=ID
   column.4.link.linkproperty.0.valueformat=int
   column.4.link.lookup=link.view
   column.4.link.value=val(objCode)
   column.4.listdelimiter=
   column.4.listmethod=nested(userRoles).lists
   column.4.namekey=jobrole.plural
   column.4.stretch=50
   column.4.type=iterate
   column.4.valuefield=role:name
   column.4.valueformat=HTML
   column.4.width=150
   column.5.descriptionkey=company
   column.5.link.linkproperty.0.name=ID
   column.5.link.linkproperty.0.valuefield=company:ID
   column.5.link.linkproperty.0.valueformat=int
   column.5.link.lookup=link.view
   column.5.link.valuefield=company:objCode
   column.5.link.valueformat=val
   column.5.linkedname=company
   column.5.listsort=nested(company).string(name)
   column.5.namekey=company
   column.5.querysort=company:name
   column.5.shortview=false
   column.5.stretch=0
   column.5.valuefield=company:name
   column.5.valueformat=HTML
   column.5.width=150
   ```

1. Klik **Gedaan** > **sparen Mening**.
