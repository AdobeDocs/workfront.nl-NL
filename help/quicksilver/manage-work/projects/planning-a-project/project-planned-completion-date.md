---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: De geplande projectuitvoeringsdatum instellen
description: De geplande uitvoeringsdatum van een project is de datum waarop het project moet worden voltooid.
author: Alina
feature: Work Management, Projects
role: User
exl-id: 996398c5-de92-445e-8e86-36b2efdcf6b5
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 0%

---

# Geplande afsluitdatum van project instellen

<!-- Audited: 4/2025 -->

De geplande uitvoeringsdatum van een project is de datum waarop het project moet worden voltooid.

Voor het geplande begin en de geplande einddatum van een project wordt uitgegaan van de datum van de taken van het project. In dit artikel wordt beschreven hoe u de geplande voltooiingsdatum van een project handmatig of automatisch kunt instellen. Voor meer informatie over de Geplande Datum van de Voltooiing van een taak, zie [ Overzicht van de taak Geplande Datum van de Voltooiing ](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

De geplande Voltooiingsdatum van een project kan manueel of automatisch worden geplaatst, afhankelijk van of u het project van het Begin of van de Datum van de Voltooiing plant.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
   <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten bewerken</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het project beheren</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>
   New: Standard

   Or

   Current: Plan </p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## De geplande voltooiingsdatum van een project handmatig instellen

U moet manueel de Geplande Datum van de Voltooiing van een project plaatsen wanneer u het project van de Datum van de Voltooiing plant.

>[!NOTE]
>
>Wanneer u manueel de Geplande Datum van de Voltooiing van een project plaatst, berekent Workfront automatisch de Geplande Datum van het Begin van het project dat op de Duur van alle taken wordt gebaseerd.


Een project plannen vanaf de voltooiingsdatum:

{{step1-to-projects}}

1. Klik **Nieuw Project**, dan uitgezocht **Nieuw Project** van dropdown.

   Voor meer informatie over het creëren van projecten, zie het artikel [ een project ](../../../manage-work/projects/create-projects/create-project.md) creëren.

1. Selecteer **Details van het Project** in het linkerpaneel.

1. Klik **uitgeven het pictogram van het Project** ![ geeft pictogram ](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png) in de hoger-juiste hoek uit en selecteert dan **Overzicht** in de drop-down die verschijnt.

1. In de **sectie van de Datums van het 0} Project {, klik het** gebied van de Wijze van het Programma **, dan selecteer** Datum van de Voltooiing **.**

1. Specificeer de **Geplande Datum van de Voltooiing** van het project.
1. Klik **sparen Veranderingen**.

   Aangezien u begint taken aan uw project toe te voegen, berekent de **Geplande Datum van het Begin** van het project gebaseerd op de totale Duur van alle taken.

## De geplande voltooiingsdatum van een project automatisch instellen

De geplande Voltooiingsdatum van een project wordt automatisch berekend door Workfront wanneer u het project van de Datum van het Begin plant.

Een project plannen vanaf de begindatum:

{{step1-to-projects}}

1. Klik **Nieuw Project**, dan uitgezocht **Nieuw Project** van drop-down die verschijnt.

   Voor meer informatie over het creëren van projecten, zie het artikel [ een project ](../../../manage-work/projects/create-projects/create-project.md) creëren.

1. Selecteer **Details van het Project** in het linkerpaneel.

1. Klik **uitgeven het pictogram van het Project** ![ geeft pictogram ](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png) in de hoger-juiste hoek uit en selecteert dan **Overzicht** in de drop-down die verschijnt.

1. In de **sectie van de Datums van het 0} Project {, klik het** gebied van de Wijze van het Programma **, dan selecteer** Datum van het Begin **.**

1. Specificeer de **Geplande Datum van het Begin** van het project.
1. Klik **sparen Veranderingen**.

   Aangezien u begint taken aan uw project toe te voegen, berekent de **Geplande Datum van de Voltooiing** van het project gebaseerd op de totale Duur van alle taken.

   Voor meer informatie over de Duur van de Taak, zie het artikel [ Overzicht van het Type van Duur en van de Duur van de Taak ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   De geplande datum van voltooiing van het project valt in dit geval samen met de geplande datum van voltooiing van de laatste taak van het project.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>The Planned Completion Date of a task</h2>
<p>(NOTE: drafted because I created a new article, here: /Content/Manage work/Tasks/Task information/task-planned-completion-date.htm)</p>
<p>You can either specify the Planned Completion Date of a task, or you can leave it up to Workfront to calculate it depending on certain criteria. </p>
<ul>
<li><a href="#manually-set-the-planned-completion-date-of-a-task" class="MCXref xref">Manually set the Planned Completion Date of a task</a> </li>
<li><a href="#how-the-planned-completion-date-is-calculated-for-a-task" class="MCXref xref">How the Planned Completion Date is calculated for a task</a> </li>
</ul>
<p><strong>Manually set the Planned Completion Date of a task</strong></p>
<p>Setting the Planned Completion Date of a task depends on the type of Task Constraint you assign to the task. </p>
<p>You can manually set the Planned Completion Date when creating a task, as described in the article <a href="../../../manage-work/tasks/create-tasks/create-tasks-in-project.md" class="MCXref xref">Create tasks in a project</a>.</p>
<p>You can manually specify the Planned Completion Date when you select any of the following Task Constraints: </p>
<table border="1" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th> <p><strong>Task Constraint Type</strong> </p> </th>
<th> <p><strong>Effect of Manually Changing the Planned Completion Date</strong> </p> </th>
</tr>
</thead>
<tbody>
<tr>
<td> <p>Must Finish On</p> <p>Finish No Later Than</p> <p>Finish No Earlier Than</p> </td>
<td> <p><span class="s1">The Planned Start Date is adjusted in order to keep the Duration the same.</span> </p> </td>
</tr>
<tr>
<td> <p>Fixed Dates</p> </td>
<td> <p>The Duration is adjusted in order to keep the Planned Start Date the same.</p> </td>
</tr>
</tbody>
</table>
<p><strong>How the Planned Completion Date is calculated for a task</strong></p>
<p>When it is calculated automatically by the system, the following can influence the Planned Completion Date of a Task:</p>
<ul>
<li> <p>Task Constraint</p> <p>For more information about Task Constraints, see the article <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </li>
<li> <p>Task predecessor relationship</p> <p>For more information about task predecessors, see the article <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p> </li>
<li>Project Completion Date, when the project is scheduled from Completion Date.</li>
<li> <p>The time off schedule of the Primary Assignee of the task. </p> <p>When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the <strong>Consider user time off in task durations</strong> setting is selected for the <strong>User Time Off</strong> field. New projects inherit this setting from the Project Preferences area, but you can edit the setting at the project level. </p> <p>For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 2 marked for Time-off, the task Planned Completion Date becomes June 4. </p> <p>For information about the <strong>User Time Off</strong> preference, see the articles <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a> or <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li>
</ul>
<p>When set automatically, the Planned Completion Date is determined based on the following calculation: </p>
<p><code>Planned Completion Date = Planned Start Date + Duration</code> </p>
<p>For example, if your task has a start date of September 16 and a duration of 10 days, the Planned Completion Date is September 26.</p> <note type="note">
 The Update Type for the project must also be set to Automatic and On Change or Automatically in order for the Planned Hours and Duration to be automatically adjusted.
<br>For more information about the Update Type, see the article
<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.
</note>
</div>
-->
