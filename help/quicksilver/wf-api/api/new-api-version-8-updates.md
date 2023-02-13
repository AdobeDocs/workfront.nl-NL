---
content-type: api
navigation-topic: api-navigation-topic
title: Updates voor API versie 8
description: 'De volgende bestaande bronnen zijn bijgewerkt met deze versie van de Adobe Workfront API. Zie Nieuwe functies in API-versie 8 voor informatie over de bronnen die nieuw zijn voor versie 8. Wijzigingen in een bron worden als volgt aangegeven: BEWERK ME.'
author: John
feature: Workfront API
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 0%

---

# Updates voor API versie 8

## Bijgewerkte bronnen

De volgende bestaande bronnen zijn bijgewerkt met deze versie van de Adobe Workfront API. Als u de bronnen wilt bekijken die nieuw zijn voor versie 8, raadpleegt u [Nieuw in API-versie 8](../../wf-api/api/new-api-version-8.md). Wijzigingen in een bron worden als volgt aangegeven:

* Toevoegingen worden gewoon vermeld
* Verwijderingen worden aangegeven met doorhalingstekst
* Wijzigingen worden vermeld in de notitie na de tabel

### AccessRequest

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| Actie¹  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

### AccessRule¹ 

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| coreAction²  |   |   |   |   |   |   |
| forbiddenActions² |   |   |   |   |   |   |
| secundairActions² |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ vlag verwijderd: RAPPORTAGE\
² Wijzigingen in mogelijke waarden

### Goedkeuring

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  | resourcePools |   |   |   |   |
| backlogOrder² | kanbanBoard  |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden\
・Vlaggen toegevoegd: DYNAMIC, LAZY_READ en NOT_GROUPABLE

### Toewijzing

|   |   |   |   | Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnTasks | getAssignAssignmentForTasks  |   |   |   |   |   |
|   |   |   |   | swapUsersOnTasks | getUnassignAssignmentForTasks |   |   |   |   |   |
|   |   |   |   | unassignUserFromTasks |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Klant

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| bizRuleExclusions¹ |   |   |   | getPackagingOptionValue |   |   |
| proofPlan¹ |   |   |   | isPackagingOptionEnabled |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

### Klantvoorkeuren

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| name¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

### DocumentApproval

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

³ Markering toegevoegd: NOT_FILTERABLE

### DocumentVersion

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| activeProofStage |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Groep

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   | eigenaars |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### HourType

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| appGlobalID¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

³ Markering toegevoegd: NOT_FILTERABLE

### Iteratie

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   | moveStories |   |   |

{style=&quot;table-layout:auto&quot;}

### leuk

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Opmerking

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

### OpTask

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   | defaultShownTimesheetIssues  |   |
| backlogOrder | herhaling |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| schatten |   |   |   |   |   |   |
| iterationID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

### Portfolio

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

### Programma

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

### Project

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditTypes¹ |   | resourcePools |   |   | defaultShownTimesheetProjecten |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

### Goedkeuring proef

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| fiatverID | fiatteur |   |   |   |   |   |
| documentVersionID | documentVersion |   |   |   |   |   |
| ID¹ |   |   |   |   |   |   |
| proofCreationDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

³ Markering toegevoegd: NOT_FILTERABLE

### QueueDef

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| aanvragerCoreAction¹ |   |   |   |   |   |   |
| requestorForbiddenActions¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

### Snelheid

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| endDate |   |   |   | setRatesForRole  |   |   |
| name |   |   |   |   |   |   |
| startDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### ReservedTime

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| extRefID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### ResourceManager

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| projectPriority |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Taak

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   | allTasksOnIterations  |   |
| backlogParent | kanbanBoard |   |   |   | defaultShownTimesheetTasks |   |
| kanbanBoardID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

### Team

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| agileMethodology |   |   |   |   |   |   |
| autoAddNextStory |   |   |   |   |   |   |
| includeIssues |   |   |   |   |   |   |
| teamStoryBoardIssueStatuses |   |   |   |   |   |   |
| wipLimit |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Sjabloon

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### TemplateTask

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditTypes¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

Bijwerken

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| updateType¹ | `updateEndorsement` |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

### Gebruiker

|   |   | Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |   |   |
|   |   | usergroups |   |   |   |   |   |   |
|   |   | userRoles |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### UserNote

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |
| `endorsementShareID` | `endorsementShare` |   |   |   |   |   |
| eventType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

### Werk

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| auditTypes¹ | agileWork  |   |   |   |   |   |
| backlogOrder² | kanbanBoard  |   |   |   |   |   |
| backlogParent  |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden\
・Vlaggen toegevoegd: DYNAMIC, LAZY_READ en NOT_GROUPABLE
