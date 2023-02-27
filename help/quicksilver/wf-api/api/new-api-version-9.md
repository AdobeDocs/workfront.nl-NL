---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuw in API-versie 9
description: Dit is een lijst met bronnen die nieuw zijn voor API versie 9. Ga naar Updates voor API versie 9 voor een lijst met updates die zijn aangebracht in de bronnen van versie 9.
author: Becky
feature: Workfront API
exl-id: 29d922f4-f4c6-45e5-b9fa-43e2068ec66d
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 0%

---

# Nieuw in API-versie 9

## Nieuwe bronnen

Dit is een lijst met bronnen die nieuw zijn voor API-versie 9. Ga naar [Updates voor API versie 9](../../wf-api/api/new-api-version-9-updates.md)

### AccessLevel

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `accessRestrictions` | `customer` | `accessLevelPermissions` |  |  |  | `ADD` |
| `customerID` | `lastUpdatedBy` | `accessRulePreferences` |  |  |  | `COPY` |
| `description` |  |  |  |  |  | `COUNT` |
| `descriptionKey` |  |  |  |  |  | `DELETE` |
| `entryDate` |  |  |  |  |  | `EDIT` |
| `extRefID` |  |  |  |  |  | `GET` |
| `fieldAccessPrivileges` |  |  |  |  |  | `REPLACE` |
| `ID` |  |  |  |  |  | `REPORT` |
| `isAdmin` |  |  |  |  |  | `SEARCH` |
| `isUnsupportedWorkerLicense` |  |  |  |  |  |   |
| `lastUpdatedByID` |  |  |  |  |  |   |
| `lastUpdatedDate` |  |  |  |  |  |  |
| `licenseType` |  |  |  |  |  |  |
| `name` |  |  |  |  |  |  |
| `nameKey` |  |  |  |  |  |  |
| `securityModelType` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### AccessLevelPermissions

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `coreAction` |  |  |  |  |  |   |
| `forbiddenActions` |  |  |  |  |  |   |
| `ID` |  |  |  |  |  |   |
| `isAdmin` |  |  |  |  |  |   |
| `objObjCode` |  |  |  |  |  |  |
| `secondaryActions` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### AccessRulePreference

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `ID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### BudgetedHour

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `allocationDate` |  |  |  |  |  | `ADD` |
| `budgetedHours` |  |  |  |  |  | `DELETE` |
| `GUID` |  |  |  |  |  | `GET` |
| `plannedBudgetedHours` |  |  |  |  |  | `SEARCH` |
| `projectID` |   |   |   |   |   |   |
| `roleID`  |   |   |   |   |   |   |
| `userID`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### CalendarPortalSection

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `calendarInfoID` | `customer` |  | `displayDescription` |  |  | `ADD` |
| `customerID` | `enteredBy` |  | `displayName` |  |  | `COPY` |
| `enteredByID` |  |  |  |  |  | `COUNT` |
| `entryDate` |  |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `name` |  |  |  |  |  | `SEARCH` |
| `objID`  |   |   |   |   |   |   |
| `objObjCode`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### CalendarSection

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `calendarID` | `customer` | `filters` |  | `getConcatenatedExpressionForm` |  | `ADD` |
| `calEvents` |  |  |  | `getPrettyExpressionForm` |  | `COUNT` |
| `color` |  |  |  |  |  | `DELETE` |
| `customerID` |  |  |  |  |  | `EDIT` |
| `duration` |  |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `milestone` |  |  |  |  |  | `SEARCH` |
| `name`  |   |   |   |   |   |   |
| `plannedDate` |   |   |   |   |   |   |
| `startDate` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### ExternalSection

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `appGlobalID` | `customer` |  | `displayDescription` | `calculateURL` |  | `ADD` |
| `calculatedURL` | `enteredBy` |  | `displayName` | `calculateURLS` |  | `COPY` |
| `customerID` | `view` |  | `linkedCustomersMM` |  |  | `COUNT` |
| `description` |  |  | `linkedUsersMM` |  |  | `DELETE` |
| `descriptionKey` |  |  |  |  |  | `EDIT` |
| `enteredByID` |  |  |  |  |  | `GET` |
| `entryDate` |  |  |  |  |  | `REPORT` |
| `extRefID` |  |  |  |  |  | `SEARCH` |
| `frame`  |   |   |   |   |   |   |
| `friendlyURL`  |   |   |   |   |   |   |
| `globalUIKey`  |   |   |   |   |   |   |
| `height`  |   |   |   |   |   |   |
| `ID`  |   |   |   |   |   |   |
| `name`  |   |   |   |   |   |   |
| `nameKey`  |   |   |   |   |   |   |
| `objID`  |   |   |   |   |   |   |
| `objInterface`  |   |   |   |   |   |   |
| `objObjCode`  |   |   |   |   |   |   |
| `scrolling` |   |   |   |   |   |   |
| `url` |   |   |   |   |   |   |
| `viewID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

Deze lijst is opgesplitst in twee helften. Als u de tweede helft wilt weergeven, raadpleegt u [Nieuwe functies in API-versie 9 (vervolg)](../../wf-api/api/new-api-version-9-continue.md). Als u de lijst met versie 9-updates wilt weergeven, gaat u naar [Updates voor API versie 9](../../wf-api/api/new-api-version-9-updates.md)
