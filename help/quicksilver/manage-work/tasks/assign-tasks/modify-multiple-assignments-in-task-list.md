---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Meerdere gebruikerstoewijzingen wijzigen in een takenlijst
description: Wanneer het beheren van taaktaken, kunt u hen voor veelvoudige taken tegelijkertijd wijzigen door de bulkbewerkingseigenschap in een lijst van taken te gebruiken.
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 21c98e443a6d6ca79045e2f4aba5f792340833cd
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 0%

---

# Meerdere gebruikerstoewijzingen in een takenlijst wijzigen

<!--Audited: 11/2025-->

<!--remove the old/new experience references when the toggles are removed-->

<!--
this article is similar and updates on this one might need to be repeated here: help/quicksilver/manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Second Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md).  

</div>-->

Wanneer het beheren van taaktaken, kunt u hen voor veelvoudige taken tegelijkertijd wijzigen door de bulkbewerkingseigenschap in een lijst van taken te gebruiken.

In dit artikel wordt verwezen naar het wijzigen van meerdere gebruikerstoewijzingen voor meerdere taken in een takenlijst. Zie ook de volgende artikelen voor het wijzigen van toewijzingen voor meerdere taken op andere gebieden:

* Voor informatie over het toewijzen van taken die de Balancer van de Werklast gebruiken, zie [&#x200B; Overzicht van het toewijzen van het werk in de Balancer van de Werkbelasting &#x200B;](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Voor informatie over het toewijzen van een taak aan één middel in een lijst, zie [&#x200B; taken toewijzen &#x200B;](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

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
   <td>Contribute of hoger machtigingen voor de taken</td>
  </tr>
 </tbody>
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on tasks</h2>
<p>(NOTE: moved to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>You might want to modify the user assignments for multiple tasks for a variety of reasons, including the following:</p>
<ul>
<li>Users join or leave your team</li>
<li> <p>A user takes a vacation that extends beyond task due dates</p> <note type="note">
When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li>A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
<p><strong>How removing assignees affects task hours and allocation percentages</strong></p>
<p>(NOTE: move to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration Types:</p>
<ul>
<li> <p><strong>Simple:</strong> The planned hours assigned to that user are subtracted from the task's total planned hours.</p> <note type="important">
<span class="s1">This could negatively affect your project plan because it changes the total planned hours for the task and the project.</span>
</note> </li>
<li><span class="s1"><strong>Effort Driven:</strong> The allocation percentage does not change for other users.</span> </li>
<li><span class="s1"><strong>Calculated Assignment:</strong> The allocation percentages of other users are adjusted so that the total equals 100%.</span> </li>
<li><span class="s1"><strong>Calculated Work:</strong> The allocation percentage does not change for other users.</span> </li>
</ul>
</div>
-->

## Toewijzingen wijzigen voor meerdere taken

1. Ga naar de lijst die de taken bevat waar u taken wilt wijzigen.
1. (Optioneel) Maak een filter om alleen taken weer te geven die zijn toegewezen aan de ontvanger die u wilt wijzigen.

   Bijvoorbeeld, als uw project een specifieke rol als standaardontvanger voor veelvoudige taken bevat, kunt u een filter tot stand brengen om slechts taken met die rol als toegewezen te tonen. Vervolgens kunt u de rol vervangen door een specifieke gebruiker.

   Voor informatie over het creëren van een filter, zie [&#x200B; filters &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md) creëren of uitgeven.


1. Om op een rol te filtreren, uitgezochte **Rollen van de Taak**, dan klik **identiteitskaart**.

   >[!TIP]
   >
   >Gebruik niet **Toegewezen aan** gebied. Dit vindt slechts de Primaire Eigenaar voor de taak in plaats van om het even welke rollen die aan hen konden worden toegewezen.

   of

   Om voor een gebruiker te filtreren, uitgezochte **Gebruikers van de Taak,** dan klik **identiteitskaart.**

   >[!TIP]
   >
   >Gebruik niet **Toegewezen aan** gebied. Hiermee vindt u alleen de primaire eigenaar voor de taak in plaats van de gebruikers die aan hen kunnen worden toegewezen.

1. Selecteer de taken waarvoor u taken wilt wijzigen, dan **uitgeven** pictogram ![&#x200B; uitgeven pictogram &#x200B;](assets/edit-icon.png).

   1. Voer een van de volgende handelingen uit om toewijzingen toe te voegen of te verwijderen:

      * Om toegewezen toe te voegen, begin het typen van de naam van een toegewezen op het **mensen van het Onderzoek, de rollen, of het gebied van teams**, dan selecteren hen wanneer zij in de lijst tonen.

        De nieuwe toegewezen persoon wordt toegevoegd aan de bestaande taken in de geselecteerde taken.
      * Om toegewezen te verwijderen, klik de naam van een toegewezen in **verwijder toegewezen persoon** doos

        of

        Klik **verwijderen alle bestaande wijzen**.

        Toewijzingen worden verwijderd uit alle geselecteerde taken.

        Het verwijderen van gebruikers uit taken kan taakuren en toewijzingspercentages beïnvloeden.

        Voor meer informatie, zie [&#x200B; Overzicht van het wijzigen van taaktaken &#x200B;](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).


        >[!TIP]
        >
        >* U kunt meerdere gebruikers, taakrollen of teams toewijzen. U kunt alleen actieve gebruikers, taakrollen en teams toewijzen.
        >   
        >* Wanneer u een gebruikerstoewijzing toevoegt, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen. Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt. De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Voor informatie, zie [&#x200B; toegang van de Verlening tot gebruikers &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
        > 
        >   Als een gebruiker, een baanrol, of een team werd toegewezen alvorens zij werden gedeactiveerd, blijven zij toegewezen aan het het werkpunt. In dit geval raden we het volgende aan:
        >   
        >* Wijs het werkitem opnieuw toe aan actieve bronnen.
        >* Koppel de gebruikers in een gedeactiveerd team aan een actief team en wijs het het werkpunt aan het actieve team opnieuw toe.


   1. (Optioneel) Wijzig een of meer van de volgende opties voor toewijzingen:

      * (Voorwaardelijk) **toewijzing % of Uren**: specificeer een nieuw toewijzingspercentage of uren.

      >[!NOTE]
      >
      >Deze optie kan slechts worden gewijzigd als het Type van Duur het zelfde over alle taken is die worden uitgegeven. Wanneer het Type van Duur het Getoonde Werk of de Bediende van de inspanning wordt berekend kunt u de Toewijzing % bijwerken. Wanneer het Type van Duur Eenvoudig is kunt u de Uren bijwerken. Voor informatie over het Type van Duur, zie [&#x200B; Overzicht van het Type van Duur en van de Duur van de Taak &#x200B;](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
      >
      >
      >Als het veld leeg is, betekent dit dat de waarde voor alle taken anders is. U kunt de waarde echter wel wijzigen.

      * **maak Primair**: Beweeg over de geselecteerde taken en selecteer deze optie om de toegewezen eigenaar van de taak voor alle taken te maken die worden uitgegeven.
      * **Rol van de Ontvanger**: Selecteer een rol van de drop-down lijst. Als deze optie niet is geselecteerd, selecteert Adobe Workfront automatisch de primaire rol van de gebruiker.
      * **Type van Duur**
      * **Duur**
      * **Geplande Uren**

   1. Klik **sparen**.

<!-- temporary content - for Assignments redesign:

Editing assignments on tasks differs depending on which environment you choose. 

1. (Conditional) If you are using the Production environment to assign tasks, the **Edit Tasks** box opens in the new experience. Do the following in the Production environment: 

   1. To add or remove assignees, do one of the following:

      * To add assignees, start typing the name of an assignee in the **Search people, roles, or teams** field, then select them when they display in the list. 
      * To remove assignees, click the **x** icon to the right of their name. Only assignees that are common to all tasks display in the list. 
      * Click Assign to me to assign the selected tasks to yourself.

   1. (Conditional) When using the new experience, click **Save**.

   1. (Optional) Click **Switch to old experience** at the bottom of the **Edit Tasks** box.
      
      The **Edit Tasks** box opens in the old experience.

   1. (Conditional) In the old experience, do the following to modify the assignees:

      1. Go to the **Assignments** section.

         >[!IMPORTANT]
         >
         >Removing assignees can affect the task hours and allocation percentages. For more information, see the section [How removing assignees affects task hours and allocation percentages](#how-removing-assignees-affects-task-hours-and-allocation-percentages) in this article.

      1. Do one of the following to add or remove assignees:

         * To add a new assignee:

            1. In the **Assignments** section, select **Assignee**.

               Information that is common across all tasks selected displays. For example, if the same user is assigned to all tasks, that user displays in the **Assignee** column. If information is not common across the tasks selected, no information displays.
            
            1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected tasks.

            >[!TIP]
            >
            > * You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
            >   
            > * When adding a user assignment, notice the avatar, the user's Primary Role, or their email address to distinguish between users with identical names. Users must be associated with at least one job role to view it as you add them. You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
            > 
            >   If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
            >   
            >     * Reassign the work item to active resources.
            >     * Associate the users in a deactivated team with an active team and reassign the work item to the active team.


         * To remove individual assignees:

            1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.

               Or

               (Conditional) If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the tasks that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.

         * To remove all existing assignees:

            1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.

               This removes not only common assignees (assignees that are displayed in the edit dialog box), but also all assignees on all the selected tasks.

            Removing users from tasks can affect task hours and allocation percentages.
            
            For more information, see [Overview of modifying task assignments](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

      1. (Optional) Modify any of the following options for assignees:

         * (Conditional) **Allocation % or Hours**: Specify a new allocation percentage or hours.

         >[!NOTE]
         >
         >This option can be modified only if the Duration Type is the same across all tasks that are being edited. When the Duration Type is Calculated Work or Effort Driven you can update the Allocation %. When the Duration Type is Simple you can update the Hours. For information about Duration Type, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
         >
         >
         >If the field is blank, this means that the value is different across tasks; however, you are still able to modify it.

         * **Task Owner**: Select this option to make the assignee the owner of the task for all tasks being edited.
         * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Adobe Workfront automatically selects the Primary Role of the user. 

      1. Click **Save Changes.**
        

1. <span class="preview">(Conditional) If you are using the Preview environment to assign tasks, the **Edit Tasks** box opens. Do the following in the Preview environment: </span>

   <div class="preview">-->





