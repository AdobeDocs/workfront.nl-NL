---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Werkelijke uren weergeven
description: De uren die u in Adobe Workfront inlogt op uw werkitems worden beschouwd als Werkelijke uren. Werkelijke uren geven de werkelijke tijd aan waarin u een taak, uitgave of project hebt voltooid.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: 957c6e6955a828aa40ac996490d66e9c46f594bc
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 0%

---

# Werkelijke uren weergeven

<!-- Audited: 5/2025 -->

De uren die u in Adobe Workfront inlogt op uw werkitems worden beschouwd als Werkelijke uren.

Werkelijke uren geven de werkelijke tijd aan waarin u een taak, uitgave of project hebt voltooid.

Wij adviseren dat de uren op het werkpunten zouden moeten worden geregistreerd, die taken en kwesties zijn. Als Workfront-beheerder kunt u gebruikers echter toestaan zich ook aan te melden bij projecten, afhankelijk van de workflows van uw organisatie.

Voor meer informatie over hoe te opstelling uw systeem om gebruikers toe te staan om tijd op projecten te registreren, zie [ timesheet en uurvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md) vormen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> 
   <p>Nieuw: Standaard<p>
   <p>of</p>
   <p>Huidig: Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>De mening of hogere toegang tot Taken, Projecten, of Kwesties</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Bekijk of hogere toestemmingen aan een taak, een project, of een kwestie</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Werkelijke uren vs verouderde werkelijke uren

Afhankelijk van welk gebied van Workfront u tot de daadwerkelijke uren van toegang hebt, konden zij naar één van de volgende geregistreerde uren verwijzen:

* In project, de taken, en geven rapporten en lijsten uit:

   * **Ware Uren**: Uren die voor project, taken, of kwesties na Mei 2021 worden geregistreerd. Ze worden in uren opgeslagen in de Workfront-database en hun waardeveld is `actualWorkRequiredDouble` .
   * **Verouderde Werkelijke Uren**: Uren die voor projecten, taken, of kwesties worden geregistreerd om het even welke tijd, met inbegrip van vóór Mei 2021. Ze worden in de Workfront-database opgeslagen als minuten en hun waardeveld is `actualWorkRequired` . <!--check below and see if you need to add this to the API section - asked on the tech doc task -->

* In het project, de taak, of het gebied van de Details van de kwestie:

   * **Ware Uren**: Uren die voor projecten, taken, of kwesties vóór Mei 2021 worden geregistreerd. Ze worden in uren opgeslagen in de Workfront-database en hun waardeveld is `actualWorkRequiredDouble` .

## Werkelijke uren voor taken en problemen versus Werkelijke uren voor projecten

De Werkelijke Uren op taken en kwesties vertegenwoordigen het aantal uren die rechtstreeks op de taken en de kwesties worden geregistreerd.

Werkelijke uren van onderliggende taken lopen door tot de werkelijke uren van de bovenliggende taak. De volgende formule is van toepassing voor de Werkelijke Uren op een oudertaak:

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

Werkelijke uren voor Projecten vertegenwoordigen een totaal van Werkelijke Uren van alle taken van het project (met inbegrip van uren die direct op oudertaken worden geregistreerd), alle kwesties van het project, en de Werkelijke Uren die op het project zelf het programma worden geopend.

De volgende formule is van toepassing voor de Werkelijke Uren op een project:

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## Werkelijke uren zoeken

Het vinden van de waarde voor Werkelijke Uren voor een punt is identiek voor taken, projecten, en kwesties.

### Werkelijke uren in de sectie Details {#actual-hours-in-the-details-section}

Werkelijke uren zoeken in de sectie Details is identiek voor projecten, taken en problemen.

Werkelijke uren zoeken in taakdetails:

1. Ga naar een taak u de Ware Uren voor wilt herzien.
1. In het linkerpaneel, klik **Details van de Taak**. De **vertoningen van de 1} sectie van het Overzicht {.**
1. Bepaal de plaats van de **Ware 1} waarde van Uren {in de** 3} sectie van de Werktijd. **** Dit is het totaal aantal uren dat op deze taak is aangemeld.

### Werkelijke uren in de sectie Uren {#actual-hours-in-the-hours-section}

Het vinden van Werkelijke Uren in de sectie van Uren is identiek voor projecten, taken, en kwesties.

Werkelijke uren zoeken in de sectie Uren:

1. Ga naar een taak u de Ware Uren voor wilt herzien.

1. In het linkerpaneel, klik **Uren**. Een lijst van uuringangen die op de taakvertoningen worden geregistreerd, met de **1} kolom die van Uren {het totale aantal Werkelijke Uren voor de taak tonen.**

1. Zorg ervoor dat de **Standaard** mening en de **groepering van het Project** op deze lijst worden toegepast.

### Werkelijke uren in rapporten {#actual-hours-in-reports}

Wanneer het bouwen van taken, kwesties, of projectrapporten, kunt u de Werkelijke waarde van Uren voor elke taak, kwestie, of project in het rapport tonen.

Werkelijke uren weergeven in een taakrapport:

{{step1-to-reports}}

1. Op de **pagina van Rapporten**, klik **Nieuw Rapport**, dan kies **Taak** als uw voorwerp.
1. In de bodem-juiste hoek van de pagina, klik **voegt Kolom** toe.
1. In **toon in deze kolom** drop-down gebied dat verschijnt, begin **Werkelijke Uren** te typen, dan het gebied te selecteren wanneer het in de lijst verschijnt.

1. In de bodem-linkerhoek van de pagina, klik **sparen + Sluiten** om het rapport te bewaren.

1. In de **Naam dit Rapport om het** dialoogvakje te bewaren, ga een nieuwe rapportnaam in, dan klik **** van toepassing zijn.

### Werkelijke uren aan hulpmiddelen voor bronnenbeheer {#actual-hours-in-resource-management-tools}

Als u de vooruitgang wilt zien van het werk uw gebruikers aan hun toegewezen taken en kwesties doen, kunt u hen in de volgende hulpmiddelen van het Beheer van het Middel bekijken:

* Het gebruiksrapport.\
  Voor informatie, zie [ Overzicht van het rapport van het Gebruik van het Middel ](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* De bronnenplanner.

  Voor informatie, zie [ Beschikbare Mening, Geplant, en Ware Uren of VTE in de Planner van het Middel wanneer het gebruiken van de mening van de Gebruiker ](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).


### Werkelijke uren in de Workfront API

<!--this section was added as a result to this issue: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/6810910e0001b932e0948336208e76f2/overview-->

De meeste Workfront-velden waarin uren worden opgeslagen, worden in minuten opgeslagen in de Workfront-database. De naam van het veld Geplande uren van een taak is bijvoorbeeld `workRequired` in de Workfront-database en wordt in minuten opgeslagen.

U moet de conversie van minuten naar uren uitvoeren wanneer u deze velden opent in API-aanroepen of in berekende aangepaste velden of kolommen.

De Werkelijke uren die voor projecten, taken, of kwesties worden geregistreerd worden momenteel opgeslagen in het gegevensbestand van Workfront als notulen en hun waardegebied is `actualWorkRequired`.

Met de volgende versie van de Workfront API die later in 2025 wordt uitgebracht, worden de Werkelijke uren opgeslagen in de volgende velden en eenheden in de database:

* **Ware Uren**: Uren die voor project, taken, of kwesties na Mei 2021 worden geregistreerd. Ze worden in uren opgeslagen in de Workfront-database en hun waardeveld is `actualWorkRequiredDouble` .
   * **Verouderde Werkelijke Uren**: Uren die voor projecten, taken, of kwesties worden geregistreerd om het even welke tijd, met inbegrip van vóór Mei 2021. Ze worden in de Workfront-database opgeslagen als minuten en hun waardeveld is `actualWorkRequired` .

Voor informatie over het gebruiken van Werkelijke Uren in berekende kolommen of gebieden, zie [ FAQs van het Rapport ](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

## Logtijd

U kunt tijd op taken, kwesties, en projecten op veelvoudige manieren registreren.

Voor meer informatie, zie [ tijd van het Logboek ](../../../timesheets/create-and-manage-timesheets/log-time.md).
