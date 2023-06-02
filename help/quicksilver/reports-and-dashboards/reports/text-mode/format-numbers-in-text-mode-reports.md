---
product-area: reporting
navigation-topic: text-mode-reporting
title: Getallen, valuta en percentagewaarden in tekstmodusrapporten opmaken
description: Numerieke waarden, waaronder valuta, kunnen zo worden geconfigureerd dat ze in verschillende indelingen worden weergegeven in rapporten en lijsten in Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: e1411ce49d8668ba50bcb9b80d4a4b47d0dd00fc
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 5%

---

# Getallen, valuta en percentagewaarden in tekstmodusrapporten opmaken

Numerieke waarden, waaronder valuta, kunnen zo worden geconfigureerd dat ze in verschillende indelingen worden weergegeven in rapporten en lijsten in Adobe Workfront.

Als u de notatie van een numerieke waarde wilt wijzigen, moet u de opdracht **taxeformat** lijn van uw kolom.

Bijvoorbeeld, als u de kolom van de Begroting als $1000 wilde tonen, zou de lijn van het waardeformaat als kijken:

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Ga voor meer informatie over het toepassen van voorwaardelijke opmaak in Workfront-rapporten en -lijsten in de tekstmodus naar [Voorwaardelijke opmaak gebruiken in tekstmodus](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

U kunt getallen opmaken met de volgende waarden voor de `valueformat` Regel van de kolom:

| Voorbeeld | `valueformat=` |
|---|---|
| 1234 | <pre>doubleAsString</pre> <br>of <br><pre>int</pre> |
| 1,234 | <pre>doubleAsInt</pre> |
| $1,234 | <pre>currencyStringCurrencyRounded</pre> |
| 1234.56 | <pre>doubleAsDouble</pre> |
| $1,234.56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounded</pre> |
| 12.34% | <pre>doubleAsPercent</pre> |
| (1,234.56) | <pre>doubleAsFinancial</pre> |
| (1,234) | <pre>doubleAsFinancialRounded</pre> |

