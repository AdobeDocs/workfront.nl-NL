---
content-type: api
navigation-topic: api-navigation-topic
title: Updates voor API versie 9
description: Bijgewerkte bronnen
author: Becky
feature: Workfront API
role: Developer
exl-id: 51892846-d93f-4363-8416-4118fb2ef84d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Updates voor API versie 9

## Bijgewerkte bronnen

De volgende bestaande bronnen zijn bijgewerkt met deze versie van de Adobe Workfront API. Om de middelen te bekijken die aan versie 9 nieuw zijn kunt u [ bezoeken wat in API Versie 9 ](../../wf-api/api/new-api-version-9.md) Nieuw is en [ wat in (voortgezette) API Versie 9 Nieuw is ](../../wf-api/api/new-api-version-9-continue.md). Wijzigingen in een bron worden als volgt aangegeven:

* Toevoegingen worden gewoon vermeld
* Verwijderingen worden aangegeven met doorhalingstekst
* Wijzigingen worden vermeld in de notitie na de tabel

### AgileWork

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `opTaskID`<sup> 2 </sup> |  |   |  |   |   |  |
| `taskID`<sup> 2 </sup> |   |   |  |  |  |  |

{style="table-layout:auto"}

<sup> 1 </sup> verwijderde vlag: VERSLAGBARE\
<sup> 2 </sup> verwijderde vlag: NOT_GROUPABLE

### Goedkeuring

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   |   |   |   |

{style="table-layout:auto"}

Toewijzing

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| |   |  |  | `assignUserToRoleOnProjects`<sup> 1 </sup> |   |   |
|   |   |   |   | `assignUserToRoleOnTasks`<sup> 1 </sup> |   |   |
|   |   |   |   | `swapUsersOnProjects`<sup> 1 </sup> |   |   |
|   |   |   |   | `swapUsersOnTasks`<sup> 1 </sup> |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> Toegevoegd gebied: lockToRole

### Klantvoorkeuren

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `name`<sup> 1 </sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> Veranderingen in possibleValues

### Uur

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `days` |   |   |   |   |   |   |
| `workHoursPerDay` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Iteratie

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   | `moveIssues` |   |   |

{style="table-layout:auto"}

### LayoutTemplates

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `groupID` | `group` |   |   |   |   |   |

{style="table-layout:auto"}

### Opmerking

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `html` |   |   |   |   |   |   |
| `json` |   |   |   |   |   |   |
| `richTextNoteID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### OpTask

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `color` | `agileWork` |   |   | `convertToProject` |   |   |
| `isReady` |   |   |   | `convertToTask` |   |   |
| `storyBoardOrder` |   |   |   | `linkExternalObject` |   |   |
|   |   |   |   | `unlinkExternalObject` |   |   |

{style="table-layout:auto"}

### ResourceBudget

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `ID` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup> 1 </sup> verwijderde vlag: VERSLAGBARE

### Schema

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `homeGroupID` | `homeGroup` |   |   |   |   |   |

{style="table-layout:auto"}

### Taak

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   | `agileWork` |   |   | `convertToProject` |   |   |
|   |   |   |   | `linkExternalObject` |   |   |
|   |   |   |   | `unlinkExternalObject` |   |   |

{style="table-layout:auto"}

### Team

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `includeIssues` |   |   |   |   |   |   |

{style="table-layout:auto"}

### TimesheetProfile

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `groupID` | `group` |   |   |   |   |   |

{style="table-layout:auto"}

### UIFilter

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `filtersForObjCode` |   |

{style="table-layout:auto"}

### UIView

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `viewsForObjCode` |   |

{style="table-layout:auto"}

### Gebruiker

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `logTimeInDays` |   |   |   |   |   |   |
| `workHoursPerDay` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Werk

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   | `getWFHomeObjects` |   |   |
