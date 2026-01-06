---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'Overzicht van taakbeperking: moet voltooien op'
description: U kunt gebruiken moet Eindigen op (MFO) de Beperking van de Taak om een taak te plannen om op een specifieke datum te beëindigen.
author: Alina
feature: Work Management
exl-id: 9e546a0f-7f7a-4f1c-9d9d-aa3cea377fdf
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Overzicht van taakbeperking: moet voltooien op

U kunt gebruiken moet Eindigen op (MFO) de Beperking van de Taak om een taak te plannen om op een specifieke datum te beëindigen.

Moet op beperking beëindigen plant een taak precies in de tijd en de datum te beëindigen u op het **Geplande gebied van de Datum van de Voltooiing** specificeert.

>[!TIP]
>
>Als u de geplande voltooiingsdatum van een taak handmatig bijwerkt, wordt de beperking van de taak gewijzigd in Moet voltooid op.

## Overzicht van de must Finish on Task Restriction

Overweeg het volgende wanneer het plannen van een taak met moet op beperking eindigen:

* De vorige verhoudingen dwingen niet de taak om worden opnieuw gepland. Adobe Workfront negeert in wezen de eerdere relaties.
* De taak toont als **bij Risico** als predecessors beginnen achterna te lopen of te laat zijn.

* Wanneer u een taak met een MFO beperking aan een ander project beweegt of kopieert, zou de beperking van de taak of de data van het project afhankelijk van kunnen veranderen wat de beperkingsdata zijn en wat de Datums van het Begin en van de Voltooiing van het project zijn. De volgende scenario&#39;s bestaan:

   * Wanneer het bestemmingsproject van Begin wordt gepland:

      * Wanneer de beperkingsdatum van de taak vroeger is dan de geplande begindatum van het project, verandert de taakbeperking in zo snel mogelijk.
      * Wanneer de beperkingsdatum van de taak later is dan de geplande de VoltooiingsDatum van het project, verandert de geplande Datum van de Voltooiing van het project om de voltooiingsbeperkingsdatum van de taak aan te passen.

      * Wanneer het bestemmingsproject van Voltooiing wordt gepland:

         * Wanneer de beperkingsdatum van de taak later is dan de Datum van de Voltooiing van het Project, verandert de taakbeperking in zo laat mogelijk.
         * Wanneer de beperkingsdatum van de taak vroeger is dan de Geplande Datum van het Begin van het project, verandert de Geplande Datum van het Begin van het project om de beginbeperkingsdatum van de taak aan te passen.

      * Ongeacht het programma van het project, wanneer de beperkingsdatum van de taak binnen de Datums van het Begin en van de Voltooiing van het project is, zijn er geen veranderingen in de Beperking van de Taak of de projectdata.

  Voor informatie over het bewegen van taken, zie [&#x200B; de taken van de Beweging &#x200B;](../../../manage-work/tasks/manage-tasks/move-tasks.md). Voor informatie over het kopiëren van taken, zie [&#x200B; Kopiëren en dupliceren taken &#x200B;](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

Voor informatie over hoe te om de Restrictie van de Taak op een taak bij te werken, zie [&#x200B; de Restrictie van de Taak van een taak &#x200B;](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md) bijwerken.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Must Finish On Task Constraint</h2>
<p>To update the Task Constraint to Must Finish On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Finish On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete by this date, and no later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
