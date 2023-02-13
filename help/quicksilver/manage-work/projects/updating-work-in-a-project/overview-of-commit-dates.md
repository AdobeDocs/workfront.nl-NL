---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: Overzicht van datum vastleggen
description: De datum van het Vastleggen is de datum waaraan een gebruiker aan taak of een kwestie toezegt om de taak of de kwestie te voltooien. Dit is anders dan de geplande afsluitende datum, aangezien het een realistischere schatting is van de afwerkingsdatum die alleen door de met het werk belaste gebruiker wordt gegeven. Voor informatie over de Geplande Datum van de Voltooiing, zie Overzicht van de taak Geplande Datum van de Voltooiing.
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# Overzicht van datum vastleggen

De datum van het Vastleggen is de datum waaraan een gebruiker aan taak of een kwestie toezegt om de taak of de kwestie te voltooien. Dit is anders dan de geplande afsluitende datum, aangezien het een realistischere schatting is van de afwerkingsdatum die alleen door de met het werk belaste gebruiker wordt gegeven. Voor informatie over de Geplande Datum van Voltooiing, zie [Overzicht van de geplande voltooiing van de taak](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

## Overzicht van datum vastleggen

Houd rekening met het volgende wanneer u werkt met datums toewijzen:

* Alleen taken en problemen hebben een datum vastleggen.
* Datums vastleggen worden niet automatisch ingesteld door Adobe Workfront.\
   Wanneer u een taak of kwestie creeert, is er geen datum die aan de taak of de kwestie wordt toegewezen.
* Als u aan een taak of een kwestie wordt toegewezen, kunt u de Vastlegdatum plaatsen door één van het volgende te doen:

   * Laat Workfront de Vastlegdatum plaatsen om de bestaande Geplande Datum van Voltooiing van de taak of de kwestie te passen door het Werk aan het, Uitgave van het Begin, of Taak van het Begin op de taak of de kwestie te klikken. Voor informatie over het vervangen van het Werk aan het knoop door een knoop van het Begin, zie  [De knop Aan de werkbalk vervangen door de knop Start](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * Stel handmatig de datum voor vastleggen in op basis van het tijdstip waarop de taak of uitgave mogelijk is voltooid. Dit is uw schatting en uw verplichting, als toegewezen, aan de Projectleider dat u de taak of de kwestie tegen een bepaalde datum zult hebben voltooid.

>[!NOTE]
>
>U moet de Taakeigenaar van een taak zijn om de Vastlegdatum te veranderen. De volgende gebruikers kunnen de datum van vastleggen van een taak niet wijzigen:
>
>* Projecteigenaar
>* Projectsponsor
>* Resource Manager
>* Systeembeheerder
>* Elke andere aangewezen persoon
>* Een andere gebruiker met machtigingen voor de taak.
>
>Voor meer informatie over de Eigenaar van de Taak, zie de sectie [Taken bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) in het artikel [Taken bewerken](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Meldingen en updates die worden geactiveerd door het wijzigen van de Vastlegdatum {#notifications-and-updates-triggered-by-changing-the-commit-date}

Wanneer een taak of uitgifteontvanger een Datum selecteert die van het Vastleggen verschilt dan de Geplande Datum van de Voltooiing die door de Eigenaar van het Project wordt geplaatst, zijn er een aantal berichten en updates die de Eigenaar van het Project en andere gebruikers van deze verandering waarschuwen.

>[!NOTE]
>
>Wijzigingen in de datum van vastleggen veranderen niet automatisch de geplande datums en wijzigingen in de geplande datums veranderen niet automatisch de datum van vastleggen. 

Als u de datum Vastleggen voor een taak of uitgave instelt, worden de volgende wijzigingen doorgevoerd:

* De datum van het Vastleggen vult in de Stroom van de Update van de taak of de kwestie.

   ![](assets/update-stream-confirmation-that-commit-date-changed-nwe-350x73.png)

   De verandering van de Vastlegdatum toont op het gebied van Updates van de taak of de kwestie wanneer de beheerder van Workfront deze update in het gebied van de Eisen van Updates in Opstelling toelaat. Zie voor meer informatie [Door het systeem bijgehouden updates](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

* De geplande datum van voltooiing van de taak of uitgifte is op dezelfde datum vastgesteld, omdat de taak nu nauwkeuriger aangeeft wanneer deze waarschijnlijk zal worden voltooid.

   Voor meer informatie over de Geprojecteerde Datum van Voltooiing, zie [Overzicht van de geplande afsluitdatum voor projecten, taken en problemen](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

   ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* De eigenaar van het project wordt op de hoogte gesteld in het berichtgebied en op het tabblad Updates van de taak of deze wijziging van invloed is op de projecttijdlijn.

   ![](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

   >[!TIP]
   Het bericht dat de Datum van het Vastleggen is veranderd wordt verzonden naar de Eigenaar van het Project slechts wanneer de beheerder van Workfront het tonen van de Datum van het Vastleggen in het gebied van de Eigendommen van Updates in Opstelling toelaat. Zie voor meer informatie [Door het systeem bijgehouden updates](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

   Als een projecteigenaar de wijziging niet wil accepteren, raden we de gebruiker aan een nieuwe datum voor te stellen om hem te vragen de datum voor vastleggen te wijzigen in de oorspronkelijk geplande datum of een nieuwe datum te selecteren. Als een projecteigenaar de wijziging accepteert, kunnen deze handmatig de geplande Voltooiingsdatum aanpassen aan de datum van vastleggen die wordt aangeboden door de gebruiker die aan het item is toegewezen.

   De eigenaar van het project kan de datum Vastleggen gebruiken om de geplande voltooiingsdatum opnieuw in te stellen. U doet dit door de Vastgestelde geplande datum aan optie op het lusje van Updates van de taak te selecteren. U moet toegang hebben om de taak en het project te beheren om deze wijziging te accepteren.

   >[!NOTE]
   Als u wilt zien hoe de tijdlijn van het project wordt beïnvloed door het accepteren van het wijzigen van de geplande Voltooiingsdatum van de taak, klikt u op **Tijdlijn project**. Hiermee opent u het Gantt-diagram waarin u de datumwijzigingen kunt beoordelen.
   ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >

Voor informatie over de extra functionaliteit die beschikbaar is wanneer het bijwerken van een het werkpunt, zie  [Werk bijwerken](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

Voor informatie over het bijwerken van Datums voor vastleggen voor taken en problemen raadpleegt u [Datums vastleggen bijwerken voor taken en problemen](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update Commit Dates on tasks and issues</h2>
<p>(NOTE:&nbsp;moved to its own article) </p>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <strong>Task Owner</strong>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click Work on it in the task or issue header</p> <p>Or</p> <p>Click <strong>Start Task</strong> or <strong>Start Issue</strong> if the Work on it button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <strong>Undo</strong> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On&nbsp;It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <strong>This will be done by</strong> date picker, and select a new Commit Date.</p>
<div>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>Updates</strong> in the left panel, then click the <strong>Start a new update</strong>><strong>Commit Date</strong></p>
<p>Or</p>
<p>Click <strong>Task Details</strong> or <strong>Issue Details</strong> in the left panel, then double click&nbsp;<strong>Commit Date</strong> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifications-and-updates-triggered-by-changing-the-commit-date" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->
