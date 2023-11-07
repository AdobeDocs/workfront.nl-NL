---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuw in API-versie 6
description: Nieuw in API-versie 6
author: Becky
feature: Workfront API
role: Developer
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Nieuw in API-versie 6

## Nieuwe objecten

### Resource Manager

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID | klant |   |   |   |   | Toevoegen |
| customerID | project |   |   |   |   | Aantal |
| projectID | resourceManager |   |   |   |   | Verwijderen |
| resourceManagerID | template |   |   |   |   | Get |
| templateID |   |   |   |   |   | Rapport  |
|   |   |   |   |   |   | Zoeken  |


### Ews

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | uploaden |   |
| handgreep |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### Aangepast label

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | Toevoegen |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | Aantal |
|   |   |   |   | removeCustomLabel |   | Verwijderen |
|   |   |   |   |   |   | Get |
|   |   |   |   |   |   | Rapport |
|   |   |   |   |   |   | Zoeken |


## Bijgewerkte objecten

Wijzigingen in bestaande objecten: toevoegingen worden gewoon weergegeven, verwijderingen zijn doorgehaald, wijzigingen in bestaande objecten hebben een gekoppelde notitie na de tabel

### Bijwerken

 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Wijzigingen in mogelijke waarden

<sup>2</sup> hasFilters-kenmerk gewijzigd in true

 

### Goedkeuring

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManagers | resourceManagerIDs |   |   |   |
| constraintDate<sup>1</sup> |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Validatie van datum toegevoegd

<sup>2</sup> NOT_FILTERABLE, markering toegevoegd

 

### Goedkeuringsproces

|   | Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### Goedkeuringsstap

 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Wijzigingen in mogelijke waarden

 

### Goedkeuringspad<sup>1</sup>

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| selectedStatus |   |   |   |   |   | Toevoegen |
| selectedStatusLabel |   |   |   |   |   | Aantal |
| opmerking |   |   |   |   |   | Verwijderen |
| enteredByID |   |   |   |   |   | Bewerken |
| entryDate |   |   |   |   |   | Get |
| globalPathID |   |   |   |   |   | Rapport |
| isPrivate |   |   |   |   |   | Zoeken |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| name<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Gewijzigd in Te Rapporteren

<sup>2</sup> Validator voor Max. lengte toegevoegd

 

### Object voor werkservice

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired<sup>2</sup> |   |   |   | workItemStatusLabels  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Datum van validatie toegevoegd

<sup>2</sup> Niet_filterbare vlag toegevoegd

 

### Toewijzing

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnprojects |   |   |
|   |   |   |   | swapUsersOnProjecten |   |   |
|   |   |   |   | unassignUserFromprojects |   |   |

{style="table-layout:auto"}

 

### Basislijn 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Niet_filterbare vlag toegevoegd

 

### Basislijntaak

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Niet_filterbare vlag toegevoegd

 

### Factureringsrecord

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| factureringsdatum<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> markering toegevoegd NO_TIME-veld

### Burndown-gebeurtenis 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style="table-layout:auto"}

 

### Categorie 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style="table-layout:auto"}

 

Aangepaste Enum 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuses |   |
|   |   |   |   | isMogelijkToUnlockStatus | projectGroupStatuses |   |
|   |   |   |   |   | taskGroupStatuses |   |

{style="table-layout:auto"}

 

Document 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

Wisselkoers 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| tarief<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Gewijzigde PRECISION-validator voor 8-9

 

### Integratie

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Dagboekinvoer

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Wijzigingen in mogelijke waarden

 

### Optask (probleem)<sup>1</sup> 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Met vlag gemarkeerd als HERSTELBAAR

<sup>2</sup> Niet_filterbare vlag toegevoegd

 

### Project<sup>1</sup> 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManagers | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| werk |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Met vlag gemarkeerd als RESTORABLE en RESOURCE_MANAGEABLE

<sup>2</sup> Niet_filterbare vlag toegevoegd

 

### Taak<sup>1</sup>

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |   |   |   |   |   |   |
| workRequired<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Met vlag gemarkeerd als HERSTELBAAR

<sup>2</sup> AT_DATE_YEAR_BEFORE-validator toegevoegd

<sup>3</sup> Niet_filterbare vlag toegevoegd

 

### Team

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### Sjabloon<sup>1</sup> 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   | resourceManagers | resourceManagerIDs |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Met vlag gemarkeerd als RESTORABLE en RESOURCE_MANAGEABLE

### Sjabloontaak<sup>1</sup> 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Met vlag gemarkeerd als HERSTELBAAR

<sup>2</sup> Niet_filterbare vlag toegevoegd

 

### Gebruiker

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> MAX_LENGTH-overtreders

 

### Opmerking gebruiker

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| eventType<sup>1</sup> |   |   |   |   | myNotifications<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> Mogelijke waarden gewijzigd

<sup>2</sup> heeft filters Gewijzigd in `[true]`

 

### Aankondiging

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
