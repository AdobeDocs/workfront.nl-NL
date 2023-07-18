---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel
description: Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel
author: Alina
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: 3aad2a3d9ad32313cb14670965bc3ad05ab215d3
workflow-type: tm+mt
source-wordcount: '1379'
ht-degree: 0%

---

# Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

U kunt de toewijzing en beschikbaarheid van uw middelen in de Planner van het Middel door Uren, VTE, of Kosten tonen.\
Voor meer informatie over het berekenen van Kosten in de Planner van het Middel, zie [Kosten berekenen in de bronnenplanner](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

&quot;FTE&quot; staat voor voltijdequivalent. Het is een tijdsmeting die de hoeveelheid uren vertegenwoordigt die aan echt werk tijdens een dag of week voor een gebruiker of baanrol wordt gewijd.

De volgende reeksen van middelinformatie worden berekend verschillend in de Planner van het Middel:

* De waarden voor Beschikbare uren of FTE worden berekend op basis van de manier waarop de systeembeheerder de voorkeuren voor Bronbeheer in uw systeem configureert.\
  Voor meer informatie over hoe de Beschikbare Uren en FTE waarden worden berekend, zie [Beschikbare uren of FTE voor gebruikers en baanrollen in de Planner van het Middel berekenen](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner).\
  Voor meer informatie over het bepalen van de voorkeur van het Beheer van Middelen voor het systeem van Adobe Workfront, zie [Voorkeuren voor beheer van bronnen configureren](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* Alle andere FTE-waarden worden berekend op basis van het standaardschema van het systeem.\
  Voor meer informatie over hoe alle andere waarden in de Planner van het Middel wanneer het gebruiken van FTE tonen, zie de sectie [Bereken alle andere uren en FTE waarden voor gebruikers en baanrollen in de Planner van het Middel](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) in dit artikel.

Het is belangrijk om te begrijpen wat FTE voor elk van uw gebruikers en hun baanrollen is om uw middelen nauwkeurig te beheren aangezien u hen aan het werk toewijst.

## Beschikbare uren of FTE voor gebruikers en baanrollen in de Planner van het Middel berekenen {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

* [Bereken de Beschikbare Uren en FTE voor een gebruiker in de Planner van het Middel](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)
* [Bereken de Beschikbare Uren en FTE voor een baanrol in de Planner van het Middel](#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner)
* [Bereken de Beschikbare Uren en FTE voor een gebruiker in de Planner van het Middel (Voorbeeld)](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example)

### Bereken de Beschikbare Uren en FTE voor een gebruiker in de Planner van het Middel {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

De beheerder van Workfront bepaalt hoe de beschikbare tijd voor een gebruiker door te selecteren wordt berekend om één van het volgende op het gebied van het Beheer van het Middel in Opstelling te gebruiken wordt berekend:

* Het standaardschema van het systeem en FTE van de gebruiker.
* Het schema van de gebruiker.

![Systeeminstelling voor gebruikersschema&#39;s](assets/setup-resource-mgmt.png)

>[!NOTE]
>
>Dit bepaalt hoe te om middelbeschikbaarheid op het systeemniveau te berekenen. Voor meer informatie over het bepalen van de voorkeur van het Beheer van het Middel voor het systeem, zie [Voorkeuren voor beheer van bronnen configureren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Gebaseerd op hoe dit het plaatsen wordt gevormd, wordt de beschikbaarheid van de gebruikers in de Planner van het Middel (uren evenals beschikbaarheid FTE) berekend gebruikend de volgende methodes:

* **Het standaardschema**: Het standaardprogramma van het systeem en gebruiker FTE worden gebruikt om de Beschikbare Uren en waarde FTE voor de gebruiker in de Planner van het Middel te bepalen. Het schema van de gebruiker wordt genegeerd. In dit geval:

   * De **Beschikbare uren** in de functie Resourceplanner wordt berekend met behulp van de volgende formule:

     `User Available Hours = Default Schedule Hours * User FTE value`

     Bijvoorbeeld, als het Standaard Programma 40 uren per week beschikbaar voor het werk heeft, en de gebruiker FTE 0.5 is, is de gebruiker beschikbaar om 20 uren per week in de Planner van het Middel te werken.

     Voor meer informatie over programma&#39;s, met inbegrip van het StandaardProgramma, zie [Een schema maken](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * De **Beschikbare FTE** voor de gebruiker in de Planner van het Middel is het zelfde als gebruiker FTE die in de gebruikersmontages wordt gespecificeerd.
Bijvoorbeeld, als de gebruiker FTE 0.5 in de gebruikersmontages is, beschikbaar FTE van de gebruiker is 0.5 in de Planner van het Middel. Voor meer informatie over de waarde van de gebruiker FTE aangezien het in de gebruikersmontages toont, zie [Gebruikersprofiel bewerken](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* **Het schema van de gebruiker**: Het Programma van de gebruiker wordt gebruikt om de beschikbaarheid van de gebruiker in de Planner van het Middel te bepalen. De waarde van de gebruiker FTE wordt genegeerd. In dit geval:

   * De **Beschikbare uren** in de Planner van het Middel is het zelfde als de Uren van het Programma van de gebruiker.

  Bijvoorbeeld, als het Programma van de gebruiker 40 uren per week beschikbaar voor het werk heeft, is de gebruiker beschikbaar om 40 uren per week in de Planner van het Middel te werken.

   * De **Beschikbare FTE** in de Resource Planner wordt berekend aan de hand van de volgende formule:

  `User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours`

  Bijvoorbeeld, als het Programma van de gebruiker 20 uren beschikbaar heeft om te werken, en het Standaard Plan in Workfront 40 uren beschikbaar heeft om te werken, FTE van de gebruiker is 0.5.

  Voor meer informatie over programma&#39;s, met inbegrip van het StandaardProgramma, zie [Een schema maken](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

>[!NOTE]
>
>Als de gebruiker niet aan een programma wordt geassocieerd, worden de Beschikbare Uren voor de gebruiker berekend gebruikend het StandaardProgramma.

### Bereken de Beschikbare Uren en FTE voor een baanrol in de Planner van het Middel {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

U moet eerst de gebruikersbeschikbaarheid berekenen, en dan kunt u de beschikbaarheid van elk van hun baanrollen berekenen.

De beschikbaarheid van taakrollen in de functie voor middelenplanning houdt rekening met de totale beschikbaarheid van de gebruiker en met de **Percentage van de beschikbaarheid van VTE** gekoppeld aan elke rol van de gebruiker.\
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

Voor meer informatie over het associëren van a **Percentage van de beschikbaarheid van VTE** waarde met een taakrol voor een gebruiker, zie [Gebruikersprofiel bewerken](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Bijvoorbeeld, als de waarde van Beschikbare Uren voor een gebruiker 40 is en zij één Primaire Rol voor 75% van die tijd kunnen vervullen, en één Andere Rol voor 25% van die tijd, toont de Planner van het Middel dat **Beschikbare uren** waarde voor de Primaire Rol voor één week is 30 uur, en dat **Beschikbare uren** waarde voor de Andere Rol is 10 uren. In dit geval is de VTE voor de primaire rol 0,75 en de VTE voor de andere rol 0,25.

>[!NOTE]
>
>De totale beschikbare tijd voor de gebruiker wordt berekend op basis van een van de twee methoden die in het dialoogvenster [Bereken de Beschikbare Uren en FTE voor een gebruiker in de Planner van het Middel](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner) in dit artikel.

Wanneer het bekijken van de Planner van het Middel in de Mening van de Rol, is de beschikbaarheid van één baanrol een totaal van de beschikbaarheid van alle gebruikers die die baanrol kunnen vervullen.\
Voor meer informatie over beschikbaarheid van middelen in de Planner van het Middel, zie [Overzicht van de bronnenplanner](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Bereken de Beschikbare Uren en FTE voor een gebruiker in de Planner van het Middel (Voorbeeld) {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

De volgende lijst illustreert hoe de Beschikbare Uren en Beschikbare FTE voor de gebruiker in de Planner van het Middel worden berekend, afhankelijk van welke methode door de systeembeheerder voor de FTE berekening in de Voorkeur van het Beheer van het Middel wordt gebruikt.

In dit voorbeeld gebruiken we de volgende getallen:

* Een standaardschema voor het systeem van 40 uur
* Een gebruikersschema van 20 uur
* Een FTE van 0,75 voor gebruikers

| Methode voor FTE-berekening (systeeminstelling) | **Uren van planning van gebruiker** | **Uren van het standaardschema** | **FTE-veld gebruiker** | **Beschikbare uren in de bronnenplanner** | **Beschikbare VTE in de Planner van het Middel** |
|---|---|---|---|---|---|
| **Het standaardschema** | Genegeerd | 40 | 0.8 | **32** (berekend) | **0.8** |
| **Het schema van de gebruiker** | 20 | 40 | Genegeerd | **20** | **0,5** (berekend) |

De uitzonderingen van het programma en de onderbreking zouden de hoeveelheid Geplande Uren of VTE kunnen beïnvloeden. Zie voor meer informatie [Voorkeuren voor beheer van bronnen configureren](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Voorbeeldweergave van de functie Bronnen per gebruiker en aantal uren:

![Weergave Bronnen per gebruiker en per uur](assets/resource-planner-by-user-by-hours.png)

Voorbeeldweergave van bronnenplanner op gebruiker en FTE:

![Weergave Resourceplanner op gebruiker en FTE](assets/resource-planner-by-user-by-fte.png)

## Bereken alle andere uren en FTE waarden voor gebruikers en baanrollen in de Planner van het Middel {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

Naast Beschikbare Uren of FTE, wordt de volgende tijdinformatie ook getoond in de Planner van het Middel:

* Geplande uren
* Geforceerde uren
* Uurvariatie
* Nettouren\
  Zie voor meer informatie over deze waarden [Overzicht van uren, FTE, en kosteninformatie in de mening van het Project en van de Rol van de Planner van het Middel](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

* Uurverschil\
  Zie voor meer informatie over wat deze waarde vertegenwoordigt [Overzicht van uren, FTE, en kosteninformatie in de mening van het Project en van de Rol van de Planner van het Middel](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

U kunt de zelfde informatie in de Planner van het Middel zoals VTE of als uren tonen.

Workfront gebruikt de volgende formule om alle andere waarden als FTE in de Planner van het Middel te tonen:

`FTE = Resource Planner Hours/ Default Schedule Hours`

>[!NOTE]
>
>Het schema van de gebruiker wordt genegeerd wanneer het berekenen van FTE voor alle waarden behalve Beschikbare (AVL) waarden FTE, in de Planner van het Middel. Alleen het standaardschema wordt in aanmerking genomen voor de berekening.

Deze berekening geldt voor de volgende waarden:

* Geplande VTE (PLN)
* FTE (BDG)
* FTE-variantie (VAR)
* NETTO FTE
* FTE-verschil (DIF)
