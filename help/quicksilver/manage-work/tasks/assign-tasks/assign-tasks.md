---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Taken toewijzen
description: U kunt taken aan gebruikers, rollen, of teams toewijzen om erop te wijzen wie voor de voltooiing van de taken verantwoordelijk is. U kunt een taak aan meer dan één middel tegelijkertijd toewijzen.
author: Lisa
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 21c98e443a6d6ca79045e2f4aba5f792340833cd
workflow-type: tm+mt
source-wordcount: '1617'
ht-degree: 0%

---

# Taken toewijzen

<!--Audited: 10/2025-->

<!--remove production/ preview and old/ new experience references at prod-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Second Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md). 

</div>-->

U kunt taken aan gebruikers, baanrollen, of teams toewijzen om erop te wijzen wie voor de voltooiing van de taken verantwoordelijk is. U kunt een taak aan meer dan één middel tegelijkertijd toewijzen.

>[!TIP]
>
>U kunt meerdere gebruikers, taakrollen of teams toewijzen. U kunt alleen actieve gebruikers, taakrollen en teams toewijzen.
>
>Als een gebruiker, een baanrol, of een team werd toegewezen alvorens zij werden gedeactiveerd, blijven zij toegewezen aan het het werkpunt. In dit geval raden we het volgende aan:
>
>* Wijs het werkitem opnieuw toe aan actieve bronnen.
>* Koppel de gebruikers in een gedeactiveerd team aan een actief team en wijs het het werkpunt aan het actieve team opnieuw toe.
>

Het aantal gebruikers dat aan een taak en het programma van de taakeigenaar wordt toegewezen kan de geplande data van een taak wijzigen die in het veranderen van de chronologie van het project resulteert. Voor informatie over het effect van het toewijzen van veelvoudige gebruikers aan een taak, zie [&#x200B; Overzicht van het wijzigen van taaktaken &#x200B;](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

Naast dit artikel raden we u aan de volgende artikelen te lezen voor meer informatie over het toewijzen van taken:

* [&#x200B; Overzicht van het wijzigen van taaktaken &#x200B;](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [&#x200B; Slim overzicht van taken &#x200B;](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [&#x200B; maak slimme taken &#x200B;](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [&#x200B; creeer geavanceerde taken &#x200B;](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [&#x200B; wijzigt veelvoudige gebruikerstoewijzingen in een taaklijst &#x200B;](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [&#x200B; geef taken &#x200B;](../../../manage-work/tasks/manage-tasks/edit-tasks.md) uit
* [&#x200B; Plan een projectoverzicht &#x200B;](../../../manage-work/projects/planning-a-project/plan-project.md)
* [&#x200B; Overzicht van de taak Geplande Datum van de Voltooiing &#x200B;](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [&#x200B; plaats het project Geplande Datum van de Voltooiing &#x200B;](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [&#x200B; vorm systeem-brede projectvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [Overzicht van het toewijzen van werk in de werklastverdeler](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td> <p>Standard</p>
   <p>Werk of hoger</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten en taken bewerken</p> <p>Toegang tot gebruikers weergeven of vergroten</p> </td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td>
   <td>Contribute of hoger machtigingen voor de taak</td>
  </tr>
 </tbody>
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen voor veelvoudige taken aan baanrollen, teams, en gebruikers

Overweeg het volgende wanneer het toewijzen van veelvoudige middelen aan een het werkpunt:

* Gebruikers kunnen meer dan één taakrol aan hun profiel koppelen. Voor informatie over het associëren van gebruikers met baanrollen, zie [&#x200B; het profiel van een gebruiker &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

* Als u meerdere gebruikers aan een taak of uitgave toewijst, wordt de eerste gebruiker die u selecteert, automatisch aangewezen als de eigenaar van de taak of uitgave.
Voor instructies bij het veranderen van dit, zie de informatie over de Primaire optie van het Merk in het artikel [&#x200B; Geavanceerde taken &#x200B;](create-advanced-assignments.md) creëren.

* Een team kan geen primaire ontvanger zijn voor een taak of kwestie. Alleen een gebruiker of een taakrol kan worden aangewezen als primair op een taak of kwestie.

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* De taken en de kwesties op een project zouden eerst aan één of meerdere teams of baanrollen kunnen worden toegewezen. Wanneer het project klaar is te beginnen, zouden zij ook aan gebruikers kunnen moeten worden toegewezen:

  <table>
  <col> 
  <col> 
  <tbody>
  <tr>
   <td>Teams</td>
   <td>Als u een taak aan een team toewijst en u ook een gebruiker toewijst, blijft de taak toegewezen aan het team en aan de gebruiker, zelfs als de gebruiker geen lid van het team is.</td>
  </tr>
  <tr>
   <td>Functies</td>
   <td><p>Als u een taak of een kwestie aan één of veelvoudige rollen toewijst en dan ook een gebruiker toewijst, besluit welke baanrol aan de extra gebruiker (als om het even welk) te associëren volgens de volgende regels:</p>
     <ul>
      <li>Als er slechts één toegewezen baanrol is en het de primaire rol van de gebruiker (die in hun profiel wordt gevormd) aanpast, wordt de taak of de kwestie toegewezen slechts aan die gebruiker.</li>
      <li>Als de veelvoudige rollen worden toegewezen en minstens één van hen één van de andere rollen van de gebruiker aanpast, wordt de taak of de kwestie toegewezen aan de gebruiker (de rol wordt willekeurig geselecteerd als er veelvoudige gelijken zijn), samen met om het even welke extra rollen die worden toegewezen</li>
      <li>Als minstens één baanrol wordt toegewezen en er geen gelijken aan de de baanrollen van de gebruiker zijn, wordt de taak of de kwestie toegewezen aan zowel de rol of de rollen als aan de gebruiker.</li>
     </ul>
   <p>Voor informatie over de primaire rol van een gebruiker en andere rollen, zie <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md"> het profiel van een gebruiker </a> uitgeven.</p>
   </td> 
     </tr>
  </tbody>
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations for multiple user assignments and using schedules</h2>
<p>(NOTE: moved to the Modify task assignments overview standalone article)</p>
<p>You can assign multiple resources to a task. When you assign a user to a task, Workfront uses the user's schedule to calculate the planned dates for the task which ultimately determine the timeline of the project. Using the schedule of the user takes into account their time off, holidays, and weekend days which are considered non-working days when task activity cannot occur. </p>
<p>When you assign multiple users to a task, your Workfront administrator <span>or a group administrator</span> determines which one of the following schedules Workfront uses to determine the planned dates of the tasks, based on schedules: </p>
<ul>
<li> <p><strong>The Primary Assignee's schedule</strong>: this is the schedule associated with the user designated as the task Owner.</p> <p>For information about associating users with schedules, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li>
<li><strong>The Project's schedule</strong>: this is the schedule associated with the project. For adding a schedule to a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
</ul>
<p>For information about setting up which schedule a project uses in the case of multiple assignments, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p>
</div>
-->

## Eén taak toewijzen

1. Ga naar een taak die u wilt toewijzen.
1. Klik **toewijzen aan** in het **3&rbrace; gebied van Taken &lbrace;in de kopbal van de taak**

   of

   Klik op de naam van de toewijzingen als de taak al is toegewezen.

   ![&#x200B; Taken &#x200B;](assets/assignments-from-task-header-0825.png)

1. Voer een van de volgende handelingen uit:

   * Typ de naam van een gebruiker, taakrol of team die u wilt toewijzen en klik vervolgens op de naam wanneer deze in de lijst wordt weergegeven.

     >[!TIP]
     >
     >Wanneer u een gebruikerstoewijzing toevoegt, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen. Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt.
     >
     >De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Voor informatie, zie [&#x200B; toegang van de Verlening tot gebruikers &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

   * (Voorwaardelijk) klik één van de namen in de **Gebruikers en teams** of **de rollen van de Baan** lijsten wanneer zij tonen. Voor meer informatie, zie [&#x200B; Slim toewijzingsoverzicht &#x200B;](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

     U kunt de naam typen van een gebruiker, team of taakrol die u wilt toewijzen aan de taak, en deze vervolgens selecteren wanneer deze wordt weergegeven in de lijst.

   * Klik **Geavanceerd**.

     Voor informatie over hoe te om geavanceerde taken te maken, zie [&#x200B; Geavanceerde taken &#x200B;](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md) creëren.

1. Klik **sparen**.
1. (Facultatief en voorwaardelijk) klik het **pictogram van X** naast de naam van de taak in het juiste paneel van de taak om een taak te verwijderen, als u **Geavanceerd** klikte.

## Een taak in een lijst toewijzen bij inlinebewerking

U kunt taken toewijzen in een lijst of rapport wanneer een van de toewijzingsvelden zichtbaar is in de lijstweergave. Dit is een snellere manier om taken toe te wijzen. In dit artikel wordt beschreven hoe u toewijzingen voor één taak in een lijst kunt wijzigen. Voor informatie over het wijzigen van veelvoudige taken voor veelvoudige taken in een lijst, zie [&#x200B; veelvoudige gebruikerstoewijzingen in een taaklijst &#x200B;](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md) wijzigen.

Afhankelijk van welk veld zichtbaar is in de weergave, kunt u de volgende entiteiten aan de taak toewijzen:

| Veld | Toegewezen entiteiten |
|---|---|
| **toewijzen aan** | Eén gebruiker toewijzen |
| **Toegewezen** | Eén gebruiker toewijzen |
| **Taken** | Gebruikers, taakrollen of teams toewijzen |

Taken in een lijst toewijzen:

1. Ga naar een lijst met taken waarvoor de velden Toegewezen aan, Toegewezen of Toegewezen in de weergave staan.
1. (Facultatief) klik **Autosave** drop-down menu en selecteer van de volgende opties:

   | Optie | Optiebeschrijving |
   |---|---|
   | Automatisch opslaan | Wijzigingen die u aanbrengt in de taken worden automatisch opgeslagen en u kunt ze niet terugzetten |
   | Handmatig opslaan | U moet uw wijzigingen handmatig opslaan. U kunt uw wijzigingen herstellen voordat u ze opslaat. |
   | Tijdlijnplanning | U moet uw wijzigingen handmatig opslaan. U kunt uw wijzigingen herstellen voordat u ze opslaat. Het opslaan van uw wijzigingen en alle projectafhankelijkheden is sneller dan wanneer u Handmatig opslaan selecteert. |

   Voor meer informatie over besparingstaken aangezien u hen in een lijst uitgeeft, zie [&#x200B; taken in een lijst &#x200B;](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) uitgeven.

1. Voer een van de volgende handelingen uit om taken toe te wijzen:

   * Klik binnen **Toegewezen aan** of **toegewezen** gebieden en begin de naam van een actieve gebruiker te typen die u aan de taak wilt toewijzen, dan het te klikken wanneer het in de lijst toont.
   * Klik binnen het **gebied van Taken** en begin de naam van een actieve gebruiker, baanrol, of team te typen die u aan de taak wilt toewijzen, dan het klikken wanneer het in de lijst toont.

     >[!TIP]
     >
     >Wanneer u een gebruikerstoewijzing toevoegt, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen. Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt.
     >
     >De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Voor informatie, zie [&#x200B; Toegang van de Verlening tot gebruikers &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)

     <!--<span class="preview">When adding a job role assignment, you can search for the job role or location. Select a Job role to use the default billing rate for the assignment, or select a Rate Card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>-->


1. (Voorwaardelijk) op het gebied van Taken, klik **Geavanceerd** bij de bodem van de lijst, of het **pictogram van Mensen** ![&#x200B; het pictogram van Mensen &#x200B;](assets/teams.png) in de hoger-juiste hoek van de toewijzingsdoos, om **Geavanceerde de doos van Toewijzingen** te openen en geavanceerde taken tot stand te brengen.

   Voor meer informatie, zie [&#x200B; Geavanceerde taken &#x200B;](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md) creëren.

   >[!TIP]
   >
   >U kunt geen geavanceerde toewijzingen maken vanuit de velden Toegewezen aan of Toegewezen.

1. Nadat u de toewijzingen aan de taak hebt toegevoegd, drukt u op Enter of klikt u ergens op de pagina om de wijzigingen op te slaan als u Automatisch opslaan hebt geselecteerd. Anders, klik **sparen**.

## Meerdere taken bulksgewijs vanuit een lijst toewijzen

1. Ga naar een lijst van taken die u in bulk wilt toewijzen.
1. (Voorwaardelijk) zorg ervoor dat de **optie Autosave** wordt geselecteerd als u op een lijst van taken onder een project bent.

   >[!IMPORTANT]
   >
   >U kunt taken niet bulksgewijs bewerken wanneer u taken handmatig in een project opslaat.

1. Selecteer verschillende taken in de takenlijst.
1. Klik **uitgeven**.

   Het **geeft de doos van Taken** uit opent.

1. In het **gebied van Taken**, begin de naam van gebruikers, teams, of rollen in het **Gebieden de mensen van het Onderzoek, rollen, of teams** gebied, dan klikken hen wanneer zij in de lijst tonen

   >[!IMPORTANT]
   >
   >Als om het even welke taken reeds wordt toegewezen, worden de middelen u hier op wijst toegevoegd aan de taken in plaats van het vervangen van de bestaande middelen op de taken.

1. Geef de volgende velden op voor de geselecteerde taken:

   * Beweeg over de toewijzingsnaam, dan klik **Primair maken** om erop te wijzen welke ontvanger de eigenaar van de taak is.
   * **Type van Duur**

     Voor informatie over het Type van Duur op taken, zie [&#x200B; Overzicht van het Type van Duur van de Taak en van de Duur &#x200B;](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **Duur**
   * **Geplande Uren**

     Voor meer informatie, zie [&#x200B; taken &#x200B;](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md) uitgeven.

1. (Optioneel) Als u bestaande toewijzingen uit alle taken wilt verwijderen, klikt u op **x** naast hun naam in het **gebied van het Onderzoek mensen, rollen, of teams**.

1. Klik **sparen**.
1. (Facultatief en voorwaardelijk) wanneer **aan** of de **3&rbrace; gebieden van Taken &lbrace;in uw lijst van taken wordt toegewezen, klik binnen één van deze kolommen voor een taak, dan klik het** X pictogram **naast de naam van een ontvanger om het uit de taak te verwijderen.**


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations about unassigning tasks</h2>
<p>(NOTE: moved this to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm)</p>
<p>You can remove assignments from one task at a time, or you can remove assignments from multiple tasks in bulk.</p>
<p>For more information about removing assignments from tasks in bulk, see <a href="../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md" class="MCXref xref">Modify multiple user assignments in a task list</a>. </p>
<p>Consider the following when removing assignments from tasks: </p>
<ul>
<li>When you unassign a user from a task, the task remains assigned to the job role that the user fulfilled on the task.</li>
<li>When you unassign a job role or a team from a task, the task remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->


<!--Assigning multiple tasks in bulk from a list differs depending on which environment you choose. 

### Assign multiple tasks in bulk from a list in the Production environment

1. Go to a list of tasks that you want to assign in bulk. 
1. (Conditional) Ensure that the **Autosave** option is selected if you are on a list of tasks under a project.

   >[!IMPORTANT]
   >
   >You cannot edit tasks in bulk when saving tasks manually on a project.

1. Select several tasks in the tasks list. 
1. Click **Edit**.

   The **Edit Tasks** dialog box opens in the new experience.

1. Continue assigning the tasks using the new experience.

   For more information, see the section [Assign multiple tasks in bulk from a list in the new experience](#assign-multiple-tasks-in-bulk-from-a-list-in-the-new-experience) in this article.

1. (Optional) Click **Switch back to old experience** at the bottom of the **Edit Tasks** box to open the old experience.

1. (Conditional) Using the old experience, in the **Assignments** area, select the **Assignee** box, then start typing the name of a user, job role, or team that you want to assign to all the tasks.

   >[!IMPORTANT]
   >
   >If any of the tasks is already assigned, the resources you indicate here are added to the tasks instead of replacing the existing resources on the tasks. 

1. (Optional) Select the radio button in the **Task Owner** column to indicate which resource is the primary assignee or the Owner of the task, when you assign more than one resource to the task. This is not available for teams. 
1. (Conditional) Specify the **Allocation %** for each resource assigned to the task if all the tasks you selected have a Duration Type of Effort Driven or Calculated Assignment. This indicates how much of their time these resources should spend on completing the task. This is only available for users and job roles.

   Or

   Specify the amount of **Hours** for each resource assigned to the task if all the tasks you selected have a Duration Type of Simple. The total of all hours for all resources should equal the number of Planned Hours for the task.

   >[!IMPORTANT]
   >
   >You cannot specify the allocation percentage or the number of hours per resource if the tasks you selected have different Duration Types or of the tasks you selected have different Duration Types.

   For information about Duration Type on tasks, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Optional) Select a role that the user should fulfill on the task from the **Pick a role** drop-down menu in the **Assignee's Role** column when you assign users to tasks. If you do not select a role, Workfront automatically selects the user's Primary Role. 

1. (Optional) If you want to remove existing assignees from all tasks do one of the following:

   1. Start typing the name of a user, role, or team you want to remove from the task, then select it when it appears on the list and click **Remove Assignee** to remove more assignees.
   1. Click **Remove All Existing Assignees** to remove all assignees from all selected tasks.

1. Click **Save Changes**.
1. (Optional and conditional) When the Assigned to or the Assignments fields display in your list of tasks, click inside one of these columns for a task, then click the **X icon** next to the name of an assignee to remove it from the task.


#### Assign multiple tasks in bulk from a list in the new experience

1. Go to a list of tasks that you want to assign in bulk.
1. (Conditional) Ensure that the **Autosave** option is selected if you are on a list of tasks under a project.

   >[!IMPORTANT]
   >
   >You cannot edit tasks in bulk when saving tasks manually on a project.

1. Select several tasks in the tasks list. 
1. Click **Edit**.

   The **Edit Tasks** dialog box opens.

1. In the **Assignments** area, start typing the name of users, teams, or roles in the **Search people, roles, or teams** field provided, then click them when they display in the list

   Or 

   Click **Assign to me** to assign it to yourself.

   >[!IMPORTANT]
   >
   >If any of the tasks is already assigned, the resources you indicate here are added to the tasks instead of replacing the existing resources on the tasks.

1. Click inside the **Duration Type** field and choose a Duration Type. 

   For information about Duration Type on tasks, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Conditional) Depending on what **Duration Type** you selected, update the following fields: 

   * Duration
   * Planned Hours

      For more information, see [Edit tasks](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md). 

1. (Optional) If you want to remove existing assignees from all tasks, click the **x** next to their name in the **Search people, roles, or teams** field.

1. Click **Save**.
1. (Optional and conditional) When the **Assigned to** or the **Assignments** fields display in your list of tasks, click inside one of these columns for a task, then click the **X icon** next to the name of an assignee to remove it from the task.

<div class="preview">
### Assign multiple tasks in bulk from a list in the Preview environment
-->