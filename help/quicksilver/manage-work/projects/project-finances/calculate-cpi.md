---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Kostenprestatie-index (CPI) berekenen
description: De kostenprestatie-index (CPI) beschrijft de relatie op het project- of taakniveau tussen de geplande kosten en de werkelijke kosten. De Managers van het project herzien dit metrisch om taken of projecten te identificeren die momenteel onder of over kosten op een bepaald punt volgen.
author: Lisa
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: f88b6ec019963ff6256e35b9c94eb4d1b7e99730
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# Kostenprestatie-index (CPI) berekenen

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

De kostenprestatie-index (CPI) beschrijft de relatie op het project- of taakniveau tussen de geplande kosten en de werkelijke kosten. De Managers van het project herzien dit metrisch om taken of projecten te identificeren die momenteel onder of over kosten op een bepaald punt volgen. De kosten kunnen in uren of valuta, afhankelijk van uw Methode van de Index van Prestaties (PIM) worden gemeten. Voor meer informatie over het plaatsen van de Methode van de Index van Prestaties, zie [ de Methode van de Index van Prestaties (PIM) plaatsen ](../../../manage-work/projects/project-finances/set-pim.md).

Slechts kunnen de organisaties die tijdingang vereisen CPI gebruiken. Bovendien zijn op kosten gebaseerde PIM-waarden alleen correct in organisaties die kostenpercentages voor taaktoewijzing hebben gedefinieerd (functies of gebruikers).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td>
   <p>Licht of hoger</p>
   <p>Controleren of hoger</p></td>  
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>Toegang tot projecten en financiële gegevens weergeven</td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td> 
   <td>De mening of hogere toestemmingen aan het project met toestemmingen aan de Financiën van de Mening</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overzicht van de kostenprestatie-index (CPI)

### De CPI-waarde {#the-cpi-value}

Projectbeheerders begrijpen dat een CPI-waarde van 1 betekent dat het project precies op de begroting staat. Waarden groter dan 1 geven aan dat een project onder de begroting valt (er zijn minder uren of kosten geregistreerd dan oorspronkelijk gepland) en waarden kleiner dan 1 betekenen dat een project langer is dan de begroting (er zijn meer uren of kosten geregistreerd dan oorspronkelijk gepland). Hoe verder van 1, hoe verder van het plan wordt afgeweken.

| **CPI Waarde** | **Indicatie op Begroting** |
|---|---|
| 1 | Op plan of begroting |
| > 1 (groter dan 1) | Onder de begroting |
| &lt; 1 (kleiner dan 1) | Boven de begroting |


### Hoe CPI wordt berekend {#how-cpi-is-calculated}

In Adobe Workfront, hangt de berekening voor CPI van de Methode van de Index van Prestaties af die voor het project wordt geselecteerd. Voor meer informatie over het plaatsen van de Methode van de Index van Prestaties, zie [ de Methode van de Index van Prestaties (PIM) plaatsen ](../../../manage-work/projects/project-finances/set-pim.md).

* [ CPI berekeningen wanneer het gebruiken van Op uren-Gebaseerde PIM ](#cpi-calculations-when-using-hour-based-pim)
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

* **voor een niet oudertaak:**

  ```
  Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
  ```

* **voor een oudertaak:**
Totaal uitgevoerd begrotingskostenwerk = de som van het veld Totaal begrote kosten uitgevoerd voor alle directe onderliggende taken.

* **voor een project:**
Totaal uitgevoerd begroot kostenwerk = de som van het totaal uitgevoerd budget-kostenwerkveld voor alle taken op topniveau (ouders en zelfstandige taken).

Voor informatie over het totale Gedragsde Uitgevoerde Werk van Kosten (BCWP), zie [ Gemaakt het Geplande Gepresteerde Werk van Kosten (BCWP) ](../../../manage-work/projects/project-finances/calculate-bcwp.md) berekenen.

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

* **voor een niet oudertaak:**

  ```
  Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
  ```

* **voor een oudertaak:**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field from all direct child tasks)
  ```

* **voor een project:**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field for all top-level tasks)
  ```



## Zoek CPI in een project of een taak

U kunt CPI van een project of een taak in een project of een taaklijst of rapport tonen. Bovendien kunt u het op het project of taakniveau bekijken.

1. Ga naar het project of de taak waar u CPI wilt bekijken.
1. Breid {de Details van het 0} Project **of** Details van de Taak **in het linkerpaneel uit, afhankelijk van of u CPI voor een project of een taak bekijkt.**

1. Klik **Financiën**. De vertoningen CPI op het **CPI/SPI/CSI** gebied.

   ![ CPI op project ](assets/cpi-on-project-nwe.png)
