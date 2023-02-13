---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuwe functies in API-versie 9 (vervolg)
description: Deze lijst is de tweede helft van een grotere lijst. De eerste helft kan bij wat in API Versie 9 Nieuw is worden gevestigd. De lijst met updates voor versie 9 vindt u bij Updates voor API versie 9.
author: John
feature: Workfront API
exl-id: 0af97c16-e6a7-4796-92e0-4c2d9751c845
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---

# Nieuwe functies in API-versie 9 (vervolg)

Deze lijst is de tweede helft van een grotere lijst. De eerste helft kan worden gevestigd bij [Nieuw in API-versie 9](../../wf-api/api/new-api-version-9.md). U vindt de lijst met updates voor versie 9 op [Updates voor API versie 9](../../wf-api/api/new-api-version-9-updates.md).

## PortalSection

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `accessorIDs` | `customer` | `accessRules` | `accessLevelMM` | `exportFusionChartToPDF` |  | `ADD` |
| `appGlobalID` | `enteredBy` | `lastViewers` | `displayDescription` | `getPK` |  | `COPY` |
| `controllerClass` | `filter` | `linkedRoles` | `displayName` | `getReportFromCache` |  | `COUNT` |
| `currency` | `groupBy` | `linkedTeams` | `groupIDs` | `isReportFilterable` |  | `DELETE` |
| `customerID` | `lastUpdatedBy` | `linkedUsers` | `linkedCustomersMM` | `linkCustomer` |  | `EDIT` |
| `dashboards` | `publicRunAsUser` | `portalTabSections` | `linkedPortalTabsMM` | `migratePortalSectionsPPMToAnaconda` |  | `GET` |
| `defaultTab` | `reportFolder` | `scheduledReports` | `linkedRoleIDs` | `unlinkCustomer` |  | `REPORT` |
| `definition` | `runAsUser` |  | `linkedTeamIDs` |  |  | `SEARCH` |
| `description` | `scheduledReport` |  | `linkedUsersMM` |   |   |   |
| `descriptionKey` | `statisticInfo` |  | `portalTabsMM`  |   |   |   |
| `enablePromptSecurity` | `view` |  | `scheduledReportsOM`  |   |   |   |
| `enteredByID`  |   |   |   |   |   |   |
| `extRefID`  |   |   |   |   |   |   |
| `filterControl`  |   |   |   |   |   |   |
| `filterID`  |   |   |   |   |   |   |
| `folderName`  |   |   |   |   |   |   |
| `forceLoad`  |   |   |   |   |   |   |
| `ganttOpen`  |   |   |   |   |   |   |
| `globalUIKey`  |   |   |   |   |   |   |
| `groupByID`  |   |   |   |   |   |   |
| `groupControl`  |   |   |   |   |   |   |
| `ID`  |   |   |   |   |   |   |
| `isAppGlobalCopiable`  |   |   |   |   |   |   |
| `isAppGlobalEditable`  |   |   |   |   |   |   |
| `isNewFormat` |   |   |   |   |   |   |
| `isPublic`  |   |   |   |   |   |   |
| `isReport`  |   |   |   |   |   |   |
| `isStandalone`  |   |   |   |   |   |   |
| `lastUpdateDate`  |   |   |   |   |   |   |
| `lastUpdatedByID`  |   |   |   |   |   |   |
| `maxResults`  |   |   |   |   |   |   |
| `methodName`  |   |   |   |   |   |   |
| `modDate`  |   |   |   |   |   |   |
| `name` |   |   |   |   |   |   |
| `nameKey`  |   |   |   |   |   |   |
| `objID`  |   |   |   |   |   |   |
| `objInterface` |   |   |   |   |   |   |
| `objObjCode` |   |   |   |   |   |   |
| `preferenceID` |   |   |   |   |   |   |
| `publicRunAsUserID` |   |   |   |   |   |   |
| `publicToken` |   |   |   |   |   |   |
| `reportFolderID`  |   |   |   |   |   |   |
| `reportType` |   |   |   |   |   |   |
| `runAsUserID`  |   |   |   |   |   |   |
| `scheduledReportID`  |   |   |   |   |   |   |
| `securityAncestorsDisabled`  |   |   |   |   |   |   |
| `securityRootID`  |   |   |   |   |   |   |
| `securityRootObjCode`  |   |   |   |   |   |   |
| `showPrompts`  |   |   |   |   |   |   |
| `sortBy`  |   |   |   |   |   |   |
| `sortBy2` |   |   |   |   |   |   |
| `sortBy3`  |   |   |   |   |   |   |
| `sortType`  |   |   |   |   |   |   |
| `sortType2` |   |   |   |   |   |   |
| `sortType3` |   |   |   |   |   |   |
| `specialView` |   |   |   |   |   |   |
| `toolBar` |   |   |   |   |   |   |
| `uiObjCode`  |   |   |   |   |   |   |
| `viewControl` |   |   |   |   |   |   |
| `viewID` |   |   |   |   |   |   |
| `width` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

## PortalSectionLastViewer

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| creationDate | `customer` |  |  |  |  | `COUNT` |
| `customerID` | `report` |  |  |  |  | `GET` |
| `ID` | `viewer` |  |  |  |  | `REPORT` |
| `reportID` |  |  |  |  |  | `SEARCH` |
| viewerID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

## PortalSectionStatisticInfo

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `allViews` | `customer` |  |  |  |  | `COUNT` |
| `customerID` | `report` |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `lastUpdatedDate` |  |  |  |  |  | `SEARCH` |
| `reportID`  |   |   |   |   |   |   |
| `viewsLastMonth`  |   |   |   |   |   |   |
| `viewsLastQuarter` |   |   |   |   |   |   |
| `viewsLastYear` |   |   |   |   |   |   |
| `viewsThisMonth`  |   |   |   |   |   |   |
| `viewsThisQuarter`  |   |   |   |   |   |   |
| `viewsThisYear`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

## PortalTab

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `accessorIDs` | `customer` | `accessRules` | `linkedRoleIDs` | `advancedCopy` |  | `ADD` |
| `customerID` | `lastUpdatedBy` | `linkedRoles` | `linkedTeamIDs` | `exportDashboard` |  | `COPY` |
| `description` | `user` | `linkedTeams` | `linkedUsersMM` | `migrateCustomTabUserPrefs` |  | `COUNT` |
| `displayOrder` |  | `linkedUsers` |  |  |  | `DELETE` |
| `docID` |  | `portalTabSections` |  |  |  | `EDIT` |
| `extRefID` |  |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `isPublic` |  |  |  |  |  | `SEARCH` |
| `lastUpdateDate`  |   |   |   |   |   |   |
| `lastUpdatedByID`  |   |   |   |   |   |   |
| `name` |   |   |   |   |   |   |
| `nameKey`  |   |   |   |   |   |   |
| `portalProfileID`  |   |   |   |   |   |   |
| `tabname` |   |   |   |   |   |   |
| `userID`  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

## PortalTabSection

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `area` | `calendarPortalSection`  |   |   |   |   |   |
| `calendarPortalSectionID` | `customer`  |   |   |   |   |   |
| `customerID` | `externalSection`  |   |   |   |   |   |
| `displayOrder` | `internalSection`  |   |   |   |   |   |
| `externalSectionID` | `portalTab` |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| `internalSectionID` |   |   |   |   |   |   |
| `portalSectionObjCode`  |   |   |   |   |   |   |
| `portalSectionObjID`  |   |   |   |   |   |   |
| `portalTabID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

## ReportFolder

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| customerID | `customer` |   |   |   |   |   |
| `ID`  |   |   |   |   |   |   |
| name |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

## ScheduleReport

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `customerID` | `customer` | `groups` | `accessLevelMM` | `sendReportDeliveryNow` |  | `ADD` |
| `description` | `enteredBy` | `roles` |  |  |  | `COPY` |
| `enteredByID` | `portalSection` | `teams` |  |  |  | `COUNT` |
| `externalEmails` | `runAsUser` | `users` |  |  |  | `DELETE` |
| `format` |  |  |  |  |  | `EDIT` |
| `groupIDs` |  |  |  |  |  | `GET` |
| `ID` |  |  |  |  |  | `REPORT` |
| `isExcelHyperlinksEnabled` |  |  |  |  |  | `SEARCH` |
| `lastRuntimeMilliseconds` |   |   |   |   |   |   |
| `lastSentDate` |   |   |   |   |   |   |
| `name`  |   |   |   |   |   |   |
| `pageSize`  |   |   |   |   |   |   |
| `portalSectionID`  |   |   |   |   |   |   |
| `recipients`  |   |   |   |   |   |   |
| `recurrenceRule` |   |   |   |   |   |   |
| `roleIDs` |   |   |   |   |   |   |
| `runAsUserID` |   |   |   |   |   |   |
| `runAsUserTypeAhead` |   |   |   |   |   |   |
| `schedTime`  |   |   |   |   |   |   |
| `schedule` |   |   |   |   |   |   |
| `scheduleStart`  |   |   |   |   |   |   |
| `startDate`  |   |   |   |   |   |   |
| `teamIDs` |   |   |   |   |   |   |
| `uiObjCode`  |   |   |   |   |   |   |
| `uiObjID`  |   |   |   |   |   |   |
| `userIDs`  |   |   |   |   |   |   |
