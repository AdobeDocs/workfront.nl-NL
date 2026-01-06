---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Voorbeeld van berekening - EAC berekenen op projectniveau
description: In dit artikel wordt een voorbeeld gegeven van de berekening van de raming bij voltooiing (EAC) van een project op projectniveau in Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '2213'
ht-degree: 0%

---

# Berekeningsvoorbeeld - berekening EAC op projectniveau

## EAC-methode: berekenen op projectniveau

* [&#x200B; PIM = op uur-Gebaseerde &#x200B;](#pim-hour-based)
* [PIM= op basis van kosten](#pim-cost-based)

### PIM = op uurbasis {#pim-hour-based}

* [&#x200B; Eenvoudig voorbeeld: het project heeft geen kindtaken &#x200B;](#simple-example-project-has-no-children-tasks)
* [Gecompliceerd voorbeeld: project heeft onderliggende taken](#complicated-example-project-has-children-tasks)

#### Eenvoudig voorbeeld: project heeft geen onderliggende taken {#simple-example-project-has-no-children-tasks}

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
1. **CPI voor Taak 1** = .04 berekend als volgt:\
   **CPI voor Taak 1** = *ALS* Ware Uren > 0 *VERVOLGENS* CPI = TotalBudgetedCostWorkPerformance/Ware Uren\
   *ELSE* CPI = 1\
   **CPI voor Taak 1** = 1 / 25\
   **CPI voor Taak 1** = .04

1. **EAC voor Taak 1** = 125 uren berekend als volgt:\
   **EAC voor Taak 1** = *ALS* CPI &lt;> 0 *VERVOLGENS* EAC = Geplande Uren/CPI\
   *ELSE* EAC = Geplande Uren + Werkelijke Uren\
   **EAC voor Taak 1** = 5 / .04\
   **EAC voor Taak 1** = 125 uren***

1. CPI/EAC voor de taken 2 en 3 zijn:\
   Taak 2 = 0,12 / 83,33 uur\
   Taak 3 = 0,24 / 62,5 uur

1. **CPI voor Project** = .13 berekend als volgt:\
   **CPI voor Project** = *ALS* Ware Uren > 0 *DAN* CPI = TotalBudgetedCostWorkPerformance/Ware Uren\
   *ELSE* CPI = 1\
   **CPI voor Project** = 10/75\
   **CPI voor Project** = .13

1. **EAC voor Project** = 225 uren berekend als volgt:\
   **EAC voor Project** = *ALS* CPI &lt;> 0 *VERVOLGENS* EAC = Geplande Uren/CPI\
   *ELSE* EAC = Geplande Uren + Werkelijke Uren\
   **EAC voor Project** = 30 /.13333\
   **EAC voor Project** = 225 uren

#### Gecompliceerd voorbeeld: project heeft onderliggende taken {#complicated-example-project-has-children-tasks}

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

1. Voeg 50 uur rechtstreeks toe aan het project (Meer>Uren>Logtijden).
1. **CPI voor Taak 2** = .1 berekend als volgt:\
   **CPI voor Taak 2** = *ALS* Ware Uren > 0 *VERVOLGENS* CPI = TotalBudgetedCostWorkPerformance/Ware Uren\
   *ELSE* CPI = 1\
   **CPI voor Taak 2** = 1 / 10\
   **CPI voor Taak 2** = .1

1. **EAC voor Taak 2** = 50 uren berekend als volgt:\
   **EAC voor Taak 2** = *ALS* CPI &lt;> 0 *VERVOLGENS* EAC = Geplande Uren/CPI\
   *ELSE* EAC = Geplande Uren + Werkelijke Uren\
   **EAC voor Taak 2** = 5 / .1\
   **EAC voor Taak 2** = 50 uren

1. De CPI/EAC voor Taken 4, 5, en 6 zijn als volgt:\
   Taak 4: 0,4 / 25 uur\
   Taak 5: 0,75 / 20 uur\
   Taak 6: 1,2 / 16,67 uur

1. **CPI voor Taak 3** = .38 berekend als volgt:\
   **CPI voor Taak 3** = *ALS* Ware Uren > 0 *VERVOLGENS* CPI = TotalBudgetedCostWorkPerformance/Ware Uren\
   *ELSE* CPI = 1\
   **CPI voor Taak 3** = 11.5 / 30\
   **CPI voor Taak 3** = .38

1. **EAC voor Taak 3** = 65.22 uren berekend als volgt:\
   **EAC voor Taak 3** = *ALS* CPI &lt;> 0 *VERVOLGENS* EAC = Geplande Uren/CPI\
   *ELSE* EAC = Geplande Uren + Werkelijke Uren\
   **EAC voor Taak 3** = 25 / .383333\
   **EAC voor Taak 3** = 65.22 uren

1. **CPI voor Taak 1** = .25 berekend als volgt:\
   **CPI voor Taak 1** = *ALS* Ware Uren > 0 *VERVOLGENS* CPI = TotalBudgetedCostWorkPerformance/Ware Uren\
   *ELSE* CPI = 1\
   **CPI voor Taak 1** = 12.5 / 50\
   **CPI voor Taak 1** = .25

1. **EAC voor Taak 1** = 120 uren berekend als volgt:\
   **EAC voor Taak 1** = *ALS* CPI &lt;> 0 *VERVOLGENS* EAC = Geplande Uren/CPI\
   *ELSE* EAC = Geplande Uren + Werkelijke Uren\
   **EAC voor Taak 1** = 30/.25\
   **EAC voor Taak 1** = 120 uren

1. **CPI voor Project** = .22 berekend als volgt:\
   **CPI voor Project** = *ALS* Ware Uren > 0 *DAN* CPI = TotalBudgetedCostWorkPerformance/Ware Uren\
   *ELSE* CPI = 1\
   **CPI voor Project** = 24.5 / 110\
   **CPI voor Project** = .2272\
   **CPI voor Project** = .22

1. **EAC voor Project** = 224.49 uren berekend als volgt:\
   **EAC voor Project** = *ALS* CPI &lt;> 0 *VERVOLGENS* EAC = Geplande Uren/CPI\
   *ELSE* EAC = Geplande Uren + Werkelijke Uren\
   **EAC voor Project** = 50 /.22272\
   **EAC voor Project** = 224.49 uur

### PIM= op basis van kosten {#pim-cost-based}

* [&#x200B; Eenvoudig voorbeeld: het project heeft geen kindtaken &#x200B;](#simple-example-project-has-no-children-tasks)
* [Gecompliceerd voorbeeld: project heeft onderliggende taken](#complicated-example-project-has-children-tasks)

#### Eenvoudig voorbeeld: project heeft geen onderliggende taken {#simple-example-project-has-no-children-tasks-1}

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
   <td> <p> $ 2.700,00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. Voer vanuit Projecthandelingen de herberekening van financiën uit
1. **CPI voor Taak 1** = .14
1. **CPI**&#x200B;**for Taak 1** = .14 berekend als volgt:\
   **CPI** **voor Taak 1** = ** de Ware Kosten van de Arbeid + IncurredActualExpenseCost &lt;> 0 *VERVOLGENS*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor\
     **CPI**&#x200B;**for Taak 1** = (100+300) / (2500+400)\
     **CPI** **voor Taak 1** = 400/2900\
     **CPI** **voor Taak 1** = .14***

1. **EAC**&#x200B;**for Taak 1** = $13.400.00\
   **CPI Arbeid** **voor Taak 1** = ALS de Ware loonkosten &lt;> 0 DAN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **CPI Arbeid** **voor Taak 1** = 100/2500\
   **CPI Arbeid** **voor Taak 1** = .04&#x200B;*** &#x200B;** Ecc Arbeid **&#x200B;**&#x200B;voor Taak 1**=* IF *CPI_Labor &lt;> 0* *Ecc Arbeid = Geplande Arbeid Kosten/CPI_Arbeid
   * ELSE* EAC Labour = Geplande loonkosten + Werkelijke loonkosten\
     **Ecc Arbeid**&#x200B;**voor Taak 1** = 500.00/.04\
     **Ecc Arbeid**&#x200B;**voor Taak 1** = $12.500.00\
     **uitgaven EAC**&#x200B;**voor Taak 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
     **uitgaven EAC**&#x200B;**voor Taak 1** = $400.00 + $500.00\
     **uitgaven EAC**&#x200B;**voor Taak 1** = $900.00\
     **EAC**&#x200B;**for Taak 1** = EC Arbeid + EAC Uitgaven\
     **EAC**&#x200B;**for Taak 1** = $12.500.00 + $900.00\
     **EAC**&#x200B;**for Taak 1** = $13.400.00

1. Hier zijn de waarden CPI/EAC voor Taak 2 en Taak 3:\
   Taak 2 = .19 / $8.433.33\
   Taak 3 = .44 / $6.950.00

1. **CPI voor Project** = .32 berekend als volgt:\
   **CPI**&#x200B;**for Project** = ** de Ware Kosten van de Arbeid + IncurredActualExpenseCost &lt;> 0 *DAN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor\
     **CPI**&#x200B;**for Project** = (1000 + 2300) / (7500 + 2700)\
     **CPI**&#x200B;**for Project** = 3300/10200\
     **CPI**&#x200B;**for Project** = .32

1. **EAC voor Project** = $28.200.00 berekende als volgt:\
   **CPI Arbeid**&#x200B;**voor Project** = ALS de Ware Arbeidskosten &lt;> 0 DAN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **CPI Arbeid**&#x200B;**voor Project** = 1000 / 7500\
   **CPI Arbeid**&#x200B;**for Project** = .13333\
   **CPI Arbeid**&#x200B;**for Project** = .13

   **EAC Arbeid**&#x200B;**for Project** = *ALS* CPI_Labour &lt;> 0 *VERVOLGENS*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   * ELSE* EAC Labour = Geplande loonkosten + Werkelijke loonkosten\
     **Arbeid EAC**&#x200B;**voor Project** = 3000/.13333\
     **Ecc Arbeid**&#x200B;**voor Project** = $22.500.00

   **uitgaven EAC***Project** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **uitgaven EAC***Project** = $3000.00 + 2.700.00\
   **uitgaven EAC***Project** = $5.700.00

   **EAC***Project** = EC Arbeid + EAC Uitgaven\
   **EAC***Project** = $22.500.00 + $5.700.00\
   **EAC**&#x200B;**Project** = $28.200.00

#### Gecompliceerd voorbeeld: project heeft onderliggende taken {#complicated-example-project-has-children-tasks-1}

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
   <td> </td> 
   <td> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>5 uur</p> </td> 
   <td> <p>$ 500,00</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 4</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 5</p> </td> 
   <td> <p>15 uur</p> </td> 
   <td> <p>$ 1.500,00</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 6</p> </td> 
   <td> <p>20 uur</p> </td> 
   <td> <p>$ 2.000,00</p> </td> 
   <td> <p>10 uur</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Voeg 50 uur rechtstreeks toe aan het project (More>Hours>Log Hours) zodat er $5.000.00 van daadwerkelijke arbeidskosten die rechtstreeks aan het project worden geregistreerd is. **&#x200B;**
1. Voeg uitgaven aan elke taak volgens de lijst toe hieronder (ik heb een lege rij binnen tussen elke taak toegevoegd om het gemakkelijker te maken te lezen):

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
   <td> <p>- $ 400,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> <p>Taak 1 Exp 2</p> </td> 
   <td> <p>-$ 500,00</p> </td> 
   <td> <p>$ 800,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> <p>Taak 1 Exp 3</p> </td> 
   <td> <p>$ 400,00</p> </td> 
   <td> <p>$ 0,00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>Taak 2 Uitp 1</p> </td> 
   <td> <p>$ 500,00</p> </td> 
   <td> <p>$ 700,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>Taak 2 Exp 2</p> </td> 
   <td> <p>- $ 400,00</p> </td> 
   <td> <p>$ 0,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>Taak 2 Uitp 3</p> </td> 
   <td> <p>- $ 200,00</p> </td> 
   <td> <p>$ 600,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>Taak 2 Uitp 4</p> </td> 
   <td> <p>$ 700,00</p> </td> 
   <td> <p>- $ 200,00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 3</p> </td> 
   <td> <p>Taak 3 Uitv</p> </td> 
   <td> <p>$ 0,00</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 4</p> </td> 
   <td> <p>Taak 4 Uitp 1</p> </td> 
   <td> <p>$ 800,00</p> </td> 
   <td> <p>$ 0,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 4</p> </td> 
   <td> <p>Taak 4 Exp 2</p> </td> 
   <td> <p>- $ 100,00</p> </td> 
   <td> <p>$ 300,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 4 </p> </td> 
   <td> <p>Taak 4 Uitp. 3</p> </td> 
   <td> <p>-200,00</p> </td> 
   <td> <p>$ 0,00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 5</p> </td> 
   <td> <p>Taak 5 Uitp 1</p> </td> 
   <td> <p>$ 700,00</p> </td> 
   <td> <p>$ 800,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 5</p> </td> 
   <td> <p>Taak 5 Uitp 2</p> </td> 
   <td> <p>- $ 100,00</p> </td> 
   <td> <p>$ 300,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 5</p> </td> 
   <td> <p>Taak 5 Uitp 3</p> </td> 
   <td> <p>- $ 400,00</p> </td> 
   <td> <p>- $ 200,00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 6</p> </td> 
   <td> <p>Taak 6 Uitp 1</p> </td> 
   <td> <p>$ 600,00</p> </td> 
   <td> <p>$ 700,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 6</p> </td> 
   <td> <p>Taak 6 Uitp 2</p> </td> 
   <td> <p>$ 500,00</p> </td> 
   <td> <p>-$ 300,0</p> </td> 
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
   <td> <p> $ 0,00 <strong></strong></p> </td> 
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
   <th> <p><strong> Taak </strong> </p> </th> 
   <th> <p><strong> niet Beoogde Geplande Uitgaven </strong> </p> </th> 
   <th> <p><strong> Beoogde Beoogde Uitgaven </strong> </p> </th> 
   <th> <p><strong> curred daadwerkelijke uitgaven </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Taak 1</p> </td> 
   <td> <p>$ 400,00</p> </td> 
   <td> <p>-$ 500,00</p> </td> 
   <td> <p>$ 800,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 2</p> </td> 
   <td> <p>- $ 400,00</p> </td> 
   <td> <p>$ 300,00</p> </td> 
   <td> <p>$ 1.300,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 3</p> </td> 
   <td> <p>$ 0,00</p> </td> 
   <td> <p>$ 0,00</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 4</p> </td> 
   <td> <p>$ 600,00</p> </td> 
   <td> <p>- $ 100,00</p> </td> 
   <td> <p>$ 300,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 5</p> </td> 
   <td> <p>$ 0,00</p> </td> 
   <td> <p>$ 600,00</p> </td> 
   <td> <p>$ 1.100,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taak 6</p> </td> 
   <td> <p>$ 0,00</p> </td> 
   <td> <p>$ 600,00</p> </td> 
   <td> <p>$ 700,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Project</p> </td> 
   <td> <p>$ 2.500,00</p> </td> 
   <td> <p>$ 1000,00</p> </td> 
   <td> <p>$ 1.500,00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Voer vanuit Projecthandelingen de herberekening van financiën uit
1. **CPI** voor Taak 2 = .17 berekend als volgt:\
   **CPI Taak 2** = ** Ware Arbeidskosten + IncurredActualExpenseCost &lt;> 0 *VEREN* CPI = (TotalBudgetedCostWorkPerformance + IncurredPlannedExpenseCost) / (ActualLabourCost + IncurredActualExpenseCost)
   * ELSE* CPI = CPI_Labor\
     **CPI**&#x200B;**Taak 2** = (100+300) / (1000+1300)\
     **CPI**&#x200B;**Taak 2** = 400 / 2300\
     **CPI**&#x200B;**Taak 2** = .17

1. **EAC** voor Taak 2 = $5.900.00\
   **CPI Arbeid**&#x200B;**Taak 2** = ALS Ware Arbeidskosten &lt;> 0 DAN CPI_Arbeid = TotalBudgetedCostWorkPerformance/Ware Arbeidskosten\
   ELSE CPI_Labor = 1\
   **CPI Arbeid***Taak 2** = 100/1000\
   **CPI Arbeid***Taak 2** = .1

   **Ecc Arbeid***Taak 2** = *ALS* CPI_Labor &lt;> 0 *DAN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   * ELSE* EAC Labour = Geplande loonkosten + Werkelijke loonkosten\
     **Ecc Arbeid***Taak 2** = 500.00/.1\
     **Ecc Arbeid***Taak 2 **&#x200B; = $5.000.00 &#x200B;**&#x200B;**&#x200B;** Ecc- Uitgaven **&#x200B;**&#x200B;Taak 2 **= IncurredActualExpenseCost + NotIncurredPlannedExpense\
     **EAC Vergoeding &#x200B;**&#x200B;**Taak 2** = $1,300.00 + -$400.00\
     **uitgaven EAC***Taak 2** = $900.00

   **EAC**&#x200B;**Taak 2** = EC Arbeid + EAC Uitgaven\
   **EAC**&#x200B;**Taak 2** = $5.000.00 + $900.00\
   **EAC**&#x200B;**Taak 2** = $5.900.00

1. CPI/EAC voor Taken 4, 5, en 6 worden bepaald de zelfde manier zodat zal ik enkel die hieronder waarden verstrekken:\
   Taak 4: 0,23 / $ 3.400,00\
   Taak 5: 0,64 / $ 3.100,00\
   Taak 6: 1,06 / $ 2.366,67

1. CPI voor Taak 3 = .31 berekend als volgt:\
   **CPI***Taak 3 **&#x200B; = &#x200B;** Ware Arbeidskosten + IncurredActualExpenseCost &lt;> 0 *VERVOLGENS*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor\
     **CPI**&#x200B;**Taak 3** = (1.150 + 500) / (3000 + 2400)\
     **CPI**&#x200B;**Taak 3** = 1650/5400\
     **CPI***Taak 3 **&#x200B; = .31 &#x200B;**&#x200B;**&#x200B;** EAC voor Taak 3 **= $9.521.74 berekend als volgt:\
     **CPI Arbeid &#x200B;**&#x200B;**Taak 3** = ALS de Ware Arbeidskosten &lt;> 0 DAN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **CPI Arbeid***Taak 3** = 1150/3000\
   **CPI Arbeid**&#x200B;**Taak 3** = .383333\
   **CPI Arbeid**&#x200B;**Taak 3** = .38

   **Ecc Arbeid***Taak 3 **&#x200B; = &#x200B;** CPI_Labor &lt;> 0 *DAN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   * ELSE* EAC Labour = Geplande loonkosten + Werkelijke loonkosten\
     **Arbeid EAC***Taak 3** = $2.500.00 / .383333\
     **Ecc Arbeid***Taak 3** = $6.521.74

   **uitgaven EAC***Taak 3** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **uitgaven EAC***Taak 3** = $2.400.00 + $600.00\
   **uitgaven EAC***Taak 3** = $3.000.00

   **EAC***Taak 3** = EC Arbeid + EAC Uitgaven\
   **EAC**&#x200B;**Taak 3** = $6.521.74 + $3.000.00\
   **EAC**&#x200B;**Taak 3** = $9.521.74

1. CPI voor Taak 1 = .16 berekend als volgt:\
   **CPI***Taak 1 **&#x200B; = &#x200B;** de Ware Arbeidskosten + IncurredActualExpenseCost &lt;> 0 *VERVOLGENS*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor\
     **CPI**&#x200B;**Taak 1** = (1250 + 300) / (5000 + 4500)\
     **CPI**&#x200B;**Taak 1** = 1550/9500=\
     **CPI**&#x200B;**Taak 1** = .16

1. EAC voor Taak 1 is $17.100.00 die als volgt wordt berekend:\
   **CPI Arbeid**&#x200B;**Taak 1** = ALS de Ware Arbeidskosten &lt;> 0 DAN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **CPI Arbeid**&#x200B;**Taak 1** = 1250 / 5000\
   **CPI Arbeid**&#x200B;**Taak 1** = .25

   **EAC Arbeid***Taak 1** = *ALS* CPI_Labor &lt;> 0 *DAN* EAC Arbeid = Geplande Arbeidskosten / CPI_Arbeid
   * ELSE* EAC Labour = Geplande loonkosten + Werkelijke loonkosten\
     **Ecc Arbeid***Taak 1** = $3.000.00 / .25\
     **Ecc Arbeid***Taak 1** = $12.000.00

   **uitgaven EAC***Taak 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **uitgaven EAC**&#x200B;**Taak 1** = $4500 + 600\
   **uitgaven EAC***Taak 1** = $5.100.00

   **EAC**&#x200B;**Taak 1** = EC Arbeid + EAC Uitgaven\
   **EAC**&#x200B;**Taak 1** = $12.000.00 + 5.100.00\
   **EAC**&#x200B;**Taak 1** = $17.100.00

1. CPI voor Project is .25\
   **CPI**&#x200B;**for Project** = ** de Ware Kosten van de Arbeid + IncurredActualExpenseCost &lt;> 0 *DAN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor

   **CPI**&#x200B;**for Project** = (2450 + 1900) / (11000 + 6700)\
   **CPI**&#x200B;**for Project** =   4350 / 17700\
   **CPI**&#x200B;**for Project** = .25

1. **EAC voor Project** = $32.248.98 berekende als volgt:\
   **CPI Arbeid**&#x200B;**voor Project** = ALS de Ware Arbeidskosten &lt;> 0 DAN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **CPI Arbeid**&#x200B;**voor Project** = 2450 / 11000\
   **CPI Arbeid**&#x200B;**for Project** = .22272\
   **CPI Arbeid**&#x200B;**for Project** = .22

   **EAC Arbeid**&#x200B;**for Project** = *ALS* CPI_Labour &lt;> 0 *VERVOLGENS*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   * ELSE* EAC Labour = Geplande loonkosten + Werkelijke loonkosten\
     **Arbeid EAC**&#x200B;**voor Project** = $5.000.00 /.22272\
     **Arbeid EAC**&#x200B;**voor Project** = $22.448.97959\
     **Arbeid EAC**&#x200B;**voor Project** = $22.448.98

   **uitgaven EAC***Project** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **uitgaven EAC***Project** = $3,100.00 + $6,700.00\
   **uitgaven EAC***Project** = $9.800.00

   **EAC***Project** = EC Arbeid + EAC Uitgaven\
   **EAC***Project** = $22.448.98 + 9.800.00\
   **EAC**&#x200B;**Project** = $32.248.98
