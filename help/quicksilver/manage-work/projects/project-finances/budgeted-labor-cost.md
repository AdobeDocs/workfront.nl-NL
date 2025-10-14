---
content-type: reference
product-area: projects
navigation-topic: financials
title: Begrijpte arbeidskosten en begrotingsuren voor projecten begrijpen
description: Begrijpte arbeidskosten en begrotingsuren voor projecten begrijpen
author: Lisa
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '1140'
ht-degree: 0%

---

# Begrijpte arbeidskosten en begrotingsuren voor projecten begrijpen

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

Met de Adobe Workfront Resource Planner kunt u uw middelen begroten voor werk.

Terwijl u uw middelen begroot voor projecten, berekent Workfront de begrote loonkosten voor de rollen, projecten en gebruikers op basis van kosten per uur.

De begrote arbeidskosten van een project in het kader van de planning van het Middel is een berekening tussen de kosten verbonden aan de baanrollen die worden toegewezen om het werk aan het project te voltooien en de geschatte hoeveelheid uren (het Voorgenomen Uren van de Planner van het Middel) die elke rol zouden kunnen nemen om het werk te voltooien.

>[!IMPORTANT]
>
>De begrote loonkosten voor gebruikers in het bronnenplan zijn niet van invloed op die van het project. Alleen de loonkosten voor functies beïnvloeden de kosten van het project.

## Overzicht van de begrote loonkosten voor de rol van de baan en het project

Workfront maakt gebruik van de begrote loonkosten van de functies van het project om de begrote arbeidskosten van het project te berekenen.

>[!TIP]
>
>De begrote Arbeidskosten van een project in het BedrijfsGeval toont als Voorgenomen Kosten van de Arbeid van het Plan van het Middel in rapporten en lijsten.

De **Begrotende Kosten van de Arbeid** (of de Voorgenomen Kosten van de Arbeid van de Planner van het Middel) van een project wordt berekend door de volgende formule:

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

De velden die in bovenstaande berekening worden gebruikt, hebben betrekking op het volgende:

* De in de begroting opgenomen uren voor taakrollen in het gebied van de Begroting van het Middel van het project of de Planner van het Middel.

  Voor meer informatie over het in de begroting opnemen van middelen in de Planner van het Middel, zie de &quot;Begrotende Middelen in de sectie van de Planner van het Middel in het artikel [&#x200B; overzicht van de Planner van het Middel &#x200B;](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

  Voor meer informatie over het in de begroting opnemen van middelen op het gebied van de Begroting van het Middel van het BedrijfsGeval, zie [&#x200B; middelen van de Begroting in het BedrijfsGeval &#x200B;](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

* De **Kosten per tarief van het Uur van een baanrol** in de bovengenoemde berekening verwijst naar de kosten verbonden aan elke baanrol op het project.\
  Voor meer informatie over het creëren van en het leiden van baanrollen en het associëren van hen met de Tarieven van Kosten, zie het artikel [&#x200B; baanrollen &#x200B;](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md) creëren en beheren.

>[!NOTE]
>
>Workfront berekent alle kosteninformatie met behulp van de valuta van het project. Als u de Beoogde Uren voor uw middelen in de Planner van het Middel specificeert, wordt de optie om projectvaluta te veranderen gehandicapt.\
>Voor meer informatie over het veranderen van de munt van een project, zie het artikel [&#x200B; Verandering de projectmunt &#x200B;](../../../manage-work/projects/project-finances/change-project-currency.md).

## Overzicht van de begrote loonkosten voor gebruikers

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>De door de gebruiker begrote loonkosten zijn niet van invloed op de begrote arbeidskosten van het project. Alleen de loonkosten van de functies op een project zijn van invloed op de begrote loonkosten van het project in het bronnenplan.
> 
>Het totaal van alle arbeidskosten van alle gebruikers kan al dan niet gelijk zijn aan de begrote loonkosten van de bronnenplanning van de functies die aan de gebruikers zijn gekoppeld.
>
>Als u begrotingsuren voor gebruikers in de Planner van het Middel schat, zijn de kosten verbonden aan hen die van de baanrollen verbonden aan de gebruikers. Het zijn geen kosten die verband houden met de gebruikers of hun tarieven.

Als de gebruikers met de baanrollen op het project worden geassocieerd en hun uren in de Planner van het Middel worden begroot, tonen hun Begroeide Kosten van de Arbeid door de volgende namen, afhankelijk van waar u hen in Workfront bekijkt:

* [!UICONTROL **Begroeide Arbeidskosten**]: Het gebied van de Begroting van het Middel van het BedrijfsGeval onder hun respectieve rollen.

  ![&#x200B; Begrotende arbeidskosten in BedrijfsGeval &#x200B;](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]: De Planner van het Middel wanneer het bekijken van informatie in de mening van het Project en van de Rol door Kosten.

  ![&#x200B; Begroeide arbeidskosten in de Plaatsen van het Middel &#x200B;](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

De gebruikers tonen in het gebied van de Begroting van het Middel van het BedrijfsGeval onder hun respectieve rollen of in de Planner van het Middel als zij aan de volgende vereisten voldoen:

* Zij worden geassocieerd met één van de baanrollen op het project.
* Ze hebben de opgegeven uren begroot in de Resource Planner.
* De kosten per uur zijn gekoppeld aan hun profiel.

  Voor meer informatie over het toevoegen van Kosten per de tarieven van het Uur aan gebruikers, zie het artikel [&#x200B; uitgeven het profiel van een gebruiker &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* De gebruiker maakt deel uit van één van de Pools van het Middel verbonden aan het project.

De begrote loonkosten van een gebruiker worden berekend aan de hand van de volgende formule:

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## Zoek de begrote arbeidskosten van een project

De begrote arbeidskosten zoals die in het gebied van de Begroting van het Middel van het BedrijfsGeval of de Planner van het Middel in de volgende gebieden van Workfront onder de volgende namen worden weerspiegeld:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Weergavenaam budgettaire arbeidskosten</strong></td> 
     <td><strong>Gebied van Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>begrote arbeidskosten</td> 
     <td>Bronbudgettair gebied van de Business Case</td> 
    </tr> 
    <tr> 
     <td>Geraamde kosten</td> 
     <td><p>Gebruiksrapport Kostenweergave</p><p>Voor meer informatie, zie <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md"> het gebruiksinformatie van de Mening </a>.</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>Project of weergave Rol van bronnenplanner, op kosten</td> 
    </tr> 
    <tr> 
     <td>Projectbegroting van de planning van de middelen</td> 
     <td> <p>Projectrapport</p> <p>Project (Financial Data)-rapport</p> <p>Taakrapport</p> <p>Probleemrapport</p> <p>Rapport over Budgeted Hour</p> <p>Voor informatie over het creëren van een rapport, zie het artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref"> een douanerapport </a> creëren.</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>Als u de Adobe Workfront Scenario Planner gebruikt om projectmiddelen te begroten, zijn de begrote arbeidskosten op het gebied van de begroting van het Middel van het BedrijfsGeval het zelfde als de Kosten van het Mensen van het initiatief verbonden aan het project. De Scenario Planner is alleen beschikbaar in de nieuwe Adobe Workfront-ervaring en vereist een aanvullende licentie. Voor informatie over de Planner van het Scenario van Workfront, zie [&#x200B; het overzicht van de Planner van het Scenario &#x200B;](../../../scenario-planner/scenario-planner-overview.md). Voor informatie over het opnemen van middelen die de Planner van het Scenario gebruiken, zie [&#x200B; middelen van de Begroting in het BedrijfsGeval gebruikend de Planner van het Scenario &#x200B;](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## De begrote uren uren van een project zoeken

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

De begrotingsuren beïnvloeden de waarde van de begrote arbeidskosten (of de begrote kosten van het plan van het Middel) van het project.

De begrote arbeidskosten van een project zijn de kosten die verband houden met de functies die zijn toegewezen om het werk aan het project te voltooien en de geschatte hoeveelheid uren (begrote uren uren) die elke rol zouden kunnen nemen om het werk te voltooien.

U kunt de begrotingsuren in Workfront weergeven in de velden in de onderstaande tabel.

>[!NOTE]
>
>Elke andere vermelding van &quot;Budgeted Hours&quot; in Workfront heeft betrekking op uren die in de begroting zijn opgenomen met vervangen functies die uit Workfront zijn verwijderd. Dit zijn alleen-weergeven velden en werken niet bij met de huidige informatie wanneer u de huidige bronnen in de begroting opneemt.

De in de begroting opgenomen uren op het gebied van de begroting van het Middel van het BedrijfsGeval of de vertoning van de Planner van het Middel op de volgende gebieden van Workfront en onder de volgende namen:

* **Uren**: Het budgetterende gebied van het Middel van het BedrijfsGeval
* **BDG**:De Planner van het middel die door Uren wordt bekeken
* **Begrotende Uren**: De mening van uren van het rapport van het gebruik
Voor informatie, zie [&#x200B; de informatie van het middelgebruik van de Mening &#x200B;](../../../resource-mgmt/resource-utilization/view-utilization-information.md).
* **Bud. Uren**: Het rapport van de Boekte Uur

  Het object Budgeted Hour in het rapport Budgeted Hour verwijst naar informatie met betrekking tot een verouderd hulpmiddel voor middelenbeheer. Alleen de Bud. Het gebied van uren&quot;in dit rapport verwijst naar de uren die in de Planner van het Middel of het gebied van de Begroting van het Middel van het BedrijfsGeval van het project worden begroot.

  Voor meer informatie over het creëren van een rapport, zie het artikel **een douanerapport** creëren.
* **de Planner van het Middel besteedde Uren**: in de volgende rapporten:

   * Projectrapport
   * Project (Financial Data)-rapport
   * Taakrapport
   * Probleemrapport
   * Rapport over Budgeted Hour
