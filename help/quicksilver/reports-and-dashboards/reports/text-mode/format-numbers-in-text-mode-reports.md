---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formaatnummers, valuta- en percentagewaarden in tekstmodusrapporten
description: Numerieke waarden, waaronder valuta, kunnen zo worden geconfigureerd dat ze in verschillende indelingen worden weergegeven in rapporten en lijsten in Adobe Workfront.
author: Courtney
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 2%

---

# Formaatnummers, valuta- en percentagewaarden in tekstmodusrapporten

<!-- Audited: 1/2025 -->

Numerieke waarden, waaronder valuta, kunnen zo worden geconfigureerd dat ze in verschillende indelingen worden weergegeven in rapporten en lijsten in Adobe Workfront.

Om het formaat van een numerieke waarde te wijzigen, moet u de **waardevormings** lijn van uw kolom uitgeven.

Als u bijvoorbeeld de kolom Begroting wilt weergeven als $1000, zou de regel voor de waardeopmaak er als volgt uitzien:

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Voor meer informatie over het toepassen van voorwaardelijk het formatteren in de rapporten en lijsten van Workfront gebruikend tekstwijze, zie [ Voorwaardelijk het formatteren van het Gebruik in de Wijze van de Tekst ](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

U kunt getallen opmaken met de volgende waarden voor de `valueformat` -regel van uw kolom:

| Voorbeeld | `valueformat=` |
|---|---|
| 1234 | `doubleAsString`<br> of <br>`int` |
| 1.234 | `doubleAsInt` |
| $ 1.234 | `currencyStringCurrencyRounded` |
| 1234,56 | `doubleAsDouble` |
| $ 1.234,56 | `currencyStringCurrency` |
| 12% | `doubleAsPercentRounded` |
| 12,34% | `doubleAsPercent` |
| (1 234,56) | `doubleAsFinancial` |
| (1 234) | `doubleAsFinancialRounded` |

