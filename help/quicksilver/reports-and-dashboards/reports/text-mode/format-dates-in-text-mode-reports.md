---
product-area: reporting
navigation-topic: text-mode-reporting
title: Datums opmaken in tekstmodusrapporten
description: Datums kunnen zo worden geconfigureerd dat ze in verschillende indelingen worden weergegeven in rapporten en lijsten in Adobe Workfront. Als u een datumnotatie wilt instellen, moet u de regel met de waarde van de code voor de tekstmodus in de kolom wijzigen.
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Datums opmaken in tekstmodusrapporten

<!-- Audited: 1/2025 -->

Datums kunnen zo worden geconfigureerd dat ze in verschillende indelingen worden weergegeven in rapporten en lijsten in Adobe Workfront. Als u een datumnotatie wilt instellen, moet u de regel `valueformat` van de code in de tekstmodus wijzigen.

`valueformat= [new date format]` Als u bijvoorbeeld wilt dat de Geprojecteerde Voltooiingsdatum wordt weergegeven als MM/DD/YY, ziet de code er als volgt uit:

```
valueformat=atDate
valuefield=projectedCompletionDate
```

Als u de Geplande Datum van de Voltooiing als *Maand, DD, Jaar* wilde tonen, zou de code als kijken:

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

Voor meer informatie over het toepassen van voorwaardelijk formatteren in de rapporten en lijsten van Workfront die tekstwijze gebruiken, zie [&#x200B; Voorwaardelijk het formatteren van het Gebruik in de Wijze van de Tekst &#x200B;](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

U kunt datums opmaken met de volgende waarden in de tekstmodus `valueformat` :

| **Formaat** | Voorbeeld  | ***valueformat=*** |
|---|---|---|
| MM/DD/YY | 11-10-18 | `atDate` |
| MM/DD/YY-tijd | 11-10-18 12:00 | `longAtDate` |
| MM/DD/YY | 11-10-18 | `shortAtDate` |
| Mth, DD, YR | 11 okt. 2018 | `mediumAtDate` |
| DW, Mth, Day, YR | Mon, okt. 11, 2018 | `partialAtDate` |
| DW, Math, Dag, JR Tijd | Ma, okt, 11 oktober 2018 12:00 pm | `fullAtDate` |
