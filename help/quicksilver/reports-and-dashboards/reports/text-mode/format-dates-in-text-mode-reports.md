---
product-area: reporting
navigation-topic: text-mode-reporting
title: Datums opmaken in tekstmodusrapporten
description: Datums kunnen zo worden geconfigureerd dat ze in verschillende indelingen worden weergegeven in rapporten en lijsten in Adobe Workfront. Als u een datumnotatie wilt instellen, moet u de regel met de waarde van de code voor de tekstmodus in de kolom wijzigen.
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 1%

---

# Datums opmaken in tekstmodusrapporten

Datums kunnen zo worden geconfigureerd dat ze in verschillende indelingen worden weergegeven in rapporten en lijsten in Adobe Workfront. Als u een datumnotatie wilt instellen, moet u de opdracht `valueformat` regel van de code van de tekstmodus in de kolom.

`valueformat= [new date format]` Als u bijvoorbeeld de Geprojecteerde Voltooiingsdatum wilt weergeven als MM/DD/YY, ziet de code er als volgt uit:

```
valueformat=atDate
valuefield=projectedCompletionDate
```

Als u de Geplande Datum van Voltooiing wilt tonen zoals *Math, DD, Year* De code ziet er als volgt uit:

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

Ga voor meer informatie over het toepassen van voorwaardelijke opmaak in Workfront-rapporten en -lijsten in de tekstmodus naar [Voorwaardelijke opmaak gebruiken in tekstmodus](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

U kunt datums als volgt opmaken

```
valueformat
```

 waarden voor de tekstmodus:

| **Indeling** | Voorbeeld  | ***valueformat=*** |
|---|---|---|
| MM/DD/YY | 10/11/18 | `atDate` |
| MM/DD/YY-tijd | 11-10-18 12:00 | `longAtDate` |
| MM/DD/YY | 10/11/18 | `shortAtDate` |
| Mth, DD, YR | 11 okt. 2018 | `mediumAtDate` |
| DW, Mth, Day, YR | Mon, okt. 11, 2018 | `partialAtDate` |
| DW, Math, Dag, JR Tijd | Ma, okt, 11 oktober 2018 12:00 pm | `fullAtDate` |
