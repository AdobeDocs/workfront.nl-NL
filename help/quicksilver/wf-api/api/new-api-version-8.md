---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuw in API-versie 8
description: Dit is een lijst met bronnen die nieuw zijn voor API-versie 9. Voor een lijst met updates voor de bronnen van versie 8 gaat u naar Updates voor API versie 8
author: Becky
feature: Workfront API
role: Developer
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 1%

---

# Nieuw in API-versie 8

## Nieuwe bronnen

Dit is een lijst met bronnen die nieuw zijn voor API versie 9. Voor een lijst van updates die aan de middelen van versie 8 zijn gemaakt te bezoeken gelieve [&#x200B; Updates aan API Versie 8 &#x200B;](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| backlogOrder | klant |   |   | bulkCopy  |   | KOPIE |
| kleur | herhaling  |   |   |   |   | TELLEN |
| customerID | lastUpdatedBy |   |   |   |   | DELETE |
| schatten | opTask |   |   |   |   | BEWERKEN |
| ID | project |   |   |   |   | GET  |
| isReady | storyboardParent |   |   |   |   | RAPPORT |
| iterationID | taak |   |   |   |   | ZOEKEN |
| lastUpdateDate | team |   |   |   |   |   |
| lastUpdatedByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |
| opTaskID |   |   |   |   |   |   |
| parentStoryBoardOrder |   |   |   |   |   |   |
| projectID |   |   |   |   |   |   |
| storyBoardOrder |   |   |   |   |   |   |
| storyBoardParentID |   |   |   |   |   |   |
| taskID  |   |   |   |   |   |   |
| teamID |   |   |   |   |   |   |
| type |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style="table-layout:auto"}

### APIVersionMetadata

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | TELLEN  |
| removeRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | ZOEKEN |

{style="table-layout:auto"}

**KanbanBoard**

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADD |
| name |   |   |   |   |   | TELLEN |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | BEWERKEN |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | ZOEKEN |

{style="table-layout:auto"}

### ProofApprovalStatus

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style="table-layout:auto"}

**ProofFileMetadata**

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style="table-layout:auto"}

**ResourceBudgetedHour**

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| assignDate |   |   |   |   |   | ADD |
| budgetedHours |   |   |   |   |   | TELLEN |
| scheduledBudgetedHours |   |   |   |   |   | DELETE |
| projectID |   |   |   |   |   | BEWERKEN |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | ZOEKEN |

{style="table-layout:auto"}

### ResourcePlannerFilter

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADD |
| name |   |   |   |   |   | TELLEN |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | BEWERKEN |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | ZOEKEN |

{style="table-layout:auto"}

**RichTextNote**

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | TELLEN |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | ZOEKEN |

{style="table-layout:auto"}

### Abonneren

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | abonnees | ADD |
|   |   |   |   | removeSubscribers |   | TELLEN  |
|   |   |   |   | abonnees |   | DELETE |
|   |   |   |   | afmelden |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | ZOEKEN |

{style="table-layout:auto"}

### UserRole

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| roleID | rol |   |   |   |   |   |
| timePercentage | user |   |   |   |   |   |
| userID |   |   |   |   |   |   |
