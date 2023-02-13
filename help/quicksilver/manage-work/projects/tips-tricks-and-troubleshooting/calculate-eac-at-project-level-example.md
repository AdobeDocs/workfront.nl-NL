---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Berekeningsvoorbeeld - berekening EAC op projectniveau
description: PIM = op uurbasis
author: Alina
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1768'
ht-degree: 6%

---

# Berekeningsvoorbeeld - berekening EAC op projectniveau

## EAC-methode: Berekenen op projectniveau

* [PIM = op uurbasis](#pim-hour-based)
* [PIM= op basis van kosten](#pim-cost-based)

### PIM = op uurbasis {#pim-hour-based}

* [Eenvoudig voorbeeld: project bevat geen onderliggende taken](#simple-example-project-has-no-children-tasks)
* [Gecompliceerd voorbeeld: project bevat onderliggende taken](#complicated-example-project-has-children-tasks)

#### Eenvoudig voorbeeld: project bevat geen onderliggende taken {#simple-example-project-has-no-children-tasks}

PIM = op uurbasis

EAC-methode = Berekenen op projectniveau ***

1. Creeer Project A met drie taken (geen kindtaken) allen die aan Gebruiker 1 worden toegewezen de waarvan kosten/uur $100.00 is.
1. Voeg geplande en werkelijke uren toe aan elke taak en % voltooid volgens de onderstaande tabel:

   <table style="table-layout:auto">
    <col>
    <col>
    <col>
    <col>
    <thead>
     <tr>
      <th><br><p><strong>Taak</strong></p></th>
      <th><br><p><strong>Pln uur</strong></p></th>
      <th><br><p><strong>Act Hrs</strong></p></th>
      <th><p><strong>% voltooid</strong></p></th>
     </tr>
    </thead>
    <tbody>
     <tr>
      <td><p>Taak 1</p></td>
      <td><p>5 uur</p></td>
      <td><p>25 uur</p></td>
      <td><p>20%</p></td>
     </tr>
     <tr>
      <td><p>Taak 2</p></td>
      <td><p>10 uur</p></td>
      <td><p>25 uur</p></td>
      <td><p>30%</p></td>
     </tr>
     <tr>
      <td><p>Taak 3</p></td>
      <td><p>15 uur</p></td>
      <td><p>25 uur</p></td>
      <td><p>40%</p></td>
     </tr>
    </tbody>
   </table>

1. De financiering van het project opnieuw berekenen.
1. **CPI voor Taak 1** = .04, berekend als volgt:\
   **CPI voor Taak 1** = *IF* Werkelijke uren > 0 *DAN* CPI = TotalBudgetedCostWorkPerformance/Actual Hours\
      *ELSE* CPI = 1\
   **CPI voor Taak 1** = 1 / 25\
   **CPI voor Taak 1** = 0,04

1. **EAC voor Taak 1** = 125 uur, berekend als volgt:\
   **EAC voor Taak 1** = *IF* CPI &lt;> 0 *DAN* EAC = geplande uren/CPI\
       *ELSE* EAC = geplande uren + werkelijke uren\
   **EAC voor Taak 1** = 5 / 0,04\
   **EAC voor Taak 1** = 125 uur***

1. CPI/EAC voor de taken 2 en 3 zijn:\
   Taak 2 = 0,12 / 83,33 uur\
   Taak 3 = 0,24 / 62,5 uur

1. **CPI voor Project** = .13 berekend als volgt:\
   **CPI voor Project** = *IF* Werkelijke uren > 0 *DAN* CPI = TotalBudgetedCostWorkPerformance/Actual Hours\
       *ELSE* CPI = 1\
   **CPI voor Project** = 10 / 75\
   **CPI voor Project** = 0,13

1. **EAC voor project** = 225 uur, berekend als volgt:\
   **EAC voor project** = *IF* CPI &lt;> 0 *DAN* EAC = geplande uren/CPI\
       *ELSE* EAC = geplande uren + werkelijke uren\
   **EAC voor project** = 30 / 0,1333\
   **EAC voor project** = 225 uur

#### Gecompliceerd voorbeeld: project bevat onderliggende taken {#complicated-example-project-has-children-tasks}

PIM = op uurbasis

EAC-methode = Berekenen op projectniveau

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
   <th> <br> <p><strong>Taak</strong> </p> </th> 
   <th> <br> <p><strong>Pln uur</strong> </p> </th> 
   <th> <br> <p><strong>Act Hrs</strong> </p> </th> 
   <th> <p><strong>% voltooid</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> </td> 
   <td> <p>10 uur</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>5 uur</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 3</p> </td> 
   <td> </td> 
   <td> <p>10 uur</p> </td> 
   <td> </td> 
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

1. Voeg 50 uur rechtstreeks toe aan het project (Meer>Uren>Logtijden).
1. **CPI voor Taak 2** = .1, berekend als volgt:\
   **CPI voor Taak 2** = *IF* Werkelijke uren > 0 *DAN* CPI = TotalBudgetedCostWorkPerformance/Actual Hours\
       *ELSE* CPI = 1\
   **CPI voor Taak 2** = 1 / 10\
   **CPI voor Taak 2** = .1

1. **EAC voor Taak 2** = 50 uur, berekend als volgt:\
   **EAC voor Taak 2** = *IF* CPI &lt;> 0 *DAN* EAC = geplande uren/CPI\
       *ELSE* EAC = geplande uren + werkelijke uren\
   **EAC voor Taak 2** = 5 / 0,1\
   **EAC voor Taak 2** = 50 uur

1. De CPI/EAC voor Taken 4, 5, en 6 zijn als volgt:\
   Taak 4: 0,4 / 25 uur\
   Taak 5: 0,75 / 20 uur\
   Taak 6: 1,2 uur

1. **CPI voor Taak 3** = .38 berekend als volgt:\
   **CPI voor Taak 3** = *IF* Werkelijke uren > 0 *DAN* CPI = TotalBudgetedCostWorkPerformance/Actual Hours\
       *ELSE* CPI = 1\
   **CPI voor Taak 3** = 11,5 / 30\
   **CPI voor Taak 3** = 0,38

1. **EAC voor Taak 3** = 65,22 uur, berekend als volgt:\
   **EAC voor Taak 3** = *IF* CPI &lt;> 0 *DAN* EAC = geplande uren/CPI\
       *ELSE* EAC = geplande uren + werkelijke uren\
   **EAC voor Taak 3** = 25 / 0,383333\
   **EAC voor Taak 3** = 65,22 uur

1. **CPI voor Taak 1** = .25, berekend als volgt:\
   **CPI voor Taak 1** = *IF* Werkelijke uren > 0 *DAN* CPI = TotalBudgetedCostWorkPerformance/Actual Hours\
       *ELSE* CPI = 1\
   **CPI voor Taak 1** = 12,5 / 50\
   **CPI voor Taak 1** = 0,25

1. **EAC voor Taak 1** = 120 uur, berekend als volgt:\
   **EAC voor Taak 1** = *IF* CPI &lt;> 0 *DAN* EAC = geplande uren / CPI\
       *ELSE* EAC = geplande uren + werkelijke uren\
   **EAC voor Taak 1** = 30/,25\
   **EAC voor Taak 1** = 120 uur

1. **CPI voor Project** = .22, berekend als volgt:\
   **CPI voor Project** = *IF* Werkelijke uren > 0 *DAN* CPI = TotalBudgetedCostWorkPerformance/Actual Hours\
       *ELSE* CPI = 1\
   **CPI voor Project** = 24,5 / 110\
   **CPI voor Project** = .22272\
   **CPI voor Project** = 0,22

1. **EAC voor project** = 224,49 uur, berekend als volgt:\
   **EAC voor project** = *IF* CPI &lt;> 0 *DAN* EAC = geplande uren/CPI\
       *ELSE* EAC = geplande uren + werkelijke uren\
   **EAC voor project** = 50 / 0,22272\
   **EAC voor project** = 224,49 uur

### PIM= op basis van kosten {#pim-cost-based}

* [Eenvoudig voorbeeld: project bevat geen onderliggende taken](#simple-example-project-has-no-children-tasks)
* [Gecompliceerd voorbeeld: project bevat onderliggende taken](#complicated-example-project-has-children-tasks)

#### Eenvoudig voorbeeld: project bevat geen onderliggende taken {#simple-example-project-has-no-children-tasks-1}

PIM = op kosten gebaseerd

EAC-methode = Berekenen op projectniveau

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
   <th> <br> <p><strong>Taak</strong> </p> </th> 
   <th> <br> <p><strong>Pln uur</strong> </p> </th> 
   <th> <br> <p><strong>LBR-kosten afspelen</strong> </p> </th> 
   <th> <br> <p><strong>Act Hrs</strong> </p> </th> 
   <th> <br> <p><strong>LBR-kosten van wet</strong> </p> </th> 
   <th> <p><strong>% voltooid</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> <p>5 uur</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>25 uur</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>25 uur</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 3</p> </td> 
   <td> <p>15 uur</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>25 uur</p> </td> 
   <td> <p>$2,500.00</p> </td> 
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
   <th> <p><strong>Taak</strong> </p> </th> 
   <th> <p><strong>Kosten</strong> </p> </th> 
   <th> <p><strong>Geplande hoeveelheid</strong> </p> </th> 
   <th> <p><strong>Werkelijk bedrag</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> <p>Taak 1 Exp 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> <p>Taak 1 Exp 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>Taak 2 Exp</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 3</p> </td> 
   <td> <p>Taak 3 Uitv</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
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
   <th> <p><strong>Kosten</strong> </p> </th> 
   <th> <p><strong>Geplande hoeveelheid</strong> </p> </th> 
   <th> <p><strong>Werkelijk bedrag</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Project Exp 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 1 Exp 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
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
   <th> <p><strong>Taak</strong> </p> </th> 
   <th> <p><strong>Niet-geplande kosten</strong> </p> </th> 
   <th> <p><strong>Ongewenste geplande kosten</strong> </p> </th> 
   <th> <p><strong>Opgelopen werkelijke kosten</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>$3,000.00</p> </td> 
   <td> <p>$2,300.00</p> </td> 
   <td> <p> $2,700.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. Voer vanuit Projecthandelingen de herberekening van financiën uit
1. **CPI voor Taak 1** = 0,14
1. **CPI*** voor taak 1** = .14 berekend als volgt:\
   **CPI**  **voor taak 1** = *IF* Werkelijke loonkosten + IncurredActualExpenseCost &lt;> 0 *DAN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = CPI_Labor\
   **CPI*** voor taak 1** = (100+300) / (2500+400)\
   **CPI**  **voor taak 1** = 400 / 2900\
   **CPI**  **voor taak 1**  = .14***

1. **EAC****voor taak 1** = $ 13.400,00\
   **CPI Arbeid**  **voor taak 1** = INDIEN werkelijke loonkosten &lt;> 0 VERVOLGENS

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Arbeid**  **voor taak 1** = 100/2500\
   **CPI Arbeid**  **voor taak 1** = 0,04 ****** EAC Arbeid ****voor taak 1 **=*IF *CPI_Labour &lt;> 0*DAN *EAC Labour = Geplande loonkosten/CPI_Labour\
   *    ELSE* EAC-arbeid = geplande loonkosten + werkelijke loonkosten\
   **EAC Arbeid ****voor taak 1** = 500.00/.04\
   **EAC-arbeid**** voor taak 1** = $ 12.500,00\
   **EAC-uitgaven**** voor taak 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC-uitgaven**** voor taak 1** = $ 400,00 + $ 500,00\
   **EAC-uitgaven**** voor taak 1** = $ 900,00\
   **EAC****voor taak 1** = EAC-arbeid + EAC-uitgaven\
   **EAC****voor taak 1**  = $ 12.500,00 + $ 900,00\
   **EAC****voor taak 1**  = $ 13.400,00

1. Hier zijn de waarden CPI/EAC voor Taak 2 en Taak 3:\
   Taak 2 = .19 / $8.433.33\
   Taak 3 = .44 / $6.950.00

1. **CPI voor Project** = .32, berekend als volgt:\
   **CPI**** voor project** = *IF* Werkelijke loonkosten + IncurredActualExpenseCost &lt;> 0 *DAN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI**** voor project** = (1000 + 2300) / (7500 + 2700)\
   **CPI**** voor project** = 3300 / 10200\
   **CPI**** voor project** = 0,32

1. **EAC voor project** = $ 28.200,00, berekend als volgt:\
   **CPI Arbeid*** voor Project** = INDIEN werkelijke loonkosten &lt;> 0 VERVOLGENS

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Arbeid*** voor Project** = 1000 / 7500\
   **CPI Arbeid*** voor Project** = .13333\
   **CPI Arbeid*** voor Project** = 0,13

   **EAC-arbeid*** voor project** = *IF* CPI_Labour &lt;> 0 *DAN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC-arbeid = geplande loonkosten + werkelijke loonkosten\
   **EAC-arbeid*** voor project** = 3000/,13333\
   **EAC-arbeid*** voor project** = $ 22.500,00

   **Uitgaven EAC*** Project** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **Uitgaven EAC*** Project** = $ 3000,00 + 2.700,00\
   **Uitgaven EAC*** Project** = $ 5.700,00

   **EAC*** Project** = EAC-arbeid + EAC-uitgaven\
   **EAC*** Project**  = $ 22.500,00 + $ 5.700,00\
   **EAC*** Project**  = $ 28.200,00

#### Gecompliceerd voorbeeld: project bevat onderliggende taken {#complicated-example-project-has-children-tasks-1}

PIM = op kosten gebaseerd

EAC-methode = Berekenen op projectniveau

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
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Taak</strong> </p> </th> 
   <th> <br> <p><strong>Pln uur</strong> </p> </th> 
   <th> <br> <p><strong>LBR-kosten afspelen</strong> </p> </th> 
   <th> <br> <p><strong>Act Hrs</strong> </p> </th> 
   <th> <br> <p><strong>LBR-kosten van wet</strong> </p> </th> 
   <th> <p><strong>% voltooid</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>5 uur</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 4</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 5</p> </td> 
   <td> <p>15 uur</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 6</p> </td> 
   <td> <p>20 uur</p> </td> 
   <td> <p>$2,000.00</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Voeg 50 uur rechtstreeks toe aan het project (More>Hours>Log Hours) zodat er $5.000.00 van daadwerkelijke arbeidskosten die rechtstreeks aan het project worden geregistreerd is. ****
1. Voeg uitgaven aan elke taak volgens de lijst toe hieronder (ik heb een lege rij binnen tussen elke taak toegevoegd om het gemakkelijker te maken te lezen):

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Taak</strong> </p> </th> 
   <th> <p><strong>Kosten</strong> </p> </th> 
   <th> <p><strong>Geplande hoeveelheid</strong> </p> </th> 
   <th> <p><strong>Werkelijk bedrag</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> <p>Taak 1 Exp 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>-$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> <p>Taak 1 Exp 2</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> <p>Taak 1 Exp 3</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>Taak 2 Uitp 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>Taak 2 Exp 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>Taak 2 Uitp 3</p> </td> 
   <td> <p>-$200.00</p> </td> 
   <td> <p>$600.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>Taak 2 Uitp 4</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 3</p> </td> 
   <td> <p>Taak 3 Uitv</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 4</p> </td> 
   <td> <p>Taak 4 Uitp 1</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 4</p> </td> 
   <td> <p>Taak 4 Exp 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 4 </p> </td> 
   <td> <p>Taak 4 Uitp. 3</p> </td> 
   <td> <p>-200.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 5</p> </td> 
   <td> <p>Taak 5 Uitp 1</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 5</p> </td> 
   <td> <p>Taak 5 Uitp 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 5</p> </td> 
   <td> <p>Taak 5 Uitp 3</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 6</p> </td> 
   <td> <p>Taak 6 Uitp 1</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 6</p> </td> 
   <td> <p>Taak 6 Uitp 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>-$300.0</p> </td> 
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
   <th> <p><strong>Kosten</strong> </p> </th> 
   <th> <p><strong>Geplande hoeveelheid</strong> </p> </th> 
   <th> <p><strong>Werkelijk bedrag</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Project Exp 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 1 Exp 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p> $0.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. Op basis van bovenstaande waarden worden de toegerekende/niet-geïnde kosten als volgt bepaald:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Taak</strong> </p> </th> 
   <th> <p><strong>Niet-geplande kosten</strong> </p> </th> 
   <th> <p><strong>Ongewenste geplande kosten</strong> </p> </th> 
   <th> <p><strong>Opgelopen werkelijke kosten</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$1,300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 4</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 5</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$1,100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 6</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$1000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Voer vanuit Projecthandelingen de herberekening van financiën uit
1. **CPI** voor taak 2 = .17, berekend als volgt:\
   **CPI-taak 2** = *IF* Werkelijke loonkosten + IncurredActualExpenseCost &lt;> 0 *DAN* CPI = (TotalBudgetedCostWorkPerformance + IncurredPlannedExpenseCost) / (ActualLabourCost + IncurredActualExpenseCost)\
   *   ELSE* CPI = CPI_Labor\
   **CPI*** Taak 2** = (100+300) / (1000+1300)\
   **CPI*** Taak 2**  = 400 / 2300\
   **CPI*** Taak 2**  = 0,17

1. **EAC** voor Taak 2 = $5.900.00\
   **CPI Arbeid*** Taak 2** = INDIEN werkelijke loonkosten &lt;> 0 VERVOLGENS CPI_Labour = TotalBudgetedCostWorkPerformance / Werkelijke loonkosten\
      ELSE CPI_Labor = 1\
   **CPI Arbeid*** Taak 2** = 100/1000\
   **CPI Arbeid*** Taak 2** = .1

   **EAC-arbeid*** Taak 2** = *IF* CPI_Labour &lt;> 0 *DAN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC-arbeid = geplande loonkosten + werkelijke loonkosten\
   **EAC-arbeid*** Taak 2** = 500,00/,1\
   **EAC-arbeid*** Taak 2** = $ 5.000,00 ****** EAC-uitgaven ****Taak 2 **= IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC-uitgaven ****Taak 2** = $1.300.00 + -$400.00\
   **EAC-uitgaven****Taak 2** = $ 900,00

   **EAC***Taak 2** = EAC-arbeid + EAC-uitgaven\
   **EAC***Taak 2**  = $ 5.000,00 + $ 900,00\
   **EAC***Taak 2**  = $ 5.900,00

1. CPI/EAC voor Taken 4, 5, en 6 worden bepaald de zelfde manier zodat zal ik enkel die hieronder waarden verstrekken:\
   Taak 4: 0,23 / $ 3.400,00\
   Taak 5: 0,64 / $ 3.100,00\
   Taak 6: 1,06 / $ 2.366,67

1. CPI voor Taak 3 = .31 berekend als volgt:\
   **CPI*** Taak 3** = *IF* Werkelijke loonkosten + IncurredActualExpenseCost &lt;> 0 *DAN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI*** Taak 3**  = (1,150 + 500) / (3000 + 2400)\
   **CPI*** Taak 3**  = 1650 / 5400\
   **CPI*** Taak 3**  = 0,31 ****** EAC voor Taak 3 **= $ 9.521,74, berekend als volgt:\
   **CPI Arbeid ****Taak 3** = indien werkelijke loonkosten &lt;> 0 DAN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Arbeid*** Taak 3** = 1150/3000\
   **CPI Arbeid*** Taak 3** = .383333\
   **CPI Arbeid*** Taak 3** = 0,38

   **EAC-arbeid*** Taak 3** = *IF* CPI_Labour &lt;> 0 *DAN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC-arbeid = geplande loonkosten + werkelijke loonkosten\
   **EAC-arbeid*** Taak 3** = $ 2.500,00 / ,383333\
   **EAC-arbeid*** Taak 3** = $ 6.521,74

   **EAC-uitgaven****Taak 3** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC-uitgaven****Taak 3** = $ 2.400,00 + $ 600,00\
   **EAC-uitgaven****Taak 3** = $ 3.000,00

   **EAC*** Taak 3** = EAC-arbeid + EAC-uitgaven\
   **EAC*** Taak 3**  = $ 6.521,74 + $ 3.000,00\
   **EAC*** Taak 3**  = $ 9.521,74

1. CPI voor Taak 1 = .16 berekend als volgt:\
   **CPI*** Taak 1** = *IF* Werkelijke loonkosten + IncurredActualExpenseCost &lt;> 0 *DAN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI*** Taak 1**  = (1250 + 300) / (5000 + 4500)\
   **CPI*** Taak 1**  = 1550 / 9500=\
   **CPI*** Taak 1**  = 0,16

1. EAC voor Taak 1 is $17.100.00 die als volgt wordt berekend:\
   **CPI Arbeid*** Taak 1** = INDIEN werkelijke loonkosten &lt;> 0 VERVOLGENS

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Arbeid*** Taak 1** = 1250 / 5000\
   **CPI Arbeid*** Taak 1** = 0,25

   **EAC-arbeid*** Taak 1** = *IF* CPI_Labour &lt;> 0 *DAN* EAC Labour = Geplande loonkosten / CPI_Labour\
   *   ELSE* EAC-arbeid = geplande loonkosten + werkelijke loonkosten\
   **EAC-arbeid*** Taak 1** = $ 3.000,00 / 0,25\
   **EAC-arbeid*** Taak 1** = $ 12.000,00

   **Uitgaven EAC****Taak 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Uitgaven EAC****Taak 1** = $ 4500 + 600\
   **Uitgaven EAC****Taak 1** = $ 5.100,00

   **EAC***Taak 1** = EAC-arbeid + EAC-uitgaven\
   **EAC***Taak 1**  = $ 12.000,00 + 5.100,00\
   **EAC***Taak 1**  = $ 17.100,00

1. CPI voor Project is .25\
   **CPI**** voor project** = *IF* Werkelijke loonkosten + IncurredActualExpenseCost &lt;> 0 *DAN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor

   **CPI**** voor project** = (2450 + 1900) / (11000 + 6700)\
   **CPI**** voor project** = 4350 / 17700\
   **CPI**** voor project** = 0,25

1. **EAC voor project** = $ 32.248,98, berekend als volgt:\
   **CPI Arbeid*** voor Project** = INDIEN werkelijke loonkosten &lt;> 0 VERVOLGENS

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Arbeid*** voor Project** = 2450 / 11000\
   **CPI Arbeid*** voor Project** = .22272\
   **CPI Arbeid*** voor Project** = 0,22

   **EAC-arbeid*** voor project** = *IF* CPI_Labour &lt;> 0 *DAN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC-arbeid = geplande loonkosten + werkelijke loonkosten\
   **EAC-arbeid*** voor project** = $ 5.000,00 / 0,22272\
   **EAC-arbeid*** voor project** = $ 22.448,97959\
   **EAC-arbeid*** voor project** = $ 22.448,98

   **Uitgaven EAC*** Project** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Uitgaven EAC*** Project** = $ 3.100,00 + $ 6.700,00\
   **Uitgaven EAC*** Project** = $ 9.800,00

   **EAC*** Project** = EAC-arbeid + EAC-uitgaven\
   **EAC*** Project**  = $ 22.448,98 + 9.800,00\
   **EAC*** Project**  = $ 32.248,98
