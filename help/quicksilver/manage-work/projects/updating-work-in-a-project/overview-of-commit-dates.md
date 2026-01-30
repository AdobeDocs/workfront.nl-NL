---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: Datumoverzicht vastleggen
description: De datum van het Vastleggen is de datum een gebruiker aan taak of een kwestie toezegt om de taak of de kwestie te voltooien. Dit is anders dan de geplande voltooiingsdatum, omdat het een realistischere schatting is van de voltooiingsdatum die wordt gegeven door de gebruiker die rechtstreeks met het werk is belast.
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# Overzicht van datum vastleggen

<!--Audited: 05/2025-->

<!-- <span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

De datum van het Vastleggen is de datum een gebruiker aan taak of een kwestie toezegt om de taak of de kwestie te voltooien. Dit verschilt van de geplande afsluitende datum van een taak of kwestie aangezien het een realistischere schatting van de afwerkingsdatum is die slechts door de gebruiker wordt gegeven die het werk leidt.

Voor informatie over de Geplande Datum van de Voltooiing, zie [&#x200B; Overzicht van de taak Geplande Datum van de Voltooiing &#x200B;](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

## Overzicht van datum vastleggen

Houd rekening met het volgende wanneer u werkt met datums toewijzen:

* Alleen taken en problemen hebben een datum vastleggen.
* Datums vastleggen worden niet automatisch ingesteld door Adobe Workfront. Wanneer u een taak of een kwestie creeert, is er geen datum die aan het wordt toegewezen.
* Als u aan een taak of een kwestie wordt toegewezen, kunt u de Vastlegdatum plaatsen door één van het volgende te doen:

   * Laat Workfront de Vastlegdatum plaatsen om de bestaande Geplande Datum van Voltooiing van de taak of de kwestie te passen door het Werk aan het, Uitgave van het Begin, of Taak van het Begin op de taak of de kwestie te klikken. Voor informatie, zie [&#x200B; het Werk op het knoop met een knoop van het Begin vervangen &#x200B;](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * Stel handmatig de datum voor vastleggen in op basis van het tijdstip waarop de taak of het probleem wordt voltooid. Dit is uw schatting en uw verplichting, als toegewezen, aan de Projectleider dat u de taak of de kwestie tegen een bepaalde datum zult hebben voltooid. Voor informatie, zie [&#x200B; Update Commit Dates op taken en kwesties &#x200B;](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

>[!NOTE]
>
>U moet de Taakeigenaar van een taak zijn om de Vastlegdatum te veranderen. De volgende gebruikers kunnen de Datum van het Vastleggen van een taak niet veranderen:
>
>* Projecteigenaar
>* Projectsponsor
>* Resource Manager
>* Systeembeheerder
>* Elke andere aangewezen persoon
>* Een andere gebruiker met machtigingen voor de taak
>
>Voor meer informatie over de Eigenaar van de Taak, zie [&#x200B; taken &#x200B;](../../../manage-work/tasks/manage-tasks/edit-tasks.md) uitgeven.

## De datum van vastleggen van taken en problemen zoeken

U kunt de Vastlegdatum van taken en kwesties op de volgende gebieden van Workfront vinden:

* De pagina Details
* Het deelvenster Samenvatting nadat een Workfront- of groepsbeheerder het heeft toegevoegd aan uw lay-outsjabloon. Voor informatie, zie [&#x200B; het Summiere paneel aanpassen gebruikend een lay-outmalplaatje &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).
* De kopbal van een taak of kwestie nadat een Workfront of groepsbeheerder het aan uw lay-outmalplaatje toevoegt. Voor informatie, zie [&#x200B; objecten kopballen aanpassen gebruikend een lay-outmalplaatje &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Meldingen en updates die worden geactiveerd door het wijzigen van de Vastlegdatum {#notifications-and-updates-triggered-by-changing-the-commit-date}

Wanneer een taak of een uitgave wordt toegewezen manueel een Datum van het Vastleggen in een datum verandert die verschillend is dan de Geplande Datum van de Voltooiing die door de Eigenaar van het Project wordt geplaatst, zijn er een aantal berichten en updates die de Eigenaar van het Project en andere gebruikers van deze verandering waarschuwen.

>[!NOTE]
>
>Wijzigingen in de datum vastleggen veranderen niet automatisch de geplande datums en wijzigingen in de geplande datums veranderen niet automatisch de datum vastleggen.

Als u de datum vastleggen voor een taak of uitgave handmatig instelt, worden de volgende wijzigingen doorgevoerd:

* De verandering van de Datum van het Vastleggen bevolkt in de Activiteit van het Systeem en de Alle lusjes van de sectie van de Update van de taak of de kwestie.

  ![&#x200B; verbind het bericht van de datumverandering &#x200B;](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)

  De verandering van de Datum van het Vastleggen toont in het gebied van Updates van de taak of de kwestie wanneer de beheerder van Workfront deze update in het gebied van de Eigendommen van Updates in Opstelling toelaat. Voor informatie, zie [&#x200B; systeem-geleide updates &#x200B;](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

  Als een projecteigenaar de wijziging niet wil accepteren, raden we hem aan om een opmerking terug te sturen naar de gebruiker die een nieuwe datum voorstelt via het tabblad Opmerkingen in de sectie Updates. Vraag hem of haar om de datum vastleggen te wijzigen in de oorspronkelijk geplande datum of een nieuwe datum te selecteren.

  Als een eigenaar van het project de wijziging accepteert, kunnen de geplande voltooiingsdatum handmatig worden aangepast aan de vastlegdatum die wordt aangeboden door de gebruiker die aan het item is toegewezen door de taak of uitgave te bewerken.

  U moet toegang hebben om de taak of de uitgave te beheren om hen uit te geven.

  >[!TIP]
  >
  >U kunt het systeem of de groepsbeheerder vragen om het veld Datum vastleggen toe te voegen aan het deelvenster Overzicht of de koptekst, zodat u het bijwerken kunt vereenvoudigen.
  >
  >Raadpleeg de volgende artikelen voor meer informatie:
  >
  >* [&#x200B; Overzicht van de Samenvatting &#x200B;](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
  >* [&#x200B; pas het Summiere paneel aan gebruikend een lay-outmalplaatje &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
  >* [&#x200B; pas objecten kopballen aan gebruikend een lay-outmalplaatje &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)

<!--this is no longer possible: 
>[!NOTE]
>
>If you want to see how the timeline of the project is affected by accepting to change the Planned Completion Date of the task, click **Project Timeline**. This opens the task list where you can evaluate the date changes and the project timeline.
>
>
>![Project owner notification update stream about commit date change](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >
>
-->


* De verwachte Voltooiingsdatum van de taak of de kwestie wordt geplaatst aan de zelfde datum omdat de taak nu een nauwkeurigere aanwijzing heeft van wanneer het waarschijnlijk zal worden voltooid.

  Voor meer informatie, zie [&#x200B; Overzicht van de Verwachte Datum van de Voltooiing voor projecten, taken, en kwesties &#x200B;](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

  ![&#x200B; Taak geprojecteerde voltooiingsdatum in benadrukte details &#x200B;](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* De eigenaar van het project wordt in het gebied Meldingen op de hoogte gesteld van het feit dat een taak of uitgifte Vastlegdatum is gewijzigd.

  ![&#x200B; verbind het bericht van de datumverandering &#x200B;](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

  >[!TIP]
  >
  >Het bericht dat de Datum van het Vastleggen is veranderd wordt verzonden naar de Eigenaar van het Project slechts wanneer de beheerder van Workfront het tonen van de Datum van het Vastleggen in het gebied van de Eigendommen van Updates in Opstelling toelaat. Voor informatie, zie [&#x200B; systeem-geleide updates &#x200B;](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

Voor informatie over de extra functionaliteit die wanneer het bijwerken van een het werkpunt beschikbaar is, zie [&#x200B; het werk van de Update &#x200B;](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Voor informatie over het bijwerken verbind Datums voor taken en kwesties, zie [&#x200B; Update Commit Data op taken en kwesties &#x200B;](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update Commit Dates on tasks and issues</h2>
<p>(NOTE: moved to its own article) </p>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <strong>Task Owner</strong>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click Work on it in the task or issue header</p> <p>Or</p> <p>Click <strong>Start Task</strong> or <strong>Start Issue</strong> if the Work on it button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <strong>Undo</strong> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <strong>This will be done by</strong> date picker, and select a new Commit Date.</p>
<div>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>Updates</strong> in the left panel, then click the <strong>Start a new update</strong>><strong>Commit Date</strong></p>
<p>Or</p>
<p>Click <strong>Task Details</strong> or <strong>Issue Details</strong> in the left panel, then double click <strong>Commit Date</strong> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifications-and-updates-triggered-by-changing-the-commit-date" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->
