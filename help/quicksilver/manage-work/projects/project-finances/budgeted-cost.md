---
content-type: reference
product-area: projects
navigation-topic: financials
title: Geraamde kosten berekenen
description: Bereken de Beoogde Voortgang van het Project CostTracking met een Rapport van het Gebruik""
author: Lisa
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Geraamde kosten berekenen

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked from "Tracking Project Progress with a Utilization Report"</p>
<p>Keep the structure of this article similar to Calculating Budgeted Labor Cost)</p>
</div>
-->

De begrote Kosten van een project zijn de totale kosten verbonden aan het project zoals geschat wanneer u het project plant.

## Overzicht van begrote kosten in een project

U kunt de begrote kosten van een project niet handmatig wijzigen. Adobe Workfront berekent de begrote kosten aan de hand van de volgende formule:

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* De **Plan van het Middel begrote Arbeidskosten** in de berekening hierboven is de kosten verbonden aan de baanrollen in het project.

  U kunt de begrote arbeidskosten van een project in het gebied van de Begroting van het Middel van het BedrijfsGeval of de Planner van het Middel volgen.

  >[!TIP]
  >
  >  De begrote Arbeidskosten van een project in het BedrijfsGeval toont als Voorgenomen Kosten van de Arbeid van het Plan van het Middel in rapporten en lijsten.

  Voor informatie over de Begrotende Kosten van de Arbeid, zie het artikel [ Begonnen de Kosten van de Arbeid en Begrotingspunten voor projecten ](../../../manage-work/projects/project-finances/budgeted-labor-cost.md) begrijpen.

* De **Begroeide Kosten van Uitgaven** in de berekening hierboven is de Geplande Kosten verbonden aan de kosten op het project, aangezien zij op het gebied van Uitgaven van het BedrijfsGeval of het lusje van Uitgaven van het project worden berekend.\
  Voor meer informatie over Uitgaven op een project, zie het artikel [ projectuitgaven ](../../../manage-work/projects/project-finances/manage-project-expenses.md) beheren.

* **Vaste Kosten** in de berekening hierboven is het vaste bedrag verbonden aan de Kosten van het project, zoals die in het gebied van Financiën van de sectie van Details van het project wordt bepaald.\
  Voor meer informatie over sub-lusje van Financiën van een project, zie het artikel [ informatie in het gebied van de Projectfinanciering beheren ](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>Workfront berekent alle kosteninformatie met behulp van de valuta van het project. Als u de Beoogde Uren voor uw middelen in de Planner van het Middel specificeert, wordt de optie om projectvaluta te veranderen gehandicapt.
>
>Voor meer informatie over het veranderen van de munt van een project, zie het artikel [ Verandering de projectmunt ](../../../manage-work/projects/project-finances/change-project-currency.md).

## De begrote kosten van een project zoeken

De begrote Kosten zoals weerspiegeld in het gebied van de Begroting van het Middel van het BedrijfsGeval of de Planner van het Middel toont op de volgende gebieden van Workfront onder de volgende namen:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Weergavenaam van begrote kosten</strong></td> 
     <td><strong>Gebied van Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Geraamde kosten</td> 
     <td> <p>Overzicht van bedrijfscase</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>Kosten</td> 
     <td> <p>Portfolio optimaliseren</p> <p>Tip: Het totaal van alle begrote kosten voor het project is de begrote kosten van de portefeuille.</p> </td> 
    </tr> 
    <tr> 
     <td>Geraamde projectkosten</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>Projectrapport</p> <p>Project (Financial Data)-rapport</p> <p>Taakrapport</p> <p>Probleemrapport</p> <p>Rapport over Budgeted Hour</p> <p>Voor meer informatie over het creëren van een rapport, zie het artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref"> een douanerapport </a> creëren.</p> </td> 
    </tr> 
   </tbody> 
  </table>
