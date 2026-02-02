---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Overzicht van slimme toewijzingen
description: Bij het beheren van taken en uitgaven kunt u slimme toewijzingen gebruiken om te bepalen wie de beste gebruiker het werk moet voltooien. De slimme taken zijn suggesties die Adobe Workfront aan u voorstelt wanneer u het werkpunten aan middelen toewijst die op een algoritme worden gebaseerd dat het meest aangewezen middel voor de baan bepaalt.
author: Lisa
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Overzicht van slimme toewijzingen

<!--Audited: 07/2024-->

Bij het beheren van taken en uitgaven kunt u slimme toewijzingen gebruiken om te bepalen wie de beste bron is om het werk te voltooien.

De slimme taken zijn suggesties die Adobe Workfront aan u voorstelt wanneer u het werkpunten aan middelen toewijst die op een algoritme worden gebaseerd dat het meest aangewezen middel voor de baan bepaalt. De slimme taken kunnen gebruikers, baanrollen, of teams zijn.

>[!NOTE]
>
>Bij het voorstellen van gebruikers houden slimme toewijzingen geen rekening met de beschikbaarheid van de gebruiker. De beschikbaarheid volgens de planning is echter van invloed op de geplande en verwachte datum van taken en problemen wanneer deze worden toegewezen. Voor informatie over programma&#39;s, zie het artikel [&#x200B; een programma &#x200B;](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

Dit artikel bevat algemene informatie over slimme toewijzingen. Voor informatie over het gebruiken van slimme taken om taken en kwesties aan gebruikers toe te wijzen, zie [&#x200B; Slimme taken &#x200B;](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md) maken.

## Overzicht van slimme toewijzingen

Houd rekening met het volgende wanneer u werkt met slimme toewijzingen:

<!--* <span class="preview">The algorithm works independently for tasks and issues. This means that the list of suggested users for issues might differ from the list of suggested users for a task because Workfront builds the lists according to criteria pertaining to issues and tasks separately. </span>-->
<!--not sure this is accurate: * Smart assignments do not recommend job roles or teams. Instead, they are suggestions of users who are best fit to complete a task or an issue. -->
* De voorgestelde taken zijn altijd actieve gebruikers, baanrollen, of teams.
* De bron die eerst wordt vermeld zou de beste gelijke voor de taak moeten zijn.

## Suggesties voor slimme toewijzingen zoeken

U kunt slimme toewijzingen weergeven op de volgende plaatsen waar u taken of problemen kunt toewijzen:

* Een uitgiftenlijst of rapport in de kolom Toewijzingen

  ![&#x200B; de kolom van de Lijsten van de Uitgave &#x200B;](assets/smart-assignments-issue-list.png)

* Een taaklijst of rapport in de kolom van Taken

  ![&#x200B; de kolom van Toewijzingen van de Lijst van de Taak &#x200B;](assets/smart-assignments-task-list.png)

* Een taakkoptekst in het veld Toewijzingen

  ![&#x200B; het gebied van Toewijzingen van de kopbal van de Taak &#x200B;](assets/smart-assignments-task-header-nwe-350x302.png)

* Een uitgiftekop in het veld Toewijzingen

  ![&#x200B; het gebied van de kopbalToewijzingen van de Uitgave &#x200B;](assets/smart-assignments-issue-header.png)

* Het deelvenster Overzicht van taken of uitgaven in het gebied Toewijzingen

  ![&#x200B; het gebied van de Kaarten van het Summiere paneel &#x200B;](assets/issue-assignments-summary-panel.png)

<!--* The Assignments field in the New Task box, when adding a task to a project

  (![Smart assignments new task]assets/smart-assignments-new-task-modal.png)-->

<!--this is not possible in the new home  - we have Summary there: 
* The Assignments field for an item listed in the Home area, when you open a task or issue

  ![Smart assignments in Home](assets/smart-assignments-in-home-nwe-350x216.png)
-->

* Werklastverdeling in het gedeelte Toegewezen aan als u een taak of uitgave toewijst

  ![&#x200B; het gebied van de Toewijzingen van de Balans van de Werkbelasting &#x200B;](assets/smart-assignments-workload-balancer-bulk-assignments.png)

## Criteria voor slimme toewijzingen

<!--Smart assignments work differently for tasks than for issues.  -->

<!--### Smart assignments criteria for tasks

The task smart assignments calculation works in <span class="preview">two phases which use two different algorithms.</span>

<span class="preview">Depending on which algorithm finds the smart assignment, the assignments are listed under two separate sections in the Assignments field.</span> For information, see [Make smart assignments](/help/quicksilver/manage-work/tasks/assign-tasks/make-smart-assignments.md). 

![Smart assignments in tasks list](assets/smart-assignments-task-list.png)

<div class="preview">

#### First phase of smart assignment calculation for tasks 

In the first phase of calculating smart assignments, Workfront calculates a similarity score for every assignment. 

>[!NOTE]
>
>The first phase of the smart assignments calculation does not apply to the following task areas:
>
>* Bulk Assignments in the Workload Balancer.
>* Connected cards on boards.


The calculation for the similarity score and the order in which the assignments are listed take into account the following:  

* A score of 100% is given to an existing assignment where the task, project, and portfolio names are identical to the task you're trying to assign. The project and portfolio names of the task of an existing assignment must also match the project and portfolio of the task you are trying to assign.   

* If only some of this information from other assignments matches on the existing tasks, the score might be lower than 100%.  

  For example, if you are assigning a task called "My second task" on a project called "My project" in a portfolio called "My portfolio" and you have an existing task called "My task" in another project called "My project" in a portfolio called "My portfolio", the user assigned to "My task" might get a score of 95% because the name of the existing task and the task you're trying to assign now are similar, but not identical.  
 
    >[!TIP]
    >
    >  Workfront looks for matches only in the Name fields of tasks, projects, and portfolios and not in any other fields. 

* An assignment could get a higher score when they are assigned to a lot of tasks in the system that have similar names. For example, if a team called "Development" is assigned to 50% of the tasks in the system containing "AI" in the name and you are now assigning another task with "AI" in the name, the score of the "Development" team is higher. In this case, the names of  projects and portfolios are not as important.  

* Taking into account this scoring system, the first 7 suggestions are listed as smart assignments, in the descending order of their scores. Assignments with scores lower than 40% do not display.  

* If several assignments have identical scores, they display in order of the date on which the assignments were made, starting from the most recent date.  

  For example, if Rick was assigned to a similar task earlier today and Jennifer was assigned to a similar task two days ago, Rick displays first.  

* Assignments identified in this phase are listed in the    **Suggested assignments**  section of the Assignments field for tasks. 

* If there are no matches using this calculation, the second phase of smart assignments starts which is calculated using a different algorithm.  

</div>

#### Second phase of smart assignment calculation for tasks-->

<!--If the first step of task smart assignments has found no matches,-->

Workfront berekent slimme toewijzingen voor taken op dezelfde manier als voor uitgaven.

<!--For more information, see the section [Smart assignments criteria for tasks and issues](#smart-assignments-criteria-for-tasks-and-issues) in this article. -->

De geïdentificeerde taken worden vermeld in de **Gebruikers en teams** en **de rollen van de Baan**<!--, and <span class="preview">**Rate card roles**</span>--> secties van het gebied van Taken. <!--<span class="preview">For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)</span>. keep the rate cards roles in yellow after the release of assignments to Prod-->

<!--
### Smart assignments criteria for tasks and issues 

>[!NOTE]
>
>The following criteria applies for tasks only when the first phase of the task smart assignment calculation did not find any matches. For information, see the section [First phase of smart assignment calculation for tasks](#first-phase-of-smart-assignment-calculation-for-tasks) in this article. The following criteria always applies for issues, by default. -->

![&#x200B; Slimme taak van het Voorbeeld &#x200B;](assets/smart-assignments-issue-header.png)

De gebruikers worden geadviseerd in de slimme drop-down lijst van Toewijzingen die op een combinatie van de volgende criteria (die in orde van belangrijkst tot minst belangrijk worden vermeld) wordt gebaseerd:

1. Gebruikers die in de afgelopen 30 dagen aan andere werkitems zijn toegewezen door de gebruiker die de toewijzing maakt. De eerste 50 gebruikers die aan deze criteria voldoen, worden weergegeven. De gebruiker die het vaakst wordt toegewezen toont eerst.

2. Als het het werkpunt aan een team of een rol wordt toegewezen, wordt de lijst van voorgestelde gebruikers gefiltreerd verder rekening houdend met de bestaande taken hieronder. In dit geval worden alleen de volgende gebruikers weergegeven in de lijst met suggesties:

   * Gebruikers van wie het Team van het Huis het team is dat aan het het werkpunt wordt toegewezen.
   * Gebruikers waarvan de primaire rol de rol is die aan het werkitem is toegewezen.

>[!TIP]
>
>* Als er geen rol of team aan de taak of kwestie wordt toegewezen, toont Workfront alle gebruikers die voor de laatste 30 dagen, tot 50 gebruikers worden toegewezen.
>
>* Als u geen taken in de afgelopen 30 dagen hebt gemaakt, slechts gebruikers die tot of het toegewezen team behoren of de rol hebben die aan het het werkpunt wordt toegewezen tonen in de slimme lijst van taken.



<!--the commented out piece in the tip above was live before but I am not totally sure that smart assignments look at your team. I think they look JUST at the team/ role assigned to the work item; see this help site request for more info: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/62fd222200037eb87572c5b6ad6bf53e/overview -->
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h3>Smart assignments criteria for the Production environment</h3>
<p>(NOTE: drafted,this was the case BEFORE we updated the logic in the WB - with the 21.4 release)</p>
</div>
<p>Smart assignments display on tasks and issues when the following conditions are met:</p>
<ul>
<li>The task or issue is subordinate to a parent task or issue that has a user, team, or job role currently assigned. </li>
</ul>
<p>Smart assignments display the top twenty recommendations based on a proprietary algorithm that uses your own team information.</p>
<p>Users are recommended in the smart assignments drop-down list based on a combination of the following criteria (listed in order from most important to least important):</p>
<ul>
<li>The user has the team assigned to the task or issue designated as their Home Team</li>
<li>The user is also assigned to the parent task</li>
<li>The user has the same primary job role as is currently assigned to the task or issue</li>
<li>The user has the team assigned to the parent task or issue designated as their Home Team</li>
<li>The user is associated with the same primary job role currently assigned to the parent task</li>
<li>The user is a member of the same team as the user who assigned the task or issue and the team is designated as their Home Team</li>
<li>The user is a member of the same Home Group as the user who is assigning the task or issue</li>
<li>The user has the same primary job role as the user who is assigning the task or issue.</li>
</ul>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Make smart assignments</h2>
<p>(NOTE: this was moved to its own article: make-smart-assignments.) </p>
<p>Smart assignments are available in most locations where you can make assignments in Workfront.</p>
<p>You can use smart assignments on tasks and issues that have previously been assigned to a job role or a team.</p> <note type="note">
You must have a Plan or a Work license and have at least Contribute permissions to a task or an issue to be able to make assignments to the task or the issue. You must have the Make Assignments option enabled in your permission level to make assignments.
</note>
<p>To use smart assignments:</p>
<ol>
<li value="1">Navigate to an issue or a task and click one of the following fields to edit them: <br>
<ul>
<li><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The <strong>Assignments</strong> field in the task or issue header</p></li>
<li>The <strong>Assignments</strong> field of a task or issue list using in-line editing in a task or issue list. </li>
<li>The <strong>Assignee</strong> field after you have clicked <strong>Advanced</strong> from a task or an issue. </li>
</ul></li>
<li value="2"> <p>Place your cursor in the assignment field, and wait for two seconds, then the <strong>Suggestions</strong> list is displayed.</p> <p>Users displayed in this list are the smart assignment suggestions for the task or the issue.<br></p> <p> <img src="assets/nwe-smart-assignment-suggestions-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p>Select the user in the recommendations list by clicking their name. </p> <p>If there are no suggestions, the suggestion list does not open.</p> </li>
<li value="4">(Optional) If you do not want to use one of the recommended users from the smart assignments list, start typing the name of the desired user and select the name when it appears in the list.</li>
<li value="5">Click <strong>Enter</strong> to make the assignment. </li>
</ol>
</div>
-->
