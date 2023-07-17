---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel
description: Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel
author: Alina
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: 4331917d133c52cf727f148b75a213853c1e5679
workflow-type: tm+mt
source-wordcount: '977'
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

Zie voor meer informatie [Voorkeuren voor beheer van bronnen configureren](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><br></p>
<p> <img src="assets/nwe-resource-management-system-setting-user's-schedule-350x157.png" style="width: 350;height: 157;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p>
<p>(NOTE: The determines how to calculate resource availability at the system level.For more information about defining the Resource Management preferences for the system, see Configure Resource Management preferences.)</p>
<p>Based on how this setting is configured, the availability of the users in the Resource Planner (hours as well as FTE availability) is calculated by using the following methods: </p>
<ul>
<li><strong>The Default Schedule</strong>: The Default Schedule of the system and the user FTE are used to determine the Available Hours and FTE value for the user in the Resource Planner. The Schedule of the user is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are calculated using the following formula:<br><code>User Available Hours = Default Schedule Hours * User FTE value</code> <span style="color: #dc143c;">( NOTE: this is the correct value. If this shows as a division in other articles, that is wrong. It's a multiplication between these 2 values).</span><br>For example, if the Default Schedule has 40 hours a week available for work, and the user FTE is 0.5, the user is available to work for 20 hours a week in the Resource Planner.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a></li>
<li style="font-weight: normal;"> The <strong>Available FTE</strong> for the user in the<strong>Resource Planner</strong> is the same as the user FTE specified in the user settings. <br>For example, if the user FTE is 0.5 in the user settings, the available FTE of the user is 0.5 in the Resource Planner. For more information about the value of the user FTE as it displays in the user settings, see <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.<br></li>
</ul></li>
<li><strong>The User's Schedule</strong>: The Schedule of the user is used to determine the availability of the user in the Resource Planner. The value of the user FTE is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are the same as the Hours from the Schedule of the user.<br>For example, if the Schedule of the user has 40 hours a week available for work, the user is available to work for 40 hours a week in the Resource Planner. </li>
<li> The <strong>Available FTE</strong> in the<strong>Resource Planner</strong> is calculated by the following formula:<br><em><code>User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code><br></em>For example, if the Schedule of the user has 20 hours available to work, and the Default Schedule in Workfront has 40 hours available to work, the user's FTE is 0.5.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li>
</ul></li>
</ul> <note type="note">
If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.
</note>
</div>
-->

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
| **Het standaardschema** | Genegeerd | 40 | 0.75 | **30** (berekend) | **0.75** |
| **Het schema van de gebruiker** | 20 | 40 | Genegeerd | **20** | **0,5** (berekend) |

De uitzonderingen van het programma en de onderbreking zouden de hoeveelheid Geplande Uren of VTE kunnen beïnvloeden. Zie voor meer informatie [Voorkeuren voor beheer van bronnen configureren](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

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
