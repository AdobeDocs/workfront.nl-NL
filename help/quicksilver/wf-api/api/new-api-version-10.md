---
content-type: api
navigation-topic: api-navigation-topic
title: Nieuw in API-versie 10
description: Bijgewerkte bronnen
author: Becky
feature: Workfront API
role: Developer
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '472'
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
|   |   |   |   |   |   | ADD |
|   |   |   |   |   |   | TELLEN |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | ZOEKEN |

{style="table-layout:auto"}

### CalendarEntry

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADD |
|   |   |   |   |   |   | TELLEN  |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | BEWERKEN  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RAPPORT  |
|   |   |   |   |   |   | ZOEKEN |

{style="table-layout:auto"}

### CalendarEntryExternalReference

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | TELLEN |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RAPPORT  |
|   |   |   |   |   |   | ZOEKEN  |

{style="table-layout:auto"}

### ExternalAuthToken

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADD |
|   |   |   |   |   |   | TELLEN |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | BEWERKEN  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | RAPPORT  |
|   |   |   |   |   |   | ZOEKEN  |

{style="table-layout:auto"}

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

{style="table-layout:auto"}

### UserHomeCalendarPreferences

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| customerID | klant |   |   |   |   | ADD |
| edTime | user |   |   |   |   | TELLEN |
| firstDayOfWeek |   |   |   |   |   | DELETE |
| ID |   |   |   |   |   | BEWERKEN |
| showPTO |   |   |   |   |   | GET |
| startTime |   |   |   |   |   | RAPPORT |
| userID |   |   |   |   |   | ZOEKEN |
| workDate |   |   |   |   |   |   |

{style="table-layout:auto"}

**Bijgewerkte bronnen**

De volgende bestaande bronnen zijn bijgewerkt met deze versie van de Workfront API. Wijzigingen in een bron worden als volgt aangegeven:

* Toevoegingen worden gewoon vermeld
* Verwijderingen worden aangegeven met doorhalingstekst
* Wijzigingen worden weergegeven in de notitie na de tabel

### Goedkeuring

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval `<sup>1</sup>`   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |
| projectBudgetedCost  |   |   |   |   |   |   |
| projectNetValue  |   |   |   |   |   |   |
| projectRoi  |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost  |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup> Type changed from null to boolean`

### Toewijzing

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| toewijzingspercentage `<sup>1</sup>` |   |   |   |   |   |   |
| viewByAssignedToUser |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup>`added validator LESS_THAN_EQUAL

### BudgetedHour

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Klantvoorkeuren

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| name `<sup>1</sup>` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Wijzigingen in mogelijke waarden

### DocMetadataLinkGroup

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style="table-layout:auto"}

### Document

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |   |   |   |   |   |

{style="table-layout:auto"}

### DocumentRequest

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

DocumentVersion

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| externalIntegrationType <sup>1</sup> |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Wijzigingen in mogelijke waarden

Kosten

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Groep

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style="table-layout:auto"}

### LinkedFolder

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| externalIntegrationType<sup>1</sup> |  |  |  |  |   |   |

{style="table-layout:auto"}

<sup>1</sup> Wijzigingen in mogelijke waarden

### OpTask

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| priorityColor |   |  | pendingApproval<sup>1</sup> |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Type gewijzigd van null in Boolean

### PortalSection

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |  |   | groupIDs |   |   |   |

{style="table-layout:auto"}

### Portfolio

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| portfolioNetValue |   |   |   |  |  |   |
| portfolioRoi |   |   |   |   |   |   |

{style="table-layout:auto"}

### Project

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| projectBudgetedCost  |   |   |   | linkExternalObject  |   |   |
| projectNetValue |   |   |   | unlinkExternalObject |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost |   |   |   |   |   |   |

{style="table-layout:auto"}

### Goedkeuring proef

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| fiatteurDecision |   |   |   |   |   |   |

{style="table-layout:auto"}

### Snelheid

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| rateValue <sup>1</sup> |  |  |  |  |  |   |

{style="table-layout:auto"}

<sup>1</sup>added validator CURRENCY

### Taak

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| kanbanFlag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### Team

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| hoursPerPoint <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> added validator LESS_THAN

### TeamAssignment

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### TeamTask

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Tijdschema

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### Bijwerken

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| updateType `<sup>1</sup>` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style="table-layout:auto"}

<sup>1</sup> wijzigingen in possibleValues

### Gebruiker

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
|   | accessLevel  |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| eventType <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> wijzigingen in possibleValues

### Werk

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval <sup>1</sup>  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Type gewijzigd van null in Boolean

## Verwijderde bronnen {#removed-resources}

### ResourceBudgetedHour

| Velden | Verwijzingen | Verzamelingen | Zoeken | Handelingen | Zoekopdrachten | Bewerkingen |
|---|---|---|---|---|---|---|
| assignDate |   |   |   |   |   | ADD  |
| budgetedHours |   |   |   |   |   | TELLEN  |
| ID |   |   |   |   |   | DELETE  |
| scheduledBudgetedHours |   |   |   |   |   | BEWERKEN  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | RAPPORT  |
| userID |   |   |   |   |   | ZOEKEN |

{style="table-layout:auto"}

 

 

 
