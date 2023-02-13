---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Schatting berekenen bij voltooiing (EAC)
description: Als prestatiemetrisch, vertegenwoordigt de Schatting bij Voltooiing (EAC) de verwachte totale kosten van uw project of taak wanneer het voltooit.
author: Alina
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# Schatting berekenen bij voltooiing (EAC)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

Als prestatiemetrisch, vertegenwoordigt de Schatting bij Voltooiing (EAC) de verwachte totale kosten van uw project of taak wanneer het voltooit.

Als instelling kunt u definiëren hoe de EAC-waarde moet worden berekend. 

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
   <td> <p>Toegang tot projecten en financiële gegevens weergeven</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De mening of hogere toestemmingen aan het project met toestemmingen aan de Financiën van de Mening</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Definiëren hoe EAC moet worden berekend

Als deel van de voorkeur van het projectsysteem, kan de beheerder van Adobe Workfront bepalen hoe te om EAC te berekenen. EAC kan op een van de volgende twee manieren worden berekend:

* [Berekenen op projectniveau](#calculate-at-the-project-level)
* [Rollen omhoog van taken en subtaken](#roll-up-from-tasks-and-subtasks)

Ga voor meer informatie over het instellen van projectvoorkeuren in Workfront, waaronder hoe u de schatting bij voltooiing kunt berekenen naar [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Als projectmanager, kunt u deze voorkeur op het projectniveau, in sub-lusje van de Financiën van het project ook veranderen. Zie voor meer informatie over het bewerken van het subtabblad Financiën van een project [Informatie beheren in het gebied Projectfinanciering](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### Berekenen op projectniveau {#calculate-at-the-project-level}

EAC voor de bovenliggende taak en het project wordt bepaald door de werkelijke uren/werkelijke loonkosten in de OAG-formules in te voeren. Deze berekening omvat Werkelijke uren/kosten en uitgaven die rechtstreeks aan de oudertaak of het project worden toegevoegd.

### Rollen omhoog van taken en subtaken {#roll-up-from-tasks-and-subtasks}

EAC voor de oudertaak en het project worden bepaald door EAC voor elke kindtaak samen te vatten. Deze berekening sluit Werkelijke uren/kosten en kosten uit die rechtstreeks aan de oudertaak of het project worden toegevoegd.

## Hoe wordt EAC berekend op basis van de Performance Index Methode (PIM)

In Workfront hangt de berekening voor EAC af van de geselecteerde Prestatisindexmethode (PIM) van het project. Voor meer informatie over het plaatsen van PIM voor uw systeem of voor uw project, zie [De PIM-methode (Performance Index) instellen](../../../manage-work/projects/project-finances/set-pim.md).

* [EAC berekenen met PIM op basis van uren](#calculate-eac-using-hour-based-pim)
* [EAC berekenen met PIM op basis van kosten](#calculate-eac-using-cost-based-pim)

### EAC berekenen met PIM op basis van uren {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;Als kostenprestatie-index [Kostenprestatie-index (CPI) berekenen](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0, EAC = totaal geplande uren + werkelijke uren. Dit komt voor wanneer de uren zijn gevangen, maar project/de taak is bij 0% volledig.

Voor meer informatie over het berekenen van CPI, zie [Kostenprestatie-index (CPI) berekenen](../../../manage-work/projects/project-finances/calculate-cpi.md).

### EAC berekenen met PIM op basis van kosten {#calculate-eac-using-cost-based-pim}

De EAC van een project wordt berekend aan de hand van de volgende formule:

```
EAC = EAC Labor + EAC Expense 
```

<pre>EAC Labour =  <em>IF</em> CPI Arbeid &lt;&gt; 0 VERVOLGENS EAC Arbeid = Geplande loonkosten / CPI Arbeid</pre><pre><em>ELSE</em> EAC-arbeid = geplande loonkosten + werkelijke loonkosten</pre><pre>CPI-arbeid = indien werkelijke loonkosten &lt;&gt; 0 VERVOLGENS CPI-arbeid = TotalBudgetedCostWorkPerformance / Werkelijke loonkosten</pre><pre>ELSE CPI Labour = 1 </pre>Bij de berekening van de EAC wordt rekening gehouden met de volgende velden:

* Totaal uitgevoerd begrotingskostenwerk (BCWP) = het resultaat van de vermenigvuldiging van de begrote kosten van het geplande werk (begrote kosten) en het percentage van de tot dusver voltooide taak.

   Voor informatie over het totale Gedetailleerde Geoefende Werk van Kosten (BCWP), zie [Geraamd het Geregistreerde Uitgevoerde Werk van Kosten berekenen (BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

   * **Voor een niet-bovenliggende taak:**

      ```
      Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
      ```

   * **Voor een bovenliggende taak:**
Totaal uitgevoerd begrotingskostenwerk = de som van het veld Totaal begrote kosten uitgevoerd voor alle directe onderliggende taken.

   * **Voor een project:**
Totaal uitgevoerd begroot kostenwerk = de som van het totaal uitgevoerd budget-kostenwerkveld voor alle taken op het hoogste niveau (ouders en zelfstandige taken). 

* EAC-kosten = het resultaat van de optelling van de indirecte werkelijke kosten bij de niet-geplande kosten. Deze wordt berekend aan de hand van de volgende formule:

   ```
   EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
   ```

   * Opgelopen werkelijke kosten = de som van het veld Gepland bedrag voor alle uitgaven waarbij het veld Werkelijk bedrag > 0 is. Bijvoorbeeld, als u een uitgave voor Taak 1 creeert en $500.00 op het Geplande gebied van het Bedrag en een bedrag > 0 op het Werkelijke gebied van het Bedrag ingaat (d.w.z. $ 600,00), de Geplande Vergoeding Kosten voor deze taak is $500.00.
   * Niet-gedekte geplande kosten = de som van het veld Gepland bedrag voor alle uitgaven waarbij het veld Werkelijk bedrag = 0 is. Als u bijvoorbeeld twee uitgaven maakt voor taak 1, waarbij voor de eerste uitgave de waarde in het veld Gepland bedrag $500,00 is en de waarde in het veld Ware bedrag $600,00 en voor de tweede uitgave, de waarde in het veld Gepland bedrag $300,00 en de waarde in het veld Ware bedrag $0,00, is, is de waarde van De niet-geplande kosten voor deze taak zijn $ 300,00. 

## Plaats EAC in een project of een taak

1. Ga naar het project of de taak waar u EAC wilt bekijken.
1. Uitbreiden **Projectdetails** of **Taken** in het linkerpaneel van het project of de taak, afhankelijk van waar u EAC bekijkt.

1. Klikken **Financiën**. 

   De EAC-waarde wordt weergegeven in het dialoogvenster **Schatting bij voltooiing** veld.

   ![](assets/eac-highlighted-on-project-350x112.png)
