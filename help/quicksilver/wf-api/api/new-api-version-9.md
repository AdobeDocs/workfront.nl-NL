---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuw in API-versie 9
description: Dit is een lijst met bronnen die nieuw zijn voor API versie 9. Ga naar Updates voor API versie 9 voor een lijst met updates die zijn aangebracht in de bronnen van versie 9.
author: Becky
feature: Workfront API
role: Developer
exl-id: 29d922f4-f4c6-45e5-b9fa-43e2068ec66d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '168'
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

{style="table-layout:auto"}

### AccessLevelPermissions

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `coreAction` |  |  |  |  |  |   |
| `forbiddenActions` |  |  |  |  |  |   |
| `ID` |  |  |  |  |  |   |
| `isAdmin` |  |  |  |  |  |   |
| `objObjCode` |  |  |  |  |  |  |
| `secondaryActions` |  |  |  |  |  |  |

{style="table-layout:auto"}

### AccessRulePreference

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `ID` |   |   |   |   |   |   |

{style="table-layout:auto"}

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

{style="table-layout:auto"}

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

{style="table-layout:auto"}

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

{style="table-layout:auto"}

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

{style="table-layout:auto"}

 

Deze lijst is opgesplitst in twee helften. Als u de tweede helft wilt weergeven, raadpleegt u [Nieuwe functies in API-versie 9 (vervolg)](../../wf-api/api/new-api-version-9-continue.md). Als u de lijst met versie 9-updates wilt weergeven, gaat u naar [Updates voor API versie 9](../../wf-api/api/new-api-version-9-updates.md)
