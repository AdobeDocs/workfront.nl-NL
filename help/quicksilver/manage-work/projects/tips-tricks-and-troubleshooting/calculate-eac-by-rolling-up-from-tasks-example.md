---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Het Voorbeeld van de berekening - berekent EAC als Roll omhoog van Taken
description: In dit artikel wordt een voorbeeld gegeven van de berekening van de raming bij voltooiing van een project (EAC) als een aanvulling op alle taken van het project in Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 0%

---

# Voorbeeld van berekening - EAC berekenen als een roll-up van taken

## EAC-methode: rollen vanaf taken of subtaken

* [ PIM= op uur-Gebaseerde ](#pim-hour-based)
* [PIM= op basis van kosten](#pim-cost-based)

### PIM= op uurbasis {#pim-hour-based}

* [ Eenvoudig voorbeeld: het project heeft geen kindtaken ](#simple-example-project-has-no-children-tasks)
* [Gecompliceerd voorbeeld: project heeft onderliggende taken](#complicated-example-project-has-children-tasks)

#### Eenvoudig voorbeeld: project heeft geen onderliggende taken {#simple-example-project-has-no-children-tasks}

PIM = op uurbasis

EAC Methode = Rolup van taken/subtaken

1. Creeer Project A met drie taken (geen kindtaken) allen die aan Gebruiker 1 worden toegewezen de waarvan kosten/uur $100.00 is.
1. Voeg geplande/werkelijke uren toe aan elke taak en % Voltooid volgens de onderstaande tabel:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong> Taak </strong> </p> </th> 
   <th> <br> <p><strong> PlnHrs </strong> </p> </th> 
   <th> <br> <p><strong> Akte Hrs </strong> </p> </th> 
   <th> <p><strong>% voltooid </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> <p>5 uur</p> </td> 
   <td> <p>25 uur</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>25 uur</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 3</p> </td> 
   <td> <p>15 uur</p> </td> 
   <td> <p>25 uur</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Herberekening van financiën
1. **CPI voor Taak 1** = .04 berekend als volgt:\
   **CPI voor Taak 1** = *ALS* Ware Uren > 0 *VERVOLGENS* CPI = TotalBudgetedCostWorkPerformance/Ware Uren\
   *ELSE* CPI = 1\
   **CPI voor Taak 1** = 1 / 25\
   **CPI voor Taak 1** = .04

1. **EAC voor Taak 1** = 125 uren berekend als volgt:\
   **EAC voor Taak 1** = *ALS* CPI &lt;> 0 *VERVOLGENS* EAC = Geplande Uren/CPI\
   *ELSE*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **EAC voor Taak 1** = 5 / .04\
   **EAC voor Taak 1** = 125 uren

1. CPI/EAC voor de taken 2 en 3 zijn:\
   Taak 2 = 0,12 / 83,33 uur\
   Taak 3 = 0,24 / 62,5 uur

1. **CPI voor Project** = .13 berekend als volgt:\
   **CPI voor Project** = ** Ware Uren > 0 *VERVOLGENS*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1 
   **CPI voor Project** = 10/75\
   **CPI voor Project** = .13

1. **EAC voor Project** = 270.83 die uren als volgt worden berekend\
   **EAC voor Project** = EAC Taak 1 + EAC Taak 2 + EAC Taak 3\
   **EAC voor Project** = 125 + 83.33 + 62.5\
   **EAC voor Project** = 270.83 uren

#### Gecompliceerd voorbeeld: project heeft onderliggende taken {#complicated-example-project-has-children-tasks}

PIM = op uurbasis

EAC Methode = Rolup van taken/subtaken

1. Creeer Project A met zes taken waar Taak 3 de ouder van Taken 4 en 5 is en Taak 1 de ouder van Taken 2 en 3 zoals hieronder getoond is:\
   Taak 1\
   Taak 2\
   Taak 3\
   Taak 4\
   Taak 5\
   Taak 6

1. Wijs Taken 2, 4, 5, en 6 aan Gebruiker 1 toe het waarvan kosten/uurtarief $100.00 is.
1. Voeg geplande/werkelijke uren toe voor elke taak en % Voltooien volgens de onderstaande tabel.

   >[!NOTE]
   >
   >Voor Taken 1 en 3, voegt u slechts daadwerkelijke uren toe.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong> Taak </strong> </p> </th> 
   <th> <br> <p><strong> PlnHrs </strong> </p> </th> 
   <th> <br> <p><strong> Akte Hrs </strong> </p> </th> 
   <th> <p><strong>% voltooid </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> </td> 
   <td> <p>10 uur</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>5 uur</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 3</p> </td> 
   <td> </td> 
   <td> <p>10 uur</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 4</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 5</p> </td> 
   <td> <p>15 uur</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 6</p> </td> 
   <td> <p>20 uur</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Voeg 50 uur rechtstreeks toe aan het project (More>Hours>Log Hours) zodat er $5.000.00 van daadwerkelijke arbeidskosten die rechtstreeks aan het project worden geregistreerd is.
1. Herberekende financiën uitvoeren
1. **CPI voor Taak 2** = .1 berekend als volgt:\
   **CPI voor Taak 2** = ** Ware Uren > 0 *VERVOLGENS*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1 
   **CPI voor Taak 2** = 1 / 10\
   **CPI voor Taak 2** = .1

1. **EAC voor Taak 2** = 50 uren berekend als volgt:\
   **EAC voor Taak 2** = *ALS* CPI &lt;> 0 *VERVOLGENS*

   ```
   EAC = Planned Hours / CPI
   ```

       *ELSE* EAC = Geplande uren + Werkelijke uren 
   **EAC voor Taak 2** = 5 / .1\
   **EAC voor Taak 2** = 50 uren

1. CPI/EAC voor Taak 4, Taak 5, en Taak 6:\
   Taak 4 = 0,4 / 25 uur\
   Taak 5 = 0,75 / 20 uur\
   Taak 6 = 1,2 / 16,67 uur

1. **CPI voor Taak 3** = .38\
   **CPI voor Taak 3** = ** Ware Uren > 0 *VERVOLGENS*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1 
   **CPI voor Taak 3** = 11.5 / 30\
   **CPI voor Taak 3** = .38

1. **EAC voor Taak 3** = EAC Taak 4 + EAC Taak 5\
   **EAC voor Taak 3** = 25 + 20\
   **EAC voor Taak 3** = 45 uren

1. **CPI voor Taak 1** = .25 berekend als volgt:\
   **CPI voor Taak 1** = ** Ware Uren > 0 *VERVOLGENS*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1 
   **CPI voor Taak 1** = 12.5 / 50\
   **CPI voor Taak 1** = .25

1. **EAC voor Taak 1** = EAC Taak 2 + EAC Taak 3\
   **EAC voor Taak 1** = 50 + 45\
   **EAC voor Taak 1** = 95 uren

1. CPI voor project = 0,22 berekend als volgt:\
   **CPI voor Project** = ** Ware Uren > 0 *VERVOLGENS*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1 
   **CPI voor Project** = 24.5 / 110\
   **CPI voor Project** = .2272\
   **CPI voor Project** = .22

1. **EAC voor project** = EAC Taak 1 + EAC Taak 6\
   **EAC voor project** = 95 + 16.67\
   **EAC voor project** = 111.67 uren

### PIM= op basis van kosten {#pim-cost-based}

* [Eenvoudig voorbeeld: project heeft geen onderliggende taken](#simple-example-project-has-no-children-tasks)

#### Eenvoudig voorbeeld: project heeft geen onderliggende taken {#simple-example-project-has-no-children-tasks-1}

PIM = op kosten gebaseerd

EAC Methode = Rolup van taken/subtaken

1. Creeer Project A met drie taken (geen kindtaken) allen die aan Gebruiker 1 worden toegewezen de waarvan kosten/uur $100.00 is.
1. Voeg geplande/werkelijke uren toe aan elke taak en % Voltooid volgens de onderstaande tabel:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong> Taak </strong> </p> </th> 
   <th> <br> <p><strong> PlnHrs </strong> </p> </th> 
   <th> <br> <p><strong> Pln Lbr Kosten </strong> </p> </th> 
   <th> <br> <p><strong> Akte Hrs </strong> </p> </th> 
   <th> <br> <p><strong> de Kosten van Lbr van de Akte </strong> </p> </th> 
   <th> <p><strong>% voltooid </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> <p>5 uur</p> </td> 
   <td> <p>$ 500,00</p> </td> 
   <td> <p>25 uur</p> </td> 
   <td> <p>$ 2.500,00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> <p>25 uur</p> </td> 
   <td> <p>$ 2.500,00</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 3</p> </td> 
   <td> <p>15 uur</p> </td> 
   <td> <p>$ 1.500,00</p> </td> 
   <td> <p>25 uur</p> </td> 
   <td> <p>$ 2.500,00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Voeg uitgaven aan elke taak toe volgens onderstaande tabel:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong> Taak </strong> </p> </th> 
   <th> <p><strong> Kosten </strong> </p> </th> 
   <th> <p><strong> Gepland Bedrag </strong> </p> </th> 
   <th> <p><strong> Ware Bedrag </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> <p>Taak 1 Exp 1</p> </td> 
   <td> <p>$ 300,00</p> </td> 
   <td> <p>$ 400,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> <p>Taak 1 Exp 2</p> </td> 
   <td> <p>$ 500,00</p> </td> 
   <td> <p>$ 0,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>Taak 2 Exp</p> </td> 
   <td> <p>$ 200,00</p> </td> 
   <td> <p>$ 100,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 3</p> </td> 
   <td> <p>Taak 3 Uitv</p> </td> 
   <td> <p>$ 800,00</p> </td> 
   <td> <p>$ 700,00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Voeg als volgt twee uitgaven toe aan het project (d.w.z. niet aan een taak gebonden):

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong> Kosten </strong> </p> </th> 
   <th> <p><strong> Gepland Bedrag </strong> </p> </th> 
   <th> <p><strong> Ware Bedrag </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Project Exp 1</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> <p>$ 1.500,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 1 Exp 2</p> </td> 
   <td> <p>$ 2.500,00</p> </td> 
   <td> <p>$ 0,00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Op basis van de bovenstaande waarden worden de toegerekende/niet-geïnde kosten als volgt bepaald:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong> Taak </strong> </p> </th> 
   <th> <p><strong> niet Beoogde Geplande Uitgaven </strong> </p> </th> 
   <th> <p><strong> Beoogde Beoogde Uitgaven </strong> </p> </th> 
   <th> <p><strong> curred daadwerkelijke uitgaven </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> <p>$ 500,00</p> </td> 
   <td> <p>$ 300,00</p> </td> 
   <td> <p>$ 400,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>$ 0,00</p> </td> 
   <td> <p>$ 200,00</p> </td> 
   <td> <p>$ 100,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 3</p> </td> 
   <td> <p>$ 0,00</p> </td> 
   <td> <p>$ 800,00</p> </td> 
   <td> <p>$ 700,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>$ 3.000,00</p> </td> 
   <td> <p>$ 2.300,00</p> </td> 
   <td> <p>$ 2.700,00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Voer vanuit Projecthandelingen de herberekening van financiën uit
1. **CPI****for Taak 1** = .14 berekend als volgt:\
   **CPI****for Taak 1** = ** de Ware Kosten van de Arbeid + IncurredActualExpenseCost &lt;> 0 *DAN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor\
     **CPI****for Taak 1** = (100+300) / (2500+400)\
     **CPI****for Taak 1** = 400/2900\
     **CPI****for Taak 1** = .14

1. **EAC****for Taak 1** = $13.400.00\
   **CPI Arbeid****for Taak 1** = ALS de Ware Arbeidskosten &lt;> 0 DAN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **CPI Arbeid****for Taak 1** = 100/2500\
   **CPI Arbeid****for Taak 1** = .04

   **Ecc Arbeid****for Taak 1** = *ALS* CPI_Labor &lt;> 0 *DAN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   * ELSE* EAC Labour = Geplande loonkosten + Werkelijke loonkosten\
     **Ecc Arbeid****voor Taak 1** = 500.00/.04\
     **Ecc Arbeid****voor Taak 1** = $12.500.00

   **uitgaven EAC****voor Taak 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **uitgaven EAC****voor Taak 1** = $400.00 + $500.00\
   **uitgaven EAC****voor Taak 1** = $900.00

   **EAC****for Taak 1** = EC Arbeid + EAC Uitgaven\
   **EAC****for Taak 1** = $12.500.00 + $900.00\
   **EAC****for Taak 1** = $13.400.00

1. Hier zijn de waarden CPI/EAC voor Taak 2 en Taak 3:\
   Taak 2 = .19 / $8.433.33\
   Taak 3 = .44 / $6.950.00***

1. CPI voor het project = .32\
   **CPI****for Project** = ** de Ware Kosten van de Arbeid + IncurredActualExpenseCost &lt;> 0 *DAN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor\
     **CPI****for Project** = (1000 + 2300) / (7500 + 2700)\
     **CPI****for Project** = 3300/10200\
     **CPI****for Project** = .32

1. EAC voor het project is $ 28.783,33\
   **EAC****for Project** = EAC Taak 1 + EAC Taak 2 + EAC Taak 3\
   **EAC****for Project** = $13.400.00 + $8.433.33 + $6.950.00\
   **EAC****for Project** = $28.783.33
