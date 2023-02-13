---
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: Beschikbare, geplande en Werkelijke uren of FTE weergeven in de bronnenplanner bij gebruik van de gebruikersweergave
description: De mening Beschikbare, Geplande, en Ware Uren of FTE in de Planner van het Middel wanneer het gebruiken van de gebruiker viewPlanning"in RP" - misschien "het opnemen van middelen in RP"of "het Leiden Middelen in RP." enz. - of moet een andere POV opnieuw worden gebruikt?!)"
author: Alina
feature: Resource Management
exl-id: 6b532aa2-435f-4fda-b7ce-abe0a785638f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1738'
ht-degree: 0%

---

# Beschikbare, geplande en Werkelijke uren of FTE weergeven in de bronnenplanner bij gebruik van de gebruikersweergave

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Consider renaming this article (probably split already) to something other than "Planning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)</p>
-->

Naast het opnemen van middelen in de mening van het Project en van de Rol, kunt u de Mening van de Gebruiker van de Planner van het Middel van Adobe Workfront gebruiken om informatie over Geplande, Beschikbare, en Ware Uren of waarden van FTE voor projecten en middelen te tonen.

## Overzicht van de weergave Gebruiker in de functie voor middelenplanner

Overweeg het volgende wanneer het bekijken van de informatie van Uren of FTE in de Planner van het Middel:

* U kunt de Beschikbare en Geplande Uren of de informatie FTE voor gebruikers, baanrollen, en projecten in alle meningen van de Planner van het Middel bekijken.
* U kunt de volgende informatie alleen weergeven in de weergave Gebruiker:

   * Het verschil tussen de hoeveelheid geplande uren of VTE en de hoeveelheid beschikbare uren of VTE. Vervolgens kunt u de toewijzing van uw gebruikers begroeten op basis van dit verschil in de projectweergave en de weergave Rol.
   * De werkelijke uren of VTE.

* U kunt het verschil tussen de Beschikbare Gebruiker en de hoeveelheid Geplande Uren of VTE of als aantal of als percentagewaarde in de mening van de Gebruiker tonen.
* U kunt de gegevens niet in de weergave Gebruiker weergeven op kosten.
* Adobe Workfront vult Beschikbare uren of VTE volgens de arbeidstijd verbonden aan de gebruikers in hun programma&#39;s.\
   De gebruikers niet verbonden aan een programma tonen beschikbaarheid volgens het StandaardProgramma.\
   Voor informatie over het Standaard Programma, zie [Een schema maken](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Workfront vult geplande uren of VTE van de Geplande Uren informatie over de taken en de kwesties betreffende de projecten.
* Workfront vult Werkelijke uren met de daadwerkelijke tijd die aan taken en kwesties wordt geregistreerd door de gebruikers die aan hen worden toegewezen. Dit omvat tijd die op een project wordt het programma wordt geopend.
* In de weergave Gebruiker kunt u het volgende doen:

   * Breid elke gebruiker uit om een lijst van projecten te tonen waar die gebruiker wordt toegewezen.

      >[!NOTE]
      >
      >Alleen gebruikers die zijn gekoppeld aan de projecten die in de filters zijn opgenomen, kunnen worden uitgebreid.

   * Breid elk project uit om een lijst van baanrollen te tonen die de gebruiker op die projecten kan vervullen.
   * Breid elke rol uit om een lijst van taken te tonen de gebruiker in die rol wordt toegewezen aan.

   Als gebruikers geen functies hebben die aan hen zijn gekoppeld, worden hun Beschikbare, Geplande en Werkelijke uren of VTE vermeld in het dialoogvenster **Geen rol** sectie.\
   Voor informatie over welke gebieden en punten wanneer het toepassen van de mening van de Gebruiker op de Planner van het Middel tonen, zie de &quot;sectie van het Project/van de Rol/van de Mening van de Gebruiker van de Selectie&quot;in [Overzicht van de navigatie in de bronnenplanner](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Overzicht van velden die zichtbaar zijn in de weergave Gebruiker van de functie voor middelenplanner

Verwijs naar de volgende lijsten voor het begrip van de informatie die in de mening van de Gebruiker van de Planner van het Middel wordt getoond. De informatie wordt weergegeven in uren of FTE-waarden.

* [De kolom AVL (Beschikbaar)](#the-avl-available-column)
* [De kolom PLN (gepland)](#the-pln-planned-column)
* [De kolom ACT (Actual)](#The%C2%A0ACT)
* [De DIF-kolom (Verschil)](#the-dif-difference-column)
* [De kolom % (percentage geplande uren toewijzing)](#the-planned-hours-allocation-percentage-column)

### De kolom AVL (Beschikbaar) {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Weergegeven door</strong> </td> 
   <td> <p><strong>Beschrijving</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Gebruiker</td> 
   <td>Het totaal van Beschikbare Uren of VTE voor de gebruiker volgens hun programma. </td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>Deze informatie is niet beschikbaar voor het Project wanneer het toepassen van de mening van de Gebruiker op de Planner van het Middel. </td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> <p>Het totaal van Beschikbare uren of VTE voor de rol volgens het programma van de gebruiker en <strong>Percentage van de beschikbaarheid van VTE</strong> van de rol.</p> </td> 
  </tr> 
  <tr> 
   <td>Taak of probleem</td> 
   <td>Deze informatie is niet beschikbaar voor de Taak of de Uitgave. </td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie over hoe de gebruiker en rolbeschikbaarheid gebaseerd op het programma van de gebruiker en het Percentage van VTE Beschikbaarheid van de rol wordt berekend, zie [Overzicht van het berekenen van uren en FTE voor gebruikers en rollen in de Planner van het Middel](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

### De kolom PLN (gepland) {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Weergegeven door</strong> </td> 
   <td> <p><strong>Beschrijving</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Gebruiker</td> 
   <td> Het totaal van Geplande Uren of VTE van alle taken of kwesties die aan de gebruiker op alle projecten worden toegewezen.<br><p>Dit omvat taken en kwesties die aan de gebruiker worden toegewezen maar niet verbonden aan enige baanrol en taken of kwesties die niet op projecten zijn die u toegang tot Beheren hebt.</p><p>Wanneer de gebruikerstoewijzing voor uren is gewijzigd met behulp van Workload Balancer, kunnen de gegevens in de Planner van het Middel worden beïnvloed als de geselecteerde data slechts een gedeelte van een taak of kwestie bevatten. Voor informatie over het wijzigen van toewijzingen voor gebruikers raadpleegt u <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Toewijzingen van gebruikers beheren in Workload Balancer</a> . </p></td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td> Het totaal van Geplande Uren of VTE van alle taken en kwesties die aan een specifieke gebruiker op het project worden toegewezen.<br><p>Opmerking: Hieronder vallen niet de geplande uren of VTE van taken of problemen die niet aan gebruikers zijn toegewezen. </p></td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> <p>Het totaal van Geplande Uren of VTE van alle taken en kwesties die aan de gebruiker in deze rol op het project worden toegewezen.</p> <p> <p>Opmerking: Dit omvat niet de Geplande Uren of VTE van taken of kwesties die aan deze rol maar niet aan deze gebruiker in deze rol worden toegewezen. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Taak of probleem</td> 
   <td>De geplande uren of VTE verbonden aan de taak of de kwestie op het project.</td> 
  </tr> 
 </tbody> 
</table>

Houd rekening met het volgende wanneer u geplande uren bekijkt:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view)</p>
-->

* De geplande uren worden gelijkelijk verdeeld aan elke dag binnen de Duur van taken en kwesties, voor elke middelen die aan hen worden toegewezen. De taak of de duur van de kwestie is gebaseerd op hun Geplande Datum van Begin en Voltooiing en omvat elke kalenderdag binnen die periode.\
   Workfront houdt rekening met het programma van de gebruiker of van het project wanneer het verdelen van Geplande Uren aan gebruikers of projecten. In dit geval worden de geplande uren gelijkelijk verdeeld over elke dag binnen de Duur van taken of kwesties exclusief weekends, time-off dagen, en planningsuitzonderingen.

   Als u de Planner van het Middel door Week, bijvoorbeeld toont, en u taken hebt die veelvoudige weken op projecten overspannen, hangt het aantal Geplande Uren per week af van hoeveel dagen binnen die week deel van de taakDuur uitmaken. Dit werkt op dezelfde manier wanneer het tonen van de Planner van het Middel door Maand of Kwart en wanneer de taken veelvoudige maanden of kwartalen overspannen.\
   De dagen van het weekeinde, de programmauitzonderingen, en de tijd-off dagen worden uitgesloten van deze distributie.

* De volgende taakcategorieën worden opgenomen in de berekening van de geplande uren voor elke bron:

   * taken die aan gebruikers in de Groepen van het Middel, baanrollen, of teams op het project worden toegewezen.

      >[!TIP]
      >
      >Als de taken aan teams worden toegewezen, zal hun toewijzing onder **Geen rol** en **Geen gebruiker** secties. U kunt de Geplande Uren zien verbonden aan teams, maar u kunt niet de uren begroten, omdat geen rollen noch gebruikers met de taken worden geassocieerd.

* De geplande uren in de Planner van het Middel omvatten geen Geplande Uren verbonden aan het volgende:

   * bovenliggende taken
   * niet toegewezen taken
   * , wanneer de **Uren opnemen uit uitgaven** instellen is uitgeschakeld.

* Geplande uren worden niet weergegeven in de bronnenplanner als de taak of uitgave nul is.
* De geplande uren die zijn gekoppeld aan gedeactiveerde gebruikers worden niet weergegeven.

Voor meer informatie over Geplande Uren en VTE in de Planner van het Middel, zie [Overzicht van uren, FTE, en kosteninformatie in de mening van het Project en van de Rol van de Planner van het Middel](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

### De kolom ACT (Actual)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Weergegeven door</strong> </td> 
   <td> <p><strong>Beschrijving</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Gebruiker </td> 
   <td> <p>De tijd die door de gebruiker op alle taken of kwesties wordt geregistreerd die aan hen worden toegewezen.</p> <p>Dit omvat het volgende:</p> 
    <ul> 
     <li>Taken en problemen die aan de gebruiker zijn toegewezen, maar niet aan een taakrol zijn gekoppeld.</li> 
     <li>Taken en kwesties die zich niet op projecten bevinden waarvoor u toegang hebt tot Beheren. </li> 
    </ul> <p>Dit omvat de tijd die op het project wordt het programma wordt geopend slechts wanneer de gebruiker aan taken of kwesties op dat project wordt toegewezen.  </p> </td> 
  </tr> 
  <tr> 
   <td>Project </td> 
   <td> <p>De tijd die door de gebruiker op alle taken en kwesties wordt geregistreerd die aan hen op het project worden toegewezen.</p> <p>Dit omvat om het even welke tijd dat zij direct op het project het programma opende.</p> <p>Hieronder vallen niet:</p> 
    <ul> 
     <li> <p>De tijd het programma geopende taken en kwesties die niet aan om het even welke gebruikers worden toegewezen. </p> </li> 
     <li> <p>Tijd die op oudertaken wordt geregistreerd. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> <p>De tijd het programma werd geopend alle taken of kwesties die aan de gebruiker in deze rol worden toegewezen. </p> <p>Hieronder vallen niet:</p> 
    <ul> 
     <li>Tijd het programma geopende taken en kwesties die aan deze rol maar niet aan deze gebruiker in deze rol worden toegewezen.</li> 
     <li>Tijd die direct op het project of oudertaken wordt geregistreerd. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Taak of probleem </td> 
   <td> <p>De tijd het programma werd geopend taken en kwesties door de gebruiker die ook aan hen wordt toegewezen. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>De tijd het programma wordt geopend toont in timeframe die overeenkomt met de ingangsdatum van de ingang van het uur, ongeacht het tijdframe van de taak, uitgave of project waar de uren worden geregistreerd.

Zie voor meer informatie over Werkelijke uren [Werkelijke uren weergeven](../../manage-work/tasks/task-information/actual-hours.md).

### De DIF-kolom (Verschil) {#the-dif-difference-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Weergegeven door</strong> </td> 
   <td> <p><strong>Beschrijving</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Gebruiker</td> 
   <td> <p>Het verschil tussen de Beschikbare en Geplande Uren of VTE van de gebruiker. </p> <p>Het Uur- of FTE-verschil wordt berekend aan de hand van de volgende formule:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>Opmerking: Als de waarde in negatieve rode getallen wordt weergegeven, wordt de gebruiker oververdeeld. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>Deze informatie is niet beschikbaar voor het project. </td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> <p>Het verschil tussen de Beschikbare en Geplande Uren of VTE van de baanrol. </p> <p>Het Uur- of FTE-verschil wordt berekend aan de hand van de volgende formule:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>Opmerking: Als de waarde in negatieve rode aantallen wordt getoond, is de rol oververdeeld. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Taak of probleem</td> 
   <td>Deze informatie is niet beschikbaar voor de Taak, de Uitgave, of het Project. </td> 
  </tr> 
 </tbody> 
</table>

### De kolom % (percentage geplande uren toewijzing) {#the-planned-hours-allocation-percentage-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Weergegeven door</strong> </td> 
   <td> <p><strong>Beschrijving</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>Gebruiker</td> 
   <td> <p>De toewijzing van de geplande uren of VTE als percentage van de beschikbare uren. Het percentage van de geplande uurtoerekening wordt berekend aan de hand van de volgende formule:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>Dezelfde berekening wordt gebruikt voor FTE-waarden. </p> </td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>Deze informatie is niet beschikbaar voor het project wanneer u het <strong>Weergeven op gebruiker</strong> aan de Planner van het Middel.</td> 
  </tr> 
  <tr> 
   <td>Rol</td> 
   <td> De toewijzing van de geplande uren of VTE als percentage van de beschikbare uren. <p>Het percentage van de geplande uurtoerekening wordt berekend aan de hand van de volgende formule:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>Dezelfde berekening wordt gebruikt voor FTE-waarden.</p></td> 
  </tr> 
  <tr> 
   <td>Taak of probleem</td> 
   <td>Deze informatie is niet beschikbaar voor de Taak, de Uitgave, of het Project. </td> 
  </tr> 
 </tbody> 
</table>

Als de waarde van de Geplande Uren of VTE nul is, is de Percentage Toewijzing 0%. Als de waarde van de Beschikbare Uren of FTE nul is, kan de Percentage van Toewijzing niet worden berekend.

Voor meer informatie over Geplande Uren en VTE en hoe zij in de Planner van het Middel worden getoond, zie [De middelen van de begroting in de Planner van het Middel gebruikend de meningen van het Project en van de Rol](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this table is ideal but it does not render in Markdown) </p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours or FTE)</strong> </td>
<td><strong>Displayed By</strong> </td>
<td> <p><strong>Description</strong> </p> </td>
</tr>
<tr>
<td rowspan="5">AVL <br>(Available Hours or FTE)</td>
<td>User</td>
<td>The total of Available Hours or FTE for the user according to their schedule. </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the User view to the Resource Planner. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Available Hours or FTE for the role according to the schedule of the user and the <strong>Percentage of FTE Availability</strong> of the role.</p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project.</td>
</tr>
<tr>
<td colspan="2"> <p colspan="2">For more information about how user and role availability is calculated based on the schedule of the user and the Percentage of FTE Availability of the role, see <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">PLN <br>(Planned Hours or FTE)</td>
<td>User</td>
<td> The total of Planned Hours or FTE from all the tasks or issues assigned to the user on all the projects.<br><p>This includes tasks and issues that are assigned to the user but not associated with any job role and tasks or issues that are not on projects that you have access to Manage.</p><p>When the user allocation for hours has been modified using the Workload Balancer, the data in the Resource Planner can be affected if the dates selected contain only a portion of a task or issue. For information about modifying allocations for users, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a> . </p></td>
</tr>
<tr>
<td>Project</td>
<td> The total of Planned Hours or FTE from all the tasks and issues assigned to a specific user on the project.<br><note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are not assigned to any users.
</note></td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Planned Hours or FTE from all the tasks and issues assigned to the user in this role on the project.</p> <p> <note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are assigned to this role but not to this user in this role.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>The Planned Hours or FTE associated with the task or the issue on the project.</td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view))</p>
<ul>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks and issues , for each resource assigned to them. The task or issue Duration is based on their Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks or issues excluding weekends, time-off days, and schedule exceptions.</p> <p>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> <p>The following categories of tasks are included in calculating the Planned Hours for each resource: </p>
<ul>
<li> <p> tasks assigned to users in Resource Pools, job roles, or teams on the project.</p> <note type="tip">
If tasks are assigned to teams, their allocation will appear under
<strong>No Role</strong> and
<strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks.
</note> </li>
</ul> </li>
</ul>
<ul>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>unassigned tasks</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task or issue Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> <p>For more information about Planned Hours and FTE in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">ACT<br>(Actual Hours or FTE) </td>
<td>User </td>
<td> <p>The time logged by the user on all the tasks or issues assigned to them.</p> <p>This includes the following:</p>
<ul>
<li>Tasks and issues that are assigned to the user but not associated with any job role.</li>
<li>Tasks and issues that are not on projects for which you have access to Manage.. </li>
</ul> <p>This does not include time logged directly on the project or on parent tasks. </p> </td>
</tr>
<tr>
<td>Project </td>
<td> <p>The time logged by the user on all the tasks and issues assigned to them on the project.</p> <p>This includes any time that they logged directly on the project.</p> <p>This does not include the following:</p>
<ul>
<li> <p>Time logged on tasks and issues that are not assigned to any users. </p> </li>
<li> <p>Time logged on parent tasks. </p> </li>
</ul> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The time logged on all the tasks or issues assigned to the user in this role. </p> <p>This does not include the following:</p>
<ul>
<li>Time logged on tasks and issues assigned to this role but not to this user in this role.<em> </em></li>
<li>Time logged directly on the project or parent tasks. </li>
</ul> </td>
</tr>
<tr>
<td>Task or Issue </td>
<td> <p>The time logged on tasks and issues by the user who is also assigned to them. </p> </td>
</tr>
<tr>
<td colspan="2"> <p> <note type="important">
The time logged is displayed in the timeframe corresponding to the Entry Date of the hour entry, regardless of the timeframe of the task, issue, or project where the hours are logged.
</note> </p> <p>For more information about Actual Hours, see <a href="../../manage-work/tasks/task-information/actual-hours.md" class="MCXref xref">View Actual Hours</a></p> </td>
</tr>
<tr>
<td rowspan="4">DIF <br>(Hour or FTE Difference) <br><br></td>
<td>User</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the user. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <note type="note">
If the value displays in negative red numbers, the user is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the job role. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <note type="note">
If the value is displayed in negative red numbers, the role is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td rowspan="5">Planned Hours or FTE Allocation Percentage (%)</td>
<td>User</td>
<td> <p>The allocation of the Planned Hours or FTE as a percentage of the Available Hours. The percentage of the Planned Hours Allocation is calculated using the following formula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>The same calculation is used for FTE values. </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the <strong>View by User</strong> view to the Resource Planner.</td>
</tr>
<tr>
<td>Role</td>
<td> The allocation of the Planned Hours or FTE as a percentage of the Available Hours. <p>The percentage of the Planned Hours Allocation is calculated using the following formula:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>The same calculation is used for FTE values.</p></td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td colspan="2"> <p> If the value of the Planned Hours or FTE is zero, the Percentage Allocation is 0%. If the value of the Available Hours or FTE is zero, the Percentage Allocation cannot be calculated. </p> <p>For more information about Planned Hours and FTE and how they are displayed in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> </td>
</tr>
</tbody>
</table>
-->
