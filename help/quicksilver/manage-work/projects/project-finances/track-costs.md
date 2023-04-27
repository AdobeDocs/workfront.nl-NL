---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: Trackkosten
description: U kunt de kosten voor projecten, taken en problemen in Adobe Workfront bijhouden.
author: Alina
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: 7e78ca8c8ea7f037b55b06e7452ac5c562b99eca
workflow-type: tm+mt
source-wordcount: '2418'
ht-degree: 0%

---

# Trackkosten

U kunt de kosten voor projecten, taken en problemen in Adobe Workfront bijhouden.

## Hoe Workfront kosten berekent

Om kosten te volgen, moet u gebruikers en baanrollen met uurkostentarieven associëren.

De kostencijfers van de uren zijn bedragen van kosten per het werkeenheid verbonden aan baanrollen of gebruikers. Door de tarieven te vermenigvuldigen met de uren die aan het werk worden besteed, worden kosten voor uw projecten, taken of problemen gegenereerd.

De volgende scenario&#39;s bestaan:

* Als het Type van Kosten van uw taken Uur van de Gebruiker is, berekent het tarief van het gebruikersuur de taak en projectkosten.

   Voor informatie over het associëren van gebruikers met kostentarieven, zie [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Als het Type van Kosten van uw taken de Uur van de Rol is, berekent de baan het uurtarief van de rol de taak en projectkosten.

   Voor informatie over het associëren van baanrollen met kostentarieven, zie [Taakrollen maken en beheren](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront berekent alleen de werkelijke kosten voor uitgaven en uitgaven hebben geen Type kosten. Zie de sectie voor meer informatie [Hoe Workfront de kosten voor problemen traceert](#how-workfront-tracks-costs-for-issues) in dit artikel.

>[!TIP]
>
>U kunt kostentarieven voor projecten niet overschrijven. Zodra u de kosten per uurtarief op een gebruiker of baanrol bepaalt, berekent dat tarief alle kosten in het systeem.

## Workfront-kostenprestatie-indexen

Workfront berekent een aantal kostenprestatiesindexen voor projecten zodat kunnen de projecten voor kostenefficiency worden gevolgd.\
Voor meer informatie over het berekenen van kosten-prestatiesindexen, zie:

* [Kostenprestatie-index (CPI) berekenen](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [Prestatie-index (CSI) voor kostenplanning berekenen](../../../manage-work/projects/project-finances/calculate-csi.md)
* [Prestatie-index (SPI) voor planning berekenen](../../../manage-work/projects/project-finances/calculate-spi.md)

## Hoe Workfront de kosten voor taken en projecten traceert

* [Hoe Workfront kosten traceert](#how-workfront-tracks-costs)
* [Hoe Workfront geplande, begrote en werkelijke kosten berekent](#how-workfront-calculates-planned-budgeted-and-actual-costs)
* [Hoe Workfront kostentypen berekent voor taken](#how-workfront-calculates-cost-types-for-tasks)

### Hoe Workfront kosten traceert  {#how-workfront-tracks-costs}

U kunt verschillende typen kosten bijhouden voor taken en projecten in Workfront. De totale kosten worden berekend aan de hand van de volgende formule:

```
Costs = Labor Costs + Expense Costs
```

* **Arbeidskosten** worden geassocieerd met de uren op taken en projecten en de Kosten per uur van de middelen verbonden aan taken. In het algemeen berekent Workfront de volgende arbeidskosten:

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Geplande loonkosten</td> 
     <td> <p>Zij worden berekend met behulp van de volgende formule:</p><pre>Geplande loonkosten = geplande uren * Kosten per uur</pre> </td> 
    </tr> 
    <tr> 
     <td>begrote loonkosten</td> 
     <td> <p>Zij worden berekend met behulp van de volgende formule:</p><pre>Voorziene arbeidskosten = begrote uren uren * Kosten per uur</pre> </td> 
    </tr> 
    <tr> 
     <td>Werkelijke loonkosten</td> 
     <td> <p>Zij worden berekend met behulp van de volgende formule:</p><pre>Werkelijke loonkosten = Werkelijke uren * Kosten per uur</pre> </td> 
    </tr> 
   </tbody> 
  </table>

   Zie voor meer informatie de [Hoe Workfront geplande, begrote en werkelijke kosten berekent](#how-workfront-calculates-planned-budgeted-and-actual-costs) in dit artikel.

* **Kosten** worden geassocieerd met uitgaven voor projecten en taken.\
   Wanneer u een project creeert, kunt u geplande uitgaven voor het volledige project plaatsen. Daarnaast kunt u uitgaven koppelen aan nieuwe of bestaande taken. Zie voor meer informatie [Projectkosten beheren](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **Vaste kosten** worden gedefinieerd als een vast bedrag aan kosten voor een project. Dit maakt deel uit van de geplande kosten van het project dat het bedrag vertegenwoordigt dat u nodig hebt om het project te voltooien.

   >[!TIP]
   >
   >Wanneer het vastmaken van een malplaatje aan een project, worden de Vaste Kosten van een malplaatje toegevoegd aan Vaste Kosten van het project. Zie voor meer informatie [Overzicht van het koppelen van een sjabloon aan een project](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### Hoe Workfront geplande, begrote en werkelijke kosten berekent {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront berekent de geplande kosten en de werkelijke kosten voor elke afzonderlijke taak in een project. Workfront gebruikt deze berekeningen voor individuele taken om de geplande kosten en de werkelijke kosten voor het project te berekenen.

* [Geplande kosten](#planned-cost)
* [Geraamde kosten](#budgeted-cost)
* [Werkelijke kosten](#actual-cost)

#### Geplande kosten {#planned-cost}

De geplande kosten van een project zijn de kosten van de geplande werkzaamheden (geplande uren) voor het project.

De geplande kosten van een project worden berekend aan de hand van de volgende formule:

```
Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project
```

U hebt bijvoorbeeld de volgende uitgaven op het tabblad Uitgaven van een taak: een marketinguitgave van $100 en een administratieve uitgave van $50. In het lusje van Financiën, selecteert u het de kostentype van de Uur van de Gebruiker. Een gebruiker wordt toegewezen aan de taak, en het uurtarief van de gebruiker is $15. De gebruiker wordt toegewezen om 5 uur aan deze taak te werken. Op het lusje van Uitgaven van het project, hebt u $100 Geplande Kosten voor een uitgave genoemd het Raadplegen. U hebt ook vaste kosten van $200 voor het project.

De geplande kosten van het project worden als volgt berekend:

```
$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525
```

#### Geraamde kosten {#budgeted-cost}

De begrote kosten van een project zijn de kosten in verband met de begrote werkzaamheden (begrotingsuren) voor het project.

De begrote kosten van het project zijn gelijk aan de geplande kosten van het project indien aan de volgende twee voorwaarden is voldaan:

* De geplande uren van de taken op het project passen de begrote Uren (in de Planner van het Middel) aan
* Het type van de taakfacturering is Rol Uur.

De begrote kosten van het project worden berekend aan de hand van de onderstaande formule indien aan de volgende voorwaarden is voldaan:

* De geplande uren van de taken voor het project komen niet overeen met de begrote uren uren (in het bronnenplan)
* Het facturatietype van de taken is Role Hourly.

Wanneer aan bovenstaande voorwaarden is voldaan, berekent Workfront de begrote kosten van het project aan de hand van de volgende formule:
<pre>Beoogde projectkosten = begrote arbeidskosten + begrote kosten van alle taken + begrote kosten van de uitgaven van het project</pre>

#### Werkelijke kosten {#actual-cost}

De Ware Kosten van een project zijn de kosten verbonden aan het daadwerkelijke werk (uren die) op het project worden geregistreerd.

De werkelijke kosten worden berekend aan de hand van de volgende formule:

```
Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project
```

U hebt bijvoorbeeld de volgende uitgaven op het tabblad Uitgaven van een taak: een marketinguitgave met een werkelijke kostprijs van $110 en een administratieve uitgave met een werkelijke kostprijs van $40. U selecteert het kostentype Rol Uourly en wijst de de baanrol van de Consultant aan de taak toe. Het tarief van de de baanrol van de consultant is $15 per uur, en er zijn 6 uren het programma geopend op de taak voor de Consultant baanrol. Er is een het Raadplegend uitgave verbonden aan het project (op het lusje van Uitgaven), met een Ware Kosten van $100 en een gebruiker met een Kosten per Uur tarief van $20 in hun gebruikersprofiel registreert 10 uren op het project. U hebt ook vaste kosten van $200 voor het project.

De werkelijke kosten van het project worden als volgt berekend:

```
$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740
```

>[!NOTE]
>
>De werkelijke kosten van het project worden als volgt berekend:
>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>Deze kosten worden niet gedupliceerd in de berekening van de werkelijke kosten. Als bijvoorbeeld een vaste kostprijs deel uitmaakt van de werkelijke kosten van het project, wordt deze niet afzonderlijk toegevoegd aan de werkelijke kosten.

>[!NOTE]
>
>Wanneer het registreren van tijd op een project, bestaan de volgende scenario&#39;s wanneer het berekenen van de Ware Kosten van de Arbeid voor het project:
>
>* Standaard gebruikt Workfront de kosten per uur van de gebruiker om de werkelijke loonkosten te berekenen.
>* Als de gebruiker die de tijd registreert niet met om het even welke kosten wordt geassocieerd, dan gebruikt Workfront de Kosten per Uur tarief van de Primaire Rol van de gebruiker.
>* Als uw Workfront-beheerder het **Taken handmatig toewijzen aan uurwaarden** het plaatsen in het gebied van de Voorkeur van Timesheets &amp; van Uren, en de gebruiker het registreren tijd op het project selecteert een verschillende rol om met deze tijd te associëren, berekent de Ware Kosten van het project gebaseerd op de rol die werd gespecificeerd toen de uren werden geregistreerd. Zie het artikel voor informatie over het inschakelen van logboektijd voor een specifieke taakrol [Voorkeuren voor tijdpagina&#39;s en uren configureren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).


### Hoe Workfront kostentypen berekent voor taken {#how-workfront-calculates-cost-types-for-tasks}

De geplande en werkelijke kosten van de taken en hun arbeidskosten worden bepaald door het soort kosten van elke taak.

U kunt het Type van Kosten voor individuele taken binnen het project vormen. Elk kostentype beïnvloedt de Geplande Kosten en de Ware Waarden van Kosten.

Voor informatie over hoe te om het Type van Kosten van een taak te wijzigen, zie [Type kosten taak bijwerken](../../../manage-work/tasks/task-information/update-task-cost-type.md).

In de volgende tabel worden de beschikbare typen taakkosten in Workfront beschreven:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Type taakkosten</strong> </p> </th> 
   <th> <p><strong>Beschrijving</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Uur gebruiker</p> </td> 
   <td> <p>Dit is het standaardtype van Kosten wanneer u een taak creeert.</p> <p><strong>Geplande kosten</strong> wordt berekend met de volgende formule: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Wanneer de geraamde loonkosten worden berekend door:<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>Opmerking:   <p>Houd rekening met de volgende effecten van het gebruik van het kostentype Uurtijd van de gebruiker en het berekenen van de geplande kosten:</p> 
     <ul> 
      <li>Als u veelvoudige middelen aan een taak toewijst, past Workfront berekeningen voor Geplande Kosten aan op basis van het percentage van de taak die aan elk middel wordt toegewezen.</li> 
      <li>De waarde van het Geplande gebied van Kosten kan verschillen afhankelijk van of u de Geplande Kosten van de taak zelf of van het rapport van het Gebruik bekijkt.<br><strong>Wanneer het bekijken Geplande Kosten van de taak zelf:</strong> In het veld Geplande kosten wordt rekening gehouden met het veld Kosten/uur dat is ingesteld op taakrolniveau (wanneer het veld Kosten/uur niet op gebruikersniveau is ingesteld).<br><strong>Wanneer het bekijken Geplande Kosten van het rapport van het Gebruik over het project:</strong> In het veld Geplande kosten wordt geen rekening gehouden met het veld Kosten/uur dat op taakrolniveau is ingesteld. In plaats daarvan, als u het rapport van het Gebruik om rekening te houden met het Kosten/Hr- gebied dat op het niveau van de Rol van de Baan wordt geplaatst, moet u het Type van Kosten op de taak plaatsen aan Rol. </li> 
     </ul> </p> <p><strong>Werkelijke kosten</strong> wordt berekend met de volgende formule: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Wanneer de werkelijke loonkosten worden berekend door:</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>Een gebruiker heeft bijvoorbeeld een kosten per uur van $20 in zijn profiel. Wanneer zij 5 uren voor een taak registreren, is de Ware Kosten van de Arbeid $100 voor die taak. Als de gebruiker geen Kosten per uur aan hen wordt geassocieerd, berekent de Ware Kosten gebaseerd op de Kosten per uur van hun Primaire Rol van de Baan. Als zij geen baan hebben of het Kosten per Uur tarief van hun baanrol niet wordt bepaald, dan is de Ware Kosten van de taak nul. </p> <p>Opmerking: De daadwerkelijke kosten worden berekend gebaseerd op de Kosten per het tarief van het Uur voor de gebruiker die de tijd registreert, ongeacht wie aan de taak wordt toegewezen. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Rol Uur</p> </td> 
   <td> <p><strong>Geplande kosten</strong> wordt berekend met de volgende formule: </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>Wanneer de geplande loonkosten voor de taak worden berekend door:</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Opmerking: Als u veelvoudige middelen aan een taak toewijst, past Workfront berekeningen voor Geplande Uren aan die op het percentage van de taak worden gebaseerd aan elk middel wordt toegewezen.</p> <p><strong>Werkelijke kosten</strong> wordt berekend met de volgende formule: </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>Wanneer de werkelijke loonkosten van de taak worden berekend door:</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>Bijvoorbeeld, wordt een taak toegewezen aan een baanrol of een gebruiker met een baanrol waarvoor het Tarief van de Kosten per Uur $20 is. Wanneer een gebruiker 5 uur voor een taak registreert, is de Ware Kosten van de Arbeid $100 voor die taak. Als de gebruiker aan de taak wordt toegewezen geen baanrol verbonden aan hen op de taak heeft, berekent de Ware Kosten gebaseerd op de Kosten per uur van hun Primaire Rol van de Baan. Als zij geen baan hebben of het Kosten per Uur tarief van hun baanrol niet wordt bepaald, dan is de Ware Kosten van de taak nul. </p> <p>Opmerking:   <p> De Werkelijke Uren van een Taak van de Uur van de Rol berekenen gebaseerd op de baanrollen van de gebruikers verbonden aan de taak, niet op de rollen verbonden aan de gebruiker die de tijd registreert.</p> <p>Als uw Workfront-beheerder het <strong>Taken handmatig toewijzen aan uurwaarden</strong> het plaatsen in het gebied van de Voorkeur van Timesheets &amp; van Uren, en de gebruiker het registreren tijd op de taak selecteert een verschillende rol om met deze tijd te associëren, berekent de Ware Kosten van een taak van de Rol Uur gebaseerd op de rol die werd gespecificeerd toen de uren werden geregistreerd. Zie het artikel voor informatie over het inschakelen van logboektijd voor een specifieke taakrol <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Voorkeuren voor tijdpagina's en uren configureren</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Vaste uren</p> </td> 
   <td> <p><strong>Geplande kosten</strong> wordt berekend met de volgende formule:</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>Wanneer de kosten van de taakarbeid worden berekend door:</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>Werkelijke kosten</strong> wordt berekend met de volgende formule: </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>Wanneer de werkelijke loonkosten van de taak worden berekend door:</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>Dit kostentype houdt geen rekening met individuele gebruikers of baanrollen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Geen kosten</p> </td> 
   <td> <p>Dit type kosten heeft geen invloed op de kosten. Als een oudertaak dit Type van Kosten heeft, berekenen de subtaken met een ander Type van Kosten volgens hun individuele Types van Kosten, en de Kosten van de oudertaak wordt dienovereenkomstig beïnvloed. </p> <p>Wanneer een gebruiker zonder Toegang tot Financiële Gegevens of een gebruiker zonder financiële toestemmingen op een malplaatje een project van dat malplaatje leidt, is dit het standaardType van Kosten voor de taken op het project.</p> <p>Zie het artikel voor informatie over toegang tot financiële gegevens <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Toegang tot financiële gegevens verlenen</a>.</p> <p>Zie het artikel voor informatie over financiële machtigingen voor objecten <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Financiële machtigingen delen op een object</a>.</p> <p>Voor informatie over het creëren van projecten van malplaatjes, zie het artikel <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Een project maken met een sjabloon</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because this was moved to its own how-to article linked above. Could be removed after some time.) </p>
<p>To configure the Cost Type of an individual task:</p>
<ol>
<li value="1">Go to the task where you want to configure the Cost Type. </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then expand the <strong>Finance</strong> area. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Double click <strong>Cost Type</strong> and select the cost type that you want to apply to the task. </p> </li>
<li value="4">Click <strong>Save.</strong></li>
</ol>
</div>
-->

## Hoe Workfront de kosten voor problemen traceert {#how-workfront-tracks-costs-for-issues}

De kwesties hebben en beïnvloeden niet de volgende soorten kosten voor een project:

* Geplande kosten
* Geraamde kosten

Problemen kunnen echter **Werkelijke kosten** die ook van invloed zijn op de werkelijke kosten van het project.

In de volgende tabel wordt aangegeven hoe de werkelijke kosten worden berekend voor emissies, afhankelijk van het type toewijzing voor de uitgifte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th colspan="4">Werkelijke kosten van uitgave</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Gebruikerstoewijzing</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Werkelijke kosten</strong> wordt berekend met de volgende formule:</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>De kosten per uur van de gebruiker die de tijd registreert wordt in dit geval in aanmerking genomen, ongeacht wie aan de kwestie wordt toegewezen. </p> <p>Als de gebruiker die de tijd registreert geen Kosten per uur tarief in hun profiel heeft, berekent de Kosten per uur van hun Primaire Rol van de Baan de Ware Kosten van de kwestie. Als de gebruiker die de tijd registreert geen rol in hun profiel of geen tarief verbonden aan het heeft, worden de Ware Uren berekend gebruikend het Tarief van Kosten per Uur van de Primaire Rol van de Taak van de Primaire Ontvanger op de kwestie. Als voor die rol geen tarief is gedefinieerd, is de werkelijke kostprijs van de uitgave nul. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Roltoewijzing</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Werkelijke kosten</strong> wordt berekend met de volgende formule:</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>De kosten per uur van de gebruiker die de tijd op de kwestie registreert wordt in aanmerking genomen, ongeacht welke rol aan de kwestie wordt toegewezen. </p> <p>Als de gebruiker die de tijd registreert geen Kosten per Uur verbonden aan hen heeft, berekent de Kosten per Uuretarief van hun Primaire Rol de Ware Kosten van de kwestie.<br>Als de gebruiker die de tijd registreert geen rol in hun profiel of geen tarief verbonden aan het heeft, is de Ware Kosten van de kwestie nul. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Geen toewijzing</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>Werkelijke kosten</strong> wordt berekend met de volgende formule:</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>Als de gebruiker die de tijd registreert geen Kosten per uur tarief verbonden aan hun profiel heeft, berekent de Kosten per uur van hun Primaire Rol van de Baan de Ware Kosten van de kwestie. </p> <p>Als de gebruiker die de tijd registreert geen baanrol verbonden aan zijn profiel of hun Primaire Rol van de Baan heeft geen bepaalde Kosten per Uren tarief, is de Ware Kosten van de kwestie nul. </p> </td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td colspan="4"> 
    <div> <MadCap:conditionalText data-mc-conditions="">
       If your Workfront administrator enabled the 
      <strong>Assign Job Roles to hour entries manually</strong> setting in the Timesheets &amp; Hours Preferences area, and the user logging time on the issue selects a different role to associate with this time, the Actual Cost of the issue calculates based on the role specified when the hours were logged. For information about enabling logging time for a specific job role, see the article 
      <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configure timesheet and hour preferences</a>. 
     </MadCap:conditionalText> 
    </div> </td> 
  </tr> 
  -->
 </tbody> 
</table>
