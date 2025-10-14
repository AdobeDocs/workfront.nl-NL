---
content-type: api
navigation-topic: api-navigation-topic
title: Updates voor API versie 8
description: Bekijk de updates voor API versie 8.
author: Becky
feature: Workfront API
role: Developer
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# Updates voor API versie 8

## Bijgewerkte bronnen

De volgende bestaande bronnen zijn bijgewerkt met deze versie van de Adobe Workfront API. Om de middelen te bekijken die aan versies 8 nieuw zijn, gelieve te zien [&#x200B; wat in API Versie 8 &#x200B;](../../wf-api/api/new-api-version-8.md) Nieuw is. Wijzigingen in een bron worden als volgt aangegeven:

* Toevoegingen worden gewoon vermeld
* Verwijderingen worden aangegeven met doorhalingstekst
* Wijzigingen worden vermeld in de notitie na de tabel

### AccessRequest

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| actie <sup> 1 </sup>  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> Veranderingen in mogelijke waarden

### AccessRule <sup> 1 </sup> 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| coreAction <sup> 2 </sup>  |   |   |   |   |   |   |
| forbiddenActions <sup>  </sup> |   |   |   |   |   |   |
| secundairActions <sup> 2 </sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> verwijderde vlag: VERSLAGBARE\
<sup> 2 </sup> Veranderingen in mogelijke waarden

### Goedkeuring

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditTypes <sup> 1 </sup> | agileWork  | resourcePools |   |   |   |   |
| backlogOrder <sup> 2 </sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> Veranderingen in mogelijke waarden\
<sup> 2 </sup> toegevoegde vlaggen: DYNAMIC, LAZY_READ, en NOT_GROUPABLE

### Toewijzing

|   |   |   |   | Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnTasks | getAssignAssignmentForTasks  |   |   |   |   |   |
|   |   |   |   | swapUsersOnTasks | getUnassignAssignmentForTasks |   |   |   |   |   |
|   |   |   |   | unassignUserFromTasks |   |   |   |   |   |   |

{style="table-layout:auto"}

### Klant

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| bizRuleExclusions <sup> 1 </sup> |   |   |   | getPackagingOptionValue |   |   |
| proofPlan <sup> 1 </sup> |   |   |   | isPackagingOptionEnabled |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> Veranderingen in mogelijke waarden

### Klantvoorkeuren

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| naam <sup> 1 </sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> Veranderingen in mogelijke waarden

### DocumentApproval

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| identiteitskaart <sup> 1 </sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> toegevoegde vlag: NOT_FILTERABLE

### DocumentVersion

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| activeProofStage |   |   |   |   |   |   |

{style="table-layout:auto"}

### Groep

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   | eigenaars |   |   |   |   |

{style="table-layout:auto"}

### HourType

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| appGlobalID <sup> 1 </sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> toegevoegde vlag: NOT_FILTERABLE

### Iteratie

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   | moveStories |   |   |

{style="table-layout:auto"}

### leuk

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |

{style="table-layout:auto"}

### Opmerking

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditType <sup> 1 </sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> Veranderingen in mogelijke waarden

### OpTask

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditTypes <sup> 1 </sup> | agileWork  |   |   |   | defaultShownTimesheetIssues  |   |
| backlogOrder | herhaling |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| schatten |   |   |   |   |   |   |
| iterationID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> Veranderingen in mogelijke waarden

### Portfolio

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditTypes <sup> 1 </sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> Veranderingen in mogelijke waarden

### Programma

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditTypes <sup> 1 </sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> Veranderingen in mogelijke waarden

### Project

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditTypes <sup> 1 </sup> |   | resourcePools |   |   | defaultShownTimesheetProjecten |   |

{style="table-layout:auto"}

<sup> 1 </sup> Veranderingen in mogelijke waarden

### Goedkeuring proef

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| fiatverID | fiatteur |   |   |   |   |   |
| documentVersionID | documentVersion |   |   |   |   |   |
| identiteitskaart <sup> 1 </sup> |   |   |   |   |   |   |
| proofCreationDate |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> toegevoegde vlag: NOT_FILTERABLE

### QueueDef

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| requestorCoreAction <sup> 1 </sup> |   |   |   |   |   |   |
| requestorForbiddenActions <sup> 1 </sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> Veranderingen in mogelijke waarden

### Snelheid

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| endDate |   |   |   | setRatesForRole  |   |   |
| name |   |   |   |   |   |   |
| startDate |   |   |   |   |   |   |

{style="table-layout:auto"}

### ReservedTime

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| extRefID |   |   |   |   |   |   |

{style="table-layout:auto"}

### ResourceManager

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| projectPriority |   |   |   |   |   |   |

{style="table-layout:auto"}

### Taak

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditTypes <sup> 1 </sup> | agileWork  |   |   |   | allTasksOnIterations  |   |
| backlogParent | kanbanBoard |   |   |   | defaultShownTimesheetTasks |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> Veranderingen in mogelijke waarden

### Team

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| agileMethodology |   |   |   |   |   |   |
| autoAddNextStory |   |   |   |   |   |   |
| includeIssues |   |   |   |   |   |   |
| teamStoryBoardIssueStatuses |   |   |   |   |   |   |
| wipLimit |   |   |   |   |   |   |

{style="table-layout:auto"}

### Sjabloon

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |

{style="table-layout:auto"}

### TemplateTask

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditTypes <sup> 1 </sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> Veranderingen in mogelijke waarden

Bijwerken

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| updateType <sup> 1 </sup> | `updateEndorsement` |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> Veranderingen in mogelijke waarden

### Gebruiker

|   |   | Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |   |   |
|   |   | usergroups |   |   |   |   |   |   |
|   |   | userRoles |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |
| `endorsementShareID` | `endorsementShare` |   |   |   |   |   |
| eventType <sup> 1 </sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> Veranderingen in mogelijke waarden

### Werk

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditTypes <sup> 1 </sup> | agileWork  |   |   |   |   |   |
| backlogOrder <sup> 2 </sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent  |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> Veranderingen in mogelijke waarden\
<sup> 2 </sup> toegevoegde vlaggen: DYNAMIC, LAZY_READ, en NOT_GROUPABLE
