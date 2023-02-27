---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuw in API-versie 8
description: Dit is een lijst met bronnen die nieuw zijn voor API-versie 9. Voor een lijst met updates voor de bronnen van versie 8 gaat u naar Updates voor API versie 8
author: Becky
feature: Workfront API
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---

# Nieuw in API-versie 8

## Nieuwe bronnen

Dit is een lijst met bronnen die nieuw zijn voor API-versie 9. Voor een lijst met updates van de bronnen van versie 8 gaat u naar [Updates voor API versie 8](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| backlogOrder | klant |   |   | bulkCopy  |   | KOPIËREN |
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

{style=&quot;table-layout:auto&quot;}

### APIVersionMetadata

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | TELLEN  |
| removeRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | ZOEKEN |

{style=&quot;table-layout:auto&quot;}

**KanbanBoard**

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | TOEVOEGEN |
| name |   |   |   |   |   | TELLEN |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | BEWERKEN |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | ZOEKEN |

{style=&quot;table-layout:auto&quot;}

### ProofApprovalStatus

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ProofFileMetadata**

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ResourceBudgetedHour**

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| assignDate |   |   |   |   |   | TOEVOEGEN |
| budgetedHours |   |   |   |   |   | TELLEN |
| scheduledBudgetedHours |   |   |   |   |   | DELETE |
| projectID |   |   |   |   |   | BEWERKEN |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | ZOEKEN |

{style=&quot;table-layout:auto&quot;}

### ResourcePlannerFilter

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | TOEVOEGEN |
| name |   |   |   |   |   | TELLEN |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | BEWERKEN |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | ZOEKEN |

{style=&quot;table-layout:auto&quot;}

**RichTextNote**

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | TELLEN |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | ZOEKEN |

{style=&quot;table-layout:auto&quot;}

### Abonneren

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | abonnees | TOEVOEGEN |
|   |   |   |   | removeSubscribers |   | TELLEN  |
|   |   |   |   | abonnees |   | DELETE |
|   |   |   |   | afmelden |   | GET |
|   |   |   |   |   |   | RAPPORT |
|   |   |   |   |   |   | ZOEKEN |

{style=&quot;table-layout:auto&quot;}

### UserRole

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| roleID | rol |   |   |   |   |   |
| timePercentage | user |   |   |   |   |   |
| userID |   |   |   |   |   |   |
