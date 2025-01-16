---
product-area: reporting
navigation-topic: text-mode-reporting
title: Getallen, valuta en percentagewaarden in tekstmodusrapporten opmaken
description: Numerieke waarden, waaronder valuta, kunnen zo worden geconfigureerd dat ze in verschillende indelingen worden weergegeven in rapporten en lijsten in Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 2%

---

# Getallen, valuta en percentagewaarden in tekstmodusrapporten opmaken

<!-- Audited: 1/2025 -->

Numerieke waarden, waaronder valuta, kunnen zo worden geconfigureerd dat ze in verschillende indelingen worden weergegeven in rapporten en lijsten in Adobe Workfront.

Om het formaat van een numerieke waarde te wijzigen, moet u de **waardevormings** lijn van uw kolom uitgeven.

Bijvoorbeeld, als u de kolom van de Begroting als $1000 wilde tonen, zou de lijn van het waardeformaat als kijken:

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Voor meer informatie over het toepassen van voorwaardelijk formatteren in de rapporten en lijsten van Workfront die tekstwijze gebruiken, zie [ Voorwaardelijk het formatteren van het Gebruik in de Wijze van de Tekst ](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

U kunt getallen opmaken met de volgende waarden voor de regel `valueformat` in de kolom:

| Voorbeeld | `valueformat=` |
|---|---|
| 1234 | `doubleAsString`<br> of <br>`int` |
| 1.234 | `doubleAsInt` |
| USD 1.234 | `currencyStringCurrencyRounded` |
| 1234,56 | `doubleAsDouble` |
| $ 1.234,56 | `currencyStringCurrency` |
| 12% | `doubleAsPercentRounded` |
| 12,34% | `doubleAsPercent` |
| (1 234,56) | `doubleAsFinancial` |
| (1,234) | `doubleAsFinancialRounded` |

