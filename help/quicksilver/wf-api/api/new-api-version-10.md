---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuw in API-versie 10
description: Bijgewerkte bronnen
author: Becky
feature: Workfront API
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Nieuw in API-versie 10

* [Nieuwe bronnen](#new-resources)
* [Bijgewerkte bronnen](#updated-resources)
* [Verwijderde bronnen](#removed-resources)

## Nieuwe bronnen {#new-resources}

### ActivityLog

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | TOEVOEGEN |
|   |   |   |   |   |   | TELLEN |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | ZOEKEN |

{style=&quot;table-layout:auto&quot;}

### CalendarEntry

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | TOEVOEGEN |
|   |   |   |   |   |   | TELLEN  |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | BEWERKEN  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RAPPORT  |
|   |   |   |   |   |   | ZOEKEN |

{style=&quot;table-layout:auto&quot;}

### CalendarEntryExternalReference

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | TELLEN |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RAPPORT  |
|   |   |   |   |   |   | ZOEKEN  |

{style=&quot;table-layout:auto&quot;}

### ExternalAuthToken

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | TOEVOEGEN |
|   |   |   |   |   |   | TELLEN |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | BEWERKEN  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RAPPORT  |
|   |   |   |   |   |   | ZOEKEN  |

{style=&quot;table-layout:auto&quot;}

### LicenseTypeGroupLimit

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| customerID | klant |   |   |   |   |   |
| groupID | groep |   |   |   |   |   |
| planLimit |   |   |   |   |   |   |
| usedLicences |   |   |   |   |   |   |
| werklimiet |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### UserHomeCalendarPreference

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| customerID | klant |   |   |   |   | TOEVOEGEN |
| edTime | user |   |   |   |   | TELLEN |
| firstDayOfWeek |   |   |   |   |   | DELETE |
| ID |   |   |   |   |   | BEWERKEN |
| showPTO |   |   |   |   |   | GET |
| startTime |   |   |   |   |   | RAPPORT |
| userID |   |   |   |   |   | ZOEKEN |
| workDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**Bijgewerkte bronnen**

De volgende bestaande bronnen zijn bijgewerkt met deze versie van de Workfront API. Wijzigingen in een bron worden als volgt aangegeven:

* Toevoegingen worden gewoon vermeld
* Verwijderingen worden aangegeven met doorhalingstekst
* Wijzigingen worden weergegeven in de notitie na de tabel

### Goedkeuring

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval `¹`   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |
| projectBudgetedCost  |   |   |   |   |   |   |
| projectNetValue  |   |   |   |   |   |   |
| projectRoi  |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

`¹ Type changed from null to boolean`

### Toewijzing

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| assignPercent `¹` |   |   |   |   |   |   |
| viewByAssignedToUser |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

`¹`added validator LESS_THAN_EQUAL

### BudgetedHour

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Klantvoorkeuren

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| name `¹` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

### DocMetadataLinkGroup

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style=&quot;table-layout:auto&quot;}

### Document

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### DocumentRequest

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

DocumentVersion

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| externalIntegrationType ¹ |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

Kosten

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Groep

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style=&quot;table-layout:auto&quot;}

### LinkedFolder

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| externalIntegrationType¹ |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹ Wijzigingen in mogelijke waarden

### OpTask

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| priorityColor |  |  | pendingApproval¹ |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹ Type gewijzigd van null in Boolean

### PortalSection

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|  |  |  | groupIDs |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Portfolio

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| portfolioNetValue |  |  |  |  |  |  |
| portfolioRoi |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Project

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| projectBudgetedCost  |   |   |   | linkExternalObject  |   |   |
| projectNetValue |   |   |   | unlinkExternalObject |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Goedkeuring proef

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| fiatteurDecision |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

### Snelheid

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| rateValue ¹ |  |  |  |  |  |  |

{style=&quot;table-layout:auto&quot;}

¹ bijgewerkte VALUTA voor validatie

### Taak

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| kanbanFlag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### Team

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| hoursPerPoint ¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ added validator LESS_THAN

### TeamAssignment

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### TeamTask

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Tijdschema

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### Bijwerken

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| updateType `¹` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style=&quot;table-layout:auto&quot;}

¹ verandert in possibleValues

### Gebruiker

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   | accessLevel  |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### UserNote

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| eventType ¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ verandert in possibleValues

### Werk

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval ¹  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ Type gewijzigd van null in Boolean

## Verwijderde bronnen {#removed-resources}

### ResourceBudgetedHour

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| assignDate |   |   |   |   |   | TOEVOEGEN  |
| budgetedHours |   |   |   |   |   | TELLEN  |
| ID |   |   |   |   |   | DELETE  |
| scheduledBudgetedHours |   |   |   |   |   | BEWERKEN  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | RAPPORT  |
| userID |   |   |   |   |   | ZOEKEN |

{style=&quot;table-layout:auto&quot;}

 

 

 
