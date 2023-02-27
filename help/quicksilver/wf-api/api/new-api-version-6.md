---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuw in API-versie 6
description: Nieuw in API-versie 6
author: Becky
feature: Workfront API
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '570'
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

Wijzigingen in bestaande objecten: de toevoegingen worden eenvoudig vermeld, verwijderingen hebben doorhaling, veranderingen in bestaand hebben een nota in bijlage na de lijst

### Bijwerken

 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| updateType¹ |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID² |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

² hasFilters-kenmerk gewijzigd in true

 

### Goedkeuring

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManagers | resourceManagerIDs |   |   |   |
| constraintDate¹ |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Datum van validatie toegevoegd

² NOT_FILTERABLE, markering toegevoegd

 

### Goedkeuringsproces

|   | Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|---|
|  |  | `attachedApprovalPaths` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Goedkeuringsstap

 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| approvalType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

 

### Goedkeuringspad¹

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
| name² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Gewijzigd in Te Rapporteren

² Toegevoegde Max Length Validator

 

### Object voor werkservice

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| constraintDate¹ |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired² |   |   |   | workItemStatusLabels  |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Datum van validatie toegevoegd

² Niet_Filterbare vlag toegevoegd

 

### Toewijzing

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnprojects |   |   |
|   |   |   |   | swapUsersOnProjecten |   |   |
|   |   |   |   | unassignUserFromprojects |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Basislijn 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Niet_filterbare vlag toegevoegd

 

### Basislijntaak

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Niet_filterbare vlag toegevoegd

 

### Factureringsrecord

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| factureringsdatum¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ added NO_TIME field flag

### Burndown-gebeurtenis 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style=&quot;table-layout:auto&quot;}

 

### Categorie 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style=&quot;table-layout:auto&quot;}

 

Aangepaste Enum 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuses |   |
|   |   |   |   | isMogelijkToUnlockStatus | projectGroupStatuses |   |
|   |   |   |   |   | taskGroupStatuses |   |

{style=&quot;table-layout:auto&quot;}

 

Document 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

Wisselkoers 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| rate¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Gewijzigde PRECISION-validator voor 8 t/m 9

 

### Integratie

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Dagboekinvoer

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| changeType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

 

### Optask (Issue)¹ 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Met vlag HERSTELBAAR

² Niet_Filterbare vlag toegevoegd

 

### Project¹ 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManagers | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| werk |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Gemarkeerd als RESTORABLE en RESOURCE_MANAGEABLE

² Niet_Filterbare vlag toegevoegd

 

### Taak¹

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| constraintDate² |   |   |   |   |   |   |
| workRequired³ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Met vlag HERSTELBAAR

² AT_DATE_YEAR_BEFORE validator added

³ Niet_Filterbare vlag toegevoegd

 

### Team

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Template¹ 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   | resourceManagers | resourceManagerIDs |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Gemarkeerd als RESTORABLE en RESOURCE_MANAGEABLE

### Sjabloontaak¹ 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| workRequired² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Met vlag HERSTELBAAR

² Niet_Filterbare vlag toegevoegd

 

### Gebruiker

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| myInfo¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ MAX_LENGTH violators

 

### Opmerking gebruiker

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| eventType¹ |   |   |   |   | myNotifications² |   |

{style=&quot;table-layout:auto&quot;}

¹ Mogelijke waarden gewijzigd

² heeft filters gewijzigd in `[true]`

 

### Aankondiging

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
