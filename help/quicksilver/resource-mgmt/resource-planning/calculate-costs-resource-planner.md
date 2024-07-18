---
product-area: resource-management
navigation-topic: resource-planning
title: Kosten berekenen in de bronnenplanner
description: U kunt uw middelen in de Planner van het Middel van Adobe Workfront begroten door Kostenwaarden, in plaats van Uren of VTE waarden te gebruiken. Kostenwaarden zijn niet beschikbaar voor de weergave**Weergeven door gebruiker** in de functie Bronnen.
author: Lisa
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '1458'
ht-degree: 0%

---

# Kosten berekenen in de bronnenplanner

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

<!--'(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)'-->

U kunt uw middelen in de Planner van het Middel van Adobe Workfront begroten door Kostenwaarden, in plaats van Uren of VTE waarden te gebruiken. De waarden van kosten zijn niet beschikbaar voor de **Mening door gebruiker** mening in de Planner van het Middel.

>[!IMPORTANT]
>
>U moet gebruikers en baanrollen met de Tarieven van Kosten per Uur associëren om de informatie van Kosten in de Planner van het Middel te tonen.\
>Voor meer informatie over het associëren van de Tarieven van Kosten per Uur met baanrollen, zie [ baanrollen ](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md) creëren en beheren.\
>Voor meer informatie over het associëren van Kosten per de tarieven van het Uur met gebruikers, zie [ het profiel van een gebruiker ](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

Voordat u uw bronnen in een begroting opneemt, moet u goed begrijpen wat er moet gebeuren (geplande uren, VTE of kosten) en op welk moment uw gebruikers kunnen werken (Beschikbare uren, VTE of Kosten).\
Voor meer informatie over het begrip van de informatie in de Planner van het Middel wanneer het opnemen door Uren of FTE, zie [ Overzicht van uren, FTE, en kosteninformatie in de meningen van het Project en van de Rol van de Planner van het Middel ](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Pro en hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot resourcebeheer bewerken, inclusief toegang tot bewerkingsprioriteiten en begrotingstijden in de bronnenplanner</p> <p>Toegang tot financiële gegevens, projecten en gebruikers bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Beheer machtigingen voor de projecten waarvoor u begrotingsgegevens wilt maken met de mogelijkheid om financiën te beheren</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## De informatie van de vertoning in de Planner van het Middel door Kosten

Door gebrek, wordt de beschikbaarheid en toewijzingsinformatie getoond in Uren in de Planner van het Middel.

Om Beschikbare, Geplande, en Gefabriceerde informatie door Kosten in de Planner van het Middel te tonen:

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront.

1. Klik **Middelen**.
1. Ga naar de bronnenplanner.
1. (Voorwaardelijk) selecteer **Mening door Project** of **Mening door Rol**.\
   Door gebrek **Mening door Project** wordt geselecteerd.\
   De informatie over toewijzing en beschikbaarheid wordt weergegeven in uren.

1. Van het **drop-down menu van Uren**, uitgezochte **Kosten**.

   Als u geen toegang tot Financiële Gegevens in uw toegangsniveau hebt, is deze optie niet beschikbaar.\
   Als projecten een andere valuta hebben dan de systeemvaluta, worden de kosten voor deze projecten weergegeven in de bronnenplanner die is omgezet in de valuta van het systeem. De systeembeheerder definieert de systeemvaluta.\
   Voor meer informatie over vestiging de systeemmunt in Workfront en omzettingspercentages, zie [ de Wisselkoersen van de Opstelling ](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).\
   ![ cost_in_the_planner_with_no_budgeting.png ](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## Beschikbare kosten berekenen in de bronnenplanner

Om Beschikbare Kostenwaarden in de Planner van het Middel te tonen moet u het volgende hebben:

* Kosten per uur voor gebruikers en rollen
* Informatie over de beschikbaarheid van gebruikers.

  Het verkrijgen van informatie over de beschikbaarheid van gebruikers hangt af van hoe uw Workfront-beheerder de voorkeuren voor het beheer van bronnen configureert.\
  Voor meer informatie over het berekenen van gebruikersbeschikbaarheid en het plaatsen van de Voorkeur van het Beheer van het Middel, zie [ de voorkeur van het Beheer van het Middel ](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md) vormen.

De volgende lijst illustreert hoe Beschikbare Kosten in de Planner van het Middel wordt berekend:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Beschikbare Kosten </strong> </th> 
   <th><strong> Berekening </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Beschikbare kosten gebruiker</td> 
   <td> <p>De Beschikbare Kosten per gebruiker wordt berekend gebruikend de volgende formule:</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>OPMERKING</b>

Als de gebruiker geen Kosten per Uur in zijn profiel heeft, wordt het Kosten per Uur tarief van de baanrol waaronder zij worden vermeld gebruikt in de berekening. Als de gebruiker geen rol verbonden aan hen heeft, is de Beschikbare Kosten van de Gebruiker $0. </p> </td>
</tr> 
  <tr> 
   <td>Beschikbare kosten voor rollen</td> 
   <td> <p>De Beschikbare Kosten per rol wordt berekend gebruikend de volgende formule:</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>OPMERKING</b>

Als de rol geen Kosten per Uur tarief heeft, is de Beschikbare Kosten van de Rol $0.</p> </td>
</tr> 
  <tr> 
   <td>Beschikbare projectkosten</td> 
   <td> <p>De beschikbare kosten per project worden berekend aan de hand van de volgende formule:</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Geplande kosten berekenen in de bronnenplanner

Hoewel u taakinformatie in de Planner van het Middel niet kunt bekijken, worden de Geplande Kosten voor gebruikers, rollen, en de projecten berekend door met de volgende taakinformatie rekening te houden:

* Het type toewijzing op de taak.\
  U kunt een taak niet toewijzen of de volgende entiteiten aan een taak toewijzen:

   * Een gebruiker (met of zonder taakrol)
   * Een rol
   * Een team\
     Een taak die aan een Team wordt toegewezen wordt beschouwd als niet toegewezen, vanuit het perspectief van de Planner van het Middel.

* Het **Type van Kosten** van de taken op het project.\
  Voor meer informatie over het Type van Kosten van een taak, zie [ Kosten van het Spoor ](../../manage-work/projects/project-finances/track-costs.md).

* De effectieve data van de kostenpercentages voor functies en gebruikers.

  Bijvoorbeeld, als de rol of de gebruiker 10 geplande uren in Februari en 10 geplande uren in Maart heeft, maar het kostentarief is veranderd van $12 in $20 in Maart, is de waarde voor de Geplande Kosten in Februari $120, en in Maart is de Geplande Kosten $200.

>[!NOTE]
>
>Door de gebruiker geplande kosten hebben geen invloed op de geplande projectkosten. Alleen de geplande kosten voor de rol hebben invloed op de geplande kosten van het project in de bronnenplanner.

De volgende scenario&#39;s bestaan wanneer het berekenen van de Geplande Kosten voor gebruikers, rollen, en het project:

* Wanneer het **Type van Kosten** **User Uur **is en er **geen taak** op de taak is:

   * **Rol en gebruiker Geplande Kosten**:

     De door de gebruiker geplande kosten voor Rol en Gebruiker bedragen $0,00.

   * **Geplande Kosten van het Project**:

     De geplande projectkosten bedragen $0,00.

* Wanneer het **Type van Kosten** **Uur van de Gebruiker** is en er a **gebruikerstaak** op de taak is:

   * **Rol en gebruiker Geplande Kosten**:

     De door de gebruiker geplande kosten worden berekend aan de hand van de volgende formule:

     `User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate`

     Als een gebruiker een kostenpercentage in zijn profiel heeft, wordt dat tarief gebruikt om Geplande Kosten te berekenen. Anders worden de kosten op systeemniveau per uur van hun primaire rol gebruikt.

     >[!NOTE]
     >
     >De gebruiker kan aan de taak met één van hun secundaire baanrollen worden toegewezen, maar het tarief van de primaire baanrol wordt hier gebruikt.

     De geplande kosten van de rol wordt berekend met behulp van de volgende formule:

     `Role Planned Cost = SUM(User Planned Cost)`

   * **Geplande Kosten van het Project**:

     De geplande projectkosten bedragen $0,00.

* Wanneer het **Type van Kosten** **Uur van de Gebruiker** is en er is de taak van de a **baanrol** op de taak:

   * **Rol en gebruiker Geplande Kosten**:

     De door de gebruiker geplande kosten bedragen $0,00.

     De geplande kosten van de rol wordt berekend met behulp van de volgende formule:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     De kosten op systeemniveau per uur van de taakrol die aan de taak is toegewezen, worden gebruikt om de geplande kosten te berekenen.

   * **Geplande Kosten van het Project**:

     De geplande projectkosten bedragen $0,00.

* Wanneer het **Type van Kosten** **Huur van de Rol** is en er **geen taak** op de taak is:

   * **Rol en gebruiker Geplande Kosten**:

     De door de gebruiker geplande kosten voor Rol en Gebruiker bedragen $0,00.

   * **Geplande Kosten van het Project**:

     De geplande projectkosten bedragen $0,00.

* Wanneer het **Type van Kosten** **Huur van de Rol** is en er a **gebruikerstaak** op de taak is:

   * **Rol en gebruiker Geplande Kosten**:

     De door de gebruiker geplande kosten bedragen $0,00.

     De geplande kosten van de rol wordt berekend aan de hand van de volgende formule:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront bekijkt de baanrol die de gebruiker op de taak vervult om de Geplande Kosten voor de rol te berekenen.

     Als de gebruiker niet aan om het even welke rol op de taak wordt geassocieerd, is de Geplande Kosten $0.00.

   * **Geplande Kosten van het Project**:

     De geplande projectkosten worden berekend aan de hand van de volgende formule:

     `Project Planned Cost = SUM(Role Planned Costs)`

* Wanneer het **Type van Kosten** **Huur van de Rol** is en er is de taak van de a **rol** op de taak:

   * **Rol en gebruiker Geplande Kosten**:

     De door de gebruiker geplande kosten bedragen $0,00.

     De geplande kosten van de rol wordt berekend aan de hand van de volgende formule:

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront bekijkt de baanrol die de gebruiker op de taak vervult om de Geplande Kosten voor de rol te berekenen.

   * **Geplande Kosten van het Project**:

     De geplande projectkosten worden berekend aan de hand van de volgende formule:

     `Project Planned Cost = SUM(Role Planned Costs)`

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(table below ideal but drafted because it does not display correctly in Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td rowspan="2">&nbsp;</td>
<td colspan="3"> <p><strong>Cost Type = User Hourly</strong> </p><strong>User Planned Cost</strong> </td>
<td colspan="3"> <p><strong>Cost Type = Role Hourly</strong> </p><strong>Role Planned Cost</strong> </td>
</tr>
<tr>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>User and Role Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is calculated using the following formula: </p> <p><code> User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate </code> </p> <p> If a user has a cost rate in their profile, then that rate is used to calculate Planned Cost. Otherwise, the system-level Cost per Hour rate of their Primary Role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code>Role Planned Cost = SUM(User Planned Cost)</code> </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code> Role Planned Cost = Role Planned Hours * Role Cost per Hours </code> </p> <p> The system-level Cost per Hour rate of the job role assigned to the task is used to calculate Planned Cost. </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> If the user is not associated with any role on the task, the Planned Cost is $0.00. </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td rowspan="2"> <p><strong>Project Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td colspan="2"> <p> The Project Planned Cost is calculated using the following formula: </p> <p><code> Project Planned Cost = SUM(Role Planned Costs) </code> </p> <p> </p> </td>
</tr>
<tr>
<td colspan="6"> <note type="note">
User Planned Costs do not influence the Project Planned Cost. Only the Role Planned costs affect the Project Planned Costs, in the Resource Planner.
</note> </td>
</tr>
</tbody>
</table>
-->

## Beoogde kosten berekenen in de bronnenplanner

Om de begrote waarden van Kosten in de Planner van het Middel te tonen moet u het volgende hebben:

* Begrotingsuren voor rollen, gebruikers en projecten.
* Kosten per uur voor gebruikers en rollen.

>[!NOTE]
>
>De begrotingsuren voor de projecten worden berekend op basis van de begrotingsuren voor de rollen, niet die van de gebruikers.

De volgende lijst illustreert hoe de Gefabriceerde Kosten in de Planner van het Middel wordt berekend:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> begrote Kosten </strong> </th> 
   <th><strong> Berekening </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Door gebruiker begrote kosten</td> 
   <td> <p>De begrote Kosten per gebruiker wordt berekend met behulp van de volgende formule:</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>OPMERKING</b>

Als de gebruiker geen Kosten per Uur in hun profiel heeft, is de Gefabriceerde Kosten van de Gebruiker $0.00.</p> </p> </td>
</tr> 
  <tr> 
   <td>Geraamde kosten voor rol</td> 
   <td> <p>De Rol begrote Kosten wordt berekend gebruikend de volgende formule:</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>OPMERKING</b>

Als de rol geen Kosten per Uur tarief heeft, is de begrote Kosten van de Rol $0.00.</p> </p> </td>
</tr> 
  <tr> 
   <td>Geraamde projectkosten</td> 
   <td> <p>De begrote kosten per project worden berekend aan de hand van de volgende formule:</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
