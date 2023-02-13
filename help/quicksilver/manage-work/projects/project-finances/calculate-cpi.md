---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Kostenprestatie-index (CPI) berekenen
description: De kostenprestatie-index (CPI) beschrijft de relatie op het project- of taakniveau tussen de geplande kosten en de werkelijke kosten. De Managers van het project herzien dit metrisch om taken of projecten te identificeren die momenteel onder of over kosten op een bepaald punt volgen.
author: Alina
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# Kostenprestatie-index (CPI) berekenen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

De kostenprestatie-index (CPI) beschrijft de relatie op het project- of taakniveau tussen de geplande kosten en de werkelijke kosten. De Managers van het project herzien dit metrisch om taken of projecten te identificeren die momenteel onder of over kosten op een bepaald punt volgen. De kosten kunnen in uren of dollars, afhankelijk van uw Methode van de Index van Prestaties (PIM) worden gemeten. Voor meer informatie over het plaatsen van de Methode van de Index van Prestaties, zie [De PIM-methode (Performance Index) instellen](../../../manage-work/projects/project-finances/set-pim.md).

Slechts kunnen de organisaties die tijdingang vereisen CPI gebruiken. Bovendien zijn op kosten gebaseerde PIM-waarden alleen correct in organisaties die kostenpercentages voor taaktoewijzing hebben gedefinieerd (functies of gebruikers).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Controleren of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten en financiële gegevens weergeven</p> <p> Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De mening of hogere toestemmingen aan het project met toestemmingen aan de Financiën van de Mening</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Overzicht van de kostenprestatie-index (CPI)

* [De CPI-waarde](#the-cpi-value)
* [Hoe CPI wordt berekend](#how-cpi-is-calculated)

### De CPI-waarde {#the-cpi-value}

Projectbeheerders begrijpen dat een CPI-waarde van 1 betekent dat het project precies op de begroting staat. Waarden groter dan 1 geven aan dat een project onder de begroting valt (er zijn minder uren of kosten geregistreerd dan oorspronkelijk gepland) en waarden kleiner dan 1 betekenen dat een project langer is dan de begroting (er zijn meer uren of kosten geregistreerd dan oorspronkelijk gepland). Hoe verder van 1, hoe verder van het plan wordt afgeweken.

| **CPI-waarde** | **Opgave van de begroting** |
|---|---|
| 1 | Op plan of begroting |
| > 1 (groter dan 1) | Onder de begroting |
| &lt; 1 (kleiner dan 1) | Boven de begroting |


### Hoe CPI wordt berekend {#how-cpi-is-calculated}

In Adobe Workfront, hangt de berekening voor CPI van de Methode van de Index van Prestaties af die voor het project wordt geselecteerd. Voor meer informatie over het plaatsen van de Methode van de Index van Prestaties, zie [De PIM-methode (Performance Index) instellen](../../../manage-work/projects/project-finances/set-pim.md).

* [CPI berekeningen wanneer het gebruiken van op uren-gebaseerde PIM](#cpi-calculations-when-using-hour-based-pim)
* [CPI Berekeningen wanneer het gebruiken van Op kosten-gebaseerde PIM](#cpi-calculations-when-using-cost-based-pim)

#### CPI berekeningen wanneer het gebruiken van op uren-gebaseerde PIM {#cpi-calculations-when-using-hour-based-pim}

Indien

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

Anders

```
CPI = 1
```

* **Voor een niet-bovenliggende taak:**

   ```
   Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
   ```

* **Voor een bovenliggende taak:**
Totaal uitgevoerd begrotingskostenwerk = de som van het veld Totaal begrote kosten uitgevoerd voor alle directe onderliggende taken.

* **Voor een project:**
Totaal uitgevoerd begroot kostenwerk = de som van het totaal uitgevoerd budget-kostenwerkveld voor alle taken op het hoogste niveau (ouders en zelfstandige taken).

Voor informatie over het totale Gedetailleerde Geoefende Werk van Kosten (BCWP), zie [Geraamd het Geregistreerde Uitgevoerde Werk van Kosten berekenen (BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

#### CPI Berekeningen wanneer het gebruiken van Op kosten-gebaseerde PIM {#cpi-calculations-when-using-cost-based-pim}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>CPI = (Planned Cost of Work Performed + Planned Cost of Incurred Expenses) / (Total Actual Cost + Actual Cost of Incurred Expenses) </code> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>NOTE: this used to be here before - above - but Anna sent me the one below. I kept the other one, although she is still researching its validity - see this issue: https://hub.workfront.com/issue/5fc7b1cf00012aeebf9e822db8ea2513/overview)</code> </p>
-->

Indien

```
Actual Labor Cost + Incurred Actual Expense Cost <> 0 THEN CPI = (Total Budgeted Cost Work Performed + Incurred Planned Expense Cost) / (Actual Labor Cost + Incurred Actual Expense Cost)
```



Anders

```
CPI = 1
```

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>(NOTE: above: this used to say: CPI = CPI Labor, but Anna had me fix it on July 21, 2021)</code> </p>
-->

De velden in deze berekening worden hieronder beschreven:

```
Total Actual Cost = Actual (logged) Hours * Hourly Rate of assignees
```

```
Incurred Actual Expense Cost = Actual Cost
```

Inbegrepen kosten is de kosten waarop de werkelijke kosten > 0

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* De geplande kosten van het uitgevoerde werk worden berekend aan de hand van de volgende formule:

   ```
   Planned Cost of Work Performed = Planned cost * Percent Complete / 100
   ```

De totale begrote uitgevoerde kosten worden berekend voor het volgende:

* **Voor een niet-bovenliggende taak:**

   ```
   Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
   ```

* **Voor een bovenliggende taak:**

   ```
   Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field from all direct child tasks)
   ```

* **Voor een project:**

   ```
   Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field for all top level tasks)
   ```



## Bepaal de plaats van CPI in een project of een taak

U kunt CPI van een project of een taak in een project of een taaklijst of rapport tonen. Bovendien kunt u het op het project of taakniveau bekijken.

1. Ga naar het project of de taak waar u CPI wilt bekijken.
1. Uitbreiden **Projectdetails** of **Taakdetails** in het linkerpaneel, afhankelijk van of u CPI voor een project of een taak bekijkt.

1. Klikken **Financiën**.

   De vertoningen CPI in **CPI/SPI/CSI** veld.

   ![](assets/cpi-on-project-nwe.png)
