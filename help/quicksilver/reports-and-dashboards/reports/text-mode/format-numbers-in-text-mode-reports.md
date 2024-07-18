---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formaatnummers, valuta- en percentagewaarden in tekstmodusrapporten
description: Numerieke waarden, waaronder valuta, kunnen zo worden geconfigureerd dat ze in verschillende indelingen worden weergegeven in rapporten en lijsten in Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 8de9c79f6c62b74a652482ec10bf38fada8c5fc8
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 1%

---

# Formaatnummers, valuta- en percentagewaarden in tekstmodusrapporten

<!-- Audited: 2/2024 -->

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
| 1234 | <pre>doubleAsString</pre> <br> of <br><pre>int</pre> |
| 1.234 | <pre>doubleAsInt</pre> |
| $ 1.234 | <pre>currencyStringCurrencyRounded</pre> |
| 1234,56 | <pre>doubleAsDouble</pre> |
| $ 1.234,56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounded</pre> |
| 12,34% | <pre>doubleAsPercent</pre> |
| (1 234,56) | <pre>doubleAsFinancial</pre> |
| (1 234) | <pre>doubleAsFinancialRounded</pre> |

