---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Schatting berekenen bij voltooiing (EAC)
description: Als prestatiemetrisch, vertegenwoordigt de Schatting bij Voltooiing (EAC) de verwachte totale kosten van uw project of taak wanneer het voltooit.
author: Lisa
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# Schatting berekenen bij voltooiing (EAC)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

Als prestatiemetrisch, vertegenwoordigt de Schatting bij Voltooiing (EAC) de verwachte totale kosten van uw project of taak wanneer het voltooit.

Als instelling kunt u definiëren hoe de EAC-waarde moet worden berekend.

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

## Definiëren hoe EAC moet worden berekend

Als deel van de voorkeur van het projectsysteem, kan de beheerder van Adobe Workfront bepalen hoe te om EAC te berekenen. EAC kan op een van de volgende twee manieren worden berekend:

* [ berekent op het projectniveau ](#calculate-at-the-project-level)
* [Rollen omhoog van taken en subtaken](#roll-up-from-tasks-and-subtasks)

Voor meer informatie over vestiging projectvoorkeur in Workfront, met inbegrip van hoe te om de Schatting bij Voltooiing te berekenen, zie [ systeem-brede projectvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

Als projectmanager, kunt u deze voorkeur op het projectniveau, in sub-lusje van de Financiën van het project ook veranderen. Voor meer informatie over het uitgeven van sub-lusje van Financiën van een project, zie [ informatie in het gebied van de Projectfinanciering beheren ](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### Berekenen op projectniveau {#calculate-at-the-project-level}

EAC voor de bovenliggende taak en het project wordt bepaald door de werkelijke uren/werkelijke loonkosten in de OAG-formules in te voeren. Deze berekening omvat Werkelijke uren/kosten en uitgaven die rechtstreeks aan de oudertaak of het project worden toegevoegd.

### Rollen omhoog van taken en subtaken {#roll-up-from-tasks-and-subtasks}

EAC voor de oudertaak en het project worden bepaald door EAC voor elke kindtaak samen te vatten. Deze berekening sluit Werkelijke uren/kosten en kosten uit die rechtstreeks aan de oudertaak of het project worden toegevoegd.

## Hoe wordt EAC berekend op basis van de Performance Index Methode (PIM)

In Workfront hangt de berekening voor EAC af van de geselecteerde Prestatisindexmethode (PIM) van het project. Voor meer informatie over het plaatsen van PIM voor uw systeem of voor uw project, zie [ Plaats de Methode van de Index van Prestaties (PIM) ](../../../manage-work/projects/project-finances/set-pim.md).

* [ berekent EAC gebruikend op uren-Gebaseerde PIM ](#calculate-eac-using-hour-based-pim)
* [EAC berekenen met PIM op basis van kosten](#calculate-eac-using-cost-based-pim)

### EAC berekenen met PIM op basis van uren {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42; als de Index van de Prestaties van Kosten [ de Index van de Prestaties van Kosten berekent (CPI) ](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0, EAC = Totale Geplande Uren + Werkelijke Uren. Dit komt voor wanneer de uren zijn gevangen, maar project/de taak is bij 0% volledig.

Voor meer informatie over het berekenen van CPI, zie [ de Index van de Prestaties van de Kosten (CPI) berekenen ](../../../manage-work/projects/project-finances/calculate-cpi.md).

### EAC berekenen met PIM op basis van kosten {#calculate-eac-using-cost-based-pim}

De EAC van een project wordt berekend aan de hand van de volgende formule:

```
EAC = EAC Labor + EAC Expense 
```

<pre>EAC Arbeid = <em> ALS </em> CPI Arbeid &lt;&gt; 0 DAN EAC Arbeid = Geplande Arbeidskosten/CPI Arbeid</pre><pre><em> ELSE </em> EAC Arbeid = Geplande Kosten van de Arbeid + Werkelijke Kosten van de Arbeid</pre><pre>CPI-arbeid = indien werkelijke loonkosten &lt;&gt; 0 VERVOLGENS CPI-arbeid = TotalBudgetedCostWorkPerformance / Werkelijke loonkosten</pre><pre>ELSE CPI Labour = 1 </pre>Bij de berekening van de EAC wordt rekening gehouden met de volgende velden:

* Totaal uitgevoerd begrotingskostenwerk (BCWP) = het resultaat van de vermenigvuldiging van de begrote kosten van het geplande werk (begrote kosten) en het percentage van de tot dusver voltooide taak.

  Voor informatie over het totale Gedragsde Uitgevoerde Werk van Kosten (BCWP), zie [ Gemaakt het Geplande Gepresteerde Werk van Kosten (BCWP) ](../../../manage-work/projects/project-finances/calculate-bcwp.md) berekenen.

   * **voor een niet oudertaak:**

     ```
     Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
     ```

   * **voor een oudertaak:**
Totaal uitgevoerd begrotingskostenwerk = de som van het veld Totaal begrote kosten uitgevoerd voor alle directe onderliggende taken.

   * **voor een project:**
Totaal uitgevoerd begroot kostenwerk = de som van het totaal uitgevoerd budget-kostenwerkveld voor alle taken op het hoogste niveau (ouders en zelfstandige taken).

* EAC-kosten = het resultaat van de optelling van de indirecte werkelijke kosten bij de niet-geplande kosten. Deze wordt berekend aan de hand van de volgende formule:

  ```
  EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
  ```

   * Opgelopen werkelijke kosten = de som van het veld Gepland bedrag voor alle uitgaven waarbij het veld Werkelijk bedrag > 0 is. Als u bijvoorbeeld een uitgave maakt voor Taak 1 en $500,00 invoert in het veld Gepland bedrag en een bedrag > 0 in het veld Werkelijk bedrag (d.w.z. $600,00), is de geplande onkosten voor deze taak $500,00.
   * Niet-gedekte geplande kosten = de som van het veld Gepland bedrag voor alle uitgaven waarbij het veld Werkelijk bedrag = 0 is. Als u bijvoorbeeld twee uitgaven maakt voor taak 1, waarbij voor de eerste uitgave de waarde in het veld Gepland bedrag $500,00 is en de waarde in het veld Ware bedrag $600,00 en voor de tweede uitgave, de waarde in het veld Gepland bedrag $300,00 en de waarde in het veld Ware bedrag $0,00, is, is de waarde van De niet-geplande kosten voor deze taak zijn $ 300,00.

## Plaats EAC in een project of een taak

1. Ga naar het project of de taak waar u EAC wilt bekijken.
1. Breid {de Details van het 0} Project **of** Details van Taken **in het linkerpaneel van het project of de taak uit, afhankelijk van waar u EAC bekijkt.**

1. Klik **Financiën**.

   De waarde EAC toont op **Schatting bij het gebied van de Voltooiing**.

   ![ EAC op project ](assets/eac-highlighted-on-project-350x112.png)
